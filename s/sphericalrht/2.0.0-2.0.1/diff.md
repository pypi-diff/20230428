# Comparing `tmp/sphericalrht-2.0.0.tar.gz` & `tmp/sphericalrht-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/users/georgech/sphericalrht/dist/.tmp-fl9m5toc/sphericalrht-2.0.0.tar", last modified: Fri Apr 28 01:32:07 2023, max compression
+gzip compressed data, was "/home/users/georgech/sphericalrht/dist/.tmp-re9c0i6x/sphericalrht-2.0.1.tar", last modified: Fri Apr 28 19:54:55 2023, max compression
```

## Comparing `sphericalrht-2.0.0.tar` & `sphericalrht-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.847927 sphericalrht-2.0.0/
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.566987 sphericalrht-2.0.0/.github/
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.672497 sphericalrht-2.0.0/.github/workflows/
--rw-r--r--   0 georgech (355130) seclark1 (377337)      969 2021-11-09 19:57:02.000000 sphericalrht-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0 georgech (355130) seclark1 (377337)     1056 2021-11-04 19:06:51.000000 sphericalrht-2.0.0/LICENSE
--rw-r--r--   0 georgech (355130) seclark1 (377337)      196 2021-11-09 22:55:35.000000 sphericalrht-2.0.0/MANIFEST.in
--rw-r--r--   0 georgech (355130) seclark1 (377337)     2923 2023-04-28 01:32:07.849035 sphericalrht-2.0.0/PKG-INFO
--rw-r--r--   0 georgech (355130) seclark1 (377337)     2100 2021-11-12 01:13:46.000000 sphericalrht-2.0.0/README.md
--rw-r--r--   0 georgech (355130) seclark1 (377337)     7108 2023-04-28 01:05:27.000000 sphericalrht-2.0.0/README.rst
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.735565 sphericalrht-2.0.0/docs/
--rw-r--r--   0 georgech (355130) seclark1 (377337)      638 2021-11-08 16:39:26.000000 sphericalrht-2.0.0/docs/Makefile
--rw-r--r--   0 georgech (355130) seclark1 (377337)      834 2021-11-08 16:39:52.000000 sphericalrht-2.0.0/docs/make.bat
--rw-r--r--   0 georgech (355130) seclark1 (377337)      538 2022-03-04 19:57:24.000000 sphericalrht-2.0.0/pyproject.toml
--rw-r--r--   0 georgech (355130) seclark1 (377337)       69 2021-11-05 18:58:31.000000 sphericalrht-2.0.0/requirements.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)      110 2021-11-09 05:49:42.000000 sphericalrht-2.0.0/requirements_dev.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)     1164 2023-04-28 01:32:07.853917 sphericalrht-2.0.0/setup.cfg
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.572491 sphericalrht-2.0.0/src/
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.771396 sphericalrht-2.0.0/src/sphericalrht/
--rw-r--r--   0 georgech (355130) seclark1 (377337)      891 2023-04-28 01:24:05.000000 sphericalrht-2.0.0/src/sphericalrht/__init__.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-04 20:48:45.000000 sphericalrht-2.0.0/src/sphericalrht/py.typed
--rw-r--r--   0 georgech (355130) seclark1 (377337)    20597 2023-04-28 01:26:53.000000 sphericalrht-2.0.0/src/sphericalrht/spherical_rht.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)      900 2023-04-28 01:24:47.000000 sphericalrht-2.0.0/src/sphericalrht/utils.py
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.797264 sphericalrht-2.0.0/src/sphericalrht.egg-info/
--rw-r--r--   0 georgech (355130) seclark1 (377337)     2923 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/PKG-INFO
--rw-r--r--   0 georgech (355130) seclark1 (377337)      636 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/SOURCES.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)        1 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/dependency_links.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)      132 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/requires.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)       13 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/top_level.txt
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.818540 sphericalrht-2.0.0/tests/
--rw-r--r--   0 georgech (355130) seclark1 (377337)       86 2023-04-28 01:25:10.000000 sphericalrht-2.0.0/tests/__init__.py
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.840874 sphericalrht-2.0.0/tests/data/
--rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-11 23:22:43.000000 sphericalrht-2.0.0/tests/data/__init__.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)     8640 2021-11-11 23:12:34.000000 sphericalrht-2.0.0/tests/data/test_map.fits
--rw-r--r--   0 georgech (355130) seclark1 (377337)     8640 2023-04-28 01:22:20.000000 sphericalrht-2.0.0/tests/data/test_map2.fits
--rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-07 01:49:54.000000 sphericalrht-2.0.0/tests/py.typed
--rw-r--r--   0 georgech (355130) seclark1 (377337)     6185 2023-04-28 01:03:00.000000 sphericalrht-2.0.0/tests/test_spherical_rht.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)      754 2021-11-12 01:46:19.000000 sphericalrht-2.0.0/tests/test_utils.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)      486 2021-11-09 19:56:12.000000 sphericalrht-2.0.0/tox.ini
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.903657 sphericalrht-2.0.1/
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.677882 sphericalrht-2.0.1/.github/
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.766611 sphericalrht-2.0.1/.github/workflows/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      969 2021-11-09 19:57:02.000000 sphericalrht-2.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     1056 2021-11-04 19:06:51.000000 sphericalrht-2.0.1/LICENSE
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      196 2021-11-09 22:55:35.000000 sphericalrht-2.0.1/MANIFEST.in
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     2923 2023-04-28 19:54:55.905202 sphericalrht-2.0.1/PKG-INFO
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     2100 2021-11-12 01:13:46.000000 sphericalrht-2.0.1/README.md
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     7108 2023-04-28 01:49:44.000000 sphericalrht-2.0.1/README.rst
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.782141 sphericalrht-2.0.1/docs/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      638 2021-11-08 16:39:26.000000 sphericalrht-2.0.1/docs/Makefile
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      834 2021-11-08 16:39:52.000000 sphericalrht-2.0.1/docs/make.bat
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      538 2022-03-04 19:57:24.000000 sphericalrht-2.0.1/pyproject.toml
+-rw-r--r--   0 georgech (355130) seclark1 (377337)       69 2021-11-05 18:58:31.000000 sphericalrht-2.0.1/requirements.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      110 2021-11-09 05:49:42.000000 sphericalrht-2.0.1/requirements_dev.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     1164 2023-04-28 19:54:55.913041 sphericalrht-2.0.1/setup.cfg
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.687529 sphericalrht-2.0.1/src/
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.811543 sphericalrht-2.0.1/src/sphericalrht/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      891 2023-04-28 19:51:05.000000 sphericalrht-2.0.1/src/sphericalrht/__init__.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-04 20:48:45.000000 sphericalrht-2.0.1/src/sphericalrht/py.typed
+-rw-r--r--   0 georgech (355130) seclark1 (377337)    20850 2023-04-28 19:51:05.000000 sphericalrht-2.0.1/src/sphericalrht/spherical_rht.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      900 2023-04-28 19:51:05.000000 sphericalrht-2.0.1/src/sphericalrht/utils.py
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.843541 sphericalrht-2.0.1/src/sphericalrht.egg-info/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     2923 2023-04-28 19:54:55.000000 sphericalrht-2.0.1/src/sphericalrht.egg-info/PKG-INFO
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      636 2023-04-28 19:54:55.000000 sphericalrht-2.0.1/src/sphericalrht.egg-info/SOURCES.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)        1 2023-04-28 19:54:55.000000 sphericalrht-2.0.1/src/sphericalrht.egg-info/dependency_links.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      132 2023-04-28 19:54:55.000000 sphericalrht-2.0.1/src/sphericalrht.egg-info/requires.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)       13 2023-04-28 19:54:55.000000 sphericalrht-2.0.1/src/sphericalrht.egg-info/top_level.txt
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.870516 sphericalrht-2.0.1/tests/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)       86 2023-04-28 19:51:05.000000 sphericalrht-2.0.1/tests/__init__.py
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 19:54:55.896349 sphericalrht-2.0.1/tests/data/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-11 23:22:43.000000 sphericalrht-2.0.1/tests/data/__init__.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     8640 2021-11-11 23:12:34.000000 sphericalrht-2.0.1/tests/data/test_map.fits
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     8640 2023-04-28 01:22:20.000000 sphericalrht-2.0.1/tests/data/test_map2.fits
+-rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-07 01:49:54.000000 sphericalrht-2.0.1/tests/py.typed
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     6183 2023-04-28 01:57:36.000000 sphericalrht-2.0.1/tests/test_spherical_rht.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      754 2021-11-12 01:46:19.000000 sphericalrht-2.0.1/tests/test_utils.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      486 2021-11-09 19:56:12.000000 sphericalrht-2.0.1/tox.ini
```

### Comparing `sphericalrht-2.0.0/.github/workflows/tests.yml` & `sphericalrht-2.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/LICENSE` & `sphericalrht-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/PKG-INFO` & `sphericalrht-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphericalrht
-Version: 2.0.0
+Version: 2.0.1
 Summary: Spherical implementation of the Rolling Hough Transform
 Home-page: https://github.com/georgehalal/sphericalrht
 Author: George Halal
 Author-email: halalgeorge@gmail.com
 Project-URL: Bug Tracker, https://github.com/georgehalal/sphericalrht/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sphericalrht Version: 2.0.0 Summary: Spherical
