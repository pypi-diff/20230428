# Comparing `tmp/vamb-4.1.0.tar.gz` & `tmp/vamb-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vamb-4.1.0.tar", last modified: Fri Apr 21 09:42:18 2023, max compression
+gzip compressed data, was "vamb-4.1.1.tar", last modified: Fri Apr 28 10:39:53 2023, max compression
```

## Comparing `vamb-4.1.0.tar` & `vamb-4.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.090484 vamb-4.1.0/
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1081 2023-03-10 08:42:57.000000 vamb-4.1.0/LICENSE
--rw-r--r--   0 jakni     (1000) jakni     (1000)       24 2023-03-10 08:42:57.000000 vamb-4.1.0/MANIFEST.in
--rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-04-21 09:42:18.090484 vamb-4.1.0/PKG-INFO
--rw-r--r--   0 jakni     (1000) jakni     (1000)    15245 2023-03-30 12:20:17.000000 vamb-4.1.0/README.md
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1005 2023-04-21 09:41:38.000000 vamb-4.1.0/pyproject.toml
--rw-r--r--   0 jakni     (1000) jakni     (1000)      146 2023-04-21 09:42:18.090484 vamb-4.1.0/setup.cfg
--rw-r--r--   0 jakni     (1000) jakni     (1000)      128 2023-03-10 08:42:57.000000 vamb-4.1.0/setup.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.087151 vamb-4.1.0/src/
--rw-r--r--   0 jakni     (1000) jakni     (1000)     2846 2023-03-10 08:42:57.000000 vamb-4.1.0/src/_vambtools.pyx
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1804 2023-03-30 12:20:17.000000 vamb-4.1.0/src/concatenate.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.087151 vamb-4.1.0/test/
--rw-r--r--   0 jakni     (1000) jakni     (1000)    12734 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_benchmark.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     4879 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_cluster.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     7231 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_encode.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     3392 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_parsebam.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     3841 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_parsecontigs.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     5604 2023-04-17 07:28:18.000000 vamb-4.1.0/test/test_results.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    18325 2023-04-12 11:37:11.000000 vamb-4.1.0/test/test_vambtools.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1425 2023-04-12 11:37:11.000000 vamb-4.1.0/test/testtools.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.090484 vamb-4.1.0/vamb/
--rw-r--r--   0 jakni     (1000) jakni     (1000)      941 2023-04-21 09:41:38.000000 vamb-4.1.0/vamb/__init__.py
--rwxr-xr-x   0 jakni     (1000) jakni     (1000)    42915 2023-04-21 09:30:49.000000 vamb-4.1.0/vamb/__main__.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    17951 2023-04-21 09:30:49.000000 vamb-4.1.0/vamb/aamb_encode.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    25117 2023-04-19 06:13:21.000000 vamb-4.1.0/vamb/benchmark.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    19328 2023-04-21 09:30:49.000000 vamb-4.1.0/vamb/cluster.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    22117 2023-04-21 09:30:49.000000 vamb-4.1.0/vamb/encode.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    77187 2022-04-05 08:20:29.000000 vamb-4.1.0/vamb/kernel.npz
--rw-r--r--   0 jakni     (1000) jakni     (1000)     7902 2023-04-17 07:28:18.000000 vamb-4.1.0/vamb/parsebam.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     7041 2023-04-17 07:28:18.000000 vamb-4.1.0/vamb/parsecontigs.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    21213 2023-04-21 09:41:38.000000 vamb-4.1.0/vamb/vambtools.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-21 09:42:18.090484 vamb-4.1.0/vamb.egg-info/
--rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/PKG-INFO
--rw-r--r--   0 jakni     (1000) jakni     (1000)      620 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/SOURCES.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)        1 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/dependency_links.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/entry_points.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/requires.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)        5 2023-04-21 09:42:18.000000 vamb-4.1.0/vamb.egg-info/top_level.txt
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-28 10:39:53.979144 vamb-4.1.1/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1081 2023-03-10 08:42:57.000000 vamb-4.1.1/LICENSE
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       24 2023-03-10 08:42:57.000000 vamb-4.1.1/MANIFEST.in
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-04-28 10:39:53.979144 vamb-4.1.1/PKG-INFO
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    15245 2023-03-30 12:20:17.000000 vamb-4.1.1/README.md
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1005 2023-04-21 09:41:38.000000 vamb-4.1.1/pyproject.toml
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      146 2023-04-28 10:39:53.979144 vamb-4.1.1/setup.cfg
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      128 2023-03-10 08:42:57.000000 vamb-4.1.1/setup.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-28 10:39:53.979144 vamb-4.1.1/src/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     2846 2023-03-10 08:42:57.000000 vamb-4.1.1/src/_vambtools.pyx
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1804 2023-03-30 12:20:17.000000 vamb-4.1.1/src/concatenate.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-28 10:39:53.979144 vamb-4.1.1/test/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    12734 2023-04-17 07:28:18.000000 vamb-4.1.1/test/test_benchmark.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     4879 2023-04-17 07:28:18.000000 vamb-4.1.1/test/test_cluster.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7231 2023-04-17 07:28:18.000000 vamb-4.1.1/test/test_encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     3392 2023-04-17 07:28:18.000000 vamb-4.1.1/test/test_parsebam.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     3841 2023-04-17 07:28:18.000000 vamb-4.1.1/test/test_parsecontigs.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     5604 2023-04-17 07:28:18.000000 vamb-4.1.1/test/test_results.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    18325 2023-04-12 11:37:11.000000 vamb-4.1.1/test/test_vambtools.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1425 2023-04-12 11:37:11.000000 vamb-4.1.1/test/testtools.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-28 10:39:53.979144 vamb-4.1.1/vamb/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      941 2023-04-28 10:39:35.000000 vamb-4.1.1/vamb/__init__.py
+-rwxr-xr-x   0 jakni     (1000) jakni     (1000)    42915 2023-04-21 09:30:49.000000 vamb-4.1.1/vamb/__main__.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    17951 2023-04-21 09:30:49.000000 vamb-4.1.1/vamb/aamb_encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    25117 2023-04-19 06:13:21.000000 vamb-4.1.1/vamb/benchmark.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    19328 2023-04-21 09:30:49.000000 vamb-4.1.1/vamb/cluster.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    22117 2023-04-21 09:30:49.000000 vamb-4.1.1/vamb/encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    77187 2022-04-05 08:20:29.000000 vamb-4.1.1/vamb/kernel.npz
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7905 2023-04-28 10:39:35.000000 vamb-4.1.1/vamb/parsebam.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7041 2023-04-17 07:28:18.000000 vamb-4.1.1/vamb/parsecontigs.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    21213 2023-04-21 09:41:38.000000 vamb-4.1.1/vamb/vambtools.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-04-28 10:39:53.979144 vamb-4.1.1/vamb.egg-info/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-04-28 10:39:53.000000 vamb-4.1.1/vamb.egg-info/PKG-INFO
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      620 2023-04-28 10:39:53.000000 vamb-4.1.1/vamb.egg-info/SOURCES.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)        1 2023-04-28 10:39:53.000000 vamb-4.1.1/vamb.egg-info/dependency_links.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-04-28 10:39:53.000000 vamb-4.1.1/vamb.egg-info/entry_points.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-04-28 10:39:53.000000 vamb-4.1.1/vamb.egg-info/requires.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)        5 2023-04-28 10:39:53.000000 vamb-4.1.1/vamb.egg-info/top_level.txt
```

### Comparing `vamb-4.1.0/LICENSE` & `vamb-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/README.md` & `vamb-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/pyproject.toml` & `vamb-4.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/src/_vambtools.pyx` & `vamb-4.1.1/src/_vambtools.pyx`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/src/concatenate.py` & `vamb-4.1.1/src/concatenate.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/test/test_benchmark.py` & `vamb-4.1.1/test/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/test/test_cluster.py` & `vamb-4.1.1/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/test/test_encode.py` & `vamb-4.1.1/test/test_encode.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/test/test_parsebam.py` & `vamb-4.1.1/test/test_parsebam.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/test/test_parsecontigs.py` & `vamb-4.1.1/test/test_parsecontigs.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/test/test_results.py` & `vamb-4.1.1/test/test_results.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/test/test_vambtools.py` & `vamb-4.1.1/test/test_vambtools.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/test/testtools.py` & `vamb-4.1.1/test/testtools.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb/__init__.py` & `vamb-4.1.1/vamb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 3) Calculate a Composition of contigs using vamb.parsecontigs
 4) Create Abundance object from BAM files using vamb.parsebam
 5) Train autoencoder using vamb.encode
 6) Cluster latent representation using vamb.cluster
 7) Split bins using vamb.vambtools
 """
 
-__version__ = (4, 1, 0)
+__version__ = (4, 1, 1)
 
 from . import vambtools
 from . import parsebam
 from . import parsecontigs
 from . import cluster
 from . import benchmark
 from . import encode
```

