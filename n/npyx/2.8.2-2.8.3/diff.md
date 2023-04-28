# Comparing `tmp/npyx-2.8.2.tar.gz` & `tmp/npyx-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npyx-2.8.2.tar", last modified: Sun Apr 23 14:38:55 2023, max compression
+gzip compressed data, was "dist/npyx-2.8.3.tar", last modified: Fri Apr 28 13:30:52 2023, max compression
```

## Comparing `npyx-2.8.2.tar` & `npyx-2.8.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-23 14:38:55.154370 npyx-2.8.2/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2022-11-30 14:14:46.000000 npyx-2.8.2/LICENSE.md
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-23 14:38:55.154370 npyx-2.8.2/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    31591 2023-03-28 09:45:46.000000 npyx-2.8.2/README.md
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-23 14:38:55.154370 npyx-2.8.2/npyx/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      789 2023-04-23 14:38:20.000000 npyx-2.8.2/npyx/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   142298 2023-03-06 16:29:02.000000 npyx-2.8.2/npyx/behav.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/circuitProphyler.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   106738 2023-04-20 20:31:09.000000 npyx-2.8.2/npyx/corr.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    28838 2023-04-20 18:33:44.000000 npyx-2.8.2/npyx/datasets.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    56712 2023-04-20 20:40:50.000000 npyx-2.8.2/npyx/feat.py
--rwxrwxr-x   0 maxime    (1000) maxime    (1000)    17109 2023-04-20 18:33:44.000000 npyx-2.8.2/npyx/gl.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    38180 2023-04-20 19:53:38.000000 npyx-2.8.2/npyx/h5.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-11-30 14:14:47.000000 npyx-2.8.2/npyx/histo.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16050 2022-11-30 14:14:47.000000 npyx-2.8.2/npyx/info.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    49232 2023-04-14 12:13:22.000000 npyx-2.8.2/npyx/inout.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/merger.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2023-03-20 15:37:11.000000 npyx-2.8.2/npyx/metrics.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4936 2023-04-20 18:33:44.000000 npyx-2.8.2/npyx/ml.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/model.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   149739 2023-04-20 20:19:11.000000 npyx-2.8.2/npyx/plot.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/preprocess.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    40231 2023-04-23 14:37:23.000000 npyx-2.8.2/npyx/spk_t.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    47559 2023-04-20 18:33:44.000000 npyx-2.8.2/npyx/spk_wvf.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    14661 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/stats.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/testing.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    65528 2023-03-24 11:24:27.000000 npyx-2.8.2/npyx/utils.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-23 14:38:55.154370 npyx-2.8.2/npyx.egg-info/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      492 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/top_level.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-04-23 14:38:55.154370 npyx-2.8.2/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1491 2023-04-14 12:19:49.000000 npyx-2.8.2/setup.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-28 13:30:52.299945 npyx-2.8.3/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2022-11-30 14:14:46.000000 npyx-2.8.3/LICENSE.md
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-28 13:30:52.299945 npyx-2.8.3/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    31591 2023-03-28 09:45:46.000000 npyx-2.8.3/README.md
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-28 13:30:52.295945 npyx-2.8.3/npyx/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      789 2023-04-28 13:29:58.000000 npyx-2.8.3/npyx/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   142298 2023-03-06 16:29:02.000000 npyx-2.8.3/npyx/behav.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/circuitProphyler.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   106738 2023-04-20 20:31:09.000000 npyx-2.8.3/npyx/corr.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    28838 2023-04-20 18:33:44.000000 npyx-2.8.3/npyx/datasets.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    56712 2023-04-20 20:40:50.000000 npyx-2.8.3/npyx/feat.py
+-rwxrwxr-x   0 maxime    (1000) maxime    (1000)    17109 2023-04-20 18:33:44.000000 npyx-2.8.3/npyx/gl.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    38231 2023-04-28 10:55:51.000000 npyx-2.8.3/npyx/h5.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-11-30 14:14:47.000000 npyx-2.8.3/npyx/histo.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16050 2022-11-30 14:14:47.000000 npyx-2.8.3/npyx/info.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    49232 2023-04-14 12:13:22.000000 npyx-2.8.3/npyx/inout.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/merger.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2023-03-20 15:37:11.000000 npyx-2.8.3/npyx/metrics.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5152 2023-04-28 13:28:54.000000 npyx-2.8.3/npyx/ml.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/model.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   149779 2023-04-25 12:52:34.000000 npyx-2.8.3/npyx/plot.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/preprocess.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    40231 2023-04-23 14:37:23.000000 npyx-2.8.3/npyx/spk_t.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    47559 2023-04-20 18:33:44.000000 npyx-2.8.3/npyx/spk_wvf.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    14661 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/stats.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2023-03-01 11:06:59.000000 npyx-2.8.3/npyx/testing.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    65528 2023-03-24 11:24:27.000000 npyx-2.8.3/npyx/utils.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-28 13:30:52.299945 npyx-2.8.3/npyx.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      492 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2023-04-28 13:30:52.000000 npyx-2.8.3/npyx.egg-info/top_level.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-04-28 13:30:52.299945 npyx-2.8.3/setup.cfg
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1491 2023-04-14 12:19:49.000000 npyx-2.8.3/setup.py
```

### Comparing `npyx-2.8.2/LICENSE.md` & `npyx-2.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/PKG-INFO` & `npyx-2.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 2.8.2
+Version: 2.8.3
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `npyx-2.8.2/README.md` & `npyx-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/__init__.py` & `npyx-2.8.3/npyx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,10 +36,10 @@
  .behav
  .merger
  .circuitProphyler
  .feat
  .h5
 """
 
-__version__ = "2.8.2"
+__version__ = "2.8.3"
 
 print(f"npyx version {__version__} imported.")
```

