# Comparing `tmp/pymuco-1.1b1.tar.gz` & `tmp/pymuco-1.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymuco-1.1b1.tar", last modified: Mon Apr 24 09:28:52 2023, max compression
+gzip compressed data, was "pymuco-1.1b3.tar", last modified: Fri Apr 28 09:12:39 2023, max compression
```

## Comparing `pymuco-1.1b1.tar` & `pymuco-1.1b3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-24 09:28:52.866638 pymuco-1.1b1/
--rw-r--r--   0 germanmargon   (501) staff       (20)     1505 2023-04-24 09:26:41.000000 pymuco-1.1b1/LICENSE
--rw-r--r--   0 germanmargon   (501) staff       (20)      875 2023-04-24 09:28:52.866215 pymuco-1.1b1/PKG-INFO
-drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-24 09:28:52.864103 pymuco-1.1b1/pymuco/
--rw-r--r--   0 germanmargon   (501) staff       (20)    17825 2023-04-20 07:51:40.000000 pymuco-1.1b1/pymuco/AudioConverter.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     7956 2023-04-20 07:33:57.000000 pymuco-1.1b1/pymuco/Chord.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     7420 2023-04-19 21:10:47.000000 pymuco-1.1b1/pymuco/CircleOfFifths.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     5230 2023-04-19 21:07:01.000000 pymuco-1.1b1/pymuco/Enharmonic.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     4087 2023-04-19 21:02:01.000000 pymuco-1.1b1/pymuco/EnharmonicMapping.py
--rw-r--r--   0 germanmargon   (501) staff       (20)    17548 2023-04-19 20:59:04.000000 pymuco-1.1b1/pymuco/Interval.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     8558 2023-04-19 20:46:05.000000 pymuco-1.1b1/pymuco/KeySignature.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     5690 2023-04-20 07:35:27.000000 pymuco-1.1b1/pymuco/MIDIUtils.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     3752 2023-04-19 20:36:53.000000 pymuco-1.1b1/pymuco/MusicComputationNotation.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     2886 2023-04-19 20:31:25.000000 pymuco-1.1b1/pymuco/MusicData.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     7514 2023-04-20 07:43:41.000000 pymuco-1.1b1/pymuco/NoteDuration.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     3600 2023-04-20 10:05:17.000000 pymuco-1.1b1/pymuco/NoteFrequencyConverter.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     8081 2023-04-20 11:34:01.000000 pymuco-1.1b1/pymuco/NoteMapping.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     3465 2023-04-20 11:34:09.000000 pymuco-1.1b1/pymuco/Player.py
--rw-r--r--   0 germanmargon   (501) staff       (20)    12792 2023-04-20 10:55:29.000000 pymuco-1.1b1/pymuco/Scale.py
--rw-r--r--   0 germanmargon   (501) staff       (20)     7438 2023-04-20 11:33:33.000000 pymuco-1.1b1/pymuco/ScientificPitchNotation.py
--rw-r--r--   0 germanmargon   (501) staff       (20)      764 2023-04-20 12:09:54.000000 pymuco-1.1b1/pymuco/Tonality.py
--rw-r--r--   0 germanmargon   (501) staff       (20)        0 2022-12-29 20:39:36.000000 pymuco-1.1b1/pymuco/__init__ .py
-drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-24 09:28:52.865733 pymuco-1.1b1/pymuco.egg-info/
--rw-r--r--   0 germanmargon   (501) staff       (20)      875 2023-04-24 09:28:52.000000 pymuco-1.1b1/pymuco.egg-info/PKG-INFO
--rw-r--r--   0 germanmargon   (501) staff       (20)      552 2023-04-24 09:28:52.000000 pymuco-1.1b1/pymuco.egg-info/SOURCES.txt
--rw-r--r--   0 germanmargon   (501) staff       (20)        1 2023-04-24 09:28:52.000000 pymuco-1.1b1/pymuco.egg-info/dependency_links.txt
--rw-r--r--   0 germanmargon   (501) staff       (20)        7 2023-04-24 09:28:52.000000 pymuco-1.1b1/pymuco.egg-info/top_level.txt
--rw-r--r--   0 germanmargon   (501) staff       (20)       38 2023-04-24 09:28:52.866730 pymuco-1.1b1/setup.cfg
--rw-r--r--   0 germanmargon   (501) staff       (20)      951 2023-04-22 20:58:24.000000 pymuco-1.1b1/setup.py
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:12:39.424369 pymuco-1.1b3/
+-rw-r--r--   0 germanmargon   (501) staff       (20)     1506 2023-04-24 21:32:50.000000 pymuco-1.1b3/LICENSE
+-rw-r--r--   0 germanmargon   (501) staff       (20)      875 2023-04-28 09:12:39.424098 pymuco-1.1b3/PKG-INFO
+-rw-r--r--   0 germanmargon   (501) staff       (20)     2348 2023-04-28 09:02:22.000000 pymuco-1.1b3/README.md
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:12:39.422311 pymuco-1.1b3/pymuco/
+-rw-r--r--   0 germanmargon   (501) staff       (20)    17141 2023-04-26 09:23:37.000000 pymuco-1.1b3/pymuco/AudioConverter.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7956 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/Chord.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7420 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/CircleOfFifths.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     5230 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/Enharmonic.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     4087 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/EnharmonicMapping.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)    17548 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/Interval.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     8558 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/KeySignature.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     5690 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/MIDIUtils.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3167 2023-04-26 09:23:37.000000 pymuco-1.1b3/pymuco/MusicComputationNotation.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     2886 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/MusicData.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7514 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/NoteDuration.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3600 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/NoteFrequencyConverter.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     8081 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/NoteMapping.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     2903 2023-04-26 09:23:37.000000 pymuco-1.1b3/pymuco/Player.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)    12792 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/Scale.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7438 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/ScientificPitchNotation.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)      764 2023-04-26 09:18:37.000000 pymuco-1.1b3/pymuco/Tonality.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)        0 2023-04-24 21:32:50.000000 pymuco-1.1b3/pymuco/__init__ .py
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-28 09:12:39.423634 pymuco-1.1b3/pymuco.egg-info/
+-rw-r--r--   0 germanmargon   (501) staff       (20)      875 2023-04-28 09:12:39.000000 pymuco-1.1b3/pymuco.egg-info/PKG-INFO
+-rw-r--r--   0 germanmargon   (501) staff       (20)      562 2023-04-28 09:12:39.000000 pymuco-1.1b3/pymuco.egg-info/SOURCES.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)        1 2023-04-28 09:12:39.000000 pymuco-1.1b3/pymuco.egg-info/dependency_links.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)        7 2023-04-28 09:12:39.000000 pymuco-1.1b3/pymuco.egg-info/top_level.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)       38 2023-04-28 09:12:39.424430 pymuco-1.1b3/setup.cfg
+-rw-r--r--   0 germanmargon   (501) staff       (20)      951 2023-04-28 09:10:13.000000 pymuco-1.1b3/setup.py
```

### Comparing `pymuco-1.1b1/LICENSE` & `pymuco-1.1b3/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pymuco-1.1b1/PKG-INFO` & `pymuco-1.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymuco
-Version: 1.1b1
+Version: 1.1b3
 Summary: A Python Music Computation Library
 Home-page: https://www.pymuco.org/
 Author: German Margon
 Author-email: gmargon@pymuco.org
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pymuco-1.1b1/pymuco/AudioConverter.py` & `pymuco-1.1b3/pymuco/AudioConverter.py`

 * *Files 6% similar despite different names*

```diff
@@ -477,34 +477,7 @@
             note_duration,
         ) in self._note_duration_mapping.get_note_duration():
             if note == duration or note_duration == duration:
                 if isinstance(duration, int):
                     return float(duration)
                 else:
                     return NoteDuration(duration).duration_length