+Metadata-Version: 2.1 Name: sphericalrht Version: 2.0.1 Summary: Spherical
 implementation of the Rolling Hough Transform Home-page: https://github.com/
 georgehalal/sphericalrht Author: George Halal Author-email:
 halalgeorge@gmail.com Project-URL: Bug Tracker, https://github.com/georgehalal/
 sphericalrht/issues Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `sphericalrht-2.0.0/README.md` & `sphericalrht-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/README.rst` & `sphericalrht-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/docs/Makefile` & `sphericalrht-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/docs/make.bat` & `sphericalrht-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/pyproject.toml` & `sphericalrht-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/setup.cfg` & `sphericalrht-2.0.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sphericalrht
-version = 2.0.0
+version = 2.0.1
 author = George Halal
 author_email = halalgeorge@gmail.com
 description = Spherical implementation of the Rolling Hough Transform
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/georgehalal/sphericalrht
 project_urls =
```

### Comparing `sphericalrht-2.0.0/src/sphericalrht/__init__.py` & `sphericalrht-2.0.1/src/sphericalrht/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
 from .spherical_rht import StokesQU, CubeAndStokes
 from .utils import set_logger
 
 
 __author__ = "George Halal"
 __email__ = "halalgeorge@gmail.com"
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __all__ = ["StokesQU", "CubeAndStokes", "set_logger"]
```

### Comparing `sphericalrht-2.0.0/src/sphericalrht/spherical_rht.py` & `sphericalrht-2.0.1/src/sphericalrht/spherical_rht.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     CubeAndStokes: Define an instance of this class with input
         parameters, then use the build_and_save method to run
         the algorthm.
 
 Author: George Halal
 Email: halalgeorge@gmail.com
 Date: 04/27/2023
