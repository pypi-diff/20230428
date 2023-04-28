# Comparing `tmp/CoLT5-attention-0.2.4.tar.gz` & `tmp/CoLT5-attention-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.2.4.tar", last modified: Fri Apr 21 14:30:56 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.2.5.tar", last modified: Fri Apr 28 21:37:12 2023, max compression
```

## Comparing `CoLT5-attention-0.2.4.tar` & `CoLT5-attention-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:30:56.548388 CoLT5-attention-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:30:56.544388 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-21 14:30:56.548388 CoLT5-attention-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:30:56.548388 CoLT5-attention-0.2.4/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:30:56.548388 CoLT5-attention-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:37:12.234505 CoLT5-attention-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:37:12.230505 CoLT5-attention-0.2.5/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 21:37:12.000000 CoLT5-attention-0.2.5/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 21:37:12.000000 CoLT5-attention-0.2.5/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:37:12.000000 CoLT5-attention-0.2.5/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 21:37:12.000000 CoLT5-attention-0.2.5/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 21:37:12.000000 CoLT5-attention-0.2.5/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 21:36:59.000000 CoLT5-attention-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 21:37:12.234505 CoLT5-attention-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-28 21:36:59.000000 CoLT5-attention-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:37:12.234505 CoLT5-attention-0.2.5/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-28 21:36:59.000000 CoLT5-attention-0.2.5/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 21:36:59.000000 CoLT5-attention-0.2.5/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 21:36:59.000000 CoLT5-attention-0.2.5/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25268 2023-04-28 21:36:59.000000 CoLT5-attention-0.2.5/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:37:12.234505 CoLT5-attention-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 21:36:59.000000 CoLT5-attention-0.2.5/setup.py
```

### Comparing `CoLT5-attention-0.2.4/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.2.5/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.4
+Version: 0.2.5
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.4/LICENSE` & `CoLT5-attention-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.4/PKG-INFO` & `CoLT5-attention-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.4
+Version: 0.2.5
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.4/README.md` & `CoLT5-attention-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 - [x] figure out if it can be done autoregressively and try it out - moving to <a href="https://github.com/lucidrains/coordinate-descent-attention">this repo</a>
 - [x] allow for multi-headed routing (multiple routing tokens), only for key-values
 
 - [ ] for variable sequence lengths, allow for setting k as a function of sequence lengths per sample in batch
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 - [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
 - [ ] make flash attention compatible
+- [ ] work out a triton forward / backward version of coordinate descent (coor_descent), as it seems torch compile does not work well enough for coor_descent function just yet
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -52,13 +52,15 @@
 [x] figure out if it can be done autoregressively and try it out - moving to
 this_repo - [x] allow for multi-headed routing (multiple routing tokens), only
 for key-values - [ ] for variable sequence lengths, allow for setting k as a
 function of sequence lengths per sample in batch - [ ] create a variant of
 CoLT5 for high resolution feature maps (image attention) - then try out for
 diffusion - [ ] in the cross attention scenario, support for routing token that
 first queries the source tokens, before retrieving from memories - [ ] make
-flash attention compatible ## Citations ```bibtex @inproceedings
-{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range Transformers with
-Conditional Computation}, author = {Joshua Ainslie and Tao Lei and Michiel de
-Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David
-Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit
-Sanghai}, year = {2023} } ```
+flash attention compatible - [ ] work out a triton forward / backward version
+of coordinate descent (coor_descent), as it seems torch compile does not work
+well enough for coor_descent function just yet ## Citations ```bibtex
+@inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
+Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
+Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
+Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
+Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
```

### Comparing `CoLT5-attention-0.2.4/colt5_attention/coor_descent.py` & `CoLT5-attention-0.2.5/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.4/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.2.5/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.4/colt5_attention/transformer_block.py` & `CoLT5-attention-0.2.5/colt5_attention/transformer_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,14 +185,19 @@
         self.is_one_routing_token = num_routing_tokens == 1
         self.num_routing_tokens = num_routing_tokens
         self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
 
         self.straight_through = straight_through
         self.temperature = temperature
 
+    def route_back(self, src, routed_tokens, indices):
+        batch_range = create_batch_range(routed_tokens)
+        src[batch_range, indices] = routed_tokens
+        return src
+
     def forward(
         self,
         x,
         *,
         num_tokens,
         mask = None
     ):
@@ -263,14 +268,17 @@
         self.is_one_routing_token = num_routing_tokens == 1
         self.num_routing_tokens = num_routing_tokens
         self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
 
         self.straight_through = straight_through
         self.gumbel_sinkhorn_fn = partial(gumbel_sinkhorn, temperature = temperature, n_iters = n_iters)
 
+    def route_back(self, src, routed_tokens, indices):
+        return scatter_mean(src, routed_tokens, indices, dim = 1)
+
     def forward(
         self,
         x,
         *,
         num_tokens,
         mask = None
     ):
@@ -354,14 +362,19 @@
         self.fetch_k_ratio = fetch_k_ratio
 
         self.is_one_routing_token = num_routing_tokens == 1
         self.num_routing_tokens = num_routing_tokens
         self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
         self.straight_through = straight_through
 
+    def route_back(self, src, routed_tokens, indices):
+        batch_range = create_batch_range(routed_tokens)
+        src[batch_range, indices] = routed_tokens
+        return src
+
     def forward(
         self,
         x,
         *,
         num_tokens,
         mask = None
     ):
@@ -476,18 +489,15 @@
 
         routed_tokens_out = self.heavy_ff(routed_tokens) * rearrange(normalized_scores, '... -> ... 1')
 
         # scatter back the output of the heavy feedforward branch
 
         heavy_out = torch.zeros_like(x)
 
-        if self.router_type == 'sinkhorn':
-            heavy_out = scatter_mean(heavy_out, routed_tokens_out, indices, dim = 1)
-        else:
-            heavy_out[batch_range, indices] = routed_tokens_out
+        heavy_out = self.router.route_back(heavy_out, routed_tokens_out, indices)
 
         # sum light and heavy branches
 
         return light_out + heavy_out
 
 class ConditionalRoutedAttention(nn.Module):
     def __init__(
@@ -599,19 +609,15 @@
         )
 
         routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
 
         # scatter back the output of the heavy branch
 
         heavy_out = torch.zeros_like(x)
-
-        if self.router_type == 'sinkhorn':
-            heavy_out = scatter_mean(heavy_out, routed_tokens_out, indices_q, dim = 1)
-        else:
-            heavy_out[batch_range, indices_q] = routed_tokens_out
+        heavy_out = self.q_router.route_back(heavy_out, routed_tokens_out, indices_q)
 
         # sum light and heavy branches
 
         return light_out + heavy_out
 
 # adapting the conditional routed self attention to cross attention
 
@@ -726,18 +732,15 @@
         if not should_route_queries:
             return routed_tokens_out
 
         # otherwise, scatter back the query outputs
 
         out = torch.zeros_like(x)
 
-        if self.router_type == 'sinkhorn':
-            out = scatter_mean(heavy_out, routed_tokens_out, indices_q, dim = 1)
-        else:
-            out[batch_range, indices_q] = routed_tokens_out
+        out = self.q_router.route_back(out, routed_tokens_out, indices_q)
 
         return out
 
 # block
 
 class ConditionalRoutedTransformerBlock(nn.Module):
     def __init__(
```

### Comparing `CoLT5-attention-0.2.4/setup.py` & `CoLT5-attention-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.2.4',
+  version = '0.2.5',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

