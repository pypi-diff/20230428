# Comparing `tmp/depp-0.3.0.tar.gz` & `tmp/depp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depp-0.3.0.tar", last modified: Thu Dec  8 18:48:42 2022, max compression
+gzip compressed data, was "depp-0.3.1.tar", last modified: Thu Apr 27 23:35:57 2023, max compression
```

## Comparing `depp-0.3.0.tar` & `depp-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,48 @@
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2022-12-08 18:48:42.540741 depp-0.3.0/
--rw-r--r--   0 yueyu      (501) staff       (20)      469 2022-12-08 18:48:42.540574 depp-0.3.0/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)       15 2022-12-08 05:14:10.000000 depp-0.3.0/README.md
--rw-r--r--   0 yueyu      (501) staff       (20)     1941 2022-12-08 03:54:04.000000 depp-0.3.0/agg_dist.py
--rw-r--r--   0 yueyu      (501) staff       (20)      577 2022-12-08 03:54:04.000000 depp-0.3.0/comb_json.py
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2022-12-08 18:48:42.539642 depp-0.3.0/depp/
--rw-r--r--   0 yueyu      (501) staff       (20)     4350 2022-12-08 07:03:21.000000 depp-0.3.0/depp/Agg_model.py
--rw-r--r--   0 yueyu      (501) staff       (20)     8431 2022-12-08 07:01:02.000000 depp-0.3.0/depp/Model_pl.py
--rw-r--r--   0 yueyu      (501) staff       (20)    11451 2022-12-08 03:54:04.000000 depp-0.3.0/depp/Model_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)        0 2022-12-08 03:54:04.000000 depp-0.3.0/depp/__init__.py
--rw-r--r--   0 yueyu      (501) staff       (20)      526 2022-12-08 09:46:07.000000 depp-0.3.0/depp/count_gapped_ratio.py
--rw-r--r--   0 yueyu      (501) staff       (20)    12410 2022-12-08 04:25:11.000000 depp-0.3.0/depp/data.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2431 2022-12-08 03:54:04.000000 depp-0.3.0/depp/data.split.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4009 2022-12-08 04:17:46.000000 depp-0.3.0/depp/data_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1620 2022-12-08 07:14:23.000000 depp-0.3.0/depp/default_config.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1655 2022-12-08 07:38:53.000000 depp-0.3.0/depp/depp_distance.py
--rw-r--r--   0 yueyu      (501) staff       (20)      766 2022-12-08 09:41:19.000000 depp-0.3.0/depp/filter_by_entropy_gap.sh
--rw-r--r--   0 yueyu      (501) staff       (20)      782 2022-12-08 09:46:07.000000 depp-0.3.0/depp/get_names_by_entropy_gap.py
--rw-r--r--   0 yueyu      (501) staff       (20)      576 2022-12-08 09:46:07.000000 depp-0.3.0/depp/grep_jplace.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1008 2022-12-08 09:46:07.000000 depp-0.3.0/depp/grep_seq.py
--rw-r--r--   0 yueyu      (501) staff       (20)     7731 2022-12-08 03:54:04.000000 depp-0.3.0/depp/submodule.py
--rw-r--r--   0 yueyu      (501) staff       (20)    27080 2022-12-08 07:43:41.000000 depp-0.3.0/depp/utils.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5457 2022-12-08 05:10:22.000000 depp-0.3.0/depp-place-rRNA-one-type.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     6045 2022-12-08 10:38:29.000000 depp-0.3.0/depp-place-rRNA.sh
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2022-12-08 18:48:42.540379 depp-0.3.0/depp.egg-info/
--rw-r--r--   0 yueyu      (501) staff       (20)      469 2022-12-08 18:48:42.000000 depp-0.3.0/depp.egg-info/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)      670 2022-12-08 18:48:42.000000 depp-0.3.0/depp.egg-info/SOURCES.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2022-12-08 18:48:42.000000 depp-0.3.0/depp.egg-info/dependency_links.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2022-12-08 18:48:36.000000 depp-0.3.0/depp.egg-info/not-zip-safe
--rw-r--r--   0 yueyu      (501) staff       (20)      154 2022-12-08 18:48:42.000000 depp-0.3.0/depp.egg-info/requires.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        5 2022-12-08 18:48:42.000000 depp-0.3.0/depp.egg-info/top_level.txt
--rw-r--r--   0 yueyu      (501) staff       (20)     1149 2022-12-08 03:54:04.000000 depp-0.3.0/merge_json.py
--rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2022-12-08 03:54:01.000000 depp-0.3.0/run_upp.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     2148 2022-12-08 03:54:04.000000 depp-0.3.0/seq_sep.py
--rw-r--r--   0 yueyu      (501) staff       (20)       38 2022-12-08 18:48:42.540791 depp-0.3.0/setup.cfg
--rw-r--r--   0 yueyu      (501) staff       (20)     1768 2022-12-08 18:48:30.000000 depp-0.3.0/setup.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4821 2022-12-08 07:34:47.000000 depp-0.3.0/train_depp.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2796 2022-12-08 03:54:04.000000 depp-0.3.0/train_depp_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5173 2022-12-08 03:54:01.000000 depp-0.3.0/wol_placement.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 23:35:57.983669 depp-0.3.1/
+-rw-r--r--   0 yueyu      (501) staff       (20)      469 2023-04-27 23:35:57.983527 depp-0.3.1/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)       15 2022-12-08 05:14:10.000000 depp-0.3.1/README.md
+-rw-r--r--   0 yueyu      (501) staff       (20)     1941 2022-12-08 03:54:04.000000 depp-0.3.1/agg_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      577 2022-12-08 03:54:04.000000 depp-0.3.1/comb_json.py
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 23:35:57.982548 depp-0.3.1/depp/
+-rw-r--r--   0 yueyu      (501) staff       (20)     5764 2023-02-01 22:01:10.000000 depp-0.3.1/depp/Agg_model.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4909 2023-04-15 21:40:03.000000 depp-0.3.1/depp/Agg_model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     8710 2023-02-01 19:47:27.000000 depp-0.3.1/depp/Model_pl.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    11301 2023-04-20 17:57:40.000000 depp-0.3.1/depp/Model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)        0 2022-12-08 03:54:04.000000 depp-0.3.1/depp/__init__.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1605 2022-12-23 18:59:14.000000 depp-0.3.1/depp/assign_cluster_by_placement.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      526 2022-12-08 09:46:07.000000 depp-0.3.1/depp/count_gapped_ratio.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    12673 2023-01-05 06:08:45.000000 depp-0.3.1/depp/data.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2431 2022-12-08 03:54:04.000000 depp-0.3.1/depp/data.split.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4009 2022-12-08 04:17:46.000000 depp-0.3.1/depp/data_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1730 2023-01-05 18:39:30.000000 depp-0.3.1/depp/default_config.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2433 2023-04-19 17:27:35.000000 depp-0.3.1/depp/depp_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2063 2023-04-19 17:32:01.000000 depp-0.3.1/depp/depp_distance_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      766 2022-12-08 09:41:19.000000 depp-0.3.1/depp/filter_by_entropy_gap.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)      782 2022-12-08 09:46:07.000000 depp-0.3.1/depp/get_names_by_entropy_gap.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      873 2023-04-27 22:18:06.000000 depp-0.3.1/depp/get_tree_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      576 2022-12-08 09:46:07.000000 depp-0.3.1/depp/grep_jplace.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1008 2022-12-08 09:46:07.000000 depp-0.3.1/depp/grep_seq.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      909 2023-04-27 22:17:54.000000 depp-0.3.1/depp/grep_seq_group.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      743 2022-12-23 19:57:48.000000 depp-0.3.1/depp/select_placement.py
+-rw-------   0 yueyu      (501) staff       (20)      895 2023-04-27 22:17:54.000000 depp-0.3.1/depp/select_species_by_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      366 2023-04-27 22:17:54.000000 depp-0.3.1/depp/set_bl_one.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     7731 2022-12-08 03:54:04.000000 depp-0.3.1/depp/submodule.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    32601 2023-04-19 17:28:16.000000 depp-0.3.1/depp/utils.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5802 2023-02-03 22:09:45.000000 depp-0.3.1/depp-place-rRNA-one-type.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     6477 2023-02-25 20:07:16.000000 depp-0.3.1/depp-place-rRNA.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 23:35:57.983341 depp-0.3.1/depp.egg-info/
+-rw-r--r--   0 yueyu      (501) staff       (20)      469 2023-04-27 23:35:57.000000 depp-0.3.1/depp.egg-info/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)      904 2023-04-27 23:35:57.000000 depp-0.3.1/depp.egg-info/SOURCES.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2023-04-27 23:35:57.000000 depp-0.3.1/depp.egg-info/dependency_links.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2023-04-27 23:35:50.000000 depp-0.3.1/depp.egg-info/not-zip-safe
+-rw-r--r--   0 yueyu      (501) staff       (20)      154 2023-04-27 23:35:57.000000 depp-0.3.1/depp.egg-info/requires.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        5 2023-04-27 23:35:57.000000 depp-0.3.1/depp.egg-info/top_level.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)     1149 2022-12-08 03:54:04.000000 depp-0.3.1/merge_json.py
+-rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2022-12-08 03:54:01.000000 depp-0.3.1/run_upp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     2339 2023-02-01 07:34:59.000000 depp-0.3.1/seq_sep.py
+-rw-r--r--   0 yueyu      (501) staff       (20)       38 2023-04-27 23:35:57.983718 depp-0.3.1/setup.cfg
+-rw-r--r--   0 yueyu      (501) staff       (20)     1989 2023-04-27 23:35:23.000000 depp-0.3.1/setup.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     6524 2023-04-27 23:07:34.000000 depp-0.3.1/train_cluster_depp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     4773 2023-02-01 20:15:45.000000 depp-0.3.1/train_depp.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5033 2023-04-19 17:48:08.000000 depp-0.3.1/train_depp_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5173 2022-12-08 03:54:01.000000 depp-0.3.1/wol_placement.sh
```

### Comparing `depp-0.3.0/agg_dist.py` & `depp-0.3.1/agg_dist.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/comb_json.py` & `depp-0.3.1/comb_json.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/Agg_model.py` & `depp-0.3.1/depp/Agg_model_recon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 #!/usr/bin/env python3
+import json
 
 import torch
 import torch.nn as nn
 from depp import utils
-from depp import Model_pl
+from depp import Model_recon
 from pytorch_lightning.core.lightning import LightningModule
 from torch.utils.data import DataLoader
 from typing import List, Dict, Optional, Callable, Union
 import numpy as np
 import math
 import omegaconf
 import sys
 
 
 class model(LightningModule):
