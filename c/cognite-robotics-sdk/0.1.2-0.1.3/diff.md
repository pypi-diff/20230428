# Comparing `tmp/cognite_robotics_sdk-0.1.2.tar.gz` & `tmp/cognite_robotics_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_robotics_sdk-0.1.2.tar", max compression
+gzip compressed data, was "cognite_robotics_sdk-0.1.3.tar", max compression
```

## Comparing `cognite_robotics_sdk-0.1.2.tar` & `cognite_robotics_sdk-0.1.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      698 2023-04-28 07:37:50.819267 cognite_robotics_sdk-0.1.2/README.md
--rw-r--r--   0        0        0       74 2023-04-28 07:37:50.819267 cognite_robotics_sdk-0.1.2/cognite_robotics/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-28 07:37:50.819267 cognite_robotics_sdk-0.1.2/cognite_robotics/config/config.py
--rw-r--r--   0        0        0      255 2023-04-28 07:37:50.819267 cognite_robotics_sdk-0.1.2/cognite_robotics/data_classes.py
--rw-r--r--   0        0        0       67 2023-04-28 07:37:50.819267 cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-28 07:37:50.819267 cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/data_classes.py
--rw-r--r--   0        0        0    11895 2023-04-28 07:37:50.819267 cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/data_uploader.py
--rw-r--r--   0        0        0     1798 2023-04-28 07:37:50.819267 cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/data_uploader_task.py
--rw-r--r--   0        0        0    11631 2023-04-28 07:37:50.820268 cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/helpers.py
--rw-r--r--   0        0        0     9030 2023-04-28 07:37:50.820268 cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/clients/robot_interface_client.py
--rw-r--r--   0        0        0     1505 2023-04-28 07:37:50.820268 cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/clients/web_interface_client.py
--rw-r--r--   0        0        0       62 2023-04-28 07:37:50.820268 cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/helpers/__init__.py
--rw-r--r--   0        0        0      821 2023-04-28 07:37:50.820268 cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/helpers/bearer_token_auth.py
--rw-r--r--   0        0        0      826 2023-04-28 07:37:50.820268 cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/helpers/channel.py
--rw-r--r--   0        0        0     4846 2023-04-28 07:37:50.820268 cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/helpers/messages.py
--rw-r--r--   0        0        0        0 2023-04-28 07:50:50.607169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-28 07:50:50.609169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/common_pb2.py
--rw-r--r--   0        0        0     1702 2023-04-28 07:50:50.590168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/common_pb2.pyi
--rw-r--r--   0        0        0     2519 2023-04-28 07:50:50.610169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/connectivity_pb2.py
--rw-r--r--   0        0        0     6430 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/connectivity_pb2.pyi
--rw-r--r--   0        0        0     3047 2023-04-28 07:50:50.610169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/control_authority_pb2.py
--rw-r--r--   0        0        0     7303 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/control_authority_pb2.pyi
--rw-r--r--   0        0        0     2302 2023-04-28 07:50:50.610169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/data_pb2.py
--rw-r--r--   0        0        0     4811 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/data_pb2.pyi
--rw-r--r--   0        0        0     3228 2023-04-28 07:50:50.610169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/geometry_pb2.py
--rw-r--r--   0        0        0     8503 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/geometry_pb2.pyi
--rw-r--r--   0        0        0     1444 2023-04-28 07:50:50.610169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/joint_state_pb2.py
--rw-r--r--   0        0        0     1705 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/joint_state_pb2.pyi
--rw-r--r--   0        0        0     2590 2023-04-28 07:50:50.610169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_event_pb2.py
--rw-r--r--   0        0        0     5930 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_event_pb2.pyi
--rw-r--r--   0        0        0     1842 2023-04-28 07:50:50.611169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_log_pb2.py
--rw-r--r--   0        0        0     2460 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_log_pb2.pyi
--rw-r--r--   0        0        0     2384 2023-04-28 07:50:50.611169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_pb2.py
--rw-r--r--   0        0        0     5977 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_pb2.pyi
--rw-r--r--   0        0        0     1461 2023-04-28 07:50:50.611169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/payloads_pb2.py
--rw-r--r--   0        0        0     1805 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/payloads_pb2.pyi
--rw-r--r--   0        0        0     8330 2023-04-28 07:50:50.611169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_control_pb2.py
--rw-r--r--   0        0        0    23660 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_control_pb2.pyi
--rw-r--r--   0        0        0     2549 2023-04-28 07:50:50.611169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_registration_pb2.py
--rw-r--r--   0        0        0     4966 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_registration_pb2.pyi
--rw-r--r--   0        0        0     4899 2023-04-28 07:50:50.611169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_state_pb2.py
--rw-r--r--   0        0        0    12598 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_state_pb2.pyi
--rw-r--r--   0        0        0     4507 2023-04-28 07:50:50.611169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/video_pb2.py
--rw-r--r--   0        0        0    15277 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/video_pb2.pyi
--rw-r--r--   0        0        0     1597 2023-04-28 07:50:50.612169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/web_pb2.py
--rw-r--r--   0        0        0     2003 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/web_pb2.pyi
--rw-r--r--   0        0        0     2845 2023-04-28 07:50:50.612169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/robot_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/robot_interface_pb2.pyi
--rw-r--r--   0        0        0    15062 2023-04-28 07:50:50.612169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
--rw-r--r--   0        0        0     2853 2023-04-28 07:50:50.612169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/web_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-04-28 07:50:50.591168 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/web_interface_pb2.pyi
--rw-r--r--   0        0        0    14820 2023-04-28 07:50:50.612169 cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/web_interface_pb2_grpc.py
--rw-r--r--   0        0        0       60 2023-04-28 07:37:50.822268 cognite_robotics_sdk-0.1.2/cognite_robotics/rest/__init__.py
--rw-r--r--   0        0        0      943 2023-04-28 07:37:50.822268 cognite_robotics_sdk-0.1.2/cognite_robotics/rest/base_model.py
--rw-r--r--   0        0        0       64 2023-04-28 07:37:50.822268 cognite_robotics_sdk-0.1.2/cognite_robotics/rest/client.py
--rw-r--r--   0        0        0    45829 2023-04-28 07:50:52.705309 cognite_robotics_sdk-0.1.2/cognite_robotics/rest/models.py
--rw-r--r--   0        0        0       58 2023-04-28 07:37:50.822268 cognite_robotics_sdk-0.1.2/cognite_robotics/utils/__init__.py
--rw-r--r--   0        0        0      645 2023-04-28 07:37:50.822268 cognite_robotics_sdk-0.1.2/cognite_robotics/utils/env_utils.py
--rw-r--r--   0        0        0     3016 2023-04-28 07:37:50.822268 cognite_robotics_sdk-0.1.2/cognite_robotics/utils/token.py
--rw-r--r--   0        0        0     2766 2023-04-28 07:37:50.822268 cognite_robotics_sdk-0.1.2/cognite_robotics/utils/utils.py
--rw-r--r--   0        0        0     1530 2023-04-28 07:37:50.823268 cognite_robotics_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1243 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0       74 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/__init__.py
+-rw-r--r--   0        0        0     1190 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/config/config.py
+-rw-r--r--   0        0        0      255 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_classes.py
+-rw-r--r--   0        0        0       67 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_classes.py
+-rw-r--r--   0        0        0    11895 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_uploader.py
+-rw-r--r--   0        0        0     1722 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_uploader_task.py
+-rw-r--r--   0        0        0    11631 2023-04-28 08:39:47.575761 cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/helpers.py
+-rw-r--r--   0        0        0     9030 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/clients/robot_interface_client.py
+-rw-r--r--   0        0        0     1505 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/clients/web_interface_client.py
+-rw-r--r--   0        0        0       62 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/bearer_token_auth.py
+-rw-r--r--   0        0        0      826 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/channel.py
+-rw-r--r--   0        0        0    10271 2023-04-28 08:39:47.576761 cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/messages.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:54:05.074480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/__init__.py
+-rw-r--r--   0        0        0     1453 2023-04-28 08:54:05.076480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/common_pb2.py
+-rw-r--r--   0        0        0     1702 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/common_pb2.pyi
+-rw-r--r--   0        0        0     2519 2023-04-28 08:54:05.076480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/connectivity_pb2.py
+-rw-r--r--   0        0        0     6430 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/connectivity_pb2.pyi
+-rw-r--r--   0        0        0     3047 2023-04-28 08:54:05.076480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/control_authority_pb2.py
+-rw-r--r--   0        0        0     7303 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/control_authority_pb2.pyi
+-rw-r--r--   0        0        0     2302 2023-04-28 08:54:05.076480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/data_pb2.py
+-rw-r--r--   0        0        0     4811 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/data_pb2.pyi
+-rw-r--r--   0        0        0     3228 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/geometry_pb2.py
+-rw-r--r--   0        0        0     8503 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/geometry_pb2.pyi
+-rw-r--r--   0        0        0     1444 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/joint_state_pb2.py
+-rw-r--r--   0        0        0     1705 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/joint_state_pb2.pyi
+-rw-r--r--   0        0        0     2590 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_event_pb2.py
+-rw-r--r--   0        0        0     5930 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_event_pb2.pyi
+-rw-r--r--   0        0        0     1842 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_log_pb2.py
+-rw-r--r--   0        0        0     2460 2023-04-28 08:54:05.056479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_log_pb2.pyi
+-rw-r--r--   0        0        0     2384 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_pb2.py
+-rw-r--r--   0        0        0     5977 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_pb2.pyi
+-rw-r--r--   0        0        0     1461 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/payloads_pb2.py
+-rw-r--r--   0        0        0     1805 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/payloads_pb2.pyi
+-rw-r--r--   0        0        0     8330 2023-04-28 08:54:05.077480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_control_pb2.py
+-rw-r--r--   0        0        0    23660 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_control_pb2.pyi
+-rw-r--r--   0        0        0     2549 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_registration_pb2.py
+-rw-r--r--   0        0        0     4966 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_registration_pb2.pyi
+-rw-r--r--   0        0        0     4899 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_state_pb2.py
+-rw-r--r--   0        0        0    12598 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_state_pb2.pyi
+-rw-r--r--   0        0        0     4507 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/video_pb2.py
+-rw-r--r--   0        0        0    15277 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/video_pb2.pyi
+-rw-r--r--   0        0        0     1597 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/web_pb2.py
+-rw-r--r--   0        0        0     2003 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/web_pb2.pyi
+-rw-r--r--   0        0        0     2845 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2.pyi
+-rw-r--r--   0        0        0    15062 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
+-rw-r--r--   0        0        0     2853 2023-04-28 08:54:05.078480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-04-28 08:54:05.057479 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2.pyi
+-rw-r--r--   0        0        0    14820 2023-04-28 08:54:05.079480 cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2_grpc.py
+-rw-r--r--   0        0        0       60 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/rest/__init__.py
+-rw-r--r--   0        0        0      943 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/rest/base_model.py
+-rw-r--r--   0        0        0       64 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/rest/client.py
+-rw-r--r--   0        0        0    45829 2023-04-28 08:54:06.934622 cognite_robotics_sdk-0.1.3/cognite_robotics/rest/models.py
+-rw-r--r--   0        0        0       58 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/utils/__init__.py
+-rw-r--r--   0        0        0      645 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/utils/env_utils.py
+-rw-r--r--   0        0        0     3016 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/utils/token.py
+-rw-r--r--   0        0        0     2766 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/cognite_robotics/utils/utils.py
+-rw-r--r--   0        0        0     1428 2023-04-28 08:39:47.578761 cognite_robotics_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.3/PKG-INFO
```

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/config/config.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/config/config.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/data_classes.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/data_uploader.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_uploader.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/data_uploader_task.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/data_uploader_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from cognite_robotics.grpc.clients.robot_interface_client import CogniteRobotInterfaceClient
 from cognite_robotics.protos.messages import data_pb2
 
 
 async def data_uploader_tasks(
     stop_task_trigger: asyncio.Event,
     robot_interface_client: CogniteRobotInterfaceClient,
-    # robot_status_queue: asyncio.Queue[robot_state_pb2.RobotStateMessage],
     data_set_id: int,
     config: DataUploaderConfig,
 ) -> None:
     """Set up tasks for data uploader."""
     data_upload_event_queue: asyncio.Queue[data_pb2.DataUploadEvent] = asyncio.Queue()
     cognite_client = create_cognite_client(client_name="data_uploader")
```

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/data_uploader/helpers.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/data_uploader/helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/clients/robot_interface_client.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/clients/robot_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/clients/web_interface_client.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/clients/web_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/helpers/bearer_token_auth.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/bearer_token_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/grpc/helpers/channel.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/grpc/helpers/channel.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/common_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/common_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/common_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/connectivity_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/connectivity_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/connectivity_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/connectivity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/control_authority_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/control_authority_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/control_authority_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/control_authority_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/data_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/data_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/data_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/geometry_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/geometry_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/geometry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/joint_state_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/joint_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/joint_state_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/joint_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_event_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_event_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_event_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_log_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_log_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_log_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/mission_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/mission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/payloads_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/payloads_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/payloads_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_control_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_control_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_control_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_registration_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_registration_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_registration_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_registration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_state_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/robot_state_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/robot_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/video_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/video_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/video_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/web_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/web_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/messages/web_pb2.pyi` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/messages/web_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/robot_interface_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/robot_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/robot_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/web_interface_pb2.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/protos/services/web_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/protos/services/web_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/rest/base_model.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/rest/base_model.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/rest/models.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/rest/models.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/utils/env_utils.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/utils/token.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/utils/token.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/cognite_robotics/utils/utils.py` & `cognite_robotics_sdk-0.1.3/cognite_robotics/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.2/pyproject.toml` & `cognite_robotics_sdk-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 [tool.poetry]
-authors = [
-    "Niek Beckers <niek.beckers@cognite.com>",
-    "Sara Vinje Aalbu <sara.aalbu@cognite.com>",
-    "Sollimann <kristoffer.solberg@cognite.com>",
-]
-description = "Cognite Robotics SDK."
+authors = ["Cognite Robotics <robotics-team@cognite.com>"]
+description = "Cognite Robotics SDK"
 name = "cognite-robotics-sdk"
 packages = [
     { include = "cognite_robotics", from = "." },
     { include = "protos", from = "cognite_robotics" },
 ]
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 aiofiles = "23.1.0"
 cognite-sdk = "6.0.1"
 grpcio = "1.54.0"
 protobuf = "4.22.3"
 pydantic = "1.10.7"
```