-Version: 2.0.0
+Version: 2.0.1
 """
 
 
 __author__ = "George Halal"
 __email__ = "halalgeorge@gmail.com"
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __all__ = ["StokesQU", "CubeAndStokes"]
 
 
 import os
 import time
 from collections import deque
 import logging
@@ -157,15 +157,15 @@
                 Higher thresholds focus on the main orientations only,
                 while lower thresholds take more orientations into
                 account, weighted by their intensity.
             norients (int): angular resolution given by the number of
                 orientations to consider.
             mask (str or np.ndarray((Npix,))): either a path to the map
                 or an array of the map pixels. This defines the mask for
-                maps that are not defined over the entire sky. 
+                maps that are not defined over the entire sky.
             weighting (str or np.ndarray((Npix,))): either a path to the
                 map or an array of the map pixels. This is used as the
                 weight for the output Stokes Q/U maps. The map ordering
                 is assumed to be RING.
             overwrite (bool): whether to overwrite outputs of same name
                 if they already exist.
             split_factor (int): number of convolution splits to save on
@@ -223,14 +223,18 @@
         self.thresh = thresh
 
         assert norients % 1 == 0 and norients > 0, (
             "Number of orientations must be a positive integer")
         self.norients = int(norients)
 
         if weighting is not None:
+            # needed since self.weighting is not declared otherwise and
+            # needs to be replaced with self.in_map AFTER self.in_map
+            # has been proccessed.
+            self.weighting_flag = True
             assert isinstance(weighting, str) or (
                 isinstance(weighting, np.ndarray)), (
                 "Weighting map must be a path or an np.ndarray")
             if isinstance(weighting, str):
                 assert os.path.exists(weighting), (
                     "Weighting map does not exist. Check path and try again.")
                 if isinstance(in_map, str) and weighting == in_map:
@@ -239,14 +243,16 @@
                     self.weighting = hp.read_map(weighting, field=(0))
             else:
                 assert np.sqrt(weighting.shape[0]/12) % 1 == 0, (
                     "Weighting map has the wrong shape or number of pixels.")
                 self.weighting = weighting
             if hp.get_nside(self.weighting) != self.nside:
                 self.weighting = hp.ud_grade(self.weighting, self.nside)
+        else:
+            self.weighting_flag = False
 
         self.overwrite = overwrite
 
         if split_factor is not None:
             assert split_factor % 1 == 0 and split_factor > 0, (
                 "Split factor must be a positive integer")
             self.split_factor = int(split_factor)
@@ -281,15 +287,15 @@
         Returns:
             high-pass filtered map of 1s and 0s (np.ndarray)
         """
         original_map[original_map != original_map] = 0
 
         smoothed_map = hp.smoothing(
             original_map * self.mask, fwhm=np.radians(self.fwhm / 60.))