### Comparing `vamb-4.1.0/vamb/__main__.py` & `vamb-4.1.1/vamb/__main__.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb/aamb_encode.py` & `vamb-4.1.1/vamb/aamb_encode.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb/benchmark.py` & `vamb-4.1.1/vamb/benchmark.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb/cluster.py` & `vamb-4.1.1/vamb/cluster.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb/encode.py` & `vamb-4.1.1/vamb/encode.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb/kernel.npz` & `vamb-4.1.1/vamb/kernel.npz`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb/parsebam.py` & `vamb-4.1.1/vamb/parsebam.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         paths: list[Path],
         cache_directory: Path,
         nthreads: int,
         minid: float,
         target_refhash: Optional[bytes],
         mask: _np.ndarray,
     ) -> A:
-        _os.mkdir(cache_directory)
+        _os.makedirs(cache_directory)
 
         chunks = [
             (i, min(len(paths), i + nthreads)) for i in range(0, len(paths), nthreads)
         ]
         filenames = [
             _os.path.join(cache_directory, str(i) + ".npz") for i in range(len(chunks))
         ]
```

### Comparing `vamb-4.1.0/vamb/parsecontigs.py` & `vamb-4.1.1/vamb/parsecontigs.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb/vambtools.py` & `vamb-4.1.1/vamb/vambtools.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.0/vamb.egg-info/SOURCES.txt` & `vamb-4.1.1/vamb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

