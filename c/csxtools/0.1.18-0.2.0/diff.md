# Comparing `tmp/csxtools-0.1.18.tar.gz` & `tmp/csxtools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csxtools-0.1.18.tar", last modified: Fri Jan 20 02:08:40 2023, max compression
+gzip compressed data, was "csxtools-0.2.0.tar", last modified: Fri Apr 28 20:24:03 2023, max compression
```

## Comparing `csxtools-0.1.18.tar` & `csxtools-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-01-20 02:08:40.755978 csxtools-0.1.18/
--rw-r--r--   0 mrakitin   (501) staff       (20)     1584 2022-12-09 23:03:36.000000 csxtools-0.1.18/LICENSE.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)      141 2023-01-20 02:03:03.000000 csxtools-0.1.18/MANIFEST.in
--rw-r--r--   0 mrakitin   (501) staff       (20)      275 2023-01-20 02:08:40.756176 csxtools-0.1.18/PKG-INFO
--rw-r--r--   0 mrakitin   (501) staff       (20)      614 2023-01-20 01:43:54.000000 csxtools-0.1.18/README.md
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-01-20 02:08:40.757556 csxtools-0.1.18/csxtools/
--rw-r--r--   0 mrakitin   (501) staff       (20)      290 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/__init__.py
--rw-r--r--   0 mrakitin   (501) staff       (20)      472 2023-01-20 02:08:40.757669 csxtools-0.1.18/csxtools/_version.py
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-01-20 02:08:40.744896 csxtools-0.1.18/csxtools/ext/
--rw-r--r--   0 mrakitin   (501) staff       (20)        0 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/ext/__init__.py
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-01-20 02:08:40.746431 csxtools-0.1.18/csxtools/fastccd/
--rw-r--r--   0 mrakitin   (501) staff       (20)      248 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/fastccd/__init__.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     1807 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/fastccd/images.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     1505 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/fastccd/phocount.py
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-01-20 02:08:40.747931 csxtools-0.1.18/csxtools/image/
--rw-r--r--   0 mrakitin   (501) staff       (20)      411 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/image/__init__.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     4728 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/image/stack.py
--rw-r--r--   0 mrakitin   (501) staff       (20)      834 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/image/transform.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     2642 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/image_corr.py
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-01-20 02:08:40.749999 csxtools-0.1.18/csxtools/ipynb/
--rw-r--r--   0 mrakitin   (501) staff       (20)      328 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/ipynb/__init__.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     3906 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/ipynb/animation.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     1033 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/ipynb/nbviewer.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     1215 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/plotting.py
--rw-r--r--   0 mrakitin   (501) staff       (20)      108 2022-12-09 23:03:36.000000 csxtools-0.1.18/csxtools/settings.py
--rw-r--r--   0 mrakitin   (501) staff       (20)    10393 2023-01-20 01:43:54.000000 csxtools-0.1.18/csxtools/utils.py
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-01-20 02:08:40.744425 csxtools-0.1.18/csxtools.egg-info/
--rw-r--r--   0 mrakitin   (501) staff       (20)      275 2023-01-20 02:08:40.000000 csxtools-0.1.18/csxtools.egg-info/PKG-INFO
--rw-r--r--   0 mrakitin   (501) staff       (20)      803 2023-01-20 02:08:40.000000 csxtools-0.1.18/csxtools.egg-info/SOURCES.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)        1 2023-01-20 02:08:40.000000 csxtools-0.1.18/csxtools.egg-info/dependency_links.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)       56 2023-01-20 02:08:40.000000 csxtools-0.1.18/csxtools.egg-info/requires.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)       32 2023-01-20 02:08:40.000000 csxtools-0.1.18/csxtools.egg-info/top_level.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)       38 2022-12-09 23:03:36.000000 csxtools-0.1.18/requirements-extras.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)        6 2022-12-09 23:03:36.000000 csxtools-0.1.18/requirements.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)      416 2023-01-20 02:08:40.757093 csxtools-0.1.18/setup.cfg
--rw-r--r--   0 mrakitin   (501) staff       (20)     1552 2022-12-09 23:03:36.000000 csxtools-0.1.18/setup.py
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-01-20 02:08:40.755345 csxtools-0.1.18/src/
--rw-r--r--   0 mrakitin   (501) staff       (20)     3830 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/fastccd.c
--rw-r--r--   0 mrakitin   (501) staff       (20)     2754 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/fastccd.h
--rw-r--r--   0 mrakitin   (501) staff       (20)     5536 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/fastccdmodule.c
--rw-r--r--   0 mrakitin   (501) staff       (20)     6612 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/image.c
--rw-r--r--   0 mrakitin   (501) staff       (20)     2668 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/image.h
--rw-r--r--   0 mrakitin   (501) staff       (20)     5872 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/imagemodule.c
--rw-r--r--   0 mrakitin   (501) staff       (20)     5665 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/phocount.c
--rw-r--r--   0 mrakitin   (501) staff       (20)     2700 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/phocount.h
--rw-r--r--   0 mrakitin   (501) staff       (20)     4915 2022-12-09 23:03:36.000000 csxtools-0.1.18/src/phocountmodule.c
--rw-r--r--   0 mrakitin   (501) staff       (20)    62436 2022-12-09 23:03:36.000000 csxtools-0.1.18/versioneer.py
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.605963 csxtools-0.2.0/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     1584 2023-02-02 19:25:12.000000 csxtools-0.2.0/LICENSE.txt
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      141 2023-02-02 19:25:12.000000 csxtools-0.2.0/MANIFEST.in
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      229 2023-04-28 20:24:03.605968 csxtools-0.2.0/PKG-INFO
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      614 2023-02-02 19:25:12.000000 csxtools-0.2.0/README.md
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.608966 csxtools-0.2.0/csxtools/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      290 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/__init__.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      471 2023-04-28 20:24:03.608971 csxtools-0.2.0/csxtools/_version.py
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.559967 csxtools-0.2.0/csxtools/ext/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)        0 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/ext/__init__.py
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.565970 csxtools-0.2.0/csxtools/fastccd/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      248 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/fastccd/__init__.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     1807 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/fastccd/images.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     1505 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/fastccd/phocount.py
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.572965 csxtools-0.2.0/csxtools/image/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      411 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/image/__init__.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     4728 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/image/stack.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      834 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/image/transform.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     2642 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/image_corr.py
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.579963 csxtools-0.2.0/csxtools/ipynb/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      328 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/ipynb/__init__.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     3906 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/ipynb/animation.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     1033 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/ipynb/nbviewer.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     1215 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/plotting.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      108 2023-02-02 19:25:12.000000 csxtools-0.2.0/csxtools/settings.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     9895 2023-04-28 20:21:32.000000 csxtools-0.2.0/csxtools/utils.py
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.557967 csxtools-0.2.0/csxtools.egg-info/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      229 2023-04-28 20:24:03.000000 csxtools-0.2.0/csxtools.egg-info/PKG-INFO
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      845 2023-04-28 20:24:03.000000 csxtools-0.2.0/csxtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)        1 2023-04-28 20:24:03.000000 csxtools-0.2.0/csxtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)       51 2023-04-28 20:24:03.000000 csxtools-0.2.0/csxtools.egg-info/requires.txt
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)       32 2023-04-28 20:24:03.000000 csxtools-0.2.0/csxtools.egg-info/top_level.txt
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)       33 2023-04-28 20:21:32.000000 csxtools-0.2.0/requirements-extras.txt
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)        6 2023-02-02 19:25:13.000000 csxtools-0.2.0/requirements.txt
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)      416 2023-04-28 20:24:03.607971 csxtools-0.2.0/setup.cfg
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     1552 2023-02-02 19:25:13.000000 csxtools-0.2.0/setup.py
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.598962 csxtools-0.2.0/src/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     3830 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/fastccd.c
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     2754 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/fastccd.h
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     5536 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/fastccdmodule.c
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     6612 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/image.c
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     2668 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/image.h
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     5872 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/imagemodule.c
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     5665 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/phocount.c
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     2700 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/phocount.h
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     4915 2023-02-02 19:25:13.000000 csxtools-0.2.0/src/phocountmodule.c
+drwxrwxr-x   0 dallan    (2285) dallan    (2285)        0 2023-04-28 20:24:03.603963 csxtools-0.2.0/tests/
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     1395 2023-02-02 19:25:13.000000 csxtools-0.2.0/tests/test_fastccd.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)     3308 2023-02-02 19:25:13.000000 csxtools-0.2.0/tests/test_image.py
+-rw-rw-r--   0 dallan    (2285) dallan    (2285)    62436 2023-02-02 19:25:13.000000 csxtools-0.2.0/versioneer.py
```

### Comparing `csxtools-0.1.18/LICENSE.txt` & `csxtools-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/README.md` & `csxtools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/fastccd/images.py` & `csxtools-0.2.0/csxtools/fastccd/images.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/fastccd/phocount.py` & `csxtools-0.2.0/csxtools/fastccd/phocount.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/image/stack.py` & `csxtools-0.2.0/csxtools/image/stack.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/image/transform.py` & `csxtools-0.2.0/csxtools/image/transform.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/image_corr.py` & `csxtools-0.2.0/csxtools/image_corr.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/ipynb/animation.py` & `csxtools-0.2.0/csxtools/ipynb/animation.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/ipynb/nbviewer.py` & `csxtools-0.2.0/csxtools/ipynb/nbviewer.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/plotting.py` & `csxtools-0.2.0/csxtools/plotting.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/csxtools/utils.py` & `csxtools-0.2.0/csxtools/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import time as ttime
-from pims import pipeline
 
 from .fastccd import correct_images
 from .image import rotate90, stackmean
 from .settings import detectors
 from databroker.assets.handlers import AreaDetectorHDF5TimestampHandler
 
 import logging
