# Comparing `tmp/unitranscode-0.2.0.tar.gz` & `tmp/unitranscode-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitranscode-0.2.0.tar", last modified: Fri Apr 21 07:42:30 2023, max compression
+gzip compressed data, was "unitranscode-0.3.0.tar", last modified: Fri Apr 28 03:38:10 2023, max compression
```

## Comparing `unitranscode-0.2.0.tar` & `unitranscode-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 07:42:30.237139 unitranscode-0.2.0/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.2.0/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-04-21 07:42:30.237139 unitranscode-0.2.0/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.2.0/README.md
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-04-21 07:42:30.237139 unitranscode-0.2.0/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      716 2023-04-21 07:41:27.000000 unitranscode-0.2.0/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 07:42:30.237139 unitranscode-0.2.0/tests/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      672 2023-04-21 07:38:21.000000 unitranscode-0.2.0/tests/test_transcoder.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 07:42:30.237139 unitranscode-0.2.0/unitranscode/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.2.0/unitranscode/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3187 2022-12-31 23:03:38.000000 unitranscode-0.2.0/unitranscode/custom_types.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    22131 2023-04-21 07:36:48.000000 unitranscode-0.2.0/unitranscode/transcoder.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-01-01 01:28:30.000000 unitranscode-0.2.0/unitranscode/utils.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 07:42:30.237139 unitranscode-0.2.0/unitranscode.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/top_level.txt
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-28 03:38:10.667604 unitranscode-0.3.0/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.3.0/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-04-28 03:38:10.667604 unitranscode-0.3.0/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.3.0/README.md
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-04-28 03:38:10.667604 unitranscode-0.3.0/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-04-28 03:37:51.000000 unitranscode-0.3.0/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-28 03:38:10.663604 unitranscode-0.3.0/tests/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1138 2023-04-28 03:34:33.000000 unitranscode-0.3.0/tests/test_transcoder.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-28 03:38:10.663604 unitranscode-0.3.0/unitranscode/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.3.0/unitranscode/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.3.0/unitranscode/custom_types.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    24953 2023-04-28 03:34:41.000000 unitranscode-0.3.0/unitranscode/transcoder.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-01-01 01:28:30.000000 unitranscode-0.3.0/unitranscode/utils.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-28 03:38:10.663604 unitranscode-0.3.0/unitranscode.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/top_level.txt
```

### Comparing `unitranscode-0.2.0/LICENSE` & `unitranscode-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitranscode-0.2.0/PKG-INFO` & `unitranscode-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.2.0
+Version: 0.3.0
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
+License: UNKNOWN
 Keywords: unitranscode
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `unitranscode-0.2.0/README.md` & `unitranscode-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `unitranscode-0.2.0/setup.py` & `unitranscode-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup
 
