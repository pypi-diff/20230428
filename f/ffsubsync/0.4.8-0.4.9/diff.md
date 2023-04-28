# Comparing `tmp/ffsubsync-0.4.8.tar.gz` & `tmp/ffsubsync-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffsubsync-0.4.8.tar", last modified: Wed Sep 23 03:20:14 2020, max compression
+gzip compressed data, was "dist/ffsubsync-0.4.9.tar", last modified: Sun Oct 11 19:22:05 2020, max compression
```

## Comparing `ffsubsync-0.4.8.tar` & `ffsubsync-0.4.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2020-09-23 03:20:14.000000 ffsubsync-0.4.8/
--rw-r--r--   0 smacke     (501) staff       (20)     4620 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/HISTORY.rst
--rw-r--r--   0 smacke     (501) staff       (20)       66 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/MANIFEST.in
--rw-r--r--   0 smacke     (501) staff       (20)     9937 2020-09-23 03:20:14.000000 ffsubsync-0.4.8/PKG-INFO
--rw-r--r--   0 smacke     (501) staff       (20)     7808 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/README.md
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2020-09-23 03:20:14.000000 ffsubsync-0.4.8/ffsubsync/
--rw-r--r--   0 smacke     (501) staff       (20)      599 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)      497 2020-09-23 03:20:14.000000 ffsubsync-0.4.8/ffsubsync/_version.py
--rw-r--r--   0 smacke     (501) staff       (20)     3238 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/aligners.py
--rw-r--r--   0 smacke     (501) staff       (20)     1054 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/constants.py
--rw-r--r--   0 smacke     (501) staff       (20)     2854 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/ffmpeg_utils.py
--rwxr-xr-x   0 smacke     (501) staff       (20)    17258 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/ffsubsync.py
--rwxr-xr-x   0 smacke     (501) staff       (20)     3540 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/ffsubsync_gui.py
--rw-r--r--   0 smacke     (501) staff       (20)     1040 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/file_utils.py
--rw-r--r--   0 smacke     (501) staff       (20)     4473 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/generic_subtitles.py
--rw-r--r--   0 smacke     (501) staff       (20)    12952 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/sklearn_shim.py
--rw-r--r--   0 smacke     (501) staff       (20)    12162 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/speech_transformers.py
--rw-r--r--   0 smacke     (501) staff       (20)      594 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/suboffset.py
--rwxr-xr-x   0 smacke     (501) staff       (20)     4176 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/subtitle_parser.py
--rw-r--r--   0 smacke     (501) staff       (20)     4594 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/subtitle_transformers.py
--rw-r--r--   0 smacke     (501) staff       (20)     1190 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/ffsubsync/version.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2020-09-23 03:20:14.000000 ffsubsync-0.4.8/ffsubsync.egg-info/
--rw-r--r--   0 smacke     (501) staff       (20)     9937 2020-09-23 03:20:13.000000 ffsubsync-0.4.8/ffsubsync.egg-info/PKG-INFO
--rw-r--r--   0 smacke     (501) staff       (20)      685 2020-09-23 03:20:13.000000 ffsubsync-0.4.8/ffsubsync.egg-info/SOURCES.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2020-09-23 03:20:13.000000 ffsubsync-0.4.8/ffsubsync.egg-info/dependency_links.txt
--rw-r--r--   0 smacke     (501) staff       (20)       92 2020-09-23 03:20:13.000000 ffsubsync-0.4.8/ffsubsync.egg-info/entry_points.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2020-09-23 03:20:13.000000 ffsubsync-0.4.8/ffsubsync.egg-info/not-zip-safe
--rw-r--r--   0 smacke     (501) staff       (20)      215 2020-09-23 03:20:13.000000 ffsubsync-0.4.8/ffsubsync.egg-info/requires.txt
--rw-r--r--   0 smacke     (501) staff       (20)       10 2020-09-23 03:20:13.000000 ffsubsync-0.4.8/ffsubsync.egg-info/top_level.txt
--rw-r--r--   0 smacke     (501) staff       (20)      414 2020-09-23 03:20:14.000000 ffsubsync-0.4.8/setup.cfg
--rw-r--r--   0 smacke     (501) staff       (20)     1939 2020-09-23 03:10:53.000000 ffsubsync-0.4.8/setup.py
--rw-r--r--   0 smacke     (501) staff       (20)    68611 2020-09-23 03:08:33.000000 ffsubsync-0.4.8/versioneer.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/
+-rw-r--r--   0 smacke     (501) staff       (20)     5147 2020-10-11 19:07:45.000000 ffsubsync-0.4.9/HISTORY.rst
+-rw-r--r--   0 smacke     (501) staff       (20)       66 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/MANIFEST.in
+-rw-r--r--   0 smacke     (501) staff       (20)     9937 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/PKG-INFO
+-rw-r--r--   0 smacke     (501) staff       (20)     7808 2020-09-23 03:20:18.000000 ffsubsync-0.4.9/README.md
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync/
+-rw-r--r--   0 smacke     (501) staff       (20)      599 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/ffsubsync/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)      497 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync/_version.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4816 2020-10-11 19:16:58.000000 ffsubsync-0.4.9/ffsubsync/aligners.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1053 2020-09-28 00:25:25.000000 ffsubsync-0.4.9/ffsubsync/constants.py
+-rw-r--r--   0 smacke     (501) staff       (20)     2854 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/ffsubsync/ffmpeg_utils.py
+-rwxr-xr-x   0 smacke     (501) staff       (20)    18424 2020-10-11 19:01:39.000000 ffsubsync-0.4.9/ffsubsync/ffsubsync.py
+-rwxr-xr-x   0 smacke     (501) staff       (20)     3540 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/ffsubsync/ffsubsync_gui.py
+-rw-r--r--   0 smacke     (501) staff       (20)      893 2020-10-11 19:01:39.000000 ffsubsync-0.4.9/ffsubsync/file_utils.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4473 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/ffsubsync/generic_subtitles.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1792 2020-10-11 19:12:52.000000 ffsubsync-0.4.9/ffsubsync/golden_section_search.py
+-rw-r--r--   0 smacke     (501) staff       (20)    12952 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/ffsubsync/sklearn_shim.py
+-rw-r--r--   0 smacke     (501) staff       (20)    12355 2020-09-27 23:57:49.000000 ffsubsync-0.4.9/ffsubsync/speech_transformers.py
+-rw-r--r--   0 smacke     (501) staff       (20)      594 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/ffsubsync/suboffset.py
+-rwxr-xr-x   0 smacke     (501) staff       (20)     4242 2020-10-11 19:07:45.000000 ffsubsync-0.4.9/ffsubsync/subtitle_parser.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4594 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/ffsubsync/subtitle_transformers.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1190 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/ffsubsync/version.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync.egg-info/
+-rw-r--r--   0 smacke     (501) staff       (20)     9937 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync.egg-info/PKG-INFO
+-rw-r--r--   0 smacke     (501) staff       (20)      720 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync.egg-info/SOURCES.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync.egg-info/dependency_links.txt
+-rw-r--r--   0 smacke     (501) staff       (20)       92 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync.egg-info/entry_points.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync.egg-info/not-zip-safe
+-rw-r--r--   0 smacke     (501) staff       (20)      215 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync.egg-info/requires.txt
+-rw-r--r--   0 smacke     (501) staff       (20)       10 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/ffsubsync.egg-info/top_level.txt
+-rw-r--r--   0 smacke     (501) staff       (20)      414 2020-10-11 19:22:05.000000 ffsubsync-0.4.9/setup.cfg
+-rw-r--r--   0 smacke     (501) staff       (20)     1939 2020-09-23 03:20:18.000000 ffsubsync-0.4.9/setup.py
+-rw-r--r--   0 smacke     (501) staff       (20)    68611 2020-09-23 03:08:33.000000 ffsubsync-0.4.9/versioneer.py
```

### Comparing `ffsubsync-0.4.8/HISTORY.rst` & `ffsubsync-0.4.9/HISTORY.rst`

 * *Files 17% similar despite different names*

```diff
@@ -157,7 +157,18 @@
 0.4.6 (2020-06-10)
 ------------------
 * Bugfix for writing subs to stdout;
 
 0.4.7 (2020-09-05)
 ------------------
 * Misc bugfixes and stability improvements;