-        
+
         subtracted_map = original_map*self.mask - smoothed_map
 
         return (subtracted_map > 0.).astype(int)
 
     def prep_intensity(self, return_alm: bool = False) -> Union[
             np.ndarray, None]:
         """Process the intensity map for saving with the Stokes Q/U
@@ -394,15 +400,15 @@
         psis = np.repeat(orients, phis.shape[0])
         phis = np.tile(phis, orients.shape[0])
         thetas = np.tile(thetas, orients.shape[0])
 
         return np.vstack((thetas, phis, psis)).T
 
     def save_cube_and_stokes(
-            self, 
+            self,
             interpolator: ducc0.totalconvolve.Interpolator) -> None:
         """Run the convolution and save the resulting cube and maps.
 
         Parameters:
             interpolator (ducc0.totalconvolve.Interpolator): object
                 encapsulating the convolution functionality
         """
@@ -447,15 +453,15 @@
             norm += spherical_rht_temp.sum(axis=0)
             process = psutil.Process(os.getpid())
             logging.info(f"* Using {process.memory_info().rss / 1e9}GB of"
                          " memory to make spherical RHT cube.")
 
         f.close()
 
-        if self.weighting is not None:
+        if self.weighting_flag:
             stokes.normalize_and_weight(norm, self.weighting)
         else:
             stokes.normalize_and_weight(norm, self.in_map)
 
         hp.write_map(os.path.join(self.out_dir, "IQU_" + self.out_name
                      + ".fits"), (self.in_map, stokes.stokes_q,
                      stokes.stokes_u), dtype=["float32", "float32", "float32"],
```

### Comparing `sphericalrht-2.0.0/src/sphericalrht/utils.py` & `sphericalrht-2.0.1/src/sphericalrht/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 import logging
 
 
 __author__ = "George Halal"
 __email__ = "halalgeorge@gmail.com"
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __all__ = ["set_logger"]
 
 
 def set_logger(log_path: str) -> None:
     """Log output in the terminal to a file.
 
     Args:
```

### Comparing `sphericalrht-2.0.0/src/sphericalrht.egg-info/PKG-INFO` & `sphericalrht-2.0.1/src/sphericalrht.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphericalrht
-Version: 2.0.0
+Version: 2.0.1
 Summary: Spherical implementation of the Rolling Hough Transform
 Home-page: https://github.com/georgehalal/sphericalrht
 Author: George Halal
 Author-email: halalgeorge@gmail.com
 Project-URL: Bug Tracker, https://github.com/georgehalal/sphericalrht/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sphericalrht Version: 2.0.0 Summary: Spherical
+Metadata-Version: 2.1 Name: sphericalrht Version: 2.0.1 Summary: Spherical
 implementation of the Rolling Hough Transform Home-page: https://github.com/
 georgehalal/sphericalrht Author: George Halal Author-email:
 halalgeorge@gmail.com Project-URL: Bug Tracker, https://github.com/georgehalal/
 sphericalrht/issues Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `sphericalrht-2.0.0/src/sphericalrht.egg-info/SOURCES.txt` & `sphericalrht-2.0.1/src/sphericalrht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/tests/data/test_map.fits` & `sphericalrht-2.0.1/tests/data/test_map.fits`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/tests/data/test_map2.fits` & `sphericalrht-2.0.1/tests/data/test_map2.fits`

 * *Files identical despite different names*

### Comparing `sphericalrht-2.0.0/tests/test_spherical_rht.py` & `sphericalrht-2.0.1/tests/test_spherical_rht.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 from sphericalrht import StokesQU, CubeAndStokes
 
 
 NSIDE = 2
 NPIX = 12 * NSIDE**2
 NORIENTS = 6
-TEST_MAP_PATH = os.path.abspath("tests/data/test_map.fits") 
-TEST_MAP2_PATH = os.path.abspath("tests/data/test_map2.fits") 
+TEST_MAP_PATH = os.path.abspath("tests/data/test_map.fits")
+TEST_MAP2_PATH = os.path.abspath("tests/data/test_map2.fits")
 OUT_DIR = os.path.abspath("tests/data/out")
 
 
 class TestStokesQU(unittest.TestCase):
     """Test of the StokesQU class."""
 
     def test_update(self):
```

### Comparing `sphericalrht-2.0.0/tests/test_utils.py` & `sphericalrht-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

