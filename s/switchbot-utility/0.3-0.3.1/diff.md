# Comparing `tmp/switchbot_utility-0.3.tar.gz` & `tmp/switchbot_utility-0.3.1.tar.gz`

## Comparing `switchbot_utility-0.3.tar` & `switchbot_utility-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 switchbot_utility-0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 switchbot_utility-0.3/example/create_keypad_passcode.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 switchbot_utility-0.3/example/get_devicelist.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 switchbot_utility-0.3/example/get_plug_status.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 switchbot_utility-0.3/example/get_temperature.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 switchbot_utility-0.3/example/open_curtain.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/_version.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/battery_mixin.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/onoff_mixin.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_blind_tilt.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_bot.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ceiling_light.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ceiling_light_pro.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_color_bulb.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_contact_sensor.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_curtain.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_device.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_humidifier.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_air_conditioner.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_device.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_dvd_speaker.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_fan.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_light.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_others.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_tv_ipstreamer_stb.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_keypad.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_keypad_touch.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_lock.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_meter.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_meter_plus.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_motion_sensor.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_plug.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_plug_mini_jp.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_plug_mini_us.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_robot_vacuum_cleaner_s1.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_robot_vacuum_cleaner_s1_plus.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_strip_light.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 switchbot_utility-0.3/src/switchbot_utility/switchbot_webhook.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 switchbot_utility-0.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 switchbot_utility-0.3/LICENSE
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 switchbot_utility-0.3/README.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 switchbot_utility-0.3/pyproject.toml
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 switchbot_utility-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/example/create_keypad_passcode.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/example/get_devicelist.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/example/get_plug_status.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/example/get_temperature.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/example/open_curtain.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/_version.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/battery_mixin.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/command_mixin.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/onoff_mixin.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_blind_tilt.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_bot.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ceiling_light.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ceiling_light_pro.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_color_bulb.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_contact_sensor.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_curtain.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_device.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_humidifier.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_air_conditioner.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_device.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_dvd_speaker.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_fan.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_light.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_others.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_tv_ipstreamer_stb.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_keypad.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_keypad_touch.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_lock.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_meter.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_meter_plus.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_motion_sensor.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_plug.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_plug_mini_jp.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_plug_mini_us.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_robot_vacuum_cleaner_s1.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_robot_vacuum_cleaner_s1_plus.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_strip_light.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/src/switchbot_utility/switchbot_webhook.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/README.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 switchbot_utility-0.3.1/PKG-INFO
```

### Comparing `switchbot_utility-0.3/.github/workflows/python-publish.yml` & `switchbot_utility-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_blind_tilt.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_blind_tilt.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_bot.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_bot.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_ceiling_light.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ceiling_light.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_color_bulb.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_color_bulb.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_curtain.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_curtain.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_humidifier.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_humidifier.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_air_conditioner.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_air_conditioner.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_dvd_speaker.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_dvd_speaker.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_fan.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_fan.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_light.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_light.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_others.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_others.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_ir_tv_ipstreamer_stb.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_ir_tv_ipstreamer_stb.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_keypad.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_keypad.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_lock.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_lock.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_meter.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_meter.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_motion_sensor.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_motion_sensor.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_plug_mini_us.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_plug_mini_us.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_robot_vacuum_cleaner_s1.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_robot_vacuum_cleaner_s1.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_strip_light.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_strip_light.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/src/switchbot_utility/switchbot_webhook.py` & `switchbot_utility-0.3.1/src/switchbot_utility/switchbot_webhook.py`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/.gitignore` & `switchbot_utility-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/LICENSE` & `switchbot_utility-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/README.md` & `switchbot_utility-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/pyproject.toml` & `switchbot_utility-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `switchbot_utility-0.3/PKG-INFO` & `switchbot_utility-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchbot_utility
-Version: 0.3
+Version: 0.3.1
 Summary: Python Switchbot utilities
 Project-URL: Homepage, https://github.com/iCarrot0605/Switchbot_utility
 Project-URL: Bug Tracker, https://github.com/iCarrot0605/Switchbot_utility/issues
 Author-email: MATSUMURA Hidetoshi <icarrot@mac.com>
 License-File: LICENSE
 Keywords: IoT,Switchbot,Switchbot API
 Classifier: License :: OSI Approved :: MIT License
```