-    def __init__(self, args, load_model=False):
+    def __init__(self, args, load_model=False, classifier_cluster_num=None):
         super(model, self).__init__()
         self.save_hyperparameters(args)
         if not self.hparams.sequence_length:
             utils.get_seq_length(self.hparams)
         embedding_size = self.hparams.embedding_size
         self.encoders = []
         for i in range(self.hparams.cluster_num):
             if isinstance(self.hparams.embedding_size, omegaconf.listconfig.ListConfig) or \
                     isinstance(self.hparams.embedding_size, list):
                 self.hparams.embedding_size = embedding_size[i]
-                self.encoders.append(Model_pl.encoder(self.hparams))
+                self.encoders.append(Model_recon.encoder(self.hparams))
                 self.hparams.embedding_size = []
             else:
-                self.encoders.append(Model_pl.encoder(self.hparams))
-        self.classifier = Model_pl.classifier(self.hparams)
+                self.encoders.append(Model_recon.encoder(self.hparams))
+        self.classifier = Model_recon.classifier(self.hparams, cluster_num=classifier_cluster_num)
 
         if load_model:
             for i in range(self.hparams.cluster_num):
                 print(f'loading {i} model...')
                 save_epoch_num = self.hparams.epoch - self.hparams.epoch % 100
-                sub_model = Model_pl.model.load_from_checkpoint(
+                sub_model = Model_recon.model.load_from_checkpoint(
                     f'{self.hparams.model_dir}/{i}/epoch-{save_epoch_num}.pth', current_model=i)
                 # breakpoint()
                 self.encoders[i].load_state_dict(sub_model.encoder.state_dict(), strict=True)
-            classifier = Model_pl.model.load_from_checkpoint(
+            classifier = Model_recon.model.load_from_checkpoint(
                 f'{self.hparams.model_dir}/classifier/epoch-{self.hparams.classifier_epoch - self.hparams.classifier_epoch % 100}.pth', current_model=-1)
             self.classifier.load_state_dict(classifier.classifier.state_dict(), strict=True)
 
         self.hparams.embedding_size = embedding_size
         self.encoders = nn.ModuleList(self.encoders)
         self.channel = 4
         self.hparams.distance_ratio = math.sqrt(float(1.0 / 128 / 10 * float(self.hparams.distance_alpha)))
@@ -57,19 +58,28 @@
             self.training_classifier = False
             self.current_model = -1
         else:
             self.training_classifier = True
             self.current_model = args.start_model_idx
         self.counting = 0
 
+        if load_model:
+            with open(args.cluster_corr, 'r') as f:
+                self.hparams.corr_str = f.read()
+        else:
+            corr = json.loads(self.hparams.corr_str)
+            self.corr = {int(i): torch.tensor(corr[i]) for i in corr}
+
         self.save_hyperparameters(self.hparams)
 
     def forward(self, x, model_idx=None, only_class=False) -> torch.Tensor:
         if self.testing:
             model_prob = self.classifier(x).softmax(-1)
+            model_prob = torch.stack([model_prob[:, self.corr[i]].max(-1)[0] for i in range(self.hparams.cluster_num)], dim=-1)
+            # model_prob = model_prob / model_prob.sum(-1, keepdims=True)
             model_idx = model_prob.argmax(-1)
             if only_class:
                 return model_idx, model_prob
             result_tmp = [self.encoders[model_idx[i]](x[i].unsqueeze(0)) for i in range(len(x))]
             result = np.empty(len(result_tmp), dtype=object)
             result[:] = result_tmp
             return result, model_idx, model_prob
```

### Comparing `depp-0.3.0/depp/Model_pl.py` & `depp-0.3.1/depp/Model_pl.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,41 +43,49 @@
         x = self.celu(self.conv(x))
         x = self.resblocks(x)
         x = self.linear(x).squeeze(-1)
         x = x.view(bs, -1)
         return x
 
 class classifier(nn.Module):
-    def __init__(self, args):
+    def __init__(self, args, cluster_num=None):
         super(classifier, self).__init__()
         channel = 4
 
         self.conv = nn.Conv1d(channel, args.h_channel, 1)
         self.relu = nn.ReLU()
         self.celu = nn.CELU()
         resblocks = []
         for i in range(args.resblock_num):
             resblocks.append(submodule.resblock(args.h_channel,
                                                 args.h_channel,
                                                 5, 0.3))
+
+        if args.classifier_seqdir is not None:
+            seqdir = args.classifier_seqdir
+        else:
+            seqdir = args.seqdir
+        if cluster_num is None:
+            cluster_num = len([i for i in range(len(os.listdir(seqdir))) if os.path.isfile(f'{seqdir}/{i}.fa')])
+
         self.resblocks = nn.Sequential(*resblocks)
 
         self.linear = nn.Conv1d(args.h_channel,
-                                args.cluster_num,
+                                cluster_num,
                                 args.sequence_length)
         self.args = args
         self.train_loss = 0
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         bs, channel, seq_length = x.shape
 
         x = self.celu(self.conv(x))
         x = self.resblocks(x)
         x = self.linear(x).squeeze(-1)
-        x = x.view(bs, self.args.cluster_num)
+        x = x.view(bs, -1)
         return x
 
 
 class model(LightningModule):
     def __init__(self, args, current_model):
         super(model, self).__init__()
         self.save_hyperparameters(args)
```

### Comparing `depp-0.3.0/depp/Model_recon.py` & `depp-0.3.1/depp/Model_recon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,53 @@
 #!/usr/bin/env python3
 
 import torch
 import os
 import math
 import torch.nn as nn
-import submodule
-import data_recon
-import utils
+from depp import submodule
+from depp import data
+from depp import utils
 from pytorch_lightning.core.lightning import LightningModule
 from torch.utils.data import DataLoader
 from typing import List, Dict, Optional, Callable, Union
 from torch.optim.optimizer import Optimizer
 import math
 
+class SeqNet(nn.Module):
+    def __init__(self, args):
+        super(SeqNet, self).__init__()
+        channel = 4
+
+        self.conv = nn.Conv1d(channel, args.h_channel, 1)
+        self.relu = nn.ReLU()
+        self.celu = nn.CELU()
+        resblocks = []
+        for i in range(args.resblock_num):
+            resblocks.append(submodule.resblock(args.h_channel,
+                                                args.h_channel,
+                                                5, 0.3))
+        self.resblocks = nn.Sequential(*resblocks)
+        args.seq_h = int(args.sequence_length * args.seq_h_ratio)
+        self.linear = nn.Conv1d(args.h_channel,
+                                args.seq_h,
+                                args.sequence_length)
+        self.tranconv = nn.ConvTranspose1d(args.seq_h, 4, args.sequence_length)
+        self.args = args
+        self.train_loss = 0
+        print("seq_h", args.seq_h)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        bs, channel, seq_length = x.shape
+
+        x = self.celu(self.conv(x))
+        x = self.resblocks(x)
+        x = self.celu(self.linear(x))
+        x = self.tranconv(x)
+        return x
 
 class encoder(nn.Module):
     def __init__(self, args):
         super(encoder, self).__init__()
         channel = 4
 
         self.conv = nn.Conv1d(channel, args.h_channel, 1)
@@ -28,259 +59,241 @@
                                                 args.h_channel,
                                                 5, 0.3))
         self.resblocks = nn.Sequential(*resblocks)
 
         self.linear = nn.Conv1d(args.h_channel,
                                 args.embedding_size,
                                 args.sequence_length)
+
+        self.seq_net = SeqNet(args)
+        for param in self.seq_net.parameters():
+            param.requires_grad = False
+
         self.args = args
         self.train_loss = 0
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         bs, channel, seq_length = x.shape
 
+        mask = (x == self.args.gap_encode).all(1).unsqueeze(1).repeat(1, 4, 1)
+        recon_x = self.seq_net(x)
+        softmax_recon_x = torch.softmax(recon_x, dim=1)
+        sorted_softmax = softmax_recon_x.sort(dim=1)[0]
+        valid_sites = ((sorted_softmax[:, -1] / sorted_softmax[:, -2]) > 20).unsqueeze(1).repeat(1, 4, 1)
+        x = x.clone()
+        x[mask & valid_sites] = softmax_recon_x[mask & valid_sites]
+
         x = self.celu(self.conv(x))
         x = self.resblocks(x)
         x = self.linear(x).squeeze(-1)
-        x = x.view(bs, self.args.embedding_size)
+        x = x.view(bs, -1)
         return x
-#
-#
-# class SeqNet(nn.Module):
-#     def __init__(self, args):
-#         super(SeqNet, self).__init__()
-#         self.conv1 = nn.Conv1d(4+1, 8, 1)
-#         self.lstm = nn.LSTM(8, 8, 2, batch_first=True, bidirectional=True)
-#         self.conv2 = nn.Conv1d(16, 4, 1)
-#         self.relu = nn.ReLU()
-#
-#     def forward(self, x):
-#         n, chn, l = x.shape
-#         # idx = torch.zeros(n, l, l).to(x.device)
-#         idx = torch.arange(0, l).to(x.device).view(1, 1, -1).repeat(len(x), 1, 1) * 0.01
-#         # idx[:, torch.arange(0, l), torch.arange(0, l)] = 1
-#         x = torch.cat([x, idx], dim=1)
-#         x = self.relu(self.conv1(x))
-#         x = self.lstm(x.permute(0, 2, 1))
-#         x = self.conv2(x[0].permute(0, 2, 1))
-#         return x
 
-class SeqNet(nn.Module):
-    def __init__(self, args):
-        super(SeqNet, self).__init__()
+class classifier(nn.Module):
+    def __init__(self, args, cluster_num=None):
+        super(classifier, self).__init__()
         channel = 4
 
         self.conv = nn.Conv1d(channel, args.h_channel, 1)
         self.relu = nn.ReLU()
         self.celu = nn.CELU()
         resblocks = []
         for i in range(args.resblock_num):
             resblocks.append(submodule.resblock(args.h_channel,
                                                 args.h_channel,
                                                 5, 0.3))
+
+        if args.classifier_seqdir is not None:
+            seqdir = args.classifier_seqdir
+        else:
+            seqdir = args.seqdir
+        if cluster_num is None:
+            cluster_num = len([i for i in range(len(os.listdir(seqdir))) if os.path.isfile(f'{seqdir}/{i}.fa')])
+
         self.resblocks = nn.Sequential(*resblocks)
-        args.seq_h = int(args.sequence_length * args.seq_h_ratio)
+
         self.linear = nn.Conv1d(args.h_channel,
-                                args.seq_h,
+                                cluster_num,
                                 args.sequence_length)
