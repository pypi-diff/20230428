# Comparing `tmp/tts_arranger-0.3.0.tar.gz` & `tmp/tts_arranger-0.3.1.tar.gz`

## Comparing `tts_arranger-0.3.0.tar` & `tts_arranger-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/requirements.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_abstract_writer.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_html_converter.py
--rw-r--r--   0        0        0    24605 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_writer_example.py
--rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/checkers_default.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/exclude_ids.json
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/examples/tts_processor_example.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/examples/tts_writer_example.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/__init__.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/checker.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_abstract_reader.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_epub_reader.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_html_based_reader.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_html_reader.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_srt_reader.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_text_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/tests/reader_test.py
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/LICENSE
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/requirements.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_abstract_writer.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_html_converter.py
+-rw-r--r--   0        0        0    24605 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    17364 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/checkers_default.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/exclude_ids.json
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/examples/tts_project_example.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/examples/tts_simple_example.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/__init__.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/checker.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_abstract_reader.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_epub_reader.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_html_based_reader.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_html_reader.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_srt_reader.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_text_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/tests/reader_test.py
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/README.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/PKG-INFO
```

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_abstract_writer.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_abstract_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_html_converter.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_html_converter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_processor.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_processor.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_writer.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         :return: The duration of the audio file in nanoseconds.
         :rtype: int
         """
         result = ffmpeg.probe(filename, cmd='ffprobe', show_entries='format=duration')
         return int(float(result['format']['duration']) * self.NANOSECONDS_IN_ONE_SECOND)
 
-    def _synthesize_chapters(self, chapters: list[TTS_Chapter], temp_dir: str, tts_processor: TTS_Processor, callback: Optional[Callable[[float, TTS_Item], None]] = None, optimize=True, max_pause_duration=0, preprocess=True) -> None:
+    def _synthesize_chapters(self, chapters: list[TTS_Chapter], temp_dir: str, tts_processor: TTS_Processor, callback: Optional[Callable[[float, TTS_Item], None]] = None, optimize=False, max_pause_duration=0, preprocess=True) -> None:
         """
         Private method for synthesizing chapters into audio.
 
         :param chapters: A list of TTS chapters containing text to be synthesized into audio.
         :type chapters: list[TTS_Chapter]
 
         :param temp_dir: Path to the temporary directory.
@@ -88,15 +88,15 @@
 
         :param tts_arranger: ATTS_Arranger object to be used for synthesizing.
         :type tts_arranger: TTS_Arranger
 
         :param callback: An optional function that can be used to monitor the progress of the synthesis process.
         :type callback: Optional[Callable[[float, TTS_Item], None]]
 
-        :param optimize: Defines if the chapter should be optimized before synthesizing.
+        :param optimize: Defines if the chapter should be optimized (merging pauses and similar items) before synthesizing.
         :type optimize: boolean
 
         :param max_pause_duration: An optional maximum duration (in milliseconds) of silence to be inserted between adjacent TTS items in the output audio file. 
         :type max_pause_duration: int
 
         :param preprocess: Defines if the chapter should be preprocessed before synthesizing.
         :type preprocess: boolean
@@ -236,15 +236,15 @@
 
             (
                 ffmpeg
                 .output(audio, cover, output_file, vcodec='copy', acodec='copy', map_metadata=0, **{'disposition:v:0': 'attached_pic'}, loglevel='error')
                 .run(overwrite_output=True)
             )
 
-    def synthesize_and_write(self, project_filename: str, temp_dir_prefix: str = '', concat=True, callback: Optional[Callable[[float, TTS_Item], None]] = None, max_pause_duration=0) -> None:
+    def synthesize_and_write(self, project_filename: str, temp_dir_prefix: str = '', concat=True, callback: Optional[Callable[[float, TTS_Item], None]] = None, preprocess = True, optimize = False, max_pause_duration=0) -> None:
         """
         Synthesize and write the output audio files for the given project.
 
         :param project_filename: The name or path of the project file to be synthesized.
         :type project_filename: str
 
         :param temp_dir_prefix: An optional prefix for the temporary directory name used during synthesis.
@@ -283,15 +283,15 @@
                             self.model = 'tts_models/de/thorsten/tacotron2-DDC'
                             self.vocoder = 'vocoder_models/de/thorsten/hifigan_v1'
                         case _:
                             raise ValueError(f'Language code "{self.project.lang_code}" not supported')
 
                     t = TTS_Processor(self.model, self.vocoder, self.preferred_speakers)
 
-                self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback, not self.project.raw, max_pause_duration, not self.project.raw)
+                self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback, not self.project.raw and optimize, max_pause_duration, not self.project.raw and preprocess)
 
             except Exception as e:
                 log(LOG_TYPE.ERROR, f'Synthesizing project "{self.project.title}" failed: {e}.')
                 sys.exit(1)
 
             else:
                 if len(self.temp_files) > 0:
```