### Comparing `npyx-2.8.2/npyx/behav.py` & `npyx-2.8.3/npyx/behav.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/circuitProphyler.py` & `npyx-2.8.3/npyx/circuitProphyler.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/corr.py` & `npyx-2.8.3/npyx/corr.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/datasets.py` & `npyx-2.8.3/npyx/datasets.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/feat.py` & `npyx-2.8.3/npyx/feat.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/gl.py` & `npyx-2.8.3/npyx/gl.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/h5.py` & `npyx-2.8.3/npyx/h5.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
             assert n_raw_waveforms > 0, "n_raw_waveforms must be > 0"
             if len(spike_ids) > n_raw_waveforms:
                 random_ids = np.random.randint(0, spike_ids.shape[0]-1, n_raw_waveforms)
                 spike_ids  = spike_ids[random_ids]
                 
             # load waveforms
             raw_waveforms = get_waveforms(dp, unit_id, t_waveforms=180,
-                                            spike_ids=spike_ids, med_sub_in_time=False)
+                                            spike_ids=spike_ids, med_sub_in_time=False,  ignore_ks_chanfilt=True)
             raw_waveforms = raw_waveforms[:, :, chan_bottom:chan_top].transpose(0,2,1)
 
             # recast to int16
             raw_waveforms = raw_waveforms / meta["bit_uV_conv_factor"]
             raw_waveforms = raw_waveforms.astype(np.int16)
 
             write_to_group(neuron_group, key, raw_waveforms)
@@ -625,20 +625,20 @@
     optostims_from_sync = True
     optostims_threshold = 20 * 60
 
     add_json_datasets_to_h5(
         json_path,
         h5_path,
         "hausser",
-        include_all_good=include_all_good,
-        optostims_from_sync=optostims_from_sync,
-        optostims_threshold=optostims_threshold,
-        sane_before_opto=sane_before_opto,
-        selective_overwrite=selective_overwrite,
-        overwrite_h5=overwrite_h5,
+        include_all_good    = include_all_good,
+        optostims_from_sync = optostims_from_sync,
+        optostims_threshold = optostims_threshold,
+        sane_before_opto    = sane_before_opto,
+        selective_overwrite = selective_overwrite,
+        overwrite_h5        = overwrite_h5,
         **kwargs,
     )
 
 
 def load_json_datasets(json_path, include_missing_datasets=False):
     with open(json_path) as f:
         json_f = json.load(f)
