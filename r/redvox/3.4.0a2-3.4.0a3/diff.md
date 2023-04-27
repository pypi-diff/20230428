# Comparing `tmp/redvox-3.4.0a2.tar.gz` & `tmp/redvox-3.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-3.4.0a2.tar", last modified: Fri Jul  8 00:58:17 2022, max compression
+gzip compressed data, was "redvox-3.4.0a3.tar", last modified: Thu Apr 27 23:37:57 2023, max compression
```

## Comparing `redvox-3.4.0a2.tar` & `redvox-3.4.0a3.tar`

### file list

```diff
@@ -1,156 +1,161 @@
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.016502 redvox-3.4.0a2/
--rw-rw-r--   0 opq       (1000) opq       (1000)      886 2022-07-08 00:58:17.016502 redvox-3.4.0a2/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)      517 2021-06-14 20:37:56.000000 redvox-3.4.0a2/README.md
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.003502 redvox-3.4.0a2/redvox/
--rw-rw-r--   0 opq       (1000) opq       (1000)      730 2022-07-08 00:53:08.000000 redvox-3.4.0a2/redvox/__init__.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.003502 redvox-3.4.0a2/redvox/api1000/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/__init__.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.004502 redvox-3.4.0a2/redvox/api1000/common/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/common/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    20204 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/common/common.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1050 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/common/decorators.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5359 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/common/generic.py
--rw-r--r--   0 opq       (1000) opq       (1000)      875 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/common/lz4.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2570 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/common/mapping.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2237 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/common/metadata.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2435 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/common/typing.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2114 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/errors.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.005502 redvox-3.4.0a2/redvox/api1000/gui/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/gui/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4672 2021-04-14 19:22:20.000000 redvox-3.4.0a2/redvox/api1000/gui/image_viewer.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.005502 redvox-3.4.0a2/redvox/api1000/proto/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/proto/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    39434 2022-07-07 00:07:12.000000 redvox-3.4.0a2/redvox/api1000/proto/redvox_api_m_pb2.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.005502 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5639 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/event_streams.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.006502 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    11949 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.007502 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/derived/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14890 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7398 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/image.py
--rw-r--r--   0 opq       (1000) opq       (1000)    40936 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/location.py
--rw-r--r--   0 opq       (1000) opq       (1000)    42236 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3425 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/single.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5576 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    50437 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/station_information.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19060 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/timing_information.py
--rw-r--r--   0 opq       (1000) opq       (1000)    21971 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.008502 redvox-3.4.0a2/redvox/api900/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    17514 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/concat.py
--rw-r--r--   0 opq       (1000) opq       (1000)      494 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/constants.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1689 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/deprecation.py
--rw-r--r--   0 opq       (1000) opq       (1000)      351 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/exceptions.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.008502 redvox-3.4.0a2/redvox/api900/lib/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/lib/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7591 2022-07-07 00:11:16.000000 redvox-3.4.0a2/redvox/api900/lib/api900_pb2.py
--rw-r--r--   0 opq       (1000) opq       (1000)    43091 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/location_analyzer.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2597 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/migrations.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.008502 redvox-3.4.0a2/redvox/api900/qa/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/qa/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2813 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/qa/gap_detection.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16939 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/reader.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    17096 2021-06-07 23:35:09.000000 redvox-3.4.0a2/redvox/api900/reader_utils.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.010502 redvox-3.4.0a2/redvox/api900/sensors/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2113 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/accelerometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2298 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/barometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2665 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/evenly_sampled_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     6283 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/evenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1989 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/gyroscope_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4854 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/image_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2264 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/infrared_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16540 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/interleaved_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2261 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/light_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10051 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/location_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2022 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/magnetometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3209 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/microphone_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4655 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/time_synchronization_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3536 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/unevenly_sampled_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     6619 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/unevenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5907 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1128 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/stat_utils.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8780 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/summarize.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.010502 redvox-3.4.0a2/redvox/api900/timesync/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/timesync/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    27606 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/timesync/api900_timesync.py
--rw-r--r--   0 opq       (1000) opq       (1000)    13824 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/timesync/tri_message_stats.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1537 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/types.py
--rw-r--r--   0 opq       (1000) opq       (1000)    54392 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/api900/wrapped_redvox_packet.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.010502 redvox-3.4.0a2/redvox/cli/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/cli/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22678 2021-04-14 19:22:20.000000 redvox-3.4.0a2/redvox/cli/cli.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6683 2021-06-07 23:35:09.000000 redvox-3.4.0a2/redvox/cli/conversions.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1797 2021-04-14 19:22:20.000000 redvox-3.4.0a2/redvox/cli/data_req.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.012502 redvox-3.4.0a2/redvox/cloud/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/cloud/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     2267 2021-04-06 18:15:12.000000 redvox-3.4.0a2/redvox/cloud/api.py
--rw-r--r--   0 opq       (1000) opq       (1000)   142063 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/cloud/api_m_fqns.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4334 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/cloud/auth_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    27215 2022-04-20 20:36:13.000000 redvox-3.4.0a2/redvox/cloud/client.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5905 2021-09-16 19:39:56.000000 redvox-3.4.0a2/redvox/cloud/config.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6088 2021-04-14 19:22:20.000000 redvox-3.4.0a2/redvox/cloud/data_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3829 2021-09-16 19:39:56.000000 redvox-3.4.0a2/redvox/cloud/data_client.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3094 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/cloud/data_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)      487 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/cloud/errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18946 2022-04-20 20:36:13.000000 redvox-3.4.0a2/redvox/cloud/metadata_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3770 2021-04-14 23:45:25.000000 redvox-3.4.0a2/redvox/cloud/query_timing_correction.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      902 2022-04-20 20:36:13.000000 redvox-3.4.0a2/redvox/cloud/routes.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4262 2021-04-14 23:45:25.000000 redvox-3.4.0a2/redvox/cloud/station_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     7707 2022-06-01 22:08:00.000000 redvox-3.4.0a2/redvox/cloud/subscription.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.016502 redvox-3.4.0a2/redvox/common/
--rw-r--r--   0 opq       (1000) opq       (1000)      195 2021-03-29 23:26:30.000000 redvox-3.4.0a2/redvox/common/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    55256 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/api_conversions.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    15756 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/api_reader.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5527 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/api_reader_dw.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    12875 2021-06-07 23:35:09.000000 redvox-3.4.0a2/redvox/common/api_reader_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1173 2021-04-20 02:39:13.000000 redvox-3.4.0a2/redvox/common/constants.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4126 2021-07-07 20:00:14.000000 redvox-3.4.0a2/redvox/common/cross_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    44341 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/data_window.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8246 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/data_window_configuration.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6208 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/data_window_configuration_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    12571 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/data_window_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    31911 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/data_window_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16661 2021-07-07 20:00:14.000000 redvox-3.4.0a2/redvox/common/date_time_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3250 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    39791 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/event_stream.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3397 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/event_stream_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14254 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/file_statistics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22168 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/gap_and_pad_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22503 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/gap_and_pad_utils_old.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.016502 redvox-3.4.0a2/redvox/common/gui/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-04-14 19:22:20.000000 redvox-3.4.0a2/redvox/common/gui/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16251 2021-04-14 23:46:42.000000 redvox-3.4.0a2/redvox/common/gui/cloud_data_retrieval.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    56743 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16272 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/offset_model.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    28604 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/packet_to_pyarrow.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5022 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/parallel_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1256 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/run_me.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    91890 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/sensor_data.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    44259 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/sensor_data_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1206 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/sensor_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18203 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/sensor_reader_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    55914 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/sensor_reader_utils_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    66786 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/station.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1679 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/station_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    42555 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/station_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    23699 2022-06-29 18:15:55.000000 redvox-3.4.0a2/redvox/common/station_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4002 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/stats_helper.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    24492 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/timesync.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1295 2022-04-19 20:47:15.000000 redvox-3.4.0a2/redvox/common/timesync_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    35537 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/timesync_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14138 2022-01-03 23:28:51.000000 redvox-3.4.0a2/redvox/common/tri_message_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1867 2021-07-07 20:00:14.000000 redvox-3.4.0a2/redvox/common/versioning.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     2205 2022-07-07 00:50:48.000000 redvox-3.4.0a2/redvox/settings.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-07-08 00:58:17.003502 redvox-3.4.0a2/redvox.egg-info/
--rw-rw-r--   0 opq       (1000) opq       (1000)      886 2022-07-08 00:58:16.000000 redvox-3.4.0a2/redvox.egg-info/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)     4626 2022-07-08 00:58:16.000000 redvox-3.4.0a2/redvox.egg-info/SOURCES.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)        1 2022-07-08 00:58:16.000000 redvox-3.4.0a2/redvox.egg-info/dependency_links.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       52 2022-07-08 00:58:16.000000 redvox-3.4.0a2/redvox.egg-info/entry_points.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)      386 2022-07-08 00:58:16.000000 redvox-3.4.0a2/redvox.egg-info/requires.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)        7 2022-07-08 00:58:16.000000 redvox-3.4.0a2/redvox.egg-info/top_level.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       38 2022-07-08 00:58:17.017502 redvox-3.4.0a2/setup.cfg
--rw-rw-r--   0 opq       (1000) opq       (1000)     1841 2022-05-27 20:46:10.000000 redvox-3.4.0a2/setup.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.842311 redvox-3.4.0a3/
+-rw-r--r--   0 opq       (1000) opq       (1000)    11343 2023-04-25 23:11:34.000000 redvox-3.4.0a3/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    13908 2023-04-27 23:37:57.842311 redvox-3.4.0a3/PKG-INFO
+-rw-rw-r--   0 opq       (1000) opq       (1000)      517 2021-06-14 20:37:56.000000 redvox-3.4.0a3/README.md
+-rw-r--r--   0 opq       (1000) opq       (1000)     1375 2023-04-27 23:32:39.000000 redvox-3.4.0a3/pyproject.toml
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.825312 redvox-3.4.0a3/redvox/
+-rw-r--r--   0 opq       (1000) opq       (1000)      817 2023-04-27 23:37:44.000000 redvox-3.4.0a3/redvox/__init__.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.826311 redvox-3.4.0a3/redvox/api1000/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/__init__.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.827312 redvox-3.4.0a3/redvox/api1000/common/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    20204 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/common.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1050 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/decorators.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     5359 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/generic.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      875 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/lz4.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2570 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/mapping.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2237 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/metadata.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2435 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/typing.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2114 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/errors.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.827312 redvox-3.4.0a3/redvox/api1000/gui/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/gui/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4672 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/api1000/gui/image_viewer.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.828312 redvox-3.4.0a3/redvox/api1000/proto/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/proto/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    41044 2023-04-25 01:37:07.000000 redvox-3.4.0a3/redvox/api1000/proto/redvox_api_m_pb2.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.828312 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     5639 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/event_streams.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.829311 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    11949 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.829311 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/derived/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14890 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     7398 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/image.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    40936 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/location.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    42236 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3425 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/single.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     5576 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    50437 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/station_information.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19060 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/timing_information.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    21971 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.831312 redvox-3.4.0a3/redvox/api900/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    17514 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/concat.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      494 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/constants.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1689 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/deprecation.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      351 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/exceptions.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.831312 redvox-3.4.0a3/redvox/api900/lib/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/lib/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     7970 2023-04-25 01:37:07.000000 redvox-3.4.0a3/redvox/api900/lib/api900_pb2.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    43091 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/location_analyzer.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2597 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/migrations.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.831312 redvox-3.4.0a3/redvox/api900/qa/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/qa/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2813 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/qa/gap_detection.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16939 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/reader.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    17096 2021-06-07 23:35:09.000000 redvox-3.4.0a3/redvox/api900/reader_utils.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.833311 redvox-3.4.0a3/redvox/api900/sensors/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2113 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/accelerometer_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2298 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/barometer_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2665 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/evenly_sampled_channel.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     6283 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/evenly_sampled_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1989 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/gyroscope_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4854 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/image_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2264 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/infrared_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16540 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/interleaved_channel.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2261 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/light_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    10051 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/location_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2022 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/magnetometer_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3209 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/microphone_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4655 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/time_synchronization_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3536 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/unevenly_sampled_channel.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     6619 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/unevenly_sampled_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     5907 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1128 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/stat_utils.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     8780 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/summarize.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.834311 redvox-3.4.0a3/redvox/api900/timesync/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/timesync/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    27606 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/timesync/api900_timesync.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    13824 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/timesync/tri_message_stats.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1537 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/types.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    54392 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/wrapped_redvox_packet.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.834311 redvox-3.4.0a3/redvox/cli/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cli/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    22678 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/cli/cli.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6683 2021-06-07 23:35:09.000000 redvox-3.4.0a3/redvox/cli/conversions.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1797 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/cli/data_req.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.836311 redvox-3.4.0a3/redvox/cloud/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     2267 2021-04-06 18:15:12.000000 redvox-3.4.0a3/redvox/cloud/api.py
+-rw-r--r--   0 opq       (1000) opq       (1000)   142063 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/api_m_fqns.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4334 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/auth_api.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    27215 2022-04-20 20:36:13.000000 redvox-3.4.0a3/redvox/cloud/client.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5905 2021-09-16 19:39:56.000000 redvox-3.4.0a3/redvox/cloud/config.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6088 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/cloud/data_api.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3829 2021-09-16 19:39:56.000000 redvox-3.4.0a3/redvox/cloud/data_client.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3094 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/data_io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      487 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/errors.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    18946 2022-04-20 20:36:13.000000 redvox-3.4.0a3/redvox/cloud/metadata_api.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3770 2021-04-14 23:45:25.000000 redvox-3.4.0a3/redvox/cloud/query_timing_correction.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      902 2022-04-20 20:36:13.000000 redvox-3.4.0a3/redvox/cloud/routes.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4262 2021-04-14 23:45:25.000000 redvox-3.4.0a3/redvox/cloud/station_stats.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     7707 2022-06-01 22:08:00.000000 redvox-3.4.0a3/redvox/cloud/subscription.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.842311 redvox-3.4.0a3/redvox/common/
+-rw-r--r--   0 opq       (1000) opq       (1000)      195 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/common/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    55240 2022-09-30 02:01:56.000000 redvox-3.4.0a3/redvox/common/api_conversions.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    23044 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/api_reader.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5527 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/api_reader_dw.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    12875 2021-06-07 23:35:09.000000 redvox-3.4.0a3/redvox/common/api_reader_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1173 2021-04-20 02:39:13.000000 redvox-3.4.0a3/redvox/common/constants.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4126 2021-07-07 20:00:14.000000 redvox-3.4.0a3/redvox/common/cross_stats.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    44341 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/data_window.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8246 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/data_window_configuration.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6208 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/data_window_configuration_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    12571 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/data_window_io.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    31911 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/data_window_old.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16785 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/date_time_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3250 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/errors.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    39791 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/event_stream.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3397 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/event_stream_io.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    14254 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/file_statistics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    22168 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/gap_and_pad_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    22503 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/gap_and_pad_utils_old.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.842311 redvox-3.4.0a3/redvox/common/gui/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/common/gui/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    16251 2021-04-14 23:46:42.000000 redvox-3.4.0a3/redvox/common/gui/cloud_data_retrieval.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    56743 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    25612 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/offset_model.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    27554 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/packet_to_pyarrow.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5022 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/parallel_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1256 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/run_me.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    94299 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/sensor_data.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    44259 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/sensor_data_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1206 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/sensor_io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    18349 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/sensor_reader_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    55914 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/sensor_reader_utils_old.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3352 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/session_io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    44577 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/session_model.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14986 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/session_model_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    66786 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/station.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1679 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/station_io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4515 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/station_model.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    42555 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/station_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    23699 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/station_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4002 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/stats_helper.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    24492 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/timesync.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1295 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/timesync_io.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    35537 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/timesync_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    14138 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/tri_message_stats.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1867 2021-07-07 20:00:14.000000 redvox-3.4.0a3/redvox/common/versioning.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2483 2022-09-30 02:01:51.000000 redvox-3.4.0a3/redvox/settings.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.826311 redvox-3.4.0a3/redvox.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    13908 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     4767 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       51 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/entry_points.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      386 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        7 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:37:57.842311 redvox-3.4.0a3/setup.cfg
```

### Comparing `redvox-3.4.0a2/README.md` & `redvox-3.4.0a3/README.md`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/__init__.py` & `redvox-3.4.0a3/redvox/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Provides library level metadata and constants.
 """
 
 NAME: str = "redvox"
-VERSION: str = "3.4.0a2"
+VERSION: str = "3.4.0a3"
 
 
 def version() -> str:
     """Returns the version number of this library."""
     return VERSION
 
 
@@ -23,8 +23,9 @@
     import redvox.settings
 
     print()
     print(f"version: {VERSION}")
     print(f"parallelism enabled: {redvox.settings.is_parallelism_enabled()}")
     print(f"native extra enabled: {redvox.settings.is_native_extra_enabled()}")
     print(f"gui extra enabled: {redvox.settings.is_gui_extra_enabled()}")
+    print(f"protobuf cpp backend enabled: {redvox.settings.is_cpp_backend_enabled()}")
     print()
```

