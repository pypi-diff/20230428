# Comparing `tmp/stable-ts-2.5.0.tar.gz` & `tmp/stable-ts-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.5.0.tar", last modified: Mon Apr 24 05:29:31 2023, max compression
+gzip compressed data, was "stable-ts-2.5.2.tar", last modified: Fri Apr 28 17:09:10 2023, max compression
```

## Comparing `stable-ts-2.5.0.tar` & `stable-ts-2.5.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 05:29:31.643210 stable-ts-2.5.0/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.5.0/LICENSE
--rw-rw-rw-   0        0        0     6890 2023-04-24 05:29:31.642207 stable-ts-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 05:29:31.643210 stable-ts-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 05:29:31.605197 stable-ts-2.5.0/stable_ts.egg-info/
--rw-rw-rw-   0        0        0     6890 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 05:29:31.640208 stable-ts-2.5.0/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.5.0/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.5.0/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-24 04:49:38.000000 stable-ts-2.5.0/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     6537 2023-04-19 18:39:07.000000 stable-ts-2.5.0/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.5.0/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.5.0/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    34855 2023-04-24 05:25:29.000000 stable-ts-2.5.0/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.5.0/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    14331 2023-04-18 21:08:14.000000 stable-ts-2.5.0/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.5.0/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.5.0/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    50175 2023-04-24 03:35:12.000000 stable-ts-2.5.0/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:09:10.134188 stable-ts-2.5.2/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.5.2/LICENSE
+-rw-rw-rw-   0        0        0     6890 2023-04-28 17:09:10.133186 stable-ts-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 17:09:10.134188 stable-ts-2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:09:10.076187 stable-ts-2.5.2/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0     6890 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 17:09:10.131186 stable-ts-2.5.2/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.5.2/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.5.2/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-04-28 17:07:38.000000 stable-ts-2.5.2/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.5.2/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.5.2/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.5.2/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.5.2/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    34855 2023-04-24 05:25:29.000000 stable-ts-2.5.2/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.5.2/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    14331 2023-04-18 21:08:14.000000 stable-ts-2.5.2/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.5.2/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.5.2/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    50492 2023-04-28 16:52:08.000000 stable-ts-2.5.2/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.5.0/LICENSE` & `stable-ts-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/PKG-INFO` & `stable-ts-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.5.0
+Version: 2.5.2
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.5.0/README.md` & `stable-ts-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/setup.py` & `stable-ts-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.5.2/stable_ts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.5.0
+Version: 2.5.2
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.5.0/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.5.2/stable_ts.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 stable_ts.egg-info/requires.txt
 stable_ts.egg-info/top_level.txt
 stable_whisper/__init__.py
 stable_whisper/__main__.py
 stable_whisper/_version.py
 stable_whisper/audio.py
 stable_whisper/decode.py
+stable_whisper/enhancement.py
 stable_whisper/quantization.py
 stable_whisper/result.py
 stable_whisper/stabilization.py
 stable_whisper/text_output.py
 stable_whisper/timing.py
 stable_whisper/video_output.py
 stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.5.0/stable_whisper/audio.py` & `stable-ts-2.5.2/stable_whisper/audio.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,53 +9,72 @@
 from whisper.audio import SAMPLE_RATE
 
 
 def is_ytdlp_available():
     return subprocess.run('yt-dlp -h', shell=True, capture_output=True).returncode == 0
 
 
-def _load_file(file: Union[str, bytes], verbose: bool = False):
+def _load_file(file: Union[str, bytes], verbose: bool = False, only_ffmpeg: bool = False):
     if isinstance(file, str) and '://' in file:
         if is_ytdlp_available():
             verbosity = ' -q' if verbose is None else (' --progress' if verbose else ' --progress -q')
             p = subprocess.run(
                 f'yt-dlp "{file}" -f ba/w -I 1{verbosity} -o -',
+                shell=True,
                 stdout=subprocess.PIPE
             )
             if len(p.stdout) == 0:
                 raise RuntimeError(f'Failed to download media from "{file}" with yt-dlp')
             return p.stdout
         else:
             warnings.warn('URL detected but yt-dlp not available. '
                           'To handle a greater variety of URLs (i.e. non-direct links), '
                           'install yt-dlp, \'pip install yt-dlp\' (repo: https://github.com/yt-dlp/yt-dlp).')
+        if not only_ffmpeg:
+            if is_ytdlp_available():
+                verbosity = ' -q' if verbose is None else (' --progress' if verbose else ' --progress -q')
+                p = subprocess.run(
+                    f'yt-dlp "{file}" -f ba/w -I 1{verbosity} -o -',
+                    shell=True,
+                    stdout=subprocess.PIPE
+                )
+                if p.returncode != 0 or len(p.stdout) == 0:
+                    raise RuntimeError(f'Failed to download media from "{file}" with yt-dlp')
+                return p.stdout
+            else:
+                warnings.warn('URL detected but yt-dlp not available. '
+                              'To handle a greater variety of URLs (i.e. non-direct links), '
+                              'install yt-dlp, \'pip install yt-dlp\' (repo: https://github.com/yt-dlp/yt-dlp).')
     return file
 
 
 # modified version of whisper.audio.load_audio
