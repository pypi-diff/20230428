# Comparing `tmp/ancIBD-0.3a1.tar.gz` & `tmp/ancIBD-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ancIBD-0.3a1.tar", last modified: Sun Feb 12 15:47:02 2023, max compression
+gzip compressed data, was "ancIBD-0.4.tar", last modified: Fri Apr 28 18:05:29 2023, max compression
```

## Comparing `ancIBD-0.3a1.tar` & `ancIBD-0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-02-12 15:47:02.918393 ancIBD-0.3a1/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       20 2023-02-12 15:08:40.000000 ancIBD-0.3a1/MANIFEST.in
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     5701 2023-02-12 15:47:02.914458 ancIBD-0.3a1/PKG-INFO
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4638 2023-02-12 15:44:12.000000 ancIBD-0.3a1/README.md
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-02-12 15:47:02.625450 ancIBD-0.3a1/ancIBD/
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-02-12 15:47:02.690843 ancIBD-0.3a1/ancIBD/.ipynb_checkpoints/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    21842 2023-02-12 15:19:48.000000 ancIBD-0.3a1/ancIBD/.ipynb_checkpoints/cfunc-checkpoint.pyx
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-02-12 15:47:02.807528 ancIBD-0.3a1/ancIBD/IO/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2022-05-31 15:02:15.000000 ancIBD-0.3a1/ancIBD/IO/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8719 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/IO/batch_run.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4518 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/IO/h5_load.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8621 2023-02-12 15:18:09.000000 ancIBD-0.3a1/ancIBD/IO/h5_modify.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     2888 2022-05-31 15:02:15.000000 ancIBD-0.3a1/ancIBD/IO/h5_qc.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     7793 2022-05-31 15:02:15.000000 ancIBD-0.3a1/ancIBD/IO/ind_ibd.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6606 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/IO/prepare_h5.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2022-05-31 15:02:15.000000 ancIBD-0.3a1/ancIBD/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)  1193188 2023-02-12 15:25:39.000000 ancIBD-0.3a1/ancIBD/cfunc.c
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    21842 2023-02-12 15:19:48.000000 ancIBD-0.3a1/ancIBD/cfunc.pyx
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6333 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/emission.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     3212 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/hmm.py
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-02-12 15:47:02.833614 ancIBD-0.3a1/ancIBD/ibd_stats/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2022-05-31 15:02:15.000000 ancIBD-0.3a1/ancIBD/ibd_stats/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8012 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/ibd_stats/funcs.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    10909 2023-02-12 15:20:25.000000 ancIBD-0.3a1/ancIBD/loaddata.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6150 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/main.py
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-02-12 15:47:02.896540 ancIBD-0.3a1/ancIBD/plot/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2022-05-31 15:02:15.000000 ancIBD-0.3a1/ancIBD/plot/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1096 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/plot/plot_df.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    10726 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/plot/plot_karyotype.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     3659 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/plot/plot_opphomos.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4583 2022-05-31 15:02:15.000000 ancIBD-0.3a1/ancIBD/plot/plot_posterior.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6858 2022-05-31 15:02:15.000000 ancIBD-0.3a1/ancIBD/postprocessing.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    11155 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/run.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6744 2023-02-12 15:08:40.000000 ancIBD-0.3a1/ancIBD/transition.py
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-02-12 15:47:02.682368 ancIBD-0.3a1/ancIBD.egg-info/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     5701 2023-02-12 15:47:01.000000 ancIBD-0.3a1/ancIBD.egg-info/PKG-INFO
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)      748 2023-02-12 15:47:02.656964 ancIBD-0.3a1/ancIBD.egg-info/SOURCES.txt
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        1 2023-02-12 15:47:01.000000 ancIBD-0.3a1/ancIBD.egg-info/dependency_links.txt
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       68 2023-02-12 15:47:02.677424 ancIBD-0.3a1/ancIBD.egg-info/requires.txt
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        7 2023-02-12 15:47:02.685808 ancIBD-0.3a1/ancIBD.egg-info/top_level.txt
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       38 2023-02-12 15:47:02.922311 ancIBD-0.3a1/setup.cfg
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1376 2023-02-12 15:45:51.000000 ancIBD-0.3a1/setup.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-28 18:05:29.616198 ancIBD-0.4/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       20 2023-02-12 15:08:40.000000 ancIBD-0.4/MANIFEST.in
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     5699 2023-04-28 18:05:29.614488 ancIBD-0.4/PKG-INFO
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4638 2023-02-12 15:44:12.000000 ancIBD-0.4/README.md
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-28 18:05:29.321193 ancIBD-0.4/ancIBD/
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-28 18:05:29.406412 ancIBD-0.4/ancIBD/.ipynb_checkpoints/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    21842 2023-02-12 15:19:48.000000 ancIBD-0.4/ancIBD/.ipynb_checkpoints/cfunc-checkpoint.pyx
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-28 18:05:29.501336 ancIBD-0.4/ancIBD/IO/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2022-05-31 15:02:15.000000 ancIBD-0.4/ancIBD/IO/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     9654 2023-04-12 15:26:06.000000 ancIBD-0.4/ancIBD/IO/batch_run.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4518 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/IO/h5_load.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8621 2023-02-12 15:18:09.000000 ancIBD-0.4/ancIBD/IO/h5_modify.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     2888 2022-05-31 15:02:15.000000 ancIBD-0.4/ancIBD/IO/h5_qc.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     7793 2022-05-31 15:02:15.000000 ancIBD-0.4/ancIBD/IO/ind_ibd.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6606 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/IO/prepare_h5.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2022-05-31 15:02:15.000000 ancIBD-0.4/ancIBD/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)  1193291 2023-04-28 18:05:28.000000 ancIBD-0.4/ancIBD/cfunc.c
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    21842 2023-02-12 15:19:48.000000 ancIBD-0.4/ancIBD/cfunc.pyx
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6333 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/emission.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     3212 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/hmm.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-28 18:05:29.523830 ancIBD-0.4/ancIBD/ibd_stats/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2022-05-31 15:02:15.000000 ancIBD-0.4/ancIBD/ibd_stats/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8012 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/ibd_stats/funcs.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    11840 2023-04-28 17:54:34.000000 ancIBD-0.4/ancIBD/loaddata.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6150 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/main.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-28 18:05:29.600599 ancIBD-0.4/ancIBD/plot/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2022-05-31 15:02:15.000000 ancIBD-0.4/ancIBD/plot/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1096 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/plot/plot_df.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    10726 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/plot/plot_karyotype.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     3659 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/plot/plot_opphomos.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4583 2022-05-31 15:02:15.000000 ancIBD-0.4/ancIBD/plot/plot_posterior.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6858 2022-05-31 15:02:15.000000 ancIBD-0.4/ancIBD/postprocessing.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    11207 2023-03-24 10:06:17.000000 ancIBD-0.4/ancIBD/run.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6744 2023-02-12 15:08:40.000000 ancIBD-0.4/ancIBD/transition.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-28 18:05:29.394588 ancIBD-0.4/ancIBD.egg-info/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     5699 2023-04-28 18:05:28.000000 ancIBD-0.4/ancIBD.egg-info/PKG-INFO
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)      748 2023-04-28 18:05:28.000000 ancIBD-0.4/ancIBD.egg-info/SOURCES.txt
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        1 2023-04-28 18:05:28.000000 ancIBD-0.4/ancIBD.egg-info/dependency_links.txt
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       68 2023-04-28 18:05:28.000000 ancIBD-0.4/ancIBD.egg-info/requires.txt
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        7 2023-04-28 18:05:28.000000 ancIBD-0.4/ancIBD.egg-info/top_level.txt
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       38 2023-04-28 18:05:29.617478 ancIBD-0.4/setup.cfg
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1374 2023-04-28 18:04:26.000000 ancIBD-0.4/setup.py
```

### Comparing `ancIBD-0.3a1/PKG-INFO` & `ancIBD-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ancIBD
-Version: 0.3a1
+Version: 0.4
 Summary: Identify IBD segments between pairs of individuals in ancient human DNA data
 Home-page: https://github.com/hringbauer/ancIBD
 Author: Harald Ringbauer
 Author-email: harald_ringbauer@eva.mpg.de
 License: UNKNOWN
 Description: # ancIBD
         This Python software package screens ancient human DNA for long IBD blocks (Identity by Descent segments) shared between pairs of individuals.
