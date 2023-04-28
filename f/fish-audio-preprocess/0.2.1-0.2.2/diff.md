# Comparing `tmp/fish_audio_preprocess-0.2.1.tar.gz` & `tmp/fish_audio_preprocess-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_audio_preprocess-0.2.1.tar", max compression
+gzip compressed data, was "fish_audio_preprocess-0.2.2.tar", max compression
```

## Comparing `fish_audio_preprocess-0.2.1.tar` & `fish_audio_preprocess-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11344 2023-01-06 00:07:08.214784 fish_audio_preprocess-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2023-01-06 00:28:50.280789 fish_audio_preprocess-0.2.1/fish_audio_preprocess/__init__.py
--rw-r--r--   0        0        0      812 2023-04-07 15:48:03.774064 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/__main__.py
--rw-r--r--   0        0        0     2616 2023-04-07 15:48:03.654063 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/convert_to_wav.py
--rw-r--r--   0        0        0     3220 2023-02-15 00:17:07.529910 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/frequency.py
--rw-r--r--   0        0        0     3287 2023-02-15 00:02:34.687587 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/length.py
--rw-r--r--   0        0        0     3097 2023-04-07 15:48:03.650063 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/loudness_norm.py
--rw-r--r--   0        0        0     3213 2023-04-08 04:53:11.243059 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/resample.py
--rw-r--r--   0        0        0     4312 2023-04-07 15:48:03.674063 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/separate_audio.py
--rw-r--r--   0        0        0     3866 2023-04-07 15:48:03.658063 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/slice_audio.py
--rw-r--r--   0        0        0      638 2023-02-03 07:46:26.761161 fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/to_ipa.py
--rw-r--r--   0        0        0  9504952 2023-02-03 07:46:26.809162 fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/cedict_ts.u8
--rw-r--r--   0        0        0     1783 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/file.py
--rw-r--r--   0        0        0     1821 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/loudness_norm.py
--rw-r--r--   0        0        0     1438 2023-02-03 07:46:26.809162 fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/polyphonic.yaml
--rw-r--r--   0        0        0     4158 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/separate_audio.py
--rw-r--r--   0        0        0     3869 2023-02-21 19:58:52.805912 fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/slice_audio.py
--rw-r--r--   0        0        0     4476 2023-02-14 02:37:35.397657 fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/to_ipa.py
--rw-r--r--   0        0        0     1052 2023-04-08 04:53:24.835126 fish_audio_preprocess-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 fish_audio_preprocess-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-01-06 00:07:08.214784 fish_audio_preprocess-0.2.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-06 00:28:50.280789 fish_audio_preprocess-0.2.2/fish_audio_preprocess/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-28 19:10:25.457227 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/__main__.py
+-rw-r--r--   0        0        0     2616 2023-04-07 15:48:03.654063 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/convert_to_wav.py
+-rw-r--r--   0        0        0     3220 2023-02-15 00:17:07.529910 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/frequency.py
+-rw-r--r--   0        0        0     3287 2023-02-15 00:02:34.687587 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/length.py
+-rw-r--r--   0        0        0     3097 2023-04-07 15:48:03.650063 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/loudness_norm.py
+-rw-r--r--   0        0        0     3213 2023-04-08 04:53:11.243059 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/resample.py
+-rw-r--r--   0        0        0     4312 2023-04-07 15:48:03.674063 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/separate_audio.py
+-rw-r--r--   0        0        0     7504 2023-04-28 19:21:20.252481 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/slice_audio.py
+-rw-r--r--   0        0        0      638 2023-02-03 07:46:26.761161 fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/to_ipa.py
+-rw-r--r--   0        0        0  9504952 2023-02-03 07:46:26.809162 fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/cedict_ts.u8
+-rw-r--r--   0        0        0     1781 2023-04-28 18:53:19.184053 fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/file.py
+-rw-r--r--   0        0        0     1821 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/loudness_norm.py
+-rw-r--r--   0        0        0     1438 2023-02-03 07:46:26.809162 fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/polyphonic.yaml
+-rw-r--r--   0        0        0     4158 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/separate_audio.py
+-rw-r--r--   0        0        0     3869 2023-04-28 19:13:28.710139 fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/slice_audio.py
+-rw-r--r--   0        0        0     8619 2023-04-28 19:21:20.384482 fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/slice_audio_v2.py
+-rw-r--r--   0        0        0     4476 2023-02-14 02:37:35.397657 fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/to_ipa.py
+-rw-r--r--   0        0        0     1023 2023-04-28 19:21:26.936514 fish_audio_preprocess-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 fish_audio_preprocess-0.2.2/PKG-INFO
```

### Comparing `fish_audio_preprocess-0.2.1/LICENSE` & `fish_audio_preprocess-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/__main__.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .convert_to_wav import to_wav
 from .frequency import frequency
 from .length import length
 from .loudness_norm import loudness_norm
 from .resample import resample
 from .separate_audio import separate
