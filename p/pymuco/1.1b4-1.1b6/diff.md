# Comparing `tmp/pymuco-1.1b4.tar.gz` & `tmp/pymuco-1.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymuco-1.1b4.tar", last modified: Fri Apr 28 09:36:49 2023, max compression
+gzip compressed data, was "pymuco-1.1b6.tar", last modified: Fri Apr 28 09:58:12 2023, max compression
```

## Comparing `pymuco-1.1b4.tar` & `pymuco-1.1b6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:36:49.585950 pymuco-1.1b4/
--rw-r--r--   0 germanmargon   (501) staff       (20)     1506 2023-04-24 21:32:50.000000 pymuco-1.1b4/LICENSE
--rw-r--r--   0 germanmargon   (501) staff       (20)     3265 2023-04-28 09:36:49.585569 pymuco-1.1b4/PKG-INFO
--rw-r--r--   0 germanmargon   (501) staff       (20)     2348 2023-04-28 09:02:22.000000 pymuco-1.1b4/README.md
-drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:36:49.583406 pymuco-1.1b4/pymuco/
--rw-r--r--   0 germanmargon   (501) staff       (20)    17141 2023-04-26 09:23:37.000000 pymuco-1.1b4/pymuco/AudioConverter.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     7956 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/Chord.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     7420 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/CircleOfFifths.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     5230 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/Enharmonic.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     4087 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/EnharmonicMapping.py
--rw-r--r--   0 germanmargon   (501) staff       (20)    17548 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/Interval.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     8558 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/KeySignature.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     5690 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/MIDIUtils.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     3167 2023-04-26 09:23:37.000000 pymuco-1.1b4/pymuco/MusicComputationNotation.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     2886 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/MusicData.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     7514 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/NoteDuration.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     3600 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/NoteFrequencyConverter.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     8081 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/NoteMapping.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     2903 2023-04-26 09:23:37.000000 pymuco-1.1b4/pymuco/Player.py
--rw-r--r--   0 germanmargon   (501) staff       (20)    12792 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/Scale.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     7438 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/ScientificPitchNotation.py
--rw-r--r--   0 germanmargon   (501) staff       (20)      764 2023-04-26 09:18:37.000000 pymuco-1.1b4/pymuco/Tonality.py
--rw-r--r--   0 germanmargon   (501) staff       (20)        0 2023-04-24 21:32:50.000000 pymuco-1.1b4/pymuco/__init__ .py
-drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:36:49.585000 pymuco-1.1b4/pymuco.egg-info/
--rw-r--r--   0 germanmargon   (501) staff       (20)     3265 2023-04-28 09:36:49.000000 pymuco-1.1b4/pymuco.egg-info/PKG-INFO
--rw-r--r--   0 germanmargon   (501) staff       (20)      562 2023-04-28 09:36:49.000000 pymuco-1.1b4/pymuco.egg-info/SOURCES.txt
--rw-r--r--   0 germanmargon   (501) staff       (20)        1 2023-04-28 09:36:49.000000 pymuco-1.1b4/pymuco.egg-info/dependency_links.txt
--rw-r--r--   0 germanmargon   (501) staff       (20)        7 2023-04-28 09:36:49.000000 pymuco-1.1b4/pymuco.egg-info/top_level.txt
--rw-r--r--   0 germanmargon   (501) staff       (20)       38 2023-04-28 09:36:49.586038 pymuco-1.1b4/setup.cfg
--rw-r--r--   0 germanmargon   (501) staff       (20)     1128 2023-04-28 09:35:28.000000 pymuco-1.1b4/setup.py
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:58:12.669893 pymuco-1.1b6/
+-rw-r--r--   0 germanmargon   (501) staff       (20)     1506 2023-04-24 21:32:50.000000 pymuco-1.1b6/LICENSE
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3275 2023-04-28 09:58:12.669469 pymuco-1.1b6/PKG-INFO
+-rw-r--r--   0 germanmargon   (501) staff       (20)     2358 2023-04-28 09:54:47.000000 pymuco-1.1b6/README.md
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:58:12.667678 pymuco-1.1b6/pymuco/
+-rw-r--r--   0 germanmargon   (501) staff       (20)    17141 2023-04-26 09:23:37.000000 pymuco-1.1b6/pymuco/AudioConverter.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7956 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/Chord.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7420 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/CircleOfFifths.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     5230 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/Enharmonic.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     4087 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/EnharmonicMapping.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)    17548 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/Interval.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     8558 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/KeySignature.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     5690 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/MIDIUtils.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3167 2023-04-26 09:23:37.000000 pymuco-1.1b6/pymuco/MusicComputationNotation.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     2886 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/MusicData.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7514 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/NoteDuration.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3600 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/NoteFrequencyConverter.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     8081 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/NoteMapping.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     2903 2023-04-26 09:23:37.000000 pymuco-1.1b6/pymuco/Player.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)    12792 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/Scale.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7438 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/ScientificPitchNotation.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)      764 2023-04-26 09:18:37.000000 pymuco-1.1b6/pymuco/Tonality.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)        0 2023-04-24 21:32:50.000000 pymuco-1.1b6/pymuco/__init__ .py
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:58:12.669003 pymuco-1.1b6/pymuco.egg-info/
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3275 2023-04-28 09:58:12.000000 pymuco-1.1b6/pymuco.egg-info/PKG-INFO
+-rw-r--r--   0 germanmargon   (501) staff       (20)      562 2023-04-28 09:58:12.000000 pymuco-1.1b6/pymuco.egg-info/SOURCES.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)        1 2023-04-28 09:58:12.000000 pymuco-1.1b6/pymuco.egg-info/dependency_links.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)        7 2023-04-28 09:58:12.000000 pymuco-1.1b6/pymuco.egg-info/top_level.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)       38 2023-04-28 09:58:12.669986 pymuco-1.1b6/setup.cfg
+-rw-r--r--   0 germanmargon   (501) staff       (20)     1128 2023-04-28 09:57:52.000000 pymuco-1.1b6/setup.py
```

### Comparing `pymuco-1.1b4/LICENSE` & `pymuco-1.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/PKG-INFO` & `pymuco-1.1b6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymuco
-Version: 1.1b4
+Version: 1.1b6
 Summary: A Python Music Computation Library
 Home-page: https://www.pymuco.org/
 Author: German Margon
 Author-email: gmargon@pymuco.org
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
-<img src="https://github.com/pymuco/pymuco/blob/main/docs/_static/pymucologo.png" width="150%">
+<img src="https://raw.githubusercontent.com/pymuco/pymuco/main/docs/_static/pymucologo.png" width="150%">
 </h1>
 
 [![CI](https://github.com/pymuco/pymuco/actions/workflows/python-app.yml/badge.svg)](https://github.com/pymuco/pymuco/actions/workflows/python-app.yml)
 ![PyPI Downloads](https://img.shields.io/pypi/dm/pymuco?color=%2345aaf5&label=PyPi%20Downloads)
 ![Status](https://img.shields.io/pypi/status/pymuco?color=%2345aaf5)
```

### Comparing `pymuco-1.1b4/README.md` & `pymuco-1.1b6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">
-<img src="https://github.com/pymuco/pymuco/blob/main/docs/_static/pymucologo.png" width="150%">
+<img src="https://raw.githubusercontent.com/pymuco/pymuco/main/docs/_static/pymucologo.png" width="150%">
 </h1>
 
 [![CI](https://github.com/pymuco/pymuco/actions/workflows/python-app.yml/badge.svg)](https://github.com/pymuco/pymuco/actions/workflows/python-app.yml)
 ![PyPI Downloads](https://img.shields.io/pypi/dm/pymuco?color=%2345aaf5&label=PyPi%20Downloads)
 ![Status](https://img.shields.io/pypi/status/pymuco?color=%2345aaf5)
```

### Comparing `pymuco-1.1b4/pymuco/AudioConverter.py` & `pymuco-1.1b6/pymuco/AudioConverter.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/Chord.py` & `pymuco-1.1b6/pymuco/Chord.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/CircleOfFifths.py` & `pymuco-1.1b6/pymuco/CircleOfFifths.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/Enharmonic.py` & `pymuco-1.1b6/pymuco/Enharmonic.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/EnharmonicMapping.py` & `pymuco-1.1b6/pymuco/EnharmonicMapping.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/Interval.py` & `pymuco-1.1b6/pymuco/Interval.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/KeySignature.py` & `pymuco-1.1b6/pymuco/KeySignature.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/MIDIUtils.py` & `pymuco-1.1b6/pymuco/MIDIUtils.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/MusicComputationNotation.py` & `pymuco-1.1b6/pymuco/MusicComputationNotation.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/MusicData.py` & `pymuco-1.1b6/pymuco/MusicData.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/NoteDuration.py` & `pymuco-1.1b6/pymuco/NoteDuration.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/NoteFrequencyConverter.py` & `pymuco-1.1b6/pymuco/NoteFrequencyConverter.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/NoteMapping.py` & `pymuco-1.1b6/pymuco/NoteMapping.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/Player.py` & `pymuco-1.1b6/pymuco/Player.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/Scale.py` & `pymuco-1.1b6/pymuco/Scale.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/ScientificPitchNotation.py` & `pymuco-1.1b6/pymuco/ScientificPitchNotation.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco/Tonality.py` & `pymuco-1.1b6/pymuco/Tonality.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/pymuco.egg-info/PKG-INFO` & `pymuco-1.1b6/pymuco.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymuco
-Version: 1.1b4
+Version: 1.1b6
 Summary: A Python Music Computation Library
 Home-page: https://www.pymuco.org/
 Author: German Margon
 Author-email: gmargon@pymuco.org
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
-<img src="https://github.com/pymuco/pymuco/blob/main/docs/_static/pymucologo.png" width="150%">
+<img src="https://raw.githubusercontent.com/pymuco/pymuco/main/docs/_static/pymucologo.png" width="150%">
 </h1>
 
 [![CI](https://github.com/pymuco/pymuco/actions/workflows/python-app.yml/badge.svg)](https://github.com/pymuco/pymuco/actions/workflows/python-app.yml)
 ![PyPI Downloads](https://img.shields.io/pypi/dm/pymuco?color=%2345aaf5&label=PyPi%20Downloads)
 ![Status](https://img.shields.io/pypi/status/pymuco?color=%2345aaf5)
```

### Comparing `pymuco-1.1b4/pymuco.egg-info/SOURCES.txt` & `pymuco-1.1b6/pymuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b4/setup.py` & `pymuco-1.1b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pymuco",
     packages=["pymuco"],
-    version="1.1B4",
+    version="1.1B6",
     description="A Python Music Computation Library",
     author="German Margon",
     author_email="gmargon@pymuco.org",
     url="https://www.pymuco.org/",
     license="BSD-3-Clause",
     classifiers=[
         "Development Status :: 4 - Beta",
```