-        self.tranconv = nn.ConvTranspose1d(args.seq_h, 4, args.sequence_length)
+
+        self.seq_net = SeqNet(args)
+        for param in self.seq_net.parameters():
+            param.requires_grad = False
+
         self.args = args
         self.train_loss = 0
-        print("seq_h", args.seq_h)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         bs, channel, seq_length = x.shape
 
+        mask = (x == self.args.gap_encode).all(1).unsqueeze(1).repeat(1, 4, 1)
+        recon_x = self.seq_net(x)
+        softmax_recon_x = torch.softmax(recon_x, dim=1)
+        sorted_softmax = softmax_recon_x.sort(dim=1)[0]
+        valid_sites = ((sorted_softmax[:, -1] / sorted_softmax[:, -2]) > 20).unsqueeze(1).repeat(1, 4, 1)
+        x = x.clone()
+        x[mask & valid_sites] = softmax_recon_x[mask & valid_sites]
+
         x = self.celu(self.conv(x))
         x = self.resblocks(x)
-        x = self.celu(self.linear(x))
-        x = self.tranconv(x)
+        x = self.linear(x).squeeze(-1)
+        x = x.view(bs, -1)
         return x
 
-# class SeqNet(nn.Module):
-#     def __init__(self, args):
-#         super(SeqNet, self).__init__()
-#         self.encoder = nn.Sequential(
-#             nn.Conv1d(5, 16, 5, stride=2),
-#             nn.ReLU(),
-#             nn.Conv1d(16, 32, 5, stride=2),
-#             nn.ReLU(),
-#             nn.Conv1d(32, 64, 5, stride=2),
-#             nn.ReLU(),
-#             nn.Conv1d(64, 128, 5, stride=2),
-#             nn.ReLU(),
-#             nn.Conv1d(128, 128, 5, stride=2),
-#             nn.ReLU()
-#         )
-#         self.lstm = nn.LSTM(128, 128, 1, batch_first=True, bidirectional=True)
-#         self.decoder = nn.Sequential(
-#             nn.ConvTranspose1d(128*2, 128, 5, stride=2, padding=0, output_padding=0),
-#             nn.ReLU(),
-#             nn.ConvTranspose1d(128, 64, 5, stride=2, padding=0, output_padding=0),
-#             nn.ReLU(),
-#             nn.ConvTranspose1d(64, 32, 5, stride=2, padding=0, output_padding=1),
-#             nn.ReLU(),
-#             nn.ConvTranspose1d(32, 16, 5, stride=2, padding=0, output_padding=0),
-#             nn.ReLU(),
-#             nn.ConvTranspose1d(16, 16, 5, stride=2, padding=0, output_padding=0),
-#             nn.ReLU(),
-#             nn.Conv1d(16, 4, 1)
-#         )
-#         self.L = args.sequence_length
-#
-#     def forward(self, x):
-#         idx = torch.arange(0, self.L).to(x.device).view(1, 1, -1).repeat(len(x), 1, 1) * 0.01
-#                 # idx[:, torch.arange(0, l), torch.arange(0, l)] = 1
-#         x = torch.cat([x, idx], dim=1)
-#         x = self.encoder(x)
-#         x = self.lstm(x.permute(0, 2, 1))
-#         x = self.decoder(x[0].permute(0, 2, 1))
-#         # x = self.decoder(x)
-#         if self.L % 2 == 0:
-#             x = x[:, :, :-1]
-#         return x
-
 class model(LightningModule):
-    def __init__(self, args):
+    def __init__(self, args, current_model):
         super(model, self).__init__()
         self.save_hyperparameters(args)
         if not self.hparams.sequence_length:
             utils.get_seq_length(self.hparams)
-        self.save_hyperparameters(self.hparams)
-        self.encoder = encoder(self.hparams)
+
+        if current_model != -1:
+            embedding_size = self.hparams.embedding_size
+            self.hparams.embedding_size = embedding_size[current_model]
+            self.encoder = encoder(self.hparams)
+            self.hparams.embedding_size = embedding_size
+        else:
+            self.classifier = classifier(self.hparams)
         self.channel = 4
-        self.hparams.distance_ratio = math.sqrt(
-            float(1.0 / float(self.hparams.embedding_size) / 10 * float(self.hparams.distance_alpha)))
+        self.hparams.distance_ratio = math.sqrt(float(1.0 / 128 / 10 * float(self.hparams.distance_alpha)))
 
         self.dis_loss_w = 100
         self.train_loss = []
         self.val_loss = float('inf')
-        self.seq_net = SeqNet(self.hparams)
-        self.running_recon_loss = 0
-        self.reconseq = []
-        self.wrong_site = []
-        self.is_training = True
-        self.cnt = []
 
-    def forward(self, x: torch.Tensor, train_sn=False, mask=None) -> torch.Tensor:
-        recon_x = self.seq_net(x)
-        softmax_recon_x = torch.softmax(recon_x, dim=1)
-        if not train_sn:
-            softmax_recon_x[mask.repeat(1, 4, 1)] = x[mask.repeat(1, 4, 1)]
-        encoding = self.encoder(softmax_recon_x)
-        if self.is_training:
-            return recon_x, encoding
+        self.testing = False
+        if current_model == -1:
+            self.training_classifier = True
         else:
-            return encoding
+            self.training_classifier = False
+        self.current_model = current_model
+        self.counting = 0
+
+        self.save_hyperparameters(self.hparams)
+
+    def forward(self, x, model_idx=None) -> torch.Tensor:
+        if self.training_classifier:
+            return self.classifier(x)
+        return self.encoder(x)
 
     def training_step(self, batch, batch_idx):
+
         nodes = batch['nodes']
         seq = batch['seqs'].float()
-        masked_seq = batch['masked_seqs'].float()
-        mask = batch['mask']
+        model_idx = batch['cluster_idx'].long()
         device = seq.device
 
-        if self.trainer.current_epoch < self.hparams.ae_train_epoch:
-            reconseq, _ = self(masked_seq, train_sn=True)
-            n, chn, l = reconseq.shape
-            reconseq = reconseq.permute(0, 2, 1).reshape(n*l, chn)
-            mask = mask.permute(0, 2, 1).reshape(n*l, -1).squeeze(-1)
-            seq = seq.permute(0, 2, 1).reshape(n*l, chn)
-            loss = nn.functional.cross_entropy(reconseq[mask, :], torch.argmax(seq[mask, :], dim=-1))
-            self.running_recon_loss += loss
-            if self.trainer.current_epoch % 10 == 0:
-                self.reconseq.append(reconseq.flatten())
-                wrong_site = (torch.argmax(reconseq[mask, :], dim=-1) != torch.argmax(seq[mask, :], dim=-1)).sum() / mask.sum()
-                self.wrong_site.append(wrong_site)
+        if self.training_classifier:
+            c = self(seq)
+            loss = nn.functional.cross_entropy(c, model_idx)
+            self.val_loss += loss
+            return {'loss': loss}
         else:
-            self.train_data.train_recon = False
-            _, encoding = self(masked_seq, mask=mask)
+            encoding = self(seq, model_idx[0])
             gt_distance = self.train_data.true_distance(nodes, nodes).to(device)
 
-            distance = utils.distance(encoding, encoding.detach(),
-                                      self.hparams.distance_mode) * self.hparams.distance_ratio
+            distance = utils.distance(encoding, encoding.detach(), self.hparams.distance_mode) * self.hparams.distance_ratio
 
             not_self = torch.ones_like(distance)
             not_self[torch.arange(0, len(distance)), torch.arange(0, len(distance))] = 0
 
             dis_loss = utils.mse_loss(distance[not_self == 1], gt_distance[not_self == 1], self.hparams.weighted_method)
             loss = self.dis_loss_w * dis_loss * self.hparams.dis_loss_ratio
+
+            if loss.isnan().any():
+                breakpoint()
+
             self.val_loss += loss
 
-        return {'loss': loss}
+            return {'loss': loss}
 
     def training_epoch_end(
             self,
             outputs: Union[List[Dict[str, torch.Tensor]], List[List[Dict[str, torch.Tensor]]]]
     ) -> Dict[str, Dict[str, torch.Tensor]]:
         self.dis_loss_w = 100 + 1e-3 * (self.trainer.current_epoch - 1e4) * (self.trainer.current_epoch > 1e4)
+        self.counting += 1
         if self.trainer.current_epoch % 100 == 0:
-            self.trainer.save_checkpoint(f'{self.hparams.model_dir}/epoch-{self.trainer.current_epoch}.pth')
-            #if self.trainer.current_epoch > 0:
-            #    os.remove(f'{self.hparams.model_dir}/epoch-{self.trainer.current_epoch - 100}.pth')
-    def on_train_epoch_start(self):
-        if self.trainer.current_epoch == self.hparams.ae_train_epoch:
-            self.seq_net.requires_grad_(False)
-            self.train_data.train_encoder = False
-
+            if self.training_classifier:
+                subdir = 'classifier'
+            else:
+                subdir = self.current_model
+            os.makedirs(f'{self.hparams.model_dir}/{subdir}', exist_ok=True)
+            self.trainer.save_checkpoint(f'{self.hparams.model_dir}/{subdir}/epoch-{self.trainer.current_epoch}.pth')
+            if self.trainer.current_epoch > 0:
+                try:
+                    os.remove(f'{self.hparams.model_dir}/{subdir}/epoch-{self.trainer.current_epoch - 100}.pth')
+                except:
+                    pass
 
     def configure_optimizers(self):
-        return torch.optim.RMSprop(self.parameters(), lr=self.hparams.lr)
+        if self.current_model == -1:
+            params = list(self.classifier.conv.parameters()) + list(self.classifier.resblocks.parameters()) + list(self.classifier.linear.parameters())
+        else:
+            params = list(self.encoder.conv.parameters()) + list(self.encoder.resblocks.parameters()) + list(self.encoder.linear.parameters())
+        return torch.optim.Adam(params,
+                                lr=self.hparams.lr)
 
     def train_dataloader(self) -> DataLoader:
+        # self.train_data = self.train_data_list[0]
         loader = DataLoader(self.train_data,
                             batch_size=self.hparams.batch_size,
                             num_workers=self.hparams.num_worker,
                             shuffle=True,
                             drop_last=True)
         return loader
 
     def validation_step(self, batch, batch_idx):
         return {}
 
     def validation_epoch_end(self, outputs):
         val_loss = self.val_loss
-        if self.trainer.current_epoch > 0 and self.trainer.current_epoch < self.hparams.ae_train_epoch:
-            # self.logger.experiment.add_scalar('recon_loss', self.running_recon_loss, self.trainer.current_epoch)
-            # self.logger.experiment.add_histogram('recon_seq', torch.sigmoid(torch.cat(self.reconseq)), self.trainer.current_epoch)
-            # self.logger.experiment.add_histogram('wrong_site', torch.tensor(self.wrong_site), self.trainer.current_epoch)
-            self.running_recon_loss = 0
-            self.reconseq = []
-            self.wrong_site = []
-        self.log('val_loss', val_loss)
         self.val_loss = 0
