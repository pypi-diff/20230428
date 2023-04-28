# Comparing `tmp/opensoundscape-0.8.0.tar.gz` & `tmp/opensoundscape-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensoundscape-0.8.0.tar", max compression
+gzip compressed data, was "opensoundscape-0.9.0.tar", max compression
```

## Comparing `opensoundscape-0.8.0.tar` & `opensoundscape-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,36 @@
--rw-r--r--   0        0        0     1081 2022-09-07 19:54:53.274476 opensoundscape-0.8.0/LICENSE
--rw-r--r--   0        0        0     4251 2023-01-12 21:39:23.828558 opensoundscape-0.8.0/README.md
--rw-r--r--   0        0        0       37 2022-12-19 23:38:55.202198 opensoundscape-0.8.0/opensoundscape/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-12-19 23:38:55.202391 opensoundscape-0.8.0/opensoundscape/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-12-19 23:38:55.201971 opensoundscape-0.8.0/opensoundscape/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2022-12-19 23:38:55.202593 opensoundscape-0.8.0/opensoundscape/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-12-19 23:38:55.202869 opensoundscape-0.8.0/opensoundscape/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      828 2023-01-12 21:39:24.060430 opensoundscape-0.8.0/opensoundscape/__init__.py
--rw-r--r--   0        0        0    25274 2023-01-12 21:39:24.080882 opensoundscape-0.8.0/opensoundscape/annotations.py
--rw-r--r--   0        0        0    44773 2023-01-12 21:39:24.090117 opensoundscape-0.8.0/opensoundscape/audio.py
--rw-r--r--   0        0        0     1735 2023-01-12 21:39:24.114509 opensoundscape-0.8.0/opensoundscape/audio_tools.py
--rw-r--r--   0        0        0     6727 2023-01-12 21:39:24.115205 opensoundscape-0.8.0/opensoundscape/audiomoth.py
--rw-r--r--   0        0        0     4121 2023-01-12 21:39:24.116084 opensoundscape-0.8.0/opensoundscape/data_selection.py
--rw-r--r--   0        0        0    11883 2023-01-12 21:39:24.116758 opensoundscape-0.8.0/opensoundscape/helpers.py
--rw-r--r--   0        0        0     8693 2023-01-12 21:39:24.117435 opensoundscape-0.8.0/opensoundscape/localization.py
--rw-r--r--   0        0        0     8174 2023-01-12 21:39:24.118080 opensoundscape-0.8.0/opensoundscape/metrics.py
--rw-r--r--   0        0        0      125 2022-09-07 19:54:53.425139 opensoundscape-0.8.0/opensoundscape/preprocess/__init__.py
--rw-r--r--   0        0        0      324 2022-09-09 22:08:25.205912 opensoundscape-0.8.0/opensoundscape/preprocess/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18811 2023-01-12 21:39:28.973455 opensoundscape-0.8.0/opensoundscape/preprocess/__pycache__/actions.cpython-39.pyc
--rw-r--r--   0        0        0      967 2023-01-12 21:39:28.997233 opensoundscape-0.8.0/opensoundscape/preprocess/__pycache__/img_augment.cpython-39.pyc
--rw-r--r--   0        0        0     9278 2023-01-12 21:39:29.001203 opensoundscape-0.8.0/opensoundscape/preprocess/__pycache__/preprocessors.cpython-39.pyc
--rw-r--r--   0        0        0     2887 2023-01-12 21:39:28.978766 opensoundscape-0.8.0/opensoundscape/preprocess/__pycache__/tensor_augment.cpython-39.pyc
--rw-r--r--   0        0        0     2877 2023-01-12 21:39:28.995966 opensoundscape-0.8.0/opensoundscape/preprocess/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0    24181 2023-01-12 21:39:24.118954 opensoundscape-0.8.0/opensoundscape/preprocess/actions.py
--rw-r--r--   0        0        0      730 2023-01-12 21:39:24.119511 opensoundscape-0.8.0/opensoundscape/preprocess/img_augment.py
--rw-r--r--   0        0        0    11862 2023-01-12 21:39:24.120904 opensoundscape-0.8.0/opensoundscape/preprocess/preprocessors.py
--rw-r--r--   0        0        0     2622 2023-01-12 21:39:24.122121 opensoundscape-0.8.0/opensoundscape/preprocess/tensor_augment.py
--rw-r--r--   0        0        0     2604 2023-01-12 21:39:24.123965 opensoundscape-0.8.0/opensoundscape/preprocess/utils.py
--rw-r--r--   0        0        0        0 2022-09-07 19:54:53.431876 opensoundscape-0.8.0/opensoundscape/resources/__init__.py
--rw-r--r--   0        0        0      156 2022-09-09 22:08:19.628141 opensoundscape-0.8.0/opensoundscape/resources/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    42432 2022-09-07 19:54:53.432206 opensoundscape-0.8.0/opensoundscape/resources/species_table.csv
--rw-r--r--   0        0        0     8819 2023-01-12 21:39:24.128880 opensoundscape-0.8.0/opensoundscape/ribbit.py
--rw-r--r--   0        0        0    17099 2023-01-12 21:39:24.129996 opensoundscape-0.8.0/opensoundscape/signal_processing.py
--rw-r--r--   0        0        0    32674 2023-01-12 21:39:24.132032 opensoundscape-0.8.0/opensoundscape/spectrogram.py
--rw-r--r--   0        0        0     1901 2023-01-12 21:39:24.135285 opensoundscape-0.8.0/opensoundscape/taxa.py
--rw-r--r--   0        0        0      141 2022-09-07 19:54:53.433551 opensoundscape-0.8.0/opensoundscape/torch/__init__.py
--rw-r--r--   0        0        0      343 2022-09-09 22:08:19.645167 opensoundscape-0.8.0/opensoundscape/torch/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6418 2023-01-12 21:39:29.008500 opensoundscape-0.8.0/opensoundscape/torch/__pycache__/datasets.cpython-39.pyc
--rw-r--r--   0        0        0     5258 2023-01-12 21:39:28.803216 opensoundscape-0.8.0/opensoundscape/torch/__pycache__/grad_cam.cpython-39.pyc
--rw-r--r--   0        0        0     5378 2023-01-12 21:39:28.806494 opensoundscape-0.8.0/opensoundscape/torch/__pycache__/loss.cpython-39.pyc
--rw-r--r--   0        0        0     6830 2023-01-12 21:39:28.812965 opensoundscape-0.8.0/opensoundscape/torch/__pycache__/safe_dataset.cpython-39.pyc
--rw-r--r--   0        0        0     4995 2023-01-12 21:39:28.815273 opensoundscape-0.8.0/opensoundscape/torch/__pycache__/sampling.cpython-39.pyc
--rw-r--r--   0        0        0       52 2023-01-12 21:39:24.138504 opensoundscape-0.8.0/opensoundscape/torch/architectures/__init__.py
--rw-r--r--   0        0        0      236 2023-01-12 21:39:28.822878 opensoundscape-0.8.0/opensoundscape/torch/architectures/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    20476 2023-01-12 21:39:28.842326 opensoundscape-0.8.0/opensoundscape/torch/architectures/__pycache__/cnn_architectures.cpython-39.pyc
--rw-r--r--   0        0        0     6993 2023-01-12 19:20:59.260692 opensoundscape-0.8.0/opensoundscape/torch/architectures/__pycache__/resnet.cpython-39.pyc
--rw-r--r--   0        0        0     1237 2023-01-12 21:39:28.938757 opensoundscape-0.8.0/opensoundscape/torch/architectures/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0    25987 2023-01-12 21:39:24.140879 opensoundscape-0.8.0/opensoundscape/torch/architectures/cnn_architectures.py
--rw-r--r--   0        0        0      564 2023-01-12 21:39:24.141449 opensoundscape-0.8.0/opensoundscape/torch/architectures/utils.py
--rw-r--r--   0        0        0     7315 2023-01-12 21:39:24.142017 opensoundscape-0.8.0/opensoundscape/torch/datasets.py
--rw-r--r--   0        0        0     4024 2023-01-12 21:39:24.142535 opensoundscape-0.8.0/opensoundscape/torch/grad_cam.py
--rw-r--r--   0        0        0     5970 2023-01-12 21:39:24.142977 opensoundscape-0.8.0/opensoundscape/torch/loss.py
--rw-r--r--   0        0        0       38 2022-09-07 19:54:53.436035 opensoundscape-0.8.0/opensoundscape/torch/models/__init__.py
--rw-r--r--   0        0        0      215 2022-09-09 22:08:25.186206 opensoundscape-0.8.0/opensoundscape/torch/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    34480 2023-01-12 21:39:28.956940 opensoundscape-0.8.0/opensoundscape/torch/models/__pycache__/cnn.cpython-39.pyc
--rw-r--r--   0        0        0     4147 2023-01-12 21:39:28.960348 opensoundscape-0.8.0/opensoundscape/torch/models/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0    55940 2023-01-12 21:39:24.143860 opensoundscape-0.8.0/opensoundscape/torch/models/cnn.py
--rw-r--r--   0        0        0     4246 2023-01-12 21:39:24.144502 opensoundscape-0.8.0/opensoundscape/torch/models/utils.py
--rw-r--r--   0        0        0     8248 2023-01-12 21:39:24.144907 opensoundscape-0.8.0/opensoundscape/torch/safe_dataset.py
--rw-r--r--   0        0        0     4319 2023-01-12 21:39:24.145508 opensoundscape-0.8.0/opensoundscape/torch/sampling.py
--rw-r--r--   0        0        0     4245 2023-01-12 21:39:24.145827 opensoundscape-0.8.0/opensoundscape/wandb.py
--rw-r--r--   0        0        0     1604 2023-01-12 21:39:24.148100 opensoundscape-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5974 1970-01-01 00:00:00.000000 opensoundscape-0.8.0/setup.py
--rw-r--r--   0        0        0     5690 1970-01-01 00:00:00.000000 opensoundscape-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-09-07 19:54:53.274476 opensoundscape-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4141 2023-04-28 16:25:08.326479 opensoundscape-0.9.0/README.md
+-rw-r--r--   0        0        0      835 2023-04-28 16:25:08.662321 opensoundscape-0.9.0/opensoundscape/__init__.py
+-rw-r--r--   0        0        0    30818 2023-04-28 16:25:08.663789 opensoundscape-0.9.0/opensoundscape/annotations.py
+-rw-r--r--   0        0        0     6740 2023-04-28 16:25:08.664111 opensoundscape-0.9.0/opensoundscape/aru.py
+-rw-r--r--   0        0        0    51145 2023-04-28 16:25:08.665360 opensoundscape-0.9.0/opensoundscape/audio.py
+-rw-r--r--   0        0        0     4121 2023-01-18 14:19:19.795886 opensoundscape-0.9.0/opensoundscape/data_selection.py
+-rw-r--r--   0        0        0    46865 2023-04-28 16:25:08.667564 opensoundscape-0.9.0/opensoundscape/localization.py
+-rw-r--r--   0        0        0     2755 2023-04-28 16:25:08.669350 opensoundscape-0.9.0/opensoundscape/logging.py
+-rw-r--r--   0        0        0     8174 2023-04-04 20:56:27.927318 opensoundscape-0.9.0/opensoundscape/metrics.py
+-rw-r--r--   0        0        0      180 2023-04-28 16:25:08.669653 opensoundscape-0.9.0/opensoundscape/ml/__init__.py
+-rw-r--r--   0        0        0     5759 2023-04-28 16:25:08.672220 opensoundscape-0.9.0/opensoundscape/ml/cam.py
+-rw-r--r--   0        0        0    74373 2023-04-28 16:25:08.674300 opensoundscape-0.9.0/opensoundscape/ml/cnn.py
+-rw-r--r--   0        0        0    28247 2023-04-28 16:25:08.675387 opensoundscape-0.9.0/opensoundscape/ml/cnn_architectures.py
+-rw-r--r--   0        0        0     6763 2023-04-28 16:25:08.676839 opensoundscape-0.9.0/opensoundscape/ml/datasets.py
+-rw-r--r--   0        0        0     5970 2023-04-28 16:25:08.681611 opensoundscape-0.9.0/opensoundscape/ml/loss.py
+-rw-r--r--   0        0        0     8248 2023-04-28 16:25:08.692391 opensoundscape-0.9.0/opensoundscape/ml/safe_dataset.py
+-rw-r--r--   0        0        0     4319 2023-04-28 16:25:08.692659 opensoundscape-0.9.0/opensoundscape/ml/sampling.py
+-rw-r--r--   0        0        0     4233 2023-04-28 16:25:08.693097 opensoundscape-0.9.0/opensoundscape/ml/utils.py
+-rw-r--r--   0        0        0      125 2022-09-07 19:54:53.425139 opensoundscape-0.9.0/opensoundscape/preprocess/__init__.py
+-rw-r--r--   0        0        0    25550 2023-04-28 16:25:08.694576 opensoundscape-0.9.0/opensoundscape/preprocess/actions.py
+-rw-r--r--   0        0        0      730 2023-01-18 14:19:19.798767 opensoundscape-0.9.0/opensoundscape/preprocess/img_augment.py
+-rw-r--r--   0        0        0    11929 2023-04-28 16:25:08.695323 opensoundscape-0.9.0/opensoundscape/preprocess/preprocessors.py
+-rw-r--r--   0        0        0     2622 2023-01-18 14:19:19.803780 opensoundscape-0.9.0/opensoundscape/preprocess/tensor_augment.py
+-rw-r--r--   0        0        0     2604 2023-01-18 14:19:19.804368 opensoundscape-0.9.0/opensoundscape/preprocess/utils.py
+-rw-r--r--   0        0        0        0 2022-09-07 19:54:53.431876 opensoundscape-0.9.0/opensoundscape/resources/__init__.py
+-rw-r--r--   0        0        0    42432 2022-09-07 19:54:53.432206 opensoundscape-0.9.0/opensoundscape/resources/species_table.csv
+-rw-r--r--   0        0        0     8817 2023-04-28 16:25:08.695756 opensoundscape-0.9.0/opensoundscape/ribbit.py
+-rw-r--r--   0        0        0     5042 2023-04-28 16:25:08.696268 opensoundscape-0.9.0/opensoundscape/sample.py
+-rw-r--r--   0        0        0    22972 2023-04-28 16:25:08.697235 opensoundscape-0.9.0/opensoundscape/signal_processing.py
+-rw-r--r--   0        0        0    32681 2023-04-28 16:25:08.697671 opensoundscape-0.9.0/opensoundscape/spectrogram.py
+-rw-r--r--   0        0        0     1901 2023-01-18 14:19:19.808150 opensoundscape-0.9.0/opensoundscape/taxa.py
+-rw-r--r--   0        0        0    12684 2023-04-28 16:25:08.698570 opensoundscape-0.9.0/opensoundscape/utils.py
+-rw-r--r--   0        0        0     1687 2023-04-28 16:25:08.701571 opensoundscape-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5757 1970-01-01 00:00:00.000000 opensoundscape-0.9.0/setup.py
+-rw-r--r--   0        0        0     5642 1970-01-01 00:00:00.000000 opensoundscape-0.9.0/PKG-INFO
```

### Comparing `opensoundscape-0.8.0/LICENSE` & `opensoundscape-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/README.md` & `opensoundscape-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 These utilities can be strung together to create data analysis pipelines. OpenSoundscape is designed to be run on any scale of computer: laptop, desktop, or computing cluster.
 
 OpenSoundscape is currently in active development. If you find a bug, please submit an issue. If you have another question about OpenSoundscape, please email Sam Lapp (`sam.lapp` at `pitt.edu`).
 
 
 #### Suggested Citation
 ```
-Lapp, Rhinehart, Freeland-Haynes, Khilnani, Syunkova, and Kitzes, 2022. "OpenSoundscape v0.8.0".
+Lapp, Rhinehart, Freeland-Haynes, Khilnani, Syunkova, and Kitzes, 2023. "OpenSoundscape v0.9.0".
 ```
 
 # Installation
 
-OpenSoundscape can be installed on Windows, Mac, and Linux machines. It has been tested on Python 3.7, 3.8, and 3.9. For Apple Silicon (M1 chip) users, Python 3.9 is recommended and may be required to avoid dependency issues. Python version 3.7.0 causes dependency issues 
-and should be avoided. 
+OpenSoundscape can be installed on Windows, Mac, and Linux machines. It has been tested on Python 3.8, and 3.9. For Apple Silicon (M1 chip) users, Python 3.9 is recommended and may be required to avoid dependency issues.
 