+
+0.4.8 (2020-09-22)
+------------------
+* Use webrtcvad-wheels on Windows to eliminate dependency on compiler;
+
+0.4.9 (2020-10-11)
+------------------
+* Make default offset seconds 60 and enforce during alignment as opposed to throwing away alignments with > max_offset_seconds;
+* Add experimental section for using golden section search to find framerate ratio;
+* Restore ability to read stdin and write stdout after buggy permissions check;
+* Exceptions that occur during syncing were mistakenly suppressed; this is now fixed;
```

### Comparing `ffsubsync-0.4.8/PKG-INFO` & `ffsubsync-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffsubsync
-Version: 0.4.8
+Version: 0.4.9
 Summary: Language-agnostic synchronization of subtitles with video.
 Home-page: https://github.com/smacke/ffsubsync
 Author: Stephen Macke
 Author-email: stephen.macke@gmail.com
 License: MIT
 Description: FFsubsync
         =======
```

### Comparing `ffsubsync-0.4.8/README.md` & `ffsubsync-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync/__init__.py` & `ffsubsync-0.4.9/ffsubsync/__init__.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync/aligners.py` & `ffsubsync-0.4.9/ffsubsync/aligners.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,107 @@
 # -*- coding: utf-8 -*- 
 import logging
 import math
 
 import numpy as np