+        self.log('val_loss', val_loss)
 
     def val_dataloader(self):
         # TODO: do a real train/val split
-        self.train_data = data_recon.data(self.hparams, calculate_distance_matrix=True)
+        # self.train_data = data.data(self.hparams, calculate_distance_matrix=True)
+        # self.train_data_list = data.make_datalist(self.hparams)
+        if not self.training_classifier:
+            print(f'training {self.current_model} model...')
+            self.train_data = data.get_data(self.current_model, self.hparams)
+        else:
+            # self.train_data = self.train_data_list[-1]
+            print(f'training classifier...')
+            self.train_data = data.get_data(-1, self.hparams)
         loader = DataLoader(self.train_data,
                             batch_size=self.hparams.batch_size,
                             shuffle=False,
                             num_workers=self.hparams.num_worker,
-                            drop_last=False)
+                            drop_last=True)
         return loader
 
     def optimizer_step(
             self,
             epoch: int,
             batch_idx: int,
             optimizer: Optimizer,
             optimizer_idx: int,
             optimizer_closure: Optional[Callable] = None,
             on_tpu: bool = False,
             using_native_amp: bool = False,
             using_lbfgs: bool = False,
     ) -> None:
 
-        if self.trainer.global_step % self.hparams.lr_update_freq == 0:
-
-            #lr = 3e-5 + self.hparams.lr * (0.1 ** (epoch / self.hparams.lr_decay))
-            lr = 3e-5 + self.hparams.lr * (0.1 ** (epoch / self.hparams.lr_decay))
+        if self.counting == self.hparams.lr_update_freq:
+            # if (epoch + 1) % self.hparams.lr_decay == 0:
+            # lr = 3e-5 + self.hparams.lr * (0.1 ** ((self.trainer.current_epoch + 1) / self.hparams.lr_decay))
+            # print('lr', lr)
             for param_group in optimizer.param_groups:
-                param_group['lr'] = lr
+                param_group['lr'] = param_group['lr'] * 0.1 + 2e-5
+            print('lr', param_group['lr'])
+            print(self.counting, self.hparams.lr_update_freq)
+            self.counting = 0
+
 
         super(model, self).optimizer_step(
             epoch,
             batch_idx,
             optimizer,
             optimizer_idx,
             optimizer_closure,
```

### Comparing `depp-0.3.0/depp/count_gapped_ratio.py` & `depp-0.3.1/depp/count_gapped_ratio.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/data.py` & `depp-0.3.1/depp/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,17 +104,23 @@
     def __init__(self, args, calculate_distance_matrix=False):
         self.args = args
 
         self.total_seq = 0
         self.all_seq = {}
         self.all_nodes = []
         self.all_idx = []
-        for i in range(args.cluster_num):
+        if args.classifier_seqdir is not None:
+            seqdir = args.classifier_seqdir
+        else:
+            seqdir = args.seqdir
+        print(f'classifier seqdir: {seqdir}')
+        cluster = [i for i in range(len(os.listdir(seqdir))) if os.path.isfile(f'{seqdir}/{i}.fa')]
+        for i in cluster:
             print(f'loading sequences {i}...')
-            backbone_seq_file = f'{args.seqdir}/{i}.fa'
+            backbone_seq_file = f'{seqdir}/{i}.fa'
             self_seq = SeqIO.to_dict(SeqIO.parse(backbone_seq_file, "fasta"))
             args.sequence_length = len(list(self_seq.values())[0])
             L = args.sequence_length
             nodes, seq, mask = utils.process_seq(self_seq, args, True, True)
             self.all_nodes += list(nodes)
             self.all_seq.update(dict(zip(nodes, seq)))
             self.all_idx += [i] * len(seq)
```

### Comparing `depp-0.3.0/depp/data.split.py` & `depp-0.3.1/depp/data.split.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/data_recon.py` & `depp-0.3.1/depp/data_recon.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/default_config.py` & `depp-0.3.1/depp/default_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,20 @@
 'load_model': None,
 'add_random_mask': False,
 'get_representative_emb': False,
 'start_model_idx': -1,
 'only_class': False,
 'end_model_idx': None,
 'cluster_num': 1,
-'seqdir': None
+'seqdir': None,
+'use_cluster': None,
+'classifier_seqdir': None,
+'use_multi_class': None,
+'prob_thr': 5,
+'cluster_corr': None
 }
 
 #def get_cfg_defaults():
 #    """Get a yacs CfgNode object with default values for my_project."""
 #    # Return a clone so that the defaults will not be altered
 #    # This is for the "local variable" use pattern
 #    return _C.clone()
```

### Comparing `depp-0.3.0/depp/depp_distance.py` & `depp-0.3.1/depp/depp_distance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python3
 
 import os
 import sys
+import torch
+import numpy as np
 # import Model_pl
 from depp import Agg_model
+from depp import Agg_model_recon
 from depp import Model_pl
 from depp import utils
 from depp import default_config
 from omegaconf import OmegaConf
 
 os.environ['OMP_NUM_THREADS'] = '1'
 os.environ['MKL_NUM_THREADS'] = '1'
@@ -23,29 +26,41 @@
     #     args_base.exp_name = os.path.splitext(os.path.basename(args_cli.config_file))[0]
     # elif args_cli.exp_name is None:
     #     raise ValueError('exp_name cannot be empty without specifying a config file')
     # del args_cli['config_file']
     args = OmegaConf.merge(args_base, args_cli)
     cluster_model = True
     try:
-        model = Agg_model.model.load_from_checkpoint(args.model_path, load_model=False)
+        if not torch.cuda.is_available():
+            m = torch.load(args.model_path, map_location=torch.device('cpu'))
+        else:
+            m = torch.load(args.model_path)
+        classifier_cluster_num = m['state_dict']['classifier.linear.bias'].shape[0]
+        model = Agg_model.model.load_from_checkpoint(args.model_path, load_model=False, classifier_cluster_num=classifier_cluster_num)
+
+        if not args.recon_model_path is None:
+            recon_model = Agg_model_recon.model.load_from_checkpoint(args.recon_model_path, load_model=False, classifier_cluster_num=classifier_cluster_num)
+
     except:
         cluster_model = False
         try:
             model = Model_pl.model.load_from_checkpoint(args.model_path, current_model=0)
         except:
             print(f'cannot load model {args.model_path}')
             sys.exit()
     # if args.recon_model_path:
     #     recon_model = Model_recon.model.load_from_checkpoint(args.recon_model_path)
     #     recon_model.is_training=False
     # else:
     #     recon_model = None
     if cluster_model:
-        utils.save_depp_dist_cluster(model, args)
+        if args.recon_model_path is None:
+            utils.save_depp_dist_cluster(model, args, use_cluster=args.use_cluster)
+        else:
+            utils.save_depp_dist_cluster(model, args, use_cluster=args.use_cluster, recon_model=recon_model)
     else:
         utils.save_depp_dist(model, args)
 
     if args.get_representative_emb:
         utils.save_repr_emb(model, args)
 
 if __name__ == '__main__':