```

### Comparing `ancIBD-0.3a1/README.md` & `ancIBD-0.4/README.md`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/.ipynb_checkpoints/cfunc-checkpoint.pyx` & `ancIBD-0.4/ancIBD/.ipynb_checkpoints/cfunc-checkpoint.pyx`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/IO/batch_run.py` & `ancIBD-0.4/ancIBD/IO/batch_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,21 @@
 
 #########################################################
 
 def get_iids(path_meta="/n/groups/reich/hringbauer/git/yamnaya/data/meta_v2.tsv", min_snps = 600000):
     """Return list of iids to run"""
     df1 = pd.read_csv(path_meta, sep="\t")
     df1 = df1[df1["include"]==1].copy().reset_index(drop=True) # Only include unique,unrelated samples
-    df2 = df1[df1["n_cov_snp"]>min_snps].copy()
-    print(f"Loaded {len(df2)}/{len(df1)} samples with min snps: >{min_snps}")
+    if min_snps>0:
+        df2 = df1[df1["n_cov_snp"]>min_snps].copy()
+        print(f"Loaded {len(df2)}/{len(df1)} samples with min snps: >{min_snps}")
+    else:
+        df2 = df1.copy()
+        print(f"Loaded {len(df2)}/{len(df1)} samples with include==1")
+    
     iids = df2["iid"].values
     return iids
 
 def get_batch_idcs(i, batch_size):
     """Return the Index of batch and the within batch index"""
     iw = i % batch_size       # Within Index
     ib = int(i / batch_size)  # Batch index
