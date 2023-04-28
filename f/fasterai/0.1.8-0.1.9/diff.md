# Comparing `tmp/fasterai-0.1.8.tar.gz` & `tmp/fasterai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasterai-0.1.8.tar", last modified: Sun May 29 11:14:46 2022, max compression
+gzip compressed data, was "fasterai-0.1.9.tar", last modified: Tue Jul  5 12:57:03 2022, max compression
```

## Comparing `fasterai-0.1.8.tar` & `fasterai-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-05-29 11:14:38.027332 fasterai-0.1.8/
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2348 2021-03-11 17:53:27.000000 fasterai-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)    11357 2021-03-11 17:53:27.000000 fasterai-0.1.8/LICENSE
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      111 2021-03-11 17:53:27.000000 fasterai-0.1.8/MANIFEST.in
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     6213 2022-05-29 11:14:38.026332 fasterai-0.1.8/PKG-INFO
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     5460 2022-05-29 11:05:43.000000 fasterai-0.1.8/README.md
-drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-05-29 11:14:37.994332 fasterai-0.1.8/fasterai/
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)       21 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/__init__.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2507 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/_nbdev.py
-drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-05-29 11:14:38.007332 fasterai-0.1.8/fasterai/distill/
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        0 2021-03-12 08:38:31.000000 fasterai-0.1.8/fasterai/distill/__init__.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)       38 2021-03-15 16:33:12.000000 fasterai-0.1.8/fasterai/distill/all.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     4721 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/distill/distillation_callback.py
-drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-05-29 11:14:38.011332 fasterai-0.1.8/fasterai/misc/
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        0 2021-06-16 14:36:11.000000 fasterai-0.1.8/fasterai/misc/__init__.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2129 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/misc/bn_folding.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     1788 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/misc/fc_decomposer.py
-drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-05-29 11:14:38.013332 fasterai-0.1.8/fasterai/regularization/
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        0 2021-10-29 14:56:33.000000 fasterai-0.1.8/fasterai/regularization/__init__.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      734 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/regularization/regularization_callback.py
-drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-05-29 11:14:38.025332 fasterai-0.1.8/fasterai/sparse/
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        0 2021-03-12 08:38:31.000000 fasterai-0.1.8/fasterai/sparse/__init__.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      107 2021-03-12 08:45:17.000000 fasterai-0.1.8/fasterai/sparse/all.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     3269 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/sparse/criteria.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      875 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/sparse/granularity.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     5112 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/sparse/pruner.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      657 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/sparse/schedule.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     5429 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/sparse/sparsifier.py
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     3425 2022-05-29 11:05:14.000000 fasterai-0.1.8/fasterai/sparse/sparsify_callback.py
-drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-05-29 11:14:38.003332 fasterai-0.1.8/fasterai.egg-info/
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     6213 2022-05-29 11:14:37.000000 fasterai-0.1.8/fasterai.egg-info/PKG-INFO
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      795 2022-05-29 11:14:37.000000 fasterai-0.1.8/fasterai.egg-info/SOURCES.txt
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        1 2022-05-29 11:14:37.000000 fasterai-0.1.8/fasterai.egg-info/dependency_links.txt
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        1 2021-06-01 10:56:38.000000 fasterai-0.1.8/fasterai.egg-info/not-zip-safe
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)       12 2022-05-29 11:14:37.000000 fasterai-0.1.8/fasterai.egg-info/requires.txt
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        9 2022-05-29 11:14:37.000000 fasterai-0.1.8/fasterai.egg-info/top_level.txt
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2430 2022-05-29 11:13:13.000000 fasterai-0.1.8/settings.ini
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)       38 2022-05-29 11:14:38.027332 fasterai-0.1.8/setup.cfg
--rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     1921 2021-03-11 17:53:27.000000 fasterai-0.1.8/setup.py
+drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-07-05 12:56:45.409049 fasterai-0.1.9/
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2348 2021-03-11 17:53:27.000000 fasterai-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)    11357 2021-03-11 17:53:27.000000 fasterai-0.1.9/LICENSE
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      111 2021-03-11 17:53:27.000000 fasterai-0.1.9/MANIFEST.in
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     6213 2022-07-05 12:56:45.408049 fasterai-0.1.9/PKG-INFO
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     5460 2022-07-05 12:41:10.000000 fasterai-0.1.9/README.md
+drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-07-05 12:56:45.347049 fasterai-0.1.9/fasterai/
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)       21 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/__init__.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2888 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/_nbdev.py
+drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-07-05 12:56:45.385049 fasterai-0.1.9/fasterai/distill/
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        0 2021-03-12 08:38:31.000000 fasterai-0.1.9/fasterai/distill/__init__.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)       38 2021-03-15 16:33:12.000000 fasterai-0.1.9/fasterai/distill/all.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     4721 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/distill/distillation_callback.py
+drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-07-05 12:56:45.390049 fasterai-0.1.9/fasterai/misc/
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        0 2021-06-16 14:36:11.000000 fasterai-0.1.9/fasterai/misc/__init__.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2129 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/misc/bn_folding.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     1788 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/misc/fc_decomposer.py
+drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-07-05 12:56:45.393049 fasterai-0.1.9/fasterai/regularization/
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        0 2021-10-29 14:56:33.000000 fasterai-0.1.9/fasterai/regularization/__init__.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      734 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/regularization/regularization_callback.py
+drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-07-05 12:56:45.406049 fasterai-0.1.9/fasterai/sparse/
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        0 2021-03-12 08:38:31.000000 fasterai-0.1.9/fasterai/sparse/__init__.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      107 2021-03-12 08:45:17.000000 fasterai-0.1.9/fasterai/sparse/all.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     3269 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/sparse/criteria.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      875 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/sparse/granularity.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     5112 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/sparse/pruner.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2741 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/sparse/schedule.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     5567 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/sparse/sparsifier.py
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2634 2022-07-05 12:41:06.000000 fasterai-0.1.9/fasterai/sparse/sparsify_callback.py
+drwxr-xr-x   0 HubensN  (1000021) Domain Users (1000000)        0 2022-07-05 12:56:45.370049 fasterai-0.1.9/fasterai.egg-info/
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     6213 2022-07-05 12:56:44.000000 fasterai-0.1.9/fasterai.egg-info/PKG-INFO
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)      795 2022-07-05 12:56:44.000000 fasterai-0.1.9/fasterai.egg-info/SOURCES.txt
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        1 2022-07-05 12:56:44.000000 fasterai-0.1.9/fasterai.egg-info/dependency_links.txt
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        1 2021-06-01 10:56:38.000000 fasterai-0.1.9/fasterai.egg-info/not-zip-safe
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)       12 2022-07-05 12:56:44.000000 fasterai-0.1.9/fasterai.egg-info/requires.txt
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)        9 2022-07-05 12:56:44.000000 fasterai-0.1.9/fasterai.egg-info/top_level.txt
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     2430 2022-07-05 12:41:00.000000 fasterai-0.1.9/settings.ini
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)       38 2022-07-05 12:56:45.409049 fasterai-0.1.9/setup.cfg
+-rw-r--r--   0 HubensN  (1000021) Domain Users (1000000)     1921 2021-03-11 17:53:27.000000 fasterai-0.1.9/setup.py
```

### Comparing `fasterai-0.1.8/CONTRIBUTING.md` & `fasterai-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/LICENSE` & `fasterai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/PKG-INFO` & `fasterai-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasterai
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library to make neural networks lighter and faster with fastai
 Home-page: https://github.com/nathanhubens/fasterai/tree/master/
 Author: Nathan Hubens
 Author-email: nathan.hubens@gmail.com
 License: Apache Software License 2.0
 Keywords: Pruning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fasterai Version: 0.1.8 Summary: A library to make