```

### Comparing `depp-0.3.0/depp/filter_by_entropy_gap.sh` & `depp-0.3.1/depp/filter_by_entropy_gap.sh`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/get_names_by_entropy_gap.py` & `depp-0.3.1/depp/get_names_by_entropy_gap.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/grep_jplace.py` & `depp-0.3.1/depp/grep_jplace.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/grep_seq.py` & `depp-0.3.1/depp/grep_seq.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/submodule.py` & `depp-0.3.1/depp/submodule.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/depp/utils.py` & `depp-0.3.1/depp/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import collections
 
 import torch
 import os
 import pandas as pd
 import math
 import numpy as np
 import dendropy
@@ -57,14 +58,15 @@
         cosine = torch.nn.functional.cosine_similarity(nodes1, nodes2, dim=-1)
         return (1 - cosine ** 2) / (cosine + 1e-9)
     elif mode == 'hyperbolic':
         nodes1 = nodes1.squeeze(1)
         nodes2 = nodes2.squeeze(0)
         return hyp_dist(nodes1, nodes2)
 
+
 def project_hyperbolic(x):
     N, d = x.shape[0], x.shape[1]
 
     hnorm_x = torch.norm(x, dim=1, p=2, keepdim=True)
 
     s1 = torch.cosh(hnorm_x)
     s2 = torch.div(torch.sinh(hnorm_x), hnorm_x)
@@ -87,14 +89,15 @@
     H = torch.eye(d + 1, d + 1).to(x1.device)
     H[0, 0] = -1
     N1, N2 = x1.shape[0], x2.shape[0]
     G = torch.matmul(torch.matmul(x1, H), torch.transpose(x2, 0, 1))
     G[G >= -1] = -1
     return torch.acosh(-G)
 
+
 def distance(nodes1, nodes2, mode):
     # node1: query
     # node2: backbone
     dist = torch.cat([torch.cat(
         [distance_portion(nodes1[j * 100: (j + 1) * 100], nodes2[i * 100: (i + 1) * 100], mode) for j in
          range(math.ceil(len(nodes1) / 100))],
         dim=0) for i in range(math.ceil(len(nodes2) / 100))], dim=1)
@@ -230,14 +233,15 @@
             mask = np.concatenate([i.reshape(1, 1, -1) for i in mask_df['masks'].values])
         names = comb_names
 
     if need_mask:
         return names, torch.from_numpy(seqs), torch.from_numpy(mask).bool()
     return names, torch.from_numpy(seqs)
 
+
 def get_embeddings_cluster(seqs, model, query=True, model_idx=None, only_class=False):
     with torch.no_grad():
         if query:
             model.testing = True
             if only_class:
                 idxs = []
                 idxs_probs = []
@@ -266,128 +270,230 @@
             encodings = []
             for i in range(math.ceil(len(seqs) / 2000.0)):
                 encodings_tmp = model(seqs[i * 2000: (i + 1) * 2000].float(), model_idx).detach()
                 encodings.append(encodings_tmp)
             encodings = torch.cat(encodings, dim=0)
             return encodings
 
-def save_depp_dist_cluster(model, args):
+def save_dataframe(data_origin, outfile):
+    data_origin = data_origin.astype(str)
+    data_origin = "\t" + "\t".join(data_origin.keys().astype(str)) + "\n" + \
+                  "\n".join([str(k) + "\t" + "\t".join(data_origin.loc[k].values) for k in
+                             data_origin.index]) + "\n"
+    with open(outfile, 'w') as f:
+        f.write(data_origin)
+
+# @profile
+def save_depp_dist_cluster(model, args, use_cluster=None, recon_model=None):
     t1 = time.time()
     os.makedirs(args.outdir, exist_ok=True)
     query_seq_file = args.query_seq_file
+    args.replicate_seq = model.hparams.replicate_seq
     query_seq = SeqIO.to_dict(SeqIO.parse(query_seq_file, "fasta"))
     query_seq_names, query_seq_tensor = process_seq(query_seq, args, isbackbone=False, need_mask=False)
     print('calculating query embeddings...')
     if args.only_class:
-        query_idxs, query_idxs_probs = get_embeddings_cluster(query_seq_tensor, model, query=True, only_class=True)
+        if recon_model is None:
+            query_idxs, query_idxs_probs = get_embeddings_cluster(query_seq_tensor, model, query=True, only_class=True)
+        else:
+            query_idxs, query_idxs_probs = get_embeddings_cluster(query_seq_tensor, recon_model, query=True, only_class=True)
         with open(f'{args.outdir}/class.json', 'w') as f:
             tmp_class = dict(zip(query_seq_names, list(query_idxs.numpy().astype(int))))
             tmp_class = {i: int(tmp_class[i]) for i in tmp_class}
             json.dump(tmp_class, f, sort_keys=True, indent=4)
+        torch.save(query_idxs_probs, f'{args.outdir}/class_prob.pt')
+        torch.save(query_seq_names, f'{args.outdir}/query_seq_names.pt')
         t2 = time.time()
         print('finish! take {:.2f} seconds.'.format(t2 - t1))
         return
         # torch.save(query_idxs_probs, f'{args.outdir}/class_probs.pt')
         # torch.save(query_seq_names, f'{args.outdir}/query_labels.pt')
 
-    query_encodings, query_idxs, query_idxs_probs = get_embeddings_cluster(query_seq_tensor, model, query=True)
-    query_encodings_dict = {i: torch.cat(list(query_encodings[query_idxs == i])) for i in range(model.hparams.cluster_num) if (query_idxs == i).sum() > 0}
-    query_names_dict = {i: list(np.array(query_seq_names)[query_idxs == i]) for i in range(model.hparams.cluster_num) if (query_idxs == i).sum() > 0}
-    # torch.save(query_idxs_probs, f'{args.outdir}/class_probs.pt')
-    # torch.save(query_seq_names, f'{args.outdir}/query_labels.pt')
-    entropy = scipy.stats.entropy(query_idxs_probs, axis=-1)
-    entropy_s = [f'{query_seq_names[i]}\t{entropy[i]}\n' for i in range(len(entropy))]
-    entropy_s = "".join(entropy_s)
-    with open(f'{args.outdir}/entropy.txt', 'w') as f:
-        f.write(entropy_s)
+    if use_cluster is None:
 
-    print('calculating backbone embeddings...')
+        if args.use_multi_class:
+            query_idxs, query_idxs_probs = get_embeddings_cluster(query_seq_tensor, model, query=True, only_class=True)
+            sorted_probs, sorted_probs_idx = torch.sort(query_idxs_probs, dim=-1, descending=True)
+            add_class_idx = (sorted_probs[:, 0] / sorted_probs[:, 1]) < args.prob_thr
+            add_class_idx_third = ((sorted_probs[:, 1] / sorted_probs[:, 2]) < args.prob_thr) & add_class_idx
+            add_class_idx_forth = ((sorted_probs[:, 2] / sorted_probs[:, 3]) < args.prob_thr) & add_class_idx_third
+
+            cluster_idxs = {}
+            for i in range(model.hparams.cluster_num):
+                idx1 = sorted_probs_idx[:, 0] == i
+                idx2 = (sorted_probs_idx[:, 1] == i) & add_class_idx
+                idx3 = (sorted_probs_idx[:, 2] == i) & add_class_idx_third
+                idx4 = (sorted_probs_idx[:, 3] == i) & add_class_idx_forth
+                idx_all = idx1 | idx2 | idx3 | idx4
+                if idx_all.sum() > 0:
+                    cluster_idxs[i] = torch.arange(0, len(query_seq_tensor))[idx1 | idx2 | idx3 | idx4]
+
+            query_encodings_dict = {i: get_embeddings_cluster(
+                query_seq_tensor[cluster_idxs[i]],
+                model,
+                query=False,
+                model_idx=i
+                ) for i in cluster_idxs}
+            query_names_dict = {i: list(np.array(query_seq_names)[cluster_idxs[i]]) if len(cluster_idxs[i]) > 1
+                                            else [np.array(query_seq_names)[cluster_idxs[i]]] for i in cluster_idxs}
+        else:
+            query_encodings, query_idxs, query_idxs_probs = get_embeddings_cluster(query_seq_tensor, model, query=True)
+            if len(query_encodings) == 1:
+                query_encodings_dict = {query_idxs[0].item(): query_encodings[0]}
+                query_names_dict = {query_idxs[0].item(): query_seq_names}
+            else:
+                query_encodings_dict = {i: torch.cat(list(query_encodings[query_idxs == i])) for i in
+                                        range(model.hparams.cluster_num) if (query_idxs == i).sum() > 0}
+                query_names_dict = {i: list(np.array(query_seq_names)[query_idxs == i]) for i in
+                                    range(model.hparams.cluster_num) if (query_idxs == i).sum() > 0}
+        # torch.save(query_idxs_probs, f'{args.outdir}/class_probs.pt')
+        # torch.save(query_seq_names, f'{args.outdir}/query_labels.pt')
+        entropy = scipy.stats.entropy(query_idxs_probs, axis=-1)
+        entropy_s = [f'{query_seq_names[i]}\t{entropy[i]}\n' for i in range(len(entropy))]
+        entropy_s = "".join(entropy_s)
+        with open(f'{args.outdir}/entropy.txt', 'w') as f:
+            f.write(entropy_s)
+        torch.save(query_idxs_probs, f'{args.outdir}/prob.pt')
 
+    else:
+        query_encodings = get_embeddings_cluster(query_seq_tensor, model, query=False, model_idx=use_cluster)
+        query_encodings_dict = {use_cluster: query_encodings}
+        query_names_dict = {use_cluster: query_seq_names}
+    t2 = time.time()
+    print('finish query embeddings calculation! use {:.2f} seconds.'.format(t2 - t1))
+    print('calculating backbone embeddings...')
+    t3 = time.time()
     def get_backbone_embeddings(i):
         backbone_seq_file = f"{args.seqdir}/{i}.fa"
         backbone_seq = SeqIO.to_dict(SeqIO.parse(backbone_seq_file, "fasta"))
         backbone_seq_names, backbone_seq_tensor = process_seq(backbone_seq, args, isbackbone=True)
         backbone_encodings = get_embeddings_cluster(backbone_seq_tensor, model, query=False, model_idx=i)
         return backbone_encodings, backbone_seq_names
 
     if args.backbone_emb is None:
-        backbone_embs_names_tmp = [get_backbone_embeddings(i) for i in range(model.hparams.cluster_num)]
+        if use_cluster is None:
+            backbone_embs_names_tmp = [get_backbone_embeddings(i) for i in range(model.hparams.cluster_num)]
+        else:
+            backbone_embs_names_tmp = [get_backbone_embeddings(use_cluster)]
 
-        backbone_encodings_dict = {i: backbone_embs_names_tmp[i][0] for i in range(model.hparams.cluster_num)}
-        backbone_names_dict = {i: backbone_embs_names_tmp[i][1] for i in range(model.hparams.cluster_num)}
+        if use_cluster is None:
+            backbone_encodings_dict = {i: backbone_embs_names_tmp[i][0] for i in range(model.hparams.cluster_num)}
+            backbone_names_dict = {i: backbone_embs_names_tmp[i][1] for i in range(model.hparams.cluster_num)}
+        else:
+            backbone_encodings_dict = {use_cluster: backbone_embs_names_tmp[0][0]}
+            backbone_names_dict = {use_cluster: backbone_embs_names_tmp[0][1]}
         torch.save(backbone_encodings_dict, f'{args.outdir}/backbone_emb.pt')
         torch.save(backbone_names_dict, f'{args.outdir}/backbone_ids.pt')
     else:
         backbone_names_dict = torch.load(args.backbone_id)
         backbone_encodings_dict = torch.load(args.backbone_emb)
-
+    print('finish backbone embedding calculation! use {:.2f} seconds.'.format(t3 - t2))
     print('calculating distance matrix...')
-    for i in query_encodings_dict.keys():
-        query_dist = distance(query_encodings_dict[i], backbone_encodings_dict[i], args.distance_mode) * model.hparams.distance_ratio
+    query_dist_dict = {}
+
+    for i in query_encodings_dict:
+        query_dist = distance(query_encodings_dict[i], backbone_encodings_dict[i],
+                              args.distance_mode) * model.hparams.distance_ratio
         if 'square_root' in args.weighted_method:
             query_dist = query_dist ** 2
         query_dist = np.array(query_dist)
         query_dist[query_dist < 1e-3] = 0
-        data_origin = dict(zip(query_names_dict[i], list(query_dist.astype(str))))
-        data_origin = "\t" + "\t".join(backbone_names_dict[i]) + "\n" + \
-                      "\n".join([str(k) + "\t" + "\t".join(data_origin[k]) for k in data_origin]) + "\n"
-        t4 = time.time()
+        query_dist_dict[i] = query_dist
+    t4 = time.time()
+    print('finish distance calculation! use {:.2f} seconds.'.format(t4 - t3))
+
+    if args.use_multi_class:
+        query_dist_df_dict = \
+            {i: pd.DataFrame.from_dict(dict(zip(query_names_dict[i], list(query_dist_dict[i])))) for i in query_dist_dict}
+        for i in query_dist_df_dict:
+            query_dist_df_dict[i].index = backbone_names_dict[i]
+
+        for name_idx in range(math.ceil(len(query_seq_names) / 200)):
+            cur_names = query_seq_names[name_idx*200: (name_idx+1)*200]
+            data_origin = None
+            for i in query_dist_dict:
+                inter_names = list(set(cur_names).intersection(set(query_dist_df_dict[i].keys())))
+                if len(inter_names) == 0:
+                    continue
+                if data_origin is None:
+                    data_origin = query_dist_df_dict[i][inter_names]
+                else:
+                    data_origin = pd.concat([data_origin, query_dist_df_dict[i][inter_names]], axis=0)
+            data_origin = data_origin.groupby(lambda x: x).median()
+            data_origin = data_origin.fillna(-1)
+            save_dataframe(data_origin.transpose(), f"{args.outdir}/depp{name_idx}.csv")
+    else:
+        for i in model.hparams.cluster_num:
+            data_origin = dict(zip(query_names_dict[i], list(query_dist_dict[i].astype(str))))
+            data_origin = "\t" + "\t".join(backbone_names_dict[i]) + "\n" + \
+                          "\n".join([str(k) + "\t" + "\t".join(data_origin[k]) for k in data_origin]) + "\n"
+            with open(f"{args.outdir}/depp{i}.csv", 'w') as f:
+                f.write(data_origin)
+
         # print('convert string', t4 - t3)
-        with open(os.path.join(args.outdir, f'depp{i}.csv'), 'w') as f:
-            f.write(data_origin)
+        # with open(os.path.join(args.outdir, f'depp{i}.csv'), 'w') as f:
+        #     f.write(data_origin)
     t2 = time.time()
     print('finish! take {:.2f} seconds.'.format(t2 - t1))
 
+
 def get_embeddings(seqs, model, mask=None):
     encodings = []
     for i in range(math.ceil(len(seqs) / 2000.0)):
         if not (mask is None):
             encodings_tmp = model(seqs[i * 2000: (i + 1) * 2000].float(), mask=mask[i * 2000: (i + 1) * 2000]).detach()
         else:
             encodings_tmp = model(seqs[i * 2000: (i + 1) * 2000].float()).detach()
         encodings.append(encodings_tmp)
     encodings = torch.cat(encodings, dim=0)
     return encodings
 
+
 def save_depp_dist(model, args, recon_model=None):
     t1 = time.time()
     model.eval()
     print('processing data...')
     args.replicate_seq = model.hparams.replicate_seq
     backbone_seq_file = args.backbone_seq_file
     query_seq_file = args.query_seq_file
     dis_file_root = os.path.join(args.outdir)
     # args.distance_ratio = float(1.0 / float(args.embedding_size) / 10 * float(args.distance_alpha))
     args.distance_ratio = model.hparams.distance_ratio
     args.gap_encode = model.hparams.gap_encode
     args.jc_correct = model.hparams.jc_correct
-    #args.replicate_seq = model.hparams.replicate_seq
+    # args.replicate_seq = model.hparams.replicate_seq
     print('jc_correct', args.jc_correct)
     if args.jc_correct:
         args.jc_ratio = model.hparams.jc_ratio
     if not os.path.exists(dis_file_root):
         os.makedirs(dis_file_root, exist_ok=True)
 
-    backbone_seq = SeqIO.to_dict(SeqIO.parse(backbone_seq_file, "fasta"))
+    if ((args.backbone_emb is None) or (args.backbone_id is None)) or (
+            (recon_model is not None) and (args.recon_backbone_emb is None)):
+        backbone_seq = SeqIO.to_dict(SeqIO.parse(backbone_seq_file, "fasta"))
+    else:
+        backbone_seq = None
     query_seq = SeqIO.to_dict(SeqIO.parse(query_seq_file, "fasta"))
 
     if args.jc_correct:
         backbone_seq_names, backbone_seq_names_raw, backbone_seq_tensor, backbone_raw_array = \
             process_seq(backbone_seq, args, isbackbone=True)
         query_seq_names, query_seq_names_raw, query_seq_tensor, query_raw_array = \
             process_seq(query_seq, args, isbackbone=False)
     else:
         # breakpoint()
         if not (recon_model is None):
             if (args.recon_backbone_emb is None) or (args.backbone_id is None) or (args.backbone_gap is None):
-                backbone_seq_names, backbone_seq_tensor, backbone_mask = process_seq(backbone_seq, args, isbackbone=True, need_mask=True)
+                backbone_seq_names, backbone_seq_tensor, backbone_mask = process_seq(backbone_seq, args,
+                                                                                     isbackbone=True, need_mask=True)
             else:
                 backbone_seq_names = torch.load(args.backbone_id)
                 backbone_mask = torch.load(args.backbone_gap)
-            query_seq_names, query_seq_tensor, query_mask = process_seq(query_seq, args, isbackbone=False, need_mask=True)
+            query_seq_names, query_seq_tensor, query_mask = process_seq(query_seq, args, isbackbone=False,
+                                                                        need_mask=True)
         else:
             if (args.backbone_emb is None) or (args.backbone_id is None):
                 backbone_seq_names, backbone_seq_tensor = process_seq(backbone_seq, args, isbackbone=True)
             else:
                 backbone_seq_names = torch.load(args.backbone_id)
             query_seq_names, query_seq_tensor = process_seq(query_seq, args, isbackbone=False)
 
@@ -398,69 +504,70 @@
     print(f'{len(query_seq_names)} query sequence(s)')
     print(f'calculating embeddings...')
     if (args.backbone_emb is None) or (args.backbone_id is None):
         backbone_encodings = get_embeddings(backbone_seq_tensor, model)
     else:
         backbone_encodings = torch.load(args.backbone_emb)
     query_encodings = get_embeddings(query_seq_tensor, model)
-    #torch.save(query_encodings, f'{dis_file_root}/query_embeddings.pt')
-    #torch.save(query_seq_names, f'{dis_file_root}/query_names.pt')
-    #torch.save(backbone_encodings, f'{dis_file_root}/backbone_embeddings.pt')
-    #torch.save(backbone_seq_names, f'{dis_file_root}/backbone_names.pt')
+    # torch.save(query_encodings, f'{dis_file_root}/query_embeddings.pt')
+    # torch.save(query_seq_names, f'{dis_file_root}/query_names.pt')
+    torch.save(backbone_encodings, f'{dis_file_root}/backbone_embeddings.pt')
+    torch.save(backbone_seq_names, f'{dis_file_root}/backbone_names.pt')
 
     if not (recon_model is None):
         if (args.recon_backbone_emb is None) or (args.backbone_id is None) or (args.backbone_gap is None):
             recon_backbone_encodings = get_embeddings(backbone_seq_tensor, recon_model, backbone_mask)
         else:
             recon_backbone_encodings = torch.load(args.recon_backbone_emb)
         recon_query_encodings = get_embeddings(query_seq_tensor, recon_model, query_mask)
         torch.save(recon_backbone_encodings, f'{dis_file_root}/recon_backbone_embeddings.pt')
 
     print(f'finish embedding calculation!')
     print(f'calculating distance matrix...')
     t2 = time.time()
-    #print('calculate embeddings', t2 - t1)
+    # print('calculate embeddings', t2 - t1)
 
     # query_dist = distance(query_encodings, backbone_encodings, args.distance_mode) * args.distance_ratio
     query_dist = distance(query_encodings, backbone_encodings, args.distance_mode) * args.distance_ratio
     if 'square_root' in args.weighted_method:
         query_dist = query_dist ** 2
 
     if recon_model:
         gap_portion = 1 - query_mask.int().sum(-1) / query_mask.shape[-1]
-        recon_query_dist = distance(recon_query_encodings, recon_backbone_encodings, args.distance_mode) * args.distance_ratio
+        recon_query_dist = distance(recon_query_encodings, recon_backbone_encodings,
+                                    args.distance_mode) * args.distance_ratio
         if 'square_root' in args.weighted_method:
             recon_query_dist = recon_query_dist ** 2
         query_dist = query_dist * (1 - gap_portion) + recon_query_dist * gap_portion
 
     t3 = time.time()
-    #print('calculate distance', t3 - t2)
+    # print('calculate distance', t3 - t2)
     query_dist = np.array(query_dist)
     query_dist[query_dist < 1e-3] = 0
     data_origin = dict(zip(query_seq_names, list(query_dist.astype(str))))
     data_origin = "\t" + "\t".join(backbone_seq_names) + "\n" + \
-                  "\n".join([str(k) + "\t"+ "\t".join(data_origin[k]) for k in data_origin]) + "\n"
+                  "\n".join([str(k) + "\t" + "\t".join(data_origin[k]) for k in data_origin]) + "\n"
     t4 = time.time()
-    #print('convert string', t4 - t3)
+    # print('convert string', t4 - t3)
     with open(os.path.join(dis_file_root, f'depp.csv'), 'w') as f:
         f.write(data_origin)
     t5 = time.time()
-    #print('save string', t5 - t4)
+    # print('save string', t5 - t4)
     # data_origin = pd.DataFrame.from_dict(data_origin, orient='index', columns=backbone_seq_names)
 
     if args.query_dist:
         idx = data_origin.index
         data_origin = data_origin[idx]
     # data_origin.to_csv(os.path.join(dis_file_root, f'depp.csv'), sep='\t')
     # if not os.path.isdir(f'{args.outdir}/depp_tmp'):
     #     os.makedirs(f'{args.outdir}/depp_tmp')
     # with open(f'{args.outdir}/depp_tmp/seq_name.txt', 'w') as f:
     #     f.write("\n".join(query_seq_names) + '\n')
     print('original distanace matrix saved!')
-    print("take {:.2f} seconds".format(t5-t1))
+    print("take {:.2f} seconds".format(t5 - t1))
 
 
 def save_repr_emb(model, args):
     t1 = time.time()
     os.makedirs(args.outdir, exist_ok=True)
 
     print('calculating backbone embeddings...')
@@ -468,28 +575,26 @@
     def get_backbone_embeddings(i):
         print(f'embedding {i} cluster...')
         backbone_seq_file = f"{args.seqdir}/{i}.fa"
         backbone_seq = SeqIO.to_dict(SeqIO.parse(backbone_seq_file, "fasta"))
         backbone_seq_names, backbone_seq_tensor = process_seq(backbone_seq, args, isbackbone=True)
         backbone_seq_tensor_idx = np.random.choice(len(backbone_seq_tensor), size=100, replace=False)
         backbone_seq_tensor = backbone_seq_tensor[backbone_seq_tensor_idx]
-        backbone_encodings = {i: get_embeddings(backbone_seq_tensor, model, query=False, model_idx=i).mean(0) for i in range(model.hparams.cluster_num)}
+        backbone_encodings = {i: get_embeddings(backbone_seq_tensor, model, query=False, model_idx=i).mean(0) for i in
+                              range(model.hparams.cluster_num)}
         return backbone_encodings
 
     backbone_embs_tmp = [get_backbone_embeddings(i) for i in range(model.hparams.cluster_num)]
 
     backbone_encodings_dict = {i: backbone_embs_tmp[i] for i in range(model.hparams.cluster_num)}
 
     torch.save(backbone_encodings_dict, f'{args.outdir}/repr_emb.pt')
     t2 = time.time()
     print('finish! take {:.2f} seconds.'.format(t2 - t1))
 
-
-
-
 # def save_depp_dist(model, args, recon_model=None):
 #     t1 = time.time()
 #     if model is not None:
 #         model.eval()
 #         args.replicate_seq = model.hparams.replicate_seq
 #         args.distance_ratio = model.hparams.distance_ratio
 #         args.gap_encode = model.hparams.gap_encode
@@ -607,7 +712,8 @@
 #     # data_origin.to_csv(os.path.join(dis_file_root, f'depp.csv'), sep='\t')
 #     # if not os.path.isdir(f'{args.outdir}/depp_tmp'):
 #     #     os.makedirs(f'{args.outdir}/depp_tmp')
 #     # with open(f'{args.outdir}/depp_tmp/seq_name.txt', 'w') as f:
 #     #     f.write("\n".join(query_seq_names) + '\n')
 #     print('original distanace matrix saved!')
 #     print("take {:.2f} seconds".format(t5-t1))
+
```