@@ -193,7 +198,26 @@
         folder_batch = os.path.join(folder_out, f"batch{b1}_{b2}/")
         df_ibds = join_chromosomes(folder_batch, file_out="", 
                                    chs=chs, output=output)
         res.append(df_ibds)
     df_res = pd.concat(res)
     df_res = filter_ibd_df(df_res, min_cm=min_cm, snp_cm=snp_cm, output=output) 
     return df_res 
+
+
+def print_runid_missing(b = 1, folder_out = "", output=False):
+    """Finds and prints indices of missing output (chXX.tsv) for batchwise runs.
+    Return list of missing indices. Ideal for rerunning batch scripts.
+    Uses C Indexing as would be used in submission script."""
+    batches = np.column_stack(np.tril_indices(n=b, k=0))
+
+    ls = []
+    for ch in range(1,23):
+        for b1,b2 in batches:
+            folder_batch = os.path.join(folder_out, f"batch{b1}_{b2}/ch{ch}.tsv")
+            exist = os.path.exists(folder_batch)
+            if not exist:
+                if output:
+                    print(f"Missing! ch: {ch} batch: {b1}-{b2}")
+                l = b * (b+1)/2 * (ch-1) + (b1+1) * b1/2 + b2 + 1 # The +1 is c indexing
+                ls.append(str(int(l)))
+    return ls
```

### Comparing `ancIBD-0.3a1/ancIBD/IO/h5_load.py` & `ancIBD-0.4/ancIBD/IO/h5_load.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/IO/h5_modify.py` & `ancIBD-0.4/ancIBD/IO/h5_modify.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/IO/h5_qc.py` & `ancIBD-0.4/ancIBD/IO/h5_qc.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/IO/ind_ibd.py` & `ancIBD-0.4/ancIBD/IO/ind_ibd.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/IO/prepare_h5.py` & `ancIBD-0.4/ancIBD/IO/prepare_h5.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/cfunc.c` & `ancIBD-0.4/ancIBD/cfunc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "ancIBD.cfunc",
         "sources": [
-            "/mnt/archgen/users/hringbauer/git/hapBLOCK/package/ancIBD/cfunc.pyx"
+            "ancIBD/cfunc.pyx"
         ]
     },
     "module_name": "ancIBD.cfunc"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -212,15 +212,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -251,15 +251,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -965,15 +965,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "cfunc.pyx",
+  "ancIBD/cfunc.pyx",
   "stringsource",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
@@ -2119,15 +2119,14 @@
 static const char __pyx_k_mb_usage[] = "mb_usage";
 static const char __pyx_k_n_states[] = "n_states";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_three_vi[] = "three_vi";
 static const char __pyx_k_trans_ll[] = "trans_ll";
 static const char __pyx_k_TypeError[] = "TypeError";