```

### Comparing `npyx-2.8.2/npyx/info.py` & `npyx-2.8.3/npyx/info.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/inout.py` & `npyx-2.8.3/npyx/inout.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/merger.py` & `npyx-2.8.3/npyx/merger.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/metrics.py` & `npyx-2.8.3/npyx/metrics.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/ml.py` & `npyx-2.8.3/npyx/ml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import os
 import random
 
 import numpy as np
 import pandas as pd
-import torch
+
+try:
+    import torch
+except ImportError:
+    print(("PyTorch could not be imported - "
+    "some functions from the submodule npyx.ml will not work.\n"
+    "To install PyTorch, follow the instructions at http://pytorch.org"))
+
 from imblearn.over_sampling import RandomOverSampler
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.metrics import f1_score
 from sklearn.model_selection import LeaveOneOut
 from tqdm.auto import tqdm
```

### Comparing `npyx-2.8.2/npyx/model.py` & `npyx-2.8.3/npyx/model.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/plot.py` & `npyx-2.8.3/npyx/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -2477,15 +2477,15 @@
     return fig
 
 
 def plot_acg(dp, unit, cbin=0.2, cwin=80, normalize='Hertz', periods='all',
              saveDir='~/Downloads', saveFig=False, _format='pdf', figsize=None, verbose=False,
              color=0, labels=True, title=None, ref_per=True, ylim=[0, 0], ax=None,
              acg_mn=None, acg_std=None, again=False,
-             train=None, hide_axis=False, prettify=True, **mplp_kwargs):
+             train=None, hide_axis=False, prettify=True, enforced_rp=0, **mplp_kwargs):
     """
     Plots precomputed autocorrelogram.
     Arguments:
         - dp: str, data path
         - unit: float, unit index
         - cbin: float, binsize (ms)
         - cwin: float, full window size (ms)
@@ -2523,15 +2523,15 @@
     if train is not None:
         bChs = None
     else:
         bChs = get_depthSort_peakChans(dp, units=[unit])[:, 1].flatten()
     ylim1, ylim2 = ylim[0], ylim[1]
 
     ACG = acg(dp, unit, cbin, cwin, fs=30000, normalize=normalize,
-              verbose=verbose, periods=periods, again=again, train=train)
+              verbose=verbose, periods=periods, again=again, train=train, enforced_rp=enforced_rp)
     if normalize == 'zscore':
         ACG_hertz = acg(dp, unit, cbin, cwin, fs=30000, normalize='Hertz', verbose=verbose, periods=periods)
         acg25, acg35 = ACG_hertz[:int(len(ACG_hertz) * 2. / 5)], ACG_hertz[int(len(ACG_hertz) * 3. / 5):]
         acg_std = np.std(np.append(acg25, acg35))
         acg_mn = np.mean(np.append(acg25, acg35))
     fig = plt_acg(unit, ACG, cbin, cwin, bChs, color, 30000, saveDir, saveFig, _format=_format,
                   labels=labels, title=title, ref_per=ref_per, ylim1=ylim1, ylim2=ylim2, ax=ax,
```

### Comparing `npyx-2.8.2/npyx/preprocess.py` & `npyx-2.8.3/npyx/preprocess.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/spk_t.py` & `npyx-2.8.3/npyx/spk_t.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/spk_wvf.py` & `npyx-2.8.3/npyx/spk_wvf.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/stats.py` & `npyx-2.8.3/npyx/stats.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/testing.py` & `npyx-2.8.3/npyx/testing.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx/utils.py` & `npyx-2.8.3/npyx/utils.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.2/npyx.egg-info/PKG-INFO` & `npyx-2.8.3/npyx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 2.8.2
+Version: 2.8.3
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `npyx-2.8.2/setup.py` & `npyx-2.8.3/setup.py`

 * *Files identical despite different names*