+Metadata-Version: 2.1 Name: fasterai Version: 0.1.9 Summary: A library to make
 neural networks lighter and faster with fastai Home-page: https://github.com/
 nathanhubens/fasterai/tree/master/ Author: Nathan Hubens Author-email:
 nathan.hubens@gmail.com License: Apache Software License 2.0 Keywords: Pruning
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `fasterai-0.1.8/README.md` & `fasterai-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/fasterai/_nbdev.py` & `fasterai-0.1.9/fasterai/_nbdev.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,18 +30,27 @@
          "small_init_small_final": "0b_criteria.ipynb",
          "magnitude_increase": "0b_criteria.ipynb",
          "movement": "0b_criteria.ipynb",
          "updating_magnitude_increase": "0b_criteria.ipynb",
          "updating_movement": "0b_criteria.ipynb",
          "updating_movmag": "0b_criteria.ipynb",
          "grad_crit": "0b_criteria.ipynb",
+         "Schedule": "0c_schedules.ipynb",
+         "sched_oneshot": "0c_schedules.ipynb",
          "one_shot": "0c_schedules.ipynb",
+         "sched_iterative": "0c_schedules.ipynb",
          "iterative": "0c_schedules.ipynb",
          "sched_agp": "0c_schedules.ipynb",
-         "sched_onecycle": "0c_schedules.ipynb"}
+         "agp": "0c_schedules.ipynb",
+         "sched_onecycle": "0c_schedules.ipynb",
+         "one_cycle": "0c_schedules.ipynb",
+         "cos": "0c_schedules.ipynb",
+         "lin": "0c_schedules.ipynb",
+         "sched_dsd": "0c_schedules.ipynb",
+         "dsd": "0c_schedules.ipynb"}
 
 modules = ["sparse/sparsifier.py",
            "sparse/sparsify_callback.py",
            "sparse/pruner.py",
            "distill/distillation_callback.py",
            "misc/bn_folding.py",
            "misc/fc_decomposer.py",
```