-static const char __pyx_k_cfunc_pyx[] = "cfunc.pyx";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_post_view[] = "post_view";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_trans_ll1[] = "trans_ll1";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
@@ -2153,14 +2152,15 @@
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
 static const char __pyx_k_fwd_bkwd_lowmem[] = "fwd_bkwd_lowmem";
 static const char __pyx_k_fwd_bkwd_scaled[] = "fwd_bkwd_scaled";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_ancIBD_cfunc_pyx[] = "ancIBD/cfunc.pyx";
 static const char __pyx_k_Memory_Usage_Full[] = "Memory Usage Full:";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_print_memory_usage[] = "print_memory_usage";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_Log_likelihood_Path[] = "Log likelihood Path: ";
 static const char __pyx_k_Total_Log_likelihood[] = "Total Log likelihood: ";
@@ -2218,24 +2218,24 @@
 static PyObject *__pyx_kp_u_Total_Log_likelihood;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_ancIBD_cfunc;
+static PyObject *__pyx_kp_s_ancIBD_cfunc_pyx;
 static PyObject *__pyx_n_s_argmax;
 static PyObject *__pyx_n_s_asarray;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_bwd;
 static PyObject *__pyx_n_s_bwd0;
 static PyObject *__pyx_n_s_bwd1;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_c_view;
-static PyObject *__pyx_kp_s_cfunc_pyx;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
@@ -24912,24 +24912,24 @@
   {&__pyx_kp_u_Total_Log_likelihood, __pyx_k_Total_Log_likelihood, sizeof(__pyx_k_Total_Log_likelihood), 0, 1, 0, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_ancIBD_cfunc, __pyx_k_ancIBD_cfunc, sizeof(__pyx_k_ancIBD_cfunc), 0, 0, 1, 1},
