# Comparing `tmp/vinset-4.0.2.tar.gz` & `tmp/vinset-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinset-4.0.2.tar", last modified: Thu Apr 27 23:33:46 2023, max compression
+gzip compressed data, was "vinset-4.1.0.tar", last modified: Fri Apr 28 03:27:30 2023, max compression
```

## Comparing `vinset-4.0.2.tar` & `vinset-4.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 23:33:46.927344 vinset-4.0.2/
--rw-rw-rw-   0        0        0    11558 2023-03-26 20:05:51.000000 vinset-4.0.2/LICENSE
--rw-rw-rw-   0        0        0      560 2023-04-27 23:33:46.927344 vinset-4.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9583 2023-04-27 21:17:59.000000 vinset-4.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 23:33:46.927344 vinset-4.0.2/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-04-27 23:33:22.000000 vinset-4.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 23:33:46.927344 vinset-4.0.2/vinset/
--rw-rw-rw-   0        0        0        0 2023-03-26 20:05:52.000000 vinset-4.0.2/vinset/__init__.py
--rw-rw-rw-   0        0        0    55766 2023-04-27 23:33:22.000000 vinset-4.0.2/vinset/vin.py
-drwxrwxrwx   0        0        0        0 2023-04-27 23:33:46.927344 vinset-4.0.2/vinset.egg-info/
--rw-rw-rw-   0        0        0      560 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-27 23:33:36.000000 vinset-4.0.2/vinset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 23:33:46.000000 vinset-4.0.2/vinset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 03:27:30.179891 vinset-4.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-03-26 20:05:51.000000 vinset-4.1.0/LICENSE
+-rw-rw-rw-   0        0        0      560 2023-04-28 03:27:30.179891 vinset-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9583 2023-04-27 21:17:59.000000 vinset-4.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 03:27:30.179891 vinset-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-04-28 03:24:25.000000 vinset-4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:27:30.179891 vinset-4.1.0/vinset/
+-rw-rw-rw-   0        0        0        0 2023-03-26 20:05:52.000000 vinset-4.1.0/vinset/__init__.py
+-rw-rw-rw-   0        0        0    59525 2023-04-28 03:24:25.000000 vinset-4.1.0/vinset/vin.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:27:30.179891 vinset-4.1.0/vinset.egg-info/
+-rw-rw-rw-   0        0        0      560 2023-04-28 03:27:29.000000 vinset-4.1.0/vinset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-28 03:27:29.000000 vinset-4.1.0/vinset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 03:27:29.000000 vinset-4.1.0/vinset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-28 03:27:29.000000 vinset-4.1.0/vinset.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-28 03:27:14.000000 vinset-4.1.0/vinset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-04-28 03:27:29.000000 vinset-4.1.0/vinset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 03:27:29.000000 vinset-4.1.0/vinset.egg-info/top_level.txt
```

### Comparing `vinset-4.0.2/LICENSE` & `vinset-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vinset-4.0.2/PKG-INFO` & `vinset-4.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 4.0.2
+Version: 4.1.0
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vinset-4.0.2/README.md` & `vinset-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vinset-4.0.2/setup.py` & `vinset-4.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw the graph from video and csv files.'
 
 setup(
     name='vinset',
-    version='4.0.2',
+    version='4.1.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/vinset',
     description='gaze visualisation program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

### Comparing `vinset-4.0.2/vinset/vin.py` & `vinset-4.1.0/vinset/vin.py`

 * *Files 4% similar despite different names*

```diff
@@ -843,41 +843,46 @@
         frame_count = input_video.get(cv2.CAP_PROP_FRAME_COUNT)
         print("Frame count:", frame_count)
 
         stimulus_level_array = get_logmar_level_array(timeline_info, text_info)
 
         final_stimulus_level_array = add_logmar_interval(stimulus_level_array, text_info)
 
+        # for data in final_stimulus_level_array:
+        #     print(data)
+        # return
+
         max_video_length = math.ceil(frame_count_to_time(frame_count, frame_rate))
         print(f"Video length:{max_video_length / 1000} sec")
 
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         v_writer = cv2.VideoWriter(output_video_file, fourcc, int(frame_rate), (int(frame_width), int(frame_height)))
         whole_t = time.time()
         count = 0
         drawing_graph = True
         start_drawing = False
         stimulus_display_text = None
         sweep_order = None
         final_stimulus_level_array_length = len(final_stimulus_level_array)
+        # print(final_stimulus_level_array_length)
         stimulus_index = 0
 
         while drawing_graph:
-
             # start_tt = time.time()
             ret, frame = input_video.read()
             # end_tt = time.time()
             print_percent_done(count, frame_count)
             check_timer = frame_count_to_time(count, frame_rate)
 
             if ret:
                 if stimulus_index < final_stimulus_level_array_length:
                     stimulus_timestamp_to_check = final_stimulus_level_array[stimulus_index]["timestamp"] * 1000
                     if check_timer >= stimulus_timestamp_to_check:
                         start_drawing = True
+                        print(stimulus_index)
                         stimulus_display_text = str(final_stimulus_level_array[stimulus_index]["logmar"])
                         sweep_order = final_stimulus_level_array[stimulus_index]["sweep_order"]
                         stimulus_index += 1
 
                 if start_drawing:
                     nearest_stimulus_text = get_nearest_stimulus(stimulus_display_text)
                     cv2.putText(frame, f"Stimulus Level:{str(nearest_stimulus_text)}", (sti_x_position, sti_y_position),
@@ -910,30 +915,61 @@
         input_video.release()
         v_writer.release()
         cv2.destroyAllWindows()
 
 
 def get_logmar_level_array(timeline_info_info, text_info_input):
     draw_data = []
+    end_marker_indicator = text_info_input["end_marker_location"]
+    end_marker_name = text_info_input["end_marker_name"]
+    # tt = trial_type
+    end_marker_tt = text_info_input["end_marker_trial_type"]
+    tt_indicator = text_info_input["end_marker_trial_type_location"]
     text_indicator = text_info_input["text_marker_location"]
     time_indicator = text_info_input["time_marker_location"]
     first_text_indicator, second_text_indicator, third_text_indicator = str(text_indicator).split("->")
+    first_end_indicator, second_end_indicator, third_end_indicator = str(end_marker_indicator).split("->")
+    first_tt_indicator, second_tt_indicator, third_tt_indicator = str(tt_indicator).split("->")
     first_time_indicator, second_time_indicator, third_time_indicator = str(time_indicator).split("->")
     minimum_va_decimal = text_info_input["minimum_va_decimal"]
+    stimulus_step = text_info_input["stimulus_step"]
+    last_logmar = None
+    second_last_logmar = None
     for event in timeline_info_info:
         first_attribute = str(list(event.keys())[0])
+        try:
+            second_attribute = str(list(event.keys())[1])
+        except IndexError:
+            second_attribute = None
         if first_attribute == first_text_indicator:
             event_info = event[first_attribute]
             time_value = event_info[second_time_indicator][third_time_indicator]
             text_value = str(round((float(event_info[second_text_indicator][third_text_indicator])), 2))
             text_value = check_and_add_decimal(text_value, minimum_va_decimal)
-            data = {"timestamp": time_value, "logmar": text_value}
+            if last_logmar:
+                second_last_logmar = last_logmar
+                last_logmar = text_value
+            else:
+                last_logmar = text_value
+            data = {"marker_name": first_attribute, "timestamp": time_value, "logmar": text_value}
             draw_data.append(data)
-    # for data in draw_data:
-    #     print(data)
+        elif second_attribute is not None and second_attribute == first_end_indicator:
+            event_info = event[second_attribute]
+            end_marker_string = event_info[second_end_indicator][third_end_indicator]
+            tt_string = event_info[second_tt_indicator][third_tt_indicator]
+            if end_marker_string == end_marker_name and tt_string == end_marker_tt:
+                time_value = event_info[second_time_indicator][third_time_indicator]
+                if last_logmar < second_last_logmar:
+                    text_value = str(round(float(last_logmar) - stimulus_step, 1))
+                else:
+                    text_value = str(round(float(last_logmar) + stimulus_step, 1))
+                data = {"marker_name": second_attribute, "timestamp": time_value, "logmar": text_value}
+                draw_data.append(data)
+    # for d in draw_data:
+    #     print(d)
 
     return draw_data
 
 
 def add_logmar_interval(draw_data_array_input, text_info_input):
     va_logmar_interval = text_info_input["va_logmar_interval"]
     draw_data_array_length = len(draw_data_array_input)
@@ -945,39 +981,65 @@
         if index is not last_index:
             first_value = draw_data_array_input[index]
             second_value = draw_data_array_input[index + 1]
             first_logmar = float(first_value["logmar"])
             second_logmar = float(second_value["logmar"])
             first_timestamp = first_value["timestamp"]
             second_timestamp = second_value["timestamp"]
+            first_marker = first_value["marker_name"]
+            second_marker = second_value["marker_name"]
 
-            logmar_diff = first_logmar - second_logmar
-            sweep_order = "descending" if logmar_diff >= 0 else "ascending"
-            number_of_intervals = int(round(abs(logmar_diff), 1) / va_logmar_interval)
-            first_value["sweep_order"] = sweep_order
-            second_value["sweep_order"] = sweep_order
-
-            if logmar_diff == 0:
-                first_value["sweep_order"] = "resting"
-                second_value["sweep_order"] = "resting"
-                final_data_array.append(first_value)
-                final_data_array.append(second_value)
+            if first_logmar > second_logmar:
+                sweep_order = "descending"
+            elif first_logmar < second_logmar:
+                sweep_order = "ascending"
             else:
-                extra_data = number_of_intervals - 1
-                each_time_interval_duration = (second_timestamp - first_timestamp) / number_of_intervals
-                final_data_array.append(first_value)
-                for ind in range(extra_data):
-                    time_value = first_timestamp + ((ind + 1) * each_time_interval_duration)
-                    if sweep_order == "descending":
-                        text_value = str(round((first_logmar - ((ind + 1) * va_logmar_interval)), 2))
-                    else:
-                        text_value = str(round(first_logmar + ((ind + 1) * va_logmar_interval), 2))
-                    data = {"timestamp": time_value, "logmar": text_value, "sweep_order":sweep_order}
-                    final_data_array.append(data)
-                final_data_array.append(second_value)
+                sweep_order = None
+            if sweep_order:
+                if first_marker == "end":
+                    first_value["sweep_order"] = "resting"
+                    second_value["sweep_order"] = sweep_order
+                    final_data_array.append(first_value)
+                    final_data_array.append(second_value)
+                elif second_marker == "end":
+                    first_value["sweep_order"] = sweep_order
+                    second_value["sweep_order"] = "resting"
+                    logmar_diff = first_logmar - second_logmar
+                    number_of_intervals = int(round(abs(logmar_diff), 1) / va_logmar_interval)
+                    extra_data = number_of_intervals - 1
+                    each_time_interval_duration = (second_timestamp - first_timestamp) / number_of_intervals
+                    final_data_array.append(first_value)
+                    for ind in range(extra_data):
+                        time_value = first_timestamp + ((ind + 1) * each_time_interval_duration)
+                        if sweep_order == "descending":
+                            text_value = str(round((first_logmar - ((ind + 1) * va_logmar_interval)), 2))
+                        else:
+                            text_value = str(round(first_logmar + ((ind + 1) * va_logmar_interval), 2))
+                        data = {"marker_name": second_marker, "timestamp": time_value, "logmar": text_value,
+                                "sweep_order": sweep_order}
+                        final_data_array.append(data)
+                    final_data_array.append(second_value)
+                else:
+                    logmar_diff = first_logmar - second_logmar
+                    number_of_intervals = int(round(abs(logmar_diff), 1) / va_logmar_interval)
+                    first_value["sweep_order"] = sweep_order
+                    second_value["sweep_order"] = sweep_order
+                    extra_data = number_of_intervals - 1
+                    each_time_interval_duration = (second_timestamp - first_timestamp) / number_of_intervals
+                    final_data_array.append(first_value)
+                    for ind in range(extra_data):
+                        time_value = first_timestamp + ((ind + 1) * each_time_interval_duration)
+                        if sweep_order == "descending":
+                            text_value = str(round((first_logmar - ((ind + 1) * va_logmar_interval)), 2))
+                        else:
+                            text_value = str(round(first_logmar + ((ind + 1) * va_logmar_interval), 2))
+                        data = {"marker_name": first_marker, "timestamp": time_value, "logmar": text_value,
+                                "sweep_order": sweep_order}
+                        final_data_array.append(data)
+                    final_data_array.append(second_value)
     last_data = final_data_array[-1]
     last_data["sweep_order"] = "resting"
     final_data_array = list({dictionary['timestamp']: dictionary for dictionary in final_data_array}.values())
 
     return final_data_array
 
 
@@ -1009,15 +1071,15 @@
         if float(string_input) < stimulus_value:
             string_input = str(round(float(string_input) + 0.1, 1))
     return string_input
 
 
 def main():
     parser = argparse.ArgumentParser(prog='vinset', description='VINSET package.')
-    parser.add_argument('--version', action='version', version='4.0.2'),
+    parser.add_argument('--version', action='version', version='4.1.0'),
     parser.add_argument("-i", dest="input_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
                         help="input mp4 file", metavar="filename.mp4")
     parser.add_argument("-d", dest="input_data_filename", required=False, type=argparse.FileType('r'),
                         default=sys.stdin,
                         help="input csv data file", metavar="filename.csv")
     parser.add_argument("-o", dest="output_filename", required=True, type=argparse.FileType('w'), default=sys.stdout,
                         help="output mp4 file", metavar="filename.mp4")
```

### Comparing `vinset-4.0.2/vinset.egg-info/PKG-INFO` & `vinset-4.1.0/vinset.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 4.0.2
+Version: 4.1.0
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
 Classifier: Programming Language :: Python :: 3
```