### Comparing `fasterai-0.1.8/fasterai/distill/distillation_callback.py` & `fasterai-0.1.9/fasterai/distill/distillation_callback.py`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/fasterai/misc/bn_folding.py` & `fasterai-0.1.9/fasterai/misc/bn_folding.py`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/fasterai/misc/fc_decomposer.py` & `fasterai-0.1.9/fasterai/misc/fc_decomposer.py`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/fasterai/regularization/regularization_callback.py` & `fasterai-0.1.9/fasterai/regularization/regularization_callback.py`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/fasterai/sparse/criteria.py` & `fasterai-0.1.9/fasterai/sparse/criteria.py`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/fasterai/sparse/granularity.py` & `fasterai-0.1.9/fasterai/sparse/granularity.py`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/fasterai/sparse/pruner.py` & `fasterai-0.1.9/fasterai/sparse/pruner.py`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/fasterai/sparse/sparsifier.py` & `fasterai-0.1.9/fasterai/sparse/sparsifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 import torch.nn as nn
 from fastcore.basics import store_attr, listify
 from .criteria import *
 import pickle
 
 # Cell
 class Sparsifier():
-    def __init__(self, model, granularity, method, criteria, layer_type=nn.Conv2d):
+    def __init__(self, model, granularity, context, criteria, layer_type=nn.Conv2d):
         store_attr()
         self._save_weights() # Save the original weights
 
     def prune_layer(self, m, sparsity, round_to=None):
         weight = self.criteria(m, self.granularity)
         mask = self._compute_mask(weight, sparsity, round_to)
         m.register_buffer("_mask", mask) # Put the mask into a buffer
         self._apply(m)
 
     def prune_model(self, sparsity, round_to=None):
         self.threshold=None
         sparsity_list = listify(sparsity)
-        if len(sparsity_list)>1: assert self.method=='local', f"A list of sparsities cannot be passed using: {self.method}"
+        if len(sparsity_list)>1: assert self.context=='local', f"A list of sparsities cannot be passed using: {self.context}"
         sparsities = cycle(sparsity_list) if len(sparsity_list)==1 else iter(sparsity_list)
         mods = list(self.model.modules())
         for k,m in enumerate(self.model.modules()):
             if isinstance(m, self.layer_type):
                 sp = next(sparsities)
                 self.prune_layer(m, sp, round_to)
                 if isinstance(mods[k+1], nn.modules.batchnorm._BatchNorm): self.prune_batchnorm(m, mods[k+1])
@@ -58,15 +58,16 @@
             if isinstance(m, self.layer_type) and hasattr(m, '_mask'):
                 mask = getattr(m, "_mask")
                 if m.weight.grad is not None: m.weight.grad.mul_(mask)
                 if self.granularity == 'filter' and m.bias is not None:
                     if m.bias.grad is not None: m.bias.grad.mul_(mask.squeeze())
 
 
-    def _reset_weights(self, model): # Reset non-pruned weights
+    def _reset_weights(self, model=None): # Reset non-pruned weights
+        if not model: model=self.model
         for m in model.modules():
             if hasattr(m, 'weight'):
                 init_weights = getattr(m, "_init_weights", m.weight)
                 init_biases = getattr(m, "_init_biases", m.bias)
                 with torch.no_grad():
                     if m.weight is not None: m.weight.copy_(init_weights)
                     if m.bias is not None: m.bias.copy_(init_biases)
