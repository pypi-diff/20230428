# Comparing `tmp/zaber_motion-3.2.1.tar.gz` & `tmp/zaber_motion-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-3.2.1.tar", last modified: Wed Apr  5 19:44:55 2023, max compression
+gzip compressed data, was "zaber_motion-3.3.0.tar", last modified: Fri Apr 28 18:32:16 2023, max compression
```

## Comparing `zaber_motion-3.2.1.tar` & `zaber_motion-3.3.0.tar`

### file list

```diff
@@ -1,170 +1,171 @@
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.699548 zaber_motion-3.2.1/
--rw-r--r--   0 zaber      (501) staff       (20)      236 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/DESCRIPTION.md
--rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/LICENSE.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/MANIFEST.in
--rw-r--r--   0 zaber      (501) staff       (20)      826 2023-04-05 19:44:55.699611 zaber_motion-3.2.1/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)      236 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/README.md
--rw-r--r--   0 zaber      (501) staff       (20)      134 2023-04-05 19:44:55.699852 zaber_motion-3.2.1/setup.cfg
--rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/setup.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.679755 zaber_motion-3.2.1/test/
--rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/test/test_integration.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.681638 zaber_motion-3.2.1/zaber_motion/
--rw-r--r--   0 zaber      (501) staff       (20)     5674 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/__init__.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.687344 zaber_motion-3.2.1/zaber_motion/ascii/
--rw-r--r--   0 zaber      (501) staff       (20)     2337 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/alert_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/all_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)    40795 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/axis.py
--rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/axis_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    12689 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/axis_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      272 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/can_set_state_axis_response.py
--rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/can_set_state_device_response.py
--rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)     1887 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/conversion_factor.py
--rw-r--r--   0 zaber      (501) staff       (20)    21653 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/device_io.py
--rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/device_io_info.py
--rw-r--r--   0 zaber      (501) staff       (20)    10347 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)    32387 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/lockstep.py
--rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/lockstep_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/message_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    15804 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/oscilloscope.py
--rw-r--r--   0 zaber      (501) staff       (20)     1303 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-r--r--   0 zaber      (501) staff       (20)     4860 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/oscilloscope_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/paramset_info.py
--rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/pid_tuning.py
--rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/response.py
--rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/servo_tuner.py
--rw-r--r--   0 zaber      (501) staff       (20)     1801 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/servo_tuning_param.py
--rw-r--r--   0 zaber      (501) staff       (20)      384 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/servo_tuning_paramset.py
--rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/setting_constants.py
--rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/storage.py
--rw-r--r--   0 zaber      (501) staff       (20)    74838 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/stream.py
--rw-r--r--   0 zaber      (501) staff       (20)     2133 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/stream_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      253 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/stream_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3080 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/stream_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      273 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/stream_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/transport.py
--rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/warning_flags.py
--rw-r--r--   0 zaber      (501) staff       (20)     3218 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/ascii/warnings.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.688956 zaber_motion-3.2.1/zaber_motion/binary/
--rw-r--r--   0 zaber      (501) staff       (20)      653 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/binary_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/command_code.py
--rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)    28560 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)     3346 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      276 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/device_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/error_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/message.py
--rw-r--r--   0 zaber      (501) staff       (20)      415 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/reply_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/reply_only_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/binary/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/bindings.py
--rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/call.py
--rw-r--r--   0 zaber      (501) staff       (20)     6361 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/convert_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      257 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/device_db_source_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/events.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.697514 zaber_motion-3.2.1/zaber_motion/exceptions/
--rw-r--r--   0 zaber      (501) staff       (20)     6252 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      991 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1840 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/command_preempted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/command_too_long_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      304 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/connection_closed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/connection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/conversion_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      314 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/device_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/device_db_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      911 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      283 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/device_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/device_not_identified_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/g_code_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      309 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/internal_error_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      295 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/invalid_argument_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/invalid_data_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      310 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/invalid_operation_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/invalid_packet_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/invalid_response_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      928 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      342 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/io_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      322 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      329 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      396 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/motion_lib_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/no_device_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/not_supported_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/os_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/request_timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      349 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3228 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/setting_not_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/stream_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/stream_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/transport_already_used_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/exceptions/unknown_request_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1338 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/firmware_version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.698701 zaber_motion-3.2.1/zaber_motion/gcode/
--rw-r--r--   0 zaber      (501) staff       (20)      578 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2269 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)     1571 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/axis_mapping.py
--rw-r--r--   0 zaber      (501) staff       (20)     2170 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/axis_transformation.py
--rw-r--r--   0 zaber      (501) staff       (20)     2313 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/device_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    12275 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/offline_translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/translate_message.py
--rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/translate_result.py
--rw-r--r--   0 zaber      (501) staff       (20)    12899 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     2225 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/gcode/translator_config.py
--rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/library.py
--rw-r--r--   0 zaber      (501) staff       (20)      279 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/log_output_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     1519 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/measurement.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.698947 zaber_motion-3.2.1/zaber_motion/microscopy/
--rw-r--r--   0 zaber      (501) staff       (20)       68 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/microscopy/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.699326 zaber_motion-3.2.1/zaber_motion/protobufs/
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/protobufs/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)    61630 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/protobufs/main_pb2.py
--rw-r--r--   0 zaber      (501) staff       (20)   187641 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/protobufs/main_pb2.pyi
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/py.typed
--rw-r--r--   0 zaber      (501) staff       (20)      278 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/rotation_direction.py
--rw-r--r--   0 zaber      (501) staff       (20)      987 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/serialization.py
--rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/tools.py
--rw-r--r--   0 zaber      (501) staff       (20)     5744 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/units.py
--rw-r--r--   0 zaber      (501) staff       (20)       22 2023-04-05 19:43:55.000000 zaber_motion-3.2.1/zaber_motion/version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-05 19:44:55.682224 zaber_motion-3.2.1/zaber_motion.egg-info/
--rw-r--r--   0 zaber      (501) staff       (20)      826 2023-04-05 19:44:55.000000 zaber_motion-3.2.1/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)     6753 2023-04-05 19:44:55.000000 zaber_motion-3.2.1/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 zaber      (501) staff       (20)        1 2023-04-05 19:44:55.000000 zaber_motion-3.2.1/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 zaber      (501) staff       (20)      239 2023-04-05 19:44:55.000000 zaber_motion-3.2.1/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-04-05 19:44:55.000000 zaber_motion-3.2.1/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.371494 zaber_motion-3.3.0/
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/DESCRIPTION.md
+-rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/LICENSE.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/MANIFEST.in
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-04-28 18:32:16.371584 zaber_motion-3.3.0/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/README.md
+-rw-r--r--   0 zaber      (501) staff       (20)      134 2023-04-28 18:32:16.371935 zaber_motion-3.3.0/setup.cfg
+-rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/setup.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.331669 zaber_motion-3.3.0/test/
+-rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/test/test_integration.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.335566 zaber_motion-3.3.0/zaber_motion/
+-rw-r--r--   0 zaber      (501) staff       (20)     5735 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/__init__.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.348326 zaber_motion-3.3.0/zaber_motion/ascii/
+-rw-r--r--   0 zaber      (501) staff       (20)     2337 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/alert_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/all_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)    40795 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/axis.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/axis_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12689 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/axis_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      272 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/can_set_state_device_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1887 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/conversion_factor.py
+-rw-r--r--   0 zaber      (501) staff       (20)    23731 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device_io.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device_io_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)    10347 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)    36231 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/lockstep.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/lockstep_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/message_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    15804 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1303 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4860 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/paramset_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/pid_tuning.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/servo_tuner.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1801 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/servo_tuning_param.py
+-rw-r--r--   0 zaber      (501) staff       (20)      384 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/setting_constants.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/storage.py
+-rw-r--r--   0 zaber      (501) staff       (20)    74838 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2133 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      253 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3080 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      273 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/transport.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/warning_flags.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/warnings.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.351203 zaber_motion-3.3.0/zaber_motion/binary/
+-rw-r--r--   0 zaber      (501) staff       (20)      653 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/binary_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/command_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)    28560 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3346 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      276 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/device_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/error_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/message.py
+-rw-r--r--   0 zaber      (501) staff       (20)      415 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/reply_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/reply_only_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/bindings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/call.py
+-rw-r--r--   0 zaber      (501) staff       (20)     6453 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/convert_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      257 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/device_db_source_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/events.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.367318 zaber_motion-3.3.0/zaber_motion/exceptions/
+-rw-r--r--   0 zaber      (501) staff       (20)     6320 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      991 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1840 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_preempted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_too_long_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      304 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/connection_closed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/connection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      314 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      911 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      283 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      309 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/internal_error_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      295 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_data_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      310 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_response_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      928 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      342 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/io_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      322 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      329 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      396 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/motion_lib_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/no_device_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/not_supported_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/os_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/request_timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      349 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3228 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      341 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/unknown_request_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2106 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/firmware_version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.369428 zaber_motion-3.3.0/zaber_motion/gcode/
+-rw-r--r--   0 zaber      (501) staff       (20)      578 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2269 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1571 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/axis_mapping.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2170 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/axis_transformation.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2313 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/device_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12275 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/offline_translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/translate_message.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/translate_result.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12899 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2225 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/translator_config.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/library.py
+-rw-r--r--   0 zaber      (501) staff       (20)      279 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/log_output_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1519 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/measurement.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.369862 zaber_motion-3.3.0/zaber_motion/microscopy/
+-rw-r--r--   0 zaber      (501) staff       (20)       68 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/microscopy/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.370685 zaber_motion-3.3.0/zaber_motion/protobufs/
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/protobufs/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)    62415 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/protobufs/main_pb2.py
+-rw-r--r--   0 zaber      (501) staff       (20)   190301 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/protobufs/main_pb2.pyi
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/py.typed
+-rw-r--r--   0 zaber      (501) staff       (20)      278 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/rotation_direction.py
+-rw-r--r--   0 zaber      (501) staff       (20)      987 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/serialization.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/tools.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5744 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/units.py
+-rw-r--r--   0 zaber      (501) staff       (20)       22 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.336507 zaber_motion-3.3.0/zaber_motion.egg-info/
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)     6798 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 zaber      (501) staff       (20)        1 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 zaber      (501) staff       (20)      239 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-3.2.1/LICENSE.txt` & `zaber_motion-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/PKG-INFO` & `zaber_motion-3.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 3.2.1
+Version: 3.3.0
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,8 +15,8 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Zaber Motion Library
 
 Zaber Motion Library is a multi-platform library used to operate Zaber devices.
 
