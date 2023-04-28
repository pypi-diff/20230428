# Comparing `tmp/rotary-embedding-torch-0.2.1.tar.gz` & `tmp/rotary-embedding-torch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary-embedding-torch-0.2.1.tar", last modified: Thu Dec 22 19:15:12 2022, max compression
+gzip compressed data, was "rotary-embedding-torch-0.2.2.tar", last modified: Fri Apr 28 21:11:05 2023, max compression
```

## Comparing `rotary-embedding-torch-0.2.1.tar` & `rotary-embedding-torch-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:15:12.171484 rotary-embedding-torch-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-22 19:15:00.000000 rotary-embedding-torch-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 19:15:12.171484 rotary-embedding-torch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2022-12-22 19:15:00.000000 rotary-embedding-torch-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:15:12.171484 rotary-embedding-torch-0.2.1/rotary_embedding_torch/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-22 19:15:00.000000 rotary-embedding-torch-0.2.1/rotary_embedding_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2022-12-22 19:15:00.000000 rotary-embedding-torch-0.2.1/rotary_embedding_torch/rotary_embedding_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:15:12.171484 rotary-embedding-torch-0.2.1/rotary_embedding_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 19:15:12.000000 rotary-embedding-torch-0.2.1/rotary_embedding_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2022-12-22 19:15:12.000000 rotary-embedding-torch-0.2.1/rotary_embedding_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 19:15:12.000000 rotary-embedding-torch-0.2.1/rotary_embedding_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-22 19:15:12.000000 rotary-embedding-torch-0.2.1/rotary_embedding_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-22 19:15:12.000000 rotary-embedding-torch-0.2.1/rotary_embedding_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 19:15:12.171484 rotary-embedding-torch-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2022-12-22 19:15:00.000000 rotary-embedding-torch-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/rotary_embedding_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch/rotary_embedding_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/setup.py
```

### Comparing `rotary-embedding-torch-0.2.1/LICENSE` & `rotary-embedding-torch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rotary-embedding-torch-0.2.1/PKG-INFO` & `rotary-embedding-torch-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.2.1/README.md` & `rotary-embedding-torch-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 
 q = apply_rotary_emb(freqs, q)
 k = apply_rotary_emb(freqs, k)
 ```
 
 ## Length Extrapolatable Rotary Embeddings
 
-In <a href="https://arxiv.org/abs/2212.10554v1">this paper</a>, they were able to fix length extrapolation issue with rotary embeddings by giving it a decay similar to ALiBi. They named this technique XPos, and you can use it by setting `use_xpos = True` on initialization
+In <a href="https://arxiv.org/abs/2212.10554v1">this paper</a>, they were able to fix length extrapolation issue with rotary embeddings by giving it a decay similar to ALiBi. They named this technique XPos, and you can use it by setting `use_xpos = True` on initialization.
+
+This can only be used for autoregressive transformers
 
 ```python
 import torch
 from rotary_embedding_torch import RotaryEmbedding
 
 # instantiate the positional embedding in your transformer and pass to all your attention layers
