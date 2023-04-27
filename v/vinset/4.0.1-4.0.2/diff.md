# Comparing `tmp/vinset-4.0.1.tar.gz` & `tmp/vinset-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinset-4.0.1.tar", last modified: Thu Apr 27 06:08:15 2023, max compression
+gzip compressed data, was "vinset-4.0.2.tar", last modified: Thu Apr 27 23:33:46 2023, max compression
```

## Comparing `vinset-4.0.1.tar` & `vinset-4.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 06:08:15.871229 vinset-4.0.1/
--rw-rw-rw-   0        0        0    11558 2023-02-15 23:27:28.000000 vinset-4.0.1/LICENSE
--rw-rw-rw-   0        0        0      581 2023-04-27 06:08:15.870231 vinset-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9583 2023-04-27 05:44:25.000000 vinset-4.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 06:08:15.871229 vinset-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-04-27 05:56:07.000000 vinset-4.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 06:08:15.857266 vinset-4.0.1/vinset/
--rw-rw-rw-   0        0        0        0 2023-02-15 23:27:29.000000 vinset-4.0.1/vinset/__init__.py
--rw-rw-rw-   0        0        0    55697 2023-04-27 05:56:07.000000 vinset-4.0.1/vinset/vin.py
-drwxrwxrwx   0        0        0        0 2023-04-27 06:08:15.869234 vinset-4.0.1/vinset.egg-info/
--rw-rw-rw-   0        0        0      581 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-27 06:07:44.000000 vinset-4.0.1/vinset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 23:33:46.927344 vinset-4.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-03-26 20:05:51.000000 vinset-4.0.2/LICENSE
+-rw-rw-rw-   0        0        0      560 2023-04-27 23:33:46.927344 vinset-4.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9583 2023-04-27 21:17:59.000000 vinset-4.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 23:33:46.927344 vinset-4.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-04-27 23:33:22.000000 vinset-4.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:33:46.927344 vinset-4.0.2/vinset/
+-rw-rw-rw-   0        0        0        0 2023-03-26 20:05:52.000000 vinset-4.0.2/vinset/__init__.py
+-rw-rw-rw-   0        0        0    55766 2023-04-27 23:33:22.000000 vinset-4.0.2/vinset/vin.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:33:46.927344 vinset-4.0.2/vinset.egg-info/
+-rw-rw-rw-   0        0        0      560 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-27 23:33:36.000000 vinset-4.0.2/vinset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/top_level.txt
```

### Comparing `vinset-4.0.1/LICENSE` & `vinset-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vinset-4.0.1/PKG-INFO` & `vinset-4.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 4.0.1
+Version: 4.0.2
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Command line program to draw the graph from video and csv files.
-
```

### Comparing `vinset-4.0.1/README.md` & `vinset-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vinset-4.0.1/setup.py` & `vinset-4.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw the graph from video and csv files.'
 
 setup(
     name='vinset',
-    version='4.0.1',
+    version='4.0.2',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/vinset',
     description='gaze visualisation program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

### Comparing `vinset-4.0.1/vinset/vin.py` & `vinset-4.0.2/vinset/vin.py`

 * *Files 0% similar despite different names*

```diff
@@ -843,18 +843,14 @@
         frame_count = input_video.get(cv2.CAP_PROP_FRAME_COUNT)
         print("Frame count:", frame_count)
 
         stimulus_level_array = get_logmar_level_array(timeline_info, text_info)
 
         final_stimulus_level_array = add_logmar_interval(stimulus_level_array, text_info)
 
-        # for d in final_stimulus_level_array:
-        #     print(d)
-        # return
-
         max_video_length = math.ceil(frame_count_to_time(frame_count, frame_rate))
         print(f"Video length:{max_video_length / 1000} sec")
 
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         v_writer = cv2.VideoWriter(output_video_file, fourcc, int(frame_rate), (int(frame_width), int(frame_height)))
         whole_t = time.time()
         count = 0
@@ -1001,24 +997,27 @@
         output = string_input
         output_string = check_and_add_decimal(output, min_decimal_input)
     return output_string
 
 
 def get_nearest_stimulus(string_input):
     point_index = str(string_input).find(".") + 2
+    stimulus_value = float(string_input)
     if point_index > -1:
         string_input = string_input[:point_index]
         if float(string_input) == 0:
             string_input = "0.0"
+        if float(string_input) < stimulus_value:
+            string_input = str(round(float(string_input) + 0.1, 1))
     return string_input
 
 
 def main():
     parser = argparse.ArgumentParser(prog='vinset', description='VINSET package.')
-    parser.add_argument('--version', action='version', version='4.0.1'),
+    parser.add_argument('--version', action='version', version='4.0.2'),
     parser.add_argument("-i", dest="input_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
                         help="input mp4 file", metavar="filename.mp4")
     parser.add_argument("-d", dest="input_data_filename", required=False, type=argparse.FileType('r'),
                         default=sys.stdin,
                         help="input csv data file", metavar="filename.csv")
     parser.add_argument("-o", dest="output_filename", required=True, type=argparse.FileType('w'), default=sys.stdout,
                         help="output mp4 file", metavar="filename.mp4")
```

### Comparing `vinset-4.0.1/vinset.egg-info/PKG-INFO` & `vinset-4.0.2/vinset.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 4.0.1
+Version: 4.0.2
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Command line program to draw the graph from video and csv files.
-
```