### Comparing `redvox-3.4.0a2/redvox/api1000/common/common.py` & `redvox-3.4.0a3/redvox/api1000/common/common.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/common/decorators.py` & `redvox-3.4.0a3/redvox/api1000/common/decorators.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/common/generic.py` & `redvox-3.4.0a3/redvox/api1000/common/generic.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/common/lz4.py` & `redvox-3.4.0a3/redvox/api1000/common/lz4.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/common/mapping.py` & `redvox-3.4.0a3/redvox/api1000/common/mapping.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/common/metadata.py` & `redvox-3.4.0a3/redvox/api1000/common/metadata.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/common/typing.py` & `redvox-3.4.0a3/redvox/api1000/common/typing.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/errors.py` & `redvox-3.4.0a3/redvox/api1000/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/gui/image_viewer.py` & `redvox-3.4.0a3/redvox/api1000/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/proto/redvox_api_m_pb2.py` & `redvox-3.4.0a3/redvox/api1000/proto/redvox_api_m_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-SUB_API: float = 10.0  # redvox-api-1000 -> build_protos.sh -> insert_sub_api.py on 2022-07-07 00:07:12.686182
+SUB_API: float = 10.0
 
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: src/redvox_api_m/redvox_api_m.proto
+# source: redvox_api_m.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#src/redvox_api_m/redvox_api_m.proto\x12\x0credvox_api_m\"\xecs\n\rRedvoxPacketM\x12\x0b\n\x03\x61pi\x18\x01 \x01(\x02\x12\x0f\n\x07sub_api\x18\x02 \x01(\x02\x12K\n\x13station_information\x18\x03 \x01(\x0b\x32..redvox_api_m.RedvoxPacketM.StationInformation\x12I\n\x12timing_information\x18\x04 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.TimingInformation\x12\x34\n\x07sensors\x18\x05 \x01(\x0b\x32#.redvox_api_m.RedvoxPacketM.Sensors\x12>\n\revent_streams\x18\x06 \x03(\x0b\x32\'.redvox_api_m.RedvoxPacketM.EventStream\x12;\n\x08metadata\x18\x07 \x03(\x0b\x32).redvox_api_m.RedvoxPacketM.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd1$\n\x12StationInformation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x61uth_id\x18\x04 \x01(\t\x12\x0c\n\x04make\x18\x05 \x01(\t\x12\r\n\x05model\x18\x06 \x01(\t\x12\x41\n\x02os\x18\x07 \x01(\x0e\x32\x35.redvox_api_m.RedvoxPacketM.StationInformation.OsType\x12\x12\n\nos_version\x18\x08 \x01(\t\x12\x13\n\x0b\x61pp_version\x18\t \x01(\t\x12\x12\n\nis_private\x18\n \x01(\x08\x12P\n\x0c\x61pp_settings\x18\x0b \x01(\x0b\x32:.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings\x12V\n\x0fstation_metrics\x18\x0c \x01(\x0b\x32=.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics\x12P\n\x0cservice_urls\x18\r \x01(\x0b\x32:.redvox_api_m.RedvoxPacketM.StationInformation.ServiceUrls\x12N\n\x08metadata\x18\x0e \x03(\x0b\x32<.redvox_api_m.RedvoxPacketM.StationInformation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xe1\x01\n\x0bServiceUrls\x12\x13\n\x0b\x61uth_server\x18\x01 \x01(\t\x12\x14\n\x0csynch_server\x18\x02 \x01(\t\x12\x1a\n\x12\x61\x63quisition_server\x18\x03 \x01(\t\x12Z\n\x08metadata\x18\x04 \x03(\x0b\x32H.redvox_api_m.RedvoxPacketM.StationInformation.ServiceUrls.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf9\x0c\n\x0eStationMetrics\x12=\n\ntimestamps\x18\x01 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12_\n\x0cnetwork_type\x18\x02 \x03(\x0e\x32I.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.NetworkType\x12j\n\x12\x63\x65ll_service_state\x18\x03 \x03(\x0e\x32N.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.CellServiceState\x12\x43\n\x10network_strength\x18\x04 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12>\n\x0btemperature\x18\x05 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12:\n\x07\x62\x61ttery\x18\x06 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x62\x61ttery_current\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12@\n\ravailable_ram\x18\x08 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x41\n\x0e\x61vailable_disk\x18\t \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x63pu_utilization\x18\n \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12]\n\x0bpower_state\x18\x0b \x03(\x0e\x32H.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.PowerState\x12\x62\n\x0ewifi_wake_lock\x18\x0c \x03(\x0e\x32J.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.WifiWakeLock\x12_\n\x0cscreen_state\x18\r \x03(\x0e\x32I.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.ScreenState\x12\x44\n\x11screen_brightness\x18\x0e \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12]\n\x08metadata\x18\x0f \x03(\x0b\x32K.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"U\n\x0bNetworkType\x12\x13\n\x0fUNKNOWN_NETWORK\x10\x00\x12\x0e\n\nNO_NETWORK\x10\x01\x12\x08\n\x04WIFI\x10\x02\x12\x0c\n\x08\x43\x45LLULAR\x10\x03\x12\t\n\x05WIRED\x10\x04\"C\n\x0cWifiWakeLock\x12\x08\n\x04NONE\x10\x00\x12\r\n\tHIGH_PERF\x10\x01\x12\x0f\n\x0bLOW_LATENCY\x10\x02\x12\t\n\x05OTHER\x10\x03\"^\n\x10\x43\x65llServiceState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tEMERGENCY\x10\x01\x12\x0b\n\x07NOMINAL\x10\x02\x12\x12\n\x0eOUT_OF_SERVICE\x10\x03\x12\r\n\tPOWER_OFF\x10\x04\"O\n\nPowerState\x12\x17\n\x13UNKNOWN_POWER_STATE\x10\x00\x12\r\n\tUNPLUGGED\x10\x01\x12\x0c\n\x08\x43HARGING\x10\x02\x12\x0b\n\x07\x43HARGED\x10\x03\"F\n\x0bScreenState\x12\x18\n\x14UNKNOWN_SCREEN_STATE\x10\x00\x12\x06\n\x02ON\x10\x01\x12\x07\n\x03OFF\x10\x02\x12\x0c\n\x08HEADLESS\x10\x03\x1a\xe9\x0f\n\x0b\x41ppSettings\x12i\n\x13\x61udio_sampling_rate\x18\x01 \x01(\x0e\x32L.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.AudioSamplingRate\x12\x1a\n\x12samples_per_window\x18\x02 \x01(\x02\x12i\n\x13\x61udio_source_tuning\x18\x03 \x01(\x0e\x32L.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.AudioSourceTuning\x12h\n\x18\x61\x64\x64itional_input_sensors\x18\x04 \x03(\x0e\x32\x46.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.InputSensor\x12\x1c\n\x14\x61utomatically_record\x18\x05 \x01(\x08\x12\x1a\n\x12launch_at_power_up\x18\x06 \x01(\x08\x12\x12\n\nstation_id\x18\x07 \x01(\t\x12\x1b\n\x13station_description\x18\x08 \x01(\t\x12\x16\n\x0epush_to_server\x18\t \x01(\x08\x12\x1f\n\x17publish_data_as_private\x18\n \x01(\x08\x12\x1b\n\x13scramble_audio_data\x18\x0b \x01(\x08\x12\x18\n\x10provide_backfill\x18\x0c \x01(\x08\x12\x1f\n\x17remove_sensor_dc_offset\x18\r \x01(\x08\x12Z\n\x0b\x66\x66t_overlap\x18\x0e \x01(\x0e\x32\x45.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.FftOverlap\x12#\n\x1buse_custom_time_sync_server\x18\x0f \x01(\x08\x12\x1c\n\x14time_sync_server_url\x18\x10 \x01(\t\x12\x1e\n\x16use_custom_data_server\x18\x11 \x01(\x08\x12\x17\n\x0f\x64\x61ta_server_url\x18\x12 \x01(\t\x12\x1e\n\x16use_custom_auth_server\x18\x13 \x01(\x08\x12\x17\n\x0f\x61uth_server_url\x18\x14 \x01(\t\x12\x1e\n\x16\x61uto_delete_data_files\x18\x15 \x01(\x08\x12\x1f\n\x17storage_space_allowance\x18\x16 \x01(\x02\x12$\n\x1cuse_sd_card_for_data_storage\x18\x17 \x01(\x08\x12\x1d\n\x15use_location_services\x18\x18 \x01(\x08\x12\x14\n\x0cuse_latitude\x18\x19 \x01(\x01\x12\x15\n\ruse_longitude\x18\x1a \x01(\x01\x12\x14\n\x0cuse_altitude\x18\x1b \x01(\x02\x12P\n\x0cmetrics_rate\x18\x1c \x01(\x0e\x32:.redvox_api_m.RedvoxPacketM.StationInformation.MetricsRate\x12Z\n\x08metadata\x18\x1d \x03(\x0b\x32H.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"I\n\nFftOverlap\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nPERCENT_25\x10\x01\x12\x0e\n\nPERCENT_50\x10\x02\x12\x0e\n\nPERCENT_75\x10\x03\"n\n\x11\x41udioSamplingRate\x12\x19\n\x15UNKNOWN_SAMPLING_RATE\x10\x00\x12\t\n\x05HZ_80\x10\x01\x12\n\n\x06HZ_800\x10\x02\x12\x0b\n\x07HZ_8000\x10\x03\x12\x0c\n\x08HZ_16000\x10\x04\x12\x0c\n\x08HZ_48000\x10\x05\"f\n\x11\x41udioSourceTuning\x12\x12\n\x0eUNKNOWN_TUNING\x10\x00\x12\x15\n\x11INFRASOUND_TUNING\x10\x01\x12\x14\n\x10LOW_AUDIO_TUNING\x10\x02\x12\x10\n\x0c\x41UDIO_TUNING\x10\x03\"\xa5\x03\n\x0bInputSensor\x12\x12\n\x0eUNKNOWN_SENSOR\x10\x00\x12\x11\n\rACCELEROMETER\x10\x01\x12\x16\n\x12\x41\x43\x43\x45LEROMETER_FAST\x10\x02\x12\x17\n\x13\x41MBIENT_TEMPERATURE\x10\x03\x12\t\n\x05\x41UDIO\x10\x04\x12\x14\n\x10\x43OMPRESSED_AUDIO\x10\x05\x12\x0b\n\x07GRAVITY\x10\x06\x12\r\n\tGYROSCOPE\x10\x07\x12\x12\n\x0eGYROSCOPE_FAST\x10\x08\x12\x14\n\x10IMAGE_PER_SECOND\x10\t\x12\x14\n\x10IMAGE_PER_PACKET\x10\n\x12\t\n\x05LIGHT\x10\x0b\x12\x17\n\x13LINEAR_ACCELERATION\x10\x0c\x12\x0c\n\x08LOCATION\x10\r\x12\x10\n\x0cMAGNETOMETER\x10\x0e\x12\x15\n\x11MAGNETOMETER_FAST\x10\x0f\x12\x0f\n\x0bORIENTATION\x10\x10\x12\x0c\n\x08PRESSURE\x10\x11\x12\r\n\tPROXIMITY\x10\x12\x12\x15\n\x11RELATIVE_HUMIDITY\x10\x13\x12\x13\n\x0fROTATION_VECTOR\x10\x14\x12\x0c\n\x08VELOCITY\x10\x15\"O\n\x06OsType\x12\x0e\n\nUNKNOWN_OS\x10\x00\x12\x0b\n\x07\x41NDROID\x10\x01\x12\x07\n\x03IOS\x10\x02\x12\x07\n\x03OSX\x10\x03\x12\t\n\x05LINUX\x10\x04\x12\x0b\n\x07WINDOWS\x10\x05\"D\n\x0bMetricsRate\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x13\n\x0fONCE_PER_SECOND\x10\x01\x12\x13\n\x0fONCE_PER_PACKET\x10\x02\x1a\xc0\x07\n\x11TimingInformation\x12!\n\x19packet_start_os_timestamp\x18\x01 \x01(\x01\x12#\n\x1bpacket_start_mach_timestamp\x18\x02 \x01(\x01\x12\x1f\n\x17packet_end_os_timestamp\x18\x03 \x01(\x01\x12!\n\x19packet_end_mach_timestamp\x18\x04 \x01(\x01\x12,\n$server_acquisition_arrival_timestamp\x18\x05 \x01(\x01\x12 \n\x18\x61pp_start_mach_timestamp\x18\x06 \x01(\x01\x12T\n\x0fsynch_exchanges\x18\x07 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.TimingInformation.SynchExchange\x12\x14\n\x0c\x62\x65st_latency\x18\x08 \x01(\x02\x12\x13\n\x0b\x62\x65st_offset\x18\t \x01(\x02\x12\r\n\x05score\x18\n \x01(\x02\x12U\n\x0cscore_method\x18\x0b \x01(\x0e\x32?.redvox_api_m.RedvoxPacketM.TimingInformation.TimingScoreMethod\x12.\n\x04unit\x18\x0c \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12M\n\x08metadata\x18\r \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.TimingInformation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x95\x02\n\rSynchExchange\x12\n\n\x02\x61\x31\x18\x01 \x01(\x01\x12\n\n\x02\x61\x32\x18\x02 \x01(\x01\x12\n\n\x02\x61\x33\x18\x03 \x01(\x01\x12\n\n\x02\x62\x31\x18\x04 \x01(\x01\x12\n\n\x02\x62\x32\x18\x05 \x01(\x01\x12\n\n\x02\x62\x33\x18\x06 \x01(\x01\x12.\n\x04unit\x18\x07 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12[\n\x08metadata\x18\x08 \x03(\x0b\x32I.redvox_api_m.RedvoxPacketM.TimingInformation.SynchExchange.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\" \n\x11TimingScoreMethod\x12\x0b\n\x07UNKNOWN\x10\x00\x1a\xa8\x30\n\x07Sensors\x12>\n\raccelerometer\x18\x01 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12G\n\x13\x61mbient_temperature\x18\x02 \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x38\n\x05\x61udio\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.Sensors.Audio\x12M\n\x10\x63ompressed_audio\x18\x04 \x01(\x0b\x32\x33.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio\x12\x38\n\x07gravity\x18\x05 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12:\n\tgyroscope\x18\x06 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x38\n\x05image\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.Sensors.Image\x12\x39\n\x05light\x18\x08 \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x44\n\x13linear_acceleration\x18\t \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12>\n\x08location\x18\n \x01(\x0b\x32,.redvox_api_m.RedvoxPacketM.Sensors.Location\x12=\n\x0cmagnetometer\x18\x0b \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12<\n\x0borientation\x18\x0c \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12<\n\x08pressure\x18\r \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12=\n\tproximity\x18\x0e \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x45\n\x11relative_humidity\x18\x0f \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12@\n\x0frotation_vector\x18\x10 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x39\n\x08velocity\x18\x11 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x43\n\x08metadata\x18\x12 \x03(\x0b\x32\x31.redvox_api_m.RedvoxPacketM.Sensors.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd3\x02\n\x05\x41udio\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12\x1e\n\x16\x66irst_sample_timestamp\x18\x02 \x01(\x01\x12\x13\n\x0bsample_rate\x18\x03 \x01(\x02\x12\x19\n\x11\x62its_of_precision\x18\x04 \x01(\x02\x12\x14\n\x0cis_scrambled\x18\x05 \x01(\x08\x12\x10\n\x08\x65ncoding\x18\x06 \x01(\t\x12:\n\x07samples\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12I\n\x08metadata\x18\x08 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.Sensors.Audio.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x8d\x03\n\x0f\x43ompressedAudio\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12\x1e\n\x16\x66irst_sample_timestamp\x18\x02 \x01(\x01\x12\x13\n\x0bsample_rate\x18\x03 \x01(\x02\x12\x14\n\x0cis_scrambled\x18\x04 \x01(\x08\x12\x13\n\x0b\x61udio_bytes\x18\x05 \x01(\x0c\x12S\n\x0b\x61udio_codec\x18\x06 \x01(\x0e\x32>.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio.AudioCodec\x12S\n\x08metadata\x18\x07 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"#\n\nAudioCodec\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04\x46LAC\x10\x01\x1a\x9c\x02\n\x06Single\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12:\n\x07samples\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12J\n\x08metadata\x18\x04 \x03(\x0b\x32\x38.redvox_api_m.RedvoxPacketM.Sensors.Single.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd6\x18\n\x08Location\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12\x41\n\x0etimestamps_gps\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12I\n\x10latitude_samples\x18\x04 \x01(\x0b\x32/.redvox_api_m.RedvoxPacketM.DoubleSamplePayload\x12J\n\x11longitude_samples\x18\x05 \x01(\x0b\x32/.redvox_api_m.RedvoxPacketM.DoubleSamplePayload\x12\x43\n\x10\x61ltitude_samples\x18\x06 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12@\n\rspeed_samples\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x62\x65\x61ring_samples\x18\x08 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12N\n\x1bhorizontal_accuracy_samples\x18\t \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12L\n\x19vertical_accuracy_samples\x18\n \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12I\n\x16speed_accuracy_samples\x18\x0b \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12K\n\x18\x62\x65\x61ring_accuracy_samples\x18\x0c \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12U\n\x12last_best_location\x18\r \x01(\x0b\x32\x39.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation\x12X\n\x15overall_best_location\x18\x0e \x01(\x0b\x32\x39.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation\x12$\n\x1clocation_permissions_granted\x18\x0f \x01(\x08\x12#\n\x1blocation_services_requested\x18\x10 \x01(\x08\x12!\n\x19location_services_enabled\x18\x11 \x01(\x08\x12Y\n\x12location_providers\x18\x12 \x03(\x0e\x32=.redvox_api_m.RedvoxPacketM.Sensors.Location.LocationProvider\x12L\n\x08metadata\x18\x13 \x03(\x0b\x32:.redvox_api_m.RedvoxPacketM.Sensors.Location.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xcf\r\n\x0c\x42\x65stLocation\x12m\n\x1clatitude_longitude_timestamp\x18\x01 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x63\n\x12\x61ltitude_timestamp\x18\x02 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12`\n\x0fspeed_timestamp\x18\x03 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x62\n\x11\x62\x65\x61ring_timestamp\x18\x04 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x41\n\x17latitude_longitude_unit\x18\x05 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x37\n\raltitude_unit\x18\x06 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x34\n\nspeed_unit\x18\x07 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x36\n\x0c\x62\x65\x61ring_unit\x18\x08 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12@\n\x16vertical_accuracy_unit\x18\t \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x42\n\x18horizontal_accuracy_unit\x18\n \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12=\n\x13speed_accuracy_unit\x18\x0b \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12?\n\x15\x62\x65\x61ring_accuracy_unit\x18\x0c \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x10\n\x08latitude\x18\r \x01(\x01\x12\x11\n\tlongitude\x18\x0e \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x0f \x01(\x02\x12\r\n\x05speed\x18\x10 \x01(\x02\x12\x0f\n\x07\x62\x65\x61ring\x18\x11 \x01(\x02\x12\x19\n\x11vertical_accuracy\x18\x12 \x01(\x02\x12\x1b\n\x13horizontal_accuracy\x18\x13 \x01(\x02\x12\x16\n\x0espeed_accuracy\x18\x14 \x01(\x02\x12\x18\n\x10\x62\x65\x61ring_accuracy\x18\x15 \x01(\x02\x12\r\n\x05score\x18\x16 \x01(\x02\x12]\n\x06method\x18\x17 \x01(\x0e\x32M.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.LocationScoreMethod\x12X\n\x11location_provider\x18\x18 \x01(\x0e\x32=.redvox_api_m.RedvoxPacketM.Sensors.Location.LocationProvider\x12Y\n\x08metadata\x18\x19 \x03(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf4\x01\n\rBestTimestamp\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0c\n\x04mach\x18\x02 \x01(\x01\x12\x0b\n\x03gps\x18\x03 \x01(\x01\x12g\n\x08metadata\x18\x04 \x03(\x0b\x32U.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\")\n\x13LocationScoreMethod\x12\x12\n\x0eUNKNOWN_METHOD\x10\x00\"I\n\x10LocationProvider\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\x08\n\x04USER\x10\x02\x12\x07\n\x03GPS\x10\x03\x12\x0b\n\x07NETWORK\x10\x04\x1a\x94\x03\n\x03Xyz\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12<\n\tx_samples\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12<\n\ty_samples\x18\x04 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12<\n\tz_samples\x18\x05 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12G\n\x08metadata\x18\x06 \x03(\x0b\x32\x35.redvox_api_m.RedvoxPacketM.Sensors.Xyz.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf0\x02\n\x05Image\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12\x0f\n\x07samples\x18\x03 \x03(\x0c\x12I\n\x0bimage_codec\x18\x04 \x01(\x0e\x32\x34.redvox_api_m.RedvoxPacketM.Sensors.Image.ImageCodec\x12I\n\x08metadata\x18\x05 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.Sensors.Image.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"4\n\nImageCodec\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03PNG\x10\x01\x12\x07\n\x03JPG\x10\x02\x12\x07\n\x03\x42MP\x10\x03\x1a\xf2\x07\n\x0b\x45ventStream\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12=\n\x06\x65vents\x18\x03 \x03(\x0b\x32-.redvox_api_m.RedvoxPacketM.EventStream.Event\x12G\n\x08metadata\x18\x04 \x03(\x0b\x32\x35.redvox_api_m.RedvoxPacketM.EventStream.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xdc\x05\n\x05\x45vent\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12X\n\x0estring_payload\x18\x02 \x03(\x0b\x32@.redvox_api_m.RedvoxPacketM.EventStream.Event.StringPayloadEntry\x12Z\n\x0fnumeric_payload\x18\x03 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.EventStream.Event.NumericPayloadEntry\x12Z\n\x0f\x62oolean_payload\x18\x04 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.EventStream.Event.BooleanPayloadEntry\x12T\n\x0c\x62yte_payload\x18\x05 \x03(\x0b\x32>.redvox_api_m.RedvoxPacketM.EventStream.Event.BytePayloadEntry\x12M\n\x08metadata\x18\x06 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.EventStream.Event.MetadataEntry\x1a\x34\n\x12StringPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x35\n\x13NumericPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\x1a\x35\n\x13\x42ooleanPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\x1a\x32\n\x10\x42ytePayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x94\x02\n\rSamplePayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0e\n\x06values\x18\x02 \x03(\x02\x12G\n\x10value_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12I\n\x08metadata\x18\x04 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.SamplePayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xa0\x02\n\x13\x44oubleSamplePayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0e\n\x06values\x18\x02 \x03(\x01\x12G\n\x10value_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12O\n\x08metadata\x18\x04 \x03(\x0b\x32=.redvox_api_m.RedvoxPacketM.DoubleSamplePayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd1\x02\n\rTimingPayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x12\n\ntimestamps\x18\x02 \x03(\x01\x12K\n\x14timestamp_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12\x18\n\x10mean_sample_rate\x18\x04 \x01(\x02\x12\x19\n\x11stdev_sample_rate\x18\x05 \x01(\x02\x12I\n\x08metadata\x18\x06 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.TimingPayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf5\x01\n\x11SummaryStatistics\x12\r\n\x05\x63ount\x18\x01 \x01(\x01\x12\x0c\n\x04mean\x18\x02 \x01(\x01\x12\x1a\n\x12standard_deviation\x18\x03 \x01(\x01\x12\x0b\n\x03min\x18\x04 \x01(\x01\x12\x0b\n\x03max\x18\x05 \x01(\x01\x12\r\n\x05range\x18\x06 \x01(\x01\x12M\n\x08metadata\x18\x07 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.SummaryStatistics.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x03\n\x04Unit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x1d\n\x19METERS_PER_SECOND_SQUARED\x10\x01\x12\x0e\n\nKILOPASCAL\x10\x02\x12\x16\n\x12RADIANS_PER_SECOND\x10\x03\x12\x13\n\x0f\x44\x45\x43IMAL_DEGREES\x10\x04\x12\n\n\x06METERS\x10\x05\x12\x15\n\x11METERS_PER_SECOND\x10\x06\x12\x0e\n\nMICROTESLA\x10\x07\x12\x19\n\x15LSB_PLUS_MINUS_COUNTS\x10\x08\x12!\n\x1dMICROSECONDS_SINCE_UNIX_EPOCH\x10\t\x12\x0b\n\x07\x44\x45\x43IBEL\x10\n\x12\x13\n\x0f\x44\x45GREES_CELSIUS\x10\x0b\x12\x08\n\x04\x42YTE\x10\x0c\x12\x0e\n\nPERCENTAGE\x10\r\x12\x0b\n\x07RADIANS\x10\x0e\x12\x10\n\x0cMICROAMPERES\x10\x0f\x12\x0f\n\x0b\x43\x45NTIMETERS\x10\x10\x12\x15\n\x11NORMALIZED_COUNTS\x10\x11\x12\x07\n\x03LUX\x10\x12\x12\x0c\n\x08UNITLESS\x10\x13\x12\x07\n\x03PCM\x10\x14\"\xac\x01\n\x16\x45ncryptedRedvoxPacketM\x12\x0e\n\x06header\x18\x01 \x01(\x0c\x12\x0e\n\x06packet\x18\x02 \x01(\x0c\x1ar\n\x06Header\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x12\n\nauth_token\x18\x03 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x04 \x01(\t\x12\x12\n\nauth_email\x18\x05 \x01(\t\"\x89\x01\n\x12\x41\x63quisitionRequest\x12\x12\n\nauth_token\x18\x01 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x02 \x01(\t\x12\x10\n\x08\x63hecksum\x18\x03 \x01(\x03\x12\x14\n\x0cis_encrypted\x18\x04 \x01(\x08\x12\x0f\n\x07payload\x18\x05 \x01(\x0c\x12\x0e\n\x06seq_id\x18\x06 \x01(\x03\"\xf5\x01\n\x13\x41\x63quisitionResponse\x12\x45\n\rresponse_type\x18\x01 \x01(\x0e\x32..redvox_api_m.AcquisitionResponse.ResponseType\x12\x10\n\x08\x63hecksum\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\x12\x0e\n\x06resend\x18\x04 \x01(\x08\x12\x0e\n\x06seq_id\x18\x05 \x01(\x03\"T\n\x0cResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02OK\x10\x01\x12\x0e\n\nAUTH_ERROR\x10\x02\x12\x0e\n\nDATA_ERROR\x10\x03\x12\x0f\n\x0bOTHER_ERROR\x10\x04\"\\\n\x0cSynchRequest\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x0e\n\x06seq_id\x18\x03 \x01(\r\x12\x12\n\nsub_seq_id\x18\x04 \x01(\r\"\x85\x01\n\rSynchResponse\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x0e\n\x06seq_id\x18\x03 \x01(\r\x12\x12\n\nsub_seq_id\x18\x04 \x01(\r\x12\x12\n\nrecv_ts_us\x18\x05 \x01(\x04\x12\x12\n\nsend_ts_us\x18\x06 \x01(\x04\x42\x10\n\x0eio.redvox.apisb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12redvox_api_m.proto\x12\x0credvox_api_m\"\xecs\n\rRedvoxPacketM\x12\x0b\n\x03\x61pi\x18\x01 \x01(\x02\x12\x0f\n\x07sub_api\x18\x02 \x01(\x02\x12K\n\x13station_information\x18\x03 \x01(\x0b\x32..redvox_api_m.RedvoxPacketM.StationInformation\x12I\n\x12timing_information\x18\x04 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.TimingInformation\x12\x34\n\x07sensors\x18\x05 \x01(\x0b\x32#.redvox_api_m.RedvoxPacketM.Sensors\x12>\n\revent_streams\x18\x06 \x03(\x0b\x32\'.redvox_api_m.RedvoxPacketM.EventStream\x12;\n\x08metadata\x18\x07 \x03(\x0b\x32).redvox_api_m.RedvoxPacketM.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd1$\n\x12StationInformation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x61uth_id\x18\x04 \x01(\t\x12\x0c\n\x04make\x18\x05 \x01(\t\x12\r\n\x05model\x18\x06 \x01(\t\x12\x41\n\x02os\x18\x07 \x01(\x0e\x32\x35.redvox_api_m.RedvoxPacketM.StationInformation.OsType\x12\x12\n\nos_version\x18\x08 \x01(\t\x12\x13\n\x0b\x61pp_version\x18\t \x01(\t\x12\x12\n\nis_private\x18\n \x01(\x08\x12P\n\x0c\x61pp_settings\x18\x0b \x01(\x0b\x32:.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings\x12V\n\x0fstation_metrics\x18\x0c \x01(\x0b\x32=.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics\x12P\n\x0cservice_urls\x18\r \x01(\x0b\x32:.redvox_api_m.RedvoxPacketM.StationInformation.ServiceUrls\x12N\n\x08metadata\x18\x0e \x03(\x0b\x32<.redvox_api_m.RedvoxPacketM.StationInformation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xe1\x01\n\x0bServiceUrls\x12\x13\n\x0b\x61uth_server\x18\x01 \x01(\t\x12\x14\n\x0csynch_server\x18\x02 \x01(\t\x12\x1a\n\x12\x61\x63quisition_server\x18\x03 \x01(\t\x12Z\n\x08metadata\x18\x04 \x03(\x0b\x32H.redvox_api_m.RedvoxPacketM.StationInformation.ServiceUrls.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf9\x0c\n\x0eStationMetrics\x12=\n\ntimestamps\x18\x01 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12_\n\x0cnetwork_type\x18\x02 \x03(\x0e\x32I.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.NetworkType\x12j\n\x12\x63\x65ll_service_state\x18\x03 \x03(\x0e\x32N.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.CellServiceState\x12\x43\n\x10network_strength\x18\x04 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12>\n\x0btemperature\x18\x05 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12:\n\x07\x62\x61ttery\x18\x06 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x62\x61ttery_current\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12@\n\ravailable_ram\x18\x08 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x41\n\x0e\x61vailable_disk\x18\t \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x63pu_utilization\x18\n \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12]\n\x0bpower_state\x18\x0b \x03(\x0e\x32H.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.PowerState\x12\x62\n\x0ewifi_wake_lock\x18\x0c \x03(\x0e\x32J.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.WifiWakeLock\x12_\n\x0cscreen_state\x18\r \x03(\x0e\x32I.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.ScreenState\x12\x44\n\x11screen_brightness\x18\x0e \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12]\n\x08metadata\x18\x0f \x03(\x0b\x32K.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"U\n\x0bNetworkType\x12\x13\n\x0fUNKNOWN_NETWORK\x10\x00\x12\x0e\n\nNO_NETWORK\x10\x01\x12\x08\n\x04WIFI\x10\x02\x12\x0c\n\x08\x43\x45LLULAR\x10\x03\x12\t\n\x05WIRED\x10\x04\"C\n\x0cWifiWakeLock\x12\x08\n\x04NONE\x10\x00\x12\r\n\tHIGH_PERF\x10\x01\x12\x0f\n\x0bLOW_LATENCY\x10\x02\x12\t\n\x05OTHER\x10\x03\"^\n\x10\x43\x65llServiceState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tEMERGENCY\x10\x01\x12\x0b\n\x07NOMINAL\x10\x02\x12\x12\n\x0eOUT_OF_SERVICE\x10\x03\x12\r\n\tPOWER_OFF\x10\x04\"O\n\nPowerState\x12\x17\n\x13UNKNOWN_POWER_STATE\x10\x00\x12\r\n\tUNPLUGGED\x10\x01\x12\x0c\n\x08\x43HARGING\x10\x02\x12\x0b\n\x07\x43HARGED\x10\x03\"F\n\x0bScreenState\x12\x18\n\x14UNKNOWN_SCREEN_STATE\x10\x00\x12\x06\n\x02ON\x10\x01\x12\x07\n\x03OFF\x10\x02\x12\x0c\n\x08HEADLESS\x10\x03\x1a\xe9\x0f\n\x0b\x41ppSettings\x12i\n\x13\x61udio_sampling_rate\x18\x01 \x01(\x0e\x32L.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.AudioSamplingRate\x12\x1a\n\x12samples_per_window\x18\x02 \x01(\x02\x12i\n\x13\x61udio_source_tuning\x18\x03 \x01(\x0e\x32L.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.AudioSourceTuning\x12h\n\x18\x61\x64\x64itional_input_sensors\x18\x04 \x03(\x0e\x32\x46.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.InputSensor\x12\x1c\n\x14\x61utomatically_record\x18\x05 \x01(\x08\x12\x1a\n\x12launch_at_power_up\x18\x06 \x01(\x08\x12\x12\n\nstation_id\x18\x07 \x01(\t\x12\x1b\n\x13station_description\x18\x08 \x01(\t\x12\x16\n\x0epush_to_server\x18\t \x01(\x08\x12\x1f\n\x17publish_data_as_private\x18\n \x01(\x08\x12\x1b\n\x13scramble_audio_data\x18\x0b \x01(\x08\x12\x18\n\x10provide_backfill\x18\x0c \x01(\x08\x12\x1f\n\x17remove_sensor_dc_offset\x18\r \x01(\x08\x12Z\n\x0b\x66\x66t_overlap\x18\x0e \x01(\x0e\x32\x45.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.FftOverlap\x12#\n\x1buse_custom_time_sync_server\x18\x0f \x01(\x08\x12\x1c\n\x14time_sync_server_url\x18\x10 \x01(\t\x12\x1e\n\x16use_custom_data_server\x18\x11 \x01(\x08\x12\x17\n\x0f\x64\x61ta_server_url\x18\x12 \x01(\t\x12\x1e\n\x16use_custom_auth_server\x18\x13 \x01(\x08\x12\x17\n\x0f\x61uth_server_url\x18\x14 \x01(\t\x12\x1e\n\x16\x61uto_delete_data_files\x18\x15 \x01(\x08\x12\x1f\n\x17storage_space_allowance\x18\x16 \x01(\x02\x12$\n\x1cuse_sd_card_for_data_storage\x18\x17 \x01(\x08\x12\x1d\n\x15use_location_services\x18\x18 \x01(\x08\x12\x14\n\x0cuse_latitude\x18\x19 \x01(\x01\x12\x15\n\ruse_longitude\x18\x1a \x01(\x01\x12\x14\n\x0cuse_altitude\x18\x1b \x01(\x02\x12P\n\x0cmetrics_rate\x18\x1c \x01(\x0e\x32:.redvox_api_m.RedvoxPacketM.StationInformation.MetricsRate\x12Z\n\x08metadata\x18\x1d \x03(\x0b\x32H.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"I\n\nFftOverlap\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nPERCENT_25\x10\x01\x12\x0e\n\nPERCENT_50\x10\x02\x12\x0e\n\nPERCENT_75\x10\x03\"n\n\x11\x41udioSamplingRate\x12\x19\n\x15UNKNOWN_SAMPLING_RATE\x10\x00\x12\t\n\x05HZ_80\x10\x01\x12\n\n\x06HZ_800\x10\x02\x12\x0b\n\x07HZ_8000\x10\x03\x12\x0c\n\x08HZ_16000\x10\x04\x12\x0c\n\x08HZ_48000\x10\x05\"f\n\x11\x41udioSourceTuning\x12\x12\n\x0eUNKNOWN_TUNING\x10\x00\x12\x15\n\x11INFRASOUND_TUNING\x10\x01\x12\x14\n\x10LOW_AUDIO_TUNING\x10\x02\x12\x10\n\x0c\x41UDIO_TUNING\x10\x03\"\xa5\x03\n\x0bInputSensor\x12\x12\n\x0eUNKNOWN_SENSOR\x10\x00\x12\x11\n\rACCELEROMETER\x10\x01\x12\x16\n\x12\x41\x43\x43\x45LEROMETER_FAST\x10\x02\x12\x17\n\x13\x41MBIENT_TEMPERATURE\x10\x03\x12\t\n\x05\x41UDIO\x10\x04\x12\x14\n\x10\x43OMPRESSED_AUDIO\x10\x05\x12\x0b\n\x07GRAVITY\x10\x06\x12\r\n\tGYROSCOPE\x10\x07\x12\x12\n\x0eGYROSCOPE_FAST\x10\x08\x12\x14\n\x10IMAGE_PER_SECOND\x10\t\x12\x14\n\x10IMAGE_PER_PACKET\x10\n\x12\t\n\x05LIGHT\x10\x0b\x12\x17\n\x13LINEAR_ACCELERATION\x10\x0c\x12\x0c\n\x08LOCATION\x10\r\x12\x10\n\x0cMAGNETOMETER\x10\x0e\x12\x15\n\x11MAGNETOMETER_FAST\x10\x0f\x12\x0f\n\x0bORIENTATION\x10\x10\x12\x0c\n\x08PRESSURE\x10\x11\x12\r\n\tPROXIMITY\x10\x12\x12\x15\n\x11RELATIVE_HUMIDITY\x10\x13\x12\x13\n\x0fROTATION_VECTOR\x10\x14\x12\x0c\n\x08VELOCITY\x10\x15\"O\n\x06OsType\x12\x0e\n\nUNKNOWN_OS\x10\x00\x12\x0b\n\x07\x41NDROID\x10\x01\x12\x07\n\x03IOS\x10\x02\x12\x07\n\x03OSX\x10\x03\x12\t\n\x05LINUX\x10\x04\x12\x0b\n\x07WINDOWS\x10\x05\"D\n\x0bMetricsRate\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x13\n\x0fONCE_PER_SECOND\x10\x01\x12\x13\n\x0fONCE_PER_PACKET\x10\x02\x1a\xc0\x07\n\x11TimingInformation\x12!\n\x19packet_start_os_timestamp\x18\x01 \x01(\x01\x12#\n\x1bpacket_start_mach_timestamp\x18\x02 \x01(\x01\x12\x1f\n\x17packet_end_os_timestamp\x18\x03 \x01(\x01\x12!\n\x19packet_end_mach_timestamp\x18\x04 \x01(\x01\x12,\n$server_acquisition_arrival_timestamp\x18\x05 \x01(\x01\x12 \n\x18\x61pp_start_mach_timestamp\x18\x06 \x01(\x01\x12T\n\x0fsynch_exchanges\x18\x07 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.TimingInformation.SynchExchange\x12\x14\n\x0c\x62\x65st_latency\x18\x08 \x01(\x02\x12\x13\n\x0b\x62\x65st_offset\x18\t \x01(\x02\x12\r\n\x05score\x18\n \x01(\x02\x12U\n\x0cscore_method\x18\x0b \x01(\x0e\x32?.redvox_api_m.RedvoxPacketM.TimingInformation.TimingScoreMethod\x12.\n\x04unit\x18\x0c \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12M\n\x08metadata\x18\r \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.TimingInformation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x95\x02\n\rSynchExchange\x12\n\n\x02\x61\x31\x18\x01 \x01(\x01\x12\n\n\x02\x61\x32\x18\x02 \x01(\x01\x12\n\n\x02\x61\x33\x18\x03 \x01(\x01\x12\n\n\x02\x62\x31\x18\x04 \x01(\x01\x12\n\n\x02\x62\x32\x18\x05 \x01(\x01\x12\n\n\x02\x62\x33\x18\x06 \x01(\x01\x12.\n\x04unit\x18\x07 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12[\n\x08metadata\x18\x08 \x03(\x0b\x32I.redvox_api_m.RedvoxPacketM.TimingInformation.SynchExchange.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\" \n\x11TimingScoreMethod\x12\x0b\n\x07UNKNOWN\x10\x00\x1a\xa8\x30\n\x07Sensors\x12>\n\raccelerometer\x18\x01 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12G\n\x13\x61mbient_temperature\x18\x02 \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x38\n\x05\x61udio\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.Sensors.Audio\x12M\n\x10\x63ompressed_audio\x18\x04 \x01(\x0b\x32\x33.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio\x12\x38\n\x07gravity\x18\x05 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12:\n\tgyroscope\x18\x06 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x38\n\x05image\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.Sensors.Image\x12\x39\n\x05light\x18\x08 \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x44\n\x13linear_acceleration\x18\t \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12>\n\x08location\x18\n \x01(\x0b\x32,.redvox_api_m.RedvoxPacketM.Sensors.Location\x12=\n\x0cmagnetometer\x18\x0b \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12<\n\x0borientation\x18\x0c \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12<\n\x08pressure\x18\r \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12=\n\tproximity\x18\x0e \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x45\n\x11relative_humidity\x18\x0f \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12@\n\x0frotation_vector\x18\x10 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x39\n\x08velocity\x18\x11 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x43\n\x08metadata\x18\x12 \x03(\x0b\x32\x31.redvox_api_m.RedvoxPacketM.Sensors.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd3\x02\n\x05\x41udio\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12\x1e\n\x16\x66irst_sample_timestamp\x18\x02 \x01(\x01\x12\x13\n\x0bsample_rate\x18\x03 \x01(\x02\x12\x19\n\x11\x62its_of_precision\x18\x04 \x01(\x02\x12\x14\n\x0cis_scrambled\x18\x05 \x01(\x08\x12\x10\n\x08\x65ncoding\x18\x06 \x01(\t\x12:\n\x07samples\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12I\n\x08metadata\x18\x08 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.Sensors.Audio.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x8d\x03\n\x0f\x43ompressedAudio\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12\x1e\n\x16\x66irst_sample_timestamp\x18\x02 \x01(\x01\x12\x13\n\x0bsample_rate\x18\x03 \x01(\x02\x12\x14\n\x0cis_scrambled\x18\x04 \x01(\x08\x12\x13\n\x0b\x61udio_bytes\x18\x05 \x01(\x0c\x12S\n\x0b\x61udio_codec\x18\x06 \x01(\x0e\x32>.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio.AudioCodec\x12S\n\x08metadata\x18\x07 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"#\n\nAudioCodec\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04\x46LAC\x10\x01\x1a\x9c\x02\n\x06Single\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12:\n\x07samples\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12J\n\x08metadata\x18\x04 \x03(\x0b\x32\x38.redvox_api_m.RedvoxPacketM.Sensors.Single.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd6\x18\n\x08Location\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12\x41\n\x0etimestamps_gps\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12I\n\x10latitude_samples\x18\x04 \x01(\x0b\x32/.redvox_api_m.RedvoxPacketM.DoubleSamplePayload\x12J\n\x11longitude_samples\x18\x05 \x01(\x0b\x32/.redvox_api_m.RedvoxPacketM.DoubleSamplePayload\x12\x43\n\x10\x61ltitude_samples\x18\x06 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12@\n\rspeed_samples\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x62\x65\x61ring_samples\x18\x08 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12N\n\x1bhorizontal_accuracy_samples\x18\t \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12L\n\x19vertical_accuracy_samples\x18\n \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12I\n\x16speed_accuracy_samples\x18\x0b \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12K\n\x18\x62\x65\x61ring_accuracy_samples\x18\x0c \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12U\n\x12last_best_location\x18\r \x01(\x0b\x32\x39.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation\x12X\n\x15overall_best_location\x18\x0e \x01(\x0b\x32\x39.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation\x12$\n\x1clocation_permissions_granted\x18\x0f \x01(\x08\x12#\n\x1blocation_services_requested\x18\x10 \x01(\x08\x12!\n\x19location_services_enabled\x18\x11 \x01(\x08\x12Y\n\x12location_providers\x18\x12 \x03(\x0e\x32=.redvox_api_m.RedvoxPacketM.Sensors.Location.LocationProvider\x12L\n\x08metadata\x18\x13 \x03(\x0b\x32:.redvox_api_m.RedvoxPacketM.Sensors.Location.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xcf\r\n\x0c\x42\x65stLocation\x12m\n\x1clatitude_longitude_timestamp\x18\x01 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x63\n\x12\x61ltitude_timestamp\x18\x02 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12`\n\x0fspeed_timestamp\x18\x03 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x62\n\x11\x62\x65\x61ring_timestamp\x18\x04 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x41\n\x17latitude_longitude_unit\x18\x05 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x37\n\raltitude_unit\x18\x06 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x34\n\nspeed_unit\x18\x07 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x36\n\x0c\x62\x65\x61ring_unit\x18\x08 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12@\n\x16vertical_accuracy_unit\x18\t \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x42\n\x18horizontal_accuracy_unit\x18\n \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12=\n\x13speed_accuracy_unit\x18\x0b \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12?\n\x15\x62\x65\x61ring_accuracy_unit\x18\x0c \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x10\n\x08latitude\x18\r \x01(\x01\x12\x11\n\tlongitude\x18\x0e \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x0f \x01(\x02\x12\r\n\x05speed\x18\x10 \x01(\x02\x12\x0f\n\x07\x62\x65\x61ring\x18\x11 \x01(\x02\x12\x19\n\x11vertical_accuracy\x18\x12 \x01(\x02\x12\x1b\n\x13horizontal_accuracy\x18\x13 \x01(\x02\x12\x16\n\x0espeed_accuracy\x18\x14 \x01(\x02\x12\x18\n\x10\x62\x65\x61ring_accuracy\x18\x15 \x01(\x02\x12\r\n\x05score\x18\x16 \x01(\x02\x12]\n\x06method\x18\x17 \x01(\x0e\x32M.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.LocationScoreMethod\x12X\n\x11location_provider\x18\x18 \x01(\x0e\x32=.redvox_api_m.RedvoxPacketM.Sensors.Location.LocationProvider\x12Y\n\x08metadata\x18\x19 \x03(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf4\x01\n\rBestTimestamp\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0c\n\x04mach\x18\x02 \x01(\x01\x12\x0b\n\x03gps\x18\x03 \x01(\x01\x12g\n\x08metadata\x18\x04 \x03(\x0b\x32U.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\")\n\x13LocationScoreMethod\x12\x12\n\x0eUNKNOWN_METHOD\x10\x00\"I\n\x10LocationProvider\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\x08\n\x04USER\x10\x02\x12\x07\n\x03GPS\x10\x03\x12\x0b\n\x07NETWORK\x10\x04\x1a\x94\x03\n\x03Xyz\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12<\n\tx_samples\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12<\n\ty_samples\x18\x04 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12<\n\tz_samples\x18\x05 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12G\n\x08metadata\x18\x06 \x03(\x0b\x32\x35.redvox_api_m.RedvoxPacketM.Sensors.Xyz.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf0\x02\n\x05Image\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12\x0f\n\x07samples\x18\x03 \x03(\x0c\x12I\n\x0bimage_codec\x18\x04 \x01(\x0e\x32\x34.redvox_api_m.RedvoxPacketM.Sensors.Image.ImageCodec\x12I\n\x08metadata\x18\x05 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.Sensors.Image.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"4\n\nImageCodec\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03PNG\x10\x01\x12\x07\n\x03JPG\x10\x02\x12\x07\n\x03\x42MP\x10\x03\x1a\xf2\x07\n\x0b\x45ventStream\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12=\n\x06\x65vents\x18\x03 \x03(\x0b\x32-.redvox_api_m.RedvoxPacketM.EventStream.Event\x12G\n\x08metadata\x18\x04 \x03(\x0b\x32\x35.redvox_api_m.RedvoxPacketM.EventStream.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xdc\x05\n\x05\x45vent\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12X\n\x0estring_payload\x18\x02 \x03(\x0b\x32@.redvox_api_m.RedvoxPacketM.EventStream.Event.StringPayloadEntry\x12Z\n\x0fnumeric_payload\x18\x03 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.EventStream.Event.NumericPayloadEntry\x12Z\n\x0f\x62oolean_payload\x18\x04 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.EventStream.Event.BooleanPayloadEntry\x12T\n\x0c\x62yte_payload\x18\x05 \x03(\x0b\x32>.redvox_api_m.RedvoxPacketM.EventStream.Event.BytePayloadEntry\x12M\n\x08metadata\x18\x06 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.EventStream.Event.MetadataEntry\x1a\x34\n\x12StringPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x35\n\x13NumericPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\x1a\x35\n\x13\x42ooleanPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\x1a\x32\n\x10\x42ytePayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x94\x02\n\rSamplePayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0e\n\x06values\x18\x02 \x03(\x02\x12G\n\x10value_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12I\n\x08metadata\x18\x04 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.SamplePayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xa0\x02\n\x13\x44oubleSamplePayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0e\n\x06values\x18\x02 \x03(\x01\x12G\n\x10value_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12O\n\x08metadata\x18\x04 \x03(\x0b\x32=.redvox_api_m.RedvoxPacketM.DoubleSamplePayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd1\x02\n\rTimingPayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x12\n\ntimestamps\x18\x02 \x03(\x01\x12K\n\x14timestamp_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12\x18\n\x10mean_sample_rate\x18\x04 \x01(\x02\x12\x19\n\x11stdev_sample_rate\x18\x05 \x01(\x02\x12I\n\x08metadata\x18\x06 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.TimingPayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf5\x01\n\x11SummaryStatistics\x12\r\n\x05\x63ount\x18\x01 \x01(\x01\x12\x0c\n\x04mean\x18\x02 \x01(\x01\x12\x1a\n\x12standard_deviation\x18\x03 \x01(\x01\x12\x0b\n\x03min\x18\x04 \x01(\x01\x12\x0b\n\x03max\x18\x05 \x01(\x01\x12\r\n\x05range\x18\x06 \x01(\x01\x12M\n\x08metadata\x18\x07 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.SummaryStatistics.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x03\n\x04Unit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x1d\n\x19METERS_PER_SECOND_SQUARED\x10\x01\x12\x0e\n\nKILOPASCAL\x10\x02\x12\x16\n\x12RADIANS_PER_SECOND\x10\x03\x12\x13\n\x0f\x44\x45\x43IMAL_DEGREES\x10\x04\x12\n\n\x06METERS\x10\x05\x12\x15\n\x11METERS_PER_SECOND\x10\x06\x12\x0e\n\nMICROTESLA\x10\x07\x12\x19\n\x15LSB_PLUS_MINUS_COUNTS\x10\x08\x12!\n\x1dMICROSECONDS_SINCE_UNIX_EPOCH\x10\t\x12\x0b\n\x07\x44\x45\x43IBEL\x10\n\x12\x13\n\x0f\x44\x45GREES_CELSIUS\x10\x0b\x12\x08\n\x04\x42YTE\x10\x0c\x12\x0e\n\nPERCENTAGE\x10\r\x12\x0b\n\x07RADIANS\x10\x0e\x12\x10\n\x0cMICROAMPERES\x10\x0f\x12\x0f\n\x0b\x43\x45NTIMETERS\x10\x10\x12\x15\n\x11NORMALIZED_COUNTS\x10\x11\x12\x07\n\x03LUX\x10\x12\x12\x0c\n\x08UNITLESS\x10\x13\x12\x07\n\x03PCM\x10\x14\"\xac\x01\n\x16\x45ncryptedRedvoxPacketM\x12\x0e\n\x06header\x18\x01 \x01(\x0c\x12\x0e\n\x06packet\x18\x02 \x01(\x0c\x1ar\n\x06Header\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x12\n\nauth_token\x18\x03 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x04 \x01(\t\x12\x12\n\nauth_email\x18\x05 \x01(\t\"\x89\x01\n\x12\x41\x63quisitionRequest\x12\x12\n\nauth_token\x18\x01 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x02 \x01(\t\x12\x10\n\x08\x63hecksum\x18\x03 \x01(\x03\x12\x14\n\x0cis_encrypted\x18\x04 \x01(\x08\x12\x0f\n\x07payload\x18\x05 \x01(\x0c\x12\x0e\n\x06seq_id\x18\x06 \x01(\x03\"\xf5\x01\n\x13\x41\x63quisitionResponse\x12\x45\n\rresponse_type\x18\x01 \x01(\x0e\x32..redvox_api_m.AcquisitionResponse.ResponseType\x12\x10\n\x08\x63hecksum\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\x12\x0e\n\x06resend\x18\x04 \x01(\x08\x12\x0e\n\x06seq_id\x18\x05 \x01(\x03\"T\n\x0cResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02OK\x10\x01\x12\x0e\n\nAUTH_ERROR\x10\x02\x12\x0e\n\nDATA_ERROR\x10\x03\x12\x0f\n\x0bOTHER_ERROR\x10\x04\"\\\n\x0cSynchRequest\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x0e\n\x06seq_id\x18\x03 \x01(\r\x12\x12\n\nsub_seq_id\x18\x04 \x01(\r\"\x85\x01\n\rSynchResponse\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x0e\n\x06seq_id\x18\x03 \x01(\r\x12\x12\n\nsub_seq_id\x18\x04 \x01(\r\x12\x12\n\nrecv_ts_us\x18\x05 \x01(\x04\x12\x12\n\nsend_ts_us\x18\x06 \x01(\x04\x42\x10\n\x0eio.redvox.apisb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'src.redvox_api_m.redvox_api_m_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'redvox_api_m_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016io.redvox.apis'
   _REDVOXPACKETM_METADATAENTRY._options = None
   _REDVOXPACKETM_METADATAENTRY._serialized_options = b'8\001'
   _REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY._options = None