```

#### html2text {}

```diff
@@ -28,27 +28,28 @@
 (torch.linspace(-1, 1, steps = 256), cache_key = 256) # concat the frequencies
 along each axial # broadcat function makes this easy without a bunch of expands
 freqs = broadcat((freqs_h[:, None, :], freqs_w[None, :, :]), dim = -1) # rotate
 in frequencies q = apply_rotary_emb(freqs, q) k = apply_rotary_emb(freqs, k)
 ``` ## Length Extrapolatable Rotary Embeddings In this_paper, they were able to
 fix length extrapolation issue with rotary embeddings by giving it a decay
 similar to ALiBi. They named this technique XPos, and you can use it by setting
-`use_xpos = True` on initialization ```python import torch from
-rotary_embedding_torch import RotaryEmbedding # instantiate the positional
-embedding in your transformer and pass to all your attention layers rotary_emb
-= RotaryEmbedding( dim = 32, use_xpos = True # set this to True to make rotary
-embeddings extrapolate better to sequence lengths greater than the one used at
-training time ) # mock queries and keys - dimensions should end with (seq_len,
-feature dimension), and any number of preceding dimensions (batch, heads, etc)
-q = torch.randn(1, 8, 1024, 64) # queries - (batch, heads, seq len, dimension
-of head) k = torch.randn(1, 8, 1024, 64) # keys # apply the rotations to your
-queries and keys after the heads have been split out, but prior to the dot
-product and subsequent softmax (attention) # instead of using
-`rotate_queries_or_keys`, you will use `rotate_queries_and_keys`, the rest is
-taken care of q, k = rotary_emb.rotate_queries_and_keys(q, k) ``` ## Citations
-```bibtex @misc{su2021roformer, title = {RoFormer: Enhanced Transformer with
-Rotary Position Embedding}, author = {Jianlin Su and Yu Lu and Shengfeng Pan
-and Bo Wen and Yunfeng Liu}, year = {2021}, eprint = {2104.09864},
-archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @inproceedings
-{Sun2022ALT, title = {A Length-Extrapolatable Transformer}, author = {Yutao Sun
-and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim
-and Vishrav Chaudhary and Xia Song and Furu Wei}, year = {2022} } ```
+`use_xpos = True` on initialization. This can only be used for autoregressive
+transformers ```python import torch from rotary_embedding_torch import
+RotaryEmbedding # instantiate the positional embedding in your transformer and
+pass to all your attention layers rotary_emb = RotaryEmbedding( dim = 32,
+use_xpos = True # set this to True to make rotary embeddings extrapolate better
+to sequence lengths greater than the one used at training time ) # mock queries
+and keys - dimensions should end with (seq_len, feature dimension), and any
+number of preceding dimensions (batch, heads, etc) q = torch.randn(1, 8, 1024,
+64) # queries - (batch, heads, seq len, dimension of head) k = torch.randn(1,
+8, 1024, 64) # keys # apply the rotations to your queries and keys after the
+heads have been split out, but prior to the dot product and subsequent softmax
+(attention) # instead of using `rotate_queries_or_keys`, you will use
+`rotate_queries_and_keys`, the rest is taken care of q, k =
+rotary_emb.rotate_queries_and_keys(q, k) ``` ## Citations ```bibtex @misc
+{su2021roformer, title = {RoFormer: Enhanced Transformer with Rotary Position
+Embedding}, author = {Jianlin Su and Yu Lu and Shengfeng Pan and Bo Wen and
+Yunfeng Liu}, year = {2021}, eprint = {2104.09864}, archivePrefix = {arXiv},
+primaryClass = {cs.CL} } ``` ```bibtex @inproceedings{Sun2022ALT, title = {A
+Length-Extrapolatable Transformer}, author = {Yutao Sun and Li Dong and Barun
+Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary
+and Xia Song and Furu Wei}, year = {2022} } ```
```

### Comparing `rotary-embedding-torch-0.2.1/rotary_embedding_torch/rotary_embedding_torch.py` & `rotary-embedding-torch-0.2.2/rotary_embedding_torch/rotary_embedding_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,16 @@
         freqs = self.forward(lambda: torch.arange(seq_len, device = device), cache_key = seq_len)
         return apply_rotary_emb(freqs, t)
 
     def rotate_queries_and_keys(self, q, k, seq_dim = -2):
         assert self.use_xpos
         device, seq_len = q.device, q.shape[seq_dim]
         seq = torch.arange(seq_len, device = device)
-        freqs = self.forward(lambda: seq, cache_key = seq_len)
-        scale = self.get_scale(lambda: seq, cache_key = seq_len)
+        freqs = self.forward(lambda: seq, cache_key = f'freqs:{seq_len}')
+        scale = self.get_scale(lambda: seq, cache_key = f'scale:{seq_len}')
         rotated_q = apply_rotary_emb(freqs, q, scale = scale)
         rotated_k = apply_rotary_emb(freqs, k, scale = scale ** -1)
         return rotated_q, rotated_k
 
     def get_scale(self, t, cache_key = None):
         assert self.use_xpos
 
@@ -123,15 +123,15 @@
         scale = 1.
         if self.use_xpos:
             power = t - (len(t) // 2) / self.scale_base
             scale = self.scale ** rearrange(power, 'n -> n 1')
             scale = torch.cat((scale, scale), dim = -1)
 
         if exists(cache_key):
-            self.cache[cache_key] = freqs
+            self.cache[cache_key] = scale
 
         return scale
 
     def forward(self, t, cache_key = None):
         if exists(cache_key) and cache_key in self.cache:
             return self.cache[cache_key]
```

### Comparing `rotary-embedding-torch-0.2.1/rotary_embedding_torch.egg-info/PKG-INFO` & `rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.2.1/setup.py` & `rotary-embedding-torch-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rotary-embedding-torch',
   packages = find_packages(),
-  version = '0.2.1',
+  version = '0.2.2',
   license='MIT',
   description = 'Rotary Embedding - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/rotary-embedding-torch',
   keywords = [
```