-Most users should install OpenSoundscape via pip: `pip install opensoundscape==0.8.0`. Contributors and advanced users can also use Poetry to install OpenSoundscape.
+Most users should install OpenSoundscape via pip: `pip install opensoundscape==0.9.0`. Contributors and advanced users can also use Poetry to install OpenSoundscape.
 
 For more detailed instructions on how to install OpenSoundscape and use it in Jupyter, see the [documentation](http://opensoundscape.org).
 
 # Features & Tutorials
 OpenSoundscape includes functions to:
 * load and manipulate audio files
 * create and manipulate spectrograms
@@ -62,30 +61,30 @@
 path = '/path/to/audiomoth_file.WAV' #an AudioMoth recording
 
 Audio.from_file(path, start_timestamp=start_time,duration=audio_length)
 ```
 
 Using a pre-trained CNN to make predictions on long audio files
 ```python
-from opensoundscape.torch.models.cnn import load_model
+from opensoundscape import load_model
 
 #get list of audio files
 files = glob('./dir/*.WAV')
 
 #generate predictions with a model
 model = load_model('/path/to/saved.model')
 scores = model.predict(files)
 
 #scores is a dataframe with MultiIndex: file, start_time, end_time
 #containing inference scores for each class and each audio window
 ```
 
 Training a CNN with labeled audio data
 ```python
-from opensoundscape.torch.models.cnn import CNN
+from opensoundscape import CNN
 from sklearn.model_selection import train_test_split
 
 #load a DataFrame of one-hot audio clip labels
 df = pd.read_csv('my_labels.csv') #index: paths; columns: classes
 train_df, validation_df = train_test_split(df,test_size=0.2)
 
 #create a CNN and train on 2-second spectrograms for 2 epochs
```

### Comparing `opensoundscape-0.8.0/opensoundscape/__init__.py` & `opensoundscape-0.9.0/opensoundscape/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 from . import annotations
-from . import audio_tools
 from . import audio
-from . import audiomoth
+from . import aru
 from . import data_selection
-from . import helpers
+from . import utils
 from . import localization
 from . import metrics
 from . import ribbit
+from . import sample
 from . import signal_processing
 from . import spectrogram
 from . import taxa
-from . import torch
+from . import ml
 from . import preprocess
 from . import resources
-from . import wandb
+from . import logging
 
 # expose some modules at the top level
-from .torch.models import cnn
+from .ml import cnn
 from .preprocess import preprocessors, actions
 
 # expose some classes at the top level
 from .audio import Audio
 from .spectrogram import Spectrogram
-from .torch.models.cnn import CNN
-from .torch.datasets import AudioFileDataset, AudioSplittingDataset
+from .ml.cnn import CNN, load_model
+from .ml.datasets import AudioFileDataset, AudioSplittingDataset
 from .preprocess.actions import Action
 from .preprocess.preprocessors import SpectrogramPreprocessor
+from .sample import AudioSample
```

### Comparing `opensoundscape-0.8.0/opensoundscape/annotations.py` & `opensoundscape-0.9.0/opensoundscape/annotations.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,23 @@
 includes BoxedAnnotations class and utilities to combine or "diff" annotations,
 etc.
 """
 from pathlib import Path
 from itertools import chain
 import pandas as pd
 import numpy as np
+import warnings
 
-from opensoundscape.helpers import overlap, overlap_fraction, generate_clip_times_df
+from opensoundscape.utils import (
+    overlap,
+    overlap_fraction,
+    generate_clip_times_df,
+    make_clip_df,
+    GetDurationError,
+)
 
 
 class BoxedAnnotations:
     """container for "boxed" (frequency-time) annotations of audio
     (for instance, annotations created in Raven software)
 
     includes functionality to load annotations from Pandas DataFrame
@@ -20,192 +27,264 @@
     specific clip lengths or clip start/end times, apply
     corrections/conversions to annotations, and more.
 
     Contains some analogous functions to Audio and Spectrogram, such as
     trim() [limit time range] and bandpass() [limit frequency range]
     """
 
-    def __init__(self, df, audio_file=None):
+    def __init__(self, df):
         """
         create object directly from DataFrame of frequency-time annotations
 
-        For loading annotations from Raven txt files, use `from_raven_file`
+        For loading annotations from Raven txt files, use `from_raven_files`
 
         Args:
             df: DataFrame of frequency-time labels. Columns must include:
                 - "annotation": string or numeric labels (can be None/nan)
                 - "start_time": left bound, sec since beginning of audio
                 - "end_time": right bound, sec since beginning of audio
+                optional columns:
+                - "file": name or path of corresponding audio file
                 - "low_f": lower frequency bound (values can be None/nan)
                 - "high_f": upper frequency bound (values can be None/nan)
-            audio_file: optionally include the name or path of corresponding
-            audio clip for which annotations are loaded from the DataFrame
+            Note: other columns will be retained in the .df
 
         Returns:
             BoxedAnnotations object
+
         """
-        required_cols = ["annotation", "start_time", "end_time", "low_f", "high_f"]
+        standard_cols = [
+            "file",
+            "annotation",
+            "start_time",
+            "end_time",
+            "low_f",
+            "high_f",
+        ]
+        required_cols = ["annotation", "start_time", "end_time"]
         for col in required_cols:
             assert col in df.columns, (
                 f"df columns must include all of these: {str(required_cols)}\n"
                 f"columns in df: {list(df.columns)}"
             )
-        self.df = df
-        self.audio_file = audio_file
+        # re-order columns
+        # keep any extras from input df and add any missing standard columns
+        ordered_cols = standard_cols + list(set(df.columns) - set(standard_cols))
+        self.df = df.reindex(columns=ordered_cols)
 
     def __repr__(self):
-        return (
-            f"<opensoundscape.annotations.BoxedAnnotations object with "
-            f"audio_file={self.audio_file}>"
-        )
+        return self.df.__repr__()
+
+    def _repr_html_(self):
+        return self.df._repr_html_()
 
     @classmethod
-    def from_raven_file(
-        cls, path, annotation_column, keep_extra_columns=True, audio_file=None
+    def from_raven_files(
+        cls,
+        raven_paths,
+        audio_files=None,
+        annotation_column_idx=7,
+        keep_extra_columns=True,
     ):
-        """load annotations from Raven txt file
+        """load annotations from Raven .txt files
 
         Args:
-            path: location of raven .txt file, str or pathlib.Path
-            annotation_column: (str) column containing annotations
+            raven_paths: list of raven .txt file paths (as str or pathlib.Path)
+            audio_files: (list) optionally specify audio files corresponding to each
+                raven file (length should match raven_paths)
+            annotation_column_idx: (int) position of column containing annotations
+                - [default: 7] will be correct if the first user-created column
+                in Raven contains annotations
                 - pass `None` to load the raven file without explicitly
                 assigning a column as the annotation column. The resulting
                 object's `.df` will have an `annotation` column with nan values!
             keep_extra_columns: keep or discard extra Raven file columns
                 (always keeps start_time, end_time, low_f, high_f, annotation
                 audio_file). [default: True]
                 - True: keep all
                 - False: keep none
                 - or iterable of specific columns to keep
-            audio_file: optionally specify the name or path of a corresponding
-                audio file.
 
         Returns:
-            BoxedAnnotations object containing annotaitons from the Raven file
+            BoxedAnnotations object containing annotations from the Raven files
+            (the .df attribute is a dataframe containing each annotation)
         """
-        df = pd.read_csv(path, delimiter="\t")
-        if annotation_column is not None:
-            assert annotation_column in df.columns, (
-                f"Raven file does not contain annotation_column={annotation_column}\n"
-                f"(columns in file: {list(df.columns)})"
-            )
+        all_file_dfs = []
+        for i, raven_path in enumerate(raven_paths):
+            df = pd.read_csv(raven_path, delimiter="\t")
+            if annotation_column_idx is not None:
+                df = df.rename(
+                    columns={
+                        df.columns[annotation_column_idx]: "annotation",
+                    }
+                )
+            else:
+                # user laoded table without specifying annotation column
+                # we'll create an empty `annotation` column
+                df["annotation"] = np.nan
+
+            # rename Raven columns to standard opensoundscape names
             df = df.rename(
                 columns={
-                    annotation_column: "annotation",
+                    "Begin Time (s)": "start_time",
+                    "End Time (s)": "end_time",
+                    "Low Freq (Hz)": "low_f",
+                    "High Freq (Hz)": "high_f",
                 }
             )
-        else:
-            # user laoded table without specifying annotation column
-            # we'll create an empty `annotation` column
-            df["annotation"] = np.nan
 
-        # rename Raven columns to standard opso names
-        df = df.rename(
-            columns={
-                "Begin Time (s)": "start_time",
-                "End Time (s)": "end_time",
-                "Low Freq (Hz)": "low_f",
-                "High Freq (Hz)": "high_f",
-            }
-        )
+            # remove undesired columns
+            standard_columns = ["start_time", "end_time", "low_f", "high_f"]
+            if annotation_column_idx is not None:
+                standard_columns.append("annotation")
+
+            if hasattr(keep_extra_columns, "__iter__"):
+                # keep the desired columns
+                df = df[standard_columns + list(keep_extra_columns)]
+            elif not keep_extra_columns:
+                # only keep required columns
+                df = df[standard_columns]
+            else:
+                # keep all columns
+                pass
+
+            # add audio file column
+            if audio_files is not None:
+                df["file"] = audio_files[i]
+            else:
+                df["file"] = np.nan
 
-        # remove undesired columns
-        standard_columns = ["start_time", "end_time", "low_f", "high_f"]
-        if annotation_column is not None:
-            standard_columns.append("annotation")
-
-        if hasattr(keep_extra_columns, "__iter__"):
-            # keep the desired columns
-            df = df[standard_columns + list(keep_extra_columns)]
-        elif not keep_extra_columns:
-            # only keep required columns
-            df = df[standard_columns]
-        else:
-            # keep all columns
-            pass
+            all_file_dfs.append(df)
+
+        return cls(df=pd.concat(all_file_dfs).reset_index())
 
-        return cls(df=df, audio_file=audio_file)
+    def to_raven_files(self, save_dir):  # TODO implement to_csv
+        """save annotations to a Raven-compatible tab-separated text files
 
-    def to_raven_file(self, path):
-        """save annotations to a Raven-compatible tab-separated text file
+        Creates one file per unique audio file in 'file' column of self.df
 
         Args:
-            path: path for saved test file (extension must be ".tsv")
+            save_dir: directory for saved files
                 - can be str or pathlib.Path
 
         Outcomes:
-            creates a file containing the annotations in a format compatible
-            with Raven Pro/Lite.
+            creates files containing the annotations for each audio file
+            in a format compatible with Raven Pro/Lite. File is tab-separated
+            and contains columns matching the Raven defaults.
 
         Note: Raven Lite does not support additional columns beyond a single
         annotation column. Additional columns will not be shown in the Raven
         Lite interface.
         """
-        assert Path(path).suffix == ".txt", "file extension must be .txt"
+        assert Path(save_dir).exists(), f"Output directory {save_dir} does not exist"
 
+        # create a copy of the labels, and rename columns to match Raven defaults
         df = self.df.copy().rename(
             columns={
                 "start_time": "Begin Time (s)",
                 "end_time": "End Time (s)",
                 "low_f": "Low Freq (Hz)",
                 "high_f": "High Freq (Hz)",
             }
         )
-        df.to_csv(path, sep="\t", index=False)
+
+        # we will create one selection table for each file
+        # this list may contain NaN, which we handle below
+        unique_files = df["file"].unique()
+
+        # If file names are no unique, raise an Exception
+        # otherwise, multiple selection table files with the same name would be
+        # written to one directory
+        file_stems = set([Path(f).stem for f in unique_files])
+        if len(file_stems) < len(unique_files):  # TODO write test for this exception
+            raise Exception(
+                "File names were not unique! Some files in different folders have the same name. "
+                "Consider subsetting .df to avoid this issue"
+            )
+
+        for file in unique_files:
+            # for NaN values of file, call the output file "unspecified.selections.txt"
+            if not file == file:
+                file_df = df[df["file"].isnull()]
+                fname = "unspecified_audio.selections.txt"
+            else:
+                file_df = df[df["file"] == file]
+                fname = f"{Path(file).stem}.selections.txt"
+            file_df.to_csv(f"{save_dir}/{fname}", sep="\t", index=False)
 
     def subset(self, classes):
         """subset annotations to those from a list of classes
 
         out-of-place operation (returns new filtered BoxedAnnotations object)
 
         Args:
             classes: list of classes to retain (all others are discarded)
             - the list can include `nan` or `None` if you want to keep them
 
         Returns:
             new BoxedAnnotations object containing only annotations in `classes`
         """
         df = self.df[self.df["annotation"].apply(lambda x: x in classes)]
-        return BoxedAnnotations(df, self.audio_file)
+        return BoxedAnnotations(df)
 
     def trim(self, start_time, end_time, edge_mode="trim"):
-        """Trim a set of annotations, analogous to Audio/Spectrogram.trim()
+        """Trim the annotations of each file in time
+
+        Trims annotations from outside of the time bounds. Note that the annotation
+        start and end times of different files may not represent the same real-world times.
+        This function only uses the numeric values of annotation start and end times in
+        the annotations, which should be relative to the beginning of the corresponding
+        audio file.
+
+        For zero-length annotations (start_time = end_time), start and end times are
+        inclusive on the left and exclusive on the right, ie [lower,upper).
+        For instance start_time=0, end_time=1 includes zero-length annotations at 0
+        but excludes zero-length annotations a 1.
 
         Out-of-place operation: does not modify itself, returns new object
 
         Args:
             start_time: time (seconds) since beginning for left bound
             end_time: time (seconds) since beginning for right bound
             edge_mode: what to do when boxes overlap with edges of trim region
                 - 'trim': trim boxes to bounds
                 - 'keep': allow boxes to extend beyond bounds
                 - 'remove': completely remove boxes that extend beyond bounds
         Returns:
             a copy of the BoxedAnnotations object on the trimmed region.
             - note that, like Audio.trim(), there is a new reference point for
-            0.0 seconds (located at start_time in the original object)
+            0.0 seconds (located at start_time in the original object). For example,
+            calling .trim(5,10) will result in an annotation previously starting at 6s
+            to start at 1s in the new object.
 
         """
         assert edge_mode in [
             "trim",
             "keep",
             "remove",
         ], f"invalid edge_mode argument: {edge_mode} (must be 'trim','keep', or 'remove')"
         assert start_time >= 0, "start time must be non-negative"
-        assert end_time > start_time, "end time_must be > start_time"
+        assert end_time > start_time, "end time_must be greater than start_time"
 
         df = self.df.copy()
 
-        # remove annotations that don't overlap with window
+        # select annotations that overlap with window
+        def in_bounds(t0, t1):
+            """check if annotation from t0 to t1 falls within
+            the range [start_range,end_range)
+
+            inclusive on left, exclusive on right
+            """
+            assert t0 <= t1
+            ends_before_bounds = t1 < start_time
+            starts_after_bounds = t0 >= end_time
+            return not (ends_before_bounds or starts_after_bounds)
+
         df = df.loc[
-            [
-                overlap([start_time, end_time], [t0, t1]) > 0
-                for t0, t1 in zip(df["start_time"], df["end_time"])
-            ],
-            :,
+            [in_bounds(t0, t1) for t0, t1 in zip(df["start_time"], df["end_time"])], :
         ]
 
         if edge_mode == "trim":  # trim boxes to start and end times
             df["start_time"] = [max(start_time, x) for x in df["start_time"]]
             df["end_time"] = [min(end_time, x) for x in df["end_time"]]
         elif edge_mode == "remove":  # remove boxes that extend beyond edges
             df = df[df["start_time"] >= start_time]
@@ -214,19 +293,23 @@
             pass
 
         # as in Audio.trim, the new object's labels should be relative to the
         # new start time; so we need to offset the old values.
         df["start_time"] = df["start_time"] - start_time
         df["end_time"] = df["end_time"] - start_time
 
-        return BoxedAnnotations(df, self.audio_file)
+        return BoxedAnnotations(df)
 
     def bandpass(self, low_f, high_f, edge_mode="trim"):
         """Bandpass a set of annotations, analogous to Spectrogram.bandpass()
 
+        Reduces the range of annotation boxes overlapping with the bandpass limits,
+        and removes annotation boxes entirely if they lie completely outside of the
+        bandpass limits.
+
         Out-of-place operation: does not modify itself, returns new object
 
         Args:
             low_f: low frequency (Hz) bound
             high_f: high frequench (Hz) bound
             edge_mode: what to do when boxes overlap with edges of trim region
                 - 'trim': trim boxes to bounds
@@ -259,22 +342,25 @@
             df["high_f"] = [min(high_f, x) for x in df["high_f"]]
         elif edge_mode == "remove":  # remove boxes that extend beyond edges
             df = df[df["low_f"] >= low_f]
             df = df[df["high_f"] <= high_f]
         else:  #'keep': leave boxes hanging over the edges
             pass
 
-        return BoxedAnnotations(df, self.audio_file)
+        return BoxedAnnotations(df)
 
     def unique_labels(self):
-        """get list of all unique (non-Falsy) labels"""
+        """get list of all unique labels
+
+        ignores null/Falsy labels by performing .df.dropna()
+        """
         return self.df.dropna(subset=["annotation"])["annotation"].unique()
 
     def global_one_hot_labels(self, classes):
-        """get a dictionary of one-hot labels for entire duration
+        """get a list of one-hot labels for entire set of annotations
         Args:
             classes: iterable of class names to give 0/1 labels
 
         Returns:
             list of 0/1 labels for each class
         """
         all_labels = self.unique_labels()
@@ -282,29 +368,35 @@
 
     def one_hot_labels_like(
         self,
         clip_df,
         min_label_overlap,
         min_label_fraction=None,
         class_subset=None,
-        keep_index=False,
+        warn_no_annotations=False,
     ):
         """create a dataframe of one-hot clip labels based on given starts/ends
 
-        Uses start and end clip times from clip_df to define a set of clips.
-        Then extracts annotatations associated overlapping with each clip.
-        Required overlap parameters are selected by user: annotation must satisfy
+        Uses start and end clip times from clip_df to define a set of clips
+        for each file. Then extracts annotations overlapping with each clip.
+
+        Required overlap to consider an annotation to overlap with a clip
+        is defined by user: an annotation must satisfy
         the minimum time overlap OR minimum % overlap to be included (doesn't
         require both conditions to be met, only one)
 
-        clip_df can be created using opensoundscap.helpers.generate_clip_times_df
+        clip_df can be created using `opensoundscap.utils.make_clip_df`
+
+        See also: `.one_hot_clip_labels()`, which creates even-lengthed clips
+        automatically and can often be used instead of this function.
 
         Args:
-            clip_df: dataframe with 'start_time' and 'end_time' columns
+            clip_df: dataframe with (file, start_time, end_time) MultiIndex
                 specifying the temporal bounds of each clip
+                (clip_df can be created using `opensoundscap.helpers.make_clip_df`)
             min_label_overlap: minimum duration (seconds) of annotation within the
                 time interval for it to count as a label. Note that any annotation
                 of length less than this value will be discarded.
                 We recommend a value of 0.25 for typical bird songs, or shorter
                 values for very short-duration events such as chip calls or
                 nocturnal flight calls.
             min_label_fraction: [default: None] if >= this fraction of an annotation
@@ -313,78 +405,77 @@
                 criterea (overlap and fraction) is met, the label is 1.
                 if None (default), this criterion is not used (i.e., only min_label_overlap
                 is used). A value of 0.5 for ths parameter would ensure that all
                 annotations result in at least one clip being labeled 1
                 (if there are no gaps between clips).
             class_subset: list of classes for one-hot labels. If None, classes will
                 be all unique values of self.df['annotation']
-            keep_index: if True, keeps the index of clip_df as an index
-                in the returned DataFrame. [default:False]
+            warn_no_annotations: bool [default:False] if True, raises warnings for
+                any files in clip_df with no corresponding annotations in self.df
 
         Returns:
-            DataFrame of one-hot labels (multi-index of (start_time, end_time),
-            columns for each class, values 0=absent or 1=present)
+            DataFrame of one-hot labels w/ multi-index of (file, start_time, end_time),
+            a column for each class, and values of 0=absent or 1=present
         """
         # drop nan annotations
         df = self.df.dropna(subset=["annotation"])
 
         if class_subset is None:  # include all annotations
             classes = df["annotation"].unique()
         else:  # the user specified a list of classes
             classes = class_subset
             # subset annotations to user-specified classes,
             # removing rows with annotations for other classes
             df = df[df["annotation"].isin(classes)]
 
-        # if we want to keep the original index, the best way is
-        # to store it and add again later
-        if keep_index:
-            og_idx = clip_df.index
-
-        # the clip_df should have ['start_time','end_time'] in columns
-        clip_df = clip_df.set_index(["start_time", "end_time"])
-        clip_df = clip_df[[]]  # remove any additional columns
+        # the clip_df should have ['file','start_time','end_time'] as the index
         clip_df[classes] = float("nan")  # add columns for each class
 
-        for (start, end), _ in clip_df.iterrows():
-            clip_df.loc[(start, end), :] = one_hot_labels_on_time_interval(
-                df,
+        for (file, start, end) in clip_df.index:
+            if not file == file:  # file is NaN, get corresponding rows
+                file_df = df[df["file"].isnull()]
+            else:  # subset annotations to this file
+                file_df = df[df.file == file]
+
+            # warn user if no annotations correspond to this file
+            if warn_no_annotations and len(file_df) == 0:
+                warnings.warn(
+                    f"No annotations matched the file {file}. All "
+                    "clip labels will be zero for this file."
+                )
+
+            # add clip labels for this row of clip dataframe
+            clip_df.loc[(file, start, end), :] = one_hot_labels_on_time_interval(
+                file_df,
                 start_time=start,
                 end_time=end,
                 min_label_overlap=min_label_overlap,
                 min_label_fraction=min_label_fraction,
                 class_subset=classes,
             )
 
-        # re-add the original index, if desired
-        if keep_index:
-            old_idx = clip_df.index.to_frame()
-            old_idx.insert(0, og_idx.name, og_idx.values)
-            clip_df.index = pd.MultiIndex.from_frame(old_idx)
-
         return clip_df
 
     def one_hot_clip_labels(
         self,
-        full_duration,
         clip_duration,
         clip_overlap,
         min_label_overlap,
         min_label_fraction=1,
+        full_duration=None,
         class_subset=None,
         final_clip=None,
     ):
         """Generate one-hot labels for clips of fixed duration
 
-        wraps helpers.generate_clip_times_df() with self.one_hot_labels_like()
+        wraps utils.make_clip_df() with self.one_hot_labels_like()
         - Clips are created in the same way as Audio.split()
         - Labels are applied based on overlap, using self.one_hot_labels_like()
 
         Args:
-            full_duration: The amount of time (seconds) to split into clips
             clip_duration (float):  The duration in seconds of the clips
             clip_overlap (float):   The overlap of the clips in seconds [default: 0]
             min_label_overlap: minimum duration (seconds) of annotation within the
                 time interval for it to count as a label. Note that any annotation
                 of length less than this value will be discarded.
                 We recommend a value of 0.25 for typical bird songs, or shorter
                 values for very short-duration events such as chip calls or
@@ -393,37 +484,68 @@
                 overlaps with the time window, it counts as a label regardless of
                 its duration. Note that *if either* of the two
                 criterea (overlap and fraction) is met, the label is 1.
                 if None (default), this criterion is not used (i.e., only min_label_overlap
                 is used). A value of 0.5 for ths parameter would ensure that all
                 annotations result in at least one clip being labeled 1
                 (if there are no gaps between clips).
+            full_duration: The amount of time (seconds) to split into clips for each file
+                float or `None`; if `None`, attempts to get each file's duration
+                using `librosa.get_duration(path=file)`
             class_subset: list of classes for one-hot labels. If None, classes will
                 be all unique values of self.df['annotation']
-            final_clip (str):       Behavior if final_clip is less than clip_duration
+            final_clip (str): Behavior if final_clip is less than clip_duration
                 seconds long. By default, discards remaining time if less than
                 clip_duration seconds long [default: None].
                 Options:
                 - None: Discard the remainder (do not make a clip)
                 - "extend": Extend the final clip beyond full_duration to reach
                     clip_duration length
                 - "remainder": Use only remainder of full_duration
                     (final clip will be shorter than clip_duration)
                 - "full": Increase overlap with previous clip to yield a
                     clip with clip_duration length
         Returns:
-            dataframe with index ['start_time','end_time'] and columns=classes
+            dataframe with index ['file','start_time','end_time'] and columns=classes
         """
+
         # generate list of start and end times for each clip
-        clip_df = generate_clip_times_df(
-            full_duration=full_duration,
-            clip_duration=clip_duration,
-            clip_overlap=clip_overlap,
-            final_clip=final_clip,
-        )
+        # if user passes None for full_duration, try to get the duration from each audio file
+        files = self.df["file"].unique()
+        if full_duration is None:
+            try:
+                clip_df = make_clip_df(
+                    files=[f for f in files if f == f],  # remove NaN if present
+                    clip_duration=clip_duration,
+                    clip_overlap=clip_overlap,
+                    final_clip=final_clip,
+                    raise_exceptions=True,  # raise exceptions from librosa.duration(f)
+                )
+            except GetDurationError as exc:
+                raise GetDurationError(
+                    """`full_duration` was None, but failed to retrieve the durations of 
+                    some files. This could occur if the values of 'file' in self.df are 
+                    not paths to valid audio files. Specifying `full_duration` as an 
+                    argument to `one_hot_clip_labels()` will avoid the attempt to get 
+                    audio file durations from file paths."""
+                )
+        else:  # use fixed full_duration for all files
+            # make a clip df, will be re-used for each file
+            clip_df_template = generate_clip_times_df(
+                full_duration=full_duration,
+                clip_duration=clip_duration,
+                clip_overlap=clip_overlap,
+                final_clip=final_clip,
+            )
+            # make a clip df for all files
+            clip_df = pd.concat([clip_df_template] * len(files))
+            # add file column, repeating value of file across each clip
+            clip_df["file"] = np.repeat(files, len(clip_df_template))
+            clip_df = clip_df.set_index(["file", "start_time", "end_time"])
+
         # then create 0/1 labels for each clip and each class
         return self.one_hot_labels_like(
             clip_df=clip_df,
             class_subset=class_subset,
             min_label_overlap=min_label_overlap,
             min_label_fraction=min_label_fraction,
         )
@@ -477,23 +599,15 @@
 
         ## apply conversions ##
         df["annotation"] = [
             conversion_table[k] if k in conversion_table else k
             for k in df["annotation"]
         ]
 
-        return BoxedAnnotations(df, self.audio_file)
-
-
-def combine(list_of_annotation_objects):
-    """combine annotations with user-specified preferences
-    Not Implemented.
-    """
-
-    raise NotImplementedError
+        return BoxedAnnotations(df)
 
 
 def diff(base_annotations, comparison_annotations):
     """look at differences between two BoxedAnnotations objects
     Not Implemented.
 
     Compare different labels of the same boxes
@@ -532,24 +646,24 @@
             in at least one clip being labeled 1 (if no gaps between clips).
 
     Returns:
         dictionary of {class:label 0/1} for all classes
     """
 
     # calculate amount of overlap of each clip with this time window
-    df.loc[:, "overlap"] = [
+    df["overlap"] = [
         overlap([start_time, end_time], [t0, t1])
         for t0, t1 in zip(df["start_time"], df["end_time"])
     ]
 
     # discard annotations that do not overlap with the time window
     df = df[df["overlap"] > 0].reset_index()
 
     # calculate the fraction of each annotation that overlaps with this time window
-    df.loc[:, "overlap_fraction"] = [
+    df["overlap_fraction"] = [
         overlap_fraction([t0, t1], [start_time, end_time])
         for t0, t1 in zip(df["start_time"], df["end_time"])
     ]
 
     one_hot_labels = [0] * len(class_subset)
     for i, c in enumerate(class_subset):
         # subset annotations to those of this class
```

### Comparing `opensoundscape-0.8.0/opensoundscape/audio.py` & `opensoundscape-0.9.0/opensoundscape/audio.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,25 +18,31 @@
 ```
 
 """
 import warnings
 from datetime import timedelta, datetime
 from pathlib import Path
 import json
+import io
+from urllib.request import urlopen
 
 import numpy as np
 from scipy.fftpack import fft as scipyfft
 from scipy.fft import fftfreq
 import librosa
 import soundfile
+import IPython.display
 
 import opensoundscape
-from opensoundscape.helpers import generate_clip_times_df, load_metadata
-from opensoundscape.audiomoth import parse_audiomoth_metadata
-from opensoundscape.audio_tools import bandpass_filter
+from opensoundscape.utils import generate_clip_times_df, load_metadata
+from opensoundscape.aru import parse_audiomoth_metadata
+from opensoundscape.signal_processing import tdoa
+from scipy.signal import butter, sosfiltfilt
+
+DEFAULT_RESAMPLE_TYPE = "soxr_hq"  # changed from kaiser_fast in v0.9.0
 
 
 class OpsoLoadAudioInputError(Exception):
     """Custom exception indicating we can't load input"""
 
 
 class AudioOutOfBoundsError(Exception):
@@ -53,24 +59,24 @@
     Initializing an `Audio` object directly requires the specification of the
     sample rate. Use `Audio.from_file` or `Audio.from_bytesio` with
     `sample_rate=None` to use a native sampling rate.
 
     Args:
         samples (np.array):     The audio samples
         sample_rate (integer):  The sampling rate for the audio samples
-        resample_type (str):    The resampling method to use [default: "kaiser_fast"]
+        resample_type (str):    The resampling method to use [default: "soxr_hq"]
 
     Returns:
         An initialized `Audio` object
     """
 
     __slots__ = ("samples", "sample_rate", "resample_type", "metadata")
 
     def __init__(
-        self, samples, sample_rate, resample_type="kaiser_fast", metadata=None
+        self, samples, sample_rate, resample_type=DEFAULT_RESAMPLE_TYPE, metadata=None
     ):
         self.samples = samples
         self.sample_rate = sample_rate
         self.resample_type = resample_type
         self.metadata = metadata
 
         samples_error = None
@@ -94,14 +100,30 @@
             raise ValueError(
                 f"Audio initialization failed with:\n{sample_rate_error}"
             ) from exc
 
         if samples_error:
             raise ValueError(f"Audio initialization failed with:\n{samples_error}")
 
+    def _spawn(self, **kwargs):
+        """return copy of object, replacing any desired fields from __slots__
+
+        pass any desired updates as kwargs
+        """
+        assert np.all([k in self.__slots__ for k in kwargs.keys()]), (
+            "only pass members of Audio.__slots__ to _spawn as kwargs! "
+            f"slots: {self.__slots__}"
+        )
+        # load the current values from each __slots__ key
+        slots = {key: self.__getattribute__(key) for key in self.__slots__}
+        # update any user-specified values
+        slots.update(kwargs)
+        # create new instance of the class
+        return self.__class__(**slots)
+
     @classmethod
     def silence(cls, duration, sample_rate):
         """ "Create audio object with zero-valued samples
 
         Args:
             duration: length in seconds
             sample_rate: samples per second
@@ -165,15 +187,15 @@
         return cls(np.clip(samples, -1, 1), sample_rate)
 
     @classmethod
     def from_file(
         cls,
         path,
         sample_rate=None,
-        resample_type="kaiser_fast",
+        resample_type=DEFAULT_RESAMPLE_TYPE,
         dtype=np.float32,
         load_metadata=True,
         offset=None,
         duration=None,
         start_timestamp=None,
         out_of_bounds_mode="warn",
     ):
@@ -194,15 +216,15 @@
         This function relies on librosa.load(), which supports wav natively but
         requires ffmpeg for mp3 support.
 
         Args:
             path (str, Path): path to an audio file
             sample_rate (int, None): resample audio with value and resample_type,
                 if None use source sample_rate (default: None)
-            resample_type: method used to resample_type (default: kaiser_fast)
+            resample_type: method used to resample_type (default: "soxr_hq")
             dtype: data type of samples returned [Default: np.float32]
             load_metadata (bool): if True, attempts to load metadata from the audio
                 file. If an exception occurs, self.metadata will be `None`.
                 Otherwise self.metadata is a dictionary.
                 Note: will also attempt to parse AudioMoth metadata from the
                 `comment` field, if the `artist` field includes `AudioMoth`.
                 The parsing function for AudioMoth is likely to break when new
@@ -331,24 +353,26 @@
             # if the offset > 0, we need to update the timestamp
             if "recording_start_time" in metadata and offset > 0:
                 metadata["recording_start_time"] += timedelta(seconds=offset)
 
         return cls(samples, sr, resample_type=resample_type, metadata=metadata)
 
     @classmethod
-    def from_bytesio(cls, bytesio, sample_rate=None, resample_type="kaiser_fast"):
+    def from_bytesio(
+        cls, bytesio, sample_rate=None, resample_type=DEFAULT_RESAMPLE_TYPE
+    ):
         """Read from bytesio object
 
         Read an Audio object from a BytesIO object. This is primarily used for
         passing Audio over HTTP.
 
         Args:
             bytesio: Contents of WAV file as BytesIO
             sample_rate: The final sampling rate of Audio object [default: None]
-            resample_type: The librosa method to do resampling [default: "kaiser_fast"]
+            resample_type: The librosa method to do resampling [default: "soxr_hq"]
 
         Returns:
             An initialized Audio object
         """
         samples, original_sample_rate = soundfile.read(bytesio)
         if sample_rate is not None and sample_rate != original_sample_rate:
             samples = librosa.resample(
@@ -358,17 +382,72 @@
                 res_type=resample_type,
             )
         else:
             sample_rate = original_sample_rate
 
         return cls(samples, sample_rate, resample_type=resample_type)
 
+    @classmethod
+    def from_url(cls, url, sample_rate=None, resample_type="kaiser_fast"):
+        """Read audio file from URL
+
+        Download audio from a URL and create an Audio object
+
+        Note: averages channels of multi-channel object to create mono object
+
+        Args:
+            url: Location to download the file from
+            sample_rate: The final sampling rate of Audio object [default: None]
+                - if None, retains original sample rate
+            resample_type: The librosa method to do resampling [default: "kaiser_fast"]
+
+        Returns:
+            Audio object
+        """
+        samples, original_sample_rate = soundfile.read(io.BytesIO(urlopen(url).read()))
+        samples = samples.mean(1)  # sum to mono
+        if sample_rate is not None and sample_rate != original_sample_rate:
+            samples = librosa.resample(
+                samples,
+                orig_sr=original_sample_rate,
+                target_sr=sample_rate,
+                res_type=resample_type,
+            )
+        else:
+            sample_rate = original_sample_rate
+
+        return cls(samples, sample_rate, resample_type=resample_type)
+
     def __repr__(self):
         return f"<Audio(samples={self.samples.shape}, sample_rate={self.sample_rate})>"
 
+    def _to_ipdisplay_audio(self, normalize=False, autoplay=False):
+        """create interactive IPython display audio object"""
+        return IPython.display.Audio(
+            data=self.samples,
+            rate=self.sample_rate,
+            normalize=normalize,
+            autoplay=autoplay,
+        )
+
+    def _repr_html_(self):
+        """create interactive audio widget
+
+        This method is used by Jupyter Notebook if the object is returned from a cell.
+        It uses the IPython.display.Audio class to create an interactive Audio widget.
+
+        """
+        return self._to_ipdisplay_audio()._repr_html_()
+
+    def show_widget(self, normalize=False, autoplay=False):
+        """create and display IPython.display.Audio widget; see that class for docs"""
+        IPython.display.display(
+            self._to_ipdisplay_audio(normalize=normalize, autoplay=autoplay)
+        )
+
     def resample(self, sample_rate, resample_type=None):
         """Resample Audio object
 
         Args:
             sample_rate (scalar):   the new sample rate
             resample_type (str):    resampling algorithm to use [default: None
                                     (uses self.resample_type of instance)]
@@ -382,15 +461,19 @@
         samples_resampled = librosa.resample(
             self.samples,
             orig_sr=self.sample_rate,
             target_sr=sample_rate,
             res_type=resample_type,
         )
 
-        return Audio(samples_resampled, sample_rate, resample_type=resample_type)
+        return self._spawn(
+            samples=samples_resampled,
+            sample_rate=sample_rate,
+            resample_type=resample_type,
+        )
 
     def trim(self, start_time, end_time):
         """Trim Audio object in time
 
         If start_time is less than zero, output starts from time 0
         If end_time is beyond the end of the sample, trims to end of sample
 
@@ -412,18 +495,16 @@
             metadata = self.metadata.copy()
             if "recording_start_time" in metadata:
                 metadata["recording_start_time"] += timedelta(seconds=start_time)
 
             if "duration" in metadata:
                 metadata["duration"] = len(samples_trimmed) / self.sample_rate
 
-        return Audio(
-            samples_trimmed,
-            self.sample_rate,
-            resample_type=self.resample_type,
+        return self._spawn(
+            samples=samples_trimmed,
             metadata=metadata,
         )
 
     def loop(self, length=None, n=None):
         """Extend audio file by looping it
 
         Args:
@@ -453,18 +534,16 @@
         if self.metadata is None:
             metadata = None
         else:
             metadata = self.metadata.copy()
             if "duration" in metadata:
                 metadata["duration"] = len(samples_extended) / self.sample_rate
 
-        return Audio(
-            samples_extended,
-            self.sample_rate,
-            resample_type=self.resample_type,
+        return self._spawn(
+            samples=samples_extended,
             metadata=metadata,
         )
 
     def extend(self, length):
         """Extend audio file by adding silence to the end
 
         Args:
@@ -483,18 +562,16 @@
         if self.metadata is None:
             metadata = None
         else:
             metadata = self.metadata.copy()
             if "duration" in metadata:
                 metadata["duration"] = len(samples_extended) / self.sample_rate
 
-        return Audio(
-            samples_extended,
-            self.sample_rate,
-            resample_type=self.resample_type,
+        return self._spawn(
+            samples=samples_extended,
             metadata=metadata,
         )
 
     def bandpass(self, low_f, high_f, order):
         """Bandpass audio signal with a butterworth filter
 
         Uses a phase-preserving algorithm (scipy.signal's butter and solfiltfilt)
@@ -511,17 +588,15 @@
 
         if high_f >= self.sample_rate / 2:
             raise ValueError("high_f must be less than sample_rate/2")
 
         filtered_samples = bandpass_filter(
             self.samples, low_f, high_f, self.sample_rate, order=order
         )
-        return Audio(
-            filtered_samples, self.sample_rate, resample_type=self.resample_type
-        )
+        return self._spawn(samples=filtered_samples)
 
     def spectrum(self):
         """Create frequency spectrum from an Audio object using fft
 
         Args:
             self
 
@@ -576,20 +651,15 @@
             peak_level = 10 ** (peak_dBFS / 20)
 
         abs_max = max(max(self.samples), -min(self.samples))
         if abs_max == 0:
             # don't try to normalize 0-valued samples. Return original object
             abs_max = 1
 
-        return Audio(
-            self.samples / abs_max * peak_level,
-            self.sample_rate,
-            resample_type=self.resample_type,
-            metadata=self.metadata,
-        )
+        return self._spawn(samples=self.samples / abs_max * peak_level)
 
     def apply_gain(self, dB, clip_range=(-1, 1)):
         """apply dB (decibels) of gain to audio signal
 
         Specifically, multiplies samples by 10^(dB/20)
 
         Args:
@@ -601,20 +671,15 @@
 
         Returns:
             Audio object with gain applied to samples
         """
         samples = self.samples * (10 ** (dB / 20))
         if clip_range is not None:
             samples = np.clip(samples, clip_range[0], clip_range[1])
-        return Audio(
-            samples,
-            self.sample_rate,
-            resample_type=self.resample_type,
-            metadata=self.metadata,
-        )
+        return self._spawn(samples=samples)
 
     def save(
         self,
         path,
         metadata_format="opso",
         soundfile_subtype=None,
         soundfile_format=None,
@@ -816,15 +881,15 @@
         """calculate the root-mean-square dB value relative to a full-scale sine wave"""
         return 20 * np.log10(self.rms * np.sqrt(2))
 
 
 def load_channels_as_audio(
     path,
     sample_rate=None,
-    resample_type="kaiser_fast",
+    resample_type=DEFAULT_RESAMPLE_TYPE,
     dtype=np.float32,
     offset=0,
     duration=None,
     metadata=True,
 ):
     """Load each channel of an audio file to a separate Audio object
 
@@ -907,18 +972,17 @@
     ), "all elements in audio_objects must be Audio objects"
 
     # use first object's sample rate if None provided
     if sample_rate is None:
         sample_rate = audio_objects[0].sample_rate
 
     # concatenate sample arrays to form new Audio object
-    return Audio(
-        np.hstack([a.resample(sample_rate).samples for a in audio_objects]),
-        sample_rate,
-        resample_type=audio_objects[0].resample_type,
+    return audio_objects[0]._spawn(
+        samples=np.hstack([a.resample(sample_rate).samples for a in audio_objects]),
+        sample_rate=sample_rate,
     )
 
 
 def mix(
     audio_objects,
     duration=None,
     gain=-3,
@@ -1037,15 +1101,76 @@
         # add samples to mixdown
         mixdown += audio.samples
 
     # limit sample values to clip_range
     if clip_range is not None:
         mixdown = np.clip(mixdown, clip_range[0], clip_range[1])
 
-    return Audio(mixdown, sample_rate, resample_type=audio_objects[0].resample_type)
+    return audio_objects[0]._spawn(samples=mixdown, sample_rate=sample_rate)
+
+
+def estimate_delay(
+    audio,
+    reference_audio,
+    bandpass_range=None,
+    bandpass_order=9,
+    cc_filter="phat",
+    return_cc_max=False,
+    max_delay=None,
+    skip_ref_bandpass=False,
+):
+    """Use generalized cross correlation to estimate time delay between signals
+
+    optionally bandpass audio signals to a frequency range
+
+    For example, if audio is delayed by 1 second compared to reference_audio,
+    result is 1.0.
+
+    Args:
+        audio, reference_audio: audio objects
+        bandpass_range: if None, no bandpass filter is performed
+            otherwise [low_f,high_f]
+        bandpass_order: order of Butterworth bandpass filter
+        cc_filter: generalized cross correlation type, see
+            opensoundscape.signal_processing.gcc() [default: 'phat']
+        return_cc_max: if True, returns cross correlation max value as second argument
+            (see `opensoundscape.signal_processing.tdoa`)
+        max_delay: maximum time delay to consider, in seconds
+            (see `opensoundscape.signal_processing.tdoa`) [default: None] allows any delay
+        skip_ref_bandpass: [default: False] if True, skip the bandpass operation for the
+            reference_audio object, only apply it to `audio`
+    Returns:
+        estimated time delay (seconds) from reference_audio to audio
+
+        if return_cc_max is True, also returns a second value, the max of the cross correlation
+        of the two signals
+
+    Note: resamples reference_audio if its sample rate does not match audio
+    """
+    # sample rates must match
+    sr = audio.sample_rate
+    if reference_audio.sample_rate != sr:
+        reference_audio = reference_audio.resample(sr)
+
+    # apply audio-domain butterworth bandpass filter if desired
+    if bandpass_range is not None:
+        l, h = bandpass_range  # extract low and high frequencies
+        audio = audio.bandpass(l, h, bandpass_order)
+        if not skip_ref_bandpass:
+            reference_audio = reference_audio.bandpass(l, h, bandpass_order)
+
+    # estimate time delay from reference_audio to audio using generalized cross correlation
+    return tdoa(
+        audio.samples,
+        reference_audio.samples,
+        cc_filter=cc_filter,
+        sample_rate=sr,
+        return_max=return_cc_max,
+        max_delay=max_delay,
+    )
 
 
 def parse_opso_metadata(comment_string):
     """parse metadata saved by opensoundcsape as json in comment field
 
     Parses a json string which opensoundscape saves to the comment metadata field
     of WAV files to preserve metadata. The string begins with `opso_metadata`
@@ -1196,7 +1321,57 @@
             "album",
             "license",
             "tracknumber",
             "genre",
         ]:
             if field in metadata and metadata[field] is not None:
                 s.__setattr__(field, metadata[field])
+
+
+def butter_bandpass(low_f, high_f, sample_rate, order=9):
+    """generate coefficients for bandpass_filter()
+
+    Args:
+        low_f: low frequency of butterworth bandpass filter
+        high_f: high frequency of butterworth bandpass filter
+        sample_rate: audio sample rate
+        order=9: order of butterworth filter
+
+    Returns:
+        set of coefficients used in sosfiltfilt()
+    """
+    nyq = 0.5 * sample_rate
+    low = low_f / nyq
+    high = high_f / nyq
+    sos = butter(order, [low, high], analog=False, btype="band", output="sos")
+    return sos
+
+
+def bandpass_filter(signal, low_f, high_f, sample_rate, order=9):
+    """perform a butterworth bandpass filter on a discrete time signal
+    using scipy.signal's butter and sosfiltfilt (phase-preserving filtering)
+
+    Args:
+        signal: discrete time signal (audio samples, list of float)
+        low_f: -3db point (?) for highpass filter (Hz)
+        high_f: -3db point (?) for highpass filter (Hz)
+        sample_rate: samples per second (Hz)
+        order: higher values -> steeper dropoff [default: 9]
+
+    Returns:
+        filtered time signal
+    """
+    sos = butter_bandpass(low_f, high_f, sample_rate, order=order)
+    return sosfiltfilt(sos, signal)
+
+
+def clipping_detector(samples, threshold=0.6):
+    """count the number of samples above a threshold value
+
+    Args:
+        samples: a time series of float values
+        threshold=0.6: minimum value of sample to count as clipping
+
+    Returns:
+        number of samples exceeding threshold
+    """
+    return len(list(filter(lambda x: x > threshold, samples)))
```

### Comparing `opensoundscape-0.8.0/opensoundscape/audiomoth.py` & `opensoundscape-0.9.0/opensoundscape/aru.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""Utilities specifically for audio files recoreded by AudioMoths"""
+"""Utilities specifically for audio files recoreded by AudioMoths and other ARUs"""
 from pathlib import Path
 import datetime
 
 import pytz
-from opensoundscape.helpers import hex_to_time, load_metadata
+from opensoundscape.utils import hex_to_time, load_metadata
 
 
 def audiomoth_start_time(file, filename_timezone="UTC", to_utc=False):
     """parse audiomoth file name into a time stamp
 
     AudioMoths create their file name based on the time that recording starts.
     This function parses the name into a timestamp. Older AudioMoth firmwares
```

### Comparing `opensoundscape-0.8.0/opensoundscape/data_selection.py` & `opensoundscape-0.9.0/opensoundscape/data_selection.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/helpers.py` & `opensoundscape-0.9.0/opensoundscape/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,41 @@
 import pandas as pd
 import pytz
 import soundfile
 
 import librosa
 
 
+class GetDurationError(ValueError):
+    """raised if librosa.get_duration(path=f) causes an error"""
+
+    pass
+
+
 def isNan(x):
     """check for nan by equating x to itself"""
     return not x == x
 
 
 def sigmoid(x):
     """sigmoid function"""
     return 1 / (1 + np.exp(-x))
 
 
+def identity(x):
+    """return the input unchanged"""
+    return x
+
+
 def overlap(r1, r2):
-    """ "calculate the amount of overlap between two real-numbered ranges"""
-    assert r1[1] > r1[0]
-    assert r2[1] > r2[0]
+    """ "calculate the amount of overlap between two real-numbered ranges
+
+    ranges must be [low,high] where low <= high"""
+    assert r1[1] >= r1[0]
+    assert r2[1] >= r2[0]
     lower_bound = max(r1[0], r2[0])
     upper_bound = min(r1[1], r2[1])
     return max(0, upper_bound - lower_bound)
 
 
 def overlap_fraction(r1, r2):
     """ "calculate the fraction of r1 (low, high range) that overlaps with r2"""
@@ -240,15 +253,20 @@
         starts = starts.round(rounding_precision)
         ends = ends.round(rounding_precision)
 
     return pd.DataFrame({"start_time": starts, "end_time": ends}).drop_duplicates()
 
 
 def make_clip_df(
-    files, clip_duration, clip_overlap=0, final_clip=None, return_invalid_samples=False
+    files,
+    clip_duration,
+    clip_overlap=0,
+    final_clip=None,
+    return_invalid_samples=False,
+    raise_exceptions=False,
 ):
     """generate df of fixed-length clip start/end times for a set of files
 
     Used internally to prepare a dataframe listing clips of longer audio files
 
     This function creates a single dataframe with audio files as
     the index and columns: 'start_time', 'end_time'. It will list
@@ -263,25 +281,30 @@
         files: list of audio file paths, or dataframe with file path as index
             - if dataframe, columns represent classes and values represent
             class labels. Labels for a file will be copied to all clips
             belonging to that file in the returned clip dataframe.
         clip_duration (float): see generate_clip_times_df
         clip_overlap (float): see generate_clip_times_df
         final_clip (str): see generate_clip_times_df
-        return_invalid_samples (bool): if true, returns additional value,
+        return_invalid_samples (bool): if True, returns additional value,
             a list of samples that caused exceptions
+        raise_exceptions (bool): if True, if exceptions are raised when attempting
+            to check the duration of an audio file, the exception will be raised.
+            If False [default], adds a row to the dataframe with np.nan for
+            'start_time' and 'end_time' for that file path.
 
     Returns:
         clip_df: dataframe multi-index ('file','start_time','end_time')
             - if files is a dataframe, will contain same columns as files
             - otherwise, will have no columns
 
         if return_invalid_samples==True, returns (clip_df, invalid_samples)
 
-    Note: if an exception is raised (for instance, trying to get the duration of the file),
+    Note: default behavior for raise_exceptions is the following:
+        if an exception is raised (for instance, trying to get the duration of the file),
         the dataframe will have one row with np.nan for 'start_time' and 'end_time' for that
         file path.
     """
     if isinstance(files, str):
         raise TypeError(
             "make_clip_df expects a list of files, it looks like you passed it a string"
         )
@@ -301,29 +324,32 @@
 
     assert len(files) > 0, "files list has length zero!"
 
     clip_dfs = []
     invalid_samples = set()
     for f in file_list:
         try:
-            t = librosa.get_duration(filename=f)
+            t = librosa.get_duration(path=f)
             clips = generate_clip_times_df(
                 full_duration=t,
                 clip_duration=clip_duration,
                 clip_overlap=clip_overlap,
                 final_clip=final_clip,
             )
             clips["file"] = f
 
-        except:
-            # make one row for this file with nan for start/end times
-            clips = pd.DataFrame(
-                {"file": [f], "start_time": np.nan, "end_time": np.nan}
-            )
-            invalid_samples.add(f)
+        except Exception as exc:
+            if raise_exceptions:
+                raise GetDurationError(f"Exception on file {f}") from exc
+            else:
+                # make one row for this file with nan for start/end times
+                clips = pd.DataFrame(
+                    {"file": [f], "start_time": np.nan, "end_time": np.nan}
+                )
+                invalid_samples.add(f)
 
         if label_df is not None:
             # copy labels for this file to all of its clips
             clips[label_df.columns] = label_df.loc[f]
 
         clip_dfs.append(clips)
```

### Comparing `opensoundscape-0.8.0/opensoundscape/metrics.py` & `opensoundscape-0.9.0/opensoundscape/metrics.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/preprocess/actions.py` & `opensoundscape-0.9.0/opensoundscape/preprocess/actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from torchvision import transforms
 import torch
 import pandas as pd
 
 from opensoundscape.audio import Audio, mix
 from opensoundscape.preprocess import tensor_augment as tensaug
 from opensoundscape.preprocess.utils import PreprocessingError, get_args, get_reqd_args
+from opensoundscape.sample import AudioSample
 
 
 class BaseAction:
     """Parent class for all Actions (used in Preprocessor pipelines)
 
     New actions should subclass this class.
 
@@ -30,28 +31,28 @@
     = original file path, columns=class names, values=labels (0,1). X is the
     sample, and can be of various types (path, Audio, Spectrogram, Tensor, etc).
     See Overlay for an example of an Action that uses labels.
     """
 
     def __init__(self):
         self.params = pd.Series(dtype="object")
-        self.extra_args = []
         self.returns_labels = False
         self.is_augmentation = False
         self.bypass = False
 
     def __repr__(self):
         return (
             f"{'Bypassed ' if self.bypass else ''}"
             f"{'Augmentation ' if self.is_augmentation else ''}"
             "Action"
         )
 
     def go(self, x):
-        return x
+        # modifies the sample in-place
+        pass
 
     def set(self, **kwargs):
         """only allow keys that exist in self.params"""
         unmatched_args = set(list(kwargs.keys())) - set(list(self.params.keys()))
         assert unmatched_args == set([]), (
             f"unexpected arguments: {unmatched_args}. "
             f"The valid arguments and current values are: \n{self.params}"
@@ -72,61 +73,61 @@
         eg. Audio.from_file(path,**kwargs)
     (B) method of a class, which takes 'self' as the first argument,
         eg. Spectrogram.bandpass(self,**kwargs)
 
     Other arguments are an arbitrary list of kwargs.
     """
 
-    def __init__(self, fn, is_augmentation=False, extra_args=(), **kwargs):
+    def __init__(self, fn, is_augmentation=False, **kwargs):
         super(Action, self).__init__()
 
         self.action_fn = fn
         self.is_augmentation = is_augmentation
 
-        # args that vary for each sample, will be passed from preprocessor
-        self.extra_args = extra_args
-
         # query action_fn for arguments and default values
         self.params = pd.Series(get_args(self.action_fn), dtype=object)
 
         # whether the first argument is 'self' or the incoming object,
         # we remove it from the params dict
         self.params = self.params[1:]
 
-        # remove "extra_args" from self.params if they are present:
-        # these sample-specific arguments will be passed to action.go()
-        # directly, so they should not be part of the self.params dictionary
-        self.params = self.params.drop([p for p in extra_args if p in self.params])
-
         # update self.params with any user-provided parameters
         self.set(**kwargs)
 
         # make sure all required args are given (skipping the first, which will be provided by go)
-        unmatched_reqd_args = (
-            set(get_reqd_args(self.action_fn)[1:])
-            - set(list(kwargs.keys()))
-            - set(self.extra_args)
+        unmatched_reqd_args = set(get_reqd_args(self.action_fn)[1:]) - set(
+            list(kwargs.keys())
         )
 
         assert unmatched_reqd_args == set(
             []
         ), f"These required arguments were not provided: {unmatched_reqd_args}"
 
     def __repr__(self):
         return (
             f"{'## Bypassed ## ' if self.bypass else ''}"
             f"{'Augmentation ' if self.is_augmentation else ''}"
             f"Action calling {self.action_fn}"
         )
 
-    def go(self, x, **kwargs):
+    def go(self, sample, **kwargs):
         # the syntax is the same regardless of whether
         # first argument is "self" (for a class method) or not
         # we pass self.params to kwargs along with any additional kwargs
-        return self.action_fn(x, **dict(self.params, **kwargs))
+
+        # only pass (and get back) the data of the sample to the action function
+        # to use other attributes of sample.data, write another class and override
+        # this go() method, for example:
+        # def go(self, sample, **kwargs):
+        #   self.action_fn(sample, **dict(self.params, **kwargs))
+
+        # should we make a copy to avoid modifying the original object?
+        # or accept that we are modifying the original sample in-place?
+        # I think its in-place since we now pass an object and update the data
+        sample.data = self.action_fn(sample.data, **dict(self.params, **kwargs))
 
 
 class AudioClipLoader(Action):
     """Action to load clips from an audio file
 
     Loads an audio file or part of a file to an Audio object.
     Will load entire audio file if _start_time and _end_time are None.
@@ -136,88 +137,125 @@
     see Audio.from_file() for documentation.
 
     Args:
         see Audio.from_file()
     """
 
     def __init__(self, **kwargs):
-        super(AudioClipLoader, self).__init__(
-            Audio.from_file, extra_args=["_start_time", "_end_time"], **kwargs
-        )
-        # two params are replaced by "_start_time" and "_end_time"
+        super(AudioClipLoader, self).__init__(Audio.from_file, **kwargs)
+        # two params are provided by sample.start_time and sample.duration
         self.params = self.params.drop(["offset", "duration"])
 
-    def go(self, path, _start_time, _end_time, **kwargs):
-        offset = 0 if _start_time is None else _start_time
-        duration = None if _end_time is None else _end_time - _start_time
-        return self.action_fn(
-            path, offset=offset, duration=duration, **dict(self.params, **kwargs)
+    def go(self, sample, **kwargs):
+        offset = 0 if sample.start_time is None else sample.start_time
+        duration = None if sample.duration is None else sample.duration
+        sample.data = self.action_fn(
+            sample.data, offset=offset, duration=duration, **dict(self.params, **kwargs)
         )
 
 
 class AudioTrim(Action):
     """Action to trim/extend audio to desired length
 
     Args:
         see actions.trim_audio
     """
 
     def __init__(self, **kwargs):
-        super(AudioTrim, self).__init__(
-            trim_audio, extra_args=("_sample_duration",), **kwargs
-        )
+        super(AudioTrim, self).__init__(trim_audio, **kwargs)
+
+    def go(self, sample, **kwargs):
+        self.action_fn(sample, **dict(self.params, **kwargs))
 
 
-def trim_audio(audio, _sample_duration, extend=True, random_trim=False, tol=1e-5):
+def trim_audio(sample, extend=True, random_trim=False, tol=1e-5):
     """trim audio clips (Audio -> Audio)
 
     Trims an audio file to desired length
     Allows audio to be trimmed from start or from a random time
     Optionally extends audio shorter than clip_length with silence
 
     Args:
-        audio: Audio object
-        _sample_duration: desired final length (sec)
-            - if None, no trim is performed
-        extend: if True, clips shorter than _sample_duration are
+        sample: AudioSample with .data=Audio object, .duration as sample duration
+        extend: if True, clips shorter than sample.duration are
             extended with silence to required length
-        random_trim: if True, chooses a random segment of length _sample_duration
+        random_trim: if True, chooses a random segment of length sample.duration
             from the input audio. If False, the file is trimmed from 0 seconds
-            to _sample_duration seconds.
+            to sample.duration seconds.
         tol: tolerance for considering a clip to be of the correct length (sec)
 
     Returns:
         trimmed audio
     """
+    audio = sample.data
+
     if len(audio.samples) == 0:
         raise ValueError("recieved zero-length audio")
 
-    if _sample_duration is not None:
-        if audio.duration + tol <= _sample_duration:
+    if sample.target_duration is not None:
+        if audio.duration + tol <= sample.target_duration:
             # input audio is not as long as desired length
             if extend:  # extend clip sith silence
-                audio = audio.extend(_sample_duration)
+                audio = audio.extend(sample.target_duration)
             else:
                 raise ValueError(
                     f"the length of the original file ({audio.duration} "
                     f"sec) was less than the length to extract "
-                    f"({_sample_duration} sec). To extend short "
+                    f"({sample.target_duration} sec). To extend short "
                     f"clips, use extend=True"
                 )
         if random_trim:
             # uniformly randomly choose clip time from full audio
-            extra_time = audio.duration - _sample_duration
+            extra_time = audio.duration - sample.target_duration
             start_time = np.random.uniform() * extra_time
         else:
             start_time = 0
 
-        end_time = start_time + _sample_duration
+        end_time = start_time + sample.target_duration
         audio = audio.trim(start_time, end_time)
 
-    return audio
+        # update the sample
+        sample.data = audio
+        if sample.start_time is None:
+            sample.start_time = start_time
+        else:
+            sample.start_time += start_time
+        sample.duration = sample.target_duration
+
+    return sample
+
+
+class SpectrogramToTensor(BaseAction):
+    """Action to create Tesnsor of desired shape from Spectrogram
+
+    calls .to_image on sample.data, which should be type Spectrogram
+
+    exposes `invert` argument in self.params
+    """
+
+    def __init__(
+        self,
+        colormap=None,
+        invert=False,
+    ):
+        super(SpectrogramToTensor, self).__init__()
+        self.params["colormap"] = colormap
+        self.params["invert"] = invert
+
+    def go(self, sample):
+        """converts sample.data from Spectrogram to Tensor"""
+        # sample.data must be Spectrogram object
+        # sample should have attribute target_shape [h,w,channels]
+        sample.data = sample.data.to_image(
+            shape=sample.target_shape[0:2],
+            channels=sample.target_shape[2],
+            return_type="torch",
+            colormap=self.params["colormap"],
+            invert=self.params["invert"],
+        )
 
 
 def audio_random_gain(audio, dB_range=(-30, 0), clip_range=(-1, 1)):
     """Applies a randomly selected gain level to an Audio object
 
     Gain is selected from a uniform distribution in the range dB_range
 
@@ -443,15 +481,14 @@
     """
 
     def __init__(self, is_augmentation=True, **kwargs):
 
         super(Overlay, self).__init__(
             overlay,
             is_augmentation=is_augmentation,
-            extra_args=("_labels", "_preprocessor"),
             **kwargs,
         )
 
         self.returns_labels = True
 
         overlay_df = kwargs["overlay_df"]
         overlay_df = overlay_df[~overlay_df.index.duplicated()]  # remove duplicates
@@ -470,24 +507,22 @@
                 "Consider renaming the `different` class. "
             )
 
         # move overlay_df from params to its own space so that it doesn't display with print(params)
         self.overlay_df = overlay_df
         self.params = self.params.drop("overlay_df")  # removes it
 
-    def go(self, x, **kwargs):
-        return self.action_fn(
-            x, overlay_df=self.overlay_df, **dict(self.params, **kwargs)
+    def go(self, sample, **kwargs):
+        self.action_fn(
+            sample, overlay_df=self.overlay_df, **dict(self.params, **kwargs)
         )
 
 
 def overlay(
-    x,
-    _labels,
-    _preprocessor,
+    sample,
     overlay_df,
     update_labels,
     overlay_class=None,
     overlay_prob=1,
     max_overlay_num=1,
     overlay_weight=0.5,
 ):
@@ -501,18 +536,19 @@
         1. a separate df where any file can be overlayed (overlay_class=None)
         2. same df as training, where the overlay class is "different" ie,
             does not contain overlapping labels with the original sample
         3. same df as training, where samples from a specific class are used
             for overlays
 
     Args:
+        sample: AudioSample with .labels: labels of the original sample
+            and .preprocessor: the preprocessing pipeline
         overlay_df: a labels dataframe with audio files as the index and
             classes as columns
-        _labels: labels of the original sample
-        _preprocessor: the preprocessing pipeline
+
         update_labels: if True, add overlayed sample's labels to original sample
         overlay_class: how to choose files from overlay_df to overlay
             Options [default: "different"]:
             None - Randomly select any file from overlay_df
             "different" - Select a random file from overlay_df containing none
                 of the classes this file contains
             specific class name - always choose files from this class
@@ -561,15 +597,15 @@
         if overlay_class != "different":  # user specified a single class
             assert (
                 overlay_df[overlay_class].sum() > 0
             ), "overlay_df did not contain positive labels for overlay_class"
 
     if len(overlay_df.columns) > 0:
         assert list(overlay_df.columns) == list(
-            _labels.index
+            sample.labels.index
         ), "overlay_df mast have same columns as sample's _labels or no columns"
 
     ## OVERLAY ##
     # iteratively perform overlays until stopping condition
     # each time, there is an overlay_prob probability of another overlay
     # up to a max number of max_overlay_num overlays
     overlays_performed = 0
@@ -595,15 +631,15 @@
                     attempt_counter += 1
 
                     # choose a random sample from the overlay df
                     candidate_idx = random.randint(0, len(overlay_df) - 1)
 
                     # check if this candidate sample has zero overlapping labels
                     label_intersection = np.logical_and(
-                        overlay_df.values[candidate_idx, :], _labels.values
+                        overlay_df.values[candidate_idx, :], sample.labels.values
                     )
                     good_choice = sum(label_intersection) == 0
 
                 if not good_choice:  # tried max_attempts samples, none worked
                     raise ValueError(
                         "No samples found with non-overlapping labels after 100 random draws"
                     )
@@ -615,50 +651,51 @@
                 # however, in the case of a fixed overlay class, we could
                 # pass an overlay_df containing only that class)
                 choose_from = overlay_df[overlay_df[overlay_class] == 1]
                 overlay_path = np.random.choice(choose_from.index.values)
 
             # now we have picked a file to overlay (overlay_path)
             # we also know its labels, if we need them
-            overlay_row = overlay_df.loc[overlay_path]
-            overlay_labels = overlay_row.values
+            overlay_sample = AudioSample.from_series(overlay_df.loc[overlay_path])
 
             # now we need to run the pipeline to do everything up until the Overlay step
             # create a preprocessor for loading the overlay samples
             # note that if there are multiple Overlay objects in a pipeline,
             # it will cut off the preprocessing of the overlayed sample before
             # the first Overlay object. This may or may not be the desired behavior,
             # but it will at least "work".
-            x2, _ = _preprocessor.forward(overlay_row, break_on_type=Overlay)
+            overlay_sample = sample.preprocessor.forward(
+                overlay_sample, break_on_type=Overlay
+            )
 
             # now we blend the two tensors together with a weighted average
             # Select weight of overlay; <0.5 means more emphasis on original sample
             # Supports uniform-random selection from a range of weights eg [0.1,0.7]
             weight = overlay_weight
             if hasattr(weight, "__iter__"):
                 assert len(weight) == 2, (
                     f"overlay_weight must specify a single value or range of 2 values, "
                     f"got {overlay_weight}"
                 )
                 weight = random.uniform(weight[0], weight[1])
 
-            # use a weighted sum to overlay (blend) the samples
-            x = x * (1 - weight) + x2 * weight
+            # use a weighted sum to overlay (blend) the samples (arrays or tensors)
+            sample.data = sample.data * (1 - weight) + overlay_sample.data * weight
 
             # update the labels with new classes
-            if update_labels and len(overlay_labels) > 0:
+            if update_labels and len(overlay_sample.labels) > 0:
                 # update labels as union of both files' labels
-                _labels.values[:] = np.logical_or(
-                    _labels.values, overlay_labels
+                sample.labels.values[:] = np.logical_or(
+                    sample.labels.values, overlay_sample.labels.values
                 ).astype(int)
 
             # overlay was successful, update count:
             overlays_performed += 1
 
         except PreprocessingError as ex:
             # don't try to load this sample again: remove from overlay df
             overlay_df = overlay_df.drop(overlay_path)
             warnings.warn(f"Invalid overlay sample: {overlay_path}")
             if len(overlay_df) < 1:
                 raise ValueError("tried all overlay_df samples, none were safe") from ex
 
-    return x, _labels
+    return sample
```

### Comparing `opensoundscape-0.8.0/opensoundscape/preprocess/img_augment.py` & `opensoundscape-0.9.0/opensoundscape/preprocess/img_augment.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/preprocess/preprocessors.py` & `opensoundscape-0.9.0/opensoundscape/preprocess/preprocessors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """Preprocessor classes: tools for preparing and augmenting audio samples"""
 from pathlib import Path
 import pandas as pd
+import copy
 
 from opensoundscape.preprocess import actions
 from opensoundscape.preprocess.actions import (
     Action,
     Overlay,
     AudioClipLoader,
     AudioTrim,
+    SpectrogramToTensor,
 )
 from opensoundscape.preprocess.utils import PreprocessingError
 from opensoundscape.spectrogram import Spectrogram
+from opensoundscape.sample import AudioSample
 
 
 class BasePreprocessor:
     """Class for defining an ordered set of Actions and a way to run them
 
     Custom Preprocessor classes should subclass this class or its children
 
     Preprocessors have one job: to transform samples from some input (eg
-    a file path) to some output (eg a torch.Tensor) using a specific procedure.
-    The procedure consists of Actions ordered by the Preprocessor's index.
-    Preprocessors have a forward() method which runs the set of Actions
-    specified in the index.
+    a file path) to some output (eg an AudioSample with .data as torch.Tensor)
+    using a specific procedure defined by the .pipeline attribute.
+    The procedure consists of Actions ordered by the Preprocessor's .pipeline.
+    Preprocessors have a forward() method which sequentially applies the Actions
+    in the pipeline to produce a sample.
 
     Args:
         action_dict: dictionary of name:Action actions to perform sequentially
         sample_duration: length of audio samples to generate (seconds)
     """
 
     def __init__(self, sample_duration=None):
@@ -105,97 +109,89 @@
                 - dictionary {"start_time":float,"end_time":float}:
                     the start and end time of clip in audio
             bypass_augmentations: if True, actions with .is_augmentatino=True
                 are skipped
             trace (boolean - default False): if True, saves the output of each pipeline step in the `sample_info` output argument - should be utilized for analysis/debugging on samples of interest
 
         Returns:
-            {'X':preprocessed sample, 'y':labels} if return_labels==True,
-            otherwise {'X':preprocessed sample}
+            sample (instance of AudioSample class)
 
         """
         if break_on_key is not None:
             assert (
                 break_on_key in self.pipeline
             ), f"break_on_key was {break_on_key} but no matching action found in pipeline"
 
-        # handle paths or pd.Series as input for `sample`
-        if type(sample) == str or issubclass(type(sample), Path):
-            label_df_row = pd.Series(dtype=object, name=sample)
-        else:
-            assert type(sample) == pd.Series, (
-                "sample must be pd.Series with "
-                "path as .name OR file path (str or pathlib.Path), "
-                "OR have multi-index (file,start_time,end_time)"
-                f"was {type(sample)}"
-            )
-            label_df_row = sample
-
-        has_clips = type(label_df_row.name) == tuple
-        if has_clips:
-            # if the dataframe has a multi-index, it should be (file,start_time,end_time)
-            assert (
-                len(label_df_row.name) == 3
-            ), "multi-index must be ('file','start_time','end_time')"
-            sample_path, clip_start_time, clip_end_time = label_df_row.name
-        else:
-            # Series.name (dataframe index) contains a path to a file
-            # No clip times are provided, so the entire file will be loaded
-            sample_path = Path(label_df_row.name)
-            clip_start_time = None
-            clip_end_time = None
-
-        # a list of additional variables that an action may request from the preprocessor
-        sample_info = {
-            "_path": sample_path,
-            "_labels": label_df_row.copy(deep=True),
-            "_start_time": clip_start_time,
-            "_end_time": clip_end_time,
-            "_sample_duration": self.sample_duration,
-            "_preprocessor": self,
-            "_trace": pd.Series(index=self.pipeline.index) if trace else None,
-        }
+        # create AudioSample from input path
+        sample = self._generate_sample(sample)
+        if trace:
+            sample.trace = pd.Series(index=self.pipeline.index)
 
+        # run the pipeline by performing each Action on the AudioSample
         try:
-            x = sample_path
             # perform each action in the pipeline
             for k, action in self.pipeline.items():
                 if type(action) == break_on_type or k == break_on_key:
-                    if (
-                        trace
-                    ):  # if tracing, add a note to the trace that the pipeline was terminated
-                        sample_info["_trace"][
-                            k
-                        ] = f"## Pipeline terminated ## {sample_info['_trace'][k]}"
+                    if trace:
+                        # saved "output" of this step informs user pipeline was stopped
+                        sample.trace[k] = f"## Pipeline terminated ## {sample.trace[k]}"
                     break
                 if action.bypass:
                     continue
                 if action.is_augmentation and bypass_augmentations:
-                    if (
-                        trace
-                    ):  # if tracing, add a note to the trace that the augmentation was bypassed
-                        sample_info["_trace"][
-                            k
-                        ] = f"## Bypassed ## {sample_info['_trace'][k]}"
+                    if trace:
+                        sample.trace[k] = f"## Bypassed ## {sample.trace[k]}"
                     continue
-                extra_args = {key: sample_info[key] for key in action.extra_args}
-                if action.returns_labels:
-                    x, labels = action.go(x, **extra_args)
-                    sample_info["_labels"] = labels
-                else:
-                    x = action.go(x, **extra_args)
-                if trace:  # if tracing, add the output of the action to the trace
-                    sample_info["_trace"][k] = x
+
+                # perform the action (modifies the AudioSample in-place)
+                action.go(sample)
+
+                if trace:  # user requested record of preprocessing steps
+                    # save the current state of the sample's data
+                    # (trace is a Series with index matching self.pipeline)
+                    try:
+                        sample.trace[k] = copy.deepcopy(sample.data)
+                    # this will fail on Spectrogram and Audio class, which are immutable, implemented by
+                    # raising an AttributeError if .__setattr__ is called. Since deepcopy calls setattr,
+                    # we can't deepcopy those. As a temporary fix, we can add the original object because
+                    # it is immutable. However, we should re-factor immmutable classes to avoid this issue
+                    # (see Issue #671)
+                    except AttributeError:
+                        sample.trace[k] = sample.data
+
         except Exception as exc:
             # treat any exceptions raised during forward as PreprocessingErrors
             raise PreprocessingError(
-                f"failed to preprocess sample from path: {label_df_row.name}"
+                f"failed to preprocess sample from path: {sample.source}"
             ) from exc
 
-        return x, sample_info
+        # remove temporary attributes from sample
+        del sample.preprocessor, sample.target_duration
+        return sample
+
+    def _generate_sample(self, sample):
+        """create AudioSample object from initial input (file path)
+
+        can override this method is subclasses to modify how samples
+        are created, or to add additional attributes to samples
+        """
+        # handle paths or pd.Series as input for `sample`
+        if type(sample) == str or issubclass(type(sample), Path):
+            sample = AudioSample(sample)  # initialize with source = file path
+        else:
+            assert isinstance(sample, AudioSample), (
+                "sample must be AudioSample OR file path (str or pathlib.Path), "
+                f"was {type(sample)}"
+            )
+
+        # add attributes to the sample that might be needed by actions in the pipeline
+        sample.preprocessor = self
+        sample.target_duration = self.sample_duration
+
+        return sample
 
     def _insert_action_before(self, idx, name, value):
         """insert an item before a spcific index in a series"""
         i = list(self.pipeline.index).index(idx)
         part1 = self.pipeline[0:i]
         part2 = self.pipeline[i:]
         self.pipeline = part1.append(pd.Series([value], index=[name])).append(part2)
@@ -207,19 +203,19 @@
         part2 = self.pipeline[i + 1 :]
         self.pipeline = part1.append(pd.Series([value], index=[name])).append(part2)
 
 
 class SpectrogramPreprocessor(BasePreprocessor):
     """Child of BasePreprocessor that creates specrogram Tensors w/augmentation
 
-    loads audio, creates spectrogram, performs augmentations, returns tensor
+    loads audio, creates spectrogram, performs augmentations, creates tensor
 
     by default, does not resample audio, but bandpasses to 0-11.025 kHz
     (to ensure all outputs have same scale in y-axis)
-    can change with .load_audio.set(sample_rate=sr)
+    can change with .pipeline.bandpass.set(min_f=,max_f=)
 
     during prediction, will load clips from long audio files rather than entire
     audio files.
 
     Args:
         sample_duration:
             length in seconds of audio samples generated
@@ -231,33 +227,29 @@
         out_shape:
             output shape of tensor h,w,channels [default: (224,224,3)]
     """
 
     def __init__(self, sample_duration, overlay_df=None, out_shape=(224, 224, 3)):
 
         super(SpectrogramPreprocessor, self).__init__(sample_duration=sample_duration)
+        self.out_shape = out_shape
 
         # define a default set of Actions
         self.pipeline = pd.Series(
             {
                 "load_audio": AudioClipLoader(),
                 # if we are augmenting and get a long file, take a random trim from it
                 "random_trim_audio": AudioTrim(is_augmentation=True, random_trim=True),
                 # otherwise, we expect to get the correct duration. no random trim
                 "trim_audio": AudioTrim(),  # trim or extend (w/silence) clips to correct length
                 "to_spec": Action(Spectrogram.from_audio),
                 "bandpass": Action(
                     Spectrogram.bandpass, min_f=0, max_f=11025, out_of_bounds_ok=False
                 ),
-                "to_img": Action(
-                    Spectrogram.to_image,
-                    shape=out_shape[0:2],
-                    channels=out_shape[2],
-                    return_type="torch",
-                ),
+                "to_tensor": SpectrogramToTensor(),  # uses sample.target_shape
                 "overlay": Overlay(
                     is_augmentation=True, overlay_df=overlay_df, update_labels=False
                 )
                 if overlay_df is not None
                 else None,
                 "time_mask": Action(actions.time_mask, is_augmentation=True),
                 "frequency_mask": Action(actions.frequency_mask, is_augmentation=True),
@@ -270,7 +262,15 @@
                 ),
             }
         )
 
         # remove overlay if overlay_df was not specified
         if overlay_df is None:
             self.pipeline.drop("overlay", inplace=True)
+
+    def _generate_sample(self, sample):
+        """add the target_shape attribute to the sample
+        otherwise, generate AudioSamples from paths as normal
+        """
+        sample = super()._generate_sample(sample)
+        sample.target_shape = self.out_shape
+        return sample
```

### Comparing `opensoundscape-0.8.0/opensoundscape/preprocess/tensor_augment.py` & `opensoundscape-0.9.0/opensoundscape/preprocess/tensor_augment.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/preprocess/utils.py` & `opensoundscape-0.9.0/opensoundscape/preprocess/utils.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/resources/species_table.csv` & `opensoundscape-0.9.0/opensoundscape/resources/species_table.csv`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/ribbit.py` & `opensoundscape-0.9.0/opensoundscape/ribbit.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import os
 import warnings
 
 from scipy import signal
 import numpy as np
 
-from opensoundscape.helpers import generate_clip_times_df
+from opensoundscape.utils import generate_clip_times_df
 
 
 def calculate_pulse_score(
     amplitude, amplitude_sample_rate, pulse_rate_range, plot=False, nfft=1024
 ):
     """Search for amplitude pulsing in an audio signal in a range of pulse repetition rates (PRR)
```

### Comparing `opensoundscape-0.8.0/opensoundscape/signal_processing.py` & `opensoundscape-0.9.0/opensoundscape/signal_processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Signal processing tools for feature extraction and more"""
 import numpy as np
 import pandas as pd
 from scipy import signal
 import pywt
 import matplotlib.pyplot as plt
 from pywt import central_frequency
+from scipy.signal import correlation_lags, correlate as scipy_correlate
+from scipy.fft import next_fast_len
+import torch
 
-from opensoundscape.helpers import inrange
+from opensoundscape.utils import inrange
 
 
 def frequency2scale(frequency, wavelet, sample_rate):
     """determine appropriate wavelet scale for desired center frequency
 
     Args:
         frequency: desired center frequency of wavelet in Hz (1/seconds)
@@ -451,7 +454,155 @@
     """
     if normalize:
         x = x / np.max(x)
     x_01 = (np.array(x) >= threshold).astype(int)
     starts, lengths = _get_ones_sequences(x_01)
 
     return np.array(starts) / sample_rate, np.array(lengths) / sample_rate
+
+
+def gcc(x, y, cc_filter="phat", epsilon=0.001, radius=None):
+    """
+    Generalized cross correlation of two signals
+
+    Computes a generalized cross correlation in frequency response.
+
+    The generalized cross correlation algorithm described in Knapp and Carter [1].
+
+    In the case of cc_filter='cc', gcc simplifies to cross correlation and is equivalent to
+    scipy.signal.correlate and numpy.correlate.
+
+    code adapted from github.com/axeber01/ngcc
+
+    Args:
+        x: 1d numpy array of audio samples
+        y: 1d numpy array of audio samples
+        cc_filter: which filter to use in the gcc.
+            'phat' - Phase transform. Default.
+            'roth' -
+            'scot' - Smoothed Coherence Transform,
+            'ht' - Hannan and Thomson
+            'cc' - normal cross correlation with no filter
+        epsilon: small value used to ensure denominator when applying a filter is non-zero.
+
+    Returns:
+        gcc: 1d numpy array of gcc values
+
+    see also: tdoa() uses this function to estimate time delay between two signals
+
+    [1] Knapp, C.H. and Carter, G.C (1976)
+    The Generalized Correlation Method for Estimation of Time Delay. IEEE Trans. Acoust. Speech Signal Process, 24, 320-327.
+    http://dx.doi.org/10.1109/TASSP.1976.1162830
+    """
+    # using torch speeds up our performance
+    x = torch.Tensor(x)
+    y = torch.Tensor(y)
+
+    # pad the fft shape for "full" cross correlation of both signals
+    n = x.shape[0] + y.shape[0] - 1
+    if n % 2 != 0:
+        n += 1
+    # by choosing an optimal length rather than the shortest possible, we can
+    # optimize fft speed
+    n_fast = next_fast_len(n, real=True)
+
+    # Take the reall Fast Fourier Transform of the signals
+    X = torch.fft.rfft(x, n=n_fast)
+    Y = torch.fft.rfft(y, n=n_fast)
+
+    # multiply one by the complex conjugate of the other
+    Gxy = X * torch.conj(Y)
+
+    # Apply the filter in the fourier domain
+    if cc_filter == "phat":
+        phi = 1 / (torch.abs(Gxy) + epsilon)
+
+    elif cc_filter == "roth":
+        phi = 1 / (X * torch.conj(X) + epsilon)
+
+    elif cc_filter == "scot":
+        Gxx = X * torch.conj(X)
+        Gyy = Y * torch.conj(Y)
+        phi = 1 / (torch.sqrt(Gxx * Gyy) + epsilon)
+
+    elif cc_filter == "ht":
+        Gxx = X * torch.conj(X)
+        Gyy = Y * torch.conj(Y)
+        gamma_xy = Gxy / (torch.sqrt(Gxx * Gyy) + epsilon)
+        coherence = torch.abs(gamma_xy) ** 2
+        phi = coherence / (torch.abs(Gxy) * (1 - coherence) + epsilon)
+    elif cc_filter == "cc":
+        phi = 1.0
+    else:
+        raise ValueError(
+            "Unsupported cc_filter. Must be one of: 'ht', 'phat', 'roth','scot'"
+        )
+    # Inverse FFT to get the GCC
+    cc = torch.fft.irfft(Gxy * phi, n_fast)
+
+    # reorder the cross-correlation coefficients, trimming out padded regions
+    # order of outputs matches torch.correlate and scipy.signal.correlate
+    cc = torch.concatenate((cc[-y.shape[0] + 1 :], cc[: x.shape[0]]))
+
+    return cc.numpy()
+
+
+def tdoa(
+    signal,
+    reference_signal,
+    cc_filter="phat",
+    sample_rate=1,
+    return_max=False,
+    max_delay=None,
+):
+    """estimate time difference of arrival between two signals
+
+    estimates time delay by finding the maximum of the generalized cross correlation (gcc)
+    of two signals. The two signals are discrete-time series with the same sample rate.
+
+    For example, if the signal arrives 2.5 seconds _after_ the reference signal, returns 2.5;
+    if it arrives 0.5 seconds _before_ the reference signal, returns -0.5.
+
+    Args:
+        signal, reference_signal: np.arrays or lists containing each signal
+        cc_filter: see gcc()
+        sample_rate: sample rate (Hz) of signals; both signals must have same sample rate
+        return_max: if True, returns the maximum value of the generalized cross correlation
+        max_delay: maximum possible tdoa. Cross-correlations that correspond to time delays outside of this range are ignored.
+            For example, if max_delay=0.5, the tdoa returned will be the delay between -0.5 and +0.5 seconds, that maximizes the cross-correlation.
+            This is useful if you know the maximum possible delay between the two signals, and want to ignore any tdoas outside of that range.
+            e.g. if receivers are 100m apart, and the speed of sound is 340m/s, then the maximum possible delay is 0.294 seconds.
+    Returns:
+        estimated delay from reference signal to signal, in seconds
+        (note that default samping rate is 1.0 samples/second)
+
+        if return_max is True, returns a second value, the maximum value of the
+        result of generalized cross correlation
+
+    See also: gcc() if you want the raw output of generalized cross correlation
+    """
+    # compute the generalized cross correlation between the signals
+    cc = gcc(signal, reference_signal, cc_filter=cc_filter)
+
+    # generate the relative offsets for each index position of `cc`
+    lags = correlation_lags(len(signal), len(reference_signal))
+
+    if max_delay:
+        max_lag = int(
+            max_delay * sample_rate
+        )  # convert max_delay to max_lag in samples
+        # slice cc and lags, so we only look at cross_correlations that are between -max_lag and +max_lag
+        boolean_mask = [lag < max_lag and lag > -max_lag for lag in lags]
+        cc = cc[boolean_mask]
+        lags = lags[boolean_mask]
+
+    # find the time delay using the index of the maximum cc value
+    # the maximum of the cc value represents GCC's estimate of the delay
+    # between the two signals, ie how much to shift one signal against the other
+    # to maximize their product
+    tdoa = lags[np.argmax(cc)] / sample_rate
+
+    if return_max:
+        return tdoa, max(cc)
+
+    else:
+        return tdoa
```

### Comparing `opensoundscape-0.8.0/opensoundscape/spectrogram.py` & `opensoundscape-0.9.0/opensoundscape/spectrogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from PIL import Image
 import torch
 from matplotlib import pyplot as plt
 from matplotlib.cm import get_cmap
 import matplotlib.colors
 
 from opensoundscape.audio import Audio
-from opensoundscape.helpers import min_max_scale, linear_scale
+from opensoundscape.utils import min_max_scale, linear_scale
 
 
 class Spectrogram:
     """Immutable spectrogram container
 
     Can be initialized directly from spectrogram, frequency, and time values or created from an
     Audio object using the .from_audio() method.
@@ -739,15 +739,15 @@
             scaling=scaling,
         )
 
         # choose n_fft to ensure filterbank.size[1]==spectrogram.size[0]
         n_fft = int(linear_spec.spectrogram.shape[0] - 1) * 2
         # Construct mel filter bank
         filter_bank = librosa.filters.mel(
-            audio.sample_rate, n_fft, n_mels=n_mels, norm=norm, htk=htk
+            sr=audio.sample_rate, n_fft=n_fft, n_mels=n_mels, norm=norm, htk=htk
         )
         # normalize filter bank: rows should sum to 1 #TODO: is this correct?
         fb_constant = np.sum(filter_bank, 1).mean()
         filter_bank = filter_bank / fb_constant
 
         # Apply filter bank to spectrogram with matrix multiplication
         melspectrogram = np.dot(filter_bank, linear_spec.spectrogram)
```

### Comparing `opensoundscape-0.8.0/opensoundscape/taxa.py` & `opensoundscape-0.9.0/opensoundscape/taxa.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/torch/architectures/cnn_architectures.py` & `opensoundscape-0.9.0/opensoundscape/ml/cnn_architectures.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 opensoundscape.torch.models.cnn.
 """
 import warnings
 
 from torchvision import models
 from torch import nn
 import torch
-import torchvision
 from torchvision.models.inception import BasicConv2d
 
 ARCH_DICT = dict()
 
+# inspiration from zhmiao/BirdMultiLabel
+import torch.nn as nn
+
 
 def register_arch(func):
     """add architecture to ARCH_DICT"""
     # register the model in dictionary
     ARCH_DICT[func.__name__] = func
     # return the function
     return func
@@ -86,14 +88,17 @@
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
     architecture_ft.conv1 = change_conv2d_channels(architecture_ft.conv1, num_channels)
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layer4]
+
     return architecture_ft
 
 
 @register_arch
 def resnet34(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -120,14 +125,17 @@
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
     architecture_ft.conv1 = change_conv2d_channels(architecture_ft.conv1, num_channels)
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layer4]
+
     return architecture_ft
 
 
 @register_arch
 def resnet50(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -154,14 +162,17 @@
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
     architecture_ft.conv1 = change_conv2d_channels(architecture_ft.conv1, num_channels)
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layer4]
+
     return architecture_ft
 
 
 @register_arch
 def resnet101(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -188,14 +199,17 @@
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
     architecture_ft.conv1 = change_conv2d_channels(architecture_ft.conv1, num_channels)
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layer4]
+
     return architecture_ft
 
 
 @register_arch
 def resnet152(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -226,14 +240,17 @@
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
     architecture_ft.conv1 = change_conv2d_channels(architecture_ft.conv1, num_channels)
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layer4]
+
     return architecture_ft
 
 
 @register_arch
 def alexnet(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -264,14 +281,17 @@
     )
 
     # change input shape num_channels
     architecture_ft.features[0] = change_conv2d_channels(
         architecture_ft.features[0], num_channels
     )
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.features[-1]]
+
     return architecture_ft
 
 
 @register_arch
 def vgg11_bn(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -302,14 +322,17 @@
     )
 
     # change input shape num_channels
     architecture_ft.features[0] = change_conv2d_channels(
         architecture_ft.features[0], num_channels
     )
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.features[-1]]
+
     return architecture_ft
 
 
 @register_arch
 def squeezenet1_0(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -351,14 +374,17 @@
     )
 
     # change input shape num_channels
     architecture_ft.features[0] = change_conv2d_channels(
         architecture_ft.features[0], num_channels
     )
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.features[-1]]
+
     return architecture_ft
 
 
 @register_arch
 def densenet121(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -388,14 +414,17 @@
     )
 
     # change input shape num_channels
     architecture_ft.features[0] = change_conv2d_channels(
         architecture_ft.features[0], num_channels
     )
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.features[-1]]
+
     return architecture_ft
 
 
 @register_arch
 def inception_v3(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -434,14 +463,18 @@
             "number of input channels is not implemented. First conv2d will "
             "have random weights."
         )
 
         architecture_ft.Conv2d_1a_3x3 = BasicConv2d(
             num_channels, 32, kernel_size=3, stride=2
         )
