# Comparing `tmp/curvit-1.6.3.tar.gz` & `tmp/curvit-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvit-1.6.3.tar", last modified: Sun Mar 26 08:18:06 2023, max compression
+gzip compressed data, was "curvit-1.6.4.tar", last modified: Fri Apr 28 06:18:26 2023, max compression
```

## Comparing `curvit-1.6.3.tar` & `curvit-1.6.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-03-26 08:18:06.901288 curvit-1.6.3/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.3/LICENSE
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-03-26 08:18:06.901288 curvit-1.6.3/PKG-INFO
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.3/README.md
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-03-26 08:18:06.899288 curvit-1.6.3/curvit/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      133 2023-03-19 15:24:32.000000 curvit-1.6.3/curvit/__init__.py
--rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.3/curvit/check_curvit_variability_V.0.4.py
--rwxrwxr-x   0 prajwel   (1000) prajwel   (1000)    79650 2023-03-26 08:09:38.000000 curvit-1.6.3/curvit/curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      355 2021-06-25 20:52:41.000000 curvit-1.6.3/curvit/profile_curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1003 2022-12-10 20:44:29.000000 curvit-1.6.3/curvit/test_curvit.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-03-26 08:18:06.900288 curvit-1.6.3/curvit.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-03-26 08:18:06.000000 curvit-1.6.3/curvit.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-03-26 08:18:06.000000 curvit-1.6.3/curvit.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-03-26 08:18:06.000000 curvit-1.6.3/curvit.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       63 2023-03-26 08:18:06.000000 curvit-1.6.3/curvit.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-03-26 08:18:06.000000 curvit-1.6.3/curvit.egg-info/top_level.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-03-26 08:18:06.901288 curvit-1.6.3/setup.cfg
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      894 2023-03-26 08:11:27.000000 curvit-1.6.3/setup.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 06:18:26.017010 curvit-1.6.4/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.4/LICENSE
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-04-28 06:18:26.017010 curvit-1.6.4/PKG-INFO
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.4/README.md
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 06:18:26.015010 curvit-1.6.4/curvit/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      133 2023-03-19 15:24:32.000000 curvit-1.6.4/curvit/__init__.py
+-rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.4/curvit/check_curvit_variability_V.0.4.py
+-rwxrwxr-x   0 prajwel   (1000) prajwel   (1000)    79824 2023-04-28 06:10:59.000000 curvit-1.6.4/curvit/curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      355 2021-06-25 20:52:41.000000 curvit-1.6.4/curvit/profile_curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1003 2022-12-10 20:44:29.000000 curvit-1.6.4/curvit/test_curvit.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 06:18:26.016010 curvit-1.6.4/curvit.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       63 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/top_level.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-28 06:18:26.017010 curvit-1.6.4/setup.cfg
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      894 2023-04-28 06:11:41.000000 curvit-1.6.4/setup.py
```

### Comparing `curvit-1.6.3/LICENSE` & `curvit-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `curvit-1.6.3/PKG-INFO` & `curvit-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.3
+Version: 1.6.4
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.3 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.6.4 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.3/README.md` & `curvit-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `curvit-1.6.3/curvit/check_curvit_variability_V.0.4.py` & `curvit-1.6.4/curvit/check_curvit_variability_V.0.4.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.3/curvit/curvit.py` & `curvit-1.6.4/curvit/curvit.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,17 @@
 from scipy.ndimage import zoom
 from scipy.spatial import KDTree
 from scipy.interpolate import interp1d
 from scipy.stats import median_abs_deviation
 from matplotlib.colors import LogNorm
 from photutils.detection import DAOStarFinder
 from photutils.aperture import CircularAperture
-from photutils.background import Background2D, MedianBackground
 from astropy.io import fits
 from astropy.convolution import Gaussian2DKernel, convolve
