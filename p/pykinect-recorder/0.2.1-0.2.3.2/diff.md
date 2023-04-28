# Comparing `tmp/pykinect_recorder-0.2.1-py3-none-any.whl.zip` & `tmp/pykinect_recorder-0.2.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,55 @@
-Zip file size: 2345 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       32 b- defN 23-Mar-20 05:17 src/__init__.py
--rw-rw-rw-  2.0 fat      464 b- defN 23-Mar-21 07:03 src/main.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:13 pykinect_recorder-0.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      643 b- defN 23-Mar-21 07:13 pykinect_recorder-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-21 07:13 pykinect_recorder-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       52 b- defN 23-Mar-21 07:13 pykinect_recorder-0.2.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-21 07:13 pykinect_recorder-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      673 b- defN 23-Mar-21 07:13 pykinect_recorder-0.2.1.dist-info/RECORD
-8 files, 1960 bytes uncompressed, 1145 bytes compressed:  41.6%
+Zip file size: 57348 bytes, number of entries: 53
+-rw-rw-rw-  2.0 fat       44 b- defN 23-Mar-20 05:17 pykinect_recorder/__init__.py
+-rw-rw-rw-  2.0 fat       87 b- defN 23-Mar-20 05:16 pykinect_recorder/main/__init__.py
+-rw-rw-rw-  2.0 fat     1814 b- defN 23-Mar-19 12:27 pykinect_recorder/main/logger.py
+-rw-rw-rw-  2.0 fat     9085 b- defN 23-Mar-10 02:33 pykinect_recorder/main/old_record_video.py
+-rw-rw-rw-  2.0 fat     6109 b- defN 23-Mar-17 04:50 pykinect_recorder/main/record_audio.py
+-rw-rw-rw-  2.0 fat     2985 b- defN 23-Mar-10 02:33 pykinect_recorder/main/record_video.py
+-rw-rw-rw-  2.0 fat     2539 b- defN 23-Mar-20 05:11 pykinect_recorder/main/synology_utils.py
+-rw-rw-rw-  2.0 fat       65 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/__init__.py
+-rw-rw-rw-  2.0 fat     2067 b- defN 23-Mar-21 01:56 pykinect_recorder/main/_pyk4a/pykinect.py
+-rw-rw-rw-  2.0 fat      264 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4a/__init__.py
+-rw-rw-rw-  2.0 fat    37544 b- defN 23-Mar-20 06:28 pykinect_recorder/main/_pyk4a/k4a/_k4a.py
+-rw-rw-rw-  2.0 fat    10943 b- defN 23-Mar-20 07:10 pykinect_recorder/main/_pyk4a/k4a/_k4atypes.py
+-rw-rw-rw-  2.0 fat     5639 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4a/calibration.py
+-rw-rw-rw-  2.0 fat     4160 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4a/capture.py
+-rw-rw-rw-  2.0 fat     4114 b- defN 23-Mar-20 11:45 pykinect_recorder/main/_pyk4a/k4a/configuration.py
+-rw-rw-rw-  2.0 fat     6063 b- defN 23-Mar-21 01:56 pykinect_recorder/main/_pyk4a/k4a/device.py
+-rw-rw-rw-  2.0 fat     5074 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4a/image.py
+-rw-rw-rw-  2.0 fat     1573 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4a/imu_sample.py
+-rw-rw-rw-  2.0 fat     4402 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4a/transformation.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/__init__.py
+-rw-rw-rw-  2.0 fat     8794 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/_k4abt.py
+-rw-rw-rw-  2.0 fat     8268 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/_k4abtTypes.py
+-rw-rw-rw-  2.0 fat     1146 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/body.py
+-rw-rw-rw-  2.0 fat     3012 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/body2d.py
+-rw-rw-rw-  2.0 fat     4620 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/frame.py
+-rw-rw-rw-  2.0 fat     1617 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/joint.py
+-rw-rw-rw-  2.0 fat     1228 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/joint2d.py
+-rw-rw-rw-  2.0 fat     3223 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4abt/tracker.py
+-rw-rw-rw-  2.0 fat      149 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/k4arecord/__init__.py
+-rw-rw-rw-  2.0 fat    20479 b- defN 23-Mar-10 05:47 pykinect_recorder/main/_pyk4a/k4arecord/_k4arecord.py
+-rw-rw-rw-  2.0 fat     2339 b- defN 23-Mar-10 04:43 pykinect_recorder/main/_pyk4a/k4arecord/_k4arecordTypes.py
+-rw-rw-rw-  2.0 fat      952 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4arecord/datablock.py
+-rw-rw-rw-  2.0 fat     5495 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4arecord/playback.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 23-Mar-21 01:56 pykinect_recorder/main/_pyk4a/k4arecord/record.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 23-Mar-19 07:37 pykinect_recorder/main/_pyk4a/k4arecord/record_configuration.py
+-rw-rw-rw-  2.0 fat       96 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1175 b- defN 23-Mar-10 02:33 pykinect_recorder/main/_pyk4a/utils/plot3dUtils.py
+-rw-rw-rw-  2.0 fat      917 b- defN 23-Mar-10 05:48 pykinect_recorder/main/_pyk4a/utils/postProcessing.py
+-rw-rw-rw-  2.0 fat     2472 b- defN 23-Mar-10 05:50 pykinect_recorder/main/_pyk4a/utils/utils.py
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Mar-20 05:17 pykinect_recorder/renderer/__init__.py
+-rw-rw-rw-  2.0 fat     1993 b- defN 23-Mar-21 04:39 pykinect_recorder/renderer/main_window.py
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Mar-20 05:33 pykinect_recorder/renderer/components/__init__.py
+-rw-rw-rw-  2.0 fat     2714 b- defN 23-Mar-19 12:09 pykinect_recorder/renderer/components/custom_buttons.py
+-rw-rw-rw-  2.0 fat     2919 b- defN 23-Mar-20 09:31 pykinect_recorder/renderer/components/file_viewer.py
+-rw-rw-rw-  2.0 fat     2953 b- defN 23-Mar-21 07:57 pykinect_recorder/renderer/components/pyk4a_thread.py
+-rw-rw-rw-  2.0 fat     9054 b- defN 23-Mar-21 07:57 pykinect_recorder/renderer/components/sensor_viewer.py
+-rw-rw-rw-  2.0 fat    15337 b- defN 23-Mar-20 12:05 pykinect_recorder/renderer/components/sidebar.py
+-rw-rw-rw-  2.0 fat     3723 b- defN 23-Mar-21 05:29 pykinect_recorder/renderer/components/toolbar.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:58 pykinect_recorder-0.2.3.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      637 b- defN 23-Mar-21 07:58 pykinect_recorder-0.2.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-21 07:58 pykinect_recorder-0.2.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Mar-21 07:58 pykinect_recorder-0.2.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     5376 b- defN 23-Mar-21 07:58 pykinect_recorder-0.2.3.2.dist-info/RECORD
+53 files, 219591 bytes uncompressed, 48438 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -1,25 +1,160 @@
-Filename: src/__init__.py
+Filename: pykinect_recorder/__init__.py
 Comment: 
 
