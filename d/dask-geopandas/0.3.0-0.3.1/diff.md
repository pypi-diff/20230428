# Comparing `tmp/dask-geopandas-0.3.0.tar.gz` & `tmp/dask-geopandas-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-geopandas-0.3.0.tar", last modified: Mon Jan 23 21:31:54 2023, max compression
+gzip compressed data, was "dask-geopandas-0.3.1.tar", last modified: Fri Apr 28 12:48:06 2023, max compression
```

## Comparing `dask-geopandas-0.3.0.tar` & `dask-geopandas-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/dask_geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/dask_geopandas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    33825 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/geohash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/hilbert_distance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/dask_geopandas/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/io/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/io/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/morton_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/sjoin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/dask_geopandas/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/dask_geopandas/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/io/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/io/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/io/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    28602 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/test_geohash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/test_hilbert_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/test_morton_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/test_sjoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/dask_geopandas/tests/test_spatial_partitioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/dask_geopandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-01-23 21:31:54.000000 dask-geopandas-0.3.0/dask_geopandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-01-23 21:31:54.000000 dask-geopandas-0.3.0/dask_geopandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 21:31:54.000000 dask-geopandas-0.3.0/dask_geopandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 21:31:54.000000 dask-geopandas-0.3.0/dask_geopandas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-23 21:31:54.000000 dask-geopandas-0.3.0/dask_geopandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-23 21:31:54.000000 dask-geopandas-0.3.0/dask_geopandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-01-23 21:31:54.975430 dask-geopandas-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-01-23 21:31:46.000000 dask-geopandas-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/dask_geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/dask_geopandas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34276 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/geohash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/hilbert_distance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/dask_geopandas/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/io/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/io/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/morton_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/sjoin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/dask_geopandas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/dask_geopandas/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/io/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/io/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/io/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29266 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/test_geohash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/test_hilbert_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/test_morton_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/test_sjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/dask_geopandas/tests/test_spatial_partitioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/dask_geopandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-28 12:48:06.000000 dask-geopandas-0.3.1/dask_geopandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-28 12:48:06.000000 dask-geopandas-0.3.1/dask_geopandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:48:06.000000 dask-geopandas-0.3.1/dask_geopandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:48:06.000000 dask-geopandas-0.3.1/dask_geopandas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 12:48:06.000000 dask-geopandas-0.3.1/dask_geopandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 12:48:06.000000 dask-geopandas-0.3.1/dask_geopandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 12:48:06.331654 dask-geopandas-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-28 12:47:56.000000 dask-geopandas-0.3.1/versioneer.py
```

### Comparing `dask-geopandas-0.3.0/LICENSE` & `dask-geopandas-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/PKG-INFO` & `dask-geopandas-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-geopandas
-Version: 0.3.0
+Version: 0.3.1
 Summary: Parallel GeoPandas with Dask
 Home-page: https://github.com/geopandas/dask-geopandas
 Maintainer: Julia Signell
 Maintainer-email: jsignell@gmail.com
 License: BSD
 Project-URL: Documentation, https://github.com/geopandas/dask-geopandas
 Project-URL: Source, https://github.com/geopandas/dask-geopandas/
```

### Comparing `dask-geopandas-0.3.0/README.rst` & `dask-geopandas-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/__init__.py` & `dask-geopandas-0.3.1/dask_geopandas/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/backends.py` & `dask-geopandas-0.3.1/dask_geopandas/backends.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/clip.py` & `dask-geopandas-0.3.1/dask_geopandas/clip.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/core.py` & `dask-geopandas-0.3.1/dask_geopandas/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .geohash import _geohash
 
 import dask_geopandas
 
 
 DASK_2022_8_1 = Version(dask.__version__) >= Version("2022.8.1")
 GEOPANDAS_0_12 = Version(geopandas.__version__) >= Version("0.12.0")