### Comparing `depp-0.3.0/depp-place-rRNA-one-type.sh` & `depp-0.3.1/depp-place-rRNA-one-type.sh`

 * *Files 24% similar despite different names*

```diff
@@ -83,49 +83,55 @@
 #rm -rf $upptmpdir
 
 cp ${query_file} ${tmpdir}/
 
 # split large file into multiple small ones
 N=$(grep ">" ${query_file} | wc -l)
 mkdir ${tmpdir}/split_seq
-awk -v size=20000 -v pre=${tmpdir}/split_seq/seq -v pad="${#N}" '
+awk -v size=2000 -v pre=${tmpdir}/split_seq/seq -v pad="${#N}" '
    /^>/ { n++; if (n % size == 1) { close(fname); fname = sprintf("%s.%0" pad "d", pre, n) } }
       { print >> fname }
 ' ${tmpdir}/${data_type}_aligned.fa
 
 # calculate distance
+if [[ "${data_type}" == "16s_full_length" ]];
+then
+  cores_per_job=16
+else
+  cores_per_job=8
+fi
 
 function dist_place(){
   local seq_id=$1
   local c=$2
   local accessory_dir=$3
   local data_type=$4
   local tmpdir=$5
   local idx=$6
-  taskset -c $(((idx*2)%c))-$(((idx*2)%c+1)) depp_distance.py query_seq_file=$1 outdir=../dist/$1 model_path=${accessory_dir}/${data_type}.ckpt replicate_seq=True backbone_emb=${accessory_dir}/${data_type}_emb.pt backbone_id=${accessory_dir}/${data_type}_id.pt
+  taskset -c $(((idx*cores_per_job)%c))-$(((idx*cores_per_job)%c+cores_per_job-1)) depp_distance.py query_seq_file=$1 outdir=../dist/$1 model_path=${accessory_dir}/${data_type}.ckpt replicate_seq=True backbone_emb=${accessory_dir}/${data_type}_emb.pt backbone_id=${accessory_dir}/${data_type}_id.pt use_multi_class=True prob_thr=200
   jplace_suffix="${seq_id##*.}"
-  apples_core=`python -c "print(min($c,2))"`
+  apples_core=`python -c "print(min($c,$cores_per_job))"`
   mkdir ${tmpdir}/${data_type}_${jplace_suffix}
   for depp_dist_file in ../dist/$1/depp*csv;
   do
     depp_dist_idx=`basename $depp_dist_file`
     depp_dist_idx=${depp_dist_idx%%.*}
-    taskset -c $(((idx*2)%c))-$(((idx*2)%c+1)) run_apples.py -d $depp_dist_file -t ${accessory_dir}/wol.nwk -o ${tmpdir}/${data_type}_${jplace_suffix}/${data_type}_${jplace_suffix}_${depp_dist_idx}.jplace -f 0 -b 5 -T $apples_core
+    taskset -c $(((idx*cores_per_job)%c))-$(((idx*cores_per_job)%c+cores_per_job-1)) run_apples.py -d $depp_dist_file -t ${accessory_dir}/wol.nwk -o ${tmpdir}/${data_type}_${jplace_suffix}/${data_type}_${jplace_suffix}_${depp_dist_idx}.jplace -f 0 -b 5 -T $apples_core
   done
   cp ../dist/$1/entropy.txt ${tmpdir}/${data_type}_${jplace_suffix}_entropy.txt
-  taskset -c $(((idx*2)%c))-$(((idx*2)%c+1)) comb_json.py --indir ${tmpdir}/${data_type}_${jplace_suffix} --outfile ${tmpdir}/${data_type}_${jplace_suffix}.jplace
-  taskset -c $(((idx*2)%c))-$(((idx*2)%c+1)) rm -rf ../dist/$1
-  taskset -c $(((idx*2)%c))-$(((idx*2)%c+1)) rm -rf ${tmpdir}/${data_type}_${jplace_suffix}
+  taskset -c $(((idx*cores_per_job)%c))-$(((idx*cores_per_job)%c+cores_per_job-1)) comb_json.py --indir ${tmpdir}/${data_type}_${jplace_suffix} --outfile ${tmpdir}/${data_type}_${jplace_suffix}.jplace
+  taskset -c $(((idx*cores_per_job)%c))-$(((idx*cores_per_job)%c+cores_per_job-1)) rm -rf ../dist/$1
+  taskset -c $(((idx*cores_per_job)%c))-$(((idx*cores_per_job)%c+cores_per_job-1)) rm -rf ${tmpdir}/${data_type}_${jplace_suffix}
 #  taskset -c $(((idx*4)%c))-$(((idx*4)%c+3)) rm ../dist/$1/*.pt
 }
 export -f dist_place
 
 echo "calculating distance matrix..."
 pushd ${tmpdir}/split_seq/ > /dev/null 2>&1
-depp_p=`python -c "print(max($c//2,1))"`
+depp_p=`python -c "print(max($c//$cores_per_job,1))"`
 #ls -1 seq* | xargs -n1 -P$depp_p -I% bash -c 'dist_place "%" "${c}" "${accessory_dir}" "${data_type}" "${tmpdir}"'
 n_seq=`ls -1 seq*|wc -l`
 num_jobs="\j"
 j=0
 for ((j=0; j<$n_seq; j++));
 do
         while (( ${num_jobs@P} >= $depp_p ));
```