+
+from .constants import FRAMERATE_RATIOS
+from .golden_section_search import gss
 from .sklearn_shim import TransformerMixin
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 class FailedToFindAlignmentException(Exception):
     pass
 
 
 class FFTAligner(TransformerMixin):
-    def __init__(self):
+    def __init__(self, max_offset_samples=None):
+        self.max_offset_samples = max_offset_samples
         self.best_offset_ = None
         self.best_score_ = None
         self.get_score_ = False
 
+    def _zero_out_extreme_offsets(self, convolve, substring):
+        convolve = np.copy(convolve)
+        if self.max_offset_samples is None:
+            return convolve
+        offset_to_index = lambda offset: len(convolve) - 1 + offset - len(substring)
+        convolve[:offset_to_index(-self.max_offset_samples)] = convolve[offset_to_index(self.max_offset_samples):] = 0
+        return convolve
+
+    def _compute_argmax(self, convolve, substring):
+        best_idx = np.argmax(convolve)
+        self.best_offset_ = len(convolve) - 1 - best_idx - len(substring)
+        self.best_score_ = convolve[best_idx]
+
     def fit(self, refstring, substring, get_score=False):
         refstring, substring = [
             list(map(int, s))
             if isinstance(s, str) else s
             for s in [refstring, substring]
         ]
         refstring, substring = map(
             lambda s: 2 * np.array(s).astype(float) - 1, [refstring, substring])
         total_bits = math.log(len(substring) + len(refstring), 2)
         total_length = int(2 ** math.ceil(total_bits))
         extra_zeros = total_length - len(substring) - len(refstring)
         subft = np.fft.fft(np.append(np.zeros(extra_zeros + len(refstring)), substring))
         refft = np.fft.fft(np.flip(np.append(refstring, np.zeros(len(substring) + extra_zeros)), 0))
         convolve = np.real(np.fft.ifft(subft * refft))
-        best_idx = np.argmax(convolve)
-        self.best_offset_ = len(convolve) - 1 - best_idx - len(substring)
-        self.best_score_ = convolve[best_idx]
+        self._compute_argmax(self._zero_out_extreme_offsets(convolve, substring), substring)
+        if self.best_score_ == 0.:
+            self._compute_argmax(convolve, substring)
         self.get_score_ = get_score
         return self
 
     def transform(self, *_):
         if self.get_score_:
             return self.best_score_, self.best_offset_
         else:
             return self.best_offset_
 
 
 class MaxScoreAligner(TransformerMixin):
-    def __init__(self, base_aligner, sample_rate=None, max_offset_seconds=None):
+    def __init__(self, base_aligner, srtin=None, sample_rate=None, max_offset_seconds=None):
+        self.srtin = srtin
+        if sample_rate is None or max_offset_seconds is None:
+            self.max_offset_samples = None
+        else:
+            self.max_offset_samples = abs(int(max_offset_seconds * sample_rate))
         if isinstance(base_aligner, type):