-from astropy.stats import sigma_clipped_stats, gaussian_fwhm_to_sigma, sigma_clip, SigmaClip
+from astropy.stats import sigma_clipped_stats, gaussian_fwhm_to_sigma, sigma_clip
  
 #######################################################################
 # Initial set of parameters.
 
 '''Window size Vs Framecount rate dictionary (approximate). 
 The most accurate way to get the rate would be to take the value 
 of (1 / INT_TIME). INT_TIME value can be found from the image header
@@ -131,14 +130,17 @@
 
 # Astroalign defaults. 
 NUM_NEAREST_NEIGHBORS = 8
 MIN_MATCHES_FRACTION = 0.01
 
 # For Astrometry.
 AstrometryNet_API_key = 'ujmrvwqqyelxmzcj'  
+
+# For curve_orbitwise
+time_separation = 30 * 60 #seconds
 #######################################################################
 
 
 def weighted_centre(x_coords = None, 
                     y_coords = None, 
                     weights = None, 
                     bins = 600):
@@ -1068,14 +1070,15 @@
     plt.close('all') 
  
     
 def curve_orbitwise(events_list = events_list,
                     xp = xp,
                     yp = yp,
                     radius = radius,
+                    time_separation = time_separation,
                     framecount_per_sec = framecount_per_sec,
                     background = background,
                     sky_radius = sky_radius,
                     x_bg = x_bg,
                     y_bg = y_bg,
                     aperture_correction = aperture_correction,
                     saturation_correction = saturation_correction,
@@ -1097,15 +1100,19 @@
         The X-coordinate of the source.
         
     yp : float
         The Y-coordinate of the source. 
         
     radius : float, optional
         The source aperture radius in pixels. 
-        This parameter has a default value of 6.        
+        This parameter has a default value of 6.
+        
+    time_separation : float, optional
+        The time separation in seconds. 
+        This parameter has a default value of 30 * 60 seconds.
         
     framecount_per_sec : float, optional
         The framerate of the observation, with a default value of 28.7185
         frames per second for 512 x 512 window mode. 
         The most accurate way to get the framerate would be to take the value 
         of (``1 / INT_TIME``). 
         ``INT_TIME`` value can be found from the corresponding image header. 
@@ -1265,22 +1272,19 @@
             print('Region selected for background estimate:\n* {}'.format(bg_png))
     else:
         bg_CPS, bg_CPS_e = 0, 0 
 
     unique_time = np.unique(time)
     unique_time = np.sort(unique_time)
 
-    # Define threshold for time differences (in seconds)
-    orbit_time_difference = 30 * 60 
-
     # Calculate differences between consecutive elements
     diffs = np.diff(unique_time)
 
     # Find indices where differences exceed threshold
-    boundaries = np.where(diffs > orbit_time_difference)[0] + 1
+    boundaries = np.where(diffs > time_separation)[0] + 1
     
     starts = np.concatenate([[0], boundaries])
     ends = np.concatenate([boundaries - 1, [len(unique_time) -1]])
     
     starts = unique_time[starts]
     ends = unique_time[ends]
     
@@ -1370,15 +1374,15 @@
     np.savetxt(datname, data_to_output,
                fmt = '%10.11f\t%.5e\t%.5e',
                header = 'MJD\t\t\tCPS\tCPS_error')
 
     figname = os.path.join(path_to_events_list, output_prefix + '.png')
     plt.savefig(figname, format = 'png', bbox_inches = 'tight', dpi = 150)
 
-    print('\n-------------------------- curve --------------------------')
+    print('\n-------------------------- curve_orbitwise --------------------------')
     print('source: {}\n        {}'.format(png_name, source_png))
     print('data: {}'.format(datname))
     print('plot: {}'.format(figname))
 
     print("\nDone!\n")
     plt.close('all') 
               
@@ -1588,31 +1592,29 @@
 
 
 def daofind_on_image_data(data, threshold):
     kernel = Gaussian2DKernel(x_stddev=1.5)
     binned_data = rebin(data, 2)
     smoothed_data = convolve(binned_data, kernel)
     zoomed_data = zoom(smoothed_data, zoom = 2, order = 0)
-    
-    sigma_clip = SigmaClip(sigma=3.)
-    bkg_estimator = MedianBackground()
-    bkg = Background2D(zoomed_data, (50, 50), filter_size=(3, 3),
-                       sigma_clip=sigma_clip, bkg_estimator=bkg_estimator)
-
-    daofind = DAOStarFinder(fwhm = 4, 
-                            threshold = threshold * bkg.background_rms_median, 
+    for_bkg_binned_data = rebin(zoomed_data, 64)
+    for_bkg_binned_data[for_bkg_binned_data <= 0] = np.nan
+    bkg_median = np.nanmedian(for_bkg_binned_data)
+    bkg_MAD = median_abs_deviation(for_bkg_binned_data, axis = None,
+                                            nan_policy = 'omit')
+                                          
+    daofind = DAOStarFinder(fwhm = 6,
+                            threshold = threshold * bkg_MAD, 
                             exclude_border = True)
     
-    sources = daofind(zoomed_data - bkg.background)    
-    
+    sources = daofind(zoomed_data - bkg_median)    
     sources.sort('mag')
     uA = np.array([sources['xcentroid'].data, sources['ycentroid'].data]).T
     return uA 
 
-
 def new_detect_sources_daofind(fx, fy, photons, threshold, framecount_per_sec):
     data = get_image_data(fx, fy, photons, framecount_per_sec)
     uA = daofind_on_image_data(data, threshold)
     return uA
 
 
 def combine_events_lists(events_lists_paths = None,
```

### Comparing `curvit-1.6.3/curvit/test_curvit.py` & `curvit-1.6.4/curvit/test_curvit.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.3/curvit.egg-info/PKG-INFO` & `curvit-1.6.4/curvit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.3
+Version: 1.6.4
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.3 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.6.4 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.3/setup.py` & `curvit-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="curvit", 
-    version="1.6.3",
+    version="1.6.4",
     author="Prajwel Joseph",
     author_email="prajwel.joseph@gmail.com",
     description="light curves from UVIT data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prajwel/curvit",
     packages=setuptools.find_packages(),
```

