# Comparing `tmp/whisper_voice_commands-0.0.3.tar.gz` & `tmp/whisper_voice_commands-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_voice_commands-0.0.3.tar", last modified: Fri Apr 28 14:47:37 2023, max compression
+gzip compressed data, was "whisper_voice_commands-0.0.4.tar", last modified: Fri Apr 28 15:10:16 2023, max compression
```

## Comparing `whisper_voice_commands-0.0.3.tar` & `whisper_voice_commands-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 14:47:37.183886 whisper_voice_commands-0.0.3/
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1070 2023-04-28 14:46:44.000000 whisper_voice_commands-0.0.3/LICENSE
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3377 2023-04-28 14:47:37.183886 whisper_voice_commands-0.0.3/PKG-INFO
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     2795 2023-04-28 14:46:44.000000 whisper_voice_commands-0.0.3/README.md
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1109 2023-04-28 14:47:08.000000 whisper_voice_commands-0.0.3/pyproject.toml
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       38 2023-04-28 14:47:37.183886 whisper_voice_commands-0.0.3/setup.cfg
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 14:47:37.183886 whisper_voice_commands-0.0.3/whisper_mic/
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 14:46:44.000000 whisper_voice_commands-0.0.3/whisper_mic/__init__.py
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)     6004 2023-04-28 14:46:44.000000 whisper_voice_commands-0.0.3/whisper_mic/cli.py
--rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)       85 2023-04-28 14:46:44.000000 whisper_voice_commands-0.0.3/whisper_mic/mic.py
-drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 14:47:37.183886 whisper_voice_commands-0.0.3/whisper_voice_commands.egg-info/
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3377 2023-04-28 14:47:37.000000 whisper_voice_commands-0.0.3/whisper_voice_commands.egg-info/PKG-INFO
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      372 2023-04-28 14:47:37.000000 whisper_voice_commands-0.0.3/whisper_voice_commands.egg-info/SOURCES.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)        1 2023-04-28 14:47:37.000000 whisper_voice_commands-0.0.3/whisper_voice_commands.egg-info/dependency_links.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       64 2023-04-28 14:47:37.000000 whisper_voice_commands-0.0.3/whisper_voice_commands.egg-info/entry_points.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      182 2023-04-28 14:47:37.000000 whisper_voice_commands-0.0.3/whisper_voice_commands.egg-info/requires.txt
--rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       12 2023-04-28 14:47:37.000000 whisper_voice_commands-0.0.3/whisper_voice_commands.egg-info/top_level.txt
+drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 15:10:16.747751 whisper_voice_commands-0.0.4/
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1070 2023-04-28 15:08:33.000000 whisper_voice_commands-0.0.4/LICENSE
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3693 2023-04-28 15:10:16.747751 whisper_voice_commands-0.0.4/PKG-INFO
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3116 2023-04-28 15:08:33.000000 whisper_voice_commands-0.0.4/README.md
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     1109 2023-04-28 15:09:33.000000 whisper_voice_commands-0.0.4/pyproject.toml
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       38 2023-04-28 15:10:16.747751 whisper_voice_commands-0.0.4/setup.cfg
+drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 15:10:16.744418 whisper_voice_commands-0.0.4/whisper_mic/
+-rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 15:08:33.000000 whisper_voice_commands-0.0.4/whisper_mic/__init__.py
+-rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)     6004 2023-04-28 15:08:33.000000 whisper_voice_commands-0.0.4/whisper_mic/cli.py
+-rwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)       85 2023-04-28 15:08:33.000000 whisper_voice_commands-0.0.4/whisper_mic/mic.py
+drwxr-xr-x   0 tinywizard  (1000) tinywizard  (1000)        0 2023-04-28 15:10:16.747751 whisper_voice_commands-0.0.4/whisper_voice_commands.egg-info/
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)     3693 2023-04-28 15:10:16.000000 whisper_voice_commands-0.0.4/whisper_voice_commands.egg-info/PKG-INFO
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      372 2023-04-28 15:10:16.000000 whisper_voice_commands-0.0.4/whisper_voice_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)        1 2023-04-28 15:10:16.000000 whisper_voice_commands-0.0.4/whisper_voice_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       64 2023-04-28 15:10:16.000000 whisper_voice_commands-0.0.4/whisper_voice_commands.egg-info/entry_points.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)      182 2023-04-28 15:10:16.000000 whisper_voice_commands-0.0.4/whisper_voice_commands.egg-info/requires.txt
+-rw-r--r--   0 tinywizard  (1000) tinywizard  (1000)       12 2023-04-28 15:10:16.000000 whisper_voice_commands-0.0.4/whisper_voice_commands.egg-info/top_level.txt
```

### Comparing `whisper_voice_commands-0.0.3/LICENSE` & `whisper_voice_commands-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_voice_commands-0.0.3/PKG-INFO` & `whisper_voice_commands-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: whisper_voice_commands
-Version: 0.0.3
+Version: 0.0.4
 Summary: Execute scripts with Whisper for your microphone
 Author-email: Deven B-L <deven.boutin@gmail.com>, Blake Mallory <blakecmallory@gmail.com>
 Project-URL: Homepage, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands
 Project-URL: Bug Tracker, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Whisper Mic