-from .slice_audio import slice_audio
+from .slice_audio import slice_audio, slice_audio_v2
 from .to_ipa import to_ipa
 
 
 @click.group()
 @click.option("--debug/--no-debug", default=False)
 def cli(debug: bool):
     """An audio preprocessing CLI."""
@@ -26,14 +26,15 @@
 cli.add_command(length)
 cli.add_command(frequency)
 
 cli.add_command(to_wav)
 cli.add_command(separate)
 cli.add_command(loudness_norm)
 cli.add_command(slice_audio)
+cli.add_command(slice_audio_v2)
 cli.add_command(resample)
 
 cli.add_command(to_ipa)
 
 
 if __name__ == "__main__":
     to_wav()
```

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/convert_to_wav.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/convert_to_wav.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/frequency.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/frequency.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/length.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/length.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/loudness_norm.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/loudness_norm.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/resample.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/resample.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/separate_audio.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/separate_audio.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/slice_audio.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/slice_audio.py`

 * *Files 23% similar despite different names*

```diff
@@ -132,9 +132,136 @@
             assert i.exception() is None, i.exception()
 
     logger.info("Done!")
     logger.info(f"Total: {len(files)}, Skipped: {skipped}")
     logger.info(f"Output directory: {output_dir}")
 
 
+@click.command()
+@click.argument("input_dir", type=click.Path(exists=True, file_okay=False))
+@click.argument("output_dir", type=click.Path(exists=False, file_okay=False))
+@click.option("--recursive/--no-recursive", default=True, help="Search recursively")
+@click.option(
+    "--overwrite/--no-overwrite", default=False, help="Overwrite existing files"
+)
+@click.option(
+    "--clean/--no-clean", default=False, help="Clean output directory before processing"
+)
+@click.option(
+    "--num-workers",
+    help="Number of workers to use for processing, defaults to number of CPU cores",
+    default=os.cpu_count(),
+    show_default=True,
+    type=int,
+)
+@click.option(
+    "--min-duration",
+    help="Minimum duration of each slice",
+    default=5.0,
+    show_default=True,
+    type=float,
+)
+@click.option(
+    "--max-duration",
+    help="Maximum duration of each slice",
+    default=30.0,
+    show_default=True,
+    type=float,
+)
+@click.option(
+    "--min-silence-duration",
+    help="Minimum duration of each slice",
+    default=0.3,
+    show_default=True,
+    type=float,
+)
+@click.option(
+    "--top-db",
+    help="top_db of librosa.effects.split",
+    default=-40,
+    show_default=True,
+    type=int,
+)
+@click.option(
+    "--hop-length",
+    help="hop_length of librosa.effects.split",
+    default=10,
+    show_default=True,
+    type=int,
+)
+@click.option(
+    "--max-silence-kept",
+    help="Maximum duration of each slice",
+    default=0.5,
+    show_default=True,
+    type=float,
+)
+def slice_audio_v2(
+    input_dir: str,
+    output_dir: str,
+    recursive: bool,
+    overwrite: bool,
+    clean: bool,
+    num_workers: int,
+    min_duration: float,
+    max_duration: float,
+    min_silence_duration: float,
+    top_db: int,
+    hop_length: int,
+    max_silence_kept: float,
+):
+    """(OpenVPI version) Slice audio files into smaller chunks by silence."""
+
+    from fish_audio_preprocess.utils.slice_audio_v2 import slice_audio_file_v2
+
+    input_dir, output_dir = Path(input_dir), Path(output_dir)
+
+    if input_dir == output_dir and clean:
+        logger.error("You are trying to clean the input directory, aborting")
+        return
+
+    make_dirs(output_dir, clean)
+
+    files = list_files(input_dir, extensions=AUDIO_EXTENSIONS, recursive=recursive)
+    logger.info(f"Found {len(files)} files, processing...")
+
+    skipped = 0
+
+    with ProcessPoolExecutor(max_workers=num_workers) as executor:
+        tasks = []
+
+        for file in tqdm(files, desc="Preparing tasks"):
+            # Get relative path to input_dir
+            relative_path = file.relative_to(input_dir)
+            save_path = output_dir / relative_path.parent / relative_path.stem
+
+            if save_path.exists() and not overwrite:
+                skipped += 1
+                continue
+
+            if save_path.exists() is False:
+                save_path.mkdir(parents=True)
+
+            tasks.append(
+                executor.submit(
+                    slice_audio_file_v2,
+                    input_file=str(file),
+                    output_dir=save_path,
+                    min_duration=min_duration,
+                    max_duration=max_duration,
+                    min_silence_duration=min_silence_duration,
+                    top_db=top_db,
+                    hop_length=hop_length,
+                    max_silence_kept=max_silence_kept,
+                )
+            )
+
+        for i in tqdm(as_completed(tasks), total=len(tasks), desc="Processing"):
+            assert i.exception() is None, i.exception()
+
+    logger.info("Done!")
+    logger.info(f"Total: {len(files)}, Skipped: {skipped}")
+    logger.info(f"Output directory: {output_dir}")
+
+
 if __name__ == "__main__":
     slice_audio()
```

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/cli/to_ipa.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/cli/to_ipa.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/cedict_ts.u8` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/cedict_ts.u8`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/file.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     Returns:
         list: List of files.
     """
 
     if isinstance(path, str):
         path = Path(path)
 
-    files = path.glob("**/*") if recursive else path.glob("*")
+    files = path.rglob("*") if recursive else path.glob("*")
     files = [f for f in files if f.is_file()]
 
     if extensions is not None:
         files = [f for f in files if f.suffix in extensions]
 
     if sort:
         files = sorted(files)
```

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/loudness_norm.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/loudness_norm.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/polyphonic.yaml` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/polyphonic.yaml`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/separate_audio.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/separate_audio.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/slice_audio.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/slice_audio.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/fish_audio_preprocess/utils/to_ipa.py` & `fish_audio_preprocess-0.2.2/fish_audio_preprocess/utils/to_ipa.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.1/pyproject.toml` & `fish_audio_preprocess-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 [tool.poetry]
 name = "fish-audio-preprocess"
-version = "0.2.1"
+version = "0.2.2"
 description = "Preprocess audio data"
 authors = ["Lengyue <lengyue@lengyue.me>"]
 license = "Apache"
 
 packages = [{ include = "fish_audio_preprocess" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 black = "^22.12.0"
 tqdm = "^4.64.1"
 demucs = "^4.0.0"
 loguru = "^0.6.0"
 pyloudnorm = "^0.1.1"
-transformers = "^4.25.1"
 PySoundFile = "^0.9.0"
 matplotlib = "^3.6.2"
 llvmlite = "^0.39.1"
 numba = "^0.56.4"
 librosa = "^0.9.0"
 richuru = "^0.1.1"
 praat-parselmouth = "^0.4.3"
-pyworld = { version = "^0.3.2", optional = true }
 g2pw = { version = "^0.1.1", optional = true }
 epitran = { version = "^1.24", optional = true }
+transformers = { version = "^4.25.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 isort = "^5.11.4"
 black = "^22.12.0"
 datasets = "^2.8.0"
 evaluate = "^0.4.0"
 
 [tool.poetry.extras]
-so-vits-svc = ["pyworld"]
-ipa = ["g2pw", "epitran"]
+ipa = ["g2pw", "epitran", "transformers"]
 
 [tool.poetry.scripts]
 fap = "fish_audio_preprocess.cli.__main__:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fish_audio_preprocess-0.2.1/PKG-INFO` & `fish_audio_preprocess-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: fish-audio-preprocess
-Version: 0.2.1
+Version: 0.2.2
 Summary: Preprocess audio data
 License: Apache
 Author: Lengyue
 Author-email: lengyue@lengyue.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ipa
-Provides-Extra: so-vits-svc
 Requires-Dist: PySoundFile (>=0.9.0,<0.10.0)
 Requires-Dist: black (>=22.12.0,<23.0.0)
 Requires-Dist: demucs (>=4.0.0,<5.0.0)
 Requires-Dist: epitran (>=1.24,<2.0) ; extra == "ipa"
 Requires-Dist: g2pw (>=0.1.1,<0.2.0) ; extra == "ipa"
 Requires-Dist: librosa (>=0.9.0,<0.10.0)
 Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: praat-parselmouth (>=0.4.3,<0.5.0)
 Requires-Dist: pyloudnorm (>=0.1.1,<0.2.0)
-Requires-Dist: pyworld (>=0.3.2,<0.4.0) ; extra == "so-vits-svc"
 Requires-Dist: richuru (>=0.1.1,<0.2.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: transformers (>=4.25.1,<5.0.0)
+Requires-Dist: transformers (>=4.25.1,<5.0.0) ; extra == "ipa"
```