+PANDAS_2_0_0 = Version(pd.__version__) >= Version("2.0.0")
 
 
 if Version(shapely.__version__) < Version("2.0"):
     try:
         import pygeos  # noqa
     except ImportError:
         raise ImportError(
@@ -101,14 +102,25 @@
             if len(value) != self.npartitions:
                 raise ValueError(
                     f"Expected spatial partitions of length {self.npartitions}, "
                     f"got {len(value)} instead."
                 )
         self._spatial_partitions = value
 
+    @property
+    def _args(self):
+        # Ensure we roundtrip through pickle correctly
+        # https://github.com/geopandas/dask-geopandas/issues/237
+        return super()._args + (self.spatial_partitions,)
+
+    def __setstate__(self, state):
+        *dask_state, spatial_partitions = state
+        super().__setstate__(dask_state)
+        self.spatial_partitions = spatial_partitions
+
     @classmethod
     def _bind_property(cls, attr, preserve_spatial_partitions=False):
         """Map property to partitions and bind to class"""
 
         def prop(self):
             meta = getattr(self._meta, attr)
             result = self.map_partitions(getattr, attr, token=attr, meta=meta)
```

### Comparing `dask-geopandas-0.3.0/dask_geopandas/geohash.py` & `dask-geopandas-0.3.1/dask_geopandas/geohash.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/hilbert_distance.py` & `dask-geopandas-0.3.1/dask_geopandas/hilbert_distance.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/io/arrow.py` & `dask-geopandas-0.3.1/dask_geopandas/io/arrow.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import pandas as pd
 import geopandas
 import shapely.geometry
 
 from fsspec.core import get_fs_token_paths
 
 DASK_2022_12_0_PLUS = Version(dask.__version__) >= Version("2022.12.0")
+DASK_2023_04_0 = Version(dask.__version__) >= Version("2023.4.0")
 
 
 if TYPE_CHECKING:
     import pyarrow
 
 
 def _update_meta_to_geodataframe(meta, schema_metadata):
@@ -65,14 +66,24 @@
     geometry = metadata["primary_column"]
     bbox = metadata["columns"][geometry].get("bbox", None)
     if bbox is None or all(math.isnan(val) for val in bbox):
         return None
     return shapely.geometry.box(*bbox)
 
 
+def _extract_nullable_dtypes(**kwargs):
+    if DASK_2023_04_0:
+        use_nullable_dtypes = kwargs.get("dtype_backend", None) == "numpy_nullable"
+    elif DASK_2022_12_0_PLUS:
+        use_nullable_dtypes = kwargs.get("use_nullable_dtypes", False)
+    else:
+        use_nullable_dtypes = False
+    return use_nullable_dtypes
+
+
 class ArrowDatasetEngine:
     """
     Custom IO engine based on pyarrow.dataset.
 
     This is designed after dask's ArrowDatasetEngine for Parquet IO (but simpler
     with less options, and not dealing with a legacy engine) and ArrowORCEngine
     for ORC IO (but using pyarrow.dataset for the read_metadata discovery).
@@ -129,16 +140,17 @@
     @classmethod
     def _arrow_table_to_pandas(
         cls, arrow_table: "pyarrow.Table", categories, **kwargs
     ) -> pd.DataFrame:
 
         _kwargs = kwargs.get("arrow_to_pandas", {})
         _kwargs.update({"use_threads": False, "ignore_metadata": False})
+        use_nullable_dtypes = _extract_nullable_dtypes(**kwargs)
 
-        if DASK_2022_12_0_PLUS and kwargs.get("use_nullable_dtypes", False):
+        if use_nullable_dtypes:
             from dask.dataframe.io.parquet.arrow import PYARROW_NULLABLE_DTYPE_MAPPING
 
             if "types_mapper" in _kwargs:
                 # User-provided entries take priority over PYARROW_NULLABLE_DTYPE_MAPPING
                 types_mapper = _kwargs["types_mapper"]
 
                 def _types_mapper(pa_type):
@@ -186,16 +198,17 @@
     def _arrow_table_to_pandas(
         cls, arrow_table: "pyarrow.Table", categories, **kwargs
     ) -> pd.DataFrame:
         from geopandas.io.arrow import _arrow_to_geopandas
 
         _kwargs = kwargs.get("arrow_to_pandas", {})
         _kwargs.update({"use_threads": False, "ignore_metadata": False})
+        use_nullable_dtypes = _extract_nullable_dtypes(**kwargs)
 
-        if DASK_2022_12_0_PLUS and kwargs.get("use_nullable_dtypes", False):
+        if use_nullable_dtypes:
             from dask.dataframe.io.parquet.arrow import PYARROW_NULLABLE_DTYPE_MAPPING
 
             if "types_mapper" in _kwargs:
                 # User-provided entries take priority over PYARROW_NULLABLE_DTYPE_MAPPING
                 types_mapper = _kwargs["types_mapper"]
 
                 def _types_mapper(pa_type):
```

### Comparing `dask-geopandas-0.3.0/dask_geopandas/io/file.py` & `dask-geopandas-0.3.1/dask_geopandas/io/file.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/io/parquet.py` & `dask-geopandas-0.3.1/dask_geopandas/io/parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import geopandas
 
 import dask.dataframe as dd
 
 from .arrow import (
     DASK_2022_12_0_PLUS,
+    DASK_2023_04_0,
     GeoDatasetEngine,
     _get_partition_bounds,
     _update_meta_to_geodataframe,
 )
 
 try:
     # pyarrow is imported here, but is an optional dependency
@@ -83,15 +84,15 @@
         )
         meta = cls._update_meta(meta, schema)
         return meta, index_cols, categories, index, partition_info
 
     @classmethod
     def _create_dd_meta(cls, dataset_info, use_nullable_dtypes=False):
         """Overriding private method for dask >= 2021.10.0"""
-        if DASK_2022_12_0_PLUS:
+        if DASK_2022_12_0_PLUS and not DASK_2023_04_0:
             meta = super()._create_dd_meta(dataset_info, use_nullable_dtypes)
         else:
             meta = super()._create_dd_meta(dataset_info)
 
         schema = dataset_info["schema"]
         if not schema.names and not schema.metadata:
             if len(list(dataset_info["ds"].get_fragments())) == 0:
```

### Comparing `dask-geopandas-0.3.0/dask_geopandas/morton_distance.py` & `dask-geopandas-0.3.1/dask_geopandas/morton_distance.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/sjoin.py` & `dask-geopandas-0.3.1/dask_geopandas/sjoin.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/io/conftest.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/io/test_arrow.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/io/test_arrow.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/io/test_file.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/io/test_file.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/io/test_parquet.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/test_clip.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/test_core.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pickle
 from packaging.version import Version
 import pytest
 import pandas as pd
 import numpy as np
 import geopandas
 from shapely.geometry import Polygon, Point, LineString, MultiPoint
 import dask
@@ -10,14 +11,15 @@
 import dask_geopandas
 
 from pandas.testing import assert_frame_equal, assert_series_equal
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 from dask_geopandas.hilbert_distance import _hilbert_distance
 from dask_geopandas.morton_distance import _morton_distance
 from dask_geopandas.geohash import _geohash
+from dask_geopandas.core import PANDAS_2_0_0
 
 
 @pytest.fixture
 def geoseries_polygons():
     t1 = Polygon([(0, 3.5), (7, 2.4), (1, 0.1)])
     t2 = Polygon([(0, 0), (1, 1), (0, 1)])
     sq1 = Polygon([(0, 0), (1, 0), (1, 1), (0, 1)])
@@ -441,14 +443,27 @@
         dask_obj.spatial_partitions = geodf_points
 
     # wrong length
     with pytest.raises(ValueError):
         dask_obj.spatial_partitions = geodf_points.geometry
 
 
+@pytest.mark.parametrize("calculate_spatial_partitions", [True, False])
+def test_spatial_partitions_pickle(geodf_points, calculate_spatial_partitions):
+    dask_obj = dask_geopandas.from_geopandas(geodf_points, npartitions=2)
+    if calculate_spatial_partitions:
+        dask_obj.calculate_spatial_partitions()
+
+    dask_obj2 = pickle.loads(pickle.dumps(dask_obj))
+    assert hasattr(dask_obj2, "spatial_partitions")
+
+    dask_series = pickle.loads(pickle.dumps(dask_obj.geometry))
+    assert hasattr(dask_series, "spatial_partitions")
+
+
 def test_to_crs_geodf(geodf_points_crs):
     df = geodf_points_crs
     dask_obj = dask_geopandas.from_geopandas(df, npartitions=2)
 
     new_crs = "epsg:4316"
     new = dask_obj.to_crs(new_crs)
     assert new.crs == new_crs
@@ -622,17 +637,19 @@
         dd_default = self.ddf.dissolve("continent").compute()
         assert_geodataframe_equal(gpd_default, dd_default, check_like=True)
 
     def test_sum(self):
         gpd_sum = self.world.dissolve("continent", aggfunc="sum")
         dd_sum = self.ddf.dissolve("continent", aggfunc="sum").compute()
         # drop due to https://github.com/geopandas/geopandas/issues/1999
-        assert_geodataframe_equal(
-            gpd_sum, dd_sum.drop(columns=["name", "iso_a3"]), check_like=True
-        )
+        if not PANDAS_2_0_0:
+            drop = ["name", "iso_a3"]
+        else:
+            drop = []
+        assert_geodataframe_equal(gpd_sum, dd_sum.drop(columns=drop), check_like=True)
 
     @pytest.mark.skipif(
         Version(dask.__version__) == Version("2022.01.1"),
         reason="Regression in dask 2022.01.1 https://github.com/dask/dask/issues/8611",
     )
     def test_split_out(self):
         gpd_default = self.world.dissolve("continent")
```

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/test_geohash.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/test_geohash.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/test_hilbert_distance.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/test_hilbert_distance.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/test_morton_distance.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/test_morton_distance.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/test_sjoin.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/test_sjoin.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas/tests/test_spatial_partitioning.py` & `dask-geopandas-0.3.1/dask_geopandas/tests/test_spatial_partitioning.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/dask_geopandas.egg-info/PKG-INFO` & `dask-geopandas-0.3.1/dask_geopandas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-geopandas
-Version: 0.3.0
+Version: 0.3.1
 Summary: Parallel GeoPandas with Dask
 Home-page: https://github.com/geopandas/dask-geopandas
 Maintainer: Julia Signell
 Maintainer-email: jsignell@gmail.com
 License: BSD
 Project-URL: Documentation, https://github.com/geopandas/dask-geopandas
 Project-URL: Source, https://github.com/geopandas/dask-geopandas/
```

### Comparing `dask-geopandas-0.3.0/dask_geopandas.egg-info/SOURCES.txt` & `dask-geopandas-0.3.1/dask_geopandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/setup.py` & `dask-geopandas-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `dask-geopandas-0.3.0/versioneer.py` & `dask-geopandas-0.3.1/versioneer.py`

 * *Files identical despite different names*