-Official documentation: [https://www.zaber.com/software/docs/motion-library/](https://www.zaber.com/software/docs/motion-library/)
+Official documentation: [https://software.zaber.com/motion-library/](https://software.zaber.com/motion-library/)
```

### Comparing `zaber_motion-3.2.1/setup.py` & `zaber_motion-3.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read_from_file(*filename):
     with open(path.join(*filename), 'r') as f:
         return f.read()
 
 
 setup(
     name='zaber_motion',
-    version='3.2.1',
+    version='3.3.0',
     packages=find_packages(exclude=["test*", "test_*", "*_test*"]),
     package_data={
         '': ['*.pyi', 'py.typed']
     },
     description='A library for communicating with Zaber devices',
     long_description=read_from_file('DESCRIPTION.md'),
     long_description_content_type="text/markdown",
@@ -32,12 +32,12 @@
         'License :: OSI Approved :: MIT License',
     ],
     keywords='',
     python_requires='>=3.7',
     install_requires=[
         'protobuf>=3.20.0,<4.22.0',
         'rx>=3.0.0',
-        'zaber_motion_bindings_windows==3.2.1;platform_system=="Windows"',
-        'zaber_motion_bindings_linux==3.2.1;platform_system=="Linux"',
-        'zaber_motion_bindings_darwin==3.2.1;platform_system=="Darwin"',
+        'zaber_motion_bindings_windows==3.3.0;platform_system=="Windows"',
+        'zaber_motion_bindings_linux==3.3.0;platform_system=="Linux"',
+        'zaber_motion_bindings_darwin==3.3.0;platform_system=="Darwin"',
     ],
 )
```

### Comparing `zaber_motion-3.2.1/test/test_integration.py` & `zaber_motion-3.3.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/__init__.py` & `zaber_motion-3.3.0/zaber_motion/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 from .exceptions import SetPeripheralStateFailedException as SetPeripheralStateFailedException
 from .exceptions import SettingNotFoundException as SettingNotFoundException
 from .exceptions import StreamExecutionException as StreamExecutionException
 from .exceptions import StreamModeException as StreamModeException
 from .exceptions import StreamMovementFailedException as StreamMovementFailedException
 from .exceptions import StreamMovementInterruptedException as StreamMovementInterruptedException
 from .exceptions import StreamSetupFailedException as StreamSetupFailedException
+from .exceptions import TimeoutException as TimeoutException
 from .exceptions import TransportAlreadyUsedException as TransportAlreadyUsedException
 from .exceptions import UnknownRequestException as UnknownRequestException
 from .exceptions import BinaryCommandFailedExceptionData as BinaryCommandFailedExceptionData
 from .exceptions import CommandFailedExceptionData as CommandFailedExceptionData
 from .exceptions import CommandTooLongExceptionData as CommandTooLongExceptionData
 from .exceptions import DeviceAddressConflictExceptionData as DeviceAddressConflictExceptionData
 from .exceptions import DeviceDbFailedExceptionData as DeviceDbFailedExceptionData
```

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/__init__.py` & `zaber_motion-3.3.0/zaber_motion/ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/alert_event.py` & `zaber_motion-3.3.0/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/all_axes.py` & `zaber_motion-3.3.0/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/axis.py` & `zaber_motion-3.3.0/zaber_motion/ascii/axis.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/axis_identity.py` & `zaber_motion-3.3.0/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/axis_settings.py` & `zaber_motion-3.3.0/zaber_motion/ascii/axis_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-3.3.0/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-3.3.0/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/connection.py` & `zaber_motion-3.3.0/zaber_motion/ascii/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-3.3.0/zaber_motion/ascii/conversion_factor.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/device.py` & `zaber_motion-3.3.0/zaber_motion/ascii/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Optional
 from ..call import call, call_async, call_sync
 
 from ..protobufs import main_pb2
 from .device_settings import DeviceSettings
 from .axis import Axis
 from .all_axes import AllAxes
 from .warnings import Warnings
@@ -151,45 +151,59 @@
         self._storage = DeviceStorage(self)
         self._io = DeviceIO(self)
         self._all_axes = AllAxes(self)
         self._warnings = Warnings(self, 0)
         self._oscilloscope = Oscilloscope(self)
 
     def identify(
-            self
+            self,
+            assume_version: Optional[FirmwareVersion] = None
     ) -> DeviceIdentity:
         """
         Queries the device and the database, gathering information about the product.
         Without this information features such as unit conversions will not work.
         Usually, called automatically by detect devices method.
 
+        Args:
+            assume_version: The identification assumes the specified firmware version
+                instead of the version queried from the device.
+                Providing this argument can lead to unexpected compatibility issues.
+
         Returns:
             Device identification data.
         """
-        request = main_pb2.DeviceEmptyRequest()
+        request = main_pb2.DeviceIdentifyRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
+        request.assume_version.CopyFrom(FirmwareVersion.to_protobuf(assume_version))
         response = main_pb2.DeviceIdentity()
         call("device/identify", request, response)
         return DeviceIdentity.from_protobuf(response)
 
     async def identify_async(
-            self
+            self,
+            assume_version: Optional[FirmwareVersion] = None
     ) -> DeviceIdentity:
         """
         Queries the device and the database, gathering information about the product.
         Without this information features such as unit conversions will not work.
         Usually, called automatically by detect devices method.
 
+        Args:
+            assume_version: The identification assumes the specified firmware version
+                instead of the version queried from the device.
+                Providing this argument can lead to unexpected compatibility issues.
+
         Returns:
             Device identification data.
         """
-        request = main_pb2.DeviceEmptyRequest()
+        request = main_pb2.DeviceIdentifyRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
+        request.assume_version.CopyFrom(FirmwareVersion.to_protobuf(assume_version))
         response = main_pb2.DeviceIdentity()
         await call_async("device/identify", request, response)
         return DeviceIdentity.from_protobuf(response)
 
     def generic_command(
             self,
             command: str,
@@ -591,14 +605,50 @@
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.state = state
         response = main_pb2.CanSetStateDeviceResponse()
         await call_async("device/can_set_state", request, response)
         return CanSetStateDeviceResponse.from_protobuf(response)
 
+    def wait_to_respond(
+            self,
+            timeout: float
+    ) -> None:
+        """
+        Waits for the device to start responding to messages.
+        Useful to call after resetting the device.
+        Throws RequestTimeoutException upon timeout.
+
+        Args:
+            timeout: For how long to wait in milliseconds for the device to start responding.
+        """
+        request = main_pb2.WaitToRespondRequest()
+        request.interface_id = self.connection.interface_id
+        request.device = self.device_address
+        request.timeout = timeout
+        call("device/wait_to_respond", request)
+
+    async def wait_to_respond_async(
+            self,
+            timeout: float
+    ) -> None:
+        """
+        Waits for the device to start responding to messages.
+        Useful to call after resetting the device.
+        Throws RequestTimeoutException upon timeout.
+
+        Args:
+            timeout: For how long to wait in milliseconds for the device to start responding.
+        """
+        request = main_pb2.WaitToRespondRequest()
+        request.interface_id = self.connection.interface_id
+        request.device = self.device_address
+        request.timeout = timeout
+        await call_async("device/wait_to_respond", request)
+
     def __retrieve_identity(
             self
     ) -> DeviceIdentity:
         """
         Returns identity.
 
         Returns:
```

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/device_identity.py` & `zaber_motion-3.3.0/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/device_io.py` & `zaber_motion-3.3.0/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/device_io_info.py` & `zaber_motion-3.3.0/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/device_settings.py` & `zaber_motion-3.3.0/zaber_motion/ascii/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/lockstep.py` & `zaber_motion-3.3.0/zaber_motion/ascii/lockstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -674,92 +674,194 @@
             unit: Units = Units.NATIVE
     ) -> List[float]:
         """
         Gets the initial offsets of secondary axes of an enabled lockstep group.
 
         Args:
             unit: Units of position.
+                Uses primary axis unit conversion.
 
         Returns:
             Initial offset for each axis of the lockstep group.
         """
-        request = main_pb2.LockstepGetOffsetsRequest()
+        request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.unit = unit.value
-        response = main_pb2.LockstepGetOffsetsResponse()
+        response = main_pb2.DoubleArrayResponse()
         call("device/lockstep_get_offsets", request, response)
-        return list(response.offsets)
+        return list(response.values)
 
     async def get_offsets_async(
             self,
             unit: Units = Units.NATIVE
     ) -> List[float]:
         """
         Gets the initial offsets of secondary axes of an enabled lockstep group.
 
         Args:
             unit: Units of position.
+                Uses primary axis unit conversion.
 
         Returns:
             Initial offset for each axis of the lockstep group.
         """
-        request = main_pb2.LockstepGetOffsetsRequest()
+        request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.unit = unit.value
-        response = main_pb2.LockstepGetOffsetsResponse()
+        response = main_pb2.DoubleArrayResponse()
         await call_async("device/lockstep_get_offsets", request, response)
-        return list(response.offsets)
+        return list(response.values)
 
     def get_twists(
             self,
             unit: Units = Units.NATIVE
     ) -> List[float]:
         """
         Gets the twists of secondary axes of an enabled lockstep group.
 
         Args:
             unit: Units of position.
+                Uses primary axis unit conversion.
 
         Returns:
             Difference between the initial offset and the actual offset for each axis of the lockstep group.
         """
-        request = main_pb2.LockstepGetTwistsRequest()
+        request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.unit = unit.value
-        response = main_pb2.LockstepGetTwistsResponse()
+        response = main_pb2.DoubleArrayResponse()
         call("device/lockstep_get_twists", request, response)
-        return list(response.twists)
+        return list(response.values)
 
     async def get_twists_async(
             self,
             unit: Units = Units.NATIVE
     ) -> List[float]:
         """
         Gets the twists of secondary axes of an enabled lockstep group.
 
         Args:
             unit: Units of position.
+                Uses primary axis unit conversion.
 
         Returns:
             Difference between the initial offset and the actual offset for each axis of the lockstep group.
         """
-        request = main_pb2.LockstepGetTwistsRequest()
+        request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.unit = unit.value
-        response = main_pb2.LockstepGetTwistsResponse()
+        response = main_pb2.DoubleArrayResponse()
         await call_async("device/lockstep_get_twists", request, response)
