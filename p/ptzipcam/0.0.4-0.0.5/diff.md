# Comparing `tmp/ptzipcam-0.0.4.tar.gz` & `tmp/ptzipcam-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ptzipcam-0.0.4.tar", last modified: Thu Mar  9 19:53:45 2023, max compression
+gzip compressed data, was "dist/ptzipcam-0.0.5.tar", last modified: Thu Apr 27 22:51:09 2023, max compression
```

## Comparing `ptzipcam-0.0.4.tar` & `ptzipcam-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/
--rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/setup.cfg
--rw-rw-r--   0 ian       (1000) ian       (1000)     3527 2023-03-07 19:13:46.000000 ptzipcam-0.0.4/README.md
--rw-rw-r--   0 ian       (1000) ian       (1000)     4851 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/PKG-INFO
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/ptzipcam.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)     4851 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/ptzipcam.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/ptzipcam.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)      360 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/ptzipcam.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/ptzipcam.egg-info/top_level.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)       55 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/ptzipcam.egg-info/requires.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)     1425 2023-03-07 19:13:46.000000 ptzipcam-0.0.4/setup.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-03-09 19:53:45.000000 ptzipcam-0.0.4/ptzipcam/
--rw-rw-r--   0 ian       (1000) ian       (1000)    17536 2023-03-07 19:14:06.000000 ptzipcam-0.0.4/ptzipcam/ptz_camera.py
--rw-rw-r--   0 ian       (1000) ian       (1000)       22 2023-03-09 19:53:05.000000 ptzipcam-0.0.4/ptzipcam/__init__.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2125 2023-03-07 19:13:46.000000 ptzipcam-0.0.4/ptzipcam/camera.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     4382 2023-03-07 19:14:06.000000 ptzipcam-0.0.4/ptzipcam/io.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1404 2023-03-07 19:14:06.000000 ptzipcam-0.0.4/ptzipcam/video_writer.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1563 2023-03-07 19:14:06.000000 ptzipcam-0.0.4/ptzipcam/convert.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2019 2023-03-07 19:13:46.000000 ptzipcam-0.0.4/ptzipcam/logs.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     4759 2022-07-12 19:23:50.000000 ptzipcam-0.0.4/ptzipcam/tracker.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3061 2023-03-07 19:14:06.000000 ptzipcam-0.0.4/ptzipcam/ui.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1073 2023-03-07 19:13:46.000000 ptzipcam-0.0.4/LICENSE
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/
+-rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/setup.cfg
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3527 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/README.md
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3974 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/PKG-INFO
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)     3974 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/dependency_links.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)      360 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/top_level.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       55 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/requires.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1425 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/setup.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam/
+-rw-rw-r--   0 ian       (1000) ian       (1000)    17536 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/ptz_camera.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)       89 2023-04-27 22:48:11.000000 ptzipcam-0.0.5/ptzipcam/__init__.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2125 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/camera.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     4111 2023-04-27 22:48:11.000000 ptzipcam-0.0.5/ptzipcam/io.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1404 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/video_writer.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1563 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/convert.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2019 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/logs.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     4759 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/tracker.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3061 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/ui.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1073 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/LICENSE
```

### Comparing `ptzipcam-0.0.4/README.md` & `ptzipcam-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/setup.py` & `ptzipcam-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/ptzipcam/ptz_camera.py` & `ptzipcam-0.0.5/ptzipcam/ptz_camera.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/ptzipcam/camera.py` & `ptzipcam-0.0.5/ptzipcam/camera.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/ptzipcam/io.py` & `ptzipcam-0.0.5/ptzipcam/io.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 At this stage, this amounts to a single class for recording stills.
 
 
 """
 import logging
 import os
-import time
-import math
 
 from datetime import datetime
 import cv2
 
 log = logging.getLogger(__name__)
 
 
@@ -23,16 +21,16 @@
     tied to that images capture.
 
     """
 
     def __init__(self, path):
         log.debug('Initialize recorder.')
         self.path = path
-        self.timestamp_format = "%Y-%m-%dT%H-%M-%S"
-        timestamp_string = time.strftime(self.timestamp_format)
+        self.timestamp_format = "%Y-%m-%dT%H-%M-%S_%f"
+        timestamp_string = datetime.now().strftime(self.timestamp_format[:-3])
         image_folder_name = timestamp_string + '_images'
         self.image_path = os.path.join(self.path, image_folder_name)
         if not os.path.exists(self.image_path):
             os.mkdir(self.image_path)
         else:
             warning = ('[WARNING] Images path already exists so there could '
                        'end up being images from two runs in one folder or '
@@ -73,21 +71,15 @@
         target_lbox : dict
             The parameters of the labeled bounding box of the detected target.
 
         """
 
         pan_angle, tilt_angle, zoom = ptz_state
 
-        front_bit = time.strftime(self.timestamp_format)
-        # maybe you should avoid a call to time and datetime and just
-        # get everything from datetime. later.
-        now = datetime.now()
-        milliseconds = math.floor(now.microsecond/1000)
-        front_bit = (front_bit
-                     + f'_{milliseconds:03d}')
+        front_bit = datetime.now().strftime(self.timestamp_format)[:-3]
         image_filename = front_bit + '.jpg'
 
         # full_path = os.path.join(self.path, 'images')
         # if not os.path.exists(full_path):
         #     os.mkdir(full_path)
 
         image_filename_w_path = os.path.join(self.image_path,
```

### Comparing `ptzipcam-0.0.4/ptzipcam/video_writer.py` & `ptzipcam-0.0.5/ptzipcam/video_writer.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/ptzipcam/convert.py` & `ptzipcam-0.0.5/ptzipcam/convert.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/ptzipcam/logs.py` & `ptzipcam-0.0.5/ptzipcam/logs.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/ptzipcam/tracker.py` & `ptzipcam-0.0.5/ptzipcam/tracker.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/ptzipcam/ui.py` & `ptzipcam-0.0.5/ptzipcam/ui.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.4/LICENSE` & `ptzipcam-0.0.5/LICENSE`

 * *Files identical despite different names*

