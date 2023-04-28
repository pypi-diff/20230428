# Comparing `tmp/audioprocessor-0.1.1.tar.gz` & `tmp/audioprocessor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioprocessor-0.1.1.tar", last modified: Fri Apr 28 03:53:07 2023, max compression
+gzip compressed data, was "audioprocessor-0.1.2.tar", last modified: Fri Apr 28 17:59:48 2023, max compression
```

## Comparing `audioprocessor-0.1.1.tar` & `audioprocessor-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 03:53:07.340994 audioprocessor-0.1.1/
--rw-rw-rw-   0        0        0     3099 2023-04-28 03:53:07.339993 audioprocessor-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-28 03:53:07.338993 audioprocessor-0.1.1/audioprocessor.egg-info/
--rw-rw-rw-   0        0        0     3099 2023-04-28 03:53:07.000000 audioprocessor-0.1.1/audioprocessor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-28 03:53:07.000000 audioprocessor-0.1.1/audioprocessor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 03:53:07.000000 audioprocessor-0.1.1/audioprocessor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-28 03:53:07.000000 audioprocessor-0.1.1/audioprocessor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 03:53:07.000000 audioprocessor-0.1.1/audioprocessor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 03:53:07.340994 audioprocessor-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-04-28 03:52:27.000000 audioprocessor-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:59:48.103108 audioprocessor-0.1.2/
+-rw-rw-rw-   0        0        0     3099 2023-04-28 17:59:48.102108 audioprocessor-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-28 17:59:48.102108 audioprocessor-0.1.2/audioprocessor.egg-info/
+-rw-rw-rw-   0        0        0     3099 2023-04-28 17:59:48.000000 audioprocessor-0.1.2/audioprocessor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-04-28 17:59:48.000000 audioprocessor-0.1.2/audioprocessor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:59:48.000000 audioprocessor-0.1.2/audioprocessor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-28 17:59:48.000000 audioprocessor-0.1.2/audioprocessor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:59:48.000000 audioprocessor-0.1.2/audioprocessor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 17:59:48.103108 audioprocessor-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-04-28 17:59:42.000000 audioprocessor-0.1.2/setup.py
```

### Comparing `audioprocessor-0.1.1/PKG-INFO` & `audioprocessor-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioprocessor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for recording, transcribing, and converting audio
 Home-page: https://github.com/TheWordSmith123/Audio-Processor
 Author: Andrew Horvath
 Author-email: drewfhorvath@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `audioprocessor-0.1.1/audioprocessor.egg-info/PKG-INFO` & `audioprocessor-0.1.2/audioprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioprocessor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for recording, transcribing, and converting audio
 Home-page: https://github.com/TheWordSmith123/Audio-Processor
 Author: Andrew Horvath
 Author-email: drewfhorvath@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `audioprocessor-0.1.1/setup.py` & `audioprocessor-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="audioprocessor",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
-        "speech_recognition",
+        "speech_recognition>=3.10.0",
         "gtts",
         "pyaudio",
         "wave",
         "webrtcvad",
         "pydub",
     ],
     author="Andrew Horvath",
```