### Comparing `depp-0.3.0/depp-place-rRNA.sh` & `depp-0.3.1/depp-place-rRNA.sh`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/bin/bash
 
-while getopts q:a:o:t:x:d:s: flag
+while getopts q:a:o:t:x:d:s:l: flag
 do
     case "${flag}" in
 	q) query_file=${OPTARG};;
 	a) accessory_dir=${OPTARG};;
   o) out_dir=${OPTARG};;
   t) data_type=${OPTARG};;
   x) cores=${OPTARG};;
   d) debug=${OPTARG};;
+  l) align=${OPTARG};;
 #  s) script_dir=${OPTARG};;
     esac
 done
 
+align="${align:-noalign}"
 # check if data type input is valid
 valid_data="16s_full_length 16s_v4_100 16s_v4_150 16s_v3_v4 mixed"
 #contains() {
 #  [[ $1 =~ (^|[[:space:]])$2($|[[:space:]]) ]] && exit(0) || exit(1)
 #}
 function notcontains(){
   local list="$1"
@@ -42,15 +44,14 @@
   mkdir -p ${out_dir}
 fi
 
 query_file=`realpath $query_file`
 accessory_dir=`realpath $accessory_dir`
 out_dir=`realpath $out_dir`
 #script_dir=`realpath $script_dir`
-
 if [[ "${data_type}" == "mixed" ]];
 then
   if [ -d "/scratch/$USER/job_$SLURM_JOB_ID" ];
   then
     # check whether ssds for tmp files exist
 #    echo "use /scratch/$USER/job_$SLURM_JOB_ID as temporary directory"
     export TMPDIR=/scratch/$USER/job_$SLURM_JOB_ID
@@ -60,66 +61,73 @@
   fi
   tmpdir=`mktemp -d -t 'depp-tmp-XXXXXXXXXX'`
   # check if the directory is created
   if [[ ! "$tmpdir" || ! -d "$tmpdir" ]]; then
     echo "Could not create temp dir"
     exit 1
   fi
-  mkdir ${tmpdir}/query_seq
-  seq_sep.py --infile ${query_file} --outdir ${tmpdir}/query_seq
+  if [ $align == "noalign" ];
+  then
+    mkdir ${tmpdir}/query_seq
+    seq_sep.py --infile ${query_file} --outdir ${tmpdir}/query_seq
 
-  # align sequences
-  echo "aligning the sequences..."
+    # align sequences
+    echo "aligning the sequences..."
 
-  # split query sequences into multiple files (/tmp directory)
-  for i in ${tmpdir}/query_seq/*.fa;
-  do
-    upptmpdir=`mktemp -d -t 'upp-tmp-XXXXXXXXXX'`
-    # check if the directory is created
-    if [[ ! "$tmpdir" || ! -d "$tmpdir" ]]; then
-      echo "Could not create temp dir"
-      exit 1
-    fi
-    j="${i##*/}"
-    dt="${j%.*}"
-    N=$(grep ">" ${i} | wc -l)
-    awk -v size=4000000 -v pre=${upptmpdir}/seq -v pad="${#N}" '
-       /^>/ { n++; if (n % size == 1) { close(fname); fname = sprintf("%s.%0" pad "d", pre, n) } }
-          { print >> fname }
-    ' ${i}
-
-    mkdir ${upptmpdir}/aligned
-    cnt=0
-    for i in ${upptmpdir}/seq*;
+    # split query sequences into multiple files (/tmp directory)
+    for i in ${tmpdir}/query_seq/*.fa;
     do
-      mkdir ${upptmpdir}/tmp
-      mkdir ${upptmpdir}/tmp_result
-      grep ">" ${i} | sed "s/^>//g" | sort > ${upptmpdir}/tmp_result/query_ids.txt
-      upp_c=${cores}
-    #  awk "/^>/ {n++} n>8000 {exit} {print}" ${accessory_dir}/${data_type}_a.fasta > ${i}.backbone
-      run_upp.py -s ${i} -a ${accessory_dir}/${dt}_ao.fasta -t ${accessory_dir}/${dt}.nwk -A 200 -d ${upptmpdir}/tmp_result -x $upp_c -p ${upptmpdir}/tmp 1>${tmpdir}/upp-out.log 2>>${out_dir}/${dt}_upp.log
-      grep -w -A 1 -f ${upptmpdir}/tmp_result/query_ids.txt ${upptmpdir}/tmp_result/output_alignment_masked.fasta --no-group-separator > ${upptmpdir}/aligned/${cnt}.fa
-      cnt=$((cnt+1))
-      rm -rf ${upptmpdir}/tmp
-      rm -rf ${upptmpdir}/tmp_result
+      upptmpdir=`mktemp -d -t 'upp-tmp-XXXXXXXXXX'`
+      # check if the directory is created
+      if [[ ! "$tmpdir" || ! -d "$tmpdir" ]]; then
+        echo "Could not create temp dir"
+        exit 1
+      fi
+      j="${i##*/}"
+      dt="${j%.*}"
+      N=$(grep ">" ${i} | wc -l)
+      awk -v size=4000000 -v pre=${upptmpdir}/seq -v pad="${#N}" '
+         /^>/ { n++; if (n % size == 1) { close(fname); fname = sprintf("%s.%0" pad "d", pre, n) } }
+            { print >> fname }
+      ' ${i}
+
+      mkdir ${upptmpdir}/aligned
+      cnt=0
+      for i in ${upptmpdir}/seq*;
+      do
+        mkdir ${upptmpdir}/tmp
+        mkdir ${upptmpdir}/tmp_result
+        grep ">" ${i} | sed "s/^>//g" | sort > ${upptmpdir}/tmp_result/query_ids.txt
+        upp_c=${cores}
+      #  awk "/^>/ {n++} n>8000 {exit} {print}" ${accessory_dir}/${data_type}_a.fasta > ${i}.backbone
+        run_upp.py -s ${i} -a ${accessory_dir}/${dt}_ao.fasta -t ${accessory_dir}/${dt}.nwk -A 200 -d ${upptmpdir}/tmp_result -x $upp_c -p ${upptmpdir}/tmp 1>${tmpdir}/upp-out.log 2>>${out_dir}/${dt}_upp.log
+  #      grep -w -A 1 -f ${upptmpdir}/xtmp_result/query_ids.txt ${upptmpdir}/tmp_result/output_alignment_masked.fasta --no-group-separator > ${upptmpdir}/aligned/${cnt}.fa
+        seqkit grep -w 0 -f ${upptmpdir}/tmp_result/query_ids.txt ${upptmpdir}/tmp_result/output_alignment_masked.fasta -o ${upptmpdir}/aligned/${cnt}.fa
+        cnt=$((cnt+1))
+        rm -rf ${upptmpdir}/tmp
+        rm -rf ${upptmpdir}/tmp_result
+      done
+      cat ${upptmpdir}/aligned/*.fa > ${tmpdir}/${dt}_aligned.fa
+      rm -rf $upptmpdir
     done
-    cat ${upptmpdir}/aligned/*.fa > ${tmpdir}/${dt}_aligned.fa
-    rm -rf $upptmpdir
-  done
 
-  rm ${tmpdir}/query_seq/*
-  if test -f "${tmpdir}/16s_full_length_aligned.fa";
-  then
-    cp ${tmpdir}/16s_full_length_aligned.fa ${tmpdir}/query_seq
-  fi
+    rm ${tmpdir}/query_seq/*
+    if test -f "${tmpdir}/16s_full_length_aligned.fa";
+    then
+      cp ${tmpdir}/16s_full_length_aligned.fa ${tmpdir}/query_seq
+    fi
 
-  if test -f "${tmpdir}/16s_v4_aligned.fa";
-  then
-    cp ${tmpdir}/16s_v4_aligned.fa ${out_dir}/16s_v4_aligned_all.fa
-    seq_sep.py --infile ${tmpdir}/16s_v4_aligned.fa --outdir ${tmpdir}/query_seq --aligned
+    if test -f "${tmpdir}/16s_v4_aligned.fa";
+    then
+      cp ${tmpdir}/16s_v4_aligned.fa ${out_dir}/16s_v4_aligned_all.fa
+      seq_sep.py --infile ${tmpdir}/16s_v4_aligned.fa --outdir ${tmpdir}/query_seq --aligned
+    fi
+  else
+    mkdir -p ${tmpdir}/query_seq/
+    cp $align/*aligned.fa ${tmpdir}/query_seq/
   fi
 
   for i in ${tmpdir}/query_seq/*.fa;
   do
     j="${i##*/}"
     dt="${j%_aligned.*}"
     depp-place-rRNA-one-type.sh -q ${i} -a ${accessory_dir} -o ${tmpdir} -t ${dt} -x ${cores}