### Comparing `tts_arranger-0.3.0/src/tts_arranger/data/checkers_default.json` & `tts_arranger-0.3.1/src/tts_arranger/data/checkers_default.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428572%*

 * *Differences: {"'check_entries'": "{insert: [(26, OrderedDict([('conditions', [OrderedDict([('name', 'Class'), "*

 * *                    "('arg', 'tr-caption')])]), ('properties', OrderedDict([('speaker_idx', 1), "*

 * *                    "('pause_after', 1000)]))]))]}"}*

```diff
@@ -321,14 +321,26 @@
                 "pause_after": 1000,
                 "speaker_idx": 0
             }
         },
         {
             "conditions": [
                 {
+                    "arg": "tr-caption",
+                    "name": "Class"
+                }
+            ],
+            "properties": {
+                "pause_after": 1000,
+                "speaker_idx": 1
+            }
+        },
+        {
+            "conditions": [
+                {
                     "arg": "div",
                     "name": "Name"
                 }
             ],
             "properties": {
                 "pause_after": 750,
                 "speaker_idx": 0
```

### Comparing `tts_arranger-0.3.0/src/tts_arranger/examples/tts_processor_example.py` & `tts_arranger-0.3.1/src/tts_arranger/examples/tts_project_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,45 @@
 #!/usr/bin/python3
-from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
-                          TTS_Simple_Writer, TTS_Writer)
-
-# Simple example using Simple Writer (using a simple list of TTS items)
-
-tts_items = []
+from tts_arranger import TTS_Item, TTS_Chapter, TTS_Project, TTS_Writer
 
 preferred_speakers = ['p273', 'p330']
 
-tts_items.append(TTS_Item('This is a test', 1))
-tts_items.append(TTS_Item(length=2000))  # Insert pause
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 0, length=10000))
-
-simple_writer = TTS_Simple_Writer(tts_items, preferred_speakers)
-simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
-
-# English example using tts_models/en/vctk/vits (with multispeaker support)
+# Advanced example using a TTS Project object for creating an audiobook with chapters and a title image, uses tts_models/en/vctk/vits by (default)
 
 items1 = []
-items1.append(TTS_Item('This is a test:', 0))
-items1.append(TTS_Item('This is another test:', 1))
+items1.append(TTS_Item('This is a test', 0))
+items1.append(TTS_Item('This is another test by a different speaker', 1))
 
 items2 = []
 items2.append(TTS_Item('Another test',  0))
+items2.append(TTS_Item(length=1000))
 items2.append(TTS_Item('This is getting boring!', 1))
 
+# Prepare chapters with titles
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Chapter 1'))
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
+# Prepare the project file
 project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
+project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')  # Add a cover image
 
-# Add a cover image
-project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
-
+# Finally synthesize and write the project as a m4b audiobook using our preferred speakers
 writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', preferred_speakers=preferred_speakers)
 writer.synthesize_and_write(project.author + ' - ' + project.title)
 
-# German example using Thorsten voice (no multispeaker support)
+# German example using Thorsten voice (no multispeaker support), output as mp3, writing one mp3 file per chapter
 
 items1 = []
-items1.append(TTS_Item('Dies ist ein Test:', speaker_idx=0))
-items1.append(TTS_Item('Noch ein Test:',  speaker_idx=1))
+items1.append(TTS_Item('Dies ist ein Test.'))
+items1.append(TTS_Item('Noch ein Test.'))
 
 items2 = []