@@ -71,152 +72,152 @@
   _REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY._serialized_options = b'8\001'
   _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY._options = None
   _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY._serialized_options = b'8\001'
   _REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY._options = None
   _REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY._serialized_options = b'8\001'
   _REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY._options = None
   _REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY._serialized_options = b'8\001'
-  _REDVOXPACKETM._serialized_start=54
-  _REDVOXPACKETM._serialized_end=14882
-  _REDVOXPACKETM_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_STATIONINFORMATION._serialized_start=482
-  _REDVOXPACKETM_STATIONINFORMATION._serialized_end=5171
-  _REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS._serialized_start=1107
-  _REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS._serialized_end=1332
-  _REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS._serialized_start=1335
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS._serialized_end=2992
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_NETWORKTYPE._serialized_start=2589
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_NETWORKTYPE._serialized_end=2674
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_WIFIWAKELOCK._serialized_start=2676
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_WIFIWAKELOCK._serialized_end=2743
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_CELLSERVICESTATE._serialized_start=2745
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_CELLSERVICESTATE._serialized_end=2839
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_POWERSTATE._serialized_start=2841
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_POWERSTATE._serialized_end=2920
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_SCREENSTATE._serialized_start=2922
-  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_SCREENSTATE._serialized_end=2992
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS._serialized_start=2995
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS._serialized_end=5020
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_FFTOVERLAP._serialized_start=4307
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_FFTOVERLAP._serialized_end=4380
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSAMPLINGRATE._serialized_start=4382
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSAMPLINGRATE._serialized_end=4492
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSOURCETUNING._serialized_start=4494
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSOURCETUNING._serialized_end=4596
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_INPUTSENSOR._serialized_start=4599
-  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_INPUTSENSOR._serialized_end=5020
-  _REDVOXPACKETM_STATIONINFORMATION_OSTYPE._serialized_start=5022
-  _REDVOXPACKETM_STATIONINFORMATION_OSTYPE._serialized_end=5101
-  _REDVOXPACKETM_STATIONINFORMATION_METRICSRATE._serialized_start=5103
-  _REDVOXPACKETM_STATIONINFORMATION_METRICSRATE._serialized_end=5171
-  _REDVOXPACKETM_TIMINGINFORMATION._serialized_start=5174
-  _REDVOXPACKETM_TIMINGINFORMATION._serialized_end=6134
-  _REDVOXPACKETM_TIMINGINFORMATION_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_TIMINGINFORMATION_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE._serialized_start=5823
-  _REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE._serialized_end=6100
-  _REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_TIMINGINFORMATION_TIMINGSCOREMETHOD._serialized_start=6102
-  _REDVOXPACKETM_TIMINGINFORMATION_TIMINGSCOREMETHOD._serialized_end=6134
-  _REDVOXPACKETM_SENSORS._serialized_start=6137
-  _REDVOXPACKETM_SENSORS._serialized_end=12321
-  _REDVOXPACKETM_SENSORS_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_AUDIO._serialized_start=7356
-  _REDVOXPACKETM_SENSORS_AUDIO._serialized_end=7695
-  _REDVOXPACKETM_SENSORS_AUDIO_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_AUDIO_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO._serialized_start=7698
-  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO._serialized_end=8095
-  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_AUDIOCODEC._serialized_start=8060
-  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_AUDIOCODEC._serialized_end=8095
-  _REDVOXPACKETM_SENSORS_SINGLE._serialized_start=8098
-  _REDVOXPACKETM_SENSORS_SINGLE._serialized_end=8382
-  _REDVOXPACKETM_SENSORS_SINGLE_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_SINGLE_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_LOCATION._serialized_start=8385
-  _REDVOXPACKETM_SENSORS_LOCATION._serialized_end=11543
-  _REDVOXPACKETM_SENSORS_LOCATION_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_LOCATION_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION._serialized_start=9725
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION._serialized_end=11468
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP._serialized_start=11181
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP._serialized_end=11425
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_LOCATIONSCOREMETHOD._serialized_start=11427
-  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_LOCATIONSCOREMETHOD._serialized_end=11468
-  _REDVOXPACKETM_SENSORS_LOCATION_LOCATIONPROVIDER._serialized_start=11470
-  _REDVOXPACKETM_SENSORS_LOCATION_LOCATIONPROVIDER._serialized_end=11543
-  _REDVOXPACKETM_SENSORS_XYZ._serialized_start=11546
-  _REDVOXPACKETM_SENSORS_XYZ._serialized_end=11950
-  _REDVOXPACKETM_SENSORS_XYZ_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_XYZ_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_IMAGE._serialized_start=11953
-  _REDVOXPACKETM_SENSORS_IMAGE._serialized_end=12321
-  _REDVOXPACKETM_SENSORS_IMAGE_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SENSORS_IMAGE_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SENSORS_IMAGE_IMAGECODEC._serialized_start=12269
-  _REDVOXPACKETM_SENSORS_IMAGE_IMAGECODEC._serialized_end=12321
-  _REDVOXPACKETM_EVENTSTREAM._serialized_start=12324
-  _REDVOXPACKETM_EVENTSTREAM._serialized_end=13334
-  _REDVOXPACKETM_EVENTSTREAM_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_EVENTSTREAM_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_EVENTSTREAM_EVENT._serialized_start=12602
-  _REDVOXPACKETM_EVENTSTREAM_EVENT._serialized_end=13334
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_STRINGPAYLOADENTRY._serialized_start=13071
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_STRINGPAYLOADENTRY._serialized_end=13123
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_NUMERICPAYLOADENTRY._serialized_start=13125
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_NUMERICPAYLOADENTRY._serialized_end=13178
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_BOOLEANPAYLOADENTRY._serialized_start=13180
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_BOOLEANPAYLOADENTRY._serialized_end=13233
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_BYTEPAYLOADENTRY._serialized_start=13235
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_BYTEPAYLOADENTRY._serialized_end=13285
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_EVENTSTREAM_EVENT_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SAMPLEPAYLOAD._serialized_start=13337
-  _REDVOXPACKETM_SAMPLEPAYLOAD._serialized_end=13613
-  _REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD._serialized_start=13616
-  _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD._serialized_end=13904
-  _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_TIMINGPAYLOAD._serialized_start=13907
-  _REDVOXPACKETM_TIMINGPAYLOAD._serialized_end=14244
-  _REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_SUMMARYSTATISTICS._serialized_start=14247
-  _REDVOXPACKETM_SUMMARYSTATISTICS._serialized_end=14492
-  _REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY._serialized_start=432
-  _REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY._serialized_end=479
-  _REDVOXPACKETM_UNIT._serialized_start=14495
-  _REDVOXPACKETM_UNIT._serialized_end=14882
-  _ENCRYPTEDREDVOXPACKETM._serialized_start=14885
-  _ENCRYPTEDREDVOXPACKETM._serialized_end=15057
-  _ENCRYPTEDREDVOXPACKETM_HEADER._serialized_start=14943
-  _ENCRYPTEDREDVOXPACKETM_HEADER._serialized_end=15057
-  _ACQUISITIONREQUEST._serialized_start=15060
-  _ACQUISITIONREQUEST._serialized_end=15197
-  _ACQUISITIONRESPONSE._serialized_start=15200
-  _ACQUISITIONRESPONSE._serialized_end=15445
-  _ACQUISITIONRESPONSE_RESPONSETYPE._serialized_start=15361
-  _ACQUISITIONRESPONSE_RESPONSETYPE._serialized_end=15445
-  _SYNCHREQUEST._serialized_start=15447
-  _SYNCHREQUEST._serialized_end=15539
-  _SYNCHRESPONSE._serialized_start=15542
-  _SYNCHRESPONSE._serialized_end=15675
+  _globals['_REDVOXPACKETM']._serialized_start=37
+  _globals['_REDVOXPACKETM']._serialized_end=14865
+  _globals['_REDVOXPACKETM_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_STATIONINFORMATION']._serialized_start=465
+  _globals['_REDVOXPACKETM_STATIONINFORMATION']._serialized_end=5154
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS']._serialized_start=1090
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS']._serialized_end=1315
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS']._serialized_start=1318
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS']._serialized_end=2975
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_NETWORKTYPE']._serialized_start=2572
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_NETWORKTYPE']._serialized_end=2657
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_WIFIWAKELOCK']._serialized_start=2659
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_WIFIWAKELOCK']._serialized_end=2726
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_CELLSERVICESTATE']._serialized_start=2728
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_CELLSERVICESTATE']._serialized_end=2822
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_POWERSTATE']._serialized_start=2824
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_POWERSTATE']._serialized_end=2903
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_SCREENSTATE']._serialized_start=2905
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_SCREENSTATE']._serialized_end=2975
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS']._serialized_start=2978
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS']._serialized_end=5003
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_FFTOVERLAP']._serialized_start=4290
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_FFTOVERLAP']._serialized_end=4363
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSAMPLINGRATE']._serialized_start=4365
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSAMPLINGRATE']._serialized_end=4475
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSOURCETUNING']._serialized_start=4477
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSOURCETUNING']._serialized_end=4579
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_INPUTSENSOR']._serialized_start=4582
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_INPUTSENSOR']._serialized_end=5003
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_OSTYPE']._serialized_start=5005
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_OSTYPE']._serialized_end=5084
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_METRICSRATE']._serialized_start=5086
+  _globals['_REDVOXPACKETM_STATIONINFORMATION_METRICSRATE']._serialized_end=5154
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION']._serialized_start=5157
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION']._serialized_end=6117
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE']._serialized_start=5806
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE']._serialized_end=6083
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION_TIMINGSCOREMETHOD']._serialized_start=6085
+  _globals['_REDVOXPACKETM_TIMINGINFORMATION_TIMINGSCOREMETHOD']._serialized_end=6117
+  _globals['_REDVOXPACKETM_SENSORS']._serialized_start=6120
+  _globals['_REDVOXPACKETM_SENSORS']._serialized_end=12304
+  _globals['_REDVOXPACKETM_SENSORS_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_AUDIO']._serialized_start=7339
+  _globals['_REDVOXPACKETM_SENSORS_AUDIO']._serialized_end=7678
+  _globals['_REDVOXPACKETM_SENSORS_AUDIO_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_AUDIO_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO']._serialized_start=7681
+  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO']._serialized_end=8078
+  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_AUDIOCODEC']._serialized_start=8043
+  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_AUDIOCODEC']._serialized_end=8078
+  _globals['_REDVOXPACKETM_SENSORS_SINGLE']._serialized_start=8081
+  _globals['_REDVOXPACKETM_SENSORS_SINGLE']._serialized_end=8365
+  _globals['_REDVOXPACKETM_SENSORS_SINGLE_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_SINGLE_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION']._serialized_start=8368
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION']._serialized_end=11526
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION']._serialized_start=9708
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION']._serialized_end=11451
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP']._serialized_start=11164
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP']._serialized_end=11408
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_LOCATIONSCOREMETHOD']._serialized_start=11410
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_LOCATIONSCOREMETHOD']._serialized_end=11451
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_LOCATIONPROVIDER']._serialized_start=11453
+  _globals['_REDVOXPACKETM_SENSORS_LOCATION_LOCATIONPROVIDER']._serialized_end=11526
+  _globals['_REDVOXPACKETM_SENSORS_XYZ']._serialized_start=11529
+  _globals['_REDVOXPACKETM_SENSORS_XYZ']._serialized_end=11933
+  _globals['_REDVOXPACKETM_SENSORS_XYZ_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_XYZ_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_IMAGE']._serialized_start=11936
+  _globals['_REDVOXPACKETM_SENSORS_IMAGE']._serialized_end=12304
+  _globals['_REDVOXPACKETM_SENSORS_IMAGE_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SENSORS_IMAGE_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SENSORS_IMAGE_IMAGECODEC']._serialized_start=12252
+  _globals['_REDVOXPACKETM_SENSORS_IMAGE_IMAGECODEC']._serialized_end=12304
+  _globals['_REDVOXPACKETM_EVENTSTREAM']._serialized_start=12307
+  _globals['_REDVOXPACKETM_EVENTSTREAM']._serialized_end=13317
+  _globals['_REDVOXPACKETM_EVENTSTREAM_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_EVENTSTREAM_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT']._serialized_start=12585
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT']._serialized_end=13317
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_STRINGPAYLOADENTRY']._serialized_start=13054
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_STRINGPAYLOADENTRY']._serialized_end=13106
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_NUMERICPAYLOADENTRY']._serialized_start=13108
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_NUMERICPAYLOADENTRY']._serialized_end=13161
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_BOOLEANPAYLOADENTRY']._serialized_start=13163
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_BOOLEANPAYLOADENTRY']._serialized_end=13216
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_BYTEPAYLOADENTRY']._serialized_start=13218
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_BYTEPAYLOADENTRY']._serialized_end=13268
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SAMPLEPAYLOAD']._serialized_start=13320
+  _globals['_REDVOXPACKETM_SAMPLEPAYLOAD']._serialized_end=13596
+  _globals['_REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_DOUBLESAMPLEPAYLOAD']._serialized_start=13599
+  _globals['_REDVOXPACKETM_DOUBLESAMPLEPAYLOAD']._serialized_end=13887
+  _globals['_REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_TIMINGPAYLOAD']._serialized_start=13890
+  _globals['_REDVOXPACKETM_TIMINGPAYLOAD']._serialized_end=14227
+  _globals['_REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_SUMMARYSTATISTICS']._serialized_start=14230
+  _globals['_REDVOXPACKETM_SUMMARYSTATISTICS']._serialized_end=14475
+  _globals['_REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY']._serialized_start=415
+  _globals['_REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY']._serialized_end=462
+  _globals['_REDVOXPACKETM_UNIT']._serialized_start=14478
+  _globals['_REDVOXPACKETM_UNIT']._serialized_end=14865
+  _globals['_ENCRYPTEDREDVOXPACKETM']._serialized_start=14868
+  _globals['_ENCRYPTEDREDVOXPACKETM']._serialized_end=15040
+  _globals['_ENCRYPTEDREDVOXPACKETM_HEADER']._serialized_start=14926
+  _globals['_ENCRYPTEDREDVOXPACKETM_HEADER']._serialized_end=15040
+  _globals['_ACQUISITIONREQUEST']._serialized_start=15043
+  _globals['_ACQUISITIONREQUEST']._serialized_end=15180
+  _globals['_ACQUISITIONRESPONSE']._serialized_start=15183
+  _globals['_ACQUISITIONRESPONSE']._serialized_end=15428
+  _globals['_ACQUISITIONRESPONSE_RESPONSETYPE']._serialized_start=15344
+  _globals['_ACQUISITIONRESPONSE_RESPONSETYPE']._serialized_end=15428
+  _globals['_SYNCHREQUEST']._serialized_start=15430
+  _globals['_SYNCHREQUEST']._serialized_end=15522
+  _globals['_SYNCHRESPONSE']._serialized_start=15525
+  _globals['_SYNCHRESPONSE']._serialized_end=15658
 # @@protoc_insertion_point(module_scope)
