# Comparing `tmp/cognite_robotics_sdk-0.1.3.tar.gz` & `tmp/cognite_robotics_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_robotics_sdk-0.1.3.tar", max compression
+gzip compressed data, was "cognite_robotics_sdk-0.1.5.tar", max compression
```

## Comparing `cognite_robotics_sdk-0.1.3.tar` & `cognite_robotics_sdk-0.1.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1243 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/README.md
--rw-r--r--   0        0        0       74 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/config/config.py
--rw-r--r--   0        0        0      255 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_classes.py
--rw-r--r--   0        0        0       67 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_classes.py
--rw-r--r--   0        0        0    11895 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_uploader.py
--rw-r--r--   0        0        0     1722 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_uploader_task.py
--rw-r--r--   0        0        0    11631 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/helpers.py
--rw-r--r--   0        0        0     9030 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/clients/robot_interface_client.py
--rw-r--r--   0        0        0     1505 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/clients/web_interface_client.py
--rw-r--r--   0        0        0       62 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/__init__.py
--rw-r--r--   0        0        0      821 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/bearer_token_auth.py
--rw-r--r--   0        0        0      826 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/channel.py
--rw-r--r--   0        0        0    10271 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/messages.py
--rw-r--r--   0        0        0        0 2023-04-28 08:54:05.074480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-28 08:54:05.076480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/common_pb2.py
--rw-r--r--   0        0        0     1702 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/common_pb2.pyi
--rw-r--r--   0        0        0     2519 2023-04-28 08:54:05.076480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/connectivity_pb2.py
--rw-r--r--   0        0        0     6430 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/connectivity_pb2.pyi
--rw-r--r--   0        0        0     3047 2023-04-28 08:54:05.076480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/control_authority_pb2.py
--rw-r--r--   0        0        0     7303 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/control_authority_pb2.pyi
--rw-r--r--   0        0        0     2302 2023-04-28 08:54:05.076480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/data_pb2.py
--rw-r--r--   0        0        0     4811 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/data_pb2.pyi
--rw-r--r--   0        0        0     3228 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/geometry_pb2.py
--rw-r--r--   0        0        0     8503 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/geometry_pb2.pyi
--rw-r--r--   0        0        0     1444 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/joint_state_pb2.py
--rw-r--r--   0        0        0     1705 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/joint_state_pb2.pyi
--rw-r--r--   0        0        0     2590 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_event_pb2.py
--rw-r--r--   0        0        0     5930 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_event_pb2.pyi
--rw-r--r--   0        0        0     1842 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_log_pb2.py
--rw-r--r--   0        0        0     2460 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_log_pb2.pyi
--rw-r--r--   0        0        0     2384 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_pb2.py
--rw-r--r--   0        0        0     5977 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_pb2.pyi
--rw-r--r--   0        0        0     1461 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/payloads_pb2.py
--rw-r--r--   0        0        0     1805 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/payloads_pb2.pyi
--rw-r--r--   0        0        0     8330 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_control_pb2.py
--rw-r--r--   0        0        0    23660 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_control_pb2.pyi
--rw-r--r--   0        0        0     2549 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_registration_pb2.py
--rw-r--r--   0        0        0     4966 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_registration_pb2.pyi
--rw-r--r--   0        0        0     4899 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_state_pb2.py
--rw-r--r--   0        0        0    12598 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_state_pb2.pyi
--rw-r--r--   0        0        0     4507 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/video_pb2.py
--rw-r--r--   0        0        0    15277 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/video_pb2.pyi
--rw-r--r--   0        0        0     1597 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/web_pb2.py
--rw-r--r--   0        0        0     2003 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/web_pb2.pyi
--rw-r--r--   0        0        0     2845 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2.pyi
--rw-r--r--   0        0        0    15062 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
--rw-r--r--   0        0        0     2853 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2.pyi
--rw-r--r--   0        0        0    14820 2023-04-28 08:54:05.079480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2_grpc.py
--rw-r--r--   0        0        0       60 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/rest/__init__.py
--rw-r--r--   0        0        0      943 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/rest/base_model.py
--rw-r--r--   0        0        0       64 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/rest/client.py
--rw-r--r--   0        0        0    45829 2023-04-28 08:54:06.934622 cognite_robotics_sdk-0.1.3/cognite_robotics/rest/models.py
--rw-r--r--   0        0        0       58 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/utils/__init__.py
--rw-r--r--   0        0        0      645 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/utils/env_utils.py
--rw-r--r--   0        0        0     3016 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/utils/token.py
--rw-r--r--   0        0        0     2766 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/utils/utils.py
--rw-r--r--   0        0        0     1428 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1252 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/README.md
+-rw-r--r--   0        0        0       74 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/__init__.py
+-rw-r--r--   0        0        0     1190 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/config/config.py
+-rw-r--r--   0        0        0      255 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_classes.py
+-rw-r--r--   0        0        0       67 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_classes.py
+-rw-r--r--   0        0        0    11895 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_uploader.py
+-rw-r--r--   0        0        0     1660 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_uploader_task.py
+-rw-r--r--   0        0        0    11648 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/helpers.py
+-rw-r--r--   0        0        0     9030 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/clients/robot_interface_client.py
+-rw-r--r--   0        0        0     1505 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/clients/web_interface_client.py
+-rw-r--r--   0        0        0       62 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/bearer_token_auth.py
+-rw-r--r--   0        0        0      826 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/channel.py
+-rw-r--r--   0        0        0    10275 2023-04-28 12:15:24.575271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/messages.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:29:41.554947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/__init__.py
+-rw-r--r--   0        0        0     1453 2023-04-28 12:29:41.556947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/common_pb2.py
+-rw-r--r--   0        0        0     1702 2023-04-28 12:29:41.535945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/common_pb2.pyi
+-rw-r--r--   0        0        0     2519 2023-04-28 12:29:41.556947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/connectivity_pb2.py
+-rw-r--r--   0        0        0     6430 2023-04-28 12:29:41.535945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/connectivity_pb2.pyi
+-rw-r--r--   0        0        0     3047 2023-04-28 12:29:41.556947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/control_authority_pb2.py
+-rw-r--r--   0        0        0     7303 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/control_authority_pb2.pyi
+-rw-r--r--   0        0        0     2302 2023-04-28 12:29:41.556947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/data_pb2.py
+-rw-r--r--   0        0        0     4811 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/data_pb2.pyi
+-rw-r--r--   0        0        0     3228 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/geometry_pb2.py
+-rw-r--r--   0        0        0     8503 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/geometry_pb2.pyi
+-rw-r--r--   0        0        0     1444 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/joint_state_pb2.py
+-rw-r--r--   0        0        0     1705 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/joint_state_pb2.pyi
+-rw-r--r--   0        0        0     2590 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_event_pb2.py
+-rw-r--r--   0        0        0     5930 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_event_pb2.pyi
+-rw-r--r--   0        0        0     1842 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_log_pb2.py
+-rw-r--r--   0        0        0     2460 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_log_pb2.pyi
+-rw-r--r--   0        0        0     2384 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_pb2.py
+-rw-r--r--   0        0        0     5977 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_pb2.pyi
+-rw-r--r--   0        0        0     1461 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/payloads_pb2.py
+-rw-r--r--   0        0        0     1805 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/payloads_pb2.pyi
+-rw-r--r--   0        0        0     8330 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_control_pb2.py
+-rw-r--r--   0        0        0    23660 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_control_pb2.pyi
+-rw-r--r--   0        0        0     2549 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_registration_pb2.py
+-rw-r--r--   0        0        0     4966 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_registration_pb2.pyi
+-rw-r--r--   0        0        0     4899 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_state_pb2.py
+-rw-r--r--   0        0        0    12598 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_state_pb2.pyi
+-rw-r--r--   0        0        0     4507 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/video_pb2.py
+-rw-r--r--   0        0        0    15277 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/video_pb2.pyi
+-rw-r--r--   0        0        0     1597 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/web_pb2.py
+-rw-r--r--   0        0        0     2003 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/web_pb2.pyi
+-rw-r--r--   0        0        0     2845 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2.pyi
+-rw-r--r--   0        0        0    15062 2023-04-28 12:29:41.559947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
+-rw-r--r--   0        0        0     2853 2023-04-28 12:29:41.559947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2.pyi
+-rw-r--r--   0        0        0    14820 2023-04-28 12:29:41.559947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2_grpc.py
+-rw-r--r--   0        0        0       60 2023-04-28 12:15:24.576271 cognite_robotics_sdk-0.1.5/cognite_robotics/rest/__init__.py
+-rw-r--r--   0        0        0      943 2023-04-28 12:15:24.576271 cognite_robotics_sdk-0.1.5/cognite_robotics/rest/base_model.py
+-rw-r--r--   0        0        0       64 2023-04-28 12:15:24.576271 cognite_robotics_sdk-0.1.5/cognite_robotics/rest/client.py
+-rw-r--r--   0        0        0    45829 2023-04-28 12:29:43.799103 cognite_robotics_sdk-0.1.5/cognite_robotics/rest/models.py
+-rw-r--r--   0        0        0       58 2023-04-28 12:15:24.577271 cognite_robotics_sdk-0.1.5/cognite_robotics/utils/__init__.py
+-rw-r--r--   0        0        0      645 2023-04-28 12:15:24.577271 cognite_robotics_sdk-0.1.5/cognite_robotics/utils/env_utils.py
+-rw-r--r--   0        0        0     3016 2023-04-28 12:15:24.577271 cognite_robotics_sdk-0.1.5/cognite_robotics/utils/token.py
+-rw-r--r--   0        0        0     2766 2023-04-28 12:15:24.577271 cognite_robotics_sdk-0.1.5/cognite_robotics/utils/utils.py
+-rw-r--r--   0        0        0     1452 2023-04-28 12:15:24.578271 cognite_robotics_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.5/PKG-INFO
```

### Comparing `cognite_robotics_sdk-0.1.3/README.md` & `cognite_robotics_sdk-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Cognite Robotics SDK
 