-            self.base_aligner = base_aligner()
+            self.base_aligner = base_aligner(max_offset_samples=self.max_offset_samples)
         else:
             self.base_aligner = base_aligner
         self.max_offset_seconds = max_offset_seconds
-        if sample_rate is None or max_offset_seconds is None:
-            self.max_offset_samples = None
-        else:
-            self.max_offset_samples = abs(max_offset_seconds * sample_rate)
         self._scores = []
 
+    def fit_gss(self, refstring, subpipe_maker):
+        def opt_func(framerate_ratio, is_last_iter):
+            subpipe = subpipe_maker(framerate_ratio)
+            substring = subpipe.fit_transform(self.srtin)
+            score = self.base_aligner.fit_transform(refstring, substring, get_score=True)
+            logger.info('got score %.0f (offset %d) for ratio %.3f', score[0], score[1], framerate_ratio)
+            if is_last_iter:
+                self._scores.append((score, subpipe))
+            return -score[0]
+        gss(opt_func, 0.9, 1.1)
+        return self
+
     def fit(self, refstring, subpipes):
         if not isinstance(subpipes, list):
             subpipes = [subpipes]
         for subpipe in subpipes:
-            if hasattr(subpipe, 'transform'):
-                substring = subpipe.transform(None)
+            if callable(subpipe):
+                self.fit_gss(refstring, subpipe)
+                continue
+            elif hasattr(subpipe, 'transform'):
+                substring = subpipe.transform(self.srtin)
             else:
                 substring = subpipe
             self._scores.append((
                 self.base_aligner.fit_transform(
                     refstring, substring, get_score=True
                 ),
                 subpipe
@@ -80,8 +113,8 @@
         if self.max_offset_samples is not None:
             scores = list(filter(lambda s: abs(s[0][1]) <= self.max_offset_samples, scores))
         if len(scores) == 0:
             raise FailedToFindAlignmentException('Synchronization failed; consider passing '
                                                  '--max-offset-seconds with a number larger than '
                                                  '{}'.format(self.max_offset_seconds))
         (score, offset), subpipe = max(scores, key=lambda x: x[0][0])
-        return offset, subpipe
+        return (score, offset), subpipe
```

### Comparing `ffsubsync-0.4.8/ffsubsync/constants.py` & `ffsubsync-0.4.9/ffsubsync/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DEFAULT_FRAME_RATE = 48000
 DEFAULT_ENCODING = 'infer'
 DEFAULT_MAX_SUBTITLE_SECONDS = 10
 DEFAULT_START_SECONDS = 0
 DEFAULT_SCALE_FACTOR = 1
 DEFAULT_VAD = 'subs_then_webrtc'
-DEFAULT_MAX_OFFSET_SECONDS = 600
+DEFAULT_MAX_OFFSET_SECONDS = 60
 
 SUBTITLE_EXTENSIONS = ('srt', 'ass', 'ssa', 'sub')
 
 GITHUB_DEV_USER = 'smacke'
 PROJECT_NAME = 'FFsubsync'
 PROJECT_LICENSE = 'MIT'
 COPYRIGHT_YEAR = '2019'
```

### Comparing `ffsubsync-0.4.8/ffsubsync/ffmpeg_utils.py` & `ffsubsync-0.4.9/ffsubsync/ffmpeg_utils.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync/ffsubsync.py` & `ffsubsync-0.4.9/ffsubsync/ffsubsync.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,29 +73,42 @@
     finally:
         shutil.rmtree(tar_dir)
     return 0
 
 
 def try_sync(args, reference_pipe, srt_pipes, result):
     sync_was_successful = True
+    exc = None
     try:
-        logger.info('extracting speech segments from subtitles file %s...', args.srtin)
+        logger.info('extracting speech segments from %s...',
+                    'stdin' if args.srtin is None else 'subtitles file {}'.format(args.srtin))
         for srt_pipe in srt_pipes:
-            srt_pipe.fit(args.srtin)
+            if callable(srt_pipe):
+                continue
+            else:
+                srt_pipe.fit(args.srtin)
         logger.info('...done')
         logger.info('computing alignments...')
-        offset_samples, best_srt_pipe = MaxScoreAligner(
-            FFTAligner, SAMPLE_RATE, args.max_offset_seconds
-        ).fit_transform(
-            reference_pipe.transform(args.reference),
-            srt_pipes,
-        )
+        if args.skip_sync:
+            best_score = 0.
+            best_srt_pipe = srt_pipes[0]
+            if callable(best_srt_pipe):
+                best_srt_pipe = best_srt_pipe(1.0).fit(args.srtin)
+            offset_samples = 0
+        else:
+            (best_score, offset_samples), best_srt_pipe = MaxScoreAligner(
+                FFTAligner, args.srtin, SAMPLE_RATE, args.max_offset_seconds
+            ).fit_transform(
+                reference_pipe.transform(args.reference),
+                srt_pipes,
+            )
         logger.info('...done')
         offset_seconds = offset_samples / float(SAMPLE_RATE)
         scale_step = best_srt_pipe.named_steps['scale']
+        logger.info('score: %.3f', best_score)
         logger.info('offset seconds: %.3f', offset_seconds)
         logger.info('framerate scale factor: %.3f', scale_step.scale_factor)
         output_steps = [('shift', SubtitleShifter(offset_seconds))]
         if args.merge_with_reference:
             output_steps.append(
                 ('merge',
                  SubtitleMerger(reference_pipe.named_steps['parse'].subs_))
@@ -105,18 +118,24 @@
         if args.output_encoding != 'same':
             out_subs = out_subs.set_encoding(args.output_encoding)
         logger.info('writing output to {}'.format(args.srtout or 'stdout'))
         out_subs.write_file(args.srtout)
     except FailedToFindAlignmentException as e:
         sync_was_successful = False
         logger.error(e)
+    except Exception as e:
+        exc = e
+        sync_was_successful = False
+        logger.error(e)
     else:
         result['offset_seconds'] = offset_seconds
         result['framerate_scale_factor'] = scale_step.scale_factor
     finally:
+        if exc is not None:
+            raise exc
         result['sync_was_successful'] = sync_was_successful
         return sync_was_successful
 
 
 def make_reference_pipe(args):
     ref_format = _ref_format(args.reference)
     if ref_format in SUBTITLE_EXTENSIONS:
@@ -154,18 +173,24 @@
         ])
 
 
 def make_srt_pipes(args):
     if args.no_fix_framerate:
         framerate_ratios = [1.]
     else:
-        framerate_ratios = np.concatenate([
+        framerate_ratios = list(np.concatenate([
             [1.], np.array(FRAMERATE_RATIOS), 1./np.array(FRAMERATE_RATIOS)
-        ])
-    parser = make_subtitle_parser(fmt=os.path.splitext(args.srtin)[-1][1:], caching=True, **args.__dict__)
+        ]))
+        if args.gss:
+            framerate_ratios.append(None)
+    if args.srtin is None:
+        srtin_format = 'srt'
+    else:
+        srtin_format = os.path.splitext(args.srtin)[-1][1:]
+    parser = make_subtitle_parser(fmt=srtin_format, caching=True, **args.__dict__)
     srt_pipes = [
         make_subtitle_speech_pipeline(
             **override(args, scale_factor=scale_factor, parser=parser)
         )
         for scale_factor in framerate_ratios
     ]
     return srt_pipes
@@ -222,20 +247,21 @@
         if args.make_test_case:
             raise ValueError('test case is for sync and not subtitle extraction')
         if args.srtin is not None:
             raise ValueError('stream specified for reference subtitle extraction; -i flag for sync input not allowed')
 
 
 def validate_file_permissions(args):
+    error_string_template = 'unable to {action} {file}; try ensuring file exists and has correct permissions'
     if not os.access(args.reference, os.R_OK):
-        raise ValueError('unable to read reference %s (try checking permissions)' % args.reference)
-    if not os.access(args.srtin, os.R_OK):
-        raise ValueError('unable to read input subtitles %s (try checking permissions)' % args.srtin)
-    if os.path.exists(args.srtout) and not os.access(args.srtout, os.W_OK):
-        raise ValueError('unable to write output subtitles %s (try checking permissions)' % args.srtout)
+        raise ValueError(error_string_template.format(action='read reference', file=args.reference))
+    if args.srtin is not None and not os.access(args.srtin, os.R_OK):
+        raise ValueError(error_string_template.format(action='read input subtitles', file=args.srtin))
+    if args.srtout is not None and os.path.exists(args.srtout) and not os.access(args.srtout, os.W_OK):
+        raise ValueError(error_string_template.format(action='write output subtitles', file=args.srtout))
     if args.make_test_case or args.serialize_speech:
         npy_savename = os.path.splitext(args.reference)[0] + '.npz'
         if os.path.exists(npy_savename) and not os.access(npy_savename, os.W_OK):
             raise ValueError('unable to write test case file archive %s (try checking permissions)' % npy_savename)
 
 
 def run(args):
@@ -336,15 +362,15 @@
                              '(default=%s).' % DEFAULT_ENCODING)
     parser.add_argument('--max-subtitle-seconds', type=float, default=DEFAULT_MAX_SUBTITLE_SECONDS,
                         help='Maximum duration for a subtitle to appear on-screen '
                              '(default=%.3f seconds).' % DEFAULT_MAX_SUBTITLE_SECONDS)
     parser.add_argument('--start-seconds', type=int, default=DEFAULT_START_SECONDS,
                         help='Start time for processing '
                              '(default=%d seconds).' % DEFAULT_START_SECONDS)