```

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/event_streams.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/event_streams.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/audio.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/audio.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/image.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/image.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/location.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/location.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/single.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/single.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/station_information.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/station_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/timing_information.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/timing_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py` & `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/concat.py` & `redvox-3.4.0a3/redvox/api900/concat.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/deprecation.py` & `redvox-3.4.0a3/redvox/api900/deprecation.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/lib/api900_pb2.py` & `redvox-3.4.0a3/redvox/api900/lib/api900_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,44 +11,45 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x61pi900.proto\"\xf5\x05\n\x0cRedvoxPacket\x12\x0b\n\x03\x61pi\x18\x01 \x01(\r\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x11\n\tredvox_id\x18\x03 \x01(\t\x12\x1b\n\x13\x61uthenticated_email\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x17 \x01(\t\x12\x15\n\ris_backfilled\x18\x06 \x01(\x08\x12\x12\n\nis_private\x18\x07 \x01(\x08\x12\x14\n\x0cis_scrambled\x18\x08 \x01(\x08\x12\x13\n\x0b\x64\x65vice_make\x18\t \x01(\t\x12\x14\n\x0c\x64\x65vice_model\x18\n \x01(\t\x12\x11\n\tdevice_os\x18\x0b \x01(\t\x12\x19\n\x11\x64\x65vice_os_version\x18\x0c \x01(\t\x12\x13\n\x0b\x61pp_version\x18\r \x01(\t\x12\x1d\n\x15\x62\x61ttery_level_percent\x18\x18 \x01(\x02\x12\x1c\n\x14\x64\x65vice_temperature_c\x18\x19 \x01(\x02\x12\x1a\n\x12\x61\x63quisition_server\x18\x0e \x01(\t\x12#\n\x1btime_synchronization_server\x18\x0f \x01(\t\x12\x1d\n\x15\x61uthentication_server\x18\x10 \x01(\t\x12\x37\n/app_file_start_timestamp_epoch_microseconds_utc\x18\x11 \x01(\x03\x12(\n app_file_start_timestamp_machine\x18\x12 \x01(\x03\x12/\n\'server_timestamp_epoch_microseconds_utc\x18\x13 \x01(\x03\x12\x36\n\x17\x65venly_sampled_channels\x18\x14 \x03(\x0b\x32\x15.EvenlySampledChannel\x12:\n\x19unevenly_sampled_channels\x18\x15 \x03(\x0b\x32\x17.UnevenlySampledChannel\x12\x10\n\x08metadata\x18\x16 \x03(\t\"\x1f\n\x0cInt32Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x05\" \n\rUInt32Payload\x12\x0f\n\x07payload\x18\x01 \x03(\r\"\x1f\n\x0cInt64Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x03\" \n\rUInt64Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x04\"!\n\x0e\x46loat32Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x02\"!\n\x0e\x46loat64Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x01\"\x8c\x02\n\x0b\x42ytePayload\x12\x35\n\x0f\x62ytePayloadType\x18\x01 \x01(\x0e\x32\x1c.BytePayload.BytePayloadType\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"\xb4\x01\n\x0f\x42ytePayloadType\x12\t\n\x05\x42YTES\x10\x00\x12\t\n\x05UINT8\x10\x01\x12\x0b\n\x07UNINT16\x10\x02\x12\x0b\n\x07UNINT24\x10\x03\x12\n\n\x06UINT32\x10\x04\x12\n\n\x06UINT64\x10\x05\x12\x08\n\x04INT8\x10\x06\x12\t\n\x05INT16\x10\x07\x12\t\n\x05INT24\x10\x08\x12\t\n\x05INT32\x10\t\x12\t\n\x05INT64\x10\n\x12\x0b\n\x07\x46LOAT32\x10\x0b\x12\x0b\n\x07\x46LOAT64\x10\x0c\x12\t\n\x05OTHER\x10\r\"\x9e\x04\n\x14\x45venlySampledChannel\x12#\n\rchannel_types\x18\x01 \x03(\x0e\x32\x0c.ChannelType\x12\x13\n\x0bsensor_name\x18\x02 \x01(\t\x12\x16\n\x0esample_rate_hz\x18\x03 \x01(\x01\x12\x35\n-first_sample_timestamp_epoch_microseconds_utc\x18\x04 \x01(\x03\x12$\n\x0c\x62yte_payload\x18\x05 \x01(\x0b\x32\x0c.BytePayloadH\x00\x12(\n\x0euint32_payload\x18\x06 \x01(\x0b\x32\x0e.UInt32PayloadH\x00\x12(\n\x0euint64_payload\x18\x07 \x01(\x0b\x32\x0e.UInt64PayloadH\x00\x12&\n\rint32_payload\x18\x08 \x01(\x0b\x32\r.Int32PayloadH\x00\x12&\n\rint64_payload\x18\t \x01(\x0b\x32\r.Int64PayloadH\x00\x12*\n\x0f\x66loat32_payload\x18\n \x01(\x0b\x32\x0f.Float32PayloadH\x00\x12*\n\x0f\x66loat64_payload\x18\x0b \x01(\x0b\x32\x0f.Float64PayloadH\x00\x12\x13\n\x0bvalue_means\x18\x0c \x03(\x01\x12\x12\n\nvalue_stds\x18\r \x03(\x01\x12\x15\n\rvalue_medians\x18\x0e \x03(\x01\x12\x10\n\x08metadata\x18\x0f \x03(\tB\t\n\x07payload\"\xd1\x04\n\x16UnevenlySampledChannel\x12#\n\rchannel_types\x18\x01 \x03(\x0e\x32\x0c.ChannelType\x12\x13\n\x0bsensor_name\x18\x02 \x01(\t\x12#\n\x1btimestamps_microseconds_utc\x18\x03 \x03(\x03\x12$\n\x0c\x62yte_payload\x18\x04 \x01(\x0b\x32\x0c.BytePayloadH\x00\x12(\n\x0euint32_payload\x18\x05 \x01(\x0b\x32\x0e.UInt32PayloadH\x00\x12(\n\x0euint64_payload\x18\x06 \x01(\x0b\x32\x0e.UInt64PayloadH\x00\x12&\n\rint32_payload\x18\x07 \x01(\x0b\x32\r.Int32PayloadH\x00\x12&\n\rint64_payload\x18\x08 \x01(\x0b\x32\r.Int64PayloadH\x00\x12*\n\x0f\x66loat32_payload\x18\t \x01(\x0b\x32\x0f.Float32PayloadH\x00\x12*\n\x0f\x66loat64_payload\x18\n \x01(\x0b\x32\x0f.Float64PayloadH\x00\x12\x1c\n\x14sample_interval_mean\x18\x0b \x01(\x01\x12\x1b\n\x13sample_interval_std\x18\x0c \x01(\x01\x12\x1e\n\x16sample_interval_median\x18\r \x01(\x01\x12\x13\n\x0bvalue_means\x18\x0e \x03(\x01\x12\x12\n\nvalue_stds\x18\x0f \x03(\x01\x12\x15\n\rvalue_medians\x18\x10 \x03(\x01\x12\x10\n\x08metadata\x18\x11 \x03(\tB\t\n\x07payload\"\xd7\x01\n\x14RedvoxPacketResponse\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.RedvoxPacketResponse.Type\x12\x10\n\x08\x63hecksum\x18\x02 \x01(\x03\x12+\n\x06\x65rrors\x18\x03 \x03(\x0e\x32\x1b.RedvoxPacketResponse.Error\x12\x10\n\x08metadata\x18\x04 \x03(\t\"\x19\n\x04Type\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\")\n\x05\x45rror\x12\x15\n\x11NOT_AUTHENTICATED\x10\x00\x12\t\n\x05OTHER\x10\x01*\x97\x03\n\x0b\x43hannelType\x12\x0e\n\nMICROPHONE\x10\x00\x12\r\n\tBAROMETER\x10\x01\x12\x0c\n\x08LATITUDE\x10\x02\x12\r\n\tLONGITUDE\x10\x03\x12\t\n\x05SPEED\x10\x04\x12\x0c\n\x08\x41LTITUDE\x10\x05\x12\x0e\n\nRESERVED_0\x10\x06\x12\x0e\n\nRESERVED_1\x10\x07\x12\x0e\n\nRESERVED_2\x10\x08\x12\x18\n\x14TIME_SYNCHRONIZATION\x10\t\x12\x0c\n\x08\x41\x43\x43URACY\x10\n\x12\x13\n\x0f\x41\x43\x43\x45LEROMETER_X\x10\x0b\x12\x13\n\x0f\x41\x43\x43\x45LEROMETER_Y\x10\x0c\x12\x13\n\x0f\x41\x43\x43\x45LEROMETER_Z\x10\r\x12\x12\n\x0eMAGNETOMETER_X\x10\x0e\x12\x12\n\x0eMAGNETOMETER_Y\x10\x0f\x12\x12\n\x0eMAGNETOMETER_Z\x10\x10\x12\x0f\n\x0bGYROSCOPE_X\x10\x11\x12\x0f\n\x0bGYROSCOPE_Y\x10\x12\x12\x0f\n\x0bGYROSCOPE_Z\x10\x13\x12\t\n\x05OTHER\x10\x14\x12\t\n\x05LIGHT\x10\x15\x12\t\n\x05IMAGE\x10\x16\x12\x0c\n\x08INFRARED\x10\x17\x42\x10\n\x0eio.redvox.apisb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api900_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api900_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016io.redvox.apis'
-  _CHANNELTYPE._serialized_start=2611
-  _CHANNELTYPE._serialized_end=3018
-  _REDVOXPACKET._serialized_start=17
-  _REDVOXPACKET._serialized_end=774
-  _INT32PAYLOAD._serialized_start=776
-  _INT32PAYLOAD._serialized_end=807
-  _UINT32PAYLOAD._serialized_start=809
-  _UINT32PAYLOAD._serialized_end=841
-  _INT64PAYLOAD._serialized_start=843
-  _INT64PAYLOAD._serialized_end=874
-  _UINT64PAYLOAD._serialized_start=876
-  _UINT64PAYLOAD._serialized_end=908
-  _FLOAT32PAYLOAD._serialized_start=910
-  _FLOAT32PAYLOAD._serialized_end=943
-  _FLOAT64PAYLOAD._serialized_start=945
-  _FLOAT64PAYLOAD._serialized_end=978
-  _BYTEPAYLOAD._serialized_start=981
-  _BYTEPAYLOAD._serialized_end=1249
-  _BYTEPAYLOAD_BYTEPAYLOADTYPE._serialized_start=1069
-  _BYTEPAYLOAD_BYTEPAYLOADTYPE._serialized_end=1249
-  _EVENLYSAMPLEDCHANNEL._serialized_start=1252
-  _EVENLYSAMPLEDCHANNEL._serialized_end=1794
-  _UNEVENLYSAMPLEDCHANNEL._serialized_start=1797
-  _UNEVENLYSAMPLEDCHANNEL._serialized_end=2390
-  _REDVOXPACKETRESPONSE._serialized_start=2393
-  _REDVOXPACKETRESPONSE._serialized_end=2608
-  _REDVOXPACKETRESPONSE_TYPE._serialized_start=2540
-  _REDVOXPACKETRESPONSE_TYPE._serialized_end=2565
-  _REDVOXPACKETRESPONSE_ERROR._serialized_start=2567
-  _REDVOXPACKETRESPONSE_ERROR._serialized_end=2608
+  _globals['_CHANNELTYPE']._serialized_start=2611
+  _globals['_CHANNELTYPE']._serialized_end=3018
+  _globals['_REDVOXPACKET']._serialized_start=17
+  _globals['_REDVOXPACKET']._serialized_end=774
+  _globals['_INT32PAYLOAD']._serialized_start=776
+  _globals['_INT32PAYLOAD']._serialized_end=807
+  _globals['_UINT32PAYLOAD']._serialized_start=809
+  _globals['_UINT32PAYLOAD']._serialized_end=841
+  _globals['_INT64PAYLOAD']._serialized_start=843
+  _globals['_INT64PAYLOAD']._serialized_end=874
+  _globals['_UINT64PAYLOAD']._serialized_start=876
+  _globals['_UINT64PAYLOAD']._serialized_end=908
+  _globals['_FLOAT32PAYLOAD']._serialized_start=910
+  _globals['_FLOAT32PAYLOAD']._serialized_end=943
+  _globals['_FLOAT64PAYLOAD']._serialized_start=945
+  _globals['_FLOAT64PAYLOAD']._serialized_end=978
+  _globals['_BYTEPAYLOAD']._serialized_start=981
+  _globals['_BYTEPAYLOAD']._serialized_end=1249
+  _globals['_BYTEPAYLOAD_BYTEPAYLOADTYPE']._serialized_start=1069
+  _globals['_BYTEPAYLOAD_BYTEPAYLOADTYPE']._serialized_end=1249
+  _globals['_EVENLYSAMPLEDCHANNEL']._serialized_start=1252
+  _globals['_EVENLYSAMPLEDCHANNEL']._serialized_end=1794
+  _globals['_UNEVENLYSAMPLEDCHANNEL']._serialized_start=1797
+  _globals['_UNEVENLYSAMPLEDCHANNEL']._serialized_end=2390
+  _globals['_REDVOXPACKETRESPONSE']._serialized_start=2393
+  _globals['_REDVOXPACKETRESPONSE']._serialized_end=2608
+  _globals['_REDVOXPACKETRESPONSE_TYPE']._serialized_start=2540
+  _globals['_REDVOXPACKETRESPONSE_TYPE']._serialized_end=2565
+  _globals['_REDVOXPACKETRESPONSE_ERROR']._serialized_start=2567
+  _globals['_REDVOXPACKETRESPONSE_ERROR']._serialized_end=2608
 # @@protoc_insertion_point(module_scope)
```