+
 setup(
     name='unitranscode',
-    version='0.2.0',
+    version='0.3.0',
     description='Universal transcoding library',
     url='https://github.com/MatthewScholefield/unitranscode',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `unitranscode-0.2.0/tests/test_transcoder.py` & `unitranscode-0.3.0/tests/test_transcoder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from os.path import isfile
 from pathlib import Path
 
+import pytest
 
 from unitranscode.transcoder import Transcoder
 
 
 def test_edit(example_20s_wav_file: Path, temp_folder: Path):
     in_file = example_20s_wav_file
     transcoder = Transcoder()
@@ -13,11 +14,24 @@
 
     out_file = transcoder.edit(
         in_file, cuts, temp_folder.joinpath('output.wav')
     )
 
     assert isfile(out_file)
 
-    in_file_duration = transcoder.info(in_file).duration_s
     out_file_duration = transcoder.info(out_file).duration_s
     expected_duration = sum([end - start for start, end in cuts])
-    assert abs(expected_duration - out_file_duration) < 0.1 * in_file_duration
+    assert out_file_duration == pytest.approx(expected_duration, 0.1)
+
+
+def test_extract_cuts(example_20s_wav_file: Path, temp_folder: Path):
+    in_file = example_20s_wav_file
+    transcoder = Transcoder()
+
+    cuts = [(0.0, 1.0), (3.0, 4.5), (7.0, 10.0)]
+    out_files = transcoder.extract_cuts(
+        in_file, cuts, str(temp_folder.joinpath('out-%d.wav'))
+    )
+
+    assert transcoder.info(out_files[0]).duration_s == pytest.approx(1.0)
+    assert transcoder.info(out_files[1]).duration_s == pytest.approx(1.5)
+    assert transcoder.info(out_files[2]).duration_s == pytest.approx(3.0)
```

### Comparing `unitranscode-0.2.0/unitranscode/custom_types.py` & `unitranscode-0.3.0/unitranscode/custom_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,32 @@
         return 'UnitranscodeExecError(message={}, command={})'.format(
             self.message, self.command
         )
 
 
 class EncodingInfo(dict):
     @property
+    def sample_rate_maybe(self):
+        return (
+            self.audio_streams[0].get('sample_rate')
+            if self.audio_streams
+            else None
+        )
+
+    @property
     def video_streams(self):
-        return [i for i in self['streams'] if i['codec_type'] == 'video']
+        video_streams = [
+            i for i in self['streams'] if i['codec_type'] == 'video'
+        ]
+        # Remove strange 'video' format types like MJPEG
+        if len(video_streams) > 1:
+            video_streams = [
+                i for i in video_streams if i.get('avg_frame_rate') != '0/0'
+            ] or video_streams
+        return video_streams
 
     @property
     def audio_streams(self):
         return [i for i in self['streams'] if i['codec_type'] == 'audio']
 
     @property
     def video_stream_maybe(self):
```

### Comparing `unitranscode-0.2.0/unitranscode/transcoder.py` & `unitranscode-0.3.0/unitranscode/transcoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,22 +37,20 @@
     ):
         self.transcoder = transcoder
         self.input_files: Optional[List[str]] = None
         self.output_files: Optional[List[str]] = None
         self.cmd: Optional[list] = None
         self._proc: Optional[Popen] = None
         self.is_paused = False
+        self.cancelled = False
         self.pause_lock = Lock()
         self.stdout_chunks = []
         self.stderr_chunks = []
         self.future: Optional[Future] = None
 
-    def set_proc(self, value) -> Popen:
-        ...
-
     @property
     def pid(self):
         return self._proc.pid
 
     @property
     def proc(self) -> Optional[Popen]:
         return self._proc
@@ -83,14 +81,20 @@
 
     def resume(self, _with_lock=True):
         with self.pause_lock if _with_lock else nullcontext():
             self.is_paused = False
             if self._proc:
                 self.resume_pid(self.proc.pid)
 
+    def cancel(self):
+        with self.pause_lock:
+            self.cancelled = True
+            if self._proc:
+                self._proc.kill()
+
     @cached_property
     def input_files_info(self) -> List[EncodingInfo]:
         return [self.transcoder.info(i) for i in self.input_files]
 
     @property
     def stdout_str(self):
         return b''.join(self.stdout_chunks).decode()
@@ -154,15 +158,15 @@
         proc = op.proc = Popen(op.cmd, stdout=PIPE, stderr=PIPE)
         if on_progress:
             self._track_progress(on_progress, proc, op, duration_s)
         stdout, stderr = proc.communicate()
         op.stdout_chunks.append(stdout)
         op.stderr_chunks.append(stderr)
 
-        if proc.returncode == -9 and self._shutting_down:
+        if proc.returncode == -9 and (self._shutting_down or op.cancelled):
             raise CancelledError('Ffmpeg operation cancelled')
         if proc.returncode != 0:
             raise op.exec_error(proc.returncode)
         return op
 
     def chop(
         self,
@@ -257,14 +261,19 @@
         on_progress: ProgressHandler = None,
         op: FfmpegOperation = None,
     ):
         norm_info = {
             k: '0.0' if v in ['inf', '-inf'] else v
             for k, v in norm_info.items()
         }