-def load_audio(file: Union[str, bytes], sr: int = SAMPLE_RATE, verbose: bool = True):
+def load_audio(file: Union[str, bytes], sr: int = SAMPLE_RATE, verbose: bool = True, only_ffmpeg: bool = False):
     """
     Open an audio file and read as mono waveform, resampling as necessary
 
     Parameters
     ----------
     file: str
         The audio file to open, bytes of file, or URL to audio/video
 
     sr: int
         The sample rate to resample the audio if necessary
 
     verbose: bool
         whether to print yt-dlp log
 
+    only_ffmpeg: bool
+        Whether to use only FFmpeg (and not yt-dlp) for URls. (Default: False)
+
     Returns
     -------
     A NumPy array containing the audio waveform, in float32 dtype.
     """
-    file = _load_file(file, verbose=verbose)
+    file = _load_file(file, verbose=verbose, only_ffmpeg=only_ffmpeg)
     if isinstance(file, bytes):
         inp, file = file, 'pipe:'
     else:
         inp = None
     try:
         # This launches a subprocess to decode audio while down-mixing and resampling as necessary.
         # Requires the ffmpeg CLI and `ffmpeg-python` package to be installed.
```

### Comparing `stable-ts-2.5.0/stable_whisper/decode.py` & `stable-ts-2.5.2/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/stable_whisper/quantization.py` & `stable-ts-2.5.2/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/stable_whisper/result.py` & `stable-ts-2.5.2/stable_whisper/result.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/stable_whisper/stabilization.py` & `stable-ts-2.5.2/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/stable_whisper/text_output.py` & `stable-ts-2.5.2/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/stable_whisper/timing.py` & `stable-ts-2.5.2/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/stable_whisper/video_output.py` & `stable-ts-2.5.2/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.0/stable_whisper/whisper_word_level.py` & `stable-ts-2.5.2/stable_whisper/whisper_word_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         only_voice_freq: bool = False,
         prepend_punctuations: str = "\"'“¿([{-",
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         mel_first: bool = False,
         split_callback: Callable = None,
         suppress_ts_tokens: bool = True,
         gap_padding: str = ' ...',
+        only_ffmpeg: bool = False,
         **decode_options) \
         -> WhisperResult:
     """
     Transcribe an audio file using Whisper
 
     Parameters
     ----------
@@ -187,14 +188,17 @@
         Reduces hallucinations in some cases,
             but also can reduce 'verbatimness' (i.e. ignores disfluencies and repetitions).
 
     gap_padding: str
         Padding prepend to each segments for word timing alignment. (Default: ' ...')
         Used to reduce the probability of model predicting timestamps earlier than the first utterance.
 
+    only_ffmpeg: bool
+        Whether to use only FFmpeg (and not yt-dlp) for URls. (Default: False)
+
     decode_options: dict
         Keyword arguments to construct `DecodingOptions` instances
 
     Returns
     -------
     A dictionary containing the resulting text ("text") and segment-level details ("segments"), and
     the spoken language ("language"), which is detected when `decode_options["language"]` is None.
@@ -225,15 +229,15 @@
             from .audio import demucs_audio
             audio = demucs_audio(audio,
                                  output_sr=curr_sr,
                                  device=device,
                                  verbose=verbose,
                                  save_path=demucs_output)
         else:
-            audio = torch.from_numpy(load_audio(audio, sr=curr_sr, verbose=verbose))
+            audio = torch.from_numpy(load_audio(audio, sr=curr_sr, verbose=verbose, only_ffmpeg=only_ffmpeg))
     else:
         if isinstance(audio, np.ndarray):
             audio = torch.from_numpy(audio)
         input_sr = decode_options.pop('input_sr', SAMPLE_RATE)
         if demucs:
             from .audio import demucs_audio
             audio = demucs_audio(audio,
@@ -829,14 +833,17 @@
     parser.add_argument("--no_speech_threshold", type=optional_float, default=0.6,
                         help="if the probability of the <|nospeech|> token is higher than this value AND the decoding "
                              "has failed due to `logprob_threshold`, consider the segment as silence")
     parser.add_argument("--threads", type=optional_int, default=0,
                         help="number of threads used by torch for CPU inference; "
                              "supercedes MKL_NUM_THREADS/OMP_NUM_THREADS")
 
+    parser.add_argument('--only_ffmpeg', action='store_true',
+                        help='whether to use only FFmpeg (and not yt-dlp) for URls')
+
     parser.add_argument('--overwrite', '-y', action='store_true',
                         help='overwrite all output files')
 
     parser.add_argument('--debug', action='store_true',
                         help='print all input/output pair(s) and all arguments used for transcribing/translating')
 
     args = parser.parse_args().__dict__
```