### Comparing `redvox-3.4.0a2/redvox/api900/location_analyzer.py` & `redvox-3.4.0a3/redvox/api900/location_analyzer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/migrations.py` & `redvox-3.4.0a3/redvox/api900/migrations.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/qa/gap_detection.py` & `redvox-3.4.0a3/redvox/api900/qa/gap_detection.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/reader.py` & `redvox-3.4.0a3/redvox/api900/reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/reader_utils.py` & `redvox-3.4.0a3/redvox/api900/reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/accelerometer_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/accelerometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/barometer_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/barometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/evenly_sampled_channel.py` & `redvox-3.4.0a3/redvox/api900/sensors/evenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/evenly_sampled_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/evenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/gyroscope_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/gyroscope_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/image_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/image_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/infrared_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/infrared_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/interleaved_channel.py` & `redvox-3.4.0a3/redvox/api900/sensors/interleaved_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/light_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/light_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/location_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/location_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/magnetometer_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/magnetometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/microphone_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/microphone_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/time_synchronization_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/time_synchronization_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/unevenly_sampled_channel.py` & `redvox-3.4.0a3/redvox/api900/sensors/unevenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/unevenly_sampled_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py` & `redvox-3.4.0a3/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/stat_utils.py` & `redvox-3.4.0a3/redvox/api900/stat_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/summarize.py` & `redvox-3.4.0a3/redvox/api900/summarize.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/timesync/api900_timesync.py` & `redvox-3.4.0a3/redvox/api900/timesync/api900_timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/timesync/tri_message_stats.py` & `redvox-3.4.0a3/redvox/api900/timesync/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/types.py` & `redvox-3.4.0a3/redvox/api900/types.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/api900/wrapped_redvox_packet.py` & `redvox-3.4.0a3/redvox/api900/wrapped_redvox_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cli/cli.py` & `redvox-3.4.0a3/redvox/cli/cli.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cli/conversions.py` & `redvox-3.4.0a3/redvox/cli/conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cli/data_req.py` & `redvox-3.4.0a3/redvox/cli/data_req.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/api.py` & `redvox-3.4.0a3/redvox/cloud/api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/api_m_fqns.py` & `redvox-3.4.0a3/redvox/cloud/api_m_fqns.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/auth_api.py` & `redvox-3.4.0a3/redvox/cloud/auth_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/client.py` & `redvox-3.4.0a3/redvox/cloud/client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/config.py` & `redvox-3.4.0a3/redvox/cloud/config.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/data_api.py` & `redvox-3.4.0a3/redvox/cloud/data_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/data_client.py` & `redvox-3.4.0a3/redvox/cloud/data_client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/data_io.py` & `redvox-3.4.0a3/redvox/cloud/data_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/metadata_api.py` & `redvox-3.4.0a3/redvox/cloud/metadata_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/query_timing_correction.py` & `redvox-3.4.0a3/redvox/cloud/query_timing_correction.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/routes.py` & `redvox-3.4.0a3/redvox/cloud/routes.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/station_stats.py` & `redvox-3.4.0a3/redvox/cloud/station_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/cloud/subscription.py` & `redvox-3.4.0a3/redvox/cloud/subscription.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/api_conversions.py` & `redvox-3.4.0a3/redvox/common/api_conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
     :return: A wrapped API M packet.
     """
     packet_m: api_m.RedvoxPacketM = api_m.RedvoxPacketM()
 
     # Top-level metadata
     packet_m.api = 1000.0
     # noinspection PyUnresolvedReferences,Mypy
-    packet_m.sub_api = api_m.SUB_API
+    packet_m.sub_api = 900.0
 
     # Station information
     packet_m.station_information.id = packet.redvox_id
     packet_m.station_information.uuid = packet.uuid
     packet_m.station_information.make = packet.device_make
     packet_m.station_information.model = packet.device_model
     packet_m.station_information.os = _migrate_os_type_900_to_1000_raw(packet.device_os)
@@ -799,15 +799,15 @@
     :return: A wrapped API M packet.
     """
     wrapped_packet_m: WrappedRedvoxPacketM = WrappedRedvoxPacketM.new()
 
     # Top-level metadata
     wrapped_packet_m.set_api(1000.0)
     # noinspection PyUnresolvedReferences,Mypy
