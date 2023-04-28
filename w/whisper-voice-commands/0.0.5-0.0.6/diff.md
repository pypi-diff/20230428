# Comparing `tmp/whisper_voice_commands-0.0.5.tar.gz` & `tmp/whisper_voice_commands-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_voice_commands-0.0.5.tar", last modified: Fri Apr 28 18:49:15 2023, max compression
+gzip compressed data, was "whisper_voice_commands-0.0.6.tar", last modified: Fri Apr 28 19:03:41 2023, max compression
```

## Comparing `whisper_voice_commands-0.0.5.tar` & `whisper_voice_commands-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 18:49:15.423626 whisper_voice_commands-0.0.5/
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1070 2023-04-28 16:32:31.000000 whisper_voice_commands-0.0.5/LICENSE
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3693 2023-04-28 18:49:15.423626 whisper_voice_commands-0.0.5/PKG-INFO
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3116 2023-04-28 16:32:31.000000 whisper_voice_commands-0.0.5/README.md
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1109 2023-04-28 18:46:38.000000 whisper_voice_commands-0.0.5/pyproject.toml
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       38 2023-04-28 18:49:15.423626 whisper_voice_commands-0.0.5/setup.cfg
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 18:49:15.423626 whisper_voice_commands-0.0.5/whisper_mic/
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 16:32:31.000000 whisper_voice_commands-0.0.5/whisper_mic/__init__.py
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)     6440 2023-04-28 18:43:58.000000 whisper_voice_commands-0.0.5/whisper_mic/cli.py
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)       85 2023-04-28 16:32:31.000000 whisper_voice_commands-0.0.5/whisper_mic/mic.py
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 18:49:15.423626 whisper_voice_commands-0.0.5/whisper_voice_commands.egg-info/
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3693 2023-04-28 18:49:15.000000 whisper_voice_commands-0.0.5/whisper_voice_commands.egg-info/PKG-INFO
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      372 2023-04-28 18:49:15.000000 whisper_voice_commands-0.0.5/whisper_voice_commands.egg-info/SOURCES.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)        1 2023-04-28 18:49:15.000000 whisper_voice_commands-0.0.5/whisper_voice_commands.egg-info/dependency_links.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       64 2023-04-28 18:49:15.000000 whisper_voice_commands-0.0.5/whisper_voice_commands.egg-info/entry_points.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      182 2023-04-28 18:49:15.000000 whisper_voice_commands-0.0.5/whisper_voice_commands.egg-info/requires.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       12 2023-04-28 18:49:15.000000 whisper_voice_commands-0.0.5/whisper_voice_commands.egg-info/top_level.txt
+drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 19:03:41.303419 whisper_voice_commands-0.0.6/
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1070 2023-04-28 19:03:28.000000 whisper_voice_commands-0.0.6/LICENSE
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3693 2023-04-28 19:03:41.303419 whisper_voice_commands-0.0.6/PKG-INFO
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3116 2023-04-28 19:03:28.000000 whisper_voice_commands-0.0.6/README.md
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1109 2023-04-28 19:03:28.000000 whisper_voice_commands-0.0.6/pyproject.toml
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       38 2023-04-28 19:03:41.303419 whisper_voice_commands-0.0.6/setup.cfg
+drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 19:03:41.303419 whisper_voice_commands-0.0.6/whisper_mic/
+-rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 19:03:28.000000 whisper_voice_commands-0.0.6/whisper_mic/__init__.py
+-rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)     6463 2023-04-28 19:03:28.000000 whisper_voice_commands-0.0.6/whisper_mic/cli.py
+-rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)       85 2023-04-28 19:03:28.000000 whisper_voice_commands-0.0.6/whisper_mic/mic.py
+drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 19:03:41.303419 whisper_voice_commands-0.0.6/whisper_voice_commands.egg-info/
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3693 2023-04-28 19:03:41.000000 whisper_voice_commands-0.0.6/whisper_voice_commands.egg-info/PKG-INFO
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      372 2023-04-28 19:03:41.000000 whisper_voice_commands-0.0.6/whisper_voice_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)        1 2023-04-28 19:03:41.000000 whisper_voice_commands-0.0.6/whisper_voice_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       64 2023-04-28 19:03:41.000000 whisper_voice_commands-0.0.6/whisper_voice_commands.egg-info/entry_points.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      182 2023-04-28 19:03:41.000000 whisper_voice_commands-0.0.6/whisper_voice_commands.egg-info/requires.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       12 2023-04-28 19:03:41.000000 whisper_voice_commands-0.0.6/whisper_voice_commands.egg-info/top_level.txt
```

### Comparing `whisper_voice_commands-0.0.5/LICENSE` & `whisper_voice_commands-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_voice_commands-0.0.5/PKG-INFO` & `whisper_voice_commands-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_voice_commands
-Version: 0.0.5
+Version: 0.0.6
 Summary: Execute scripts with Whisper for your microphone
 Author-email: Deven B-L <deven.boutin@gmail.com>, Blake Mallory <blakecmallory@gmail.com>
 Project-URL: Homepage, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands
 Project-URL: Bug Tracker, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `whisper_voice_commands-0.0.5/README.md` & `whisper_voice_commands-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `whisper_voice_commands-0.0.5/pyproject.toml` & `whisper_voice_commands-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whisper_voice_commands"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Deven B-L", email="deven.boutin@gmail.com" },
   { name="Blake Mallory", email="blakecmallory@gmail.com" },
 ]
 description = "Execute scripts with Whisper for your microphone"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `whisper_voice_commands-0.0.5/whisper_mic/cli.py` & `whisper_voice_commands-0.0.6/whisper_mic/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # @click.option("--script_path", help="runs scripts in script_path directories based on keywords", multiple=True, type=click.Path())
 @click.option("--script_extensions", '-s', default=[], help="valid script extensions to execute ex: .bash, defaults to .bash .py if none are provided", multiple=True, type=str)
 @click.option("--ambient", default=False, help="allows for ambient noise adjustment at startup",is_flag=True,type=bool)
 @click.option("--english", default=False, help="Whether to use English model",is_flag=True, type=bool)
 @click.option("--verbose", default=False, help="Whether to print verbose output", is_flag=True,type=bool)
 @click.option("--energy", default=300, help="Energy level for mic to detect", type=int)
 @click.option("--dynamic_energy", default=False,is_flag=True, help="Flag to enable dynamic energy", type=bool)
-@click.option("--pause", default=0.1, help="Pause time before entry ends", type=float)
-@click.option("--phrase_length", default=0.8, help="minimum sound length for transcription to start (set to 0.3 to transcribe basically everything default 0.8 )", type=float)
+@click.option("--pause", default=0.5, help="Pause time before entry ends", type=float)
+@click.option("--phrase_length", default=0.4, help="minimum sound length for transcription to start (set to 0.3 to transcribe basically everything, for a low false positive rate 0.8 )", type=float)
 @click.option("--save_file",default=False, help="Flag to save file", is_flag=True,type=bool)
 def main(model, english,verbose, energy, pause,dynamic_energy,save_file,device,script_path,script_extensions,ambient,phrase_length):
     temp_dir = tempfile.mkdtemp() if save_file else None
     #there are no english models for large
     if model != "large" and english:
         model = model + ".en"
     audio_model = whisper.load_model(model).to(device)
```

### Comparing `whisper_voice_commands-0.0.5/whisper_voice_commands.egg-info/PKG-INFO` & `whisper_voice_commands-0.0.6/whisper_voice_commands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-voice-commands
-Version: 0.0.5
+Version: 0.0.6
 Summary: Execute scripts with Whisper for your microphone
 Author-email: Deven B-L <deven.boutin@gmail.com>, Blake Mallory <blakecmallory@gmail.com>
 Project-URL: Homepage, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands
 Project-URL: Bug Tracker, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