-items2.append(TTS_Item('Ein weiterer Test',  speaker_idx=0))
-items2.append(TTS_Item('Langsam wird es langweilig!',  speaker_idx=1))
+items2.append(TTS_Item('Ein weiterer Test'))
+items2.append(TTS_Item('Langsam wird es langweilig!'))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
 chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
 
 project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
```

### Comparing `tts_arranger-0.3.0/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.3.1/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.3.1/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.3.1/src/tts_arranger/items/tts_project.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_reader/checker.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_reader/checker.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_abstract_reader.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_abstract_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,11 +62,11 @@
         :return: None
         """
 
         path, full_name = os.path.split(output_filename)
         filename, extension = os.path.splitext(full_name)
 
         writer = TTS_Writer(self.project, path, self.output_format, preferred_speakers=self.preferred_speakers)
-        writer.synthesize_and_write(self.get_output_filename(), temp_dir_prefix, callback=callback, concat=False)
+        writer.synthesize_and_write(self.get_output_filename(), temp_dir_prefix, callback=callback, concat=False, optimize=True)
 
     def get_project(self) -> TTS_Project:
         return self.project
```

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_epub_reader.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_epub_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_html_based_reader.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_html_based_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_html_reader.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_html_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_srt_reader.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_srt_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,8 +68,8 @@
         self.project.raw = True
 
     def synthesize(self, output_filename: str, temp_dir_prefix='', callback: Optional[Callable[[float, TTS_Item], None]] = None) -> None:
         path, full_name = os.path.split(output_filename)
         filename, extension = os.path.splitext(full_name)
 
         writer = TTS_Simple_Writer(self.project.tts_chapters[0].tts_items, self.preferred_speakers)
-        writer.synthesize_and_write(output_filename + '.wav', lang_code=self.project.lang_code, callback=callback, preprocess=False)
+        writer.synthesize_and_write(output_filename + '.wav', lang_code=self.project.lang_code, callback=callback)
```

### Comparing `tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_text_reader.py` & `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_text_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/src/tts_arranger/utils/log.py` & `tts_arranger-0.3.1/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/tests/reader_test.py` & `tts_arranger-0.3.1/tests/reader_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/tests/tts_arranger_test.py` & `tts_arranger-0.3.1/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/LICENSE` & `tts_arranger-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.0/README.md` & `tts_arranger-0.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 # TTS Arranger
 
-A library that simplifies arranging text items fragments with multiple speakers and processing them using coqui.ai TTS to write audio files. 
+Library that simplifies arranging text items fragments with multiple speakers and processing them using coqui.ai TTS to write audio files. It also features helper classes for converting HTML (and thus EPUB files) into TTS projects, based of customizeable rules to read specific elements with different speakers, and define pauses after certain elements.
 
-# Examples
+## Overview
+
+### TTS project elements
+* TTS_Item, TTS_Chapter, TTS_Project
+
+### Writer Classes
+* TTS_Simple_Writer: Simple single-file writer, works with lists of TTS_Items directly
+* TTS_Writer: Designed for writing audiobooks with meta data and chapters, works on with TTS_Project
+
+### Reader Classes
+* TTS_Text_Reader: Reads and converts plain text into a TTS_Project instance 
+* TTS_HTML_Reader: Reads and converts HTML content into a TTS_Project instance
+* TTS_EPUB_Reader: Reads and converts an EPUB file into a TTS_Project instance
+* TTS_SRT_Reader: Reads and converts an SRT subtitle file into a TTS_Project instance *[not working due to timing bug at this point]*
+
+### Helper Classes
+* TTS_Processor: Takes a TTS_Item, synthesizes and writes it to a file, also takes care of preprocessing the text input and post processing the audio output
+* TTS_HTML_Converter: Parses HTML content into a TTS_Project (mainly used by TTS_HTML_Reader and TTS_EPUB_Reader)
+
+## Examples
 
 ```python
 from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
@@ -31,15 +50,15 @@
 items2.append(TTS_Item('Another test',  0))
 items2.append(TTS_Item('This is getting boring!', 1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Chapter 1'))
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
-project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
+project = TTS_Project(chapter, 'Project Title', 'Project Subtitle', author='Some Author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
 writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', preferred_speakers=preferred_speakers)
 writer.synthesize_and_write(project.author + ' - ' + project.title)
 
@@ -53,12 +72,12 @@
 items2.append(TTS_Item('Ein weiterer Test',  speaker_idx=0))
 items2.append(TTS_Item('Langsam wird es langweilig!',  speaker_idx=1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
 chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
 
-project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
+project = TTS_Project(chapter, 'Projektname', 'Projekt-Untertitel', author='Ein Autor', lang_code='de')
 
 writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
 writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
 ```
```

### Comparing `tts_arranger-0.3.0/pyproject.toml` & `tts_arranger-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,21 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.3.0"
+version = "0.3.1"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
   ".mypy_cache",
   ".vscode",
 ]
+
+[tool.hatch.metadata.hooks.requirements_txt]
+files = ["requirements.txt"]
```

### Comparing `tts_arranger-0.3.0/PKG-INFO` & `tts_arranger-0.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,56 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: beautifulsoup4>=4.12.2
+Requires-Dist: ebooklib>=0.18
+Requires-Dist: ffmpeg-python>=0.2.0
+Requires-Dist: num2words>=0.5.11
+Requires-Dist: pathvalidate>=2.5.2
+Requires-Dist: pillow>=9.5.0
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: requests>=2.28.2
+Requires-Dist: scipy>=1.9.0
+Requires-Dist: srt>=3.5.2
+Requires-Dist: tts>=0.13.3
 Description-Content-Type: text/markdown
 
 # TTS Arranger
 
-A library that simplifies arranging text items fragments with multiple speakers and processing them using coqui.ai TTS to write audio files. 
+Library that simplifies arranging text items fragments with multiple speakers and processing them using coqui.ai TTS to write audio files. It also features helper classes for converting HTML (and thus EPUB files) into TTS projects, based of customizeable rules to read specific elements with different speakers, and define pauses after certain elements.
 
-# Examples
+## Overview
+
+### TTS project elements
+* TTS_Item, TTS_Chapter, TTS_Project
+
+### Writer Classes
+* TTS_Simple_Writer: Simple single-file writer, works with lists of TTS_Items directly
+* TTS_Writer: Designed for writing audiobooks with meta data and chapters, works on with TTS_Project
+
+### Reader Classes
+* TTS_Text_Reader: Reads and converts plain text into a TTS_Project instance 
+* TTS_HTML_Reader: Reads and converts HTML content into a TTS_Project instance
+* TTS_EPUB_Reader: Reads and converts an EPUB file into a TTS_Project instance
+* TTS_SRT_Reader: Reads and converts an SRT subtitle file into a TTS_Project instance *[not working due to timing bug at this point]*
+
+### Helper Classes
+* TTS_Processor: Takes a TTS_Item, synthesizes and writes it to a file, also takes care of preprocessing the text input and post processing the audio output
+* TTS_HTML_Converter: Parses HTML content into a TTS_Project (mainly used by TTS_HTML_Reader and TTS_EPUB_Reader)
+
+## Examples
 
 ```python
 from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
@@ -45,15 +75,15 @@
 items2.append(TTS_Item('Another test',  0))
 items2.append(TTS_Item('This is getting boring!', 1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Chapter 1'))
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
-project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
+project = TTS_Project(chapter, 'Project Title', 'Project Subtitle', author='Some Author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
 writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', preferred_speakers=preferred_speakers)
 writer.synthesize_and_write(project.author + ' - ' + project.title)
 
@@ -67,12 +97,12 @@
 items2.append(TTS_Item('Ein weiterer Test',  speaker_idx=0))
 items2.append(TTS_Item('Langsam wird es langweilig!',  speaker_idx=1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
 chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
 
-project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
+project = TTS_Project(chapter, 'Projektname', 'Projekt-Untertitel', author='Ein Autor', lang_code='de')
 
 writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
 writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
 ```
```

