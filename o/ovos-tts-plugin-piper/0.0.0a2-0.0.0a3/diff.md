# Comparing `tmp/ovos_tts_plugin_piper-0.0.0a2-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_piper-0.0.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10980 bytes, number of entries: 10
--rw-r--r--  2.0 unx    11610 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper/__init__.py
--rw-r--r--  2.0 unx     4518 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper/engine.py
--rw-r--r--  2.0 unx      178 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper-0.0.0a2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper-0.0.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper-0.0.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper-0.0.0a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper-0.0.0a2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper-0.0.0a2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      948 b- defN 23-Apr-28 04:40 ovos_tts_plugin_piper-0.0.0a2.dist-info/RECORD
-10 files, 29969 bytes uncompressed, 9320 bytes compressed:  68.9%
+Zip file size: 10969 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    11569 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper/__init__.py
+-rw-r--r--  2.0 unx     4518 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper/engine.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      948 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/RECORD
+10 files, 29928 bytes uncompressed, 9309 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: ovos_tts_plugin_piper/engine.py
 Comment: 
 
 Filename: ovos_tts_plugin_piper/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a2.dist-info/LICENSE
+Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a2.dist-info/METADATA
+Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a2.dist-info/WHEEL
+Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a2.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a2.dist-info/top_level.txt
+Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a2.dist-info/zip-safe
+Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a2.dist-info/RECORD
+Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_piper/__init__.py

```diff
@@ -203,10 +203,10 @@
     # TODO - list of all models + url + auto download if needed to XDG path
 }
 
 if __name__ == "__main__":
 
 
     config = {}
-    config["model"] = "~/ovos-tts-plugin-piper/en-gb-southern_english_female-low.onnx"
-    e = PiperTTSPlugin()
+    config["model"] = "alan-low"
+    e = PiperTTSPlugin(config=config)
     e.get_tts("hello world", "hello.wav")
```

## ovos_tts_plugin_piper/version.py

```diff
@@ -1,8 +1,8 @@
 
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_piper-0.0.0a2.dist-info/LICENSE` & `ovos_tts_plugin_piper-0.0.0a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_piper-0.0.0a2.dist-info/METADATA` & `ovos_tts_plugin_piper-0.0.0a3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-piper
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: piper tts plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-piper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft plugin tts OVOS OpenVoiceOS
 Platform: UNKNOWN
```

## Comparing `ovos_tts_plugin_piper-0.0.0a2.dist-info/RECORD` & `ovos_tts_plugin_piper-0.0.0a3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-ovos_tts_plugin_piper/__init__.py,sha256=r2WaGVD7GZWa5P7p2ZXfRa7eRaTFxccr96utL5DEgkE,11610
+ovos_tts_plugin_piper/__init__.py,sha256=zqb_9ZhEdX7CLSPBv2Aml40dfK-V5R6toHsIgm4b4G0,11569
 ovos_tts_plugin_piper/engine.py,sha256=WEB-2Uu9cmN3UQrltWYbB0PH1H0X03Fg6OnGXW-GS0s,4518
-ovos_tts_plugin_piper/version.py,sha256=zDy7aRJDFkQ3ABSRqkH4YuJQHLOXLb9wSbGZ35NAvH0,178
-ovos_tts_plugin_piper-0.0.0a2.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_tts_plugin_piper-0.0.0a2.dist-info/METADATA,sha256=IpK29bMZrqxz4X3Yw-jVWZ-bqm4pq9ONBb0pP6lNRDo,1065
-ovos_tts_plugin_piper-0.0.0a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_piper-0.0.0a2.dist-info/entry_points.txt,sha256=eHpADEdMHzf8Y-h30EKm587TkxMsv91Xb98ph3DgRUY,186
-ovos_tts_plugin_piper-0.0.0a2.dist-info/top_level.txt,sha256=WTvxxS42UAwh0oi25ypLaxvMGD85j_wGzrux2QFoqLs,22
-ovos_tts_plugin_piper-0.0.0a2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_tts_plugin_piper-0.0.0a2.dist-info/RECORD,,
+ovos_tts_plugin_piper/version.py,sha256=XnMBjlWuu_KTmVhM03VIPZxO-m0dNEV7U3SwDK8Amyg,178
+ovos_tts_plugin_piper-0.0.0a3.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_tts_plugin_piper-0.0.0a3.dist-info/METADATA,sha256=umyOFFxfY6HYpq5SQTnhduGFUOhuN4p-8gINhzOFJYE,1065
+ovos_tts_plugin_piper-0.0.0a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_piper-0.0.0a3.dist-info/entry_points.txt,sha256=eHpADEdMHzf8Y-h30EKm587TkxMsv91Xb98ph3DgRUY,186
+ovos_tts_plugin_piper-0.0.0a3.dist-info/top_level.txt,sha256=WTvxxS42UAwh0oi25ypLaxvMGD85j_wGzrux2QFoqLs,22
+ovos_tts_plugin_piper-0.0.0a3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_tts_plugin_piper-0.0.0a3.dist-info/RECORD,,
```

