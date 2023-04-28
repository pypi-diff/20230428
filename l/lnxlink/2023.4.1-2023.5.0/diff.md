# Comparing `tmp/lnxlink-2023.4.1.tar.gz` & `tmp/lnxlink-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnxlink-2023.4.1.tar", last modified: Thu Apr 20 18:41:29 2023, max compression
+gzip compressed data, was "lnxlink-2023.5.0.tar", last modified: Fri Apr 28 21:27:57 2023, max compression
```

## Comparing `lnxlink-2023.4.1.tar` & `lnxlink-2023.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:29.617223 lnxlink-2023.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-20 18:41:29.617223 lnxlink-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:29.613223 lnxlink-2023.4.1/lnxlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12635 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:29.617223 lnxlink-2023.4.1/lnxlink/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/boot_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/camera_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/microphone_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/network_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/network_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/notify.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/nvidia_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/required_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/screen_onoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/send_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/suspend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/sys_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/webcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/xdg_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:29.613223 lnxlink-2023.4.1/lnxlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-20 18:41:28.000000 lnxlink-2023.4.1/lnxlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 18:41:29.617223 lnxlink-2023.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/lnxlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12861 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/lnxlink/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/boot_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/camera_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/microphone_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/network_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/network_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/nvidia_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/required_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/screen_onoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/sys_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/xdg_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/lnxlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-28 21:27:57.000000 lnxlink-2023.5.0/lnxlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/setup.cfg
```

### Comparing `lnxlink-2023.4.1/LICENSE.md` & `lnxlink-2023.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/PKG-INFO` & `lnxlink-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.4.1
+Version: 2023.5.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnxlink-2023.4.1/README.md` & `lnxlink-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/__main__.py` & `lnxlink-2023.5.0/lnxlink/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,20 @@
         # Read configuration from yaml file
         self.pref_topic = 'lnxlink'
         self.config = self.read_config(config_path)
 
         # Run each addon included in the modules folder
         self.Addons = {}
         for service, addon in modules.parse_modules(self.config['modules']).items():
-            self.Addons[addon.service] = addon(self)
+            try:
+                tmp_addon = addon(self)
+                self.Addons[addon.service] = tmp_addon
+            except Exception as e:
+                print(f"Error with addon {addon.service}, please remove it from your config")
+                traceback.print_exc()
 
         # Setup MQTT
         self.client = mqtt.Client()
         self.setup_mqtt()
 
     def publish_monitor_data(self, topic, pub_data):
         # print(topic, pub_data, type(pub_data))
```

### Comparing `lnxlink-2023.4.1/lnxlink/config.py` & `lnxlink-2023.5.0/lnxlink/config.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/consts.py` & `lnxlink-2023.5.0/lnxlink/consts.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/__init__.py` & `lnxlink-2023.5.0/lnxlink/modules/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                     sys.path.append(module_path)
                     addon = getattr(import_module(f"{module_name}"), 'Addon')
                 else:
                     addon = getattr(import_module(f"{__name__}.{module_name}"), 'Addon')
                 addon.service = module_name
                 modules[module_name] = addon
                 retries = -1
-                print(f"Successfully loaded addon: {module_name}")
+                print(f"Loaded addon: {module_name}")
             except ModuleNotFoundError as e:
                 print(f"Addon {module_name} is not supported, please remove it from your config")
                 print(e)
                 retries = -1
             except Exception as e:
                 print("----------------")
                 print(f"Error with module: {module_name}")
```

### Comparing `lnxlink-2023.4.1/lnxlink/modules/battery.py` & `lnxlink-2023.5.0/lnxlink/modules/battery.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/boot_select.py` & `lnxlink-2023.5.0/lnxlink/modules/boot_select.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,17 @@
         stdout = subprocess.run(
             'grub-editenv list',
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE).stdout.decode("UTF-8")
         nextentry_pattern = re.compile(r"^next_entry=(\d+)")
         nextentry_match = re.match(nextentry_pattern, stdout)
