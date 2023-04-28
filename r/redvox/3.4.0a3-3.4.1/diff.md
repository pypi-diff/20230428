# Comparing `tmp/redvox-3.4.0a3.tar.gz` & `tmp/redvox-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-3.4.0a3.tar", last modified: Thu Apr 27 23:37:57 2023, max compression
+gzip compressed data, was "redvox-3.4.1.tar", last modified: Fri Apr 28 20:37:47 2023, max compression
```

## Comparing `redvox-3.4.0a3.tar` & `redvox-3.4.1.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.842311 redvox-3.4.0a3/
--rw-r--r--   0 opq       (1000) opq       (1000)    11343 2023-04-25 23:11:34.000000 redvox-3.4.0a3/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    13908 2023-04-27 23:37:57.842311 redvox-3.4.0a3/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)      517 2021-06-14 20:37:56.000000 redvox-3.4.0a3/README.md
--rw-r--r--   0 opq       (1000) opq       (1000)     1375 2023-04-27 23:32:39.000000 redvox-3.4.0a3/pyproject.toml
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.825312 redvox-3.4.0a3/redvox/
--rw-r--r--   0 opq       (1000) opq       (1000)      817 2023-04-27 23:37:44.000000 redvox-3.4.0a3/redvox/__init__.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.826311 redvox-3.4.0a3/redvox/api1000/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/__init__.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.827312 redvox-3.4.0a3/redvox/api1000/common/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    20204 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/common.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1050 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/decorators.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5359 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/generic.py
--rw-r--r--   0 opq       (1000) opq       (1000)      875 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/lz4.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2570 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/mapping.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2237 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/metadata.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2435 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/common/typing.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2114 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/errors.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.827312 redvox-3.4.0a3/redvox/api1000/gui/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/gui/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4672 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/api1000/gui/image_viewer.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.828312 redvox-3.4.0a3/redvox/api1000/proto/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/proto/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    41044 2023-04-25 01:37:07.000000 redvox-3.4.0a3/redvox/api1000/proto/redvox_api_m_pb2.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.828312 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5639 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/event_streams.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.829311 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    11949 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.829311 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/derived/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14890 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7398 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/image.py
--rw-r--r--   0 opq       (1000) opq       (1000)    40936 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/location.py
--rw-r--r--   0 opq       (1000) opq       (1000)    42236 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3425 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/single.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5576 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    50437 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/station_information.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19060 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/timing_information.py
--rw-r--r--   0 opq       (1000) opq       (1000)    21971 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.831312 redvox-3.4.0a3/redvox/api900/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    17514 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/concat.py
--rw-r--r--   0 opq       (1000) opq       (1000)      494 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/constants.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1689 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/deprecation.py
--rw-r--r--   0 opq       (1000) opq       (1000)      351 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/exceptions.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.831312 redvox-3.4.0a3/redvox/api900/lib/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/lib/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7970 2023-04-25 01:37:07.000000 redvox-3.4.0a3/redvox/api900/lib/api900_pb2.py
--rw-r--r--   0 opq       (1000) opq       (1000)    43091 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/location_analyzer.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2597 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/migrations.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.831312 redvox-3.4.0a3/redvox/api900/qa/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/qa/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2813 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/qa/gap_detection.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16939 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/reader.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    17096 2021-06-07 23:35:09.000000 redvox-3.4.0a3/redvox/api900/reader_utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.833311 redvox-3.4.0a3/redvox/api900/sensors/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2113 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/accelerometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2298 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/barometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2665 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/evenly_sampled_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     6283 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/evenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1989 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/gyroscope_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4854 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/image_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2264 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/infrared_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16540 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/interleaved_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2261 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/light_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10051 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/location_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2022 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/magnetometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3209 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/microphone_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4655 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/time_synchronization_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3536 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/unevenly_sampled_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     6619 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/unevenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5907 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1128 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/stat_utils.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8780 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/summarize.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.834311 redvox-3.4.0a3/redvox/api900/timesync/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/timesync/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    27606 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/timesync/api900_timesync.py
--rw-r--r--   0 opq       (1000) opq       (1000)    13824 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/timesync/tri_message_stats.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1537 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/types.py
--rw-r--r--   0 opq       (1000) opq       (1000)    54392 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/api900/wrapped_redvox_packet.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.834311 redvox-3.4.0a3/redvox/cli/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cli/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22678 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/cli/cli.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6683 2021-06-07 23:35:09.000000 redvox-3.4.0a3/redvox/cli/conversions.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1797 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/cli/data_req.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.836311 redvox-3.4.0a3/redvox/cloud/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     2267 2021-04-06 18:15:12.000000 redvox-3.4.0a3/redvox/cloud/api.py
--rw-r--r--   0 opq       (1000) opq       (1000)   142063 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/api_m_fqns.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4334 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/auth_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    27215 2022-04-20 20:36:13.000000 redvox-3.4.0a3/redvox/cloud/client.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5905 2021-09-16 19:39:56.000000 redvox-3.4.0a3/redvox/cloud/config.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6088 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/cloud/data_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3829 2021-09-16 19:39:56.000000 redvox-3.4.0a3/redvox/cloud/data_client.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3094 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/data_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)      487 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/cloud/errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18946 2022-04-20 20:36:13.000000 redvox-3.4.0a3/redvox/cloud/metadata_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3770 2021-04-14 23:45:25.000000 redvox-3.4.0a3/redvox/cloud/query_timing_correction.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      902 2022-04-20 20:36:13.000000 redvox-3.4.0a3/redvox/cloud/routes.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4262 2021-04-14 23:45:25.000000 redvox-3.4.0a3/redvox/cloud/station_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     7707 2022-06-01 22:08:00.000000 redvox-3.4.0a3/redvox/cloud/subscription.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.842311 redvox-3.4.0a3/redvox/common/
--rw-r--r--   0 opq       (1000) opq       (1000)      195 2021-03-29 23:26:30.000000 redvox-3.4.0a3/redvox/common/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    55240 2022-09-30 02:01:56.000000 redvox-3.4.0a3/redvox/common/api_conversions.py
--rw-r--r--   0 opq       (1000) opq       (1000)    23044 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/api_reader.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5527 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/api_reader_dw.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    12875 2021-06-07 23:35:09.000000 redvox-3.4.0a3/redvox/common/api_reader_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1173 2021-04-20 02:39:13.000000 redvox-3.4.0a3/redvox/common/constants.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4126 2021-07-07 20:00:14.000000 redvox-3.4.0a3/redvox/common/cross_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    44341 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/data_window.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8246 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/data_window_configuration.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6208 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/data_window_configuration_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    12571 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/data_window_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    31911 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/data_window_old.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16785 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/date_time_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3250 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    39791 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/event_stream.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3397 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/event_stream_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14254 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/file_statistics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22168 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/gap_and_pad_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22503 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/gap_and_pad_utils_old.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.842311 redvox-3.4.0a3/redvox/common/gui/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-04-14 19:22:20.000000 redvox-3.4.0a3/redvox/common/gui/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16251 2021-04-14 23:46:42.000000 redvox-3.4.0a3/redvox/common/gui/cloud_data_retrieval.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    56743 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    25612 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/offset_model.py
--rw-r--r--   0 opq       (1000) opq       (1000)    27554 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/packet_to_pyarrow.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5022 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/parallel_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1256 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/run_me.py
--rw-r--r--   0 opq       (1000) opq       (1000)    94299 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/sensor_data.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    44259 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/sensor_data_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1206 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/sensor_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    18349 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/sensor_reader_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    55914 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/sensor_reader_utils_old.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3352 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/session_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    44577 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/session_model.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14986 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/session_model_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    66786 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/station.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1679 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/station_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4515 2023-04-25 00:47:07.000000 redvox-3.4.0a3/redvox/common/station_model.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    42555 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/station_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    23699 2022-06-29 18:15:55.000000 redvox-3.4.0a3/redvox/common/station_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4002 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/stats_helper.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    24492 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/timesync.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1295 2022-04-19 20:47:15.000000 redvox-3.4.0a3/redvox/common/timesync_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    35537 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/timesync_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14138 2022-01-03 23:28:51.000000 redvox-3.4.0a3/redvox/common/tri_message_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1867 2021-07-07 20:00:14.000000 redvox-3.4.0a3/redvox/common/versioning.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2483 2022-09-30 02:01:51.000000 redvox-3.4.0a3/redvox/settings.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:37:57.826311 redvox-3.4.0a3/redvox.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    13908 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     4767 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       51 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/entry_points.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      386 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        7 2023-04-27 23:37:57.000000 redvox-3.4.0a3/redvox.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:37:57.842311 redvox-3.4.0a3/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.406221 redvox-3.4.1/
+-rw-r--r--   0 opq       (1000) opq       (1000)    11343 2023-04-28 19:34:15.000000 redvox-3.4.1/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    13906 2023-04-28 20:37:47.406221 redvox-3.4.1/PKG-INFO
+-rw-rw-r--   0 opq       (1000) opq       (1000)      517 2021-06-14 20:37:56.000000 redvox-3.4.1/README.md
+-rw-r--r--   0 opq       (1000) opq       (1000)     1375 2023-04-28 19:34:15.000000 redvox-3.4.1/pyproject.toml
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.390222 redvox-3.4.1/redvox/
+-rw-r--r--   0 opq       (1000) opq       (1000)      815 2023-04-28 20:36:50.000000 redvox-3.4.1/redvox/__init__.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.391222 redvox-3.4.1/redvox/api1000/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/__init__.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.392222 redvox-3.4.1/redvox/api1000/common/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    20204 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/common.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1050 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/decorators.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     5359 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/generic.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      875 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/lz4.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2570 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/mapping.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2237 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/metadata.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2435 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/typing.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2114 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/errors.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.393222 redvox-3.4.1/redvox/api1000/gui/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/gui/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4672 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/api1000/gui/image_viewer.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.393222 redvox-3.4.1/redvox/api1000/proto/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/proto/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    41044 2023-04-28 19:34:15.000000 redvox-3.4.1/redvox/api1000/proto/redvox_api_m_pb2.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.393222 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     5639 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/event_streams.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.394222 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    11949 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.394222 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14890 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     7398 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/image.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    40936 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/location.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    42236 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3425 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/single.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     5576 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    50437 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/station_information.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19060 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/timing_information.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    21971 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.396222 redvox-3.4.1/redvox/api900/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    17514 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/concat.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      494 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/constants.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1689 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/deprecation.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      351 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/exceptions.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.396222 redvox-3.4.1/redvox/api900/lib/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/lib/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     7970 2023-04-28 19:34:15.000000 redvox-3.4.1/redvox/api900/lib/api900_pb2.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    43091 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/location_analyzer.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2597 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/migrations.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.396222 redvox-3.4.1/redvox/api900/qa/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/qa/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2813 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/qa/gap_detection.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16939 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/reader.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    17096 2021-06-07 23:35:09.000000 redvox-3.4.1/redvox/api900/reader_utils.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.398222 redvox-3.4.1/redvox/api900/sensors/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2113 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/accelerometer_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2298 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/barometer_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2665 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/evenly_sampled_channel.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     6283 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/evenly_sampled_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1989 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/gyroscope_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4854 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/image_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2264 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/infrared_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16540 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/interleaved_channel.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2261 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/light_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    10051 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/location_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2022 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/magnetometer_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3209 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/microphone_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4655 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/time_synchronization_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3536 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/unevenly_sampled_channel.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     6619 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/unevenly_sampled_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     5907 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1128 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/stat_utils.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     8780 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/summarize.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.398222 redvox-3.4.1/redvox/api900/timesync/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/timesync/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    27606 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/timesync/api900_timesync.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    13824 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/timesync/tri_message_stats.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     1537 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/types.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    54392 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/wrapped_redvox_packet.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.399222 redvox-3.4.1/redvox/cli/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cli/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    22678 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/cli/cli.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6683 2021-06-07 23:35:09.000000 redvox-3.4.1/redvox/cli/conversions.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1797 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/cli/data_req.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.401222 redvox-3.4.1/redvox/cloud/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     2267 2021-04-06 18:15:12.000000 redvox-3.4.1/redvox/cloud/api.py
+-rw-r--r--   0 opq       (1000) opq       (1000)   142063 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/api_m_fqns.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4334 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/auth_api.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    27215 2022-04-20 20:36:13.000000 redvox-3.4.1/redvox/cloud/client.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5905 2021-09-16 19:39:56.000000 redvox-3.4.1/redvox/cloud/config.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6088 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/cloud/data_api.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3829 2021-09-16 19:39:56.000000 redvox-3.4.1/redvox/cloud/data_client.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3094 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/data_io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      487 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/errors.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    18946 2022-04-20 20:36:13.000000 redvox-3.4.1/redvox/cloud/metadata_api.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3770 2021-04-14 23:45:25.000000 redvox-3.4.1/redvox/cloud/query_timing_correction.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      902 2022-04-20 20:36:13.000000 redvox-3.4.1/redvox/cloud/routes.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4262 2021-04-14 23:45:25.000000 redvox-3.4.1/redvox/cloud/station_stats.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     7707 2022-06-01 22:08:00.000000 redvox-3.4.1/redvox/cloud/subscription.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.406221 redvox-3.4.1/redvox/common/
+-rw-r--r--   0 opq       (1000) opq       (1000)      195 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/common/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    55240 2022-09-30 02:01:56.000000 redvox-3.4.1/redvox/common/api_conversions.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    23044 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/api_reader.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5527 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/api_reader_dw.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    12875 2021-06-07 23:35:09.000000 redvox-3.4.1/redvox/common/api_reader_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1173 2021-04-20 02:39:13.000000 redvox-3.4.1/redvox/common/constants.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4126 2021-07-07 20:00:14.000000 redvox-3.4.1/redvox/common/cross_stats.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    44341 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/data_window.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8246 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/data_window_configuration.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6208 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/data_window_configuration_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    12571 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/data_window_io.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    31911 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/data_window_old.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16785 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/date_time_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3250 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/errors.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    39791 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/event_stream.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3397 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/event_stream_io.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    14254 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/file_statistics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    22168 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/gap_and_pad_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    22503 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/gap_and_pad_utils_old.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.406221 redvox-3.4.1/redvox/common/gui/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/common/gui/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    16251 2021-04-14 23:46:42.000000 redvox-3.4.1/redvox/common/gui/cloud_data_retrieval.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    56743 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    25612 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/offset_model.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    27554 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/packet_to_pyarrow.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5022 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/parallel_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1256 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/run_me.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    94299 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/sensor_data.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    44259 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/sensor_data_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1206 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/sensor_io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    18349 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/sensor_reader_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    55914 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/sensor_reader_utils_old.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3352 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/session_io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    44577 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/session_model.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14986 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/session_model_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    66786 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/station.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1679 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/station_io.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4515 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/station_model.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    42555 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/station_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    23699 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/station_utils.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4002 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/stats_helper.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    24492 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/timesync.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1295 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/timesync_io.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    35537 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/timesync_old.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    14138 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/tri_message_stats.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1867 2021-07-07 20:00:14.000000 redvox-3.4.1/redvox/common/versioning.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     2483 2022-09-30 02:01:51.000000 redvox-3.4.1/redvox/settings.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.391222 redvox-3.4.1/redvox.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    13906 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     4767 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       51 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/entry_points.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      386 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        7 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-28 20:37:47.407221 redvox-3.4.1/setup.cfg
```

### Comparing `redvox-3.4.0a3/LICENSE` & `redvox-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/PKG-INFO` & `redvox-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.4.0a3
+Version: 3.4.1
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.4.0a3/README.md` & `redvox-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/pyproject.toml` & `redvox-3.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/__init__.py` & `redvox-3.4.1/redvox/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Provides library level metadata and constants.
 """
 
 NAME: str = "redvox"
-VERSION: str = "3.4.0a3"
+VERSION: str = "3.4.1"
 
 
 def version() -> str:
     """Returns the version number of this library."""
     return VERSION
```

### Comparing `redvox-3.4.0a3/redvox/api1000/common/common.py` & `redvox-3.4.1/redvox/api1000/common/common.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/common/decorators.py` & `redvox-3.4.1/redvox/api1000/common/decorators.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/common/generic.py` & `redvox-3.4.1/redvox/api1000/common/generic.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/common/lz4.py` & `redvox-3.4.1/redvox/api1000/common/lz4.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/common/mapping.py` & `redvox-3.4.1/redvox/api1000/common/mapping.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/common/metadata.py` & `redvox-3.4.1/redvox/api1000/common/metadata.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/common/typing.py` & `redvox-3.4.1/redvox/api1000/common/typing.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/errors.py` & `redvox-3.4.1/redvox/api1000/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/gui/image_viewer.py` & `redvox-3.4.1/redvox/api1000/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/proto/redvox_api_m_pb2.py` & `redvox-3.4.1/redvox/api1000/proto/redvox_api_m_pb2.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/event_streams.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/event_streams.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/audio.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/audio.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/image.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/image.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/location.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/location.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/single.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/single.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/station_information.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/station_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/timing_information.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/timing_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py` & `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/concat.py` & `redvox-3.4.1/redvox/api900/concat.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/deprecation.py` & `redvox-3.4.1/redvox/api900/deprecation.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/lib/api900_pb2.py` & `redvox-3.4.1/redvox/api900/lib/api900_pb2.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/location_analyzer.py` & `redvox-3.4.1/redvox/api900/location_analyzer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/migrations.py` & `redvox-3.4.1/redvox/api900/migrations.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/qa/gap_detection.py` & `redvox-3.4.1/redvox/api900/qa/gap_detection.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/reader.py` & `redvox-3.4.1/redvox/api900/reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/reader_utils.py` & `redvox-3.4.1/redvox/api900/reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/accelerometer_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/accelerometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/barometer_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/barometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/evenly_sampled_channel.py` & `redvox-3.4.1/redvox/api900/sensors/evenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/evenly_sampled_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/evenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/gyroscope_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/gyroscope_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/image_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/image_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/infrared_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/infrared_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/interleaved_channel.py` & `redvox-3.4.1/redvox/api900/sensors/interleaved_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/light_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/light_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/location_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/location_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/magnetometer_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/magnetometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/microphone_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/microphone_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/time_synchronization_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/time_synchronization_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/unevenly_sampled_channel.py` & `redvox-3.4.1/redvox/api900/sensors/unevenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/unevenly_sampled_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py` & `redvox-3.4.1/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/stat_utils.py` & `redvox-3.4.1/redvox/api900/stat_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/summarize.py` & `redvox-3.4.1/redvox/api900/summarize.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/timesync/api900_timesync.py` & `redvox-3.4.1/redvox/api900/timesync/api900_timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/timesync/tri_message_stats.py` & `redvox-3.4.1/redvox/api900/timesync/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/types.py` & `redvox-3.4.1/redvox/api900/types.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/api900/wrapped_redvox_packet.py` & `redvox-3.4.1/redvox/api900/wrapped_redvox_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cli/cli.py` & `redvox-3.4.1/redvox/cli/cli.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cli/conversions.py` & `redvox-3.4.1/redvox/cli/conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cli/data_req.py` & `redvox-3.4.1/redvox/cli/data_req.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/api.py` & `redvox-3.4.1/redvox/cloud/api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/api_m_fqns.py` & `redvox-3.4.1/redvox/cloud/api_m_fqns.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/auth_api.py` & `redvox-3.4.1/redvox/cloud/auth_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/client.py` & `redvox-3.4.1/redvox/cloud/client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/config.py` & `redvox-3.4.1/redvox/cloud/config.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/data_api.py` & `redvox-3.4.1/redvox/cloud/data_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/data_client.py` & `redvox-3.4.1/redvox/cloud/data_client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/data_io.py` & `redvox-3.4.1/redvox/cloud/data_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/metadata_api.py` & `redvox-3.4.1/redvox/cloud/metadata_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/query_timing_correction.py` & `redvox-3.4.1/redvox/cloud/query_timing_correction.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/routes.py` & `redvox-3.4.1/redvox/cloud/routes.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/station_stats.py` & `redvox-3.4.1/redvox/cloud/station_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/cloud/subscription.py` & `redvox-3.4.1/redvox/cloud/subscription.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/api_conversions.py` & `redvox-3.4.1/redvox/common/api_conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/api_reader.py` & `redvox-3.4.1/redvox/common/api_reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/api_reader_dw.py` & `redvox-3.4.1/redvox/common/api_reader_dw.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/api_reader_old.py` & `redvox-3.4.1/redvox/common/api_reader_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/constants.py` & `redvox-3.4.1/redvox/common/constants.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/cross_stats.py` & `redvox-3.4.1/redvox/common/cross_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/data_window.py` & `redvox-3.4.1/redvox/common/data_window.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/data_window_configuration.py` & `redvox-3.4.1/redvox/common/data_window_configuration.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/data_window_configuration_old.py` & `redvox-3.4.1/redvox/common/data_window_configuration_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/data_window_io.py` & `redvox-3.4.1/redvox/common/data_window_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/data_window_old.py` & `redvox-3.4.1/redvox/common/data_window_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/date_time_utils.py` & `redvox-3.4.1/redvox/common/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/errors.py` & `redvox-3.4.1/redvox/common/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/event_stream.py` & `redvox-3.4.1/redvox/common/event_stream.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/event_stream_io.py` & `redvox-3.4.1/redvox/common/event_stream_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/file_statistics.py` & `redvox-3.4.1/redvox/common/file_statistics.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/gap_and_pad_utils.py` & `redvox-3.4.1/redvox/common/gap_and_pad_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/gap_and_pad_utils_old.py` & `redvox-3.4.1/redvox/common/gap_and_pad_utils_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/gui/cloud_data_retrieval.py` & `redvox-3.4.1/redvox/common/gui/cloud_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/io.py` & `redvox-3.4.1/redvox/common/io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/offset_model.py` & `redvox-3.4.1/redvox/common/offset_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/packet_to_pyarrow.py` & `redvox-3.4.1/redvox/common/packet_to_pyarrow.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/parallel_utils.py` & `redvox-3.4.1/redvox/common/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/run_me.py` & `redvox-3.4.1/redvox/common/run_me.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/sensor_data.py` & `redvox-3.4.1/redvox/common/sensor_data.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/sensor_data_old.py` & `redvox-3.4.1/redvox/common/sensor_data_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/sensor_io.py` & `redvox-3.4.1/redvox/common/sensor_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/sensor_reader_utils.py` & `redvox-3.4.1/redvox/common/sensor_reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/sensor_reader_utils_old.py` & `redvox-3.4.1/redvox/common/sensor_reader_utils_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/session_io.py` & `redvox-3.4.1/redvox/common/session_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/session_model.py` & `redvox-3.4.1/redvox/common/session_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/session_model_utils.py` & `redvox-3.4.1/redvox/common/session_model_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/station.py` & `redvox-3.4.1/redvox/common/station.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/station_io.py` & `redvox-3.4.1/redvox/common/station_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/station_model.py` & `redvox-3.4.1/redvox/common/station_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/station_old.py` & `redvox-3.4.1/redvox/common/station_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/station_utils.py` & `redvox-3.4.1/redvox/common/station_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/stats_helper.py` & `redvox-3.4.1/redvox/common/stats_helper.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/timesync.py` & `redvox-3.4.1/redvox/common/timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/timesync_io.py` & `redvox-3.4.1/redvox/common/timesync_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/timesync_old.py` & `redvox-3.4.1/redvox/common/timesync_old.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/tri_message_stats.py` & `redvox-3.4.1/redvox/common/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/common/versioning.py` & `redvox-3.4.1/redvox/common/versioning.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox/settings.py` & `redvox-3.4.1/redvox/settings.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.0a3/redvox.egg-info/PKG-INFO` & `redvox-3.4.1/redvox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.4.0a3
+Version: 3.4.1
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.4.0a3/redvox.egg-info/SOURCES.txt` & `redvox-3.4.1/redvox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

