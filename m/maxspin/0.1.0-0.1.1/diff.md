# Comparing `tmp/maxspin-0.1.0.tar.gz` & `tmp/maxspin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxspin-0.1.0.tar", max compression
+gzip compressed data, was "maxspin-0.1.1.tar", max compression
```

## Comparing `maxspin-0.1.0.tar` & `maxspin-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     4058 2022-12-18 01:40:06.937163 maxspin-0.1.0/README.md
--rw-r--r--   0        0        0      195 2022-09-19 22:16:25.732442 maxspin-0.1.0/maxspin/__init__.py
--rw-r--r--   0        0        0     3139 2022-12-18 00:44:18.938704 maxspin-0.1.0/maxspin/binning.py
--rw-r--r--   0        0        0      832 2022-12-13 00:18:27.067428 maxspin-0.1.0/maxspin/gamma_mh.py
--rw-r--r--   0        0        0      366 2022-11-01 23:52:23.746011 maxspin-0.1.0/maxspin/objectives.py
--rw-r--r--   0        0        0    10705 2022-12-18 00:52:43.467855 maxspin-0.1.0/maxspin/pairwise.py
--rw-r--r--   0        0        0    30690 2022-12-18 00:52:59.481480 maxspin-0.1.0/maxspin/spatial_information.py
--rw-r--r--   0        0        0      659 2022-12-18 01:50:28.061782 maxspin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5007 1970-01-01 00:00:00.000000 maxspin-0.1.0/setup.py
--rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 maxspin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4058 2022-12-18 01:40:06.937163 maxspin-0.1.1/README.md
+-rw-r--r--   0        0        0      195 2022-09-19 22:16:25.732442 maxspin-0.1.1/maxspin/__init__.py
+-rw-r--r--   0        0        0     3139 2022-12-18 00:44:18.938704 maxspin-0.1.1/maxspin/binning.py
+-rw-r--r--   0        0        0      832 2022-12-13 00:18:27.067428 maxspin-0.1.1/maxspin/gamma_mh.py
+-rw-r--r--   0        0        0      366 2022-11-01 23:52:23.746011 maxspin-0.1.1/maxspin/objectives.py
+-rw-r--r--   0        0        0    10784 2023-04-21 16:33:47.761408 maxspin-0.1.1/maxspin/pairwise.py
+-rw-r--r--   0        0        0    31303 2023-04-28 17:17:22.428679 maxspin-0.1.1/maxspin/spatial_information.py
+-rw-r--r--   0        0        0      712 2023-04-28 17:31:23.015457 maxspin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 maxspin-0.1.1/PKG-INFO
```

### Comparing `maxspin-0.1.0/README.md` & `maxspin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `maxspin-0.1.0/maxspin/binning.py` & `maxspin-0.1.1/maxspin/binning.py`

 * *Files identical despite different names*

### Comparing `maxspin-0.1.0/maxspin/gamma_mh.py` & `maxspin-0.1.1/maxspin/gamma_mh.py`

 * *Files identical despite different names*

### Comparing `maxspin-0.1.0/maxspin/pairwise.py` & `maxspin-0.1.1/maxspin/pairwise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from anndata import AnnData
 from flax import linen as nn
 from functools import partial
-from jax.experimental.maps import FrozenDict
 from scipy import sparse
 from tqdm import tqdm
 from typing import Optional, Any, Callable, List, Union
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
@@ -196,36 +195,41 @@
     optimizer = optax.adam(learning_rate=lr)
     train_step = make_train_step(optimizer)
 
     scores = np.zeros((ngenes, ngenes), dtype=np.float32)
 
     for receiver_gene in range(ngenes):
         print(f"Scoring all pairs with gene {receiver_gene}")
-        sample_v = lambda key, u, i: u[:,receiver_gene:receiver_gene+1]
+
+        # Always putting the receiver gene at the front of the chunk
+        def sample_v(key, u, i):
+            return u[:, 0:1]
 
         scores_chunks = []
         tpr_chunks = []
         for gene_from in range(0, ngenes, chunk_size):
             gene_to = min(gene_from + chunk_size, ngenes)
 
-            us_chunk = [u[:,gene_from:gene_to] for u in us]
+            chunk_span = [receiver_gene] + list(range(gene_from, gene_to))
+
+            us_chunk = [u[:,chunk_span] for u in us]
             αs_chunk = None
             βs_chunk = None
             σs_chunk = None
 
             if prior == "beta":
-                αs_chunk = [α[:,gene_from:gene_to] + prior_a for α in αs]
-                βs_chunk = [β[:,gene_from:gene_to] + prior_a for β in βs]
+                αs_chunk = [α[:,chunk_span] + prior_a for α in αs]
+                βs_chunk = [β[:,chunk_span] + prior_a for β in βs]
             elif prior == "dirichlet":
                 for u in us_chunk:
                     u += prior_a
                 αs_chunk = [np.sum(u, axis=1) for u in us_chunk]
-                βs_chunk = [np.sum(u + prior_a, axis=1) - α for (α, u) in zip(αs_chunk, us)]
+                βs_chunk = [np.sum(u + prior_a, axis=1) - α for (α, u) in zip(αs_chunk, us_chunk)]
             elif prior == "gaussian":
