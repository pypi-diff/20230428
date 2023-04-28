# Comparing `tmp/whisper_voice_commands-0.0.1.tar.gz` & `tmp/whisper_voice_commands-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_voice_commands-0.0.1.tar", last modified: Fri Apr 28 13:54:01 2023, max compression
+gzip compressed data, was "whisper_voice_commands-0.0.2.tar", last modified: Fri Apr 28 14:33:03 2023, max compression
```

## Comparing `whisper_voice_commands-0.0.1.tar` & `whisper_voice_commands-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 13:54:01.908698 whisper_voice_commands-0.0.1/
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1070 2023-04-28 13:53:11.000000 whisper_voice_commands-0.0.1/LICENSE
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3377 2023-04-28 13:54:01.908698 whisper_voice_commands-0.0.1/PKG-INFO
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     2795 2023-04-28 13:53:11.000000 whisper_voice_commands-0.0.1/README.md
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1098 2023-04-28 13:53:42.000000 whisper_voice_commands-0.0.1/pyproject.toml
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       38 2023-04-28 13:54:01.908698 whisper_voice_commands-0.0.1/setup.cfg
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 13:54:01.905364 whisper_voice_commands-0.0.1/whisper_mic/
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 13:53:11.000000 whisper_voice_commands-0.0.1/whisper_mic/__init__.py
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)     6004 2023-04-28 13:53:11.000000 whisper_voice_commands-0.0.1/whisper_mic/cli.py
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)       85 2023-04-28 13:53:11.000000 whisper_voice_commands-0.0.1/whisper_mic/mic.py
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 13:54:01.908698 whisper_voice_commands-0.0.1/whisper_voice_commands.egg-info/
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3377 2023-04-28 13:54:01.000000 whisper_voice_commands-0.0.1/whisper_voice_commands.egg-info/PKG-INFO
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      372 2023-04-28 13:54:01.000000 whisper_voice_commands-0.0.1/whisper_voice_commands.egg-info/SOURCES.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)        1 2023-04-28 13:54:01.000000 whisper_voice_commands-0.0.1/whisper_voice_commands.egg-info/dependency_links.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       53 2023-04-28 13:54:01.000000 whisper_voice_commands-0.0.1/whisper_voice_commands.egg-info/entry_points.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      182 2023-04-28 13:54:01.000000 whisper_voice_commands-0.0.1/whisper_voice_commands.egg-info/requires.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       12 2023-04-28 13:54:01.000000 whisper_voice_commands-0.0.1/whisper_voice_commands.egg-info/top_level.txt
+drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 14:33:03.097265 whisper_voice_commands-0.0.2/
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1070 2023-04-28 14:29:36.000000 whisper_voice_commands-0.0.2/LICENSE
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3377 2023-04-28 14:33:03.097265 whisper_voice_commands-0.0.2/PKG-INFO
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     2795 2023-04-28 14:29:36.000000 whisper_voice_commands-0.0.2/README.md
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1098 2023-04-28 14:30:59.000000 whisper_voice_commands-0.0.2/pyproject.toml
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       38 2023-04-28 14:33:03.097265 whisper_voice_commands-0.0.2/setup.cfg
+drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 14:33:03.097265 whisper_voice_commands-0.0.2/whisper_voice_commands.egg-info/
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3377 2023-04-28 14:33:03.000000 whisper_voice_commands-0.0.2/whisper_voice_commands.egg-info/PKG-INFO
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      310 2023-04-28 14:33:03.000000 whisper_voice_commands-0.0.2/whisper_voice_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)        1 2023-04-28 14:33:03.000000 whisper_voice_commands-0.0.2/whisper_voice_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       53 2023-04-28 14:33:03.000000 whisper_voice_commands-0.0.2/whisper_voice_commands.egg-info/entry_points.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      182 2023-04-28 14:33:03.000000 whisper_voice_commands-0.0.2/whisper_voice_commands.egg-info/requires.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)        1 2023-04-28 14:33:03.000000 whisper_voice_commands-0.0.2/whisper_voice_commands.egg-info/top_level.txt
```

### Comparing `whisper_voice_commands-0.0.1/LICENSE` & `whisper_voice_commands-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_voice_commands-0.0.1/PKG-INFO` & `whisper_voice_commands-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_voice_commands
-Version: 0.0.1
+Version: 0.0.2
 Summary: Execute scripts with Whisper for your microphone
 Author-email: Deven B-L <deven.boutin@gmail.com>, Blake Mallory <blakecmallory@gmail.com>
 Project-URL: Homepage, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands
 Project-URL: Bug Tracker, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `whisper_voice_commands-0.0.1/README.md` & `whisper_voice_commands-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `whisper_voice_commands-0.0.1/pyproject.toml` & `whisper_voice_commands-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whisper_voice_commands"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Deven B-L", email="deven.boutin@gmail.com" },
   { name="Blake Mallory", email="blakecmallory@gmail.com" },
 ]
 description = "Execute scripts with Whisper for your microphone"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `whisper_voice_commands-0.0.1/whisper_voice_commands.egg-info/PKG-INFO` & `whisper_voice_commands-0.0.2/whisper_voice_commands.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-voice-commands
-Version: 0.0.1
+Version: 0.0.2
 Summary: Execute scripts with Whisper for your microphone
 Author-email: Deven B-L <deven.boutin@gmail.com>, Blake Mallory <blakecmallory@gmail.com>
 Project-URL: Homepage, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands
 Project-URL: Bug Tracker, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