@@ -49,15 +48,15 @@
 
     roi : tuple
         coordinates of the upper-left corner and width and height of
         the ROI: e.g., (x, y, w, h)
 
     Returns
     -------
-        A corrected pims.pipeline of the data
+    dask.array : corrected images
 
     """
 
     if tag is None:
         tag = detectors['fccd']
 
     # Now lets sort out the ROI
@@ -87,15 +86,15 @@
                 bgnd_events = _get_images(d, tag, roi)
 
                 # We assume that all images are for the background
                 # TODO : Perhaps we can loop over the generator
                 # If we want to do something lazy
 
                 tt = ttime.time()
-                b = get_images_to_3D(bgnd_events, dtype=np.uint16)
+                b = bgnd_events.astype(dtype=np.uint16)
                 logger.info("Image conversion took %.3f seconds",
                             ttime.time() - tt)
 
                 b = correct_images(b, gain=(1, 1, 1))
                 tt = ttime.time()
                 b = stackmean(b)
                 logger.info("Mean of image stack took %.3f seconds",
@@ -173,42 +172,27 @@
 
     """
     im = np.vstack([np.asarray(im, dtype=dtype) for im in images])
     return im
 
 
 def _get_images(header, tag, roi=None):
-    t = ttime.time()
-    if isinstance(header, (list, tuple)):
-        # assumes all headers are coming from the same db
-        db = header[0].db
-        for h in header:
-            if h.db is not db:
-                raise ValueError("All headers need to come from the same "
-                                 "Broker instance.")
-        images = db.get_images(header, tag)
-    else:
-        images = header.db.get_images(header, tag)
-    t = ttime.time() - t
-    logger.info("Took %.3f seconds to read data using get_images", t)
-
+    run = header.v2.new_variation(structure_clients="dask")
+    images = run["primary"]["data"][tag][:]
     if roi is not None:
         images = _crop_images(images, roi)