-
-
-"""
-# Create a new MusicNotation object
-notation = MusicComputationNotation()
-
-# Create ScientificPitchNotation objects
-C4 = ScientificPitchNotation("C", 4)
-E4 = ScientificPitchNotation("E", 4)
-G4 = ScientificPitchNotation("G", 4)
-C5 = ScientificPitchNotation("C", 5)
-
-# Create NoteDuration objects
-whole_note = NoteDuration("WHOLE_NOTE")
-half_note = NoteDuration(0.5)
-
-notation.add_block(C4, whole_note, E4, whole_note,
-                   G4, whole_note, C5, whole_note)
-# notation.add_block(E4, whole_note)
-# notation.add_block(G4, whole_note)
-# notation.add_block(C5, whole_note)
-
-# print(notation.notation)
-
-audio = AudioConverter()
-audio.audio_converter(notation.notation)
-"""
```

### Comparing `pymuco-1.1b1/pymuco/Chord.py` & `pymuco-1.1b3/pymuco/Chord.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/CircleOfFifths.py` & `pymuco-1.1b3/pymuco/CircleOfFifths.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/Enharmonic.py` & `pymuco-1.1b3/pymuco/Enharmonic.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/EnharmonicMapping.py` & `pymuco-1.1b3/pymuco/EnharmonicMapping.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/Interval.py` & `pymuco-1.1b3/pymuco/Interval.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/KeySignature.py` & `pymuco-1.1b3/pymuco/KeySignature.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/MIDIUtils.py` & `pymuco-1.1b3/pymuco/MIDIUtils.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/MusicData.py` & `pymuco-1.1b3/pymuco/MusicData.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/NoteDuration.py` & `pymuco-1.1b3/pymuco/NoteDuration.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/NoteFrequencyConverter.py` & `pymuco-1.1b3/pymuco/NoteFrequencyConverter.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/NoteMapping.py` & `pymuco-1.1b3/pymuco/NoteMapping.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/Player.py` & `pymuco-1.1b3/pymuco/Player.py`

 * *Files 24% similar despite different names*

```diff
@@ -95,31 +95,7 @@
             print("Unsupported platform")
             return
 
         command = f'{player} "{sample._full_file_path}"'
 
         os.system(command)
         os.remove(sample._full_file_path)