@@ -76,35 +77,37 @@
     def _save_weights(self):
         for m in self.model.modules():
             if hasattr(m, 'weight'):
                 m.register_buffer("_init_weights", m.weight.clone())
                 b = getattr(m, 'bias', None)
                 if b is not None: m.register_buffer("_init_biases", b.clone())
 
-    def save_model(self, model, path):
+    def save_model(self, path, model=None):
+        if not model: model=self.model
         tmp_model = pickle.loads(pickle.dumps(model))
         self._reset_weights(tmp_model)
         self._clean_buffers(tmp_model)
         torch.save(tmp_model, path)
 
-    def _clean_buffers(self, model):
+    def _clean_buffers(self, model=None):
+        if not model: model=self.model
         for m in model.modules():
             if hasattr(m, 'weight'):
                 if hasattr(m, '_mask'): del m._buffers["_mask"]
                 if hasattr(m, '_init_weights'): del m._buffers["_init_weights"]
                 if hasattr(m, '_init_biases'): del m._buffers["_init_biases"]
 
     def _compute_threshold(self, weight, sparsity):
-        if self.method == 'global':
+        if self.context == 'global':
             global_weight = torch.cat([self.criteria(m, self.granularity).view(-1) for m in self.model.modules() if isinstance(m, self.layer_type)])
             if self.threshold is None: self.threshold = torch.quantile(global_weight, sparsity/100) # Compute the threshold globally (only once per model pruning)
             return self.threshold
-        elif self.method == 'local':
+        elif self.context == 'local':
             return torch.quantile(weight.view(-1), sparsity/100) # Compute the threshold locally
-        else: raise NameError('Invalid Method')
+        else: raise NameError('Invalid Context')
 
     def _rounded_sparsity(self, n_to_prune, round_to):
         return max(round_to*torch.ceil(n_to_prune/round_to), round_to)
 
     def _compute_mask(self, weight, sparsity, round_to):
         threshold = self._compute_threshold(weight, sparsity)
         if round_to:
```

### Comparing `fasterai-0.1.8/fasterai/sparse/sparsify_callback.py` & `fasterai-0.1.9/fasterai/sparse/sparsify_callback.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,68 +3,58 @@
 __all__ = ['SparsifyCallback']
 
 # Cell
 from fastai.vision.all import *
 from fastai.callback.all import *
 from .sparsifier import *
 from .criteria import *
+from .schedule import *
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 # Cell
 class SparsifyCallback(Callback):
-
-    def __init__(self, end_sparsity, granularity, method, criteria, sched_func, start_sparsity=0, start_epoch=0, end_epoch=None, lth=False, rewind_epoch=0, reset_end=False, model=None, round_to=None, save_tickets=False, layer_type=nn.Conv2d):
+    def __init__(self, sparsity, granularity, context, criteria, schedule, lth=False, rewind_epoch=0, reset_end=False, save_tickets=False, model=None, round_to=None, layer_type=nn.Conv2d):
         store_attr()
-        self.end_sparsity, self.current_sparsity, self.previous_sparsity = map(listify, [self.end_sparsity, self.start_sparsity, self.start_sparsity])
-
-        assert self.start_epoch>=self.rewind_epoch, 'You must rewind to an epoch before the start of the pruning process'
+        self.sparsity = listify(self.sparsity)
 
     def before_fit(self):
-        print(f'Pruning of {self.granularity} until a sparsity of {self.end_sparsity}%')
-        self.end_epoch = self.n_epoch if self.end_epoch is None else self.end_epoch
-        assert self.end_epoch <= self.n_epoch, 'Your end_epoch must be smaller than total number of epoch'
-
-        model = self.learn.model if self.model is None else self.model # Pass a model if you don't want the whole model to be pruned
-        self.sparsifier = Sparsifier(model, self.granularity, self.method, self.criteria, self.layer_type)
+        print(f'Pruning of {self.granularity} until a sparsity of {self.sparsity}%')
+        assert self.schedule.start_pct*self.n_epoch>=self.rewind_epoch, 'You must rewind to an epoch before the start of the pruning process'
+        model = self.model if self.model else self.learn.model
+        self.sparsifier = Sparsifier(model, self.granularity, self.context, self.criteria, self.layer_type)
 
     def before_epoch(self):
         if self.epoch == self.rewind_epoch:
             print(f'Saving Weights at epoch {self.epoch}')
             self.sparsifier._save_weights()
 
     def before_batch(self):