-        return list(response.twists)
+        return list(response.values)
+
+    def get_position(
+            self,
+            unit: Units = Units.NATIVE
+    ) -> float:
+        """
+        Returns current position of the primary axis.
+
+        Args:
+            unit: Units of the position.
+
+        Returns:
+            Primary axis position.
+        """
+        request = main_pb2.LockstepGetRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.lockstep_group_id = self.lockstep_group_id
+        request.unit = unit.value
+        response = main_pb2.DoubleResponse()
+        call("device/lockstep_get_pos", request, response)
+        return response.value
+
+    async def get_position_async(
+            self,
+            unit: Units = Units.NATIVE
+    ) -> float:
+        """
+        Returns current position of the primary axis.
+
+        Args:
+            unit: Units of the position.
+
+        Returns:
+            Primary axis position.
+        """
+        request = main_pb2.LockstepGetRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.lockstep_group_id = self.lockstep_group_id
+        request.unit = unit.value
+        response = main_pb2.DoubleResponse()
+        await call_async("device/lockstep_get_pos", request, response)
+        return response.value
+
+    def set_tolerance(
+            self,
+            tolerance: float,
+            unit: Units = Units.NATIVE,
+            axis_index: int = 0
+    ) -> None:
+        """
+        Sets lockstep twist tolerance.
+        Twist tolerances that do not match the system configuration can reduce performance or damage the system.
+
+        Args:
+            tolerance: Twist tolerance.
+            unit: Units of the tolerance.
+                Uses primary axis unit conversion when setting to all axes,
+                otherwise uses specified secondary axis unit conversion.
+            axis_index: Optional index of a secondary axis to set the tolerance for.
+                If left empty or set to 0, the tolerance is set to all the secondary axes.
+        """
+        request = main_pb2.LockstepSetRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.lockstep_group_id = self.lockstep_group_id
+        request.value = tolerance
+        request.unit = unit.value
+        request.axis_index = axis_index
+        call("device/lockstep_set_tolerance", request)
+
+    async def set_tolerance_async(
+            self,
+            tolerance: float,
+            unit: Units = Units.NATIVE,
+            axis_index: int = 0
+    ) -> None:
+        """
+        Sets lockstep twist tolerance.
+        Twist tolerances that do not match the system configuration can reduce performance or damage the system.
+
+        Args:
+            tolerance: Twist tolerance.
+            unit: Units of the tolerance.
+                Uses primary axis unit conversion when setting to all axes,
+                otherwise uses specified secondary axis unit conversion.
+            axis_index: Optional index of a secondary axis to set the tolerance for.
+                If left empty or set to 0, the tolerance is set to all the secondary axes.
+        """
+        request = main_pb2.LockstepSetRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.lockstep_group_id = self.lockstep_group_id
+        request.value = tolerance
+        request.unit = unit.value
+        request.axis_index = axis_index
+        await call_async("device/lockstep_set_tolerance", request)
 
     def is_enabled(
             self
     ) -> bool:
         """
         Checks if the lockstep group is currently enabled on the device.
```

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-3.3.0/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/paramset_info.py` & `zaber_motion-3.3.0/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-3.3.0/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/response.py` & `zaber_motion-3.3.0/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-3.3.0/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-3.3.0/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/setting_constants.py` & `zaber_motion-3.3.0/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-3.3.0/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/storage.py` & `zaber_motion-3.3.0/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/stream.py` & `zaber_motion-3.3.0/zaber_motion/ascii/stream.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-3.3.0/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-3.3.0/zaber_motion/ascii/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/transport.py` & `zaber_motion-3.3.0/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-3.3.0/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/ascii/warning_flags.py` & `zaber_motion-3.3.0/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/__init__.py` & `zaber_motion-3.3.0/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/binary_settings.py` & `zaber_motion-3.3.0/zaber_motion/binary/binary_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/command_code.py` & `zaber_motion-3.3.0/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/connection.py` & `zaber_motion-3.3.0/zaber_motion/binary/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/device.py` & `zaber_motion-3.3.0/zaber_motion/binary/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/device_identity.py` & `zaber_motion-3.3.0/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/device_settings.py` & `zaber_motion-3.3.0/zaber_motion/binary/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/error_code.py` & `zaber_motion-3.3.0/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/message.py` & `zaber_motion-3.3.0/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/reply_only_event.py` & `zaber_motion-3.3.0/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-3.3.0/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/bindings.py` & `zaber_motion-3.3.0/zaber_motion/bindings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/call.py` & `zaber_motion-3.3.0/zaber_motion/call.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/convert_exception.py` & `zaber_motion-3.3.0/zaber_motion/convert_exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from .exceptions.set_peripheral_state_failed_exception import SetPeripheralStateFailedException
 from .exceptions.setting_not_found_exception import SettingNotFoundException
 from .exceptions.stream_execution_exception import StreamExecutionException
 from .exceptions.stream_mode_exception import StreamModeException
 from .exceptions.stream_movement_failed_exception import StreamMovementFailedException
 from .exceptions.stream_movement_interrupted_exception import StreamMovementInterruptedException
 from .exceptions.stream_setup_failed_exception import StreamSetupFailedException
+from .exceptions.timeout_exception import TimeoutException
 from .exceptions.transport_already_used_exception import TransportAlreadyUsedException
 from .exceptions.unknown_request_exception import UnknownRequestException
 
 errorMap = {
     "BINARY_COMMAND_FAILED": BinaryCommandFailedException,
     "COMMAND_FAILED": CommandFailedException,
     "COMMAND_PREEMPTED": CommandPreemptedException,
@@ -89,14 +90,15 @@
     "SET_PERIPHERAL_STATE_FAILED": SetPeripheralStateFailedException,
     "SETTING_NOT_FOUND": SettingNotFoundException,
     "STREAM_EXECUTION": StreamExecutionException,
     "STREAM_MODE": StreamModeException,
     "STREAM_MOVEMENT_FAILED": StreamMovementFailedException,
     "STREAM_MOVEMENT_INTERRUPTED": StreamMovementInterruptedException,
     "STREAM_SETUP_FAILED": StreamSetupFailedException,
+    "TIMEOUT": TimeoutException,
     "TRANSPORT_ALREADY_USED": TransportAlreadyUsedException,
     "UNKNOWN_REQUEST": UnknownRequestException,
 }
 
 
 def convert_exception(error_type: int, message: str, custom_data: Optional[bytes] = None) -> MotionLibException:
     if custom_data:
```

### Comparing `zaber_motion-3.2.1/zaber_motion/events.py` & `zaber_motion-3.3.0/zaber_motion/events.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/__init__.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from .set_peripheral_state_failed_exception import SetPeripheralStateFailedException as SetPeripheralStateFailedException
 from .setting_not_found_exception import SettingNotFoundException as SettingNotFoundException
 from .stream_execution_exception import StreamExecutionException as StreamExecutionException
 from .stream_mode_exception import StreamModeException as StreamModeException
 from .stream_movement_failed_exception import StreamMovementFailedException as StreamMovementFailedException
 from .stream_movement_interrupted_exception import StreamMovementInterruptedException as StreamMovementInterruptedException
 from .stream_setup_failed_exception import StreamSetupFailedException as StreamSetupFailedException
+from .timeout_exception import TimeoutException as TimeoutException
 from .transport_already_used_exception import TransportAlreadyUsedException as TransportAlreadyUsedException
 from .unknown_request_exception import UnknownRequestException as UnknownRequestException
 from .motion_lib_exception import MotionLibException as MotionLibException
 
 from .binary_command_failed_exception_data import BinaryCommandFailedExceptionData as BinaryCommandFailedExceptionData
 from .command_failed_exception_data import CommandFailedExceptionData as CommandFailedExceptionData
 from .command_too_long_exception_data import CommandTooLongExceptionData as CommandTooLongExceptionData
```

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/__init__.py` & `zaber_motion-3.3.0/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/axis_definition.py` & `zaber_motion-3.3.0/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-3.3.0/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-3.3.0/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/device_definition.py` & `zaber_motion-3.3.0/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/offline_translator.py` & `zaber_motion-3.3.0/zaber_motion/gcode/offline_translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/translate_message.py` & `zaber_motion-3.3.0/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/translate_result.py` & `zaber_motion-3.3.0/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/translator.py` & `zaber_motion-3.3.0/zaber_motion/gcode/translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/gcode/translator_config.py` & `zaber_motion-3.3.0/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/library.py` & `zaber_motion-3.3.0/zaber_motion/library.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/measurement.py` & `zaber_motion-3.3.0/zaber_motion/measurement.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-3.3.0/zaber_motion/microscopy/objective_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-3.3.0/zaber_motion/protobufs/main_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,430 +9,434 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\"*\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x03 \x01(\t\x12\x0e\n\x06reason\x18\x04 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"m\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x05 \x01(\t\x12\x0e\n\x06status\x18\x06 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x07 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xe8\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"E\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"i\n\x18LockstepGetTwistsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"+\n\x19LockstepGetTwistsResponse\x12\x0e\n\x06twists\x18\x01 \x03(\x01\"j\n\x19LockstepGetOffsetsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"-\n\x1aLockstepGetOffsetsResponse\x12\x0f\n\x07offsets\x18\x01 \x03(\x01\"d\n\x1dOscilloscopeAddChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"E\n\x1dOscilloscopeCaptureProperties\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x02 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"_\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"\x96\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12:\n\x04\x61xes\x18\x04 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"w\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xae\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x8a\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12\x12\n\naxes_count\x18\x05 \x01(\x05\"c\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\"\xf8\x01\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12<\n\x04type\x18\x04 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x06 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xb1\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12;\n\x04type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x05 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x06 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\n \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xcf\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12>\n\x04type\x18\x04 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x05 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x06 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x08 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x7f\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x08\"\x91\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\x11\n\tcondition\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\"\x7f\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x08\"~\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x01\"s\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"l\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0e\n\x06values\x18\x04 \x03(\x08\"k\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0e\n\x06values\x18\x04 \x03(\x01\"h\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"s\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"M\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"a\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"t\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x11\n\tmax_speed\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"r\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x97\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12#\n\x1bmax_tangential_acceleration\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"s\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x99\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12$\n\x1cmax_centripetal_acceleration\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"X\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"S\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\"g\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\"j\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\r\n\x05\x62\x61tch\x18\x04 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\x94\x08\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\"*\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x03 \x01(\t\x12\x0e\n\x06reason\x18\x04 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"m\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x05 \x01(\t\x12\x0e\n\x06status\x18\x06 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x07 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xe8\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"E\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"d\n\x1dOscilloscopeAddChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"E\n\x1dOscilloscopeCaptureProperties\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x02 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"_\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"\x96\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12:\n\x04\x61xes\x18\x04 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"w\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xae\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x8a\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12\x12\n\naxes_count\x18\x05 \x01(\x05\"c\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\"\xf8\x01\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12<\n\x04type\x18\x04 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x06 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xb1\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12;\n\x04type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x05 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x06 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\n \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xcf\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12>\n\x04type\x18\x04 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x05 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x06 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x08 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x7f\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x08\"\x91\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\x11\n\tcondition\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\"\x7f\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x08\"~\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x01\"s\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"l\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0e\n\x06values\x18\x04 \x03(\x08\"k\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0e\n\x06values\x18\x04 \x03(\x01\"h\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"s\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"M\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"a\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"t\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x11\n\tmax_speed\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"r\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x97\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12#\n\x1bmax_tangential_acceleration\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"s\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x99\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12$\n\x1cmax_centripetal_acceleration\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"X\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"S\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\"g\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\"j\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\r\n\x05\x62\x61tch\x18\x04 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xa1\x08\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protobufs.main_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\"./protobufs;zaber_motion_protobufs'
-  _MESSAGETYPE._serialized_start=20621
-  _MESSAGETYPE._serialized_end=20666
-  _ERRORS._serialized_start=20669
-  _ERRORS._serialized_end=21713
-  _INTERFACETYPE._serialized_start=21715
-  _INTERFACETYPE._serialized_end=21796
+  _MESSAGETYPE._serialized_start=20920
+  _MESSAGETYPE._serialized_end=20965
+  _ERRORS._serialized_start=20968
+  _ERRORS._serialized_end=22025
+  _INTERFACETYPE._serialized_start=22027
+  _INTERFACETYPE._serialized_end=22108
   _REQUEST._serialized_start=48
   _REQUEST._serialized_end=74
   _RESPONSE._serialized_start=77
   _RESPONSE._serialized_end=262
   _RESPONSE_RESPONSETYPE._serialized_start=229
   _RESPONSE_RESPONSETYPE._serialized_end=262
   _EVENT._serialized_start=264
   _EVENT._serialized_end=286
   _EMPTYREQUEST._serialized_start=288
   _EMPTYREQUEST._serialized_end=302
   _BOOLRESPONSE._serialized_start=304
   _BOOLRESPONSE._serialized_end=333
   _DOUBLERESPONSE._serialized_start=335
   _DOUBLERESPONSE._serialized_end=366
-  _INTRESPONSE._serialized_start=368
-  _INTRESPONSE._serialized_end=396
-  _STRINGRESPONSE._serialized_start=398
-  _STRINGRESPONSE._serialized_end=429
-  _STRINGARRAYRESPONSE._serialized_start=431
-  _STRINGARRAYRESPONSE._serialized_end=468
-  _AXISIDENTITY._serialized_start=471
-  _AXISIDENTITY._serialized_end=692
-  _AXISIDENTITY_AXISTYPE._serialized_start=645
-  _AXISIDENTITY_AXISTYPE._serialized_end=692
-  _DEVICEIDENTITY._serialized_start=695
-  _DEVICEIDENTITY._serialized_end=898
-  _FIRMWAREVERSION._serialized_start=900
-  _FIRMWAREVERSION._serialized_end=962
-  _DEVICEIOINFO._serialized_start=965
-  _DEVICEIOINFO._serialized_end=1103
-  _MEASUREMENT._serialized_start=1105
-  _MEASUREMENT._serialized_end=1147
-  _STREAMAXISDEFINITION._serialized_start=1149
-  _STREAMAXISDEFINITION._serialized_end=1211
-  _INVALIDPACKETEXCEPTIONDATA._serialized_start=1213
-  _INVALIDPACKETEXCEPTIONDATA._serialized_end=1273
-  _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_start=1275
-  _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_end=1337
-  _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1339
-  _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1437
-  _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1439
-  _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1513
-  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1515
-  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1608
-  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1610
-  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1679
-  _STREAMEXECUTIONEXCEPTIONDATA._serialized_start=1681
-  _STREAMEXECUTIONEXCEPTIONDATA._serialized_end=1747
-  _INVALIDRESPONSEEXCEPTIONDATA._serialized_start=1749
-  _INVALIDRESPONSEEXCEPTIONDATA._serialized_end=1797
-  _COMMANDFAILEDEXCEPTIONDATA._serialized_start=1799
-  _COMMANDFAILEDEXCEPTIONDATA._serialized_end=1908
-  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_start=1910
-  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_end=1967
-  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_start=1970
-  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_end=2107
-  _SETDEVICESTATEEXCEPTIONDATA._serialized_start=2110
-  _SETDEVICESTATEEXCEPTIONDATA._serialized_end=2342
-  _COMMANDTOOLONGEXCEPTIONDATA._serialized_start=2344
-  _COMMANDTOOLONGEXCEPTIONDATA._serialized_end=2447
-  _TESTREQUEST._serialized_start=2449
-  _TESTREQUEST._serialized_end=2535
-  _TESTRESPONSE._serialized_start=2537
-  _TESTRESPONSE._serialized_end=2570
-  _TESTRESPONSELONG._serialized_start=2572
-  _TESTRESPONSELONG._serialized_end=2609
-  _TESTEVENT._serialized_start=2611
-  _TESTEVENT._serialized_end=2636
-  _TOOLSLISTSERIALPORTSRESPONSE._serialized_start=2638
-  _TOOLSLISTSERIALPORTSRESPONSE._serialized_end=2683
-  _SETINTERNALMODEREQUEST._serialized_start=2685
-  _SETINTERNALMODEREQUEST._serialized_end=2723
-  _SETDEVICEDBSOURCEREQUEST._serialized_start=2725
-  _SETDEVICEDBSOURCEREQUEST._serialized_end=2798
-  _TOGGLEDEVICEDBSTOREREQUEST._serialized_start=2800
-  _TOGGLEDEVICEDBSTOREREQUEST._serialized_end=2871
-  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_start=2873
-  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_end=2916
-  _OPENINTERFACEREQUEST._serialized_start=2919
-  _OPENINTERFACEREQUEST._serialized_end=3214
-  _OPENINTERFACERESPONSE._serialized_start=3216
-  _OPENINTERFACERESPONSE._serialized_end=3261
-  _INTERFACEEMPTYREQUEST._serialized_start=3263
-  _INTERFACEEMPTYREQUEST._serialized_end=3308
-  _SETINTERFACETIMEOUTREQUEST._serialized_start=3310
-  _SETINTERFACETIMEOUTREQUEST._serialized_end=3377
-  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_start=3379
-  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_end=3457
-  _AXISEMPTYREQUEST._serialized_start=3459
-  _AXISEMPTYREQUEST._serialized_end=3529
-  _GENERICCOMMANDREQUEST._serialized_start=3532
-  _GENERICCOMMANDREQUEST._serialized_end=3663
-  _GENERICCOMMANDRESPONSE._serialized_start=3666
-  _GENERICCOMMANDRESPONSE._serialized_end=3866
-  _GENERICCOMMANDRESPONSECOLLECTION._serialized_start=3868
-  _GENERICCOMMANDRESPONSECOLLECTION._serialized_end=3969
-  _UNKNOWNRESPONSEEVENT._serialized_start=3972
-  _UNKNOWNRESPONSEEVENT._serialized_end=4192
-  _ALERTEVENT._serialized_start=4195
-  _ALERTEVENT._serialized_end=4326
-  _DISCONNECTEDEVENT._serialized_start=4328
-  _DISCONNECTEDEVENT._serialized_end=4444
-  _DEVICERENUMBERREQUEST._serialized_start=4446
-  _DEVICERENUMBERREQUEST._serialized_end=4514
-  _DEVICEDETECTREQUEST._serialized_start=4516
-  _DEVICEDETECTREQUEST._serialized_end=4585
-  _DEVICEDETECTRESPONSE._serialized_start=4587
-  _DEVICEDETECTRESPONSE._serialized_end=4626
-  _DEVICEHOMEREQUEST._serialized_start=4628
-  _DEVICEHOMEREQUEST._serialized_end=4724
-  _DEVICEWAITUNTILIDLEREQUEST._serialized_start=4726
-  _DEVICEWAITUNTILIDLEREQUEST._serialized_end=4836
-  _DEVICEMOVEREQUEST._serialized_start=4839
-  _DEVICEMOVEREQUEST._serialized_end=5175
-  _DEVICEMOVEREQUEST_MOVETYPE._serialized_start=5120
-  _DEVICEMOVEREQUEST_MOVETYPE._serialized_end=5175
-  _DEVICESTOPREQUEST._serialized_start=5177
-  _DEVICESTOPREQUEST._serialized_end=5273
-  _DEVICEONALLREQUEST._serialized_start=5275
-  _DEVICEONALLREQUEST._serialized_end=5342
-  _DEVICEONALLRESPONSE._serialized_start=5344
-  _DEVICEONALLRESPONSE._serialized_end=5391
-  _DEVICEGETWARNINGSREQUEST._serialized_start=5393
-  _DEVICEGETWARNINGSREQUEST._serialized_end=5486
-  _DEVICEGETWARNINGSRESPONSE._serialized_start=5488
-  _DEVICEGETWARNINGSRESPONSE._serialized_end=5530
-  _DEVICEGETALLDIGITALIOREQUEST._serialized_start=5532
-  _DEVICEGETALLDIGITALIOREQUEST._serialized_end=5622
-  _DEVICEGETALLDIGITALIORESPONSE._serialized_start=5624
-  _DEVICEGETALLDIGITALIORESPONSE._serialized_end=5671
-  _DEVICEGETALLANALOGIOREQUEST._serialized_start=5673
-  _DEVICEGETALLANALOGIOREQUEST._serialized_end=5762
-  _DEVICEGETALLANALOGIORESPONSE._serialized_start=5764
-  _DEVICEGETALLANALOGIORESPONSE._serialized_end=5810
-  _DEVICEGETDIGITALIOREQUEST._serialized_start=5812
-  _DEVICEGETDIGITALIOREQUEST._serialized_end=5923
-  _DEVICEGETANALOGIOREQUEST._serialized_start=5925
-  _DEVICEGETANALOGIOREQUEST._serialized_end=6035
-  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_start=6037
-  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_end=6126
-  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_start=6128
-  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_end=6216
-  _DEVICESETDIGITALOUTPUTREQUEST._serialized_start=6218
-  _DEVICESETDIGITALOUTPUTREQUEST._serialized_end=6326
-  _DEVICESETANALOGOUTPUTREQUEST._serialized_start=6328
-  _DEVICESETANALOGOUTPUTREQUEST._serialized_end=6435
-  _SETLOGOUTPUTREQUEST._serialized_start=6437
-  _SETLOGOUTPUTREQUEST._serialized_end=6491
-  _DEVICEGETSETTINGREQUEST._serialized_start=6493
-  _DEVICEGETSETTINGREQUEST._serialized_end=6601
-  _DEVICECONVERTSETTINGREQUEST._serialized_start=6604
-  _DEVICECONVERTSETTINGREQUEST._serialized_end=6752
-  _DEVICESETSETTINGREQUEST._serialized_start=6754
-  _DEVICESETSETTINGREQUEST._serialized_end=6877
-  _DEVICESETSETTINGSTRREQUEST._serialized_start=6879
-  _DEVICESETSETTINGSTRREQUEST._serialized_end=6991
-  _PREPARECOMMANDREQUEST._serialized_start=6994
-  _PREPARECOMMANDREQUEST._serialized_end=7152
-  _LOCKSTEPENABLEREQUEST._serialized_start=7154
-  _LOCKSTEPENABLEREQUEST._serialized_end=7256
-  _LOCKSTEPDISABLEREQUEST._serialized_start=7258
-  _LOCKSTEPDISABLEREQUEST._serialized_end=7372
-  _LOCKSTEPSTOPREQUEST._serialized_start=7374
-  _LOCKSTEPSTOPREQUEST._serialized_end=7485
-  _LOCKSTEPHOMEREQUEST._serialized_start=7487
-  _LOCKSTEPHOMEREQUEST._serialized_end=7598
-  _LOCKSTEPMOVEREQUEST._serialized_start=7601
-  _LOCKSTEPMOVEREQUEST._serialized_end=7954
-  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_start=5120
-  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_end=5175
-  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_start=7956
-  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_end=8081
-  _LOCKSTEPEMPTYREQUEST._serialized_start=8083
-  _LOCKSTEPEMPTYREQUEST._serialized_end=8170
-  _LOCKSTEPAXES._serialized_start=8172
-  _LOCKSTEPAXES._serialized_end=8250
-  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_start=8252
-  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_end=8298
-  _LOCKSTEPGETTWISTSREQUEST._serialized_start=8300
-  _LOCKSTEPGETTWISTSREQUEST._serialized_end=8405
-  _LOCKSTEPGETTWISTSRESPONSE._serialized_start=8407
-  _LOCKSTEPGETTWISTSRESPONSE._serialized_end=8450
-  _LOCKSTEPGETOFFSETSREQUEST._serialized_start=8452
-  _LOCKSTEPGETOFFSETSREQUEST._serialized_end=8558
-  _LOCKSTEPGETOFFSETSRESPONSE._serialized_start=8560
-  _LOCKSTEPGETOFFSETSRESPONSE._serialized_end=8605
-  _OSCILLOSCOPEADDCHANNELREQUEST._serialized_start=8607
-  _OSCILLOSCOPEADDCHANNELREQUEST._serialized_end=8707
-  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_start=8709
-  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_end=8816
-  _OSCILLOSCOPEREADRESPONSE._serialized_start=8818
-  _OSCILLOSCOPEREADRESPONSE._serialized_end=8862
-  _OSCILLOSCOPEDATAIDENTIFIER._serialized_start=8864
-  _OSCILLOSCOPEDATAIDENTIFIER._serialized_end=8909
-  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_start=8911
-  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_end=8980
-  _OSCILLOSCOPEDATAGETREQUEST._serialized_start=8982
-  _OSCILLOSCOPEDATAGETREQUEST._serialized_end=9041
-  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_start=9043
-  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_end=9127
-  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_start=9129
-  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_end=9179
-  _STREAMSETUPLIVEREQUEST._serialized_start=9181
-  _STREAMSETUPLIVEREQUEST._serialized_end=9276
-  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_start=9279
-  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_end=9429
-  _STREAMSETUPSTOREREQUEST._serialized_start=9431
-  _STREAMSETUPSTOREREQUEST._serialized_end=9550
-  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_start=9553
-  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_end=9727
-  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_start=9730
-  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_end=9868
-  _STREAMCALLREQUEST._serialized_start=9870
-  _STREAMCALLREQUEST._serialized_end=9969
-  _STREAMLINEREQUEST._serialized_start=9972
-  _STREAMLINEREQUEST._serialized_end=10220
-  _STREAMLINEREQUEST_TYPE._serialized_start=10196
-  _STREAMLINEREQUEST_TYPE._serialized_end=10220
-  _STREAMARCREQUEST._serialized_start=10223
-  _STREAMARCREQUEST._serialized_end=10656
-  _STREAMARCREQUEST_TYPE._serialized_start=10196
-  _STREAMARCREQUEST_TYPE._serialized_end=10220
-  _STREAMCIRCLEREQUEST._serialized_start=10659
-  _STREAMCIRCLEREQUEST._serialized_end=10994
-  _STREAMCIRCLEREQUEST_TYPE._serialized_start=10196
-  _STREAMCIRCLEREQUEST_TYPE._serialized_end=10220
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=10996
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=11123
-  _STREAMWAITANALOGINPUTREQUEST._serialized_start=11126
-  _STREAMWAITANALOGINPUTREQUEST._serialized_end=11271
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=11273
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=11400
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=11402
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=11528
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=11530
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=11645
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=11647
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=11755
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=11757
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=11864
-  _STREAMWAITREQUEST._serialized_start=11866
-  _STREAMWAITREQUEST._serialized_end=11970
-  _STREAMWAITUNTILIDLEREQUEST._serialized_start=11972
-  _STREAMWAITUNTILIDLEREQUEST._serialized_end=12087
-  _STREAMEMPTYREQUEST._serialized_start=12089
-  _STREAMEMPTYREQUEST._serialized_end=12166
-  _STREAMGETAXESRESPONSE._serialized_start=12168
-  _STREAMGETAXESRESPONSE._serialized_end=12251
-  _STREAMGETMAXSPEEDREQUEST._serialized_start=12253
-  _STREAMGETMAXSPEEDREQUEST._serialized_end=12350
-  _STREAMSETMAXSPEEDREQUEST._serialized_start=12352
-  _STREAMSETMAXSPEEDREQUEST._serialized_end=12468
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=12470
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=12584
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=12587
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=12738
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=12740
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=12855
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=12858
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=13011
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=13013
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=13101
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=13103
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=13157
-  _STREAMBUFFERERASEREQUEST._serialized_start=13159
-  _STREAMBUFFERERASEREQUEST._serialized_end=13242
-  _STREAMGENERICCOMMANDREQUEST._serialized_start=13244
-  _STREAMGENERICCOMMANDREQUEST._serialized_end=13347
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=13349
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=13455
-  _BINARYREPLYONLYEVENT._serialized_start=13457
-  _BINARYREPLYONLYEVENT._serialized_end=13556
-  _OPENBINARYINTERFACEREQUEST._serialized_start=13559
-  _OPENBINARYINTERFACEREQUEST._serialized_end=13746
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=13748
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=13853
-  _GENERICBINARYREQUEST._serialized_start=13856
-  _GENERICBINARYREQUEST._serialized_end=13986
-  _BINARYMESSAGE._serialized_start=13988
-  _BINARYMESSAGE._serialized_end=14058
-  _BINARYMESSAGECOLLECTION._serialized_start=14060
-  _BINARYMESSAGECOLLECTION._serialized_end=14142
-  _DEVICEEMPTYREQUEST._serialized_start=14144
-  _DEVICEEMPTYREQUEST._serialized_end=14202
-  _BINARYDEVICEIDENTITY._serialized_start=14205
-  _BINARYDEVICEIDENTITY._serialized_end=14550
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=14501
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=14550
-  _BINARYGENERICWITHUNITSREQUEST._serialized_start=14553
-  _BINARYGENERICWITHUNITSREQUEST._serialized_end=14706
-  _BINARYDEVICEHOMEREQUEST._serialized_start=14708
-  _BINARYDEVICEHOMEREQUEST._serialized_end=14802
-  _BINARYDEVICEMOVEREQUEST._serialized_start=14805
-  _BINARYDEVICEMOVEREQUEST._serialized_end=15023
-  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5120
-  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5157
-  _BINARYDEVICESTOPREQUEST._serialized_start=15025
-  _BINARYDEVICESTOPREQUEST._serialized_end=15119
-  _BINARYDEVICEDETECTREQUEST._serialized_start=15121
-  _BINARYDEVICEDETECTREQUEST._serialized_end=15196
-  _BINARYDEVICEDETECTRESPONSE._serialized_start=15198
-  _BINARYDEVICEDETECTRESPONSE._serialized_end=15243
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=15245
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=15345
-  _BINARYDEVICESETSETTINGREQUEST._serialized_start=15347
-  _BINARYDEVICESETSETTINGREQUEST._serialized_end=15462
-  _CUSTOMINTERFACEREADREQUEST._serialized_start=15464
-  _CUSTOMINTERFACEREADREQUEST._serialized_end=15514
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=15516
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=15584
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=15586
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=15637
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=15639
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=15713
-  _CANSETSTATEREQUEST._serialized_start=15715
-  _CANSETSTATEREQUEST._serialized_end=15802
-  _CANSETSTATEAXISRESPONSE._serialized_start=15804
-  _CANSETSTATEAXISRESPONSE._serialized_end=15865
-  _CANSETSTATEDEVICERESPONSE._serialized_start=15867
-  _CANSETSTATEDEVICERESPONSE._serialized_end=15979
-  _SETSTATEREQUEST._serialized_start=15981
-  _SETSTATEREQUEST._serialized_end=16086
-  _SERVOTUNINGREQUEST._serialized_start=16088
-  _SERVOTUNINGREQUEST._serialized_end=16178
-  _SERVOTUNINGPARAM._serialized_start=16180
-  _SERVOTUNINGPARAM._serialized_end=16227
-  _PARAMSETINFO._serialized_start=16229
-  _PARAMSETINFO._serialized_end=16332
-  _SETSERVOTUNINGREQUEST._serialized_start=16335
-  _SETSERVOTUNINGREQUEST._serialized_end=16493
-  _LOADPARAMSET._serialized_start=16495
-  _LOADPARAMSET._serialized_end=16605
-  _SETSERVOTUNINGPIDREQUEST._serialized_start=16608
-  _SETSERVOTUNINGPIDREQUEST._serialized_end=16749
-  _PIDTUNING._serialized_start=16751
-  _PIDTUNING._serialized_end=16838
-  _SETSIMPLETUNING._serialized_start=16841
-  _SETSIMPLETUNING._serialized_end=17035
-  _SIMPLETUNINGPARAMDEFINITION._serialized_start=17037
-  _SIMPLETUNINGPARAMDEFINITION._serialized_end=17137
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=17139
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=17248
-  _TRANSLATORCREATEREQUEST._serialized_start=17251
-  _TRANSLATORCREATEREQUEST._serialized_end=17400
-  _TRANSLATORCREATERESPONSE._serialized_start=17402
-  _TRANSLATORCREATERESPONSE._serialized_end=17451
-  _TRANSLATORAXISDEFINITION._serialized_start=17453
-  _TRANSLATORAXISDEFINITION._serialized_end=17532
-  _TRANSLATORDEFINITION._serialized_start=17535
-  _TRANSLATORDEFINITION._serialized_end=17696
-  _TRANSLATORCONFIG._serialized_start=17699
-  _TRANSLATORCONFIG._serialized_end=17871
-  _TRANSLATORAXISMAPPING._serialized_start=17873
-  _TRANSLATORAXISMAPPING._serialized_end=17937
-  _TRANSLATORAXISTRANSFORMATION._serialized_start=17939
-  _TRANSLATORAXISTRANSFORMATION._serialized_end=18065
-  _TRANSLATORTRANSLATEREQUEST._serialized_start=18067
-  _TRANSLATORTRANSLATEREQUEST._serialized_end=18133
-  _TRANSLATEMESSAGE._serialized_start=18135
-  _TRANSLATEMESSAGE._serialized_end=18208
-  _TRANSLATORTRANSLATERESPONSE._serialized_start=18210
-  _TRANSLATORTRANSLATERESPONSE._serialized_end=18317
-  _GCODESYNTAXEXCEPTIONDATA._serialized_start=18319
-  _GCODESYNTAXEXCEPTIONDATA._serialized_end=18383
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=18385
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=18452
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=18454
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=18530
-  _TRANSLATORFLUSHRESPONSE._serialized_start=18532
-  _TRANSLATORFLUSHRESPONSE._serialized_end=18575
-  _TRANSLATORCREATELIVEREQUEST._serialized_start=18578
-  _TRANSLATORCREATELIVEREQUEST._serialized_end=18722
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=18725
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=18870
-  _TRANSLATOREMPTYREQUEST._serialized_start=18872
-  _TRANSLATOREMPTYREQUEST._serialized_end=18919
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=18921
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=19015
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=19017
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=19120
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=19122
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=19207
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=19209
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=19319
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=19321
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=19403
-  _DEVICESETSTORAGEREQUEST._serialized_start=19405
-  _DEVICESETSTORAGEREQUEST._serialized_end=19526
-  _DEVICEGETSTORAGEREQUEST._serialized_start=19528
-  _DEVICEGETSTORAGEREQUEST._serialized_end=19634
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=19636
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=19747
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=19749
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=19858
-  _DEVICESTORAGEREQUEST._serialized_start=19860
-  _DEVICESTORAGEREQUEST._serialized_end=19947
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=19949
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=20047
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=20050
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=20211
-  _CONVERSIONFACTOR._serialized_start=20213
-  _CONVERSIONFACTOR._serialized_end=20277
-  _OBJECTIVECHANGERREQUEST._serialized_start=20279
-  _OBJECTIVECHANGERREQUEST._serialized_end=20373
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=20375
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=20438
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=20441
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=20619
+  _DOUBLEARRAYRESPONSE._serialized_start=368
+  _DOUBLEARRAYRESPONSE._serialized_end=405
+  _INTRESPONSE._serialized_start=407
+  _INTRESPONSE._serialized_end=435
+  _STRINGRESPONSE._serialized_start=437
+  _STRINGRESPONSE._serialized_end=468
+  _STRINGARRAYRESPONSE._serialized_start=470
+  _STRINGARRAYRESPONSE._serialized_end=507
+  _AXISIDENTITY._serialized_start=510
+  _AXISIDENTITY._serialized_end=731
+  _AXISIDENTITY_AXISTYPE._serialized_start=684
+  _AXISIDENTITY_AXISTYPE._serialized_end=731
+  _DEVICEIDENTITY._serialized_start=734
+  _DEVICEIDENTITY._serialized_end=937
+  _FIRMWAREVERSION._serialized_start=939
+  _FIRMWAREVERSION._serialized_end=1001
+  _DEVICEIOINFO._serialized_start=1004
+  _DEVICEIOINFO._serialized_end=1142
+  _MEASUREMENT._serialized_start=1144
+  _MEASUREMENT._serialized_end=1186
+  _STREAMAXISDEFINITION._serialized_start=1188
+  _STREAMAXISDEFINITION._serialized_end=1250
+  _INVALIDPACKETEXCEPTIONDATA._serialized_start=1252
+  _INVALIDPACKETEXCEPTIONDATA._serialized_end=1312
+  _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_start=1314
+  _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_end=1376
+  _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1378
+  _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1476
+  _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1478
+  _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1552
+  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1554
+  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1647
+  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1649
+  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1718
+  _STREAMEXECUTIONEXCEPTIONDATA._serialized_start=1720
+  _STREAMEXECUTIONEXCEPTIONDATA._serialized_end=1786
+  _INVALIDRESPONSEEXCEPTIONDATA._serialized_start=1788
+  _INVALIDRESPONSEEXCEPTIONDATA._serialized_end=1836
+  _COMMANDFAILEDEXCEPTIONDATA._serialized_start=1838
+  _COMMANDFAILEDEXCEPTIONDATA._serialized_end=1947
+  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_start=1949
+  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_end=2006
+  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_start=2009
+  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_end=2146
+  _SETDEVICESTATEEXCEPTIONDATA._serialized_start=2149
+  _SETDEVICESTATEEXCEPTIONDATA._serialized_end=2381
+  _COMMANDTOOLONGEXCEPTIONDATA._serialized_start=2383
+  _COMMANDTOOLONGEXCEPTIONDATA._serialized_end=2486
+  _TESTREQUEST._serialized_start=2488
+  _TESTREQUEST._serialized_end=2574
+  _TESTRESPONSE._serialized_start=2576
+  _TESTRESPONSE._serialized_end=2609
+  _TESTRESPONSELONG._serialized_start=2611
+  _TESTRESPONSELONG._serialized_end=2648
+  _TESTEVENT._serialized_start=2650
+  _TESTEVENT._serialized_end=2675
+  _TOOLSLISTSERIALPORTSRESPONSE._serialized_start=2677
+  _TOOLSLISTSERIALPORTSRESPONSE._serialized_end=2722
+  _SETINTERNALMODEREQUEST._serialized_start=2724
+  _SETINTERNALMODEREQUEST._serialized_end=2762
+  _SETDEVICEDBSOURCEREQUEST._serialized_start=2764
+  _SETDEVICEDBSOURCEREQUEST._serialized_end=2837
+  _TOGGLEDEVICEDBSTOREREQUEST._serialized_start=2839
+  _TOGGLEDEVICEDBSTOREREQUEST._serialized_end=2910
+  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_start=2912
+  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_end=2955
+  _OPENINTERFACEREQUEST._serialized_start=2958
+  _OPENINTERFACEREQUEST._serialized_end=3253
+  _OPENINTERFACERESPONSE._serialized_start=3255
+  _OPENINTERFACERESPONSE._serialized_end=3300
+  _INTERFACEEMPTYREQUEST._serialized_start=3302
+  _INTERFACEEMPTYREQUEST._serialized_end=3347
+  _SETINTERFACETIMEOUTREQUEST._serialized_start=3349
+  _SETINTERFACETIMEOUTREQUEST._serialized_end=3416
+  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_start=3418
+  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_end=3496
+  _AXISEMPTYREQUEST._serialized_start=3498
+  _AXISEMPTYREQUEST._serialized_end=3568
+  _GENERICCOMMANDREQUEST._serialized_start=3571
+  _GENERICCOMMANDREQUEST._serialized_end=3702
+  _GENERICCOMMANDRESPONSE._serialized_start=3705
+  _GENERICCOMMANDRESPONSE._serialized_end=3905
+  _GENERICCOMMANDRESPONSECOLLECTION._serialized_start=3907
+  _GENERICCOMMANDRESPONSECOLLECTION._serialized_end=4008
+  _UNKNOWNRESPONSEEVENT._serialized_start=4011
+  _UNKNOWNRESPONSEEVENT._serialized_end=4231
+  _ALERTEVENT._serialized_start=4234
+  _ALERTEVENT._serialized_end=4365
+  _DISCONNECTEDEVENT._serialized_start=4367
+  _DISCONNECTEDEVENT._serialized_end=4483
+  _DEVICEIDENTIFYREQUEST._serialized_start=4485
+  _DEVICEIDENTIFYREQUEST._serialized_end=4611
+  _DEVICERENUMBERREQUEST._serialized_start=4613
+  _DEVICERENUMBERREQUEST._serialized_end=4681
+  _DEVICEDETECTREQUEST._serialized_start=4683
+  _DEVICEDETECTREQUEST._serialized_end=4752
+  _DEVICEDETECTRESPONSE._serialized_start=4754
+  _DEVICEDETECTRESPONSE._serialized_end=4793
+  _DEVICEHOMEREQUEST._serialized_start=4795
+  _DEVICEHOMEREQUEST._serialized_end=4891
+  _DEVICEWAITUNTILIDLEREQUEST._serialized_start=4893
+  _DEVICEWAITUNTILIDLEREQUEST._serialized_end=5003
+  _DEVICEMOVEREQUEST._serialized_start=5006
+  _DEVICEMOVEREQUEST._serialized_end=5342
+  _DEVICEMOVEREQUEST_MOVETYPE._serialized_start=5287
+  _DEVICEMOVEREQUEST_MOVETYPE._serialized_end=5342
+  _DEVICESTOPREQUEST._serialized_start=5344
+  _DEVICESTOPREQUEST._serialized_end=5440
+  _DEVICEONALLREQUEST._serialized_start=5442
+  _DEVICEONALLREQUEST._serialized_end=5509
+  _DEVICEONALLRESPONSE._serialized_start=5511
+  _DEVICEONALLRESPONSE._serialized_end=5558
+  _DEVICEGETWARNINGSREQUEST._serialized_start=5560
+  _DEVICEGETWARNINGSREQUEST._serialized_end=5653
+  _DEVICEGETWARNINGSRESPONSE._serialized_start=5655
+  _DEVICEGETWARNINGSRESPONSE._serialized_end=5697
+  _WAITTOCLEARWARNINGSREQUEST._serialized_start=5699
+  _WAITTOCLEARWARNINGSREQUEST._serialized_end=5819
+  _DEVICEGETALLDIGITALIOREQUEST._serialized_start=5821
+  _DEVICEGETALLDIGITALIOREQUEST._serialized_end=5911
+  _DEVICEGETALLDIGITALIORESPONSE._serialized_start=5913
+  _DEVICEGETALLDIGITALIORESPONSE._serialized_end=5960
+  _DEVICEGETALLANALOGIOREQUEST._serialized_start=5962
+  _DEVICEGETALLANALOGIOREQUEST._serialized_end=6051
+  _DEVICEGETALLANALOGIORESPONSE._serialized_start=6053
+  _DEVICEGETALLANALOGIORESPONSE._serialized_end=6099
+  _DEVICEGETDIGITALIOREQUEST._serialized_start=6101
+  _DEVICEGETDIGITALIOREQUEST._serialized_end=6212
+  _DEVICEGETANALOGIOREQUEST._serialized_start=6214
+  _DEVICEGETANALOGIOREQUEST._serialized_end=6324
+  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_start=6326
+  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_end=6415
+  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_start=6417
+  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_end=6505
+  _DEVICESETDIGITALOUTPUTREQUEST._serialized_start=6507
+  _DEVICESETDIGITALOUTPUTREQUEST._serialized_end=6615
+  _DEVICESETANALOGOUTPUTREQUEST._serialized_start=6617
+  _DEVICESETANALOGOUTPUTREQUEST._serialized_end=6724
+  _SETLOGOUTPUTREQUEST._serialized_start=6726
+  _SETLOGOUTPUTREQUEST._serialized_end=6780
+  _DEVICEGETSETTINGREQUEST._serialized_start=6782
+  _DEVICEGETSETTINGREQUEST._serialized_end=6890
+  _DEVICECONVERTSETTINGREQUEST._serialized_start=6893
+  _DEVICECONVERTSETTINGREQUEST._serialized_end=7041
+  _DEVICESETSETTINGREQUEST._serialized_start=7043
+  _DEVICESETSETTINGREQUEST._serialized_end=7166
+  _DEVICESETSETTINGSTRREQUEST._serialized_start=7168
+  _DEVICESETSETTINGSTRREQUEST._serialized_end=7280
+  _PREPARECOMMANDREQUEST._serialized_start=7283
+  _PREPARECOMMANDREQUEST._serialized_end=7441
+  _WAITTORESPONDREQUEST._serialized_start=7443
+  _WAITTORESPONDREQUEST._serialized_end=7520
+  _LOCKSTEPENABLEREQUEST._serialized_start=7522
+  _LOCKSTEPENABLEREQUEST._serialized_end=7624
+  _LOCKSTEPDISABLEREQUEST._serialized_start=7626
+  _LOCKSTEPDISABLEREQUEST._serialized_end=7740
+  _LOCKSTEPSTOPREQUEST._serialized_start=7742
+  _LOCKSTEPSTOPREQUEST._serialized_end=7853
+  _LOCKSTEPHOMEREQUEST._serialized_start=7855
+  _LOCKSTEPHOMEREQUEST._serialized_end=7966
+  _LOCKSTEPMOVEREQUEST._serialized_start=7969
+  _LOCKSTEPMOVEREQUEST._serialized_end=8322
+  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_start=5287
+  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_end=5342
+  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_start=8324
+  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_end=8449
+  _LOCKSTEPEMPTYREQUEST._serialized_start=8451
+  _LOCKSTEPEMPTYREQUEST._serialized_end=8538
+  _LOCKSTEPAXES._serialized_start=8540
+  _LOCKSTEPAXES._serialized_end=8618
+  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_start=8620
+  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_end=8666
+  _LOCKSTEPGETREQUEST._serialized_start=8668
+  _LOCKSTEPGETREQUEST._serialized_end=8767
+  _LOCKSTEPSETREQUEST._serialized_start=8770
+  _LOCKSTEPSETREQUEST._serialized_end=8904
+  _OSCILLOSCOPEADDCHANNELREQUEST._serialized_start=8906
+  _OSCILLOSCOPEADDCHANNELREQUEST._serialized_end=9006
+  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_start=9008
+  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_end=9115
+  _OSCILLOSCOPEREADRESPONSE._serialized_start=9117
+  _OSCILLOSCOPEREADRESPONSE._serialized_end=9161
+  _OSCILLOSCOPEDATAIDENTIFIER._serialized_start=9163
+  _OSCILLOSCOPEDATAIDENTIFIER._serialized_end=9208
+  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_start=9210
+  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_end=9279
+  _OSCILLOSCOPEDATAGETREQUEST._serialized_start=9281
+  _OSCILLOSCOPEDATAGETREQUEST._serialized_end=9340
+  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_start=9342
+  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_end=9426
+  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_start=9428
+  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_end=9478
+  _STREAMSETUPLIVEREQUEST._serialized_start=9480
+  _STREAMSETUPLIVEREQUEST._serialized_end=9575
+  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_start=9578
+  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_end=9728
+  _STREAMSETUPSTOREREQUEST._serialized_start=9730
+  _STREAMSETUPSTOREREQUEST._serialized_end=9849
+  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_start=9852
+  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_end=10026
+  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_start=10029
+  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_end=10167
+  _STREAMCALLREQUEST._serialized_start=10169
+  _STREAMCALLREQUEST._serialized_end=10268
+  _STREAMLINEREQUEST._serialized_start=10271
+  _STREAMLINEREQUEST._serialized_end=10519
+  _STREAMLINEREQUEST_TYPE._serialized_start=10495
+  _STREAMLINEREQUEST_TYPE._serialized_end=10519
+  _STREAMARCREQUEST._serialized_start=10522
+  _STREAMARCREQUEST._serialized_end=10955
+  _STREAMARCREQUEST_TYPE._serialized_start=10495
+  _STREAMARCREQUEST_TYPE._serialized_end=10519
+  _STREAMCIRCLEREQUEST._serialized_start=10958
+  _STREAMCIRCLEREQUEST._serialized_end=11293
+  _STREAMCIRCLEREQUEST_TYPE._serialized_start=10495
+  _STREAMCIRCLEREQUEST_TYPE._serialized_end=10519
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=11295
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=11422
+  _STREAMWAITANALOGINPUTREQUEST._serialized_start=11425
+  _STREAMWAITANALOGINPUTREQUEST._serialized_end=11570
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=11572
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=11699
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=11701
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=11827
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=11829
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=11944
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=11946
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=12054
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=12056
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=12163
+  _STREAMWAITREQUEST._serialized_start=12165
+  _STREAMWAITREQUEST._serialized_end=12269
+  _STREAMWAITUNTILIDLEREQUEST._serialized_start=12271
+  _STREAMWAITUNTILIDLEREQUEST._serialized_end=12386
+  _STREAMEMPTYREQUEST._serialized_start=12388
+  _STREAMEMPTYREQUEST._serialized_end=12465
+  _STREAMGETAXESRESPONSE._serialized_start=12467
+  _STREAMGETAXESRESPONSE._serialized_end=12550
+  _STREAMGETMAXSPEEDREQUEST._serialized_start=12552
+  _STREAMGETMAXSPEEDREQUEST._serialized_end=12649
+  _STREAMSETMAXSPEEDREQUEST._serialized_start=12651
+  _STREAMSETMAXSPEEDREQUEST._serialized_end=12767
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=12769
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=12883
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=12886
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=13037
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=13039
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=13154
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=13157
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=13310
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=13312
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=13400
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=13402
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=13456
+  _STREAMBUFFERERASEREQUEST._serialized_start=13458
+  _STREAMBUFFERERASEREQUEST._serialized_end=13541
+  _STREAMGENERICCOMMANDREQUEST._serialized_start=13543
+  _STREAMGENERICCOMMANDREQUEST._serialized_end=13646
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=13648
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=13754
+  _BINARYREPLYONLYEVENT._serialized_start=13756
+  _BINARYREPLYONLYEVENT._serialized_end=13855
+  _OPENBINARYINTERFACEREQUEST._serialized_start=13858
+  _OPENBINARYINTERFACEREQUEST._serialized_end=14045
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=14047
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=14152
+  _GENERICBINARYREQUEST._serialized_start=14155
+  _GENERICBINARYREQUEST._serialized_end=14285
+  _BINARYMESSAGE._serialized_start=14287
+  _BINARYMESSAGE._serialized_end=14357
+  _BINARYMESSAGECOLLECTION._serialized_start=14359
+  _BINARYMESSAGECOLLECTION._serialized_end=14441
+  _DEVICEEMPTYREQUEST._serialized_start=14443
+  _DEVICEEMPTYREQUEST._serialized_end=14501
+  _BINARYDEVICEIDENTITY._serialized_start=14504
+  _BINARYDEVICEIDENTITY._serialized_end=14849
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=14800
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=14849
+  _BINARYGENERICWITHUNITSREQUEST._serialized_start=14852
+  _BINARYGENERICWITHUNITSREQUEST._serialized_end=15005
+  _BINARYDEVICEHOMEREQUEST._serialized_start=15007
+  _BINARYDEVICEHOMEREQUEST._serialized_end=15101
+  _BINARYDEVICEMOVEREQUEST._serialized_start=15104
+  _BINARYDEVICEMOVEREQUEST._serialized_end=15322
+  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5287
+  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5324
+  _BINARYDEVICESTOPREQUEST._serialized_start=15324
+  _BINARYDEVICESTOPREQUEST._serialized_end=15418
+  _BINARYDEVICEDETECTREQUEST._serialized_start=15420
+  _BINARYDEVICEDETECTREQUEST._serialized_end=15495
+  _BINARYDEVICEDETECTRESPONSE._serialized_start=15497
+  _BINARYDEVICEDETECTRESPONSE._serialized_end=15542
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=15544
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=15644
+  _BINARYDEVICESETSETTINGREQUEST._serialized_start=15646
+  _BINARYDEVICESETSETTINGREQUEST._serialized_end=15761
+  _CUSTOMINTERFACEREADREQUEST._serialized_start=15763
+  _CUSTOMINTERFACEREADREQUEST._serialized_end=15813
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=15815
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=15883
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=15885
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=15936
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=15938
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=16012
+  _CANSETSTATEREQUEST._serialized_start=16014
+  _CANSETSTATEREQUEST._serialized_end=16101
+  _CANSETSTATEAXISRESPONSE._serialized_start=16103
+  _CANSETSTATEAXISRESPONSE._serialized_end=16164
+  _CANSETSTATEDEVICERESPONSE._serialized_start=16166
+  _CANSETSTATEDEVICERESPONSE._serialized_end=16278
+  _SETSTATEREQUEST._serialized_start=16280
+  _SETSTATEREQUEST._serialized_end=16385
+  _SERVOTUNINGREQUEST._serialized_start=16387
+  _SERVOTUNINGREQUEST._serialized_end=16477
+  _SERVOTUNINGPARAM._serialized_start=16479
+  _SERVOTUNINGPARAM._serialized_end=16526
+  _PARAMSETINFO._serialized_start=16528
+  _PARAMSETINFO._serialized_end=16631
+  _SETSERVOTUNINGREQUEST._serialized_start=16634
+  _SETSERVOTUNINGREQUEST._serialized_end=16792
+  _LOADPARAMSET._serialized_start=16794
+  _LOADPARAMSET._serialized_end=16904
+  _SETSERVOTUNINGPIDREQUEST._serialized_start=16907
+  _SETSERVOTUNINGPIDREQUEST._serialized_end=17048
+  _PIDTUNING._serialized_start=17050
+  _PIDTUNING._serialized_end=17137
+  _SETSIMPLETUNING._serialized_start=17140
+  _SETSIMPLETUNING._serialized_end=17334
+  _SIMPLETUNINGPARAMDEFINITION._serialized_start=17336
+  _SIMPLETUNINGPARAMDEFINITION._serialized_end=17436
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=17438
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=17547
+  _TRANSLATORCREATEREQUEST._serialized_start=17550
+  _TRANSLATORCREATEREQUEST._serialized_end=17699
+  _TRANSLATORCREATERESPONSE._serialized_start=17701
+  _TRANSLATORCREATERESPONSE._serialized_end=17750
+  _TRANSLATORAXISDEFINITION._serialized_start=17752
+  _TRANSLATORAXISDEFINITION._serialized_end=17831
+  _TRANSLATORDEFINITION._serialized_start=17834
+  _TRANSLATORDEFINITION._serialized_end=17995
+  _TRANSLATORCONFIG._serialized_start=17998
+  _TRANSLATORCONFIG._serialized_end=18170
+  _TRANSLATORAXISMAPPING._serialized_start=18172
+  _TRANSLATORAXISMAPPING._serialized_end=18236
+  _TRANSLATORAXISTRANSFORMATION._serialized_start=18238
+  _TRANSLATORAXISTRANSFORMATION._serialized_end=18364
+  _TRANSLATORTRANSLATEREQUEST._serialized_start=18366
+  _TRANSLATORTRANSLATEREQUEST._serialized_end=18432
+  _TRANSLATEMESSAGE._serialized_start=18434
+  _TRANSLATEMESSAGE._serialized_end=18507
+  _TRANSLATORTRANSLATERESPONSE._serialized_start=18509
+  _TRANSLATORTRANSLATERESPONSE._serialized_end=18616
+  _GCODESYNTAXEXCEPTIONDATA._serialized_start=18618
+  _GCODESYNTAXEXCEPTIONDATA._serialized_end=18682
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=18684
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=18751
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=18753
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=18829
+  _TRANSLATORFLUSHRESPONSE._serialized_start=18831
+  _TRANSLATORFLUSHRESPONSE._serialized_end=18874
+  _TRANSLATORCREATELIVEREQUEST._serialized_start=18877
+  _TRANSLATORCREATELIVEREQUEST._serialized_end=19021
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=19024
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=19169
+  _TRANSLATOREMPTYREQUEST._serialized_start=19171
+  _TRANSLATOREMPTYREQUEST._serialized_end=19218
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=19220
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=19314
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=19316
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=19419
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=19421
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=19506
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=19508
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=19618
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=19620
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=19702
+  _DEVICESETSTORAGEREQUEST._serialized_start=19704
+  _DEVICESETSTORAGEREQUEST._serialized_end=19825
+  _DEVICEGETSTORAGEREQUEST._serialized_start=19827
+  _DEVICEGETSTORAGEREQUEST._serialized_end=19933
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=19935
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=20046
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=20048
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=20157
+  _DEVICESTORAGEREQUEST._serialized_start=20159
+  _DEVICESTORAGEREQUEST._serialized_end=20246
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=20248
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=20346
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=20349
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=20510
+  _CONVERSIONFACTOR._serialized_start=20512
+  _CONVERSIONFACTOR._serialized_end=20576
+  _OBJECTIVECHANGERREQUEST._serialized_start=20578
+  _OBJECTIVECHANGERREQUEST._serialized_end=20672
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=20674
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=20737
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=20740
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=20918
 # @@protoc_insertion_point(module_scope)
```

### Comparing `zaber_motion-3.2.1/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-3.3.0/zaber_motion/protobufs/main_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     SET_DEVICE_STATE_FAILED: _Errors.ValueType  # 40
     G_CODE_SYNTAX: _Errors.ValueType  # 41
     G_CODE_EXECUTION: _Errors.ValueType  # 42
     INVALID_OPERATION: _Errors.ValueType  # 43
     COMMAND_TOO_LONG: _Errors.ValueType  # 44
     NO_VALUE_FOR_KEY: _Errors.ValueType  # 45
     DEVICE_DETECTION_FAILED: _Errors.ValueType  # 46
+    TIMEOUT: _Errors.ValueType  # 47
 
 class Errors(_Errors, metaclass=_ErrorsEnumTypeWrapper): ...
 
 REQUEST_TIMEOUT: Errors.ValueType  # 0
 CONNECTION_CLOSED: Errors.ValueType  # 1
 INVALID_ARGUMENT: Errors.ValueType  # 2
 OUT_OF_REQUEST_IDS: Errors.ValueType  # 3
@@ -131,14 +132,15 @@
 SET_DEVICE_STATE_FAILED: Errors.ValueType  # 40
 G_CODE_SYNTAX: Errors.ValueType  # 41
 G_CODE_EXECUTION: Errors.ValueType  # 42
 INVALID_OPERATION: Errors.ValueType  # 43
 COMMAND_TOO_LONG: Errors.ValueType  # 44
 NO_VALUE_FOR_KEY: Errors.ValueType  # 45
 DEVICE_DETECTION_FAILED: Errors.ValueType  # 46
+TIMEOUT: Errors.ValueType  # 47
 global___Errors = Errors
 
 class _InterfaceType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _InterfaceTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_InterfaceType.ValueType], builtins.type):
@@ -261,14 +263,30 @@
         value: builtins.float = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
 
 global___DoubleResponse = DoubleResponse
 
 @typing_extensions.final
+class DoubleArrayResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    VALUES_FIELD_NUMBER: builtins.int
+    @property
+    def values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
+        *,
+        values: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["values", b"values"]) -> None: ...
+
+global___DoubleArrayResponse = DoubleArrayResponse
+
+@typing_extensions.final
 class IntResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUE_FIELD_NUMBER: builtins.int
     value: builtins.int
     def __init__(
         self,
@@ -1249,23 +1267,48 @@
         error_message: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["error_message", b"error_message", "error_type", b"error_type", "interface_id", b"interface_id"]) -> None: ...
 
 global___DisconnectedEvent = DisconnectedEvent
 
 @typing_extensions.final
-class DeviceRenumberRequest(google.protobuf.message.Message):
+class DeviceIdentifyRequest(google.protobuf.message.Message):
     """---- /device ----
 