-    parser.add_argument('--max-offset-seconds', type=int, default=DEFAULT_MAX_OFFSET_SECONDS,
+    parser.add_argument('--max-offset-seconds', type=float, default=DEFAULT_MAX_OFFSET_SECONDS,
                         help='The max allowed offset seconds for any subtitle segment '
                              '(default=%d seconds).' % DEFAULT_MAX_OFFSET_SECONDS)
     parser.add_argument('--frame-rate', type=int, default=DEFAULT_FRAME_RATE,
                         help='Frame rate for audio extraction (default=%d).' % DEFAULT_FRAME_RATE)
     parser.add_argument('--output-encoding', default='utf-8',
                         help='What encoding to use for writing output subtitles '
                              '(default=utf-8). Can indicate "same" to use same '
@@ -368,14 +394,16 @@
         '--ffmpeg-path', '--ffmpegpath', default=None,
         help='Where to look for ffmpeg and ffprobe. Uses the system PATH by default.'
     )
     parser.add_argument('--log-dir-path', default=None, help='Where to save ffsubsync.log file (must be an existing '
                         'directory).')
     parser.add_argument('--vlc-mode', action='store_true', help=argparse.SUPPRESS)
     parser.add_argument('--gui-mode', action='store_true', help=argparse.SUPPRESS)
+    parser.add_argument('--skip-sync', action='store_true', help=argparse.SUPPRESS)
+    parser.add_argument('--gss', action='store_true', help=argparse.SUPPRESS)
 
 
 def make_parser():
     parser = argparse.ArgumentParser(description='Synchronize subtitles with video.')
     add_main_args_for_cli(parser)
     add_cli_only_args(parser)
     return parser
```

### Comparing `ffsubsync-0.4.8/ffsubsync/ffsubsync_gui.py` & `ffsubsync-0.4.9/ffsubsync/ffsubsync_gui.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync/generic_subtitles.py` & `ffsubsync-0.4.9/ffsubsync/generic_subtitles.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync/sklearn_shim.py` & `ffsubsync-0.4.9/ffsubsync/sklearn_shim.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync/speech_transformers.py` & `ffsubsync-0.4.9/ffsubsync/speech_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,28 @@
             caching=caching,
             max_subtitle_seconds=max_subtitle_seconds,
             start_seconds=start_seconds
         )
     assert parser.encoding == encoding
     assert parser.max_subtitle_seconds == max_subtitle_seconds
     assert parser.start_seconds == start_seconds