-
-
-"""
-# Create a new MusicNotation object
-notation = MusicComputationNotation()
-
-# Create ScientificPitchNotation objects
-C4 = ScientificPitchNotation("C", 4)
-E4 = ScientificPitchNotation("E", 4)
-G4 = ScientificPitchNotation("G", 4)
-C5 = ScientificPitchNotation("C", 5)
-
-# Create NoteDuration objects
-whole_note = NoteDuration("WHOLE_NOTE")
-half_note = NoteDuration(0.5)
-
-notation.add_block(C4, whole_note, E4, whole_note,
-                   G4, whole_note, C5, whole_note)
-
-acorde = AudioConverter()
-acorde.convert_to_audio(notation)
-
-Player().play(acorde)
-"""
```

### Comparing `pymuco-1.1b1/pymuco/Scale.py` & `pymuco-1.1b3/pymuco/Scale.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/ScientificPitchNotation.py` & `pymuco-1.1b3/pymuco/ScientificPitchNotation.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco/Tonality.py` & `pymuco-1.1b3/pymuco/Tonality.py`

 * *Files identical despite different names*

### Comparing `pymuco-1.1b1/pymuco.egg-info/PKG-INFO` & `pymuco-1.1b3/pymuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymuco
-Version: 1.1b1
+Version: 1.1b3
 Summary: A Python Music Computation Library
 Home-page: https://www.pymuco.org/
 Author: German Margon
 Author-email: gmargon@pymuco.org
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pymuco-1.1b1/pymuco.egg-info/SOURCES.txt` & `pymuco-1.1b3/pymuco.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 setup.py
 pymuco/AudioConverter.py
 pymuco/Chord.py
 pymuco/CircleOfFifths.py
 pymuco/Enharmonic.py
 pymuco/EnharmonicMapping.py
 pymuco/Interval.py
```

### Comparing `pymuco-1.1b1/setup.py` & `pymuco-1.1b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name="pymuco",
     packages=["pymuco"],
-    version="1.1B1",
+    version="1.1B3",
     description="A Python Music Computation Library",
     author="German Margon",
     author_email="gmargon@pymuco.org",
     url="https://www.pymuco.org/",
     license="BSD-3-Clause",
     classifiers=[
         "Development Status :: 4 - Beta",
```