+        in_file_info = self.info(in_file)
+        if not in_file_info.sample_rate_maybe and in_file_info.audio_streams:
+            logger.error(
+                'Unknown sample rate for audio file: {}', in_file_info
+            )
         self.ffmpeg(
             *['-i', in_file],
             *[
                 '-filter_complex',
                 (
                     f'[0:0]'
                     f'loudnorm=i={level}:lra=7.0:tp=-2.0:offset=0.29:'
@@ -279,16 +288,20 @@
             *['-map_metadata', '0'],
             *['-map_metadata:s:a:0', '0:s:a:0'],
             *['-map_chapters', '0'],
             *['-c:v', 'copy'],
             *['-map', '[norm0]'],
             *['-c:a:0', 'pcm_s16le'],
             *['-c:s', 'copy'],
+            *(
+                ['-ar', f'{in_file_info.sample_rate_maybe}']
+                * bool(in_file_info.sample_rate_maybe)
+            ),
             out_file,
-            duration_s=self.info(in_file).duration_s if on_progress else None,
+            duration_s=in_file_info.duration_s if on_progress else None,
             on_progress=on_progress,
             op=op,
         )
         return out_file
 
     def info(
         self, filename: str, count_frames=False, can_retry=True
@@ -388,15 +401,18 @@
             else self._handle_amix(args, infos, audio_indices)
         )
         if not did_mix and audio_index is not None:
             args.extend(['-map', f'{audio_index}:a'])
         video_indices = (
             [*range(len(infos))] if video_index is None else [video_index]
         )
-        duration_s = max(i.duration_s for i in infos)
+        try:
+            duration_s = max(i.duration_s for i in infos)
+        except UnitranscodeFormatError:
+            duration_s = None
         video_streams = [
             (i, infos[i].video_stream)
             for i in video_indices
             if len(infos[i].video_streams) > 0
         ]
         maybe_args = []
         output_ext = splitext(output)[-1].lower()
@@ -566,14 +582,86 @@
             output_file,
             duration_s=self.info(in_file).duration_s if on_progress else None,
             on_progress=on_progress,
             op=op,
         )
         return output_file
 
+    @staticmethod
+    def _format_duration(dur: float) -> str:
+        mins, secs = divmod(dur, 60.0)
+        hours, mins = divmod(dur, 60.0)
+        return f'{int(hours):02}:{int(mins):02}:{secs:.03}'
+
+    @staticmethod
+    def _chunks(arr, n):
+        for i in range(0, len(arr), n):
+            yield arr[i : i + n]
+
+    def extract_cuts(
+        self,
+        in_file: str,
+        cuts: List[Tuple[float, float]],
+        out_file_fmt='{in_base}-%d.{in_ext}',
+        on_progress: ProgressHandler = None,
+        batch_size=8,
+        op: FfmpegOperation = None,
+    ):
+        total = 0
+        out_files = []
+        for cuts_batch in self._chunks(cuts, batch_size):
+            out_files.extend(
+                self._extract_cuts_direct(
+                    in_file=in_file,
+                    cuts=cuts_batch,
+                    out_file_fmt=out_file_fmt,
+                    n_offset=total,
+                    on_progress=on_progress,
+                    op=op,
+                )
+            )
+            total += len(cuts_batch)
+        return out_files
+
+    def _extract_cuts_direct(
+        self,
+        in_file: str,
+        cuts: List[Tuple[float, float]],
+        out_file_fmt='{in_base}-%d.{in_ext}',
+        n_offset=0,
+        on_progress: ProgressHandler = None,
+        op: FfmpegOperation = None,
+    ):
+        op = op or self.op()
+        op.input_files = [in_file]
+        in_base, in_ext = splitext(in_file)
+        in_ext = in_ext.lstrip('.')
+        out_file_fmt = out_file_fmt.format(in_base=in_base, in_ext=in_ext)
+        args = [
+            *('-i', in_file),
+        ]
+        out_files = []
+        for clip_num, (clip_start, clip_end) in enumerate(cuts, n_offset):
+            out_file = out_file_fmt.replace('%d', str(clip_num))
+            args += [
+                *('-ss', str(clip_start)),
+                *('-to', str(clip_end)),
+                *('-reset_timestamps', '1'),
+                out_file,
+            ]
+            out_files += [out_file]
+        op.output_files = out_files
+        self.ffmpeg(
+            *args,
+            duration_s=self.info(in_file).duration_s,
+            on_progress=on_progress,
+            op=op,
+        )
+        return out_files
+
     def split(
         self,
         in_file: str,
         split_timestamps: Optional[List[float]],
         out_file_fmt='{in_base}-%d.{in_ext}',
         on_progress: ProgressHandler = None,
         op: FfmpegOperation = None,
```

### Comparing `unitranscode-0.2.0/unitranscode.egg-info/PKG-INFO` & `unitranscode-0.3.0/unitranscode.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.2.0
+Version: 0.3.0
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
+License: UNKNOWN
 Keywords: unitranscode
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
+
+UNKNOWN
+
```