-[![PyPI version](https://badge.fury.io/py/cognite-sdk.svg)](https://pypi.org/project/cognite-robotics-sdk/)
+[![PyPI version](https://badge.fury.io/py/cognite-robotics-sdk.svg)](https://pypi.org/project/cognite-robotics-sdk/)
 [![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
 [![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 This is the Cognite Robotics SDK for Python. It is a Python package that provides a client library for interacting with the Cognite Robotics APIs of Cognite Data Fusions.
 
 ## Installation
```

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/config/config.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/config/config.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_classes.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_uploader.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_uploader.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_uploader_task.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_uploader_task.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 """Main for data uploader."""
 import asyncio
 
-from utils import create_cognite_client
-
 from cognite_robotics.data_uploader.data_classes import DataUploaderConfig
 from cognite_robotics.data_uploader.data_uploader import data_upload_event_message_publisher, data_uploader
 from cognite_robotics.grpc.clients.robot_interface_client import CogniteRobotInterfaceClient
 from cognite_robotics.protos.messages import data_pb2
+from cognite_robotics.utils.utils import create_cognite_client
 
 
 async def data_uploader_tasks(
     stop_task_trigger: asyncio.Event,
     robot_interface_client: CogniteRobotInterfaceClient,
     data_set_id: int,
     config: DataUploaderConfig,
@@ -21,15 +20,14 @@
     cognite_client = create_cognite_client(client_name="data_uploader")
 
     data_uploader_task = asyncio.create_task(
         data_uploader(
             stop_task_trigger=stop_task_trigger,
             data_upload_event_queue=data_upload_event_queue,
             cognite_client=cognite_client,
-            # robot_status_queue: asyncio.Queue[robot_state_pb2.RobotStateMessage],
             data_set_id=data_set_id,
             config=config,
         ),
         name="data_uploader",
     )
 
     data_upload_event_message_publisher_task = asyncio.create_task(
```

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/helpers.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import shutil
 from collections import defaultdict
 from typing import Any, Dict, List, MutableMapping, Optional, Union
 
 import aiofiles
 import aiofiles.os
 import pydantic
-from data_classes import JSONRPCRequest
 
+from cognite_robotics.data_classes import JSONRPCRequest
 from cognite_robotics.data_uploader.data_classes import (
     Datapoint,
     DatapointsUploadRequest,
     DataUploaderConfig,
     FileUploadRequest,
     UploadRequestParseError,
 )
```

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/clients/robot_interface_client.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/clients/robot_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/clients/web_interface_client.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/clients/web_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/bearer_token_auth.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/bearer_token_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/channel.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/channel.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/messages.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 )
 from cognite_robotics.protos.messages.video_pb2 import CameraControls, VideoComposition, VideoConfiguration
 
 #####################
 # RobotRegistration #
 #####################
 
+
 def robot_registration_request(
     robot_name: str,
     robot_description: str,
     robot_type: str,
     robot_capability_external_ids: List[str],
     video_configuration: VideoConfiguration,
     has_estop: bool,
@@ -50,15 +51,15 @@
         RobotRegistrationRequest: RobotRegistrationRequest object
     """
     request = RobotRegistrationRequest(robot_name=robot_name, robot_description=robot_description, robot_type=robot_type)
     request.capabilities.extend(
         [RobotCapability(capability_external_id=capability_external_id) for capability_external_id in robot_capability_external_ids]
     )
     metadata = Metadata(
-        three_d_model="", # TODO: Deprecate this: https://cognitedata.atlassian.net/browse/RS-1133
+        three_d_model="",  # TODO: Deprecate this: https://cognitedata.atlassian.net/browse/RS-1133
         get_estop=has_estop,
         power_on=has_power_on,
     )
     request.video_config.CopyFrom(video_configuration)
     request.metadata.CopyFrom(metadata)
     return request
 
@@ -90,27 +91,29 @@
     )
 
 
 ######################
 # RobotStateMessages #
 ######################
 
-def robot_state_message(timestamp: int, robot_state: RobotState)-> RobotStateMessage:
+
+def robot_state_message(timestamp: int, robot_state: RobotState) -> RobotStateMessage:
     """Create a RobotStateMessage.
 
     Args:
         timestamp (int): Timestamp of the state
         robot_state (RobotState): RobotState object
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     message = RobotStateMessage(ping_sent=timestamp)
     message.robot_state.CopyFrom(robot_state)
     return message
 
+
 def robot_pose_state_message(
     timestamp: int, pos_x: float, pos_y: float, pos_z: float, quat_x: int, quat_y: int, quat_z: int, quat_w: int
 ) -> RobotStateMessage:
     """Create a RobotStateMessage with the robot pose.
 
     Args:
         timestamp (int): Timestamp of the state
@@ -126,93 +129,93 @@
     """
     position = Point(x=pos_x, y=pos_y, z=pos_z)
     orientation = Quaternion(x=quat_x, y=quat_y, z=quat_z, w=quat_w)
     transform = Transform(to=MAP, frm=BODY, translation=position, orientation=orientation)
     robot_state = RobotState(map_transform=transform)
     return robot_state_message(timestamp, robot_state)
 
-def robot_joint_states_state_message(
-    timestamp: int, joint_states: List[JointState]
-) -> RobotStateMessage:
+
+def robot_joint_states_state_message(timestamp: int, joint_states: List[JointState]) -> RobotStateMessage:
     """Create a RobotStateMessage with the joint states.
 
     Args:
         timestamp (int): Timestamp of the state
         joint_states (List[JointState]): List of joint states
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     joint_states_message = JointStates(joint_states=joint_states)
     robot_state = RobotState(joint_states=joint_states_message)
     return robot_state_message(timestamp, robot_state)
 
-def robot_mission_state_message(
-    timestamp: int, mission_state: MissionState.ValueType
-) -> RobotStateMessage:
+
+def robot_mission_state_message(timestamp: int, mission_state: MissionState.ValueType) -> RobotStateMessage:
     """Create a RobotStateMessage with the mission state.
 
     Args:
         timestamp (int): Timestamp of the state
         mission_state (MissionState.ValueType): Mission state of the robot
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     robot_state = RobotState(mission_state=mission_state)
     return robot_state_message(timestamp, robot_state)
 
-def robot_connection_state_message(
-    timestamp: int, connection_state: ConnectionState.ValueType
-) -> RobotStateMessage:
+
+def robot_connection_state_message(timestamp: int, connection_state: ConnectionState.ValueType) -> RobotStateMessage:
     """Create a RobotStateMessage with the connection state.
 
     Args:
         timestamp (int): Timestamp of the state
         connection_state (ConnectionState.ValueType): Connection state of the robot
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     robot_state = RobotState(connection_state=connection_state)
     return robot_state_message(timestamp, robot_state)
 
-def robot_docking_state_message(timestamp:int, docking_state: DockingState.ValueType)-> RobotStateMessage:
+
+def robot_docking_state_message(timestamp: int, docking_state: DockingState.ValueType) -> RobotStateMessage:
     """Create a RobotStateMessage with the docking state.
 
     Args:
         timestamp (int): Timestamp of the state
         docking_state (DockingState): Docking state of the robot
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     robot_state = RobotState(docking_state=docking_state)
     return robot_state_message(timestamp, robot_state)
 
-def robot_power_state_message(timestamp:int, power_state: PowerState.ValueType)-> RobotStateMessage:
+
+def robot_power_state_message(timestamp: int, power_state: PowerState.ValueType) -> RobotStateMessage:
     """Create a RobotStateMessage with the power state.
 
     Args:
         timestamp (int): Timestamp of the state
         power_state (PowerState): Power state of the robot
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     robot_state = RobotState(power_state=power_state)
     return robot_state_message(timestamp, robot_state)
 
-def robot_absolute_ptz_state_message(timestamp: int, pan: float, tilt: float, zoom: float)->RobotStateMessage:
+
+def robot_absolute_ptz_state_message(timestamp: int, pan: float, tilt: float, zoom: float) -> RobotStateMessage:
     """Create a RobotStateMessage with the absolute PTZ state.
 
     Args:
         timestamp (int): Timestamp of the state
         pan (float): Pan of the PTZ camera
         tilt (float): Tilt of the PTZ camera
         zoom (float): Zoom of the PTZ camera
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
-    absolute_ptz=AbsolutePTZ(pan=pan, tilt=tilt, zoom=zoom)
+    absolute_ptz = AbsolutePTZ(pan=pan, tilt=tilt, zoom=zoom)
     robot_state = RobotState(ptz_state=absolute_ptz)
     return robot_state_message(timestamp, robot_state)
 
 
 def robot_battery_percentage_state_message(timestamp: int, battery_percentage: float) -> RobotStateMessage:
     """Create a RobotStateMessage with the battery percentage.
 
@@ -222,43 +225,43 @@
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     robot_state = RobotState(battery_percentage=battery_percentage)
     return robot_state_message(timestamp, robot_state)
 
 
-def robot_log_message_state_message(timestamp: int, message: str, severity: LogSeverity.ValueType)-> RobotStateMessage:
+def robot_log_message_state_message(timestamp: int, message: str, severity: LogSeverity.ValueType) -> RobotStateMessage:
     """Create a RobotStateMessage with the log message.
 
     Args:
         timestamp (int): Timestamp of the state
         message (str): Log message
         severity (LogSeverity.ValueType): Severity of the log message
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     log_message = LogMessage(severity=severity, message=message)
     robot_state = RobotState(log_message=log_message)
     return robot_state_message(timestamp, robot_state)
 
 
-def robot_estop_state_message(timestamp: int, estop_state: EstopState.ValueType)-> RobotStateMessage:
+def robot_estop_state_message(timestamp: int, estop_state: EstopState.ValueType) -> RobotStateMessage:
     """Create a RobotStateMessage with the estop state.
 
     Args:
         timestamp (int): Timestamp of the state
         estop_state (EStopState.ValueType): EStop state of the robot
     Returns:
         RobotStateMessage: RobotStateMessage object
     """
     robot_state = RobotState(estop_state=estop_state)
     return robot_state_message(timestamp, robot_state)
 
 
-def robot_estop_registration_state_message(timestamp: int, estop_registration_state: EstopRegistrationState.ValueType)-> RobotStateMessage:
+def robot_estop_registration_state_message(timestamp: int, estop_registration_state: EstopRegistrationState.ValueType) -> RobotStateMessage:
     """Create a RobotStateMessage with the estop registration state.
 
     Args:
         timestamp (int): Timestamp of the state
         estop_registration_state (EStopRegistrationState.ValueType): EStop registration state of the robot
     Returns:
         RobotStateMessage: RobotStateMessage object
```

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/common_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/common_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/common_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/connectivity_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/connectivity_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/connectivity_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/connectivity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/control_authority_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/control_authority_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/control_authority_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/control_authority_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/data_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/data_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/data_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/geometry_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/geometry_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/geometry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/joint_state_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/joint_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/joint_state_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/joint_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_event_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_event_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_event_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_log_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_log_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_log_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/payloads_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/payloads_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/payloads_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_control_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_control_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_control_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_registration_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_registration_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_registration_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_registration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_state_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_state_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/video_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/video_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/video_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/web_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/web_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/web_pb2.pyi` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/web_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/rest/base_model.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/rest/base_model.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/rest/models.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/rest/models.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/utils/env_utils.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/utils/token.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/utils/token.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/cognite_robotics/utils/utils.py` & `cognite_robotics_sdk-0.1.5/cognite_robotics/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.3/pyproject.toml` & `cognite_robotics_sdk-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Cognite Robotics SDK"
 name = "cognite-robotics-sdk"
 packages = [
     { include = "cognite_robotics", from = "." },
     { include = "protos", from = "cognite_robotics" },
 ]
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 aiofiles = "23.1.0"
 cognite-sdk = "6.0.1"
 grpcio = "1.54.0"
 protobuf = "4.22.3"
 pydantic = "1.10.7"
@@ -50,11 +50,12 @@
 select = ["A", "D", "E", "F", "I", "ICN", "RUF", "S", "T20", "TID", "W"]
 unfixable = []
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 target-version = "py39"
 
 [tool.ruff.per-file-ignores]
+"examples/*" = ["T201"]
 "tests/*" = ["S101", "T201"]
 
 [tool.ruff.isort]
 known-third-party = ["alembic"]
```

### Comparing `cognite_robotics_sdk-0.1.3/PKG-INFO` & `cognite_robotics_sdk-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-robotics-sdk
-Version: 0.1.3
+Version: 0.1.5
 Summary: Cognite Robotics SDK
 Author: Cognite Robotics
 Author-email: robotics-team@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Requires-Dist: protobuf (==4.22.3)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: python-dotenv (==0.21.1)
 Description-Content-Type: text/markdown
 
 # Cognite Robotics SDK
 
-[![PyPI version](https://badge.fury.io/py/cognite-sdk.svg)](https://pypi.org/project/cognite-robotics-sdk/)
+[![PyPI version](https://badge.fury.io/py/cognite-robotics-sdk.svg)](https://pypi.org/project/cognite-robotics-sdk/)
 [![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
 [![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 This is the Cognite Robotics SDK for Python. It is a Python package that provides a client library for interacting with the Cognite Robotics APIs of Cognite Data Fusions.
 
 ## Installation
```