+  {&__pyx_kp_s_ancIBD_cfunc_pyx, __pyx_k_ancIBD_cfunc_pyx, sizeof(__pyx_k_ancIBD_cfunc_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_argmax, __pyx_k_argmax, sizeof(__pyx_k_argmax), 0, 0, 1, 1},
   {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_bwd, __pyx_k_bwd, sizeof(__pyx_k_bwd), 0, 0, 1, 1},
   {&__pyx_n_s_bwd0, __pyx_k_bwd0, sizeof(__pyx_k_bwd0), 0, 0, 1, 1},
   {&__pyx_n_s_bwd1, __pyx_k_bwd1, sizeof(__pyx_k_bwd1), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_c_view, __pyx_k_c_view, sizeof(__pyx_k_c_view), 0, 0, 1, 1},
-  {&__pyx_kp_s_cfunc_pyx, __pyx_k_cfunc_pyx, sizeof(__pyx_k_cfunc_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
@@ -25378,75 +25378,75 @@
  * def print_memory_usage():             # <<<<<<<<<<<<<<
  *     """Print the current Memory Usage in mB"""
  *     process = psutil.Process(os.getpid())
  */
   __pyx_tuple__29 = PyTuple_Pack(2, __pyx_n_s_process, __pyx_n_s_mb_usage); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_print_memory_usage, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ancIBD_cfunc_pyx, __pyx_n_s_print_memory_usage, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 46, __pyx_L1_error)
 
   /* "ancIBD/cfunc.pyx":53
  * 
  * 
  * def fwd_bkwd(double[:, :] e_mat, double[:, :] t_mat,             # <<<<<<<<<<<<<<
  *              double[:, :] fwd, double[:, :] bwd, double[:,:,:] t,
  *              full=False, output=True):
  */
   __pyx_tuple__31 = PyTuple_Pack(20, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_fwd, __pyx_n_s_bwd, __pyx_n_s_t, __pyx_n_s_full, __pyx_n_s_output, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_post, __pyx_n_s_trans_ll, __pyx_n_s_trans_ll_view, __pyx_n_s_t_mat0, __pyx_n_s_e_mat0, __pyx_n_s_tot_ll, __pyx_n_s_fwd1, __pyx_n_s_bwd1); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(7, 0, 20, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(7, 0, 20, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ancIBD_cfunc_pyx, __pyx_n_s_fwd_bkwd, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 53, __pyx_L1_error)
 
   /* "ancIBD/cfunc.pyx":109
  * 
  * 
  * def fwd_bkwd_fast(double[:, :] e_mat, double[:, :, :] t_mat, double in_val = 1e-4,             # <<<<<<<<<<<<<<
  *                   full=False, output=True):
  *     """Takes emission and transition probabilities, and calculates posteriors.
  */
   __pyx_tuple__33 = PyTuple_Pack(30, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_in_val, __pyx_n_s_full, __pyx_n_s_output, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_stay, __pyx_n_s_post, __pyx_n_s_trans_ll, __pyx_n_s_trans_ll_view, __pyx_n_s_trans_ll1, __pyx_n_s_trans_ll_view1, __pyx_n_s_three_v, __pyx_n_s_three_v_view, __pyx_n_s_two_v, __pyx_n_s_two_v_view, __pyx_n_s_t0, __pyx_n_s_e_mat0, __pyx_n_s_fwd0, __pyx_n_s_fwd, __pyx_n_s_bwd0, __pyx_n_s_bwd, __pyx_n_s_f_l, __pyx_n_s_tot_ll, __pyx_n_s_fwd1, __pyx_n_s_bwd1); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(5, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd_fast, 109, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(5, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ancIBD_cfunc_pyx, __pyx_n_s_fwd_bkwd_fast, 109, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 109, __pyx_L1_error)
 
   /* "ancIBD/cfunc.pyx":224
  * 
  * 
  * def fwd_bkwd_lowmem(double[:, :] e_mat, double[:, :, :] t_mat, double in_val = 1e-4,             # <<<<<<<<<<<<<<
  *                     full=False, output=True):
  *     """Takes emission and transition probabilities, and calculates posteriors.
  */
   __pyx_tuple__35 = PyTuple_Pack(31, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_in_val, __pyx_n_s_full, __pyx_n_s_output, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_stay, __pyx_n_s_tot_ll, __pyx_n_s_post, __pyx_n_s_post_view, __pyx_n_s_trans_ll, __pyx_n_s_trans_ll_view, __pyx_n_s_trans_ll1, __pyx_n_s_trans_ll_view1, __pyx_n_s_three_v, __pyx_n_s_three_v_view, __pyx_n_s_two_v, __pyx_n_s_two_v_view, __pyx_n_s_t0, __pyx_n_s_e_mat0, __pyx_n_s_fwd0, __pyx_n_s_fwd, __pyx_n_s_bwd0, __pyx_n_s_bwd, __pyx_n_s_tmp0, __pyx_n_s_tmp, __pyx_n_s_f_l); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(5, 0, 31, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd_lowmem, 224, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(5, 0, 31, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ancIBD_cfunc_pyx, __pyx_n_s_fwd_bkwd_lowmem, 224, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 224, __pyx_L1_error)
 
   /* "ancIBD/cfunc.pyx":357
  * ###############################################################################
  * 
  * def fwd_bkwd_scaled(double[:, :] e_mat, double[:, :, :] t_mat,             # <<<<<<<<<<<<<<
  *                     double in_val = 1e-4, full=False, output=True):
  *     """Takes emission and transition probabilities, and calculates posteriors.
  */
   __pyx_tuple__37 = PyTuple_Pack(28, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_in_val, __pyx_n_s_full, __pyx_n_s_output, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_stay, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_x3, __pyx_n_s_post, __pyx_n_s_c, __pyx_n_s_c_view, __pyx_n_s_temp, __pyx_n_s_temp_v, __pyx_n_s_temp1, __pyx_n_s_temp1_v, __pyx_n_s_t, __pyx_n_s_fwd1, __pyx_n_s_fwd, __pyx_n_s_bwd1, __pyx_n_s_bwd, __pyx_n_s_f_l, __pyx_n_s_tot_ll); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(5, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd_scaled, 357, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(5, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ancIBD_cfunc_pyx, __pyx_n_s_fwd_bkwd_scaled, 357, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 357, __pyx_L1_error)
 
   /* "ancIBD/cfunc.pyx":475
  * ### Viterbi Path
  * 
  * def viterbi_path(double[:, :] e_mat0, double[:, :, :] t_mat0, double[:] end_p0):             # <<<<<<<<<<<<<<
  *     """Implementation of a Viterbi Path.
  *     e_mat0  Matrices with Emission Probabilities, [k,l] (log space)
  */
   __pyx_tuple__39 = PyTuple_Pack(25, __pyx_n_s_e_mat0, __pyx_n_s_t_mat0, __pyx_n_s_end_p0, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_m, __pyx_n_s_v, __pyx_n_s_mp, __pyx_n_s_new_p, __pyx_n_s_pt, __pyx_n_s_trans_ll, __pyx_n_s_trans_ll_view, __pyx_n_s_three_v, __pyx_n_s_three_v_view, __pyx_n_s_three_vi, __pyx_n_s_three_vi_view, __pyx_n_s_two_v, __pyx_n_s_two_v_view, __pyx_n_s_two_vi, __pyx_n_s_two_vi_view, __pyx_n_s_path, __pyx_n_s_x); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 475, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_viterbi_path, 475, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ancIBD_cfunc_pyx, __pyx_n_s_viterbi_path, 475, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 475, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -27485,28 +27485,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
```

### Comparing `ancIBD-0.3a1/ancIBD/cfunc.pyx` & `ancIBD-0.4/ancIBD/cfunc.pyx`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/emission.py` & `ancIBD-0.4/ancIBD/emission.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/hmm.py` & `ancIBD-0.4/ancIBD/hmm.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/ibd_stats/funcs.py` & `ancIBD-0.4/ancIBD/ibd_stats/funcs.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/loaddata.py` & `ancIBD-0.4/ancIBD/loaddata.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         m = self.return_map()
         self.check_valid_data(htsl, p, m)
         return htsl, p, m
     
     def check_valid_data(self, htsl, p, m):
         """Check whether data in valid format"""
         assert(np.shape(htsl)[1]==len(p))
+        assert(np.sum(np.isnan(htsl))==0) # Check that no NAN exists
         assert(len(p)==len(m))
         pass 
         
     def set_params(self, **kwargs):
         """Set the Parameters.
         Takes keyworded arguments"""
         for key, value in kwargs.items():
@@ -144,15 +145,15 @@
             htsl = np.concatenate((h1,h2), axis=0)
         
         self.check_valid_data(htsl, p, m)
         return htsl, p, m, self.iids
     
 class LoadHDF5Multi(LoadHDF5):
     """Class to load HDF5 data for multiple individuals.
-    Developer Note: In progress of making this default even for pairs of individuals."""
+    Default now also for only pairs of individuals."""
     path_h5=""
     iids = []
     ch = 3   # Which chromosome to load
     min_error = 1e-5 # Minimum Probability of genotyping error  
     p_col = "" # The hdf5 column with der. all freqs. If given, use the field
     # If "default" use p=0.5 everywhere
     # default value for p_col in my hdf5s: variants/AF_ALL
@@ -167,14 +168,29 @@
         h1 = (1-h1) * m[:,:,None] + h1 * (1 - m[:,:,None]) # Probability of being ancestral
         h1 = np.swapaxes(h1, 0, 1) # ->n,l,2
         h1 = np.swapaxes(h1, 1, 2) #-> n,2,l
         h1 = h1.reshape((2*n,l))
         #h1 = np.swapaxes(h1, 0, 1)
         return h1
     
+    def filter_valid_data(self, hts, p, m):
+        """Filter to SNPs with fully valid data. 
+        Return filtered data."""
+        idx = ~(np.isnan(hts).any(axis=0)) # Flag all markers that are not null
+        
+        ### Output and Raise warning if too much data missing:
+        if self.output:
+            print(f"Filtering to {np.sum(idx)}/{len(idx)} SNPs with GP data (on target iids)")   
+        if np.mean(idx)<1:  # Missing Data detected
+            print(f"Attention: Some data in GP field is missing. Ideally, all GP entries are set.")   
+        if np.mean(idx)<0.8:  # Less than 80 percent of data there
+            raise RuntimeWarning(f"Too much data missing: {np.sum(idx)}/{len(idx)} SNPs are NULL for GP")
+            
+        return hts[:,idx], p[idx], m[idx]
+    
     def load_all_data(self, **kwargs):
         """ Return haplotype likelihoods [n*2,l] for anc. allele.
         along first axis: 2*i, 2*(i+1) haplotype of ind i
         derived allele frequencies [l]
         map in Morgan [l]"""
         path_h5_ch = f"{self.path}{self.ch}.h5"
         with h5py.File(path_h5_ch, "r") as f:
@@ -183,16 +199,19 @@
             sort = np.argsort(idcs)   # Get the sorting Indices [has to go low to high]
             samples = self.iids[sort] # Get them in sorted order
             hts = self.get_haplo_prob(f, idcs[sort])
         
             if len(self.p_col)>0:
                 p = self.get_p_hdf5(f, self.p_col)  
             else:
-                p = self.get_p(hts)  # Calculate Mean allele frequency from subset
-            
+                p = self.get_p(hts)  # Calculate Mean allele frequency from sample subset
+                
+        ### Filter to Valid data
+        hts, p, m = self.filter_valid_data(hts, p, m)
+        
         self.check_valid_data(hts, p, m)
         return hts, p, m, samples
     
     def get_p(self, htsl):
         """Get Allele frequency from haplotype probabilities.
         Return array of derived allele freqs [l]"""
         p_anc = np.mean(htsl, axis=0) # Take the expected AF of ancestral.
```

### Comparing `ancIBD-0.3a1/ancIBD/main.py` & `ancIBD-0.4/ancIBD/main.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/plot/plot_df.py` & `ancIBD-0.4/ancIBD/plot/plot_df.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/plot/plot_karyotype.py` & `ancIBD-0.4/ancIBD/plot/plot_karyotype.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/plot/plot_opphomos.py` & `ancIBD-0.4/ancIBD/plot/plot_opphomos.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/plot/plot_posterior.py` & `ancIBD-0.4/ancIBD/plot/plot_posterior.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/postprocessing.py` & `ancIBD-0.4/ancIBD/postprocessing.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD/run.py` & `ancIBD-0.4/ancIBD/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,16 @@
 ### Run and plot in one go - for one pair of iids.
 
 def run_plot_pair(path_h5="/n/groups/reich/hringbauer/git/hapBLOCK/data/hdf5/1240k_v43/ch", 
                   iids = ["", ""], ch=2, xlim=[], folder_out="", 
                   plot=False, path_fig="", output=False, exact=True,
                   ibd_in=1, ibd_out=10, ibd_jump=400, min_cm=2, 
                   cutoff_post=0.99, max_gap=0.0075, 
-                  l_model="hdf5", p_col="variants/AF_ALL",
+                  l_model="hdf5", e_model="haploid_gl", h_model="FiveStateScaled",
+                  p_col="variants/AF_ALL",
                   title="", c="gray", c_hw="maroon", 
                   state=0, return_post=False, **kwargs):
     """Run and plot IBD for pair of Individuals.
     folder_out: Where to save the hapBLOCK output to
     iids: list of two iids [List of Length 2]
     path_fig: Where to save the IBD plot to [String]
     p_col: The dataset to use in hdf5 for der. AF. If default use p=0.5.
@@ -214,15 +215,15 @@
     kwargs: Optional Keyword Arguments for Plotting (e.g. c_ibd)
     """
     assert(len(iids)==2) # Sanity Check of Input IIDs - as here it should be pairs
     
     df_ibd, post, r_vec = hapBLOCK_chrom(
            folder_in=path_h5, iids = iids,  ch=ch, folder_out=folder_out, 
            output=output, prefix_out="", logfile=False,
-           l_model=l_model, e_model="haploid_gl", h_model="FiveStateScaled", 
+           l_model=l_model, e_model=e_model, h_model=h_model, 
            t_model="standard", p_col=p_col, ibd_in=ibd_in, ibd_out=ibd_out, ibd_jump=ibd_jump, 
            min_cm=min_cm, cutoff_post=cutoff_post, max_gap=max_gap)
         
     if plot:
         if len(title)==0:
             title = f"ancIBD v0.5, {iids[0]} - {iids[1]}, Chr. {ch}"
```

### Comparing `ancIBD-0.3a1/ancIBD/transition.py` & `ancIBD-0.4/ancIBD/transition.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/ancIBD.egg-info/PKG-INFO` & `ancIBD-0.4/ancIBD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ancIBD
-Version: 0.3a1
+Version: 0.4
 Summary: Identify IBD segments between pairs of individuals in ancient human DNA data
 Home-page: https://github.com/hringbauer/ancIBD
 Author: Harald Ringbauer
 Author-email: harald_ringbauer@eva.mpg.de
 License: UNKNOWN
 Description: # ancIBD
         This Python software package screens ancient human DNA for long IBD blocks (Identity by Descent segments) shared between pairs of individuals.
```

### Comparing `ancIBD-0.3a1/ancIBD.egg-info/SOURCES.txt` & `ancIBD-0.4/ancIBD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ancIBD-0.3a1/setup.py` & `ancIBD-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     extensions = cythonize(extensions)
   
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name="ancIBD",
-    version="0.3a1",  # a means alpha
+    version="0.4",  # a means alpha
     author="Harald Ringbauer",
     author_email="harald_ringbauer@eva.mpg.de",
     description="Identify IBD segments between pairs of individuals in ancient human DNA data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hringbauer/ancIBD",
     packages=find_packages(),
```