-        if self.epoch>=self.start_epoch and self.epoch < self.end_epoch:
-            self._set_sparsity()
-            if self.current_sparsity!=self.previous_sparsity and self.training:
-                if self.lth and self.save_tickets:
-                    print('Saving Intermediate Ticket')
-                    self.sparsifier.save_model(self.learn.model, f'winning_ticket_{self.previous_sparsity[0]:.2f}.pth')
-                self.sparsifier.prune_model(self.current_sparsity, self.round_to)
+        self.current_sparsity = self.schedule(self.sparsity, round(self.pct_train,3))
+        if self.schedule.pruned and self.training:
+            if self.lth and self.save_tickets:
+                print('Saving Intermediate Ticket')
+                self.sparsifier.save_model(f'winning_ticket_{self.previous_sparsity[0]:.2f}.pth', self.learn.model)
+            self.sparsifier.prune_model(self.current_sparsity, self.round_to)
 
     def after_step(self):
-        if self.epoch>=self.start_epoch:
-            if self.lth and self.current_sparsity!=self.previous_sparsity:
-                print(f'Resetting Weights to their epoch {self.rewind_epoch} values')
-                self.sparsifier._reset_weights(self.learn.model)
-
-            self.previous_sparsity = self.current_sparsity
-            self.sparsifier._apply_masks()
+        if self.lth and self.schedule.pruned:
+            print(f'Resetting Weights to their epoch {self.rewind_epoch} values')
+            self.sparsifier._reset_weights(self.learn.model)
+        self.schedule.after_pruned()
+        self.sparsifier._apply_masks()
 
     def after_epoch(self):
         sparsity_str = [float(f"%0.2f"%sp) for sp in self.current_sparsity]
         print(f'Sparsity at the end of epoch {self.epoch}: {sparsity_str}%')
 
     def after_fit(self):
         if self.save_tickets:
             print('Saving Final Ticket')
-            self.sparsifier.save_model(self.learn.model, f'winning_ticket_{self.previous_sparsity[0]:.2f}.pth')
-
-        print(f'Final Sparsity: {self.current_sparsity:}%')
-        if self.reset_end: self.sparsifier._reset_weights(self.learn.model)
-        self.sparsifier._clean_buffers(self.learn.model)
-        self.sparsifier.print_sparsity()
-
-    def _set_sparsity(self):
-        self.current_sparsity = [self.sched_func(start=self.start_sparsity, end=end_sp, pos=(round(self.pct_train,5)*self.n_epoch-self.start_epoch)/(self.end_epoch-self.start_epoch)) for end_sp in self.end_sparsity]
+            self.sparsifier.save_model(f'winning_ticket_{self.previous_sparsity[0]:.2f}.pth', self.learn.model)
+        print(f'Final Sparsity: {self.schedule.current_sparsity:}%')
+        if self.reset_end: self.sparsifier._reset_weights()
+        self.sparsifier._clean_buffers()
+        self.schedule.reset()
+        self.sparsifier.print_sparsity()
```

### Comparing `fasterai-0.1.8/fasterai.egg-info/PKG-INFO` & `fasterai-0.1.9/fasterai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasterai
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library to make neural networks lighter and faster with fastai
 Home-page: https://github.com/nathanhubens/fasterai/tree/master/
 Author: Nathan Hubens
 Author-email: nathan.hubens@gmail.com
 License: Apache Software License 2.0
 Keywords: Pruning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fasterai Version: 0.1.8 Summary: A library to make
+Metadata-Version: 2.1 Name: fasterai Version: 0.1.9 Summary: A library to make
 neural networks lighter and faster with fastai Home-page: https://github.com/
 nathanhubens/fasterai/tree/master/ Author: Nathan Hubens Author-email:
 nathan.hubens@gmail.com License: Apache Software License 2.0 Keywords: Pruning
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `fasterai-0.1.8/fasterai.egg-info/SOURCES.txt` & `fasterai-0.1.9/fasterai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fasterai-0.1.8/settings.ini` & `fasterai-0.1.9/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = nathanhubens
 description = A library to make neural networks lighter and faster with fastai
 keywords = Pruning
 author = Nathan Hubens
 author_email = nathan.hubens@gmail.com
 copyright = Nathan Hubens
 branch = master
-version = 0.1.8
+version = 0.1.9
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = True
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `fasterai-0.1.8/setup.py` & `fasterai-0.1.9/setup.py`

 * *Files identical despite different names*