-This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
+This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic to run scripts. This repo copies some of the README from original project.
 
 ## Video Tutorial
 
-See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
-
+See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY). This is a fork of [here](https://github.com/mallorbc/whisper_mic) the video may not be relevant
 ### Professional Assistance
 
-If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
+If are in need of paid professional help, that is available through this [email](mailto:deven.boutin@gmail.com)
 
 ## Setup
 
 Now a pip package!
 
 1. Create a venv of your choice.
-2. Run ```pip install whisper-mic```
+2. Run ```pip install whisper-voice-commands```
+
+## Example usage
+```
+whisper-voice-commands --model tiny --script_path ~youruser/scripts/ --english --ambient --dynamic_energy
+```
+Check ```whisper-voice-commands --help ``` for more details
 
 ## Available models and languages
 
 There are five model sizes, four with English-only versions, offering speed and accuracy tradeoffs. Below are the names of the available models and their approximate memory requirements and relative speed. 
 
 
 |  Size  | Parameters | English-only model | Multilingual model | Required VRAM | Relative speed |
@@ -43,21 +48,21 @@
 | medium |   769 M    |    `medium.en`     |      `medium`      |     ~5 GB     |      ~2x       |
 | large  |   1550 M   |        N/A         |      `large`       |    ~10 GB     |       1x       |
 
 For English-only applications, the `.en` models tend to perform better, especially for the `tiny.en` and `base.en` models. We observed that the difference becomes less significant for the `small.en` and `medium.en` models.
 
 ## Microphone Demo
 
-You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
+You can use the model with a microphone using the ```whisper-voice-commands``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
 ## Troubleshooting
 
-If you are having issues with the ```mic.py``` not running try the following:
+If you are having issues with the ```cli.py``` not running try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
 ## Contributing
 
 Currently, this is just a cli demo.  I forsee that this pip package could become more than that for example:
```

### Comparing `whisper_voice_commands-0.0.3/README.md` & `whisper_voice_commands-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # Whisper Mic
-This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
+This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic to run scripts. This repo copies some of the README from original project.
 
 ## Video Tutorial
 
-See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
-
+See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY). This is a fork of [here](https://github.com/mallorbc/whisper_mic) the video may not be relevant
 ### Professional Assistance
 
-If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
+If are in need of paid professional help, that is available through this [email](mailto:deven.boutin@gmail.com)
 
 ## Setup
 
 Now a pip package!
 
 1. Create a venv of your choice.
-2. Run ```pip install whisper-mic```
+2. Run ```pip install whisper-voice-commands```
+
+## Example usage
+```
+whisper-voice-commands --model tiny --script_path ~youruser/scripts/ --english --ambient --dynamic_energy
+```
+Check ```whisper-voice-commands --help ``` for more details
 
 ## Available models and languages
 
 There are five model sizes, four with English-only versions, offering speed and accuracy tradeoffs. Below are the names of the available models and their approximate memory requirements and relative speed. 
 
 
 |  Size  | Parameters | English-only model | Multilingual model | Required VRAM | Relative speed |
@@ -29,21 +34,21 @@
 | medium |   769 M    |    `medium.en`     |      `medium`      |     ~5 GB     |      ~2x       |
 | large  |   1550 M   |        N/A         |      `large`       |    ~10 GB     |       1x       |
 
 For English-only applications, the `.en` models tend to perform better, especially for the `tiny.en` and `base.en` models. We observed that the difference becomes less significant for the `small.en` and `medium.en` models.
 
 ## Microphone Demo
 
-You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
+You can use the model with a microphone using the ```whisper-voice-commands``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
 ## Troubleshooting
 
-If you are having issues with the ```mic.py``` not running try the following:
+If you are having issues with the ```cli.py``` not running try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
 ## Contributing
 
 Currently, this is just a cli demo.  I forsee that this pip package could become more than that for example:
```

### Comparing `whisper_voice_commands-0.0.3/pyproject.toml` & `whisper_voice_commands-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whisper_voice_commands"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Deven B-L", email="deven.boutin@gmail.com" },
   { name="Blake Mallory", email="blakecmallory@gmail.com" },
 ]
 description = "Execute scripts with Whisper for your microphone"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `whisper_voice_commands-0.0.3/whisper_mic/cli.py` & `whisper_voice_commands-0.0.4/whisper_mic/cli.py`

 * *Files identical despite different names*