-    wrapped_packet_m.set_sub_api(api_m.SUB_API)
+    wrapped_packet_m.set_sub_api(900.0)
 
     # Station information
     station_information: StationInformation = wrapped_packet_m.get_station_information()
     station_information.set_id(wrapped_packet_900.redvox_id()).set_uuid(
         wrapped_packet_900.uuid()
     ).set_make(wrapped_packet_900.device_make()).set_model(
         wrapped_packet_900.device_model()
```

### Comparing `redvox-3.4.0a2/redvox/common/api_reader.py` & `redvox-3.4.0a3/redvox/common/api_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 import multiprocessing.pool
 
 import pyarrow as pa
 import psutil
 
 import redvox.settings as settings
 import redvox.api1000.proto.redvox_api_m_pb2 as api_m
-from redvox.common import offset_model, io,\
+from redvox.common import offset_model as om,\
+    io,\
     api_conversions as ac,\
     file_statistics as fs
 from redvox.common.parallel_utils import maybe_parallel_map
 from redvox.common.station import Station
+from redvox.common.session_model import SessionModel
 from redvox.common.errors import RedVoxExceptions
 
 
 id_py_stct = pa.struct([("id", pa.string()), ("uuid", pa.string()), ("start_time", pa.float64()),
                         ])
 meta_py_stct = pa.struct([("api", pa.float64()), ("sub_api", pa.float64()), ("make", pa.string()),
                           ("model", pa.string()), ("os", pa.int64()), ("os_version", pa.string()),
@@ -213,15 +215,15 @@
             return [station_index]
 
         stats = fs.extract_stats(station_index, pool=_pool)
         # Close pool if created here
         if pool is None:
             _pool.close()
 
-        timing_offsets: Optional[offset_model.TimingOffsets] = offset_model.compute_offsets(stats)
+        timing_offsets: Optional[om.TimingOffsets] = om.compute_offsets(stats)
 
         # punt if duration or other important values are invalid or if the latency array was empty
         if timing_offsets is None:
             return [station_index]
 
         # if our filtered files do not encompass the request even when the packet times are updated
         # try getting 1.5 times the difference of the expected start/end and the start/end of the data
@@ -372,7 +374,192 @@
         :param get_id: the id to filter on
         :return: list of all stations with the requested id or None if id can't be found
         """
         result = [s for s in self.get_stations() if s.id() == get_id]
         if len(result) < 1:
             return None
         return result
+
+
+# This class uses a slightly stripped down version of the above ApiReader meant to quickly create SessionModels.
+# Some of the checks used in ApiReader are not necessary when creating SessionModel, while the core functionality
+#  of finding and reading files remains.
+class ApiReaderModel:
+    """
+    Reads data from api 900 or api 1000 format, converting all data read into RedvoxPacketM for
+    ease of comparison and use.
+    Creates SessionModels for each station session within the data read.
+
+    Properties:
+        filter: io.ReadFilter with the station ids, start and end time, start and end time padding, and
+        types of files to read
+
+        base_dir: str of the directory containing all the files to read
+
+        structured_dir: bool, if True, the base_dir contains a specific directory structure used by the
+        respective api formats.  If False, base_dir only has the data files.  Default False.
+
+        files_index: io.Index of the files that match the filter that are in base_dir
+
+        index_summary: io.IndexSummary of the filtered data
+
+        debug: bool, if True, output additional information during function execution.  Default False.
+
+        errors: RedVoxExceptions, a container for any errors encountered during function execution.
+    """
+
+    def __init__(
+            self,
+            base_dir: str,
+            structured_dir: bool = False,
+            read_filter: io.ReadFilter = None,
+            debug: bool = False,
+            pool: Optional[multiprocessing.pool.Pool] = None,
+    ):
+        """
+        Initialize the ApiReader object
+
+        :param base_dir: directory containing the files to read
+        :param structured_dir: if True, base_dir contains a specific directory structure used by the respective
+                                api formats.  If False, base_dir only has the data files.  Default False.
+        :param read_filter: ReadFilter for the data files, if None, get everything.  Default None
+        :param debug: if True, output program warnings/errors during function execution.  Default False.
+        """
+        _pool: multiprocessing.pool.Pool = (
+            multiprocessing.Pool() if pool is None else pool
+        )
+
+        if read_filter:
+            self.filter = read_filter
+            if self.filter.station_ids:
+                self.filter.station_ids = set(self.filter.station_ids)
+        else:
+            self.filter = io.ReadFilter()
+        self.base_dir = base_dir
+        self.structured_dir = structured_dir
+        self.debug = debug
+        self.errors = RedVoxExceptions("APIReader")
+        self.session_models: List[SessionModel] = []
+        self.files_index = self._get_all_files(_pool)
+        self.index_summary = io.IndexSummary.from_index(self._flatten_files_index())
+
+        if debug:
+            self.errors.print()
+
+        if pool is None:
+            _pool.close()
+
+    def _flatten_files_index(self):
+        """
+        :return: flattened version of files_index
+        """
+        result = io.Index()
+        for i in self.files_index:
+            result.append(i.entries)
+        return result
+
+    def _get_session(self, s_id: str, uuid: str, start_date: float) -> Optional[SessionModel]:
+        """
+        get a session that matches all the inputs or None if no match
+
+        :param s_id: station id to get
+        :param uuid: station uuid to get
+        :param start_date: station start date to get
+        :return: SessionModel or None
+        """
+        for m in self.session_models:
+            if m.id == s_id and m.uuid == uuid and m.start_date == start_date:
+                return m
+        return None
+
+    def _get_all_files(
+            self, pool: Optional[multiprocessing.pool.Pool] = None
+    ) -> List[io.Index]:
+        """
+        get all files in the base dir of the ApiReader
+
+        :return: index with all the files that match the filter
+        """
+        _pool: multiprocessing.pool.Pool = (
+            multiprocessing.Pool() if pool is None else pool
+        )
+        index: List[io.Index] = []
+        # this guarantees that all ids we search for are valid
+        all_index = self._apply_filter(pool=_pool)
+        for station_id in all_index.summarize().station_ids():
+            id_index = all_index.get_index_for_station_id(station_id)
+            for f in id_index.read_contents():
+                sd = f.timing_information.app_start_mach_timestamp
+                uid = f.station_information.uuid
+                n = self._get_session(station_id, uid, sd)
+                n.add_data_from_packet(f) if n is not None \
+                    else self.session_models.append(SessionModel.create_from_packet(f))
+            index.append(id_index)
+
+        if pool is None:
+            _pool.close()
+
+        return index
+
+    def _apply_filter(
+            self,
+            reader_filter: Optional[io.ReadFilter] = None,
+            pool: Optional[multiprocessing.pool.Pool] = None,
+    ) -> io.Index:
+        """
+        apply the filter of the reader, or another filter if specified
+
+        :param reader_filter: optional filter; if None, use the reader's filter, default None
+        :return: index of the filtered files
+        """
+        _pool: multiprocessing.pool.Pool = (
+            multiprocessing.Pool() if pool is None else pool
+        )
+        if not reader_filter:
+            reader_filter = self.filter
+        if self.structured_dir:
+            index = io.index_structured(self.base_dir, reader_filter, pool=_pool)
+        else:
+            index = io.index_unstructured(self.base_dir, reader_filter, pool=_pool)
+        if pool is None:
+            _pool.close()
+        return index
+
+    def _check_station_stats(
+            self,
+            station_index: io.Index,
+            pool: Optional[multiprocessing.pool.Pool] = None,
+    ) -> List[io.Index]:
+        """
+        check the index's results; if it has enough information, return it, otherwise search for more data.
+        The index should only request one station id
+        If the station was restarted during the request period, a new group of indexes will be created
+        to represent the change in station metadata.
+        Creates SessionModels for each station session found in the requested data.
+
+        :param station_index: index representing the requested information
+        :return: List of Indexes that includes as much information as possible that fits the request
+        """
+        # if we found nothing, return the index
+        if len(station_index.entries) < 1:
+            return [station_index]
+
+        _pool: multiprocessing.pool.Pool = multiprocessing.Pool() if pool is None else pool
+
+        stats = fs.extract_stats(station_index, pool=_pool)
+        # Close pool if created here
+        if pool is None:
+            _pool.close()
+
+        results = {}
+
+        for v, e in enumerate(stats):
+            key = e.app_start_dt
+            if key not in results.keys():
+                results[key] = io.Index()
+            results[key].append(entries=[station_index.entries[v]])
+
+        for s in results.values():
+            m = SessionModel.create_from_stream(s.read_contents())
+            self.session_models.append(m)
+
+        return list(results.values())
```

### Comparing `redvox-3.4.0a2/redvox/common/api_reader_dw.py` & `redvox-3.4.0a3/redvox/common/api_reader_dw.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/api_reader_old.py` & `redvox-3.4.0a3/redvox/common/api_reader_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/constants.py` & `redvox-3.4.0a3/redvox/common/constants.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/cross_stats.py` & `redvox-3.4.0a3/redvox/common/cross_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/data_window.py` & `redvox-3.4.0a3/redvox/common/data_window.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/data_window_configuration.py` & `redvox-3.4.0a3/redvox/common/data_window_configuration.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/data_window_configuration_old.py` & `redvox-3.4.0a3/redvox/common/data_window_configuration_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/data_window_io.py` & `redvox-3.4.0a3/redvox/common/data_window_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/data_window_old.py` & `redvox-3.4.0a3/redvox/common/data_window_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/date_time_utils.py` & `redvox-3.4.0a3/redvox/common/date_time_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -483,35 +483,35 @@
 def datetime_from_epoch_seconds_utc(epoch_seconds_utc: float) -> datetime:
     """
     Given number of seconds since the epoch UTC, return a Python datetime object.
 
     :param epoch_seconds_utc: A UTC second timestamp.
     :return: A datetime object.
     """
-    return EPOCH + timedelta(seconds=epoch_seconds_utc)
+    return EPOCH + timedelta(seconds=0 if np.isnan(epoch_seconds_utc) else epoch_seconds_utc)
 
 
 def datetime_from_epoch_milliseconds_utc(epoch_milliseconds_utc: float) -> datetime:
     """
     Given number of milliseconds since the epoch UTC, return a Python datetime object.
 
     :param epoch_milliseconds_utc: UTC millisecond timestamp.
     :return: Datetime object.
     """
-    return EPOCH + timedelta(milliseconds=epoch_milliseconds_utc)
+    return EPOCH + timedelta(milliseconds=0 if np.isnan(epoch_milliseconds_utc) else epoch_milliseconds_utc)
 
 
 def datetime_from_epoch_microseconds_utc(epoch_microseconds_utc: float) -> datetime:
     """
     Given number of microseconds since the epoch UTC, return a Python datetime object.
 
     :param epoch_microseconds_utc: UTC microsecond timestamp.
     :return: A datetime object.
     """
-    return EPOCH + timedelta(microseconds=epoch_microseconds_utc)
+    return EPOCH + timedelta(microseconds=0 if np.isnan(epoch_microseconds_utc) else epoch_microseconds_utc)
 
 
 def datetimes_from_epoch_seconds_utc(epochs_seconds_utc: List[int]) -> List[datetime]:
     """
     Concerts a list of timestamps as seconds since the epoch UTC to a list of datetime objects.
 
     :param epochs_seconds_utc: List of timestamps to convert.
```

### Comparing `redvox-3.4.0a2/redvox/common/errors.py` & `redvox-3.4.0a3/redvox/common/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/event_stream.py` & `redvox-3.4.0a3/redvox/common/event_stream.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/event_stream_io.py` & `redvox-3.4.0a3/redvox/common/event_stream_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/file_statistics.py` & `redvox-3.4.0a3/redvox/common/file_statistics.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/gap_and_pad_utils.py` & `redvox-3.4.0a3/redvox/common/gap_and_pad_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/gap_and_pad_utils_old.py` & `redvox-3.4.0a3/redvox/common/gap_and_pad_utils_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/gui/cloud_data_retrieval.py` & `redvox-3.4.0a3/redvox/common/gui/cloud_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/io.py` & `redvox-3.4.0a3/redvox/common/io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/packet_to_pyarrow.py` & `redvox-3.4.0a3/redvox/common/packet_to_pyarrow.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,46 +15,14 @@
 from redvox.common import sensor_reader_utils as srupa
 from redvox.common import date_time_utils as dtu
 from redvox.common import gap_and_pad_utils as gpu
 from redvox.common.sensor_data import SensorType
 from redvox.common.errors import RedVoxExceptions
 
 
-# Maps a sensor type to a function that can extract that sensor for a particular packet.
-__SENSOR_NAME_TO_SENSOR_FN: Dict[
-    str,
-    Optional[
-        Callable[
-            [RedvoxPacketM],
-            srupa.SensorData,
-        ]
-    ],
-] = {
-    "health": None,
-    "accelerometer": lambda packet: packet.sensors.accelerometer,
-    "ambient_temperature": lambda packet: packet.sensors.ambient_temperature,
-    "audio": lambda packet: packet.sensors.audio,
-    "compressed_audio": lambda packet: packet.sensors.compressed_audio,
-    "gravity": lambda packet: packet.sensors.gravity,
-    "gyroscope": lambda packet: packet.sensors.gyroscope,
-    "image": lambda packet: packet.sensors.image,
-    "light": lambda packet: packet.sensors.light,
-    "linear_acceleration": lambda packet: packet.sensors.linear_acceleration,
-    "location": lambda packet: packet.sensors.location,
-    "best_location": lambda packet: packet.sensors.location,
-    "magnetometer": lambda packet: packet.sensors.magnetometer,
-    "orientation": lambda packet: packet.sensors.orientation,
-    "pressure": lambda packet: packet.sensors.pressure,
-    "proximity": lambda packet: packet.sensors.proximity,
-    "relative_humidity": lambda packet: packet.sensors.relative_humidity,
-    "rotation_vector": lambda packet: packet.sensors.rotation_vector,
-    "infrared": lambda packet: packet.sensors.proximity,
-}
-
-
 packet_schema = pa.schema([("packet_start_mach_timestamp", pa.float64()),
                            ("packet_end_mach_timestamp", pa.float64()),
                            ("packet_start_os_timestamp", pa.float64()),
                            ("packet_end_os_timestamp", pa.float64()),
                            ("timing_info_score", pa.int64())
                            ])
 
@@ -421,14 +389,15 @@
         load_apim_accelerometer,
         load_apim_gyroscope,
         load_apim_magnetometer,
         load_apim_gravity,
         load_apim_linear_accel,
         load_apim_orientation,
         load_apim_rotation_vector,
+        load_apim_velocity,
     ]
     sensors = map(lambda fn: fn(packet), funcs)
     for data in sensors:
         if data:
             data.start = packet_start
             if out_dir:
                 data.fdir = os.path.join(out_dir, f"{data.stype.name}_SUMMARY")
@@ -731,15 +700,25 @@
 
     :param packet: packet with data to load
     :return: linear acceleration sensor data if it exists, None otherwise
     """
     return load_xyz(packet, srupa.SensorType.LINEAR_ACCELERATION)
 
 
-def load_apim_rotation_vector(packet: RedvoxPacketM,) -> Optional[PyarrowSummary]:
+def load_apim_rotation_vector(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
     """
     load rotation vector data from a single redvox packet
 
     :param packet: packet with data to load
     :return: rotation vector sensor data if it exists, None otherwise
     """
     return load_xyz(packet, srupa.SensorType.ROTATION_VECTOR)
+
+
+def load_apim_velocity(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
+    """
+    load velocity data from a single redvox packet
+
+    :param packet: packet with data to load
+    :return: velocity sensor data if it exists, None otherwise
+    """
+    return load_xyz(packet, srupa.SensorType.VELOCITY)
```

### Comparing `redvox-3.4.0a2/redvox/common/parallel_utils.py` & `redvox-3.4.0a3/redvox/common/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/run_me.py` & `redvox-3.4.0a3/redvox/common/run_me.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/sensor_data.py` & `redvox-3.4.0a3/redvox/common/sensor_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     ROTATION_VECTOR = 16  # Unitless
     INFRARED = 17  # this is proximity
     STATION_HEALTH = 18
     # Health sensors: battery charge and current level, phone internal temperature, network source and strength,
     # available RAM of the system, cell service status, amount of hard disk space left, power charging state
     # wifi lock state, cpu utilization, screen state, and screen brightness
     BEST_LOCATION = 19  # See standard
+    VELOCITY = 20  # m/s
 
     @staticmethod
     def type_from_str(type_str: str) -> "SensorType":
         """
         converts a string to a sensor type
 
         :param type_str: string to convert
@@ -124,14 +125,16 @@
             return SensorType.PRESSURE
         elif type_str.lower() == "proximity" or type_str.lower() == "infrared":
             return SensorType.PROXIMITY
         elif type_str.lower() == "relative_humidity":
             return SensorType.RELATIVE_HUMIDITY
         elif type_str.lower() == "rotation_vector":
             return SensorType.ROTATION_VECTOR
+        elif type_str.lower() == "velocity":
+            return SensorType.VELOCITY
         else:
             return SensorType.UNKNOWN_SENSOR
 
 
 class SensorData:
     """
     Generic RedvoxSensor class for API-independent analysis
@@ -954,14 +957,15 @@
                 SensorType.ACCELEROMETER: AccelerometerSensor,
                 SensorType.GYROSCOPE: GyroscopeSensor,
                 SensorType.MAGNETOMETER: MagnetometerSensor,
                 SensorType.ORIENTATION: OrientationSensor,
                 SensorType.GRAVITY: GravitySensor,
                 SensorType.LINEAR_ACCELERATION: LinearAccelerationSensor,
                 SensorType.ROTATION_VECTOR: RotationVectorSensor,
+                SensorType.VELOCITY: VelocitySensor,
                 SensorType.UNKNOWN_SENSOR: SensorData
             }
             self.__class__ = sensor_class_from_type[self._type]
         return self
 
     def set_errors(self, errors: RedVoxExceptions):
         """
@@ -1614,14 +1618,72 @@
     def get_valid_rotation_vector_z_data(self) -> np.array:
         """
         :return: non-nan rotation vector z channel data as numpy array
         """
         return super().get_valid_data_channel_values('rotation_vector_z')
 
 
+class VelocitySensor(SensorData):
+    """
+    Rotation vector specific functions
+    """
+    def __init__(self, sensor_name: str,
+                 sensor_data: Optional[pa.Table] = None,
+                 sample_rate_hz: float = np.nan,
+                 sample_interval_s: float = np.nan,
+                 sample_interval_std_s: float = np.nan,
+                 is_sample_rate_fixed: bool = False,
+                 are_timestamps_altered: bool = False,
+                 calculate_stats: bool = False,
+                 use_offset_model_for_correction: bool = False,
+                 save_data: bool = False,
+                 base_dir: str = ".",
+                 gaps: Optional[List[Tuple[float, float]]] = None,
+                 show_errors: bool = False):
+        super().__init__(sensor_name, sensor_data, SensorType.Velocity, sample_rate_hz, sample_interval_s,
+                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
+                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def get_velocity_x_data(self) -> np.array:
+        """
+        :return: velocity x channel data as numpy array
+        """
+        return super().get_data_channel('velocity_x')
+
+    def get_valid_velocity_x_data(self) -> np.array:
+        """
+        :return: non-nan velocity x channel data as numpy array
+        """
+        return super().get_valid_data_channel_values('velocity_x')
+
+    def get_velocity_y_data(self) -> np.array:
+        """
+        :return: velocity y channel data as numpy array
+        """
+        return super().get_data_channel('velocity_y')
+
+    def get_valid_velocity_y_data(self) -> np.array:
+        """
+        :return: non-nan velocity y channel data as numpy array
+        """
+        return super().get_valid_data_channel_values('velocity_y')
+
+    def get_velocity_z_data(self) -> np.array:
+        """
+        :return: velocity z channel data as numpy array
+        """
+        return super().get_data_channel('velocity_z')
+
+    def get_valid_velocity_z_data(self) -> np.array:
+        """
+        :return: non-nan velocity z channel data as numpy array
+        """
+        return super().get_valid_data_channel_values('velocity_z')
+
+
 class GyroscopeSensor(SensorData):
     """
     Gyroscope specific functions
     """
     def __init__(self, sensor_name: str,
                  sensor_data: Optional[pa.Table] = None,
                  sample_rate_hz: float = np.nan,
```

### Comparing `redvox-3.4.0a2/redvox/common/sensor_data_old.py` & `redvox-3.4.0a3/redvox/common/sensor_data_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/sensor_io.py` & `redvox-3.4.0a3/redvox/common/sensor_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/sensor_reader_utils.py` & `redvox-3.4.0a3/redvox/common/sensor_reader_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 __LINEAR_ACCELERATION_FIELD_NAME: str = "linear_acceleration"
 __LOCATION_FIELD_NAME: str = "location"
 __MAGNETOMETER_FIELD_NAME: str = "magnetometer"
 __ORIENTATION_FIELD_NAME: str = "orientation"
 __PRESSURE_FIELD_NAME: str = "pressure"
 __PROXIMITY_FIELD_NAME: str = "proximity"
 __RELATIVE_HUMIDITY_FIELD_NAME: str = "relative_humidity"
-__ROTATION_VECTOR: str = "rotation_vector"
-__VELOCITY: str = "velocity"
+__ROTATION_VECTOR_FIELD_NAME: str = "rotation_vector"
+__VELOCITY_FIELD_NAME: str = "velocity"
 
 __SENSOR_TYPE_TO_FIELD_NAME: Dict[SensorType, str] = {
     SensorType.UNKNOWN_SENSOR: "unknown",
     SensorType.STATION_HEALTH: "unknown",
     SensorType.ACCELEROMETER: __ACCELEROMETER_FIELD_NAME,
     SensorType.AMBIENT_TEMPERATURE: __AMBIENT_TEMPERATURE_FIELD_NAME,
     SensorType.AUDIO: __AUDIO_FIELD_NAME,
@@ -96,16 +96,17 @@
     SensorType.LOCATION: __LOCATION_FIELD_NAME,
     SensorType.BEST_LOCATION: __LOCATION_FIELD_NAME,
     SensorType.MAGNETOMETER: __MAGNETOMETER_FIELD_NAME,
     SensorType.ORIENTATION: __ORIENTATION_FIELD_NAME,
     SensorType.PRESSURE: __PRESSURE_FIELD_NAME,
     SensorType.PROXIMITY: __PROXIMITY_FIELD_NAME,
     SensorType.RELATIVE_HUMIDITY: __RELATIVE_HUMIDITY_FIELD_NAME,
-    SensorType.ROTATION_VECTOR: __ROTATION_VECTOR,
+    SensorType.ROTATION_VECTOR: __ROTATION_VECTOR_FIELD_NAME,
     SensorType.INFRARED: __PROXIMITY_FIELD_NAME,
+    SensorType.VELOCITY: __VELOCITY_FIELD_NAME,
 }
 
 Sensor = Union[
     api_m.RedvoxPacketM.Sensors.Xyz,
     api_m.RedvoxPacketM.Sensors.Single,
     api_m.RedvoxPacketM.Sensors.Audio,
     api_m.RedvoxPacketM.Sensors.Image,
@@ -139,14 +140,15 @@
     SensorType.MAGNETOMETER: lambda packet: packet.sensors.magnetometer,
     SensorType.ORIENTATION: lambda packet: packet.sensors.orientation,
     SensorType.PRESSURE: lambda packet: packet.sensors.pressure,
     SensorType.PROXIMITY: lambda packet: packet.sensors.proximity,
     SensorType.RELATIVE_HUMIDITY: lambda packet: packet.sensors.relative_humidity,
     SensorType.ROTATION_VECTOR: lambda packet: packet.sensors.rotation_vector,
     SensorType.INFRARED: lambda packet: packet.sensors.proximity,
+    SensorType.VELOCITY: lambda packet: packet.sensors.velocity,
 }
 
 
 def __has_sensor(
         data: Union[api_m.RedvoxPacketM, api_m.RedvoxPacketM.Sensors], field_name: str
 ) -> bool:
     """
```

### Comparing `redvox-3.4.0a2/redvox/common/sensor_reader_utils_old.py` & `redvox-3.4.0a3/redvox/common/sensor_reader_utils_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/station.py` & `redvox-3.4.0a3/redvox/common/station.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/station_io.py` & `redvox-3.4.0a3/redvox/common/station_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/station_old.py` & `redvox-3.4.0a3/redvox/common/station_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/station_utils.py` & `redvox-3.4.0a3/redvox/common/station_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/stats_helper.py` & `redvox-3.4.0a3/redvox/common/stats_helper.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/timesync.py` & `redvox-3.4.0a3/redvox/common/timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/timesync_io.py` & `redvox-3.4.0a3/redvox/common/timesync_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/timesync_old.py` & `redvox-3.4.0a3/redvox/common/timesync_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/tri_message_stats.py` & `redvox-3.4.0a3/redvox/common/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/common/versioning.py` & `redvox-3.4.0a3/redvox/common/versioning.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a2/redvox/settings.py` & `redvox-3.4.0a3/redvox/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,7 +68,16 @@
     :return: True if the native extra is enabled, False otherwise
     """
     try:
         import redvox_native
         return True
     except ModuleNotFoundError:
         return False
+
+
+def is_cpp_backend_enabled() -> bool:
+    """
+    :return: True if the protobuf CPP backend is enabled, False otherwise
+    """
+    # noinspection PyUnresolvedReferences
+    from google.protobuf.internal import api_implementation
+    return api_implementation.Type() == "cpp"
```

### Comparing `redvox-3.4.0a2/redvox.egg-info/SOURCES.txt` & `redvox-3.4.0a3/redvox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+LICENSE
 README.md
-setup.py
+pyproject.toml
 redvox/__init__.py
 redvox/settings.py
 redvox.egg-info/PKG-INFO
 redvox.egg-info/SOURCES.txt
 redvox.egg-info/dependency_links.txt
 redvox.egg-info/entry_points.txt
 redvox.egg-info/requires.txt
@@ -117,16 +118,20 @@
 redvox/common/parallel_utils.py
 redvox/common/run_me.py
 redvox/common/sensor_data.py
 redvox/common/sensor_data_old.py
 redvox/common/sensor_io.py
 redvox/common/sensor_reader_utils.py
 redvox/common/sensor_reader_utils_old.py
+redvox/common/session_io.py
+redvox/common/session_model.py
+redvox/common/session_model_utils.py
 redvox/common/station.py
 redvox/common/station_io.py
+redvox/common/station_model.py
 redvox/common/station_old.py
 redvox/common/station_utils.py
 redvox/common/stats_helper.py
 redvox/common/timesync.py
 redvox/common/timesync_io.py
 redvox/common/timesync_old.py
 redvox/common/tri_message_stats.py
```