-                σs_chunk = [σ[:,gene_from:gene_to] for σ in σs]
+                σs_chunk = [σ[:,chunk_span] for σ in σs]
 
             scores_chunk, tpr_chunk = score_chunk(
                 xys=xys,
                 us=us_chunk,
                 cell_counts=cell_counts,
                 objective_weights=objective_weights,
                 sample_v=sample_v,
@@ -249,16 +253,16 @@
                 nepochs=nepochs,
                 resample_frequency=resample_frequency,
                 nevalsamples=nevalsamples,
                 max_unimproved_count=max_unimproved_count,
                 preload=preload,
                 quiet=quiet)
 
-            scores_chunks.append(scores_chunk)
-            tpr_chunks.append(tpr_chunk)
+            scores_chunks.append(scores_chunk[1:])
+            tpr_chunks.append(tpr_chunk[:,1:])
 
         scores[:,receiver_gene] = jnp.concatenate(scores_chunks)
 
     for adata in adatas:
         adata.varp["pairwise_spatial_information"] = np.array(scores)
```

### Comparing `maxspin-0.1.0/maxspin/spatial_information.py` & `maxspin-0.1.1/maxspin/spatial_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
 from anndata import AnnData
 from flax import linen as nn
 from functools import partial
-from jax.experimental.maps import FrozenDict
+from flax.core import FrozenDict
 from scipy import sparse
+from scipy.stats import binom
 from tqdm import tqdm
 from typing import Optional, Any, Callable, List, Union
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 import sys
 import h5py
 import time
+import tensorflow_probability.substrates.jax.distributions as tfd
 
 from .objectives import genewise_js
 from .binning import spatially_bin_adata
 
 Array = Any
 
 def spatial_information(
@@ -134,14 +136,17 @@
         quiet: Don't print stuff to stdout while running.
 
     Returns:
         Modifies each `adata` with with the following keys:
 
         - `anndata.AnnData.var["spatial_information"]`: Lower bound on spatial
             information for each gene.
+        - `anndata.AnnData.var["spatial_information_pvalue"]`: P-values from
+            testing the null hypothesis of no spatial organization.
+        - `anndata.AnnData.var["spatial_information_pvalue"]`: Log transformed p-values.
         - `anndata.AnnData.layers["spatial_information_acc"]`: Per spot/cell
             classifier accuracy. Useful for visualizing what regions were
             inferred to have high spatial coherence..
     """
 
     if isinstance(adatas, AnnData):
         adatas = [adatas]
@@ -321,16 +326,21 @@
 
         scores_chunks.append(scores_chunk)
         tpr_chunks.append(tpr_chunk)
 
     scores = jnp.concatenate(scores_chunks)
     tpr = jnp.concatenate(tpr_chunks, axis=1)
 
+    pvalues = binom(tpr.shape[0], 0.5).cdf(np.sum(tpr < 0.05, axis=0))
+    log_pvalues = binom(tpr.shape[0], 0.5).logcdf(np.sum(tpr < 0.05, axis=0))
+
     for adata in adatas:
         adata.var["spatial_information"] = np.array(scores)
+        adata.var["spatial_information_pvalue"] = pvalues
+        adata.var["spatial_information_log_pvalue"] = log_pvalues
 
         # This is mostly monotonic, and arguably more interpretable
         # adata.var["spatial_information"] = np.mean(np.array(tpr), axis=0)
 
     adatas[0].layers["spatial_information_acc"] = np.array(tpr)
 
 
@@ -781,15 +791,15 @@
         mutable=["batch_stats"])
 
     return mi_lower_bounds, metrics["tp"]
 
 
 @jax.jit
 def sample_signals_gamma(key, v, v_mean, v_std, post_θ, prior_k, cell_count):
-    v_sample = jnp.log1p(post_θ * jax.random.gamma(key, v + prior_k * cell_count) / cell_count)
+    v_sample = jnp.log1p(tfd.Gamma(concentration=v + prior_k * cell_count, rate=cell_count/post_θ).sample(seed=key))
     v_sample = (v_sample - v_mean) / v_std
     return v_sample
 
 
 @jax.jit
 def sample_signals_dirichlet(key, v, α, β, v_mean, v_std, scale):
     p = jnp.expand_dims(jax.random.beta(key, α, β), axis=-1)
```

### Comparing `maxspin-0.1.0/PKG-INFO` & `maxspin-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: maxspin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Estimate spatial information in spatial -omics datasets.
 Home-page: https://github.com/dcjones/maxspin
 Author: Daniel C. Jones
 Author-email: djones3@fredhutch.org
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: anndata (>=0.8.0,<0.9.0)
-Requires-Dist: flax (>=0.4.2,<0.5.0)
-Requires-Dist: jax (>=0.3.13,<0.4.0)
+Requires-Dist: flax (>=0.6.9,<0.7.0)
+Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: optax (>=0.1.2,<0.2.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
+Requires-Dist: squidpy (>=1.2.3,<2.0.0)
+Requires-Dist: tensorflow-probability (>=0.19.0,<0.20.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Project-URL: Documentation, https://github.com/dcjones/maxspin
 Project-URL: Repository, https://github.com/dcjones/maxspin
 Description-Content-Type: text/markdown
 
 
 ![Maxspin](https://raw.github.com/dcjones/maxspin/main/logo.png)
```