-Filename: src/main.py
+Filename: pykinect_recorder/main/__init__.py
 Comment: 
 
-Filename: pykinect_recorder-0.2.1.dist-info/LICENSE
+Filename: pykinect_recorder/main/logger.py
 Comment: 
 
-Filename: pykinect_recorder-0.2.1.dist-info/METADATA
+Filename: pykinect_recorder/main/old_record_video.py
 Comment: 
 
-Filename: pykinect_recorder-0.2.1.dist-info/WHEEL
+Filename: pykinect_recorder/main/record_audio.py
 Comment: 
 
-Filename: pykinect_recorder-0.2.1.dist-info/entry_points.txt
+Filename: pykinect_recorder/main/record_video.py
 Comment: 
 
-Filename: pykinect_recorder-0.2.1.dist-info/top_level.txt
+Filename: pykinect_recorder/main/synology_utils.py
 Comment: 
 
-Filename: pykinect_recorder-0.2.1.dist-info/RECORD
+Filename: pykinect_recorder/main/_pyk4a/__init__.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/pykinect.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/__init__.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/_k4a.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/_k4atypes.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/calibration.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/capture.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/configuration.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/device.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/image.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/imu_sample.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4a/transformation.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/__init__.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/_k4abt.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/_k4abtTypes.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/body.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/body2d.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/frame.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/joint.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/joint2d.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4abt/tracker.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4arecord/__init__.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4arecord/_k4arecord.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4arecord/_k4arecordTypes.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4arecord/datablock.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4arecord/playback.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4arecord/record.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/k4arecord/record_configuration.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/utils/__init__.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/utils/plot3dUtils.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/utils/postProcessing.py
+Comment: 
+
+Filename: pykinect_recorder/main/_pyk4a/utils/utils.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/__init__.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/main_window.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/components/__init__.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/components/custom_buttons.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/components/file_viewer.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/components/pyk4a_thread.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/components/sensor_viewer.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/components/sidebar.py
+Comment: 
+
+Filename: pykinect_recorder/renderer/components/toolbar.py
+Comment: 
+
+Filename: pykinect_recorder-0.2.3.2.dist-info/LICENSE
+Comment: 
+
+Filename: pykinect_recorder-0.2.3.2.dist-info/METADATA
+Comment: 
+
+Filename: pykinect_recorder-0.2.3.2.dist-info/WHEEL
+Comment: 
+
+Filename: pykinect_recorder-0.2.3.2.dist-info/top_level.txt
+Comment: 
+
+Filename: pykinect_recorder-0.2.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pykinect_recorder-0.2.1.dist-info/METADATA` & `pykinect_recorder-0.2.3.2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pykinect-recorder
-Version: 0.2.1
+Version: 0.2.3.2
 Summary: PyKinect Recorder: Azure Kinect Sensor with Audio, Vision Solutions
 Home-page: https://github.com/unerue/pykinect-recorder
 Author: Kyung-Su Kang
 Author-email: unerue@me.com
 License: MIT
 Keywords: azure,kinect,deep-learning,computer-vision
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: <3.12,>=3.8.1
+Requires-Python: >=3.8
 License-File: LICENSE
 
 UNKNOWN
```