```

### Comparing `depp-0.3.0/merge_json.py` & `depp-0.3.1/merge_json.py`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/run_upp.sh` & `depp-0.3.1/run_upp.sh`

 * *Files identical despite different names*

### Comparing `depp-0.3.0/seq_sep.py` & `depp-0.3.1/seq_sep.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     v4_100_p = {i: get_portion(str(all_seq[i].seq), 0, 98) for i in all_seq}
     v4_150_p = {i: get_portion(str(all_seq[i].seq), 0, 148) for i in all_seq}
     v4_p = {i: get_portion(str(all_seq[i].seq), 0, 248) for i in all_seq}
     def v4_condition(i): return (v4_p[i] >= 0.8) or (v4_p[i] >= v4_150_p[i] and v4_p[i] >= v4_100_p[i])
     def v4_150_condition(i): return (not v4_condition(i)) and (v4_150_p[i] >= 0.8 or v4_150_p[i] >= v4_100_p[i])
     def v4_100_condition(i): return (not v4_condition(i)) and (not v4_150_condition(i))
     v4 = [f'>{i}\n{str(all_seq[i].seq)}\n' for i in all_seq if v4_condition(i)]
+    # v4_150 = [f'>{i}\n{str(all_seq[i].seq)[:149]}\n' for i in all_seq if v4_150_condition(i)]
+    # v4_100 = [f'>{i}\n{str(all_seq[i].seq)[:99]}\n' for i in all_seq if v4_100_condition(i)]
     v4_150 = [f'>{i}\n{str(all_seq[i].seq)[:149]}\n' for i in all_seq if v4_150_condition(i)]
     v4_100 = [f'>{i}\n{str(all_seq[i].seq)[:99]}\n' for i in all_seq if v4_100_condition(i)]
 
     if len(v4) != 0:
         with open(f'{args.outdir}/16s_v4_aligned.fa', 'w') as f:
             f.write("".join(v4)+'\n')
```

### Comparing `depp-0.3.0/setup.py` & `depp-0.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name='depp',    # This is the name of your PyPI-package.
-        version='0.3.0',    # Update the version number for new releases
+        version='0.3.1',    # Update the version number for new releases
         scripts=['train_depp.py',
                  'depp/depp_distance.py',
                  'agg_dist.py',
                  'wol_placement.sh',
                  'run_upp.sh',
                  'merge_json.py',
 		 'train_depp_recon.py',
@@ -17,15 +17,20 @@
                  'depp-place-rRNA-one-type.sh',
                  'comb_json.py',
                  'seq_sep.py',
                  'depp/filter_by_entropy_gap.sh',
                  'depp/grep_seq.py',
                  'depp/get_names_by_entropy_gap.py',
                  'depp/grep_jplace.py',
-                 'depp/count_gapped_ratio.py'], # The name of your scipt, and also the command you'll be using for calling it
+                 'depp/count_gapped_ratio.py',
+                 'depp/set_bl_one.py',
+                 'depp/grep_seq_group.py',
+                 'depp/get_tree_dist.py',
+                 'depp/select_species_by_distance.py',
+                 'train_cluster_depp.sh'], # The name of your scipt, and also the command you'll be using for calling it
         description='DEPP: Deep Learning Enables Extending Species Trees using Single Genes',
         long_description='DEPP is a deep-learning-based tool for phylogenetic placement.'
                          'Output of the tool is the distance matrix between the query sequences and the backbone sequences',
         long_description_content_type='text/plain',
         url='https://github.com/yueyujiang/DEPP',
         author='Yueyu Jiang',
         author_email='y5jiang@ucsd.edu',
```

### Comparing `depp-0.3.0/train_depp.py` & `depp-0.3.1/train_depp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/calab_data/mirarab/home/yueyu/miniconda3/envs/depp_env/bin/python
+#!/usr/bin/env python3
 
 import os
 from depp import Model_pl
 from depp import default_config
 import pkg_resources
 from depp import Agg_model
 
@@ -63,28 +63,28 @@
                 gpus=args.gpus,
                 # progress_bar_refresh_rate=args.bar_update_freq,
                 check_val_every_n_epoch=args.val_freq,
                 max_epochs=args.classifier_epoch + 1,
                 gradient_clip_val=args.cp,
                 benchmark=True,
                 callbacks=[early_stop_callback],
-                checkpoint_callback=checkpoint_callback
+                enable_checkpointing=checkpoint_callback
             )
         else:
             classifier_trainer = pl.Trainer(
                 logger=False,
                 gpus=args.gpus,
                 # progress_bar_refresh_rate=args.bar_update_freq,
-                accelerator='ddp',
+                strategy='ddp',
                 check_val_every_n_epoch=args.val_freq,
                 max_epochs=args.classifier_epoch + 1,
                 gradient_clip_val=args.cp,
                 benchmark=True,
                 callbacks=[early_stop_callback],
-                checkpoint_callback=checkpoint_callback
+                enable_checkpointing=checkpoint_callback
             )
         model = Model_pl.model(args=args, current_model=-1)
         classifier_trainer.fit(model)
         args.start_model_idx = 0
 
     for model_idx in range(args.start_model_idx, args.end_model_idx):
         if args.gpus == 0:
@@ -93,28 +93,28 @@
                 gpus=args.gpus,
                 # progress_bar_refresh_rate=args.bar_update_freq,
                 check_val_every_n_epoch=args.val_freq,
                 max_epochs=args.epoch + 1,
                 gradient_clip_val=args.cp,
                 benchmark=True,
                 callbacks=[early_stop_callback],
-                checkpoint_callback=checkpoint_callback
+                enable_checkpointing=checkpoint_callback
             )
         else:
             trainer = pl.Trainer(
                 logger=False,
                 gpus=args.gpus,
                 # progress_bar_refresh_rate=args.bar_update_freq,
-                accelerator='ddp',
+                strategy='ddp',
                 check_val_every_n_epoch=args.val_freq,
                 max_epochs=args.epoch + 1,
                 gradient_clip_val=args.cp,
                 benchmark=True,
                 callbacks=[early_stop_callback],
-                checkpoint_callback=checkpoint_callback
+                enable_checkpointing=checkpoint_callback
             )
 
         model = Model_pl.model(args=args, current_model=model_idx)
         trainer.fit(model)
 
     if args.backbone_tree_file is not None and args.cluster_num == 1:
         os.rename(f'{args.model_dir}/0/epoch-{args.epoch - args.epoch % 100}.pth', f'{args.model_dir}/depp-model.pth')
```

### Comparing `depp-0.3.0/wol_placement.sh` & `depp-0.3.1/wol_placement.sh`

 * *Files identical despite different names*

