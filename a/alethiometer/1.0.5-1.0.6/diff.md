# Comparing `tmp/alethiometer-1.0.5.tar.gz` & `tmp/alethiometer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alethiometer-1.0.5.tar", last modified: Tue Apr 11 16:59:22 2023, max compression
+gzip compressed data, was "alethiometer-1.0.6.tar", last modified: Fri Apr 28 14:17:59 2023, max compression
```

## Comparing `alethiometer-1.0.5.tar` & `alethiometer-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.5/LICENSE
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1660 2023-04-11 16:59:22.216346 alethiometer-1.0.5/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      951 2023-04-11 15:49:09.000000 alethiometer-1.0.5/README.md
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/alethiometer/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.5/alethiometer/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-11 15:47:53.000000 alethiometer-1.0.5/alethiometer/__version__.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/alethiometer/datasets/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.5/alethiometer/datasets/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4252 2023-04-07 18:02:54.000000 alethiometer-1.0.5/alethiometer/datasets/dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.5/alethiometer/datasets/h5py_dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.5/alethiometer/datasets/imagenet16.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.5/alethiometer/utils.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3223 2023-04-11 16:58:07.000000 alethiometer-1.0.5/alethiometer/zc_proxy.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/alethiometer/zero_cost_metrics/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1348 2023-04-11 15:46:48.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/grad_norm.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/grasp.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/naswot.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/snip.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/synflow.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/alethiometer.egg-info/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1660 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      695 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/SOURCES.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/dependency_links.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/requires.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/top_level.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-11 16:59:22.216346 alethiometer-1.0.5/setup.cfg
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.5/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 14:17:59.296584 alethiometer-1.0.6/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.6/LICENSE
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2821 2023-04-28 14:17:59.292584 alethiometer-1.0.6/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2112 2023-04-28 14:16:51.000000 alethiometer-1.0.6/README.md
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 14:17:59.292584 alethiometer-1.0.6/alethiometer/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.6/alethiometer/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-28 14:17:24.000000 alethiometer-1.0.6/alethiometer/__version__.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 14:17:59.292584 alethiometer-1.0.6/alethiometer/datasets/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.6/alethiometer/datasets/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.0.6/alethiometer/datasets/dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.6/alethiometer/datasets/h5py_dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.6/alethiometer/datasets/imagenet16.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.6/alethiometer/utils.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4568 2023-04-28 14:08:17.000000 alethiometer-1.0.6/alethiometer/zc_proxy.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 14:17:59.292584 alethiometer-1.0.6/alethiometer/zero_cost_metrics/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1563 2023-04-28 13:56:51.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/grad_norm.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/grasp.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/naswot.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2025 2023-04-28 13:53:18.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/naswot_relu.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4991 2023-04-24 09:28:34.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/ntk.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/snip.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/synflow.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2587 2023-04-23 12:05:16.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/zen.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2412 2023-04-23 12:05:26.000000 alethiometer-1.0.6/alethiometer/zero_cost_metrics/zico.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 14:17:59.292584 alethiometer-1.0.6/alethiometer.egg-info/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2821 2023-04-28 14:17:59.000000 alethiometer-1.0.6/alethiometer.egg-info/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      873 2023-04-28 14:17:59.000000 alethiometer-1.0.6/alethiometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-28 14:17:59.000000 alethiometer-1.0.6/alethiometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-28 14:17:59.000000 alethiometer-1.0.6/alethiometer.egg-info/requires.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-28 14:17:59.000000 alethiometer-1.0.6/alethiometer.egg-info/top_level.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-28 14:17:59.296584 alethiometer-1.0.6/setup.cfg
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.6/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 14:17:59.292584 alethiometer-1.0.6/tests/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1851 2023-04-11 17:20:25.000000 alethiometer-1.0.6/tests/test_zc.py
```

### Comparing `alethiometer-1.0.5/LICENSE` & `alethiometer-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer/datasets/dataset.py` & `alethiometer-1.0.6/alethiometer/datasets/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-07 18:43:32
-LastEditTime: 2023-04-07 19:02:07
+LastEditTime: 2023-04-17 14:10:20
 LastEditors: ViolinSolo
 Description: dataset file from foresight/dataset.py, modified and update with more fns.
 FilePath: /zero-cost-proxies/alethiometer/datasets/dataset.py
 '''
 
 from torch.utils.data import DataLoader
 from torchvision.datasets import MNIST, CIFAR10, CIFAR100, SVHN
@@ -13,15 +13,26 @@
 from torchvision import transforms
 
 from .imagenet16 import *
 
 DATASET_SUPPORTED = ['cifar10', 'cifar100', 'svhn', 'ImageNet16-120', 'ImageNet1k']
 
 def get_cifar_dataloaders(train_batch_size, test_batch_size, dataset, num_workers, resize=None, datadir='_dataset', skip_download_check=False):
+    """
+    get cifar dataset train and test dataloaders.
 
+    :param train_batch_size     is the train dataloader batch size
+    :param test_batch_size      is the test dataloader batch size
+    :param dataset              only support ['cifar10', 'cifar100', 'svhn', 'ImageNet16-120', 'ImageNet1k']
+    :param num_workers          DataLodaer n_workers
+    :param datadir              root dataset dir, storing all dataset data.
+    :param skip_download_check  param to speed up process, skip dataset exist checking, and eliminate the logs
+    
+    :return (train_dataloader, test_dataloader)
+    """
     if dataset not in DATASET_SUPPORTED:
         raise ValueError(f'Check dataset name! "{dataset}" not supported.')
 
     if 'ImageNet16' in dataset:
         mean = [x / 255 for x in [122.68, 116.66, 104.01]]
         std  = [x / 255 for x in [63.22,  61.26 , 65.09]]
         size, pad = 16, 2
```

### Comparing `alethiometer-1.0.5/alethiometer/datasets/h5py_dataset.py` & `alethiometer-1.0.6/alethiometer/datasets/h5py_dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer/datasets/imagenet16.py` & `alethiometer-1.0.6/alethiometer/datasets/imagenet16.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer/utils.py` & `alethiometer-1.0.6/alethiometer/utils.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer/zc_proxy.py` & `alethiometer-1.0.6/alethiometer/zc_proxy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 18:35:04
-LastEditTime: 2023-04-11 17:57:53
+LastEditTime: 2023-04-28 15:08:17
 LastEditors: ViolinSolo
 Description: entry program
 FilePath: /zero-cost-proxies/alethiometer/zc_proxy.py
 '''
 import types
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.data as D
 import numpy as np