-        entry_ind = int(nextentry_match.group(1))
+        entry_ind = 0
+        if nextentry_match:
+            entry_ind = int(nextentry_match.group(1))
 
         return self.options[entry_ind]
 
     def exposedControls(self):
         return {
             "Boot Select": {
                 "type": "select",
```

### Comparing `lnxlink-2023.4.1/lnxlink/modules/brightness.py` & `lnxlink-2023.5.0/lnxlink/modules/brightness.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/camera_used.py` & `lnxlink-2023.5.0/lnxlink/modules/camera_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/disk_usage.py` & `lnxlink-2023.5.0/lnxlink/modules/disk_usage.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/keep_alive.py` & `lnxlink-2023.5.0/lnxlink/modules/keep_alive.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/media.py` & `lnxlink-2023.5.0/lnxlink/modules/media.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/microphone_used.py` & `lnxlink-2023.5.0/lnxlink/modules/microphone_used.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 class Addon():
 
     def __init__(self, lnxlink):
         self.name = 'Microphone used'
         self.icon = 'mdi:microphone'
         self.sensor_type = 'binary_sensor'
 
-        self.use_pactl = subprocess.run(f"which pactl && pactl -f json list", shell=True).returncode == 0
+        self.use_pactl = subprocess.run(
+            f"which pactl && pactl -f json list",
+            shell=True,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE).returncode == 0
 
 
     def getInfo(self):
         if self.use_pactl:
             stdout = subprocess.run(f"pactl -f json list", shell=True,
                                     stdout=subprocess.PIPE,
                                     stderr=subprocess.PIPE).stdout.decode("UTF-8")
```

### Comparing `lnxlink-2023.4.1/lnxlink/modules/network_download.py` & `lnxlink-2023.5.0/lnxlink/modules/network_download.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/network_upload.py` & `lnxlink-2023.5.0/lnxlink/modules/network_upload.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/notify.py` & `lnxlink-2023.5.0/lnxlink/modules/notify.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/nvidia_gpu.py` & `lnxlink-2023.5.0/lnxlink/modules/nvidia_gpu.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/screen_onoff.py` & `lnxlink-2023.5.0/lnxlink/modules/screen_onoff.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/screenshot.py` & `lnxlink-2023.5.0/lnxlink/modules/screenshot.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/sys_updates.py` & `lnxlink-2023.5.0/lnxlink/modules/sys_updates.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/update.py` & `lnxlink-2023.5.0/lnxlink/modules/update.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/modules/webcam.py` & `lnxlink-2023.5.0/lnxlink/modules/webcam.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink/system_monitor.py` & `lnxlink-2023.5.0/lnxlink/system_monitor.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/lnxlink.egg-info/PKG-INFO` & `lnxlink-2023.5.0/lnxlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.4.1
+Version: 2023.5.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnxlink-2023.4.1/lnxlink.egg-info/SOURCES.txt` & `lnxlink-2023.5.0/lnxlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.1/pyproject.toml` & `lnxlink-2023.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name              = "lnxlink"
-version           = "2023.4.1"
+version           = "2023.5.0"
 description       = "Internet Of Things (IOT) integration with Linux using MQTT"
 readme            = "README.md"
 keywords          = ["lnxlink"]
 requires-python   = ">=3.7.0"
 authors     = [
     {name="bkbilly", email="bkbilly@hotmail.com"}
 ]
@@ -26,15 +26,16 @@
     "pyalsaaudio>=0.9.2",
     "dbus-python>=1.3.2",
     "pgi>=0.0.11.2",
     "pyOpenSSL>=22.1.0",
     "requests>=2.28.1",
     "jc>=1.23.0",
     "dbus-idle>=2023.3.2",
-    "opencv-python>=4.7.0.68"
+    "opencv-python>=4.7.0.68",
+    "mss>=7.0.1"
 ]
 
 
 [project.urls]
 "Source Code" = "https://github.com/bkbilly/lnxlink"
 "Home Page"   = "https://bkbilly.github.io/lnxlink"
```