-    return Pipeline([
-        ('parse', parser),
-        ('scale', SubtitleScaler(scale_factor)),
-        ('speech_extract', SubtitleSpeechTransformer(
-            sample_rate=SAMPLE_RATE,
-            start_seconds=start_seconds,
-            framerate_ratio=scale_factor,
-        ))
-    ])
+    def subpipe_maker(framerate_ratio):
+        return Pipeline([
+            ('parse', parser),
+            ('scale', SubtitleScaler(framerate_ratio)),
+            ('speech_extract', SubtitleSpeechTransformer(
+                sample_rate=SAMPLE_RATE,
+                start_seconds=start_seconds,
+                framerate_ratio=framerate_ratio,
+            ))
+        ])
+    if scale_factor is None:
+        return subpipe_maker
+    else:
+        return subpipe_maker(scale_factor)
 
 
 def _make_auditok_detector(sample_rate, frame_rate):
     try:
         from auditok import \
             BufferAudioSource, ADSFactory, AudioEnergyValidator, StreamTokenizer
     except ImportError as e:
```

### Comparing `ffsubsync-0.4.8/ffsubsync/suboffset.py` & `ffsubsync-0.4.9/ffsubsync/suboffset.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync/subtitle_parser.py` & `ffsubsync-0.4.9/ffsubsync/subtitle_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         self.fit_fname = None
         self.detected_encoding_ = None
         self.sub_skippers = []
         self.max_subtitle_seconds = max_subtitle_seconds
         self.start_seconds = start_seconds
 
     def fit(self, fname, *_):