+import gc
 
 
 from . import zero_cost_metrics as M
 from .utils import get_some_data
 
 
 ZC_METRIC_SUPPORTED = [
-    '',
-
+    'grad_norm',    # grad_norm
+    'grasp',        # grasp
+    'nwot_relu',    # relu based NASWOT, original implementation
+    'nwot_relu_Kmats',  # return(Kmats, logdet) relu based NASWOT, but return Kmats and its logdet 
+    'nwot',         # our conv and fc based NASWOT
+    'nwot_Kmats',   # return(Kmats, logdet) our conv and fc based NASWOT, but return Kmats and its logdet
+    'lnwot',        # layer-wise our conv and fc based NASWOT
+    'lnwot_Kmats',  # return(Kmats, logdet) layer-wise our conv and fc based NASWOT, but return Kmats and its logdet
+    'snip',         # snip
+    'synflow',      # synflow
+    'synflow_bn',   # synflow with bn
 ]
 
 def no_op(self, x):
     return x
 
 def copynet(self, bn):
     net = copy.deepcopy(self)
@@ -60,20 +70,33 @@
                     metric_vals[mt_name] = val
 
             done = True
         except RuntimeError as e:
             if 'out of memory' in str(e):
                 done=False
                 if ds == inputs.shape[0]//2:
+                    torch.cuda.empty_cache()
+                    gc.collect()
                     raise ValueError(f'Can\'t split data anymore, but still unable to run. Something is wrong') 
                 ds += 1
                 while inputs.shape[0] % ds != 0:
                     ds += 1
                 torch.cuda.empty_cache()
                 print(f'Caught CUDA OOM, retrying with data split into {ds} parts')
+            elif 'Unable to find a valid cuDNN algorithm to run convolution' in str(e):
+                done=False
+                if ds == inputs.shape[0]//2:
+                    torch.cuda.empty_cache()
+                    gc.collect()
+                    raise ValueError(f'Can\'t split data anymore, but still unable to run. Something is wrong') 
+                ds += 1
+                while inputs.shape[0] % ds != 0:
+                    ds += 1
+                torch.cuda.empty_cache()
+                print(f'[no valid cuDNN algorithm found] Caught CUDA OOM, retrying with data split into {ds} parts')
             else:
                 raise e
 
     net_orig = net_orig.to(device).train()
     return metric_vals
```

### Comparing `alethiometer-1.0.5/alethiometer/zero_cost_metrics/grad_norm.py` & `alethiometer-1.0.6/alethiometer/zero_cost_metrics/grad_norm.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer/zero_cost_metrics/grasp.py` & `alethiometer-1.0.6/alethiometer/zero_cost_metrics/grasp.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer/zero_cost_metrics/naswot.py` & `alethiometer-1.0.6/alethiometer/zero_cost_metrics/naswot.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer/zero_cost_metrics/snip.py` & `alethiometer-1.0.6/alethiometer/zero_cost_metrics/snip.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer/zero_cost_metrics/synflow.py` & `alethiometer-1.0.6/alethiometer/zero_cost_metrics/synflow.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.5/alethiometer.egg-info/SOURCES.txt` & `alethiometer-1.0.6/alethiometer.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,14 @@
 alethiometer/datasets/dataset.py
 alethiometer/datasets/h5py_dataset.py
 alethiometer/datasets/imagenet16.py
 alethiometer/zero_cost_metrics/__init__.py
 alethiometer/zero_cost_metrics/grad_norm.py
 alethiometer/zero_cost_metrics/grasp.py
 alethiometer/zero_cost_metrics/naswot.py
+alethiometer/zero_cost_metrics/naswot_relu.py
+alethiometer/zero_cost_metrics/ntk.py
 alethiometer/zero_cost_metrics/snip.py
-alethiometer/zero_cost_metrics/synflow.py
+alethiometer/zero_cost_metrics/synflow.py
+alethiometer/zero_cost_metrics/zen.py
+alethiometer/zero_cost_metrics/zico.py
+tests/test_zc.py
```

### Comparing `alethiometer-1.0.5/setup.py` & `alethiometer-1.0.6/setup.py`

 * *Files identical despite different names*