+
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.Mixed_7c]
+
     return architecture_ft
 
 
 @register_arch
 def efficientnet_b0(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -478,14 +511,17 @@
     )
 
     # change input shape num_channels
     architecture_ft.stem.conv = change_conv2d_channels(
         architecture_ft.stem.conv, num_channels
     )
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layers[-1][-1]]
+
     return architecture_ft
 
 
 @register_arch
 def efficientnet_b4(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -522,14 +558,17 @@
     )
 
     # change input shape num_channels
     architecture_ft.stem.conv = change_conv2d_channels(
         architecture_ft.stem.conv, num_channels
     )
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layers[-1][-1]]
+
     return architecture_ft
 
 
 @register_arch
 def efficientnet_widese_b0(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -566,14 +605,17 @@
     )
 
     # change input shape num_channels
     architecture_ft.stem.conv = change_conv2d_channels(
         architecture_ft.stem.conv, num_channels
     )
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layers[-1][-1]]
+
     return architecture_ft
 
 
 @register_arch
 def efficientnet_widese_b4(
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
@@ -610,14 +652,17 @@
     )
 
     # change input shape num_channels
     architecture_ft.stem.conv = change_conv2d_channels(
         architecture_ft.stem.conv, num_channels
     )
 
+    # default target layers for activation maps like GradCAM and guided backpropagation
+    architecture_ft.cam_target_layers = [architecture_ft.layers[-1][-1]]
+
     return architecture_ft
 
 
 def change_conv2d_channels(
     conv2d,
     num_channels=3,
     reuse_weights=True,
```

### Comparing `opensoundscape-0.8.0/opensoundscape/torch/datasets.py` & `opensoundscape-0.9.0/opensoundscape/ml/datasets.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import copy
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import torch
 
-from opensoundscape.helpers import make_clip_df
+from opensoundscape.utils import make_clip_df
+from opensoundscape.sample import AudioSample
 
 
 class AudioFileDataset(torch.utils.data.Dataset):
     """Base class for audio datasets with OpenSoundscape (use in place of torch Dataset)
 
     Custom Dataset classes should subclass this class or its children.
 
@@ -31,31 +32,27 @@
              - df must have audio paths in the index.
              - If label_df has labels, the class names should be the columns, and
             the values of each row should be 0 or 1.
              - If data does not have labels, label_df will have no columns
         preprocessor:
             an object of BasePreprocessor or its children which defines
             the operations to perform on input samples
-        return_labels:
-            if True, the __getitem__ method will return {X:sample,y:labels}
-            If False, the __getitem__ method will return {X:sample}
-            If label_df has no labels (no columns), use return_labels=False
-            [default: True]
+
+    Returns:
+        sample (AudioSample object)
 
     Raises:
         PreprocessingError if exception is raised during __getitem__
 
     Effects:
         self.invalid_samples will contain a set of paths that did not successfully
             produce a list of clips with start/end times, if split_files_into_clips=True
     """
 
-    def __init__(
-        self, samples, preprocessor, return_labels=True, bypass_augmentations=False
-    ):
+    def __init__(self, samples, preprocessor, bypass_augmentations=False):
 
         ## Input Validation ##
 
         # validate type of samples: list, np array, or df
         assert type(samples) in (list, np.ndarray, pd.DataFrame,), (
             f"samples must be type list/np.ndarray of file paths, "
             f"or pd.DataFrame with index containing path (or multi-index of "
@@ -79,55 +76,44 @@
         if len(df) > 0:
             first_path = df.index[0][0] if self.has_clips else df.index[0]
             if not Path(first_path).exists():
                 warnings.warn(
                     "Index of dataframe passed to "
                     f"preprocessor must be a file path. First sample {df.index[0]} was not found."
                 )
-        if return_labels and len(df.columns) == 0:
-            warnings.warn("return_labels=True but df has no columns!")
-        elif len(df) > 0 and return_labels and not df.values[0, 0] in (0, 1):
-            warnings.warn(
-                "if return_labels=True, label_df must have labels that take values of 0 and 1"
-            )
+        elif len(df) > 0 and len(df.columns) > 0 and not df.values[0, 0] in (0, 1):
+            warnings.warn("if label_df has labels, they must take values of 0 and 1")
 
         if len(df) == 0:
             warnings.warn("Zero samples!")
 
         self.classes = df.columns
         self.label_df = df
-        self.return_labels = return_labels
         self.preprocessor = preprocessor
         self.invalid_samples = set()
 
         # if True skips Actions with .is_augmentation=True
         self.bypass_augmentations = bypass_augmentations
 
     def __len__(self):
         return self.label_df.shape[0]
 
     def __getitem__(self, idx, break_on_key=None, break_on_type=None):
 
-        label_df_row = self.label_df.iloc[idx]
+        sample = AudioSample.from_series(self.label_df.iloc[idx])
 
         # preprocessor.forward will raise PreprocessingError if something fails
-        # the preprocessor handles label_df_row having index of file or (file,start_time,end_time)
-        x, sample_info = self.preprocessor.forward(
-            label_df_row,
+        sample = self.preprocessor.forward(
+            sample,
             bypass_augmentations=self.bypass_augmentations,
             break_on_key=break_on_key,
             break_on_type=break_on_type,
         )
 
-        # Return sample & label pairs (training/validation)
-        if self.return_labels:
-            labels = torch.from_numpy(sample_info["_labels"].values)
-            return {"X": x, "y": labels}
-        else:  # Return sample only (prediction)
-            return {"X": x}
+        return sample
 
     def __repr__(self):
         return f"{self.__class__} object with preprocessor: {self.preprocessor}"
 
     def class_counts(self):
         """count number of each label"""
         labels = self.label_df.columns
@@ -168,21 +154,25 @@
 class AudioSplittingDataset(AudioFileDataset):
     """class to load clips of longer files rather than one sample per file
 
     Internally creates even-lengthed clips split from long audio files.
 
     If file labels are provided, applies copied labels to all clips from a file
 
+    NOTE: If you've already created a dataframe with clip start and end times,
+    you can use AudioFileDataset. This class is only necessary if you wish to
+    automatically split longer files into clips (providing only the file paths).
+
     Args:
         see AudioFileDataset and make_clip_df
     """
 
     def __init__(self, samples, preprocessor, overlap_fraction=0, final_clip=None):
         super(AudioSplittingDataset, self).__init__(
-            samples=samples, preprocessor=preprocessor, return_labels=False
+            samples=samples, preprocessor=preprocessor
         )
 
         self.has_clips = True
 
         # create clip df
         # self.label_df will have multi-index (file,start_time,end_time)
         # can contain rows with start/end time np.nan for failed samples
```

### Comparing `opensoundscape-0.8.0/opensoundscape/torch/loss.py` & `opensoundscape-0.9.0/opensoundscape/ml/loss.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/torch/models/cnn.py` & `opensoundscape-0.9.0/opensoundscape/ml/cnn.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,34 +15,41 @@
 
 import torch
 import torch.optim as optim
 import torch.nn.functional as F
 from torch.utils.data import DataLoader
 
 import opensoundscape
-from opensoundscape.torch.architectures import cnn_architectures
-from opensoundscape.torch.models.utils import (
+from opensoundscape.ml import cnn_architectures
+from opensoundscape.ml.utils import (
     BaseModule,
     apply_activation_layer,
 )
 from opensoundscape.preprocess.preprocessors import SpectrogramPreprocessor
-from opensoundscape.torch.loss import (
+from opensoundscape.ml.loss import (
     BCEWithLogitsLoss_hot,
     CrossEntropyLoss_hot,
     ResampleLoss,
 )
-from opensoundscape.torch.safe_dataset import SafeDataset
-from opensoundscape.torch.datasets import AudioFileDataset, AudioSplittingDataset
-from opensoundscape.torch.architectures.cnn_architectures import inception_v3
+from opensoundscape.ml.safe_dataset import SafeDataset
+from opensoundscape.ml.datasets import AudioFileDataset, AudioSplittingDataset
+from opensoundscape.ml.cnn_architectures import inception_v3
 from opensoundscape.metrics import (
     predict_multi_target_labels,
     predict_single_target_labels,
     single_target_metrics,
     multi_target_metrics,
 )
+from opensoundscape.sample import collate_samples
+from opensoundscape.utils import identity
+from opensoundscape.logging import wandb_table
+
+from opensoundscape.ml.cam import CAM
+import pytorch_grad_cam
+from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
 
 
 class CNN(BaseModule):
     """
     Generic CNN Model with .train(), .predict(), and .save()
 
     flexible architecture, optimizer, loss function, parameters
@@ -63,15 +70,15 @@
             list of class names. Must match with training dataset classes if training.
         single_target:
             - True: model expects exactly one positive class per sample
             - False: samples can have any number of positive classes
             [default: False]
         preprocessor_class: class of Preprocessor object
         sample_shape: tuple of height, width, channels for created sample
-            [default: (224,224,3)]
+            [default: (224,224,3)] #TODO: consider changing to (ch,h,w) to match torchww
 
     """
 
     def __init__(
         self,
         architecture,
         classes,
@@ -86,24 +93,32 @@
         self.name = "CNN"
 
         # model characteristics
         self.current_epoch = 0
         self.classes = classes
         self.single_target = single_target  # if True: predict only class w max score
         self.opensoundscape_version = opensoundscape.__version__
+
         # number of samples to preprocess and log to wandb during train/predict
         self.wandb_logging = dict(
             n_preview_samples=8,  # before train/predict, log n random samples
             top_samples_classes=None,  # specify list of classes to see top samples from
             n_top_samples=3,  # after prediction, log n top scoring samples per class
+            # logs histograms of params & grads every n batches;
+            watch_freq=10,  # use  None for no logging of params & grads
         )
         self.loss_fn = None
         self.train_loader = None
         self.scheduler = None
 
+        # to use a custom DataLoader or Sampler, change these attributes
+        # to the custom class (init must take same arguments)
+        self.train_dataloader_cls = DataLoader
+        self.inference_dataloader_cls = DataLoader
+
         ### architecture ###
         # can be a pytorch CNN such as Resnet18 or a custom object
         # must have .forward(), .train(), .eval(), .to(), .state_dict()
         # for convenience, also allows user to provide string matching
         # a key from cnn_architectures.ARCH_DICT
         num_channels = sample_shape[2]
         if type(architecture) == str:
@@ -135,14 +150,15 @@
         # devices could be 'cuda:0', torch.device('cuda'), torch.device('cpu')
         if torch.cuda.is_available():
             self.device = torch.device("cuda")
         else:
             self.device = torch.device("cpu")
 
         ### sample loading/preprocessing ###
+        # preprocessor will have attributes .sample_duration and .out_shape
         self.preprocessor = preprocessor_class(
             sample_duration=sample_duration, out_shape=sample_shape
         )
 
         ### loss function ###
         if self.single_target:  # use cross entropy loss by default
             self.loss_cls = CrossEntropyLoss_hot
@@ -210,29 +226,14 @@
         """initialize an instance of self.loss_cls
 
         This function is called during .train() so that the user
         has a chance to change the loss function before training.
         """
         self.loss_fn = self.loss_cls()
 
-    def _init_dataloader(
-        self, safe_dataset, batch_size=64, num_workers=1, shuffle=False
-    ):
-        """initialize dataloader for training
-
-        Override this function to use a different DataLoader or sampler
-        """
-        return DataLoader(
-            safe_dataset,
-            batch_size=batch_size,
-            shuffle=shuffle,
-            num_workers=num_workers,
-            pin_memory=True,
-        )
-
     def _set_train(self, train_df, batch_size, num_workers, raise_errors):
         """Prepare network for training on train_df
 
         Args:
             batch_size: number of training files to load/process before
                         re-calculating the loss function and backpropagation
             num_workers: parallelization (number of cores or cpus)
@@ -259,19 +260,22 @@
         # indices of bad samples are appended to SafeDataset._invalid_indices
         invalid_sample_behavior = "raise" if raise_errors else "substitute"
         train_safe_dataset = SafeDataset(
             train_dataset, invalid_sample_behavior=invalid_sample_behavior
         )
 
         # train_loader samples batches of images + labels from training set
-        self.train_loader = self._init_dataloader(
+        self.train_loader = self.train_dataloader_cls(
             train_safe_dataset,
             batch_size=batch_size,
             num_workers=num_workers,
-            shuffle=True,
+            shuffle=True,  # SHUFFLE SAMPLES because we are training
+            # use pin_memory=True when loading files on CPU and training on GPU
+            pin_memory=False if self.device == torch.device("cpu") else True,
+            collate_fn=identity,
         )
 
         ###########################
         # Setup loss function     #
         ###########################
         self._init_loss_fn()
 
@@ -315,28 +319,31 @@
         self.network.train()
 
         total_tgts = []
         total_preds = []
         total_scores = []
         batch_loss = []
 
-        for batch_idx, batch_data in enumerate(train_loader):
+        for batch_idx, samples in enumerate(train_loader):
             # load a batch of images and labels from the train loader
             # all augmentation occurs in the Preprocessor (train_loader)
-            batch_tensors = batch_data["X"].to(self.device)
-            batch_labels = batch_data["y"].to(self.device)
+            # we collate here rather than in the DataLoader so that
+            # we can still access the AudioSamples and thier information
+            batch_data = collate_samples(samples)
+            batch_tensors = batch_data["samples"].to(self.device)
+            batch_labels = batch_data["labels"].to(self.device)
             if len(self.classes) > 1:  # squeeze one dimension [1,2] -> [1,1]
                 batch_labels = batch_labels.squeeze(1)
 
             ####################
             # Forward and loss #
             ####################
 
             # forward pass: feature extractor and classifier
-            logits = self.network.forward(batch_tensors)
+            logits = self.network(batch_tensors)
 
             # save targets and predictions
             total_scores.append(logits.detach().cpu().numpy())
             total_tgts.append(batch_labels.detach().cpu().numpy())
 
             # generate boolean predictions
             if self.single_target:  # predict highest scoring class only
@@ -420,17 +427,15 @@
 
         if "lr" in self.optimizer_params:
             wandb_config["learning_rate"] = self.optimizer_params["lr"]
         else:
             wandb_config["learning_rate"] = "n/a"
 
         try:
-            wandb_config["sample_shape"] = self.preprocessor.pipeline.to_img.params[
-                "shape"
-            ] + [self.preprocessor.pipeline.to_img.params["channels"]]
+            wandb_config["sample_shape"] = self.preprocessor.out_shape
         except:
             wandb_config["sample_shape"] = "n/a"
 
         return wandb_config
 
     def train(
         self,
@@ -547,30 +552,38 @@
                     lr_update_interval=self.lr_update_interval,
                     lr_cooling_factor=self.lr_cooling_factor,
                     optimizer_cls=self.optimizer_cls,
                     model_save_path=Path(save_path).resolve(),
                 )
             )
 
+            # use wandb.watch to log histograms of parameter and gradient values
+            # value of None for log_freq means do not use wandb.watch()
+            log_freq = self.wandb_logging["watch_freq"]
+            if log_freq is not None:
+                wandb_session.watch(
+                    self.network, log="all", log_freq=log_freq, log_graph=(True)
+                )
+
             # log tables of preprocessed samples
             wandb_session.log(
                 {
-                    "Samples / training samples w/augmentation": opensoundscape.wandb.wandb_table(
+                    "Samples / training samples": wandb_table(
                         AudioFileDataset(
                             train_df, self.preprocessor, bypass_augmentations=False
                         ),
                         self.wandb_logging["n_preview_samples"],
                     ),
-                    "Samples / training samples w/o augmentation": opensoundscape.wandb.wandb_table(
+                    "Samples / training samples no aug": wandb_table(
                         AudioFileDataset(
                             train_df, self.preprocessor, bypass_augmentations=True
                         ),
                         self.wandb_logging["n_preview_samples"],
                     ),
-                    "Samples / validation samples": opensoundscape.wandb.wandb_table(
+                    "Samples / validation samples": wandb_table(
                         AudioFileDataset(
                             validation_df, self.preprocessor, bypass_augmentations=True
                         ),
                         self.wandb_logging["n_preview_samples"],
                     ),
                 }
             )
@@ -717,33 +730,130 @@
         if self.single_target:
             score = metrics_dict["f1"]
         else:
             score = metrics_dict["map"]
 
         return score, metrics_dict
 
-    def save(self, path, save_train_loader=False):
+    def save(
+        self, path, save_train_loader=False, save_hooks=False, as_torch_dict=False
+    ):
         """save model with weights using torch.save()
 
         load from saved file with torch.load(path) or cnn.load_model(path)
 
+
+        Note: saving and loading model objects across OpenSoundscape versions
+        will not work properly. Instead, use .save_torch_dict and .load_torch_dict
+        (but note that customizations to preprocessing, training params, etc will
+        not be retained using those functions).
+
+        For maximum flexibilty in further use, save the model with both .save() and
+        .save_torch_dict()
+
         Args:
             path: file path for saved model object
             save_train_loader: retrain .train_loader in saved object
                 [default: False]
+            save_hooks: retain forward and backward hooks on modules
+                [default: False] Note: True can cause issues when using
+                wandb.watch()
         """
         os.makedirs(Path(path).parent, exist_ok=True)
+
+        # save a pickled model object; will not work across opso versions
         model_copy = copy.deepcopy(self)
+
         if not save_train_loader:
             try:
                 delattr(model_copy, "train_loader")
             except AttributeError:
                 pass
+
+        if not save_hooks:
+            # remove all forward and backward hooks on network.modules()
+            from collections import OrderedDict
+
+            for m in model_copy.network.modules():
+                m._forward_hooks = OrderedDict()
+                m._backward_hooks = OrderedDict()
+
         torch.save(model_copy, path)
 
+    def save_torch_dict(self, path):
+        """save model to file for use in other opso versions
+
+         WARNING: this does not save any preprocessing or augmentation
+            settings or parameters, or other attributes such as the training
+            parameters or loss function. It only saves architecture, weights,
+            classes, sample shape, sample duration, and single_target.
+
+        To save the entire pickled model object (recover all parameters and
+        settings), use model.save() instead. Note that models saved with
+        model.save() will not work across different versions of OpenSoundscape.
+
+        To recreate the model after saving with this function, use CNN.from_torch_dict(path)
+
+        Args:
+            path: file path for saved model object
+
+        Effects:
+            saves a file using torch.save() containing model weights and other information
+        """
+
+        # warn the user if the achirecture can't be re-created from the
+        # string name (self.architecture_name)
+        if not self.architecture_name in cnn_architectures.list_architectures():
+            warnings.warn(
+                f"""\n The value of `self.architecture_name` ({self.architecture_name})
+                    is not an architecture that can be generated in OpenSoundscape. Using
+                    CNN.from_torch_dict on the saved file will cause an error. To fix this,
+                    you can use .save() instead of .save_torch_model, or change 
+                    `self.architecture_name` to one of the architecture name strings listed by 
+                    opensoundscape.torch.architectures.cnn_architectures.list_architectures()
+                    if this architecture is supported."""
+            )
+
+        os.makedirs(Path(path).parent, exist_ok=True)
+
+        # save just the basics, loses preprocessing/other settings
+        torch.save(
+            {
+                "weights": self.network.state_dict(),
+                "classes": self.classes,
+                "architecture": self.architecture_name,
+                "sample_duration": self.preprocessor.sample_duration,
+                "single_target": self.single_target,
+                "sample_shape": self.preprocessor.out_shape,
+            },
+            path,
+        )
+
+    @classmethod
+    def from_torch_dict(cls, path):
+        """load a model saved using CNN.save_torch_dict()
+
+        Args:
+            path: path to file saved using CNN.save_torch_dict()
+
+        Returns:
+            new CNN instance
+
+        Note: if you used .save() instead of .save_torch_dict(), load
+        the model using cnn.load_model(). Note that the model object will not load properly
+        across different versions of OpenSoundscape. To save and load models across
+        different versions of OpenSoundscape, use .save_torch_dict(), but note that
+        preprocessing and other customized settings will not be retained.
+        """
+        model_dict = torch.load(path)
+        state_dict = model_dict.pop("weights")
+        model = cls(**model_dict)
+        model.network.load_state_dict(state_dict)
+        return model
+
     def save_weights(self, path):
         """save just the weights of the network
 
         This allows the saved weights to be used more flexibly than model.save()
         which will pickle the entire object. The weights are saved in a pickled
         dictionary using torch.save(self.network.state_dict())
 
@@ -760,14 +870,111 @@
 
         Args:
             path: file path with saved weights
             strict: (bool) see torch.load()
         """
         self.network.load_state_dict(torch.load(path), strict=strict)
 
+    def _init_inference_dataloader(
+        self,
+        samples,
+        split_files_into_clips=True,
+        overlap_fraction=0,
+        final_clip=None,
+        bypass_augmentations=True,
+        batch_size=1,
+        num_workers=0,
+        raise_errors=False,
+    ):
+        """Create DataLoader for inference
+
+        During inference, we allow the user to pass any of 3 things to samples:
+        - list of file paths
+        - Dataframe with file as index
+        - Dataframe with file, start_time, end_time of clips as index
+
+        If file as index, default split_files_into_clips=True means that it will
+        automatically determine the number of clips that can be created from the file
+        (with overlap between subsequent clips based on overlap_fraction)
+
+        Returns:
+            DataLoader that creates lists of AudioSample objects
+        """
+        assert type(samples) in (list, np.ndarray, pd.DataFrame), (
+            "`samples` must be either: "
+            "(a) list or np.array of files, or DataFrame with (b) file as Index or "
+            "(c) (file,start_time,end_time) as MultiIndex"
+        )
+
+        # set up prediction Dataset, considering three possible cases:
+        # (c1) user provided multi-index df with file,start_time,end_time of clips
+        # (c2) user provided file list and wants clips to be split out automatically
+        # (c3) split_files_into_clips=False -> one sample & one prediction per file provided
+        if type(samples) == pd.DataFrame and type(samples.index) == MultiIndex:  # c1
+            prediction_dataset = AudioFileDataset(
+                samples=samples, preprocessor=self.preprocessor
+            )
+        elif split_files_into_clips:  # c2
+            prediction_dataset = AudioSplittingDataset(
+                samples=samples,
+                preprocessor=self.preprocessor,
+                overlap_fraction=overlap_fraction,
+                final_clip=final_clip,
+            )
+        else:  # c3
+            prediction_dataset = AudioFileDataset(
+                samples=samples, preprocessor=self.preprocessor
+            )
+        prediction_dataset.bypass_augmentations = bypass_augmentations
+
+        ## Input Validation ##
+        if len(prediction_dataset.classes) > 0 and list(self.classes) != list(
+            prediction_dataset.classes
+        ):
+            warnings.warn(
+                "The columns of input samples df differ from `model.classes`."
+            )
+
+        if len(prediction_dataset) < 1:
+            warnings.warn(
+                "prediction_dataset has zero samples. No predictions will be generated."
+            )
+            prediction_dataset = AudioFileDataset(
+                samples=[], preprocessor=self.preprocessor
+            )
+
+        # If unsafe_behavior= "substitute", a SafeDataset will not fail on bad files,
+        # but will provide a different sample! Later we go back and replace scores
+        # with np.nan for the bad samples (using safe_dataset._invalid_indices)
+        # this approach to error handling feels hacky
+        # however, returning None would break the batching of samples
+        # "raise" behavior will raise exceptions
+        invalid_sample_behavior = "raise" if raise_errors else "substitute"
+
+        safe_dataset = SafeDataset(
+            prediction_dataset, invalid_sample_behavior=invalid_sample_behavior
+        )
+
+        # initialize the dataloader
+        dataloader = self.inference_dataloader_cls(
+            safe_dataset,
+            batch_size=batch_size,
+            num_workers=num_workers,
+            shuffle=False,  # DONT CHANGE the order of samples during inference!
+            # use pin_memory=True when loading files on CPU and training on GPU
+            pin_memory=False if self.device == torch.device("cpu") else True,
+            collate_fn=identity,
+        )
+        # add any paths that failed to generate a clip df to _invalid_samples
+        dataloader.dataset._invalid_samples = dataloader.dataset._invalid_samples.union(
+            prediction_dataset.invalid_samples
+        )
+
+        return dataloader
+
     def predict(
         self,
         samples,
         batch_size=1,
         num_workers=0,
         activation_layer=None,
         split_files_into_clips=True,
@@ -810,15 +1017,15 @@
                 [default: None]
             split_files_into_clips:
                 If True, internally splits and predicts on clips from longer audio files
                 Otherwise, assumes each row of `samples` corresponds to one complete sample
             overlap_fraction: fraction of overlap between consecutive clips when
                 predicting on clips of longer audio files. For instance, 0.5
                 gives 50% overlap between consecutive clips.
-            final_clip: see `opensoundscape.helpers.generate_clip_times_df`
+            final_clip: see `opensoundscape.utils.generate_clip_times_df`
             bypass_augmentations: If False, Actions with
                 is_augmentation==True are performed. Default True.
             invalid_samples_log: if not None, samples that failed to preprocess
                 will be listed in this text file.
             raise_errors:
                 if True, raise errors when preprocessing fails
                 if False, just log the errors to unsafe_samples_log
@@ -848,78 +1055,25 @@
             If unsafe_samples_log is not None, saves a list of all file paths that
             failed to preprocess in unsafe_samples_log as a text file
 
         Note: if loading an audio file raises a PreprocessingError, the scores
             for that sample will be np.nan
 
         """
-        assert type(samples) in (list, np.ndarray, pd.DataFrame), (
-            "`samples` must be either: "
-            "(a) list or np.array of files, or DataFrame with (b) file as Index or "
-            "(c) (file,start_time,end_time) as MultiIndex"
-        )
 
-        # set up prediction Dataset, considering three possible cases:
-        # (c1) user provided multi-index df with file,start_time,end_time of clips
-        # (c2) user provided file list and wants clips to be split out automatically
-        # (c3) split_files_into_clips=False -> one sample & one prediction per file provided
-        if type(samples) == pd.DataFrame and type(samples.index) == MultiIndex:  # c1
-            prediction_dataset = AudioFileDataset(
-                samples=samples, preprocessor=self.preprocessor, return_labels=False
-            )
-        elif split_files_into_clips:  # c2
-            prediction_dataset = AudioSplittingDataset(
-                samples=samples,
-                preprocessor=self.preprocessor,
-                overlap_fraction=overlap_fraction,
-                final_clip=final_clip,
-            )
-        else:  # c3
-            prediction_dataset = AudioFileDataset(
-                samples=samples, preprocessor=self.preprocessor, return_labels=False
-            )
-        prediction_dataset.bypass_augmentations = bypass_augmentations
-
-        ## Input Validation ##
-        if len(prediction_dataset.classes) > 0 and list(self.classes) != list(
-            prediction_dataset.classes
-        ):
-            warnings.warn(
-                "The columns of input samples df differ from `model.classes`."
-            )
-
-        if len(prediction_dataset) < 1:
-            warnings.warn(
-                "prediction_dataset has zero samples. No predictions will be generated."
-            )
-            return pd.DataFrame(columns=self.classes)
-
-        # If unsafe_behavior= "substitute", a SafeDataset will not fail on bad files,
-        # but will provide a different sample! Later we go back and replace scores
-        # with np.nan for the bad samples (using safe_dataset._invalid_indices)
-        # this approach to error handling feels hacky
-        # however, returning None would break the batching of samples
-        # "raise" behavior will raise exceptions
-        invalid_sample_behavior = "raise" if raise_errors else "substitute"
-
-        safe_dataset = SafeDataset(
-            prediction_dataset, invalid_sample_behavior=invalid_sample_behavior
-        )
-
-        dataloader = torch.utils.data.DataLoader(
-            safe_dataset,
+        # create dataloader to generate batches of AudioSamples
+        dataloader = self._init_inference_dataloader(
+            samples,
+            split_files_into_clips=split_files_into_clips,
+            overlap_fraction=overlap_fraction,
+            final_clip=final_clip,
+            bypass_augmentations=bypass_augmentations,
             batch_size=batch_size,
             num_workers=num_workers,
-            shuffle=False,
-            # use pin_memory=True when loading files on CPU and training on GPU
-            pin_memory=torch.cuda.is_available(),
-        )
-        # add any paths that failed to generate a clip df to _invalid_samples
-        dataloader.dataset._invalid_samples = dataloader.dataset._invalid_samples.union(
-            prediction_dataset.invalid_samples
+            raise_errors=raise_errors,
         )
 
         # Initialize Weights and Biases (wandb) logging
         if wandb_session is not None:
 
             # update the run config with information about the model
             wandb_session.config.update(self._generate_wandb_config())
@@ -932,16 +1086,17 @@
                     activation_layer=activation_layer,
                 )
             )
 
             # Log a table of preprocessed samples to wandb
             wandb_session.log(
                 {
-                    "Samples / Preprocessed samples": opensoundscape.wandb.wandb_table(
-                        prediction_dataset, self.wandb_logging["n_preview_samples"]
+                    "Samples / Preprocessed samples": wandb_table(
+                        dataloader.dataset.dataset,
+                        self.wandb_logging["n_preview_samples"],
                     )
                 }
             )
 
         ### Prediction/Inference ###
 
         # move network to device
@@ -949,22 +1104,24 @@
         self.network.eval()
 
         # initialize scores
         total_scores = []
 
         # disable gradient updates during inference
         with torch.set_grad_enabled(False):
-
-            for i, batch in enumerate(dataloader):
-                # get batch of Tensors
-                batch_tensors = batch["X"].to(self.device)
+            for i, samples in enumerate(dataloader):
+                # load a batch of images and labels from the  dataloader
+                # we collate here rather than in the DataLoader so that
+                # we can still access the AudioSamples and thier information
+                batch_data = collate_samples(samples)
+                batch_tensors = batch_data["samples"].to(self.device)
                 batch_tensors.requires_grad = False
 
                 # forward pass of network: feature extractor + classifier
-                logits = self.network.forward(batch_tensors)
+                logits = self.network(batch_tensors)
 
                 ### Activation layer ###
                 scores = apply_activation_layer(logits, activation_layer)
 
                 # disable gradients on returned values
                 total_scores.append(scores.detach().cpu().numpy())
 
@@ -974,23 +1131,25 @@
                             "progress": i / len(dataloader),
                             "completed_batches": i,
                             "total_batches": len(dataloader),
                         }
                     )
 
         # aggregate across all batches
-        total_scores = np.concatenate(total_scores, axis=0)
-
-        # replace scores with nan for samples that failed in preprocessing
-        # this feels hacky (we predicted on substitute-samples rather than
-        # skipping the samples that failed preprocessing)
-        total_scores[dataloader.dataset._invalid_indices, :] = np.nan
+        if len(total_scores) > 0:
+            total_scores = np.concatenate(total_scores, axis=0)
+            # replace scores with nan for samples that failed in preprocessing
+            # this feels hacky (we predicted on substitute-samples rather than
+            # skipping the samples that failed preprocessing)
+            total_scores[dataloader.dataset._invalid_indices, :] = np.nan
+        else:
+            total_scores = None
 
         # return DataFrame with same index/columns as prediction_dataset's df
-        df_index = prediction_dataset.label_df.index
+        df_index = dataloader.dataset.dataset.label_df.index
         score_df = pd.DataFrame(index=df_index, data=total_scores, columns=self.classes)
 
         # warn the user if there were invalid samples (failed to preprocess)
         # and log them to a file
         invalid_samples = dataloader.dataset.report(log=invalid_samples_log)
 
         # log top-scoring samples per class to wandb table
@@ -1001,30 +1160,241 @@
                 if len(classes_to_log) > 5:  # don't accidentally log hundreds of tables
                     classes_to_log = classes_to_log[0:5]
 
             for i, c in enumerate(classes_to_log):
                 top_samples = score_df.nlargest(
                     n=self.wandb_logging["n_top_samples"], columns=[c]
                 )
+                # note: the "labels" of these samples are actually prediction scores
                 dataset = AudioFileDataset(
                     samples=top_samples,
                     preprocessor=self.preprocessor,
-                    return_labels=False,
                     bypass_augmentations=True,
                 )
-                table = opensoundscape.wandb.wandb_table(
-                    dataset=dataset, classes_to_extract=[c]
+                table = wandb_table(
+                    dataset=dataset, classes_to_extract=[c], drop_labels=True
                 )
                 wandb_session.log({f"Samples / Top scoring [{c}]": table})
 
         if return_invalid_samples:
             return score_df, invalid_samples
         else:
             return score_df
 
+    def generate_cams(
+        self,
+        samples,
+        method="gradcam",
+        classes=None,
+        target_layers=None,
+        guided_backprop=False,
+        split_files_into_clips=True,
+        bypass_augmentations=True,
+        batch_size=1,
+        num_workers=0,
+    ):
+        """
+        Generate a activation and/or backprop heatmaps for each sample
+
+        Args:
+            samples: (same as CNN.predict())
+                the files to generate predictions for. Can be:
+                - a dataframe with index containing audio paths, OR
+                - a dataframe with multi-index (file, start_time, end_time), OR
+                - a list (or np.ndarray) of audio file paths
+            method: method to use for activation map. Can be str (choose from below)
+                or a class of pytorch_grad_cam (any subclass of BaseCAM), or None
+                if None, activation maps will not be created [default:'gradcam']
+
+                str can be any of the following:
+                    "gradcam": pytorch_grad_cam.GradCAM,
+                    "hirescam": pytorch_grad_cam.HiResCAM,
+                    "scorecam": pytorch_grad_cam.ScoreCAM,
+                    "gradcam++": pytorch_grad_cam.GradCAMPlusPlus,
+                    "ablationcam": pytorch_grad_cam.AblationCAM,
+                    "xgradcam": pytorch_grad_cam.XGradCAM,
+                    "eigencam": pytorch_grad_cam.EigenCAM,
+                    "eigengradcam": pytorch_grad_cam.EigenGradCAM,
+                    "layercam": pytorch_grad_cam.LayerCAM,
+                    "fullgrad": pytorch_grad_cam.FullGrad,
+                    "gradcamelementwise": pytorch_grad_cam.GradCAMElementWise,
+
+            classes (list): list of classes, will create maps for each class
+                [default: None] if None, creates an activation map for the highest
+                scoring class on a sample-by-sample basis
+            target_layers (list): list of target layers for GradCAM
+                - if None [default] attempts to use architecture's default target_layer
+                Note: only architectures created with opensoundscape 0.9.0+ will
+                have a default target layer. See pytorch_grad_cam docs for suggestions.
+                Note: if multiple layers are provided, the activations are merged across
+                    layers (rather than returning separate activations per layer)
+            guided_backprop: bool [default: False] if True, performs guided backpropagation
+                for each class in classes. AudioSamples will have attribute .gbp_maps,
+                a pd.Series indexed by class name
+            split_files_into_clips (bool): see CNN.predict()
+            bypass_augmentations (bool): whether to bypass augmentations in preprocessing
+                see CNN.predict
+            batch_size: number of samples to simultaneously process, see CNN.predict()
+            num_workers: parallel CPU threads for preprocessing, see CNN.predict()
+
+        Returns:
+            a list of cam class activation objects. see the cam class for more details
+
+        See pytorch_grad_cam documentation for references to the source of each method.
+        """
+
+        ## INPUT VALIDATION ##
+
+        if classes is not None:  # check that classes are in model.classes
+            assert np.all(
+                [c in self.classes for c in classes]
+            ), "`classes` must be in self.classes"
+
+        # if target_layer is None, attempt to retrieve default target layers of network
+        if target_layers is None:
+            try:
+                target_layers = self.network.cam_target_layers
+            except AttributeError as exc:
+                raise AttributeError(
+                    "Please specify _init_inference_dataloadertarget_layers. Models trained with older versions of Opensoundscape do not have default target layers"
+                    "For a ResNET model, try target_layers=[model.network.layer4]"
+                ) from exc
+        else:  # check that target_layers are modules of self.network
+            for tl in target_layers:
+                assert (
+                    tl in self.network.modules()
+                ), "target_layers must be in self.network.modules(), but {tl} is not."
+
+        ## INITIALIZE CAMS AND DATALOADER ##
+
+        # initialize cam object: `method` is either str in methods_dict keys, or the class
+        methods_dict = {
+            "gradcam": pytorch_grad_cam.GradCAM,
+            "hirescam": pytorch_grad_cam.HiResCAM,
+            "scorecam": pytorch_grad_cam.ScoreCAM,
+            "gradcam++": pytorch_grad_cam.GradCAMPlusPlus,
+            "ablationcam": pytorch_grad_cam.AblationCAM,
+            "xgradcam": pytorch_grad_cam.XGradCAM,
+            "eigencam": pytorch_grad_cam.EigenCAM,
+            "eigengradcam": pytorch_grad_cam.EigenGradCAM,
+            "layercam": pytorch_grad_cam.LayerCAM,
+            "fullgrad": pytorch_grad_cam.FullGrad,
+            "gradcamelementwise": pytorch_grad_cam.GradCAMElementWise,
+        }
+        if isinstance(method, str) and method in methods_dict:
+            cam = methods_dict[method](model=self.network, target_layers=target_layers)
+        elif method is None:
+            cam = None
+        elif issubclass(method, pytorch_grad_cam.base_cam.BaseCAM):
+            cam = method(model=self.network, target_layers=target_layers)
+        else:
+            raise ValueError(
+                f"`method` {method} not supported. "
+                f"Must be str from list of supported methods or a subclass of "
+                f"pytorch_grad_cam.base_cam.BaseCAM. See docstring for details. "
+            )
+
+        # initialize guided back propagation object
+        if guided_backprop:
+            gb_model = pytorch_grad_cam.GuidedBackpropReLUModel(
+                model=self.network, use_cuda=False
+            )  # TODO cuda usage - expose? use model setting?
+
+        # create dataloader to load batches of samples
+        dataloader = self._init_inference_dataloader(
+            samples,
+            split_files_into_clips=split_files_into_clips,
+            overlap_fraction=0,
+            final_clip=None,
+            bypass_augmentations=bypass_augmentations,
+            batch_size=batch_size,
+            num_workers=num_workers,
+        )
+
+        # move model to device
+        # TODO: choose cuda or not in pytorch_grad_cam methods
+        self.network.to(self.device)
+        self.network.eval()
+
+        ## GENERATE SAMPLES ##
+
+        generated_samples = []
+        for i, samples in enumerate(dataloader):
+            # load a batch of images and labels from the dataloader
+            # we collate here rather than in the DataLoader so that
+            # we can still access the AudioSamples and thier information
+            batch_data = collate_samples(samples)
+            batch_tensors = batch_data["samples"].to(self.device)
+            batch_tensors.requires_grad = False
+
+            # generate class activation maps using cam object
+            def target(class_name):
+                """helper for pytorch_grad_cam class syntax"""
+                # first get integet position of class name in self.classes
+                class_idx = list(self.classes).index(class_name)
+                # then create list of class required by pytorch_grad_cam
+                return [ClassifierOutputTarget(class_idx)]
+
+            if cam is not None:
+                if classes is None:  # selects highest scoring class per sample
+                    batch_maps = pd.Series({None: cam(batch_tensors)})
+                else:  # one activation map per class
+                    batch_maps = pd.Series(
+                        {c: cam(batch_tensors, targets=target(c)) for c in classes}
+                    )
+
+            # update the AudioSample objects to include the activation maps
+            # and create guided backprop maps, one at a time
+            for i, sample in enumerate(samples):
+
+                if cam is None:
+                    activation_maps = None
+                else:
+                    # extract this sample's activation maps from batch (all classes)
+                    activation_maps = pd.Series(
+                        {c: batch_maps[c][i] for c in batch_maps.index}
+                    )
+
+                # if requested, calculate the ReLU backpropogation, which creates
+                # high resolution pixel-activation levels for specific classes
+                # GuidedBackpropReLUasModule does not support batching
+                if guided_backprop:
+                    t = batch_tensors[i].unsqueeze(0)  # "batch" with one sample
+                    # target_category expects the index position of the class eg 0 for
+                    # first class, rather than the class name
+                    # note: t.detach() to avoid bug,
+                    # see https://github.com/jacobgil/pytorch-grad-cam/issues/401
+                    if classes is None:  # defaults to highest scoring class
+                        gbp_maps = pd.Series({None: gb_model(t.detach())})
+                    else:  # one for each class
+                        cls_list = list(self.classes)
+                        gbp_maps = pd.Series(
+                            {
+                                c: gb_model(
+                                    t.detach(), target_category=cls_list.index(c)
+                                )
+                                for c in classes
+                            }
+                        )
+                else:  # no guided backprop requested
+                    gbp_maps = None
+
+                # add CAM object as sample.cam (includes activation_map and gbp_maps)
+                sample.cam = CAM(
+                    base_image=batch_tensors[i],
+                    activation_maps=activation_maps,
+                    gbp_maps=gbp_maps,
+                )
+
+                # add sample to list of outputs to return
+                generated_samples.append(sample)
+
+        # return list of AudioSamples containing .cam attributes
+        return generated_samples
+
 
 def use_resample_loss(model):
     """Modify a model to use ResampleLoss for multi-target training
 
     ResampleLoss may perform better than BCE Loss for multitarget problems
     in some scenarios.
     """
@@ -1171,28 +1541,31 @@
         self.network.train()
 
         total_tgts = []
         total_preds = []
         total_scores = []
         batch_loss = []
 
-        for batch_idx, batch_data in enumerate(train_loader):
+        for batch_idx, samples in enumerate(train_loader):
             # load a batch of images and labels from the train loader
             # all augmentation occurs in the Preprocessor (train_loader)
-            batch_tensors = batch_data["X"].to(self.device)
-            batch_labels = batch_data["y"].to(self.device)
+            # we collate here rather than in the DataLoader so that
+            # we can still access the AudioSamples and thier information
+            batch_data = collate_samples(samples)
+            batch_tensors = batch_data["samples"].to(self.device)
+            batch_labels = batch_data["labels"].to(self.device)
             # batch_labels = batch_labels.squeeze(1)
 
             ####################
             # Forward and loss #
             ####################
 
             # forward pass: feature extractor and classifier
             # inception returns two sets of outputs
-            inception_outputs = self.network.forward(batch_tensors)
+            inception_outputs = self.network(batch_tensors)
             logits = inception_outputs.logits
             aux_logits = inception_outputs.aux_logits
 
             # save targets and predictions
             total_scores.append(logits.detach().cpu().numpy())
             total_tgts.append(batch_labels.detach().cpu().numpy())
 
@@ -1258,45 +1631,71 @@
         # return targets, preds, scores
         total_tgts = np.concatenate(total_tgts, axis=0)
         total_preds = np.concatenate(total_preds, axis=0)
         total_scores = np.concatenate(total_scores, axis=0)
 
         return total_tgts, total_preds, total_scores
 
+    @classmethod
+    def from_torch_dict(self):
+        raise NotImplementedError(
+            "Creating InceptionV3 from torch dict is not implemented."
+        )
+
 
 def load_model(path, device=None):
     """load a saved model object
 
+    Note: saving and loading model objects across OpenSoundscape versions
+    will not work properly. Instead, use .save_torch_dict and .load_torch_dict
+    (but note that customizations to preprocessing, training params, etc will
+    not be retained using those functions).
+
+    For maximum flexibilty in further use, save the model with both .save() and
+    .save_torch_dict()
+
     Args:
         path: file path of saved model
         device: which device to load into, eg 'cuda:1'
         [default: None] will choose first gpu if available, otherwise cpu
 
     Returns:
         a model object with loaded weights
     """
+    # load the entire pickled model object from a file and
+    # move the model to the desired torch "device" (eg cpu or cuda for gpu)
     if device is None:
         device = (
             torch.device("cuda:0") if torch.cuda.is_available() else torch.device("cpu")
         )
     model = torch.load(path, map_location=device)
 
+    # warn the user if loaded model's opso version doesn't match the current one
+    if model.opensoundscape_version != opensoundscape.__version__:
+        warnings.warn(
+            f"This model was saved with an earlier version of opensoundscape "
+            f"({model.opensoundscape_version}) and will not work properly in "
+            f"the current opensoundscape version ({opensoundscape.__version__}). "
+            f"To use models across package versions use .save_torch_dict and "
+            f".load_torch_dict"
+        )
+
     # since ResampleLoss class overrides a method of an instance,
     # we need to re-change the _init_loss_fn change when we reload
     if model.loss_cls == ResampleLoss:
         use_resample_loss(model)
 
     model.device = device
     return model
 
 
 def load_outdated_model(
     path, architecture, sample_duration, model_class=CNN, device=None
 ):
-    """load a CNN saved with a previous version of OpenSoundscape
+    """load a CNN saved with a version of OpenSoundscape <0.6.0
 
     This function enables you to load models saved with opso 0.4.x and 0.5.x.
     If your model was saved with .save() in a previous version of OpenSoundscape
     >=0.6.0, you must re-load the model
     using the original package version and save it's network's state dict, i.e.,
     `torch.save(model.network.state_dict(),path)`, then load the state dict
     to a new model object with model.load_weights(). See the
@@ -1309,19 +1708,19 @@
     `model.save(path)` after creating it, then reload it with
     `model = load_model(path)`.
     The saved model will be fully compatible with opensoundscape >=0.7.0.
 
     Examples:
     ```
     #load a binary resnet18 model from opso 0.4.x, 0.5.x, or 0.6.0
-    from opensoundscape.torch.models.cnn import CNN
+    from opensoundscape import CNN
     model = load_outdated_model('old_model.tar',architecture='resnet18')
 
     #load a resnet50 model of class CNN created with opso 0.5.0
-    from opensoundscape.torch.models.cnn import CNN
+    from opensoundscape import CNN
     model_050 = load_outdated_model('opso050_pytorch_model_r50.model',architecture='resnet50')
     ```
 
     Args:
         path: path to model file, ie .model or .tar file
         architecture: see CNN docs
             (pass None if the class __init__ does not take architecture as an argument)
```

### Comparing `opensoundscape-0.8.0/opensoundscape/torch/models/utils.py` & `opensoundscape-0.9.0/opensoundscape/ml/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Utilties for .torch.models"""
+"""Utilties for .ml"""
 import warnings
 import pandas as pd
 import numpy as np
 import torch
 from torch import nn
 import torch.nn.functional as F
 from torch.utils.data import DataLoader
 from torch.nn.functional import softmax
 
 
-from opensoundscape.torch.sampling import ClassAwareSampler
+from opensoundscape.ml.sampling import ClassAwareSampler
 
 
 class BaseModule(nn.Module):
     """
     Base class for a pytorch model pipeline class.
 
     All child classes should define load, save, etc
```

### Comparing `opensoundscape-0.8.0/opensoundscape/torch/safe_dataset.py` & `opensoundscape-0.9.0/opensoundscape/ml/safe_dataset.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/opensoundscape/torch/sampling.py` & `opensoundscape-0.9.0/opensoundscape/ml/sampling.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.8.0/pyproject.toml` & `opensoundscape-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [tool.poetry]
 name = "opensoundscape"
-version = "0.8.0"
+version = "0.9.0"
 description = "Open source, scalable acoustic classification for ecology and conservation"
 authors = [
-  "Justin Kitzes <justin.kitzes@pitt.edu>",
-  "Barry Moore <moore0557@gmail.com>",
+  "Sam Lapp <sammlapp@gmail.com>",
   "Tessa Rhinehart <tessa.rhinehart@gmail.com>",
-  "Sam Lapp <sammlapp@gmail.com>"
+  "Louis Freeland-Haynes <>",
+  "Jatin Khilnani <>",
+  "Sasha Syunkova <>",
+  "Justin Kitzes <justin.kitzes@pitt.edu>",
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jkitzes/opensoundscape"
 packages = [{include = "opensoundscape"}]
 include = ["opensoundscape/**/*.py"]
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.10"
+python = ">=3.8,<3.10"
 docopt = ">=0.6.2"
-librosa = ">=0.7.0"
+librosa = ">=0.10.0"
 ray = ">=0.8.5"
-torch = ">=1.8.1"
-torchvision = ">=0.9.1"
+torch = ">=2.0.0"
+torchvision = ">=0.15.1"
 ipykernel = ">=5.2.0"
 pandas = ">=1.3"
 matplotlib = ">=3.2.1"
 schema = ">=0.7.2"
 jupyterlab = ">=2.1.4"
 scikit-image = ">=0.17.2"
 numba = ">=0.48.0"
@@ -36,14 +38,16 @@
 soundfile = ">=0.11"
 wandb = "^0.13.4"
 pillow = ">=9.3.0"
 jupyter-server = ">=1.17.0"
 protobuf = ">=4.21.6"
 joblib = ">=1.2.0"
 certifi = ">=2022.12.7"
+grad-cam = ">=1.4.6"
+sentry-sdk = ">=1.14.0"
 
 [tool.poetry.dev-dependencies]
 black = "~=22.8"
 pre-commit = ">=1.18"
 sphinx = ">=2.1"
 pytest = ">=5.1"
 sphinx-rtd-theme = ">=0.4.3"
```

### Comparing `opensoundscape-0.8.0/setup.py` & `opensoundscape-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['opensoundscape',
+ 'opensoundscape.ml',
  'opensoundscape.preprocess',
- 'opensoundscape.resources',
- 'opensoundscape.torch',
- 'opensoundscape.torch.architectures',
- 'opensoundscape.torch.models']
+ 'opensoundscape.resources']
 
 package_data = \
-{'': ['*'], 'opensoundscape': ['.pytest_cache/*', '.pytest_cache/v/cache/*']}
+{'': ['*']}
 
 install_requires = \
 ['Deprecated>=1.2.13,<2.0.0',
  'Jinja2<3.0',
  'certifi>=2022.12.7',
  'docopt>=0.6.2',
+ 'grad-cam>=1.4.6',
  'ipykernel>=5.2.0',
  'ipython>=7.10',
  'joblib>=1.2.0',
  'jupyter-server>=1.17.0',
  'jupyterlab>=2.1.4',
- 'librosa>=0.7.0',
+ 'librosa>=0.10.0',
  'matplotlib>=3.2.1',
  'numba>=0.48.0',
  'pandas>=1.3',
  'pillow>=9.3.0',
  'protobuf>=4.21.6',
  'pywavelets>=1.2.0',
  'ray>=0.8.5',
  'schema>=0.7.2',
  'scikit-image>=0.17.2',
  'scikit-learn>=0.24.2',
+ 'sentry-sdk>=1.14.0',
  'soundfile>=0.11',
- 'torch>=1.8.1',
- 'torchvision>=0.9.1',
+ 'torch>=2.0.0',
+ 'torchvision>=0.15.1',
  'wandb>=0.13.4,<0.14.0']
 
 entry_points = \
 {'console_scripts': ['build_docs = opensoundscape.console:build_docs',
                      'opensoundscape = opensoundscape.console:entrypoint']}
 
 setup_kwargs = {
     'name': 'opensoundscape',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Open source, scalable acoustic classification for ecology and conservation',
-    'long_description': '[![CI Status](https://github.com/kitzeslab/opensoundscape/workflows/CI/badge.svg)](https://github.com/kitzeslab/opensoundscape/actions?query=workflow%3ACI)\n[![Documentation Status](https://readthedocs.org/projects/opensoundscape/badge/?version=latest)](http://opensoundscape.org/en/latest/?badge=latest)\n\n# OpenSoundscape\n\nOpenSoundscape is a utility library for analyzing bioacoustic data. It consists of Python modules for tasks such as preprocessing audio data, training machine learning models to classify vocalizations, estimating the spatial location of sounds, identifying which species\' sounds are present in acoustic data, and more.\n\nThese utilities can be strung together to create data analysis pipelines. OpenSoundscape is designed to be run on any scale of computer: laptop, desktop, or computing cluster.\n\nOpenSoundscape is currently in active development. If you find a bug, please submit an issue. If you have another question about OpenSoundscape, please email Sam Lapp (`sam.lapp` at `pitt.edu`).\n\n\n#### Suggested Citation\n```\nLapp, Rhinehart, Freeland-Haynes, Khilnani, Syunkova, and Kitzes, 2022. "OpenSoundscape v0.8.0".\n```\n\n# Installation\n\nOpenSoundscape can be installed on Windows, Mac, and Linux machines. It has been tested on Python 3.7, 3.8, and 3.9. For Apple Silicon (M1 chip) users, Python 3.9 is recommended and may be required to avoid dependency issues. Python version 3.7.0 causes dependency issues \nand should be avoided. \n\nMost users should install OpenSoundscape via pip: `pip install opensoundscape==0.8.0`. Contributors and advanced users can also use Poetry to install OpenSoundscape.\n\nFor more detailed instructions on how to install OpenSoundscape and use it in Jupyter, see the [documentation](http://opensoundscape.org).\n\n# Features & Tutorials\nOpenSoundscape includes functions to:\n* load and manipulate audio files\n* create and manipulate spectrograms\n* train CNNs on spectrograms with PyTorch\n* run pre-trained CNNs to detect vocalizations\n* detect periodic vocalizations with RIBBIT\n* load and manipulate Raven annotations\n\nOpenSoundscape can also be used with our library of publicly available trained machine learning models for the detection of 500 common North American bird species.\n\nFor full API documentation and tutorials on how to use OpenSoundscape to work with audio and spectrograms, train machine learning models, apply trained machine learning models to acoustic data, and detect periodic vocalizations using RIBBIT, see the [documentation](http://opensoundscape.org).\n\n# Quick Start\n\nUsing Audio and Spectrogram classes\n```python\nfrom opensoundscape.audio import Audio\nfrom opensoundscape.spectrogram import Spectrogram\n\n#load an audio file and trim out a 5 second clip\nmy_audio = Audio.from_file("/path/to/audio.wav")\nclip_5s = my_audio.trim(0,5)\n\n#create a spectrogram and plot it\nmy_spec = Spectrogram.from_audio(clip_5s)\nmy_spec.plot()\n```\n\nLoad audio starting at a real-world timestamp\n```python\nfrom datetime import datetime; import pytz\n\nstart_time = pytz.timezone(\'UTC\').localize(datetime(2020,4,4,10,25))\naudio_length = 5 #seconds  \npath = \'/path/to/audiomoth_file.WAV\' #an AudioMoth recording\n\nAudio.from_file(path, start_timestamp=start_time,duration=audio_length)\n```\n\nUsing a pre-trained CNN to make predictions on long audio files\n```python\nfrom opensoundscape.torch.models.cnn import load_model\n\n#get list of audio files\nfiles = glob(\'./dir/*.WAV\')\n\n#generate predictions with a model\nmodel = load_model(\'/path/to/saved.model\')\nscores = model.predict(files)\n\n#scores is a dataframe with MultiIndex: file, start_time, end_time\n#containing inference scores for each class and each audio window\n```\n\nTraining a CNN with labeled audio data\n```python\nfrom opensoundscape.torch.models.cnn import CNN\nfrom sklearn.model_selection import train_test_split\n\n#load a DataFrame of one-hot audio clip labels\ndf = pd.read_csv(\'my_labels.csv\') #index: paths; columns: classes\ntrain_df, validation_df = train_test_split(df,test_size=0.2)\n\n#create a CNN and train on 2-second spectrograms for 2 epochs\nmodel = CNN(\'resnet18\',classes=df.columns,sample_duration=2.0)\nmodel.train(\n  train_df,\n  validation_df,\n  epochs=2\n)\n#the best model is automatically saved to a file `./best.model`\n```\n',
-    'author': 'Justin Kitzes',
-    'author_email': 'justin.kitzes@pitt.edu',
+    'long_description': '[![CI Status](https://github.com/kitzeslab/opensoundscape/workflows/CI/badge.svg)](https://github.com/kitzeslab/opensoundscape/actions?query=workflow%3ACI)\n[![Documentation Status](https://readthedocs.org/projects/opensoundscape/badge/?version=latest)](http://opensoundscape.org/en/latest/?badge=latest)\n\n# OpenSoundscape\n\nOpenSoundscape is a utility library for analyzing bioacoustic data. It consists of Python modules for tasks such as preprocessing audio data, training machine learning models to classify vocalizations, estimating the spatial location of sounds, identifying which species\' sounds are present in acoustic data, and more.\n\nThese utilities can be strung together to create data analysis pipelines. OpenSoundscape is designed to be run on any scale of computer: laptop, desktop, or computing cluster.\n\nOpenSoundscape is currently in active development. If you find a bug, please submit an issue. If you have another question about OpenSoundscape, please email Sam Lapp (`sam.lapp` at `pitt.edu`).\n\n\n#### Suggested Citation\n```\nLapp, Rhinehart, Freeland-Haynes, Khilnani, Syunkova, and Kitzes, 2023. "OpenSoundscape v0.9.0".\n```\n\n# Installation\n\nOpenSoundscape can be installed on Windows, Mac, and Linux machines. It has been tested on Python 3.8, and 3.9. For Apple Silicon (M1 chip) users, Python 3.9 is recommended and may be required to avoid dependency issues.\n\nMost users should install OpenSoundscape via pip: `pip install opensoundscape==0.9.0`. Contributors and advanced users can also use Poetry to install OpenSoundscape.\n\nFor more detailed instructions on how to install OpenSoundscape and use it in Jupyter, see the [documentation](http://opensoundscape.org).\n\n# Features & Tutorials\nOpenSoundscape includes functions to:\n* load and manipulate audio files\n* create and manipulate spectrograms\n* train CNNs on spectrograms with PyTorch\n* run pre-trained CNNs to detect vocalizations\n* detect periodic vocalizations with RIBBIT\n* load and manipulate Raven annotations\n\nOpenSoundscape can also be used with our library of publicly available trained machine learning models for the detection of 500 common North American bird species.\n\nFor full API documentation and tutorials on how to use OpenSoundscape to work with audio and spectrograms, train machine learning models, apply trained machine learning models to acoustic data, and detect periodic vocalizations using RIBBIT, see the [documentation](http://opensoundscape.org).\n\n# Quick Start\n\nUsing Audio and Spectrogram classes\n```python\nfrom opensoundscape.audio import Audio\nfrom opensoundscape.spectrogram import Spectrogram\n\n#load an audio file and trim out a 5 second clip\nmy_audio = Audio.from_file("/path/to/audio.wav")\nclip_5s = my_audio.trim(0,5)\n\n#create a spectrogram and plot it\nmy_spec = Spectrogram.from_audio(clip_5s)\nmy_spec.plot()\n```\n\nLoad audio starting at a real-world timestamp\n```python\nfrom datetime import datetime; import pytz\n\nstart_time = pytz.timezone(\'UTC\').localize(datetime(2020,4,4,10,25))\naudio_length = 5 #seconds  \npath = \'/path/to/audiomoth_file.WAV\' #an AudioMoth recording\n\nAudio.from_file(path, start_timestamp=start_time,duration=audio_length)\n```\n\nUsing a pre-trained CNN to make predictions on long audio files\n```python\nfrom opensoundscape import load_model\n\n#get list of audio files\nfiles = glob(\'./dir/*.WAV\')\n\n#generate predictions with a model\nmodel = load_model(\'/path/to/saved.model\')\nscores = model.predict(files)\n\n#scores is a dataframe with MultiIndex: file, start_time, end_time\n#containing inference scores for each class and each audio window\n```\n\nTraining a CNN with labeled audio data\n```python\nfrom opensoundscape import CNN\nfrom sklearn.model_selection import train_test_split\n\n#load a DataFrame of one-hot audio clip labels\ndf = pd.read_csv(\'my_labels.csv\') #index: paths; columns: classes\ntrain_df, validation_df = train_test_split(df,test_size=0.2)\n\n#create a CNN and train on 2-second spectrograms for 2 epochs\nmodel = CNN(\'resnet18\',classes=df.columns,sample_duration=2.0)\nmodel.train(\n  train_df,\n  validation_df,\n  epochs=2\n)\n#the best model is automatically saved to a file `./best.model`\n```\n',
+    'author': 'Sam Lapp',
+    'author_email': 'sammlapp@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jkitzes/opensoundscape',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.10',
+    'python_requires': '>=3.8,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `opensoundscape-0.8.0/PKG-INFO` & `opensoundscape-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: opensoundscape
-Version: 0.8.0
+Version: 0.9.0
 Summary: Open source, scalable acoustic classification for ecology and conservation
 Home-page: https://github.com/jkitzes/opensoundscape
 License: MIT
-Author: Justin Kitzes
-Author-email: justin.kitzes@pitt.edu
-Requires-Python: >=3.7.1,<3.10
+Author: Sam Lapp
+Author-email: sammlapp@gmail.com
+Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: Jinja2 (<3.0)
 Requires-Dist: certifi (>=2022.12.7)
 Requires-Dist: docopt (>=0.6.2)
+Requires-Dist: grad-cam (>=1.4.6)
 Requires-Dist: ipykernel (>=5.2.0)
 Requires-Dist: ipython (>=7.10)
 Requires-Dist: joblib (>=1.2.0)
 Requires-Dist: jupyter-server (>=1.17.0)
 Requires-Dist: jupyterlab (>=2.1.4)
-Requires-Dist: librosa (>=0.7.0)
+Requires-Dist: librosa (>=0.10.0)
 Requires-Dist: matplotlib (>=3.2.1)
 Requires-Dist: numba (>=0.48.0)
 Requires-Dist: pandas (>=1.3)
 Requires-Dist: pillow (>=9.3.0)
 Requires-Dist: protobuf (>=4.21.6)
 Requires-Dist: pywavelets (>=1.2.0)
 Requires-Dist: ray (>=0.8.5)
 Requires-Dist: schema (>=0.7.2)
 Requires-Dist: scikit-image (>=0.17.2)
 Requires-Dist: scikit-learn (>=0.24.2)
+Requires-Dist: sentry-sdk (>=1.14.0)
 Requires-Dist: soundfile (>=0.11)
-Requires-Dist: torch (>=1.8.1)
-Requires-Dist: torchvision (>=0.9.1)
+Requires-Dist: torch (>=2.0.0)
+Requires-Dist: torchvision (>=0.15.1)
 Requires-Dist: wandb (>=0.13.4,<0.14.0)
 Project-URL: Repository, https://github.com/jkitzes/opensoundscape
 Description-Content-Type: text/markdown
 
 [![CI Status](https://github.com/kitzeslab/opensoundscape/workflows/CI/badge.svg)](https://github.com/kitzeslab/opensoundscape/actions?query=workflow%3ACI)
 [![Documentation Status](https://readthedocs.org/projects/opensoundscape/badge/?version=latest)](http://opensoundscape.org/en/latest/?badge=latest)
 
@@ -48,23 +50,22 @@
 These utilities can be strung together to create data analysis pipelines. OpenSoundscape is designed to be run on any scale of computer: laptop, desktop, or computing cluster.
 
 OpenSoundscape is currently in active development. If you find a bug, please submit an issue. If you have another question about OpenSoundscape, please email Sam Lapp (`sam.lapp` at `pitt.edu`).
 
 
 #### Suggested Citation
 ```
-Lapp, Rhinehart, Freeland-Haynes, Khilnani, Syunkova, and Kitzes, 2022. "OpenSoundscape v0.8.0".
+Lapp, Rhinehart, Freeland-Haynes, Khilnani, Syunkova, and Kitzes, 2023. "OpenSoundscape v0.9.0".
 ```
 
 # Installation
 
-OpenSoundscape can be installed on Windows, Mac, and Linux machines. It has been tested on Python 3.7, 3.8, and 3.9. For Apple Silicon (M1 chip) users, Python 3.9 is recommended and may be required to avoid dependency issues. Python version 3.7.0 causes dependency issues 
-and should be avoided. 
+OpenSoundscape can be installed on Windows, Mac, and Linux machines. It has been tested on Python 3.8, and 3.9. For Apple Silicon (M1 chip) users, Python 3.9 is recommended and may be required to avoid dependency issues.
 
-Most users should install OpenSoundscape via pip: `pip install opensoundscape==0.8.0`. Contributors and advanced users can also use Poetry to install OpenSoundscape.
+Most users should install OpenSoundscape via pip: `pip install opensoundscape==0.9.0`. Contributors and advanced users can also use Poetry to install OpenSoundscape.
 
 For more detailed instructions on how to install OpenSoundscape and use it in Jupyter, see the [documentation](http://opensoundscape.org).
 
 # Features & Tutorials
 OpenSoundscape includes functions to:
 * load and manipulate audio files
 * create and manipulate spectrograms
@@ -102,30 +103,30 @@
 path = '/path/to/audiomoth_file.WAV' #an AudioMoth recording
 
 Audio.from_file(path, start_timestamp=start_time,duration=audio_length)
 ```
 
 Using a pre-trained CNN to make predictions on long audio files
 ```python
-from opensoundscape.torch.models.cnn import load_model
+from opensoundscape import load_model
 
 #get list of audio files
 files = glob('./dir/*.WAV')
 
 #generate predictions with a model
 model = load_model('/path/to/saved.model')
 scores = model.predict(files)
 
 #scores is a dataframe with MultiIndex: file, start_time, end_time
 #containing inference scores for each class and each audio window
 ```
 
 Training a CNN with labeled audio data
 ```python
-from opensoundscape.torch.models.cnn import CNN
+from opensoundscape import CNN
 from sklearn.model_selection import train_test_split
 
 #load a DataFrame of one-hot audio clip labels
 df = pd.read_csv('my_labels.csv') #index: paths; columns: classes
 train_df, validation_df = train_test_split(df,test_size=0.2)
 
 #create a CNN and train on 2-second spectrograms for 2 epochs
```