### Comparing `whisper_voice_commands-0.0.3/whisper_voice_commands.egg-info/PKG-INFO` & `whisper_voice_commands-0.0.4/whisper_voice_commands.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: whisper-voice-commands
-Version: 0.0.3
+Version: 0.0.4
 Summary: Execute scripts with Whisper for your microphone
 Author-email: Deven B-L <deven.boutin@gmail.com>, Blake Mallory <blakecmallory@gmail.com>
 Project-URL: Homepage, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands
 Project-URL: Bug Tracker, https://github.com/DevenBL/whisper_mic_exec/tree/Whisper-Voice-Commands/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Whisper Mic
-This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
+This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic to run scripts. This repo copies some of the README from original project.
 
 ## Video Tutorial
 
-See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
-
+See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY). This is a fork of [here](https://github.com/mallorbc/whisper_mic) the video may not be relevant
 ### Professional Assistance
 
-If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
+If are in need of paid professional help, that is available through this [email](mailto:deven.boutin@gmail.com)
 
 ## Setup
 
 Now a pip package!
 
 1. Create a venv of your choice.
-2. Run ```pip install whisper-mic```
+2. Run ```pip install whisper-voice-commands```
+
+## Example usage
+```
+whisper-voice-commands --model tiny --script_path ~youruser/scripts/ --english --ambient --dynamic_energy
+```
+Check ```whisper-voice-commands --help ``` for more details
 
 ## Available models and languages
 
 There are five model sizes, four with English-only versions, offering speed and accuracy tradeoffs. Below are the names of the available models and their approximate memory requirements and relative speed. 
 
 
 |  Size  | Parameters | English-only model | Multilingual model | Required VRAM | Relative speed |
@@ -43,21 +48,21 @@
 | medium |   769 M    |    `medium.en`     |      `medium`      |     ~5 GB     |      ~2x       |
 | large  |   1550 M   |        N/A         |      `large`       |    ~10 GB     |       1x       |
 
 For English-only applications, the `.en` models tend to perform better, especially for the `tiny.en` and `base.en` models. We observed that the difference becomes less significant for the `small.en` and `medium.en` models.
 
 ## Microphone Demo
 
-You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
+You can use the model with a microphone using the ```whisper-voice-commands``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
 ## Troubleshooting
 
-If you are having issues with the ```mic.py``` not running try the following:
+If you are having issues with the ```cli.py``` not running try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
 ## Contributing
 
 Currently, this is just a cli demo.  I forsee that this pip package could become more than that for example:
```