-
     return images
 
 
-@pipeline
 def _correct_fccd_images(image, bgnd, flat, gain):
     image = correct_images(image, bgnd, flat, gain)
     image = rotate90(image, 'cw')
     return image
 
 
-@pipeline
 def _crop_images(image, roi):
     return _crop(image, roi)
 
 
 def _crop(image, roi):
     image_shape = image.shape
     # Assuming ROI is specified in the "rotated" (correct) orientation
```

### Comparing `csxtools-0.1.18/csxtools.egg-info/SOURCES.txt` & `csxtools-0.2.0/csxtools.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 src/fastccd.h
 src/fastccdmodule.c
 src/image.c
 src/image.h
 src/imagemodule.c
 src/phocount.c
 src/phocount.h
-src/phocountmodule.c
+src/phocountmodule.c
+tests/test_fastccd.py
+tests/test_image.py
```

### Comparing `csxtools-0.1.18/setup.py` & `csxtools-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/fastccd.c` & `csxtools-0.2.0/src/fastccd.c`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/fastccd.h` & `csxtools-0.2.0/src/fastccd.h`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/fastccdmodule.c` & `csxtools-0.2.0/src/fastccdmodule.c`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/image.c` & `csxtools-0.2.0/src/image.c`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/image.h` & `csxtools-0.2.0/src/image.h`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/imagemodule.c` & `csxtools-0.2.0/src/imagemodule.c`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/phocount.c` & `csxtools-0.2.0/src/phocount.c`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/phocount.h` & `csxtools-0.2.0/src/phocount.h`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/src/phocountmodule.c` & `csxtools-0.2.0/src/phocountmodule.c`

 * *Files identical despite different names*

### Comparing `csxtools-0.1.18/versioneer.py` & `csxtools-0.2.0/versioneer.py`

 * *Files identical despite different names*