-        if self.caching and self.fit_fname == fname:
+        if self.caching and self.fit_fname == ('<stdin>' if fname is None else fname):
             return self
         encodings_to_try = (self.encoding,)
         with open_file(fname, 'rb') as f:
             subs = f.read()
         if self.encoding == 'infer':
             encodings_to_try = (chardet.detect(subs)['encoding'],)
             self.detected_encoding_ = encodings_to_try[0]
@@ -98,15 +98,15 @@
                 self.subs_ = GenericSubtitlesFile(
                     _preprocess_subs(parsed_subs,
                                      max_subtitle_seconds=self.max_subtitle_seconds,
                                      start_seconds=self.start_seconds),
                     sub_format=self.sub_format,
                     encoding=encoding
                 )
-                self.fit_fname = fname
+                self.fit_fname = '<stdin>' if fname is None else fname
                 if len(encodings_to_try) > 1:
                     self.detected_encoding_ = encoding
                     logger.info('detected encoding: %s' % self.detected_encoding_)
                 return self
             except Exception as e:
                 exc = e
                 continue
```

### Comparing `ffsubsync-0.4.8/ffsubsync/subtitle_transformers.py` & `ffsubsync-0.4.9/ffsubsync/subtitle_transformers.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync/version.py` & `ffsubsync-0.4.9/ffsubsync/version.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/ffsubsync.egg-info/PKG-INFO` & `ffsubsync-0.4.9/ffsubsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffsubsync
-Version: 0.4.8
+Version: 0.4.9
 Summary: Language-agnostic synchronization of subtitles with video.
 Home-page: https://github.com/smacke/ffsubsync
 Author: Stephen Macke
 Author-email: stephen.macke@gmail.com
 License: MIT
 Description: FFsubsync
         =======
```

### Comparing `ffsubsync-0.4.8/ffsubsync.egg-info/SOURCES.txt` & `ffsubsync-0.4.9/ffsubsync.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ffsubsync/aligners.py
 ffsubsync/constants.py
 ffsubsync/ffmpeg_utils.py
 ffsubsync/ffsubsync.py
 ffsubsync/ffsubsync_gui.py
 ffsubsync/file_utils.py
 ffsubsync/generic_subtitles.py
+ffsubsync/golden_section_search.py
 ffsubsync/sklearn_shim.py
 ffsubsync/speech_transformers.py
 ffsubsync/suboffset.py
 ffsubsync/subtitle_parser.py
 ffsubsync/subtitle_transformers.py
 ffsubsync/version.py
 ffsubsync.egg-info/PKG-INFO
```

### Comparing `ffsubsync-0.4.8/setup.py` & `ffsubsync-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `ffsubsync-0.4.8/versioneer.py` & `ffsubsync-0.4.9/versioneer.py`

 * *Files identical despite different names*