-    device/renumber
+    device/identify
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
+    DEVICE_FIELD_NUMBER: builtins.int
+    ASSUME_VERSION_FIELD_NUMBER: builtins.int
+    interface_id: builtins.int
+    device: builtins.int
+    @property
+    def assume_version(self) -> global___FirmwareVersion: ...
+    def __init__(
+        self,
+        *,
+        interface_id: builtins.int = ...,
+        device: builtins.int = ...,
+        assume_version: global___FirmwareVersion | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["assume_version", b"assume_version"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["assume_version", b"assume_version", "device", b"device", "interface_id", b"interface_id"]) -> None: ...
+
+global___DeviceIdentifyRequest = DeviceIdentifyRequest
+
+@typing_extensions.final
+class DeviceRenumberRequest(google.protobuf.message.Message):
+    """device/renumber"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INTERFACE_ID_FIELD_NUMBER: builtins.int
     FIRST_ADDRESS_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     first_address: builtins.int
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
@@ -1532,14 +1575,44 @@
         flags: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["flags", b"flags"]) -> None: ...
 
 global___DeviceGetWarningsResponse = DeviceGetWarningsResponse
 
 @typing_extensions.final
+class WaitToClearWarningsRequest(google.protobuf.message.Message):
+    """device/wait_to_clear_warnings"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INTERFACE_ID_FIELD_NUMBER: builtins.int
+    DEVICE_FIELD_NUMBER: builtins.int
+    AXIS_FIELD_NUMBER: builtins.int
+    TIMEOUT_FIELD_NUMBER: builtins.int
+    WARNING_FLAGS_FIELD_NUMBER: builtins.int
+    interface_id: builtins.int
+    device: builtins.int
+    axis: builtins.int
+    timeout: builtins.float
+    @property
+    def warning_flags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    def __init__(
+        self,
+        *,
+        interface_id: builtins.int = ...,
+        device: builtins.int = ...,
+        axis: builtins.int = ...,
+        timeout: builtins.float = ...,
+        warning_flags: collections.abc.Iterable[builtins.str] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axis", b"axis", "device", b"device", "interface_id", b"interface_id", "timeout", b"timeout", "warning_flags", b"warning_flags"]) -> None: ...
+
+global___WaitToClearWarningsRequest = WaitToClearWarningsRequest
+
+@typing_extensions.final
 class DeviceGetAllDigitalIORequest(google.protobuf.message.Message):
     """device/get_all_digital_io"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
@@ -1939,14 +2012,37 @@
         parameters: collections.abc.Iterable[global___Measurement] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["axis", b"axis", "command_template", b"command_template", "device", b"device", "interface_id", b"interface_id", "parameters", b"parameters"]) -> None: ...
 
 global___PrepareCommandRequest = PrepareCommandRequest
 
 @typing_extensions.final
+class WaitToRespondRequest(google.protobuf.message.Message):
+    """device/wait_to_respond"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INTERFACE_ID_FIELD_NUMBER: builtins.int
+    DEVICE_FIELD_NUMBER: builtins.int
+    TIMEOUT_FIELD_NUMBER: builtins.int
+    interface_id: builtins.int
+    device: builtins.int
+    timeout: builtins.float
+    def __init__(
+        self,
+        *,
+        interface_id: builtins.int = ...,
+        device: builtins.int = ...,
+        timeout: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "timeout", b"timeout"]) -> None: ...
+
+global___WaitToRespondRequest = WaitToRespondRequest
+
+@typing_extensions.final
 class LockstepEnableRequest(google.protobuf.message.Message):
     """---- /device lockstep ----
 
     device/lockstep_enable
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -2202,16 +2298,19 @@
         axes: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes"]) -> None: ...
 
 global___LockstepGetAxisNumbersResponse = LockstepGetAxisNumbersResponse
 
 @typing_extensions.final
-class LockstepGetTwistsRequest(google.protobuf.message.Message):
-    """device/lockstep_get_twists"""
+class LockstepGetRequest(google.protobuf.message.Message):
+    """device/lockstep_get_twists
+    device/lockstep_get_offsets
+    device/lockstep_get_pos
+    """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     LOCKSTEP_GROUP_ID_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
@@ -2225,73 +2324,47 @@
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         lockstep_group_id: builtins.int = ...,
         unit: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "lockstep_group_id", b"lockstep_group_id", "unit", b"unit"]) -> None: ...
 
-global___LockstepGetTwistsRequest = LockstepGetTwistsRequest
+global___LockstepGetRequest = LockstepGetRequest
 
 @typing_extensions.final
-class LockstepGetTwistsResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    TWISTS_FIELD_NUMBER: builtins.int
-    @property
-    def twists(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
-    def __init__(
-        self,
-        *,
-        twists: collections.abc.Iterable[builtins.float] | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["twists", b"twists"]) -> None: ...
-
-global___LockstepGetTwistsResponse = LockstepGetTwistsResponse
-
-@typing_extensions.final
-class LockstepGetOffsetsRequest(google.protobuf.message.Message):
-    """device/lockstep_get_offsets"""
+class LockstepSetRequest(google.protobuf.message.Message):
+    """device/lockstep_set_tolerance"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     LOCKSTEP_GROUP_ID_FIELD_NUMBER: builtins.int
+    VALUE_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
+    AXIS_INDEX_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     lockstep_group_id: builtins.int
+    value: builtins.float
     unit: builtins.str
+    axis_index: builtins.int
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         lockstep_group_id: builtins.int = ...,
+        value: builtins.float = ...,
         unit: builtins.str = ...,
+        axis_index: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "lockstep_group_id", b"lockstep_group_id", "unit", b"unit"]) -> None: ...
-
-global___LockstepGetOffsetsRequest = LockstepGetOffsetsRequest
-
-@typing_extensions.final
-class LockstepGetOffsetsResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    OFFSETS_FIELD_NUMBER: builtins.int
-    @property
-    def offsets(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
-    def __init__(
-        self,
-        *,
-        offsets: collections.abc.Iterable[builtins.float] | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["offsets", b"offsets"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axis_index", b"axis_index", "device", b"device", "interface_id", b"interface_id", "lockstep_group_id", b"lockstep_group_id", "unit", b"unit", "value", b"value"]) -> None: ...
 
-global___LockstepGetOffsetsResponse = LockstepGetOffsetsResponse
+global___LockstepSetRequest = LockstepSetRequest
 
 @typing_extensions.final
 class OscilloscopeAddChannelRequest(google.protobuf.message.Message):
     """---- /device oscilloscope ----
 
     oscilloscope/add_channel
     """
```

### Comparing `zaber_motion-3.2.1/zaber_motion/serialization.py` & `zaber_motion-3.3.0/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/tools.py` & `zaber_motion-3.3.0/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion/units.py` & `zaber_motion-3.3.0/zaber_motion/units.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.2.1/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-3.3.0/zaber_motion.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber-motion
-Version: 3.2.1
+Version: 3.3.0
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,8 +15,8 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Zaber Motion Library
 
 Zaber Motion Library is a multi-platform library used to operate Zaber devices.
 
-Official documentation: [https://www.zaber.com/software/docs/motion-library/](https://www.zaber.com/software/docs/motion-library/)
+Official documentation: [https://software.zaber.com/motion-library/](https://software.zaber.com/motion-library/)
```

### Comparing `zaber_motion-3.2.1/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-3.3.0/zaber_motion.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 zaber_motion/exceptions/stream_execution_exception_data.py
 zaber_motion/exceptions/stream_mode_exception.py
 zaber_motion/exceptions/stream_movement_failed_exception.py
 zaber_motion/exceptions/stream_movement_failed_exception_data.py
 zaber_motion/exceptions/stream_movement_interrupted_exception.py
 zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
 zaber_motion/exceptions/stream_setup_failed_exception.py
+zaber_motion/exceptions/timeout_exception.py
 zaber_motion/exceptions/transport_already_used_exception.py
 zaber_motion/exceptions/unknown_request_exception.py
 zaber_motion/gcode/__init__.py
 zaber_motion/gcode/axis_definition.py
 zaber_motion/gcode/axis_mapping.py
 zaber_motion/gcode/axis_transformation.py
 zaber_motion/gcode/device_definition.py
```

