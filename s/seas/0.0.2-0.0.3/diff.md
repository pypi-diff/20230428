# Comparing `tmp/seas-0.0.2.tar.gz` & `tmp/seas-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seas-0.0.2.tar", last modified: Mon May 31 20:46:01 2021, max compression
+gzip compressed data, was "seas-0.0.3.tar", last modified: Tue Apr 18 00:14:42 2023, max compression
```

## Comparing `seas-0.0.2.tar` & `seas-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-31 20:46:01.271384 seas-0.0.2/
--rwxrwxrwx   0 root         (0) root         (0)      528 2021-05-31 20:46:01.271607 seas-0.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2914 2021-04-01 15:33:50.000000 seas-0.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-31 20:46:01.264225 seas-0.0.2/seas/
--rwxrwxrwx   0 root         (0) root         (0)      570 2021-04-01 15:28:27.000000 seas-0.0.2/seas/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5929 2021-04-01 15:28:27.000000 seas-0.0.2/seas/colormaps.py
--rwxrwxrwx   0 root         (0) root         (0)     5852 2021-04-01 15:28:27.000000 seas-0.0.2/seas/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)    23634 2021-04-01 15:28:27.000000 seas-0.0.2/seas/domains.py
--rwxrwxrwx   0 root         (0) root         (0)    17978 2021-04-01 15:28:27.000000 seas-0.0.2/seas/experiment.py
--rwxrwxrwx   0 root         (0) root         (0)     9274 2021-04-01 15:28:27.000000 seas-0.0.2/seas/filemanager.py
--rwxrwxrwx   0 root         (0) root         (0)    64904 2021-04-01 15:28:27.000000 seas-0.0.2/seas/gui.py
--rwxrwxrwx   0 root         (0) root         (0)    14806 2021-04-01 15:28:27.000000 seas-0.0.2/seas/hdf5manager.py
--rwxrwxrwx   0 root         (0) root         (0)    25633 2021-04-01 19:24:07.000000 seas-0.0.2/seas/ica.py
--rwxrwxrwx   0 root         (0) root         (0)     8559 2021-04-01 15:28:27.000000 seas-0.0.2/seas/rois.py
--rwxrwxrwx   0 root         (0) root         (0)     9666 2021-04-01 15:28:27.000000 seas-0.0.2/seas/signalanalysis.py
--rwxrwxrwx   0 root         (0) root         (0)    32362 2021-04-01 15:28:27.000000 seas-0.0.2/seas/video.py
--rwxrwxrwx   0 root         (0) root         (0)    36606 2021-04-01 15:28:27.000000 seas-0.0.2/seas/waveletAnalysis.py
--rwxrwxrwx   0 root         (0) root         (0)    17274 2021-04-01 00:44:02.000000 seas-0.0.2/seas/waveletFunctions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-31 20:46:01.267675 seas-0.0.2/seas.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      528 2021-05-31 20:46:01.000000 seas-0.0.2/seas.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      530 2021-05-31 20:46:01.000000 seas-0.0.2/seas.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-05-31 20:46:01.000000 seas-0.0.2/seas.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       82 2021-05-31 20:46:01.000000 seas-0.0.2/seas.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2021-05-31 20:46:01.000000 seas-0.0.2/seas.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2021-05-31 20:46:01.272281 seas-0.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      925 2021-05-31 20:45:56.000000 seas-0.0.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-31 20:46:01.270866 seas-0.0.2/tests/
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-04-01 00:44:02.000000 seas-0.0.2/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2221 2021-04-01 15:28:27.000000 seas-0.0.2/tests/colormaps_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2283 2021-04-01 15:28:27.000000 seas-0.0.2/tests/experiment_test.py
--rwxrwxrwx   0 root         (0) root         (0)      970 2021-04-01 00:44:02.000000 seas-0.0.2/tests/filemanager_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1017 2021-04-01 02:18:27.000000 seas-0.0.2/tests/video_test.py
+drwxrwxr-x   0 sydney    (1000) sydney    (1000)        0 2023-04-18 00:14:42.861475 seas-0.0.3/
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)     1074 2023-04-16 18:10:49.000000 seas-0.0.3/LICENSE
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)      539 2023-04-18 00:14:42.861475 seas-0.0.3/PKG-INFO
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)     3017 2023-04-16 18:10:49.000000 seas-0.0.3/README.md
+drwxrwxr-x   0 sydney    (1000) sydney    (1000)        0 2023-04-18 00:14:42.861475 seas-0.0.3/seas/
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)      570 2023-04-16 18:45:26.000000 seas-0.0.3/seas/__init__.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)     5655 2023-04-16 19:47:09.000000 seas-0.0.3/seas/colormaps.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)     5862 2023-04-16 18:45:28.000000 seas-0.0.3/seas/defaults.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    24109 2023-04-16 18:58:51.000000 seas-0.0.3/seas/domains.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    18320 2023-04-16 19:58:37.000000 seas-0.0.3/seas/experiment.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    12195 2023-04-16 19:37:25.000000 seas-0.0.3/seas/filemanager.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    69366 2023-04-17 04:11:37.000000 seas-0.0.3/seas/gui.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    17569 2023-04-16 20:20:18.000000 seas-0.0.3/seas/hdf5manager.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    26572 2023-04-17 02:36:45.000000 seas-0.0.3/seas/ica.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    10425 2023-04-17 03:51:43.000000 seas-0.0.3/seas/rois.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    14007 2023-04-17 03:28:38.000000 seas-0.0.3/seas/signalanalysis.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    38898 2023-04-17 04:11:37.000000 seas-0.0.3/seas/video.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    36496 2023-04-17 03:28:33.000000 seas-0.0.3/seas/waveletAnalysis.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)    17274 2023-04-17 03:23:51.000000 seas-0.0.3/seas/waveletFunctions.py
+drwxrwxr-x   0 sydney    (1000) sydney    (1000)        0 2023-04-18 00:14:42.861475 seas-0.0.3/seas.egg-info/
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)      539 2023-04-18 00:14:42.000000 seas-0.0.3/seas.egg-info/PKG-INFO
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)      538 2023-04-18 00:14:42.000000 seas-0.0.3/seas.egg-info/SOURCES.txt
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)        1 2023-04-18 00:14:42.000000 seas-0.0.3/seas.egg-info/dependency_links.txt
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)       82 2023-04-18 00:14:42.000000 seas-0.0.3/seas.egg-info/requires.txt
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)       11 2023-04-18 00:14:42.000000 seas-0.0.3/seas.egg-info/top_level.txt
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)       79 2023-04-18 00:14:42.861475 seas-0.0.3/setup.cfg
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)      926 2023-04-17 04:32:15.000000 seas-0.0.3/setup.py
+drwxrwxr-x   0 sydney    (1000) sydney    (1000)        0 2023-04-18 00:14:42.861475 seas-0.0.3/tests/
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)        1 2023-04-16 18:10:49.000000 seas-0.0.3/tests/__init__.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)     2221 2023-04-16 18:10:49.000000 seas-0.0.3/tests/colormaps_test.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)     2284 2023-04-16 18:48:08.000000 seas-0.0.3/tests/experiment_test.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)      970 2023-04-16 18:10:49.000000 seas-0.0.3/tests/filemanager_test.py
+-rw-rw-r--   0 sydney    (1000) sydney    (1000)     1017 2023-04-16 18:10:49.000000 seas-0.0.3/tests/video_test.py
```

### Comparing `seas-0.0.2/PKG-INFO` & `seas-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: seas
-Version: 0.0.2
+Version: 0.0.3
 Summary: python Signal Extraction and Segmentation
 Home-page: https://github.com/ackmanlab/pySEAS
 Author: Sydney Weiser
 Author-email: scweiser@ucsc.edu
 License: UNKNOWN
-Description: Data-driven filtration and segmentation of mesoscale neural dynamics
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Data-driven filtration and segmentation of mesoscale neural dynamics
+
```

### Comparing `seas-0.0.2/README.md` & `seas-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pySEAS
 
 python Signal Extraction and Segmentation
 
-See readme files in examples for basic usage.
+See readme files in examples for basic usage, or the [ReadTheDocs](https://pyseas.readthedocs.io/en/latest/) page to browse available function help.
 
 ---
 
 # Installation Notes
 
 should work with most python3s.  Currently being tested and developed on 3.8.
```

### Comparing `seas-0.0.2/seas/__init__.py` & `seas-0.0.3/seas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,13 @@
 # from . import ica
 from . import domains
 # from .experiment import Experiment
 
 # from .hdf5manager import hdf5manager
 # from .gui import run_gui as run_gui
 
-
 # from . import rois
 # from . import colormap
 # from . import filemanager
 # signalanalysis.py
 # waveletAnalysis.py
-# waveletFunctions.py
+# waveletFunctions.py
```

### Comparing `seas-0.0.2/seas/colormaps.py` & `seas-0.0.3/seas/colormaps.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,18 @@
 from matplotlib import pyplot as plt
 from matplotlib.colors import ListedColormap
 import warnings
 
 from seas.defaults import config
 
 
-def get_mpl_colormap(colormap_name):
+def get_mpl_colormap(colormap_name: str):
     '''
     Convert a matplotlib colormap to a cv2-compatible colormap.
 
-    Arguments:
-        colormap_name: 
-            The name of the matplotlib colormap
-
-    Returns:
-        color_range: 
-            a 256x1x3 dimensional array holding the 8-bit color map representation compatible with opencv
-
-    Raises:
-        ValueError: if colormap_name was invalid
     '''
     # Initialize the matplotlib color map, convert to scalar mappable colormap
     matplotlib_colormap = plt.get_cmap(colormap_name)
     scalarmappable_colormap = plt.cm.ScalarMappable(cmap=matplotlib_colormap)
 
     # Obtain linear color range
     cv2_colormap = scalarmappable_colormap.to_rgba(np.linspace(0, 1, 256),
@@ -41,15 +31,15 @@
     return cv2_colormap.reshape(256, 1, 3)
 
 
 # Functions for colormap manipulation
 #------------------------------------
 
 
-def rescaled_to_dfof(rescaled_value, slope, array_min):
+def rescaled_to_dfof(rescaled_value: float, slope: float, array_min: float):
     '''
     Convert a value in 8-bit rescaled units (0-255) to a dfof value.
 
     Arguments:
         rescaled_value: 
             The rescaled_value in rescaled units to convert
         slope: 
@@ -60,15 +50,15 @@
     Returns:
         dfof_value: 
             The rescaled_value converted back to dfof by the scale and array_min parameters.
     '''
     return slope * (rescaled_value - array_min)
 
 
-def dfof_to_rescaled(dfof_value, slope, array_min):
+def dfof_to_rescaled(dfof_value: float, slope: float, array_min: float):
     '''
     Convert a dfof value to 8-bit rescaled units (0-255).
 
     Arguments:
         dfof_value: 
             The rescaled_value in dfof units to convert
         slope: 
@@ -79,38 +69,37 @@
     Returns:
         rescaled_value: 
             The rescaled_value converted to rescaled units by the scale and array_min parameters.
     '''
     return dfof_value / slope + array_min
 
 
-def save_colorbar(scale, path, colormap='default'):
+def save_colorbar(scale: dict, path: str, colormap=None):
     '''
     Save a plt colorbar with a given scale to a specified path.  Accepts plt or cv2 colormap objects.
 
     Arguments:
         scale: 
             The scale dictionary returned by rescale_movie.  Must have keys 'min' and 'max' providing the range of the rescale.
         path: 
             Where to save the file to. (supported formats: eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)
         colormap: 
-            Which colormap to save.  Should be a cv2 colormap object or name of a plt colormap.  If left as 'default', the default colormap will be loaded.  
+            Which colormap to save.  Should be a cv2 colormap object or name of a plt colormap.  If left as None, the default colormap will be loaded.  
 
     Returns:
         Nothing
 
     Raises:
         KeyError: 
             The min and/or max keys were not in scale dictionary
         ValueError: 
             The path provided was not supported by plt figure outputs.
     '''
-    if type(colormap) is str:
-        if colormap == 'default':
-            colormap = DEFAULT_COLORMAP
+    if colormap is None:
+        colormap = DEFAULT_COLORMAP
 
     if type(colormap) is np.ndarray:
         colormap = ListedColormap(colormap.squeeze() / 256)
 
     ticks = np.linspace(scale['min'], scale['max'], 5).round(4)
 
     plt.figure(figsize=(1, 2))
@@ -125,34 +114,34 @@
     plt.cla()
     plt.axis('off')
 
     plt.savefig(path, bbox_inches='tight')
     plt.close()
 
 
-def apply_colormap(video, colormap='default'):
+def apply_colormap(video: np.ndarray, colormap: np.ndarray = None):
     '''
     Save a plt colorbar with a given scale to a specified path.  Accepts plt or cv2 colormap objects.
 
     Arguments:
         video: 
             The video to apply the colormap to.  Should be in format (t,x,y)
         colormap: 
-            Which colormap to apply  Should be a cv2 colormap object.  If left as 'default', the default colormap will be loaded.  
+            Which colormap to apply  Should be a cv2 colormap object.  If left as None, the default colormap will be loaded.  
 
     Returns:
         video_color: 
             The video with colormap applied, in format (t,x,y,c)
 
     Raises:
         AssertionError: The colormap was invalid.
     '''
     print('\nApplying Color Map to Movie\n-----------------------')
 
-    if colormap == 'default':
+    if colormap is None:
         colormap = DEFAULT_COLORMAP
 
     assert type(colormap) is np.ndarray, 'Colormap was not cv2 compatible'
     assert colormap.shape == (256, 1, 3), 'Colormap input was not understood'
 
     sz = video.shape
     video_color = np.zeros((sz[0], sz[1], sz[2], 3),
@@ -162,14 +151,15 @@
                           video_color[i, :, :, :])
 
     return video_color
 
 
 # Get or set default parameters.
 #------------------------------------
+
 DEFAULT_COLORMAP = get_mpl_colormap(config['colormap']['videos'])
 COMPONENT_COLORMAP = get_mpl_colormap(config['colormap']['components'])
 
 CUSTOM_PASTEL_LISTED_VALUES = np.array(
     [[123, 219, 148, 255], [255, 178, 240, 255], [153, 85, 255, 255],
      [102, 191, 213, 255], [183, 200, 196, 255], [190, 237, 232, 255]]) / 255
```

### Comparing `seas-0.0.2/seas/defaults.py` & `seas-0.0.3/seas/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         "Olfactory": "O",
         "SuperiorColliculus": "SC",
         "Clear": "X"
     },
 }
 
 
-def write_config(path, parameters='default'):
+def write_config(path: str, parameters: dict = None):
     '''
     Writes a config file to path.  The default location is the seas module directory.
 
     Arguments:
         path: Where to save the config file.
 
     Returns:
@@ -115,27 +115,27 @@
             "Retrosplenial": "R",
             "Olfactory": "O",
             "SuperiorColliculus": "SC",
             "Clear": "X"
     '''
     config = configparser.ConfigParser()
 
-    if parameters == 'default':
+    if parameters is None:
         parameters = DEFAULT_CONFIG
 
     for key in parameters:
         config[key] = parameters[key]
 
     with open(path, 'w') as configfile:
         config.write(configfile)
 
     return config
 
 
-def load_config(path=None):
+def load_config(path: str = None):
     '''
     Load the configuration file.  The default location is the seas module directory.
 
     Arguments:
         path: Where to load the config file from.
 
     Returns:
```

### Comparing `seas-0.0.2/seas/domains.py` & `seas-0.0.3/seas/domains.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 from seas.hdf5manager import hdf5manager
 from seas.video import save, rescale, rotate
 from seas.ica import rebuild_mean_roi_timecourse, filter_mean
 from seas.rois import make_mask
 from seas.colormaps import save_colorbar, REGION_COLORMAP, DEFAULT_COLORMAP
 
 
-def get_domain_map(components,
-                   blur=21,
-                   min_size_ratio=0.1,
-                   map_only=True,
-                   apply_filter_mean=True,
-                   max_loops=2,
-                   ignore_small=True):
+def get_domain_map(components: dict,
+                   blur: int = 21,
+                   min_size_ratio: float = 0.1,
+                   map_only: bool = True,
+                   apply_filter_mean: bool = True,
+                   max_loops: int = 2,
+                   ignore_small: bool = True):
     '''
     Creates a domain map from extracted independent components.  A pixelwise maximum projection of the blurred signal components is taken through the n_components axis, to create a flattened representation of where a domain was maximally significant across the cortical surface.  Components with multiple noncontiguous significant regions are counted as two distinct domains.
 
     Arguments:
         components: 
             The dictionary of components returned from seas.ica.project.  Domains are most interesting if artifacts has already been assigned through seas.gui.run_gui.
         blur: 
@@ -226,15 +226,18 @@
             output[key] = timecourseresults[key]
     else:
         print('not calculating domain time courses')
 
     return output
 
 
-def save_domain_map(domain_ROIs, basepath, blur_level, n_rotations=0):
+def save_domain_map(domain_ROIs: np.ndarray,
+                    basepath: str,
+                    blur_level: int,
+                    n_rotations: int = 0):
     '''
     Saves domain maps to pngs for visualization.  Two files are saved to basepath_xb.png and basepath_xb_edges.png. One is the visualization of the domain indices, saved in black and white, the other is just the edge visualization.
 
     Arguments:
         domain_ROIs:
         basepath: The path to save at, including everything but the file extension.
         blur_level: The Gaussian blur kernel size, only used for generating the image name
@@ -261,17 +264,17 @@
          rescale_range=True)
     save(edges,
          savepath.replace('.png', '_edges.png'),
          apply_cmap=False,
          rescale_range=True)
 
 
-def get_domain_rebuilt_timecourses(domain_ROIs,
-                                   components,
-                                   apply_filter_mean=True):
+def get_domain_rebuilt_timecourses(domain_ROIs: np.ndarray,
+                                   components: dict,
+                                   apply_filter_mean: bool = True):
     '''
     Get time courses for each domain ROI.  The filtered movie is rebuilt under each ROI (one at a time).  The mean is taken under each domain ROI.  The ROI_timecourses and mean_filtered are returned in output.
 
     Arguments:
         domain_ROIs: 
             The domain ROI map built by get_domain_map
         components : 
@@ -293,15 +296,17 @@
     if apply_filter_mean:
         mean_filtered = filter_mean(components['mean'])
         output['mean_filtered'] = mean_filtered
 
     return output
 
 
-def get_domain_edges(domain_ROIs, clear_bg=False, linepad=None):
+def get_domain_edges(domain_ROIs: np.ndarray,
+                     clear_bg: bool = False,
+                     linepad: int = None):
     '''
     Get the edges of the domain map using canny edge detection.
 
     Arguments:
         domain_ROIs: 
             The domain map built by get_domain_map.
         clear_bg: 
@@ -329,19 +334,19 @@
     if clear_bg:
         edges = edges.astype('float64')
         edges[np.where(edges == 0)] = np.nan
 
     return edges
 
 
-def get_padded_borders(domain_ROIs,
-                       blur,
-                       rois,
-                       n_roi_rotations=0,
-                       bounding_box=None):
+def get_padded_borders(domain_ROIs: np.ndarray,
+                       blur: int,
+                       rois: dict,
+                       n_roi_rotations: int = 0,
+                       bounding_box: bool = None):
     '''
     Since a gaussian blur between a value with a number and a nan border will result in an increasingly large nan border, get this new border roi boundary.  Rois are used to separate hemispheres rather than blur together.
 
     Arguments:
         domain_ROIs: 
             The domain map built by get_domain_map.
         blur: 
@@ -377,15 +382,15 @@
         padmask[np.where(~np.isnan(blurred))] = 1
 
     padmask = rotate(padmask, n_roi_rotations)
 
     return padmask
 
 
-def domain_map(domain_ROIs, values=None):
+def domain_map(domain_ROIs: np.ndarray, values: np.ndarray = None):
     '''
     Used to generate a domain map with a specific coloration scheme.  If values are a calculated metric, such as pearson correlation, each domain i in the domain map will be colored by its value values[i] in the input vector.
 
     Arguments:
         domain_ROIs: 
             The domain map built by get_domain_map.
         values: 
@@ -406,25 +411,25 @@
             domainmap[np.where(domain_ROIs == i)] = values[i]
     else:
         domainmap = domain_ROIs
 
     return domainmap
 
 
-def mosaic_movie(domain_ROIs,
-                 ROI_timecourses,
-                 savepath=None,
-                 t_start=None,
-                 t_stop=None,
-                 n_rotations=0,
-                 colormap='default',
-                 resize_factor=1,
-                 codec=None,
-                 speed=1,
-                 fps=10):
+def mosaic_movie(domain_ROIs: np.ndarray,
+                 ROI_timecourses: np.ndarray,
+                 savepath: str = None,
+                 t_start: int = None,
+                 t_stop: int = None,
+                 n_rotations: int = 0,
+                 colormap: np.ndarray = None,
+                 resize_factor: int = 1,
+                 codec: str = None,
+                 speed: int = 1,
+                 fps: int = 10):
     '''
     Creates a mosaic movie, where the original movie is played back as a series of domain timecourses, each displayed over its original domain.
 
     Arguments:
         domain_ROIs: 
             The domain map built by get_domain_map.
         ROI_timecourses:
@@ -443,15 +448,15 @@
             The factor to resize by when writing the video.
             
     Returns:    
         Nothing.
     '''
     print('\nRebuilding Mosiac Movie\n-----------------------')
 
-    if colormap == 'default':
+    if colormap is None:
         colormap = DEFAULT_COLORMAP
 
     t, x, y = (ROI_timecourses.shape[1], domain_ROIs.shape[0],
                domain_ROIs.shape[1])
 
     if (t_start is not None) or (t_stop is not None):
         frames = np.arange(t)
@@ -484,25 +489,25 @@
              colormap=colormap,
              resize_factor=1,
              codec=None,
              speed=1,
              fps=10)
 
 
-def rolling_mosaic_movie(domain_ROIs,
-                         ROI_timecourses,
-                         savepath,
-                         t_start=None,
-                         t_stop=None,
-                         n_rotations=0,
-                         colormap='default',
-                         resize_factor=1,
-                         codec=None,
-                         speed=1,
-                         fps=10):
+def rolling_mosaic_movie(domain_ROIs: np.ndarray,
+                         ROI_timecourses: np.ndarray,
+                         savepath: str,
+                         t_start: int = None,
+                         t_stop: int = None,
+                         n_rotations: int = 0,
+                         colormap: np.ndarray = None,
+                         resize_factor: int = 1,
+                         codec: str = None,
+                         speed: int = 1,
+                         fps: int = 10):
     '''
     A low memory version of mosaic_movie.  The functionality is the same, except each frame is written one at at a time.  Movie scale values may be slightly different, since they are calculated from the first frame instead of on the entire movie.
 
         Creates a mosaic movie, where the original movie is played back as a series of domain timecourses, each displayed over its original domain.
 
     Arguments:
         domain_ROIs: 
@@ -522,58 +527,58 @@
             
     Returns:    
         Nothing.
     '''
 
     print('\nWriting Rolling Mosiac Movie\n-----------------------')
 
-    if colormap == 'default':
+    if colormap is None:
         colormap = DEFAULT_COLORMAP
 
-    # Initialize Parameters
+    # Initialize Parameters.
     resize_factor = 1 / resize_factor
     x, y = domain_ROIs.shape
     n_domains = ROI_timecourses.shape[0]
     t = np.arange(ROI_timecourses.shape[1])
     t = t[t_start:t_stop]
 
-    # Set up resizing factors
+    # Set up resizing factors.
     w = int(x // resize_factor)
     h = int(y // resize_factor)
 
-    # find codec to use if not specified
+    # Find codec to use, if not specified.
     if codec is None:
         if savepath.endswith('.mp4'):
             if os.name == 'posix':
                 codec = 'X264'
             elif os.name == 'nt':
                 codec = 'XVID'
         else:
             if os.name == 'posix':
                 codec = 'MP4V'
             elif os.name == 'nt':
                 codec = 'XVID'
             else:
                 raise TypeError('Unknown os type: {0}'.format(os.name))
 
-    # initialize movie writer
+    # Initialize movie writer.
     display_speed = fps * speed
     fourcc = cv2.VideoWriter_fourcc(*codec)
     out = cv2.VideoWriter(savepath, fourcc, display_speed, (h, w), isColor=True)
 
     def write_frame(frame):
-        # rescale and convert to uint8
+        # rescale and convert to uint8.
         frame = rescale(frame,
                         min_max=(scale['min'], scale['max']),
                         cap=False,
                         verbose=False).astype('uint8')
         frame = cv2.resize(frame, (h, w), interpolation=cv2.INTER_AREA)
         frame = rotate(frame, n_rotations)
 
-        # apply colormap, write frame to .avi
+        # Apply colormap, write frame to .avi.
         if colormap is not None:
             frame = cv2.applyColorMap(frame, colormap)
         else:
             frame = np.repeat(frame[:, :, None], 3, axis=2)
 
         out.write(frame)
 
@@ -585,15 +590,15 @@
         if f % 10 == 0:
             print('on frame:', f, '/', t.size)
 
         frame[:] = np.nan
         for i in range(n_domains):
             frame[np.where(domain_ROIs == i)] = ROI_timecourses[i, f]
 
-        # if first frame, calculate scaling parameters
+        # If first frame, calculate scaling parameters.
         if (f == 0):
             mean = np.nanmean(frame)
             std = np.nanstd(frame)
 
             fmin = mean - 3 * std
             fmax = mean + 7 * std
```

### Comparing `seas-0.0.2/seas/experiment.py` & `seas-0.0.3/seas/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 import numpy as np
 import os
 
-import seas.video 
+import seas.video
 
 from seas.video import load, dfof, rotate, rescale
 
-
 from seas.filemanager import sort_experiments, get_exp_span_string, read_yaml
 from seas.rois import roi_loader, make_mask, get_masked_region, insert_masked_region, draw_bounding_box
 from seas.hdf5manager import hdf5manager
 from seas.ica import project, filter_mean
 from seas.signalanalysis import sort_noise, lag_n_autocorr
 from seas.waveletAnalysis import waveletAnalysis
 
+from typing import List
+
 
 class Experiment:
     '''
     A class to store mesoscale calcium imaging experiment information and provide functions used for common experiment and video manipulations.
     Includes functionality for loading and rotating videos, cropping to a specific region of interest (defined by user input and/or roi files, loading and storing yaml metadata, etc.)
 
     Attributes:
         downsample: 
-            The spatial downsampling factor
+            The spatial downsampling factor.
         downsample_t:
-            The temporal downsampling factor
+            The temporal downsampling factor.
         movie:
-            The loaded raw movie file 
+            The loaded raw movie file .
         path:
-            The pathlist of loaded videos
+            The pathlist of loaded videos.
         n_rotations:
-            The number of times the video was rotated
+            The number of times the video was rotated.
         rotate_rois_with_video:
-            Whether rois are rotated with the video or not
+            Whether rois are rotated with the video or not.
         bounding_box:
-            The bounding coordinates selected for the content of interest from the video file
+            The bounding coordinates selected for the content of interest from the video file.
         shape:
-            The video shape
+            The video shape.
         name:
-            The detected name of the experiment from the input files
+            The detected name of the experiment from the input files.
         dir:
-            The directory the video files reside in
+            The directory the video files reside in.
 
     The following attributes are also available if rois are loaded:        
         n_roi_rotations:
-            The number of times the rois were rotated
+            The number of times the rois were rotated.
         rois:
-            The roi dictionary loaded from FIJI RoiSet.zip file
+            The roi dictionary loaded from FIJI RoiSet.zip file.
         roimask:
-            A binary masked array denoting where the movie should be masked
+            A binary masked array denoting where the movie should be masked.
         meta:
-            The experiment metadata loaded from a yaml file
+            The experiment metadata loaded from a yaml file.
 
     Functions:
         load_rois: 
-            Load rois from a FIJI RoiSet.zip file
+            Load rois from a FIJI RoiSet.zip file.
         load_meta:
-            Load metadata from a yaml file
+            Load metadata from a yaml file.
         rotate: 
-            Rotate the video CCW, adjust mask and bounding box accordingly
+            Rotate the video CCW, adjust mask and bounding box accordingly.
         define_mask_boundaries:
-            Auto detect the mask boundaries from the loaded roimask
+            Auto detect the mask boundaries from the loaded roimask.
         draw_bounding_box: 
-            Launch a GUI to draw a bounding box to crop the movie
+            Launch a GUI to draw a bounding box to crop the movie.
         bound_mask:
-            Returns the mask bound to the bounding box
+            Returns the mask bound to the bounding box.
         bound_movie:
-            Returns the movie bound to the bounding box
+            Returns the movie bound to the bounding box.
         ica_project:
-            Perform an ICA projection to the movie
+            Perform an ICA projection to the movie.
 
     Initialization Arguments:
         pathlist: 
             The list of paths to load raw video data from, in order.  To sort, use seas.filemanager functions.
         downsample: 
             An integer factor to spatially downsample frames with.  Implements an integer averaging spatial downsample where downsample x downsample pixels are reduced to 1.
         downsample_t: 
@@ -80,19 +81,19 @@
             The number of ccw rotations to rotate the video.
         rotate_rois_with_video: 
             If true, rotate all loaded rois by n_rotations as well.
 
     '''
 
     def __init__(self,
-                 pathlist,
-                 downsample=False,
-                 downsample_t=False,
-                 n_rotations=0,
-                 rotate_rois_with_video=False):
+                 pathlist: List[str],
+                 downsample: int = False,
+                 downsample_t: int = False,
+                 n_rotations: int = 0,
+                 rotate_rois_with_video: bool = False):
         '''
         Arguments:
             pathlist: 
                 The list of paths to load raw video data from, in order.  To sort, use seas.filemanager functions.
             downsample: 
                 An integer factor to spatially downsample frames with.  Implements an integer averaging spatial downsample where downsample x downsample pixels are reduced to 1.
             downsample_t: 
@@ -106,32 +107,32 @@
         if isinstance(pathlist, str):
             pathlist = [pathlist]
 
         movie = seas.video.load(pathlist, downsample, downsample_t)
         assert (len(movie.shape) == 3), 'File was not a 3 dimensional video.\n'
 
         if np.any(np.isnan(movie)):
-            # if the video was already masked
+            # If the video was already masked
             roimask = np.zeros(movie[0].shape, dtype='uisnt8')
             roimask[np.where(~np.isnan(movie[0]))] = 1
             self.roimask = roimask
 
         self.downsample = downsample
         self.downsample_t = downsample_t
         self.movie = movie
         self.path = pathlist
         self.n_rotations = n_rotations
         self.rotate_rois_with_video = rotate_rois_with_video
 
-        # define default bounding box as full size video
+        # Define default bounding box as full size video.
         self.bounding_box = np.array([[0, self.movie.shape[1]],
                                       [0, self.movie.shape[2]]])
         self.shape = self.bound_movie().shape
 
-        # if multiple experiments included, get a span string
+        # If multiple experiments included, get a span string.
         # (i.e. 01, 02, 03, 04 - > 01-04)
         experiments = sort_experiments(pathlist, verbose=False).keys()
         spanstring = get_exp_span_string(experiments)
         self.name = spanstring
 
         self.dir = os.path.dirname(pathlist[0])
         self.rotate()
@@ -140,18 +141,18 @@
         '''
         Rotates movie by self.n_rotations, and updates the shape and bounding box to reflect this change.
         '''
         if self.n_rotations > 0:
             self.movie = rotate(self.movie, self.n_rotations)
             self.bounding_box = np.array([[0, self.movie.shape[1]],
                                           [0, self.movie.shape[2]]
-                                         ])  #resets to whole movie
+                                         ])  # Resets to whole movie.
             self.shape = self.bound_movie().shape
 
-    def load_rois(self, path, n_roi_rotations=0):
+    def load_rois(self, path: str, n_roi_rotations: int = 0):
         '''
         Load rois set in an FIJI/ImageJ RoiSet.zip file to the experiment file, and creates a roimask based on the rois.
 
         Arguments:
             path: 
                 The path to the .zip file.
             n_roi_rotations: 
@@ -159,42 +160,42 @@
         '''
         if self.rotate_rois_with_video:
             n_roi_rotations = self.n_rotations
 
         rois = roi_loader(path)
         self.n_roi_rotations = n_roi_rotations
 
-        # Store in class file
+        # Store in class file.
         print(len(rois), 'ROIs found')
 
-        # resize (and flip) if necessary
+        # Resize (and flip) if necessary.
         if self.downsample is not False:
             print('video was downsampled.. downsampling rois.')
             for roi in rois:
                 rois[roi] = rois[roi] // self.downsample
 
         self.rois = rois
 
-        # Initialize Empty Mask
+        # Initialize Empty Mask.
         roimask = np.zeros(self.shape[1:3], dtype='uint8')
 
-        # Add mask region from all rois
+        # Add mask region from all rois.
         for i, roi in enumerate(rois):
             roimask += make_mask(rois[roi], self.shape[1:3])
 
         roimask[np.where(roimask > 1)] = 1
 
         if roimask.sum().sum() == 0:
             print('Roimask contains no ROI regions.  Not storing..')
             return
 
         self.roimask = rotate(roimask, n_roi_rotations)
         print('')
 
-    def load_meta(self, meta_path):
+    def load_meta(self, meta_path: str):
         '''
         Load metadata to the experiment file.  This is not used in any decomposition, but provides a convenient way to save metadata along with the processed file.
 
         Arguments:
             meta_path: 
                 The path to the metadata .yaml file.
         '''
@@ -227,51 +228,53 @@
 
         row, cols = np.nonzero(self.roimask)
         ROI = np.array([[np.min(row), np.max(row)],
                         [np.min(cols), np.max(cols)]])
 
         self.bounding_box = ROI
 
-    def bound_movie(self, movie=None, bounding_box=None):
+    def bound_movie(self,
+                    movie: np.ndarray = None,
+                    bounding_box: List[List[int]] = None) -> np.ndarray:
         '''
         Returns the movie cropped by the bounding box.
         '''
         if bounding_box == None:
             bounding_box = self.bounding_box
 
         if movie is None:
             movie = self.movie
 
         ROI = bounding_box
         return movie[:, ROI[0][0]:ROI[0][1], ROI[1][0]:ROI[1][1]]
 
-    def bound_mask(self, bounding_box=None):
+    def bound_mask(self, bounding_box: List[List[int]] = None) -> np.ndarray:
         '''
         Returns the roimask cropped by the bounding box.
         '''
         try:
             if bounding_box == None:
                 bounding_box = self.bounding_box
 
             ROI = bounding_box
             return self.roimask[ROI[0][0]:ROI[0][1], ROI[1][0]:ROI[1][1]]
         except:
             return None
 
     def ica_project(self,
-                    movie=None,
-                    savedata=True,
-                    calc_dfof=True,
-                    del_movie=True,
-                    n_components=None,
-                    svd_multiplier=None,
-                    suffix='',
-                    output_folder=None,
-                    mean_filter_method='wavelet',
-                    low_cutoff=0.5):
+                    movie: np.ndarray = None,
+                    savedata: bool = True,
+                    calc_dfof: bool = True,
+                    del_movie: bool = True,
+                    n_components: int = None,
+                    svd_multiplier: float = None,
+                    suffix: str = '',
+                    output_folder: str = None,
+                    mean_filter_method: str = 'wavelet',
+                    low_cutoff: float = 0.5) -> dict:
         '''
         Apply an ica decomposition to the experiment.  If rois and/or a bounding box have been defined, these will be used to crop the movie before filtration.
 
         By default, results are all saved to a [experiment]_[parameters]_ica.hdf5 file in the same directory as the original video files.
 
         Arguments:
             movie: 
@@ -295,50 +298,50 @@
             low_cutoff: 
                 The lower cutoff for a highpass filter.  Default is 0.5Hz.
 
         Returns:
             components: A dictionary containing all the results, metadata, and information regarding the filter applied.
 
                 mean: 
-                    the original video mean
+                    The original video mean.
                 roimask: 
-                    the mask applied to the video before decomposing
+                    The mask applied to the video before decomposing.
                 shape: 
-                    the original shape of the movie array
+                    The original shape of the movie array.
                 eig_mix: 
-                    the ICA mixing matrix
+                    The ICA mixing matrix.
                 timecourses: 
-                    the ICA component time series
+                    The ICA component time series.
                 eig_vec: 
-                    the eigenvectors
+                    The eigenvectors.
                 n_components:
-                    the number of components in eig_vec (reduced to only have 25% of total components as noise)
+                    The number of components in eig_vec (reduced to only have 25% of total components as noise).
                 project_meta:
                     The metadata for the ica projection
                 expmeta:
-                    All metadata created for this class
+                    All metadata created for this class.
                 lag1: 
-                    the lag-1 autocorrelation
+                    The lag-1 autocorrelation.
                 noise_components: 
-                    a vector (n components long) to store binary representation of which components were detected as noise 
+                    A vector (n components long) to store binary representation of which components were detected as noise.
                 cutoff: 
-                    the signal-noise cutoff value
+                    The signal-noise cutoff value.
                 mean_filtered: 
-                    the filtered mean
+                    The filtered mean.
                 mean_filter_meta: 
-                    metadata on how the mean filter was applied
+                    Metadata on how the mean filter was applied.
 
             if the n_components was automatically set, the following additional keys are also returned in components
 
                 svd_cutoff: 
-                    the number of components originally decomposed
+                    The number of components originally decomposed.
                 lag1_full: 
-                    the lag-1 autocorrelation of the full set of components decomposed before cropping to only 25% noise components
+                    The lag-1 autocorrelation of the full set of components decomposed before cropping to only 25% noise components.
                 svd_multiplier: 
-                    the svd multiplier value used to determine cutoff
+                    The svd multiplier value used to determine cutoff.
         '''
         print('\nICA Projecting\n-----------------------')
 
         if savedata:
             suffix_list = []
             if len(suffix) > 0:
                 suffix_list.append(suffix)
@@ -385,17 +388,17 @@
         print('Saving keys under expmeta in PC components:')
         for key in expmeta:
             print(key)
 
         if savedata:
             f.save(components)
 
-        # calculate decomposition:
+        # Calculate decomposition:
         if 'eig_vec' and 'eig_mix' in components:
-            # if data was already in the save path, use it
+            # If data was already in the save path, use it
             print('Found ICA decomposition in components')
         else:
 
             if hasattr(self, 'roimask'):
                 roimask = self.bound_mask()
             else:
                 roimask = None
@@ -406,23 +409,23 @@
                 if calc_dfof:
                     movie = dfof(movie)
 
             if del_movie:
                 print('Deleting original movie to save memory..')
                 del self.movie
 
-            #drop dimension and flip to prepare timecourse for ICA
+            # Drop dimension and flip to prepare timecourse for ICA.
             shape = movie.shape
             t, x, y = shape
             vector = movie.reshape(t, x * y)
-            vector = vector.T  # now vector is (x*y, t) for ICA along x*y dimension
+            vector = vector.T  # Now vector is (x*y, t) for ICA along x*y dimension.
             print('M has been reshaped from {0} to {1}\n'.format(
                 movie.shape, vector.shape))
 
-            # run ICA projection
+            # Run ICA projection.
             ica_project_kwargs = {'vector': vector, 'shape': shape}
 
             if svd_multiplier is not None:
                 ica_project_kwargs['svd_multiplier'] = svd_multiplier
 
             if roimask is not None:
                 ica_project_kwargs['roimask'] = roimask
@@ -432,15 +435,15 @@
 
             components = project(**ica_project_kwargs)
             components['expmeta'] = expmeta
 
             if savedata:
                 f.save(components)
 
-        # Calculate other relevant parameters
+        # Calculate other relevant parameters.
         components['mean_filtered'] = filter_mean(
             components['mean'],
             filter_method=mean_filter_method,
             low_cutoff=low_cutoff)
         components['mean_filter_meta'] = {
             'mean_filter_method': mean_filter_method,
             'low_cutoff': low_cutoff
```

### Comparing `seas-0.0.2/seas/gui.py` & `seas-0.0.3/seas/gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,23 +14,37 @@
 from seas.waveletAnalysis import waveletAnalysis
 from seas.hdf5manager import hdf5manager
 from seas.defaults import config
 from seas.ica import rebuild_eigenbrain
 from seas.domains import get_domain_map, domain_map, get_domain_edges
 
 
-def run_gui(components, rotate=0, savepath=None, default_assignment=None):
+def run_gui(components: dict,
+            rotate: int = 0,
+            savepath: str = None,
+            default_assignment: np.ndarray = None) -> dict:
     '''
     Create a tkinter GUI to select noise components from ica-decomposition components file.
+    If hdf5 information is given using a string input to components, or a savepath which is a valid hdf5 file,
+    component artifact assignment will be saved to the file.
 
     Returns toggle, a boolean array 
     of either True or False.  Components that have been determined to be 
     noise are 'True', components to keep are 'False'.
     Optional toggle input is a boolean of starting values 
     for noise_components.
+
+    Arguments:
+        components: A dictionary containing the experiment and decomposition information.
+        rotate: An integer number of counterclockwise rotations.
+        savepath: Where to save or load component information from.
+        default_assignment: The default assignment of which components are signal or artifact.
+
+    Returns:
+        components: The components dict, updated with any new region assignment, or artifact assignment, if applicable. 
     '''
 
     print('\nStarting ICA Component Selection GUI\n-----------------------')
     print(
         'If you experience problems with this GUI, check your tk version with the following terminal command:'
     )
     print('\tpython -m tkinter')
@@ -51,37 +65,37 @@
 
     if savepath is not None:
         f = hdf5manager(savepath)
         load_hdf5 = True
 
     assert type(components) is dict, 'Components were not in expected format'
 
-    # load all components from dict
+    # Load all components from dict.
     eig_vec = components['eig_vec']
     if 'thresholds' in components.keys():
         thresholds = components['thresholds']
     roimask = components['roimask']
     shape = components['shape']
     t, x, y = shape
     eigb_shape = (x, y)
 
-    # Find number of components
+    # Find number of components.
     n_components = eig_vec.shape[1]
     print('number of components:', n_components)
 
-    # start timecourses variable for storing rebuilt timecourses of PCs
+    # Start timecourses variable for storing rebuilt timecourses of components.
     if 'timecourses' in components:
         print('timecourses found')
         timecourses = components['timecourses']
     else:
         print('timecourses not found in components')
         print('Initializing empty timecourse vector')
         timecourses = components['timecourses']
 
-    # start noise_components variable for listing which components are noise
+    # Start noise_components variable for listing which components are noise.
     if ('noise_components' in components) and ('cutoff' in components):
         noise_components = components['noise_components']
         cutoff = components['cutoff']
     else:
         print('calculating noise components...')
         noise_components, cutoff = sort_noise(timecourses)
     maxval = np.argmax(noise_components == 1)
@@ -89,16 +103,16 @@
     if 'lag1_full' in components:
         lag1 = components['lag1_full']
         _, _, log_pdf = sort_noise(timecourses, lag1=lag1, return_logpdf=True)
     else:
         lag1 = lag_n_autocorr(timecourses, 1, verbose=False)
         _, _, log_pdf = sort_noise(timecourses, return_logpdf=True)
 
-    # start toggle variable for checking which components shouldn't
-    # be included
+    # Start toggle variable for checking which components shouldn't
+    # be included.
     if 'artifact_components' in components:
         toggle = components['artifact_components']
     else:
         print('initializing artifact_components toggle')
         toggle = np.zeros((n_components,), dtype='uint8')
 
     if 'flipped' in components:
@@ -127,59 +141,57 @@
                         default_assignment))
             else:
                 region_assignment[:] = np.nan
     else:
         print('domain_ROIs not found')
         domain_ROIs = None
 
-    # Load mask indexing for faster rebuilding of eigenbrains
+    # Load mask indexing for faster rebuilding of eigenbrains.
     if roimask is not None:
         maskind = np.where(roimask.flat == 1)
     else:
         maskind = None
 
     region_cm = config['colormap']['domains']
     component_cmap = config['colormap']['components']
     corr_cmap = config['colormap']['correlation']
 
     regions = config['regions']
 
-    # convert from defaults dict to sorted list of tuples
+    # Convert from defaults dict to sorted list of tuples.
     keylist = []
     valuelist = []
 
     for key in regions:
-        # print(key, regions[key])
         keylist.append(key)
         valuelist.append(regions[key])
 
     sortindex = [i[0] for i in sorted(enumerate(valuelist), key=lambda x: x[1])]
 
     regions = []
     for i in sortindex:
         regions.append((keylist[i], valuelist[i]))
 
-    # general font settings
     LARGE_FONT = ('Verdana', 12)
 
-    togglesave = [True]  # default on for easy click-to-save figures
-    toggledebug = [False]  # default off -- don't load ICA pixel properties
+    toggle_save = [True]  # Default on for easy click-to-save figures.
+    toggle_debug = [False]  # Default off -- don't load ICA pixel properties.
 
-    def saveFigure(fig_handle):
+    def save_figure(fig_handle):
         print('figure was pressed!')
-        # callback for clicks on image.
-        # Change color and toggle value
+        # Callback for clicks on image.
+        # Change color and toggle value.
 
-        if togglesave[0]:
+        if toggle_save[0]:
             print('trying to save..')
             file_path = tk.filedialog.asksaveasfilename()
             print(file_path)
 
-            if type(file_path) is str:  # If path was provided
-                # If there was no extension, add .png
+            if type(file_path) is str:  # If path was provided.
+                # If there was no extension, add .png.
                 if os.path.splitext(file_path)[1] == '':
                     file_path += '.png'
 
                 if os.path.isfile(file_path):
                     print('file already exists!')
                     yn = tk.messagebox.askquestion(
                         'Overwriting File',
@@ -197,94 +209,97 @@
                     fig_handle.savefig(file_path)
                     print('File saved to:', file_path)
             else:
                 print('No file selected')
         else:
             print('Saving functionality is turned off')
 
-    # Create main application as tk.Tk
-    class PCAgui(tk.Tk):  #<- inherits from Tk class
+    # Create main application as tk.Tk.
+    class AnalysisGui(tk.Tk):  # Note: Inherits from Tk class.
 
         def __init__(self, *args, **kwargs):
-            tk.Tk.__init__(self, *args, **kwargs)  # initialize the tk class
+            tk.Tk.__init__(self, *args,
+                           **kwargs)  # Initialize the parent tk class.
             tk.Tk.wm_title(self, 'Component Viewer')
-            # every page initializes a container to hold its content
+            # Every page initializes a container to hold its content.
             container = tk.Frame(self)
             container.pack(side='top', fill='both', expand=True)
 
-            # set page expansion properties
+            # Set page expansion properties.
             container.grid_rowconfigure(0, weight=1)
-            # row/columns expand equally
+            # Row/columns expand equally.
             container.grid_columnconfigure(0, weight=1)
 
-            # Make the menu bar (top banner)
+            # Make the menu bar (top banner).
             menubar = tk.Menu(container)
 
             filemenu = tk.Menu(menubar, tearoff=0)
             filemenu.add_separator()
             filemenu.add_command(label='save', command=self.quit)
             filemenu.add_command(label='exit',
                                  command=lambda: self.cancelcallback(toggle))
             menubar.add_cascade(label='file', menu=filemenu)
 
-            def toggleFigSaving():
-                togglesave[0] = not togglesave[0]
+            def toggle_figure_saving():
+                toggle_save[0] = not toggle_save[0]
 
-            def toggleIcaDebug():
-                toggledebug[0] = not toggledebug[0]
+            def toggle_figure_saving():
+                toggle_debug[0] = not toggle_debug[0]
 
             editmenu = tk.Menu(menubar, tearoff=0)
             editmenu.add_separator()
             editmenu.add_command(label='toggle figure saving',
-                                 command=lambda: toggleFigSaving())
+                                 command=lambda: toggle_figure_saving())
             editmenu.add_command(label='toggle ica pixel debug',
-                                 command=lambda: toggleIcaDebug())
+                                 command=lambda: toggle_ica_debug())
             menubar.add_cascade(label='edit', menu=editmenu)
 
             pagemenu = tk.Menu(menubar, tearoff=1)
             pagemenu.add_separator()
             pagemenu.add_command(label='view components',
-                                 command=lambda: self.show_frame(PCpage))
-            pagemenu.add_command(label='PC information',
-                                 command=lambda: self.show_frame(PCinfo))
+                                 command=lambda: self.show_frame(ComponentPage))
+            pagemenu.add_command(label='Component information',
+                                 command=lambda: self.show_frame(ComponentInfo))
             pagemenu.add_command(label='Domain Correlations',
                                  command=lambda: self.show_frame(DomainROIs))
             pagemenu.add_command(label='Domain Region Assignment',
                                  command=lambda: self.show_frame(DomainRegions))
-            pagemenu.add_command(label='Domain Autocorrelations',
-                                 command=lambda: self.show_frame(PCautocorr))
+            pagemenu.add_command(
+                label='Domain Autocorrelations',
+                command=lambda: self.show_frame(DomainAutoCorr))
             menubar.add_cascade(label='view', menu=pagemenu)
 
             tk.Tk.config(self, menu=menubar)
 
-            # Create container to hold for all pages for page switching
+            # Create container to hold for all pages for page switching.
             self.frames = {}
 
             # List all pages here:
-            for F in (PCpage, PCinfo, DomainROIs, DomainRegions, PCautocorr):
+            for F in (ComponentPage, ComponentInfo, DomainROIs, DomainRegions,
+                      DomainAutoCorr):
                 frame = F(container, self)
                 self.frames[F] = frame
                 # set currently active frame to StartPage
                 frame.grid(row=0, column=0, sticky='nsew')
 
-            # Initialize default page
-            default_page = PCpage
+            # Initialize default page.
+            default_page = ComponentPage
             self.show_frame(default_page)
 
-            # Global event binding commands
+            # Global event binding commands.
             self.bind("<Escape>", lambda event: self.cancelcallback(toggle))
             self.bind("s", lambda event: self.quit())
-            self.bind("<F1>", lambda event: self.show_frame(PCpage))
-            self.bind("<F2>", lambda event: self.show_frame(PCinfo))
+            self.bind("<F1>", lambda event: self.show_frame(ComponentPage))
+            self.bind("<F2>", lambda event: self.show_frame(ComponentInfo))
             self.bind("<F3>", lambda event: self.show_frame(DomainROIs))
             self.bind("<F4>", lambda event: self.show_frame(DomainRegions))
-            self.bind("<F5>", lambda event: self.show_frame(PCautocorr))
+            self.bind("<F5>", lambda event: self.show_frame(DomainAutoCorr))
 
             # Use global focus to capture bindings,
-            # send them to local callback manager
+            # send them to local callback manager.
             self.bind("<Right>",
                       lambda event: self.current_page.callback_manager(event))
             self.bind("<Left>",
                       lambda event: self.current_page.callback_manager(event))
             self.bind("<Up>",
                       lambda event: self.current_page.callback_manager(event))
             self.bind("<Down>",
@@ -292,138 +307,142 @@
 
             # When window is closed, cancel and don't save results.
             self.protocol('WM_DELETE_WINDOW',
                           lambda: self.cancelcallback(toggle))
 
         # Methods for main app:
         def show_frame(self, cont):
-            # selects frame, raises it
+            # Selects frame, raises it.
             frame = self.frames[cont]
             self.current_page = frame
             frame.tkraise()
 
         def cancelcallback(self, toggle):
-            # quits the app, doesn't rebuild the movie
+            # Quits the app, doesn't rebuild the movie.
             print('Operation was cancelled.')
             toggle[0] = 100
             self.quit()
 
     # Create each frame and components as individual classes:
-    class PCpage(tk.Frame):
-        # Page to view all principal component images, toggle via clicks
+    class ComponentPage(tk.Frame):
+        # Page to view all principal component images, toggle via clicks.
 
         def __init__(self, parent, controller):
-            tk.Frame.__init__(self, parent)  # parent is controller
+            tk.Frame.__init__(self, parent)  # Parent is controller.
 
-            # Create frame for PCs, initialize PC indices
-            self.nimages = 15
-            self.PCpage = 0
+            # Create frame for each component, initialize component indices.
+            self.n_images = 15
+            self.current_page_number = 0
 
-            # initialize the title
+            # Initialize the title.
             label = tk.Label(self,
                              text='Select Components to Remove:',
                              font=LARGE_FONT)
 
-            # initialize navigation buttons
+            # Initialize navigation buttons.
             navbuttons = tk.Frame(self)
-            self.llbutton = tk.Button(
-                navbuttons,
-                text='<<< {0} PCs'.format(4 * self.nimages),
-                command=lambda: self.changePCpage(self.PCpage - 4))
-            self.lbutton = tk.Button(
-                navbuttons,
-                text='<<< {0} PCs'.format(self.nimages),
-                command=lambda: self.changePCpage(self.PCpage - 1))
-            self.homebutton = tk.Button(navbuttons,
-                                        text='Home',
-                                        command=lambda: self.changePCpage(0))
-            self.rbutton = tk.Button(
+            self.llbutton = tk.Button(navbuttons,
+                                      text='<<< {0} PCs'.format(4 *
+                                                                self.n_images),
+                                      command=lambda: self.changeComponentPage(
+                                          self.current_page_number - 4))
+            self.lbutton = tk.Button(navbuttons,
+                                     text='<<< {0} PCs'.format(self.n_images),
+                                     command=lambda: self.changeComponentPage(
+                                         self.current_page_number - 1))
+            self.homebutton = tk.Button(
                 navbuttons,
-                text='{0} PCs >>>'.format(self.nimages),
-                command=lambda: self.changePCpage(self.PCpage + 1))
-            self.rrbutton = tk.Button(
-                navbuttons,
-                text='{0} PCs >>>'.format(4 * self.nimages),
-                command=lambda: self.changePCpage(self.PCpage + 4))
+                text='Home',
+                command=lambda: self.changeComponentPage(0))
+            self.rbutton = tk.Button(navbuttons,
+                                     text='{0} PCs >>>'.format(self.n_images),
+                                     command=lambda: self.changeComponentPage(
+                                         self.current_page_number + 1))
+            self.rrbutton = tk.Button(navbuttons,
+                                      text='{0} PCs >>>'.format(4 *
+                                                                self.n_images),
+                                      command=lambda: self.changeComponentPage(
+                                          self.current_page_number + 4))
 
-            # Make frame for pc max value controller
+            # Make frame for pc max value controller.
             pccontrol = tk.Frame(self)
             upper_limit = tk.StringVar()
             upper_limit.set(str(maxval))
             maxentry = tk.Entry(pccontrol, textvariable=upper_limit, width=5)
             entrylabel = tk.Label(pccontrol, text='Noise Floor:')
 
-            # place the title
+            # Place the title.
             label.grid(column=0, row=0)
 
-            # place the navigation buttons and load panel
+            # Place the navigation buttons and load panel.
             self.llbutton.grid(column=0, row=0)
             self.lbutton.grid(column=1, row=0)
             self.homebutton.grid(column=2, row=0)
             self.rbutton.grid(column=3, row=0)
             self.rrbutton.grid(column=4, row=0)
             navbuttons.grid(column=0, row=2)
 
-            # place max pc control panel
+            # Place max pc control panel.
             entrylabel.grid(column=0, row=0)
             maxentry.grid(column=1, row=0)
             pccontrol.grid(column=0, row=3)
 
-            self.loadPCpage()
+            self.loadComponentPage()
 
         def callback_manager(self, event):
             if event.keysym == 'Right':
-                if len(toggle) - self.nimages * (self.PCpage + 1) > 0:
-                    self.changePCpage(self.PCpage + 1)
+                if len(toggle) - self.n_images * (self.current_page_number +
+                                                  1) > 0:
+                    self.changeComponentPage(self.current_page_number + 1)
             elif event.keysym == 'Left':
-                if self.PCpage != 0:
-                    self.changePCpage(self.PCpage - 1)
+                if self.current_page_number != 0:
+                    self.changeComponentPage(self.current_page_number - 1)
             else:
                 print('No callback defined for:', event.keysym)
 
-        class PCframe(tk.Frame):
-            # Create a frame to hold all eigenbrains
+        class ComponentFrame(tk.Frame):
+            # Create a frame to hold each component.
             def __init__(self, parent, indices):
                 tk.Frame.__init__(self, parent)
 
-                # variables to hold image buttons
+                # Variables to hold image buttons.
                 self.ncol = 5
                 self.PCplotframe = tk.Frame(self, borderwidth=2)
                 self.imagebutton = []
 
-                # initialize and grid image buttons
+                # Initialize and grid image buttons.
                 for i, n in enumerate(indices):
                     frame = (tk.Frame(self.PCplotframe))
                     self.imagebutton.append(self.imButton(frame, n))
                     c = i % self.ncol
                     r = i // self.ncol
                     frame.grid(row=r, column=c)
 
                 self.PCplotframe.grid(column=0, row=1)  # grid main frame
 
             def update(self, parent, indices):
-                # update each image button to contain indices given
+                # Update each image button to contain indices given.
 
                 imagebutton = self.imagebutton
 
-                #if there isn't a full set of indices, append None
+                # If there isn't a full set of indices, append None.
                 if len(indices) < len(imagebutton):
                     print('Not enough indices to fill page')
                     lendiff = len(imagebutton) - len(indices)
                     indices.extend([None] * lendiff)
 
-                # update each image with new PC index
+                # Update each image with new PC index.
                 for i, buttonhandle in enumerate(imagebutton):
                     buttonhandle.update(indices[i])
 
             class imButton(tk.Frame):
                 # Image button.  When clicked, toggle[index] is switched.
-                # Colormap is also switched to see status of PC
-                def __init__(self, parent, pc_id):
-                    self.pc_id = pc_id
+                # Colormap is also switched to see status of PC.
+                def __init__(self, parent, component_id):
+                    self.component_id = component_id
                     f = Figure(figsize=(3, 3), dpi=100, frameon=False)
                     self.ax = f.add_subplot(111)
                     f.subplots_adjust(left=0.05,
                                       bottom=0.05,
                                       right=0.98,
                                       top=0.98)
                     self.canvas = FigureCanvasTkAgg(f, parent)
@@ -431,259 +450,262 @@
                     self.canvas.mpl_connect(
                         'button_press_event',
                         lambda event: self.on_key_press(event))
 
                     self.imgplot = self.ax.imshow(np.zeros((x, y)))
                     self.ax.axis('off')
 
-                    self.update(pc_id)
+                    self.update(component_id)
 
-                def update(self, pc_id):
-                    self.pc_id = pc_id
+                def update(self, component_id):
+                    self.component_id = component_id
                     self.ax.cla()
                     self.ax.axis('off')
 
-                    if pc_id is None:  # clear image
+                    if component_id is None:  # Clear image.
                         im = np.empty((x, y))
                         im[:] = np.NAN
                         self.imgplot = self.ax.imshow(im)
                         self.canvas.draw()
                         return ()
 
-                    eigenbrain = rebuild_eigenbrain(eig_vec, pc_id, roimask,
-                                                    eigb_shape, maskind)
+                    eigenbrain = rebuild_eigenbrain(eig_vec, component_id,
+                                                    roimask, eigb_shape,
+                                                    maskind)
                     if rotate > 0:
                         eigenbrain = np.rot90(eigenbrain, rotate)
                     mean = np.nanmean(eigenbrain)
                     std = np.abs(np.nanstd(eigenbrain))
 
                     self.imgplot = self.ax.imshow(eigenbrain,
                                                   cmap=corr_cmap,
                                                   vmin=mean - 4 * std,
                                                   vmax=mean + 4 * std)
 
-                    if toggle[pc_id] == 0:
+                    if toggle[component_id] == 0:
                         self.imgplot.set_cmap(component_cmap)
                     else:
                         self.imgplot.set_cmap('Greys')
 
-                    self.ax.annotate('Component {0}'.format(pc_id),
+                    self.ax.annotate('Component {0}'.format(component_id),
                                      color='grey',
                                      fontsize=10,
                                      xy=(1, 1))
 
                     self.canvas.draw()
 
                 def on_key_press(self, event):
                     # callback for clicks on image.
-                    # Change color and toggle value
+                    # Change color and toggle value.
                     try:
-                        if toggle[self.pc_id] == 0:
+                        if toggle[self.component_id] == 0:
                             self.imgplot.set_cmap('Greys_r')
-                            toggle[self.pc_id] = 1
-                        elif toggle[self.pc_id] == 1:
+                            toggle[self.component_id] = 1
+                        elif toggle[self.component_id] == 1:
                             self.imgplot.set_cmap(component_cmap)
-                            toggle[self.pc_id] = 0
+                            toggle[self.component_id] = 0
                         self.canvas.draw()
                     except:
                         print('Index was out of range')
 
-        def changePCpage(self, newpage):
-            # callback for buttons to change page
-            self.PCpage = newpage
-            self.loadPCpage()
+        def changeComponentPage(self, newpage):
+            # Callback for buttons to change page.
+            self.current_page_number = newpage
+            self.loadComponentPage()
 
-        def loadPCpage(self):
-            # load a PC page based on self.PCpage
+        def loadComponentPage(self):
+            # Load a PC page based on self.current_page_number.
 
-            # Reenable all buttons, disable any that shouldn't be allowed
+            # Reenable all buttons, disable any that shouldn't be allowed.
             self.llbutton.config(state=['normal'])
             self.lbutton.config(state=['normal'])
             self.homebutton.config(state=['normal'])
             self.rbutton.config(state=['normal'])
             self.rrbutton.config(state=['normal'])
 
-            if self.PCpage == 0:  # if on start page, disable home, -n
+            if self.current_page_number == 0:
+                # If on start page, disable home, -n.
                 self.homebutton.config(state=['disabled'])
                 self.lbutton.config(state=['disabled'])
                 self.llbutton.config(state=['disabled'])
-            elif self.PCpage < 4:
+            elif self.current_page_number < 4:
                 self.llbutton.config(state=['disabled'])
 
-            if len(toggle) - (self.nimages * (self.PCpage + 1)) <= 0:
-                # if total images - next page's max <=0, disable + n
+            if len(toggle) - (self.n_images *
+                              (self.current_page_number + 1)) <= 0:
+                # If total images - next page's max <=0, disable + n.
                 self.rbutton.config(state=['disabled'])
                 self.rrbutton.config(state=['disabled'])
-            elif len(toggle) - self.nimages * self.PCpage \
-                    - 4*self.nimages <= 0:
+            elif len(toggle) - self.n_images * self.current_page_number \
+                    - 4*self.n_images <= 0:
                 self.rrbutton.config(state=['disabled'])
 
-            # Refresh the PC Grid
-            startPC = self.PCpage * self.nimages
-            endPC = startPC + self.nimages
+            # Refresh the PC Grid.
+            startPC = self.current_page_number * self.n_images
+            endPC = startPC + self.n_images
             if endPC > len(toggle):
                 endPC = len(toggle)
             PCindices = list(range(startPC, endPC))
             if hasattr(self, 'PCfigure'):
                 self.PCfigure.update(self, PCindices)
                 self.PCfigure.grid(column=0, row=1)
             else:
-                self.PCfigure = self.PCframe(self, PCindices)
+                self.PCfigure = self.ComponentFrame(self, PCindices)
                 self.PCfigure.grid(column=0, row=1)
-                # grid PCfigure into StartPage
+                # Grid PCfigure into StartPage.
 
-    class PCinfo(tk.Frame):
-        # Page for viewing information about individual PCs
+    class ComponentInfo(tk.Frame):
+        # Page for viewing information about individual Components.
 
         def __init__(self, parent, controller):
-            # Change the PC text box using the +/- keys.
-            # This triggers updatePCvalue to run
+            # Change the component text box using the +/- keys.
+            # This triggers update_component_index to run.
 
-            def updatePCval_button(delta):
-                newval = int(self.selected_pc.get()) + delta
-                self.selected_pc.set(newval)
-
-            # Change the PC index using the text box
-            def updatePCval():
-                newvalue = self.selected_pc.get()
-                print('Changing PC index to: {0}'.format(newvalue))
+            def update_component_index_button(delta):
+                newval = int(self.selected_component.get()) + delta
+                self.selected_component.set(newval)
+
+            # Change the component index using the text box.
+            def update_component_index():
+                newvalue = self.selected_component.get()
+                print('Changing component index to: {0}'.format(newvalue))
 
-                if newvalue == '':  # empty value
+                if newvalue == '':  # Empty value.
                     print('Text box is blank.  Not updating')
                 else:
-                    try:  # make sure entry is an int, inside range of PCs
+                    try:  # Make sure entry is an int, inside range of PCs.
                         assert int(newvalue) < n_components - 1, (
                             'Index exceeds range')
                         assert int(newvalue) >= 0, 'Index below 0'
-                        self.pc_id[0] = int(newvalue)
-                        self.selected_pc.set(str(self.pc_id[0]))
-                        fig.updateFigures(self.pc_id[0])
+                        self.component_id[0] = int(newvalue)
+                        self.selected_component.set(str(self.component_id[0]))
+                        fig.update_figures(self.component_id[0])
 
                     except:
                         print('Not changing upper PC cutoff.')
-                        self.selected_pc.set(str(self.pc_id[0]))
-                        # reset text box to previous value
+                        self.selected_component.set(str(self.component_id[0]))
+                        # Reset text box to previous value.
 
-            # Initialize PC info page
+            # Initialize PC info page.
             tk.Frame.__init__(self, parent)
             label = tk.Label(self, text='Component Viewer:', font=LARGE_FONT)
             label.pack(pady=10, padx=10)
 
             # Two components to page:
-            pcviewer = tk.Frame(self)
-            # grid of figures about selected PC
-            pc_toolbar = tk.Frame(pcviewer)
-            # toolbar for selecting PC index
-
-            # Make PC selection toolbar
-            self.pc_id = [0]
-            self.selected_pc = tk.StringVar()
-            self.selected_pc.set(str(self.pc_id[0]))
-            pc_entry = tk.Entry(pc_toolbar,
-                                textvariable=self.selected_pc,
+            component_viewer_frame = tk.Frame(self)
+            # Grid of figures about selected PC.
+            current_component_toolbar = tk.Frame(component_viewer_frame)
+            # Toolbar for selecting PC index.
+
+            # Make PC selection toolbar.
+            self.component_id = [0]
+            self.selected_component = tk.StringVar()
+            self.selected_component.set(str(self.component_id[0]))
+            pc_entry = tk.Entry(current_component_toolbar,
+                                textvariable=self.selected_component,
                                 width=5)
-            self.selected_pc.trace('w',
-                                   lambda nm, idx, mode, var=0: updatePCval())
-            pc_entry_label = tk.Label(pc_toolbar, text='Component:')
+            self.selected_component.trace(
+                'w', lambda nm, idx, mode, var=0: update_component_index())
+            pc_entry_label = tk.Label(current_component_toolbar,
+                                      text='Component:')
 
-            pm_toolbar = tk.Frame(pcviewer)
+            component_adjust_toolbar = tk.Frame(component_viewer_frame)
 
-            inc = tk.Button(pm_toolbar,
+            inc = tk.Button(component_adjust_toolbar,
                             text='+',
-                            command=lambda: updatePCval_button(1))
-            dec = tk.Button(pm_toolbar,
+                            command=lambda: update_component_index_button(1))
+            dec = tk.Button(component_adjust_toolbar,
                             text='-',
-                            command=lambda: updatePCval_button(-1))
+                            command=lambda: update_component_index_button(-1))
 
-            # grid pc selector frame
+            # Grid pc selector frame.
             pc_entry_label.grid(column=0, row=0)
             pc_entry.grid(column=1, row=0)
             inc.grid(column=0, row=0)
             dec.grid(column=1, row=0)
 
-            # grid pcviewer frame
-            pc_toolbar.pack()
-            pm_toolbar.pack()
-            pcviewer.pack()
-            fig = self.PCfigures(self, self.pc_id)
+            # Grid component_viewer_frame frame.
+            current_component_toolbar.pack()
+            component_adjust_toolbar.pack()
+            component_viewer_frame.pack()
+            fig = self.ComponentFigures(self, self.component_id)
             fig.pack()
 
         def callback_manager(self, event):
             if event.keysym == 'Right':
-                newval = int(self.selected_pc.get()) + 1
-                self.selected_pc.set(newval)
+                new_component_value = int(self.selected_component.get()) + 1
+                self.selected_component.set(new_component_value)
             elif event.keysym == 'Left':
-                newval = int(self.selected_pc.get()) - 1
-                self.selected_pc.set(newval)
+                new_component_value = int(self.selected_component.get()) - 1
+                self.selected_component.set(new_component_value)
             else:
                 print('No callback defined for:', event.keysym)
 
-        class PCfigures(tk.Frame):
-            # Create class to hold and update all figures
+        class ComponentFigures(tk.Frame):
+            # Create class to hold and update all figures.
             def __init__(self, parent, controller):
 
-                # Create main frame, child of PCinfo page
+                # Create main frame, child of ComponentInfo page.
                 tk.Frame.__init__(self, parent)
 
-                ncol = 2  # number of columns of figures
+                ncol = 2  # Number of columns of figures.
                 self.figures = {}
 
-                # List desired figures
+                # List desired figures.
                 figlist = [
-                    self.pcImage, self.timeCourse, self.fourierWaveletHistogram,
-                    self.waveletSpectrum
+                    self.pcImage, self.timeCourse, self.FourierWaveletHistogram,
+                    self.WaveletSpectrum
                 ]
 
                 for i, Fig in enumerate(figlist):
-                    # Not being used: self.fourierTimecourse
-                    # self.fourierHistogram
-                    figure = Fig(self)  # initialize each figure
+                    # Not being used: self.fourierTimecourse,
+                    # self.fourierHistogram.
+                    figure = Fig(self)  # Initialize each figure.
                     c = i % ncol
                     r = i // ncol
-                    figure.grid(row=r, column=c)  # grid it
+                    figure.grid(row=r, column=c)  # Grid it.
                     self.figures[Fig] = figure
-                    # store each handle in self.figures
+                    # Store each handle in self.figures.
 
-                # initialize figures for PC #0
-                self.updateFigures(0)
+                # Initialize figures for PC #0.
+                self.update_figures(0)
 
-            def updateFigures(self, pc_id):
-                # Update all figures in self.figures
-                self.timecourse = timecourses[pc_id]
+            def update_figures(self, component_id):
+                # Update all figures in self.figures.
+                self.timecourse = timecourses[component_id]
 
-                eigenbrain = rebuild_eigenbrain(eig_vec, pc_id, roimask,
+                eigenbrain = rebuild_eigenbrain(eig_vec, component_id, roimask,
                                                 eigb_shape, maskind)
                 if rotate > 0:
                     eigenbrain = np.rot90(eigenbrain, rotate)
                 mean = np.nanmean(eigenbrain)
                 std = np.abs(np.nanstd(eigenbrain))
 
                 eigenbrain[np.where(np.isnan(eigenbrain))] = 0
                 self.eigenbrain = eigenbrain
 
-                # Wavelet analysis
+                # Wavelet analysis:
                 wavelet = waveletAnalysis(self.timecourse.astype('float64'),
                                           fps=10,
                                           siglvl=0.95)
 
-                # Dict to store all info for updating figures
-                pc_variables = {
-                    'pc_id': pc_id,
+                # Dict to store all info for updating figures.
+                component_variables = {
+                    'component_id': component_id,
                     'timecourse': self.timecourse,
                     'wavelet': wavelet
                 }
 
-                # Update all figures
-                # COMMENTHERE
+                # Update all figures.
                 for i, Fig in enumerate(self.figures):
                     handle = self.figures[Fig]
-                    handle.update(pc_variables)
+                    handle.update(component_variables)
 
             class pcImage(tk.Frame):
-                # View eigenbrain (same as PCpage figures)
+                # View eigenbrain (same as ComponentPage figures).
                 def __init__(self, parent):
                     tk.Frame.__init__(self, parent)
 
                     frame = tk.Frame(self)
                     f = Figure(figsize=(4, 4), dpi=100, frameon=False)
                     self.fig = f
                     self.ax = f.add_subplot(111)
@@ -696,37 +718,38 @@
                         lambda event: self.on_key_press(event))
                     self.canvas.draw()
                     self.canvas.get_tk_widget().pack()
                     frame.pack()
 
                 def on_key_press(self, event):
                     if event.button == 3:
-                        saveFigure(self.fig)
+                        save_figure(self.fig)
 
-                def update(self, pc_variables):
-                    pc_id = pc_variables['pc_id']
+                def update(self, component_variables):
+                    component_id = component_variables['component_id']
                     self.ax.cla()
 
-                    eigenbrain = rebuild_eigenbrain(eig_vec, pc_id, roimask,
-                                                    eigb_shape, maskind)
+                    eigenbrain = rebuild_eigenbrain(eig_vec, component_id,
+                                                    roimask, eigb_shape,
+                                                    maskind)
                     if rotate > 0:
                         eigenbrain = np.rot90(eigenbrain, rotate)
                     mean = np.nanmean(eigenbrain)
                     std = np.abs(np.nanstd(eigenbrain))
 
                     self.imgplot = self.ax.imshow(eigenbrain,
                                                   cmap=component_cmap,
                                                   vmin=mean - 4 * std,
                                                   vmax=mean + 4 * std)
 
                     self.ax.axis('off')
                     self.canvas.draw()
 
             class timeCourse(tk.Frame):
-                # view timecourse of PC
+                # View component timecourse.
                 def __init__(self, parent):
                     tk.Frame.__init__(self, parent)
 
                     frame = tk.Frame(self)
                     f = Figure(figsize=(4, 4), dpi=100, frameon=False)
                     self.fig = f
                     self.ax = f.add_subplot(111)
@@ -744,25 +767,25 @@
                         lambda event: self.on_key_press(event))
                     self.canvas.draw()
                     self.canvas.get_tk_widget().pack()
                     frame.pack()
 
                 def on_key_press(self, event):
                     if event.button == 3:
-                        saveFigure(self.fig)
+                        save_figure(self.fig)
 
-                def update(self, pc_variables):
-                    timecourse = pc_variables['timecourse']
+                def update(self, component_variables):
+                    timecourse = component_variables['timecourse']
                     self.ax.lines.pop(0)
                     self.ax.plot(
                         np.arange(timecourse.size) / 10, timecourse, 'k')
                     self.canvas.draw()
 
             class timeCoursePCxCorr(tk.Frame):
-                # view correlation between this PC and others
+                # View correlation between this PC and others.
                 def __init__(self, parent):
                     tk.Frame.__init__(self, parent)
 
                     frame = tk.Frame(self)
                     f = Figure(figsize=(4, 4), dpi=100, frameon=False)
                     self.fig = f
                     self.ax = f.add_subplot(111)
@@ -780,34 +803,34 @@
                         lambda event: self.on_key_press(event))
                     self.canvas.draw()
                     self.canvas.get_tk_widget().pack()
                     frame.pack()
 
                 def on_key_press(self, event):
                     if event.button == 3:
-                        saveFigure(self.fig)
+                        save_figure(self.fig)
 
-                def update(self, pc_variables):
-                    pc_id = pc_variables['pc_id']
-                    print('loading correlations for component #', pc_id)
-                    correlation = timecourses[pc_id]
+                def update(self, component_variables):
+                    component_id = component_variables['component_id']
+                    print('loading correlations for component #', component_id)
+                    correlation = timecourses[component_id]
 
                     temp = np.copy(correlation)
-                    temp[pc_id] = 0
+                    temp[component_id] = 0
                     temp[-1] = 0
                     ylim = np.std(temp)
 
                     self.ax.lines.pop(0)
                     self.ax.plot(correlation, 'k')
                     self.ax.set_ylim([-3 * ylim, 3 * ylim])
                     self.canvas.draw()
 
             class fourierTimecourse(tk.Frame):
-                # Look at the Windowed Fourier Transform of the
-                # PC timecourse
+                # Look at the windowed fourier transform of the
+                # component timecourse.
                 def __init__(self, parent):
                     tk.Frame.__init__(self, parent)
 
                     frame = tk.Frame(self)
                     f = Figure(figsize=(4, 4), dpi=100, frameon=False)
                     self.ax = f.add_subplot(111)
                     f.subplots_adjust(left=0.2,
@@ -821,18 +844,18 @@
                         lambda event: self.on_key_press(event))
                     self.canvas.draw()
                     self.canvas.get_tk_widget().pack()
                     frame.pack()
 
                 def on_key_press(self, event):
                     if event.button == 3:
-                        saveFigure(self.fig)
+                        save_figure(self.fig)
 
-                def update(self, pc_variables):
-                    timecourse = pc_variables['timecourse']
+                def update(self, component_variables):
+                    timecourse = component_variables['timecourse']
                     timecourse = timecourse - timecourse.mean()
                     stft, fps, nyq, maxData = short_time_fourier_transform(
                         timecourse)
 
                     self.ax.cla()
                     self.ax.imshow(stft,
                                    cmap='jet',
@@ -842,60 +865,59 @@
                                    clim=(0.0, maxData / 6))
                     self.ax.set_title('Sliding Fourier Transform')
                     self.ax.set_xlabel('Time (sec)')
                     self.ax.set_ylabel('Frequency (Hz)')
                     self.canvas.draw()
 
             class fourierHistogram(tk.Frame):
-                # Look at the power histogram of the Windowed
-                # Fourier Transform
+                # Look at the power histogram of the windowed
+                # fourier transform.
                 def __init__(self, parent):
                     tk.Frame.__init__(self, parent)
 
                     frame = tk.Frame(self)
                     f = Figure(figsize=(4, 4), dpi=100, frameon=False)
                     self.fig = f
                     self.ax = f.add_subplot(111)
                     f.subplots_adjust(left=0.2,
                                       bottom=0.15,
                                       right=0.85,
                                       top=0.85)
                     self.ax.plot([])
-                    # self.ax.set_xlim([0, 5])
                     self.ax.set_xlabel('Frequency (Hz)')
                     self.ax.set_ylabel('Normalized Power')
                     self.ax.set_title('Fourier Histogram')
                     self.canvas = FigureCanvasTkAgg(f, frame)
                     self.canvas.mpl_connect(
                         'button_press_event',
                         lambda event: self.on_key_press(event))
                     self.canvas.draw()
                     self.canvas.get_tk_widget().pack()
                     frame.pack()
 
                 def on_key_press(self, event):
                     if event.button == 3:
-                        saveFigure(self.fig)
+                        save_figure(self.fig)
 
-                def update(self, pc_variables):
-                    timecourse = pc_variables['timecourse']
+                def update(self, component_variables):
+                    timecourse = component_variables['timecourse']
                     timecourse = timecourse - timecourse.mean()
                     stft, fps, nyq, maxData = short_time_fourier_transform(
                         timecourse)
 
                     stfthist = stft.sum(1)
                     self.ax.lines.pop(0)
                     self.ax.plot((np.arange(stfthist.size) / 10)[::-1],
                                  stfthist, 'k')
                     self.ax.set_yscale('log')
                     self.canvas.draw()
 
-            class fourierWaveletHistogram(tk.Frame):
-                # Look at the power histogram of the Windowed
-                # Fourier Transform
+            class FourierWaveletHistogram(tk.Frame):
+                # Look at the power histogram of the windowed
+                # fourier transform.
                 def __init__(self, parent):
                     tk.Frame.__init__(self, parent)
 
                     frame = tk.Frame(self)
                     f = Figure(figsize=(4, 4), dpi=100, frameon=False)
                     self.fig = f
                     self.ax1 = f.add_subplot(111)
@@ -921,25 +943,25 @@
                         lambda event: self.on_key_press(event))
                     self.canvas.draw()
                     self.canvas.get_tk_widget().pack()
                     frame.pack()
 
                 def on_key_press(self, event):
                     if event.button == 3:
-                        saveFigure(self.fig)
+                        save_figure(self.fig)
 
-                def update(self, pc_variables):
+                def update(self, component_variables):
                     linetype = ['-', '-.', '--', ':']
-                    timecourse = pc_variables['timecourse']
+                    timecourse = component_variables['timecourse']
                     timecourse = timecourse - timecourse.mean()
                     stft, fps, nyq, maxData = short_time_fourier_transform(
                         timecourse)
                     stfthist = stft.sum(1)
 
-                    wavelet = pc_variables['wavelet']
+                    wavelet = component_variables['wavelet']
                     wavelet.globalWaveletSpectrum()
 
                     for i in range(len(self.ax1.lines)):
                         self.ax1.lines.pop(0)
                     for i in range(len(self.ax2.lines)):
                         self.ax2.lines.pop(0)
                     # self.ax2.cla()
@@ -957,16 +979,16 @@
                     self.ax2.plot(freq, stfthist, 'b')
                     self.ax2.set_yscale('log')
                     self.ax2.set_ylim([a, b])
                     self.ax2.set_xlim([0, 5])
 
                     self.canvas.draw()
 
-            class waveletSpectrum(tk.Frame):
-                # View wavelet power spectrum
+            class WaveletSpectrum(tk.Frame):
+                # View wavelet power spectrum.
                 def __init__(self, parent):
                     tk.Frame.__init__(self, parent)
 
                     frame = tk.Frame(self)
                     f = Figure(figsize=(4, 4), dpi=100, frameon=False)
                     self.fig = f
                     self.ax = f.add_subplot(111)
@@ -981,137 +1003,137 @@
                         lambda event: self.on_key_press(event))
                     self.canvas.draw()
                     self.canvas.get_tk_widget().pack()
                     frame.pack()
 
                 def on_key_press(self, event):
                     if event.button == 3:
-                        saveFigure(self.fig)
+                        save_figure(self.fig)
 
-                def update(self, pc_variables):
-                    wavelet = pc_variables['wavelet']
+                def update(self, component_variables):
+                    wavelet = component_variables['wavelet']
                     self.ax.cla()
                     wavelet.plotPower(ax=self.ax)
                     self.canvas.draw()
 
     class DomainROIs(tk.Frame):
-        # Page for viewing information about functional correlation of ICA domains
+        # Page for viewing information about functional correlation of ICA domains.
 
         def __init__(self, parent, controller):
 
             # Change the PC text box using the +/- keys.
-            # This triggers updatePCvalue to run
-            def updatePCval_button(delta):
-                newval = int(self.selected_pc.get()) + delta
-                self.selected_pc.set(newval)
-
-            # Change the PC index using the text box
-            def updatePCval():
-                newvalue = self.selected_pc.get()
+            # This triggers update_component_index to run.
+            def update_component_index_button(delta):
+                newval = int(self.selected_component.get()) + delta
+                self.selected_component.set(newval)
+
+            # Change the PC index using the text box.
+            def update_component_index():
+                newvalue = self.selected_component.get()
                 print('\nChanging component index to: {0}'.format(newvalue))
 
-                if newvalue == '':  # empty value
+                if newvalue == '':  # Empty value.
                     print('Text box is blank.  Not updating')
                 else:
-                    try:  # make sure entry is an int, inside range of PCs
+                    try:  # Make sure entry is an int, inside range of PCs.
                         assert int(newvalue) < n_components - 1, (
                             'Index exceeds range')
                         assert int(newvalue) >= 0, 'Index below 0'
-                        self.pc_id[0] = int(newvalue)
-                        self.selected_pc.set(str(self.pc_id[0]))
-                        fig.updateFigures(self.pc_id[0])
+                        self.component_id[0] = int(newvalue)
+                        self.selected_component.set(str(self.component_id[0]))
+                        fig.update_figures(self.component_id[0])
 
                     except Exception as e:
                         print('Error!')
                         print('\t', e)
                         print('Not changing upper PC cutoff.')
-                        self.selected_pc.set(str(self.pc_id[0]))
-                        # reset text box to previous value
+                        self.selected_component.set(str(self.component_id[0]))
+                        # Reset text box to previous value.
 
-            # Initialize PC info page
+            # Initialize PC info page.
             tk.Frame.__init__(self, parent)
             label = tk.Label(self, text='Domain ROI Viewer:', font=LARGE_FONT)
             label.pack(pady=10, padx=10)
 
             # Two components to page:
             domain_viewer = tk.Frame(self)
-            # grid of figures about selected PC
-            pc_toolbar = tk.Frame(domain_viewer)
+            # Grid of figures about selected PC.
+            current_component_toolbar = tk.Frame(domain_viewer)
             # toolbar for selecting PC index
 
-            # Make PC selection toolbar
-            self.pc_id = [0]
-            self.selected_pc = tk.StringVar()
-            self.selected_pc.set(str(self.pc_id[0]))
-            pc_entry = tk.Entry(pc_toolbar,
-                                textvariable=self.selected_pc,
+            # Make PC selection toolbar.
+            self.component_id = [0]
+            self.selected_component = tk.StringVar()
+            self.selected_component.set(str(self.component_id[0]))
+            pc_entry = tk.Entry(current_component_toolbar,
+                                textvariable=self.selected_component,
                                 width=5)
-            self.selected_pc.trace('w',
-                                   lambda nm, idx, mode, var=0: updatePCval())
-            pc_entry_label = tk.Label(pc_toolbar, text='Component ROI:')
+            self.selected_component.trace(
+                'w', lambda nm, idx, mode, var=0: update_component_index())
+            pc_entry_label = tk.Label(current_component_toolbar,
+                                      text='Component ROI:')
 
-            pm_toolbar = tk.Frame(domain_viewer)
+            component_adjust_toolbar = tk.Frame(domain_viewer)
 
-            inc = tk.Button(pm_toolbar,
+            inc = tk.Button(component_adjust_toolbar,
                             text='+',
-                            command=lambda: updatePCval_button(1))
-            dec = tk.Button(pm_toolbar,
+                            command=lambda: update_component_index_button(1))
+            dec = tk.Button(component_adjust_toolbar,
                             text='-',
-                            command=lambda: updatePCval_button(-1))
+                            command=lambda: update_component_index_button(-1))
 
-            # grid pc selector frame
+            # Grid pc selector frame.
             pc_entry_label.grid(column=0, row=0)
             pc_entry.grid(column=1, row=0)
             inc.grid(column=0, row=0)
             dec.grid(column=1, row=0)
 
-            # grid domain_viewer frame
-            pc_toolbar.pack()
-            pm_toolbar.pack()
-            # update_noise.pack()
+            # Grid domain_viewer frame.
+            current_component_toolbar.pack()
+            component_adjust_toolbar.pack()
             domain_viewer.pack()
-            fig = self.DomainFigures(self, self.pc_id)
+            fig = self.DomainFigures(self, self.component_id)
             fig.pack()
 
         def callback_manager(self, event):
             if event.keysym == 'Right':
-                newval = int(self.selected_pc.get()) + 1
-                self.selected_pc.set(newval)
+                newval = int(self.selected_component.get()) + 1
+                self.selected_component.set(newval)
             elif event.keysym == 'Left':
-                newval = int(self.selected_pc.get()) - 1
-                self.selected_pc.set(newval)
+                newval = int(self.selected_component.get()) - 1
+                self.selected_component.set(newval)
             else:
                 print('No callback defined for:', event.keysym)
 
         class DomainFigures(tk.Frame):
-            # Create class to hold and update all figures
+            # Create class to hold and update all figures.
             def __init__(self, parent, controller):
 
-                # Create main frame, child of PCinfo page
+                # Create main frame, child of ComponentInfo page.
                 tk.Frame.__init__(self, parent)
 
-                ncol = 2  # number of columns of figures
+                ncol = 2  # Number of columns of figures.
                 self.figures = {}
 
                 figlist = [self.domain_xcorr]
 
                 for i, Fig in enumerate(figlist):
-                    # Not being used: self.fourierTimecourse
+                    # Not being used: self.fourierTimecourse.
 
-                    figure = Fig(self)  # initialize each figure
+                    figure = Fig(self)  # Initialize each figure.
                     c = i % ncol
                     r = i // ncol
-                    figure.grid(row=r, column=c)  # grid it
+                    figure.grid(row=r, column=c)  # Grid it.
                     self.figures[Fig] = figure
-                    # store each handle in self.figures
+                    # Store each handle in self.figures.
 
                 self.loaded = False
 
-            def updateFigures(self, pc_id):
-                # Update all figures in self.figures
+            def update_figures(self, component_id):
+                # Update all figures in self.figures.
                 print('\nUpdating Domain Figures...')
 
                 if not self.loaded:
 
                     if set(['domain_ROIs',
                             'ROI_timecourses']).issubset(components.keys()):
                         print('domain_ROIs found in components')
@@ -1130,35 +1152,35 @@
 
                     else:
                         print('No ROI timecourses found!')
                         self.loaded = False
                         self.domain_ROIs = None
                         self.domain_ROIs = None
                         self.xcorr = None
-                        return  # dont try updating figures.
+                        return  # Dont try updating figures.
 
                 else:
                     print('ROI information already loaded.')
 
-                corr = self.xcorr[pc_id]
+                corr = self.xcorr[component_id]
 
-                # Dict to store all info for updating figures
-                pc_variables = {
+                # Dict to store all info for updating figures.
+                component_variables = {
                     'corr': corr,
-                    'pc_id': pc_id,
+                    'component_id': component_id,
                     'domain_ROIs': self.domain_ROIs
                 }
 
-                # Update all figures
+                # Update all figures.
                 for i, Fig in enumerate(self.figures):
                     handle = self.figures[Fig]
-                    handle.update(pc_variables)
+                    handle.update(component_variables)
 
             class domain_xcorr(tk.Frame):
-                # View eigenbrain (same as PCpage figures)
+                # View eigenbrain (same as ComponentPage figures).
                 def __init__(self, parent):
                     tk.Frame.__init__(self, parent)
                     self.parent = parent
 
                     frame = tk.Frame(self)
                     f = Figure(figsize=(8, 8), dpi=100, frameon=False)
                     f.subplots_adjust(top=1,
@@ -1185,67 +1207,67 @@
                         lambda event: self.on_key_press(event))
                     self.canvas.draw()
                     self.canvas.get_tk_widget().pack()
                     frame.pack()
 
                 def on_key_press(self, event):
 
-                    if event.button == 1:  # if left click
+                    if event.button == 1:  # If left click.
                         if self.parent.loaded:
 
                             x = int(event.xdata)
                             y = int(event.ydata)
 
                             if roimask is not None:
                                 rot_roimask = np.rot90(roimask, rotate)
                                 if rot_roimask[y, x] != 1:
-                                    # if click within brain
+                                    # If click within brain.
                                     return
 
-                            pc_id = self.parent.domain_ROIs[y,
-                                                            x].astype('uint16')
+                            component_id = self.parent.domain_ROIs[y, x].astype(
+                                'uint16')
 
-                            print('pc_id:', pc_id)
-                            pc_id = pc_id
-                            self.parent.updateFigures(pc_id)
+                            print('component_id:', component_id)
+                            component_id = component_id
+                            self.parent.update_figures(component_id)
 
                     elif event.button == 3:
                         print('right click: save figure.')
-                        saveFigure(self.fig)
+                        save_figure(self.fig)
 
-                def update(self, pc_variables):
+                def update(self, component_variables):
                     print('updating xcorr...')
-                    pc_id = pc_variables['pc_id']
-                    domain_ROIs = pc_variables['domain_ROIs']
-                    corr = pc_variables['corr']
+                    component_id = component_variables['component_id']
+                    domain_ROIs = component_variables['domain_ROIs']
+                    corr = component_variables['corr']
 
                     if corr is not None:
                         print('getting map...')
 
                     else:
                         print('noise component: not displaying correlation')
 
                     self.ax.cla()
                     if self.parent.loaded:
                         frame = domain_map(domain_ROIs, values=corr)
                         self.ax.imshow(frame, vmin=-0.5, vmax=1, cmap=corr_cmap)
                     else:
                         frame = domain_map(domain_ROIs)
                         self.ax.imshow(frame, vmin=-0.5, vmax=1, cmap='gray')
-                    self.ax.set_title('PC' + str(pc_id) +
+                    self.ax.set_title('PC' + str(component_id) +
                                       ': Domain Correlation')
                     self.ax.axis('off')
                     self.canvas.draw()
 
     class DomainRegions(tk.Frame):
-        # Page for assigning regions of ICA domains
+        # Page for assigning regions of ICA domains.
 
         def __init__(self, parent, controller):
 
-            # Initialize PC info page
+            # Initialize page.
             tk.Frame.__init__(self, parent)
             label = tk.Label(self,
                              text='Domain Region Assignment:',
                              font=LARGE_FONT)
             label.pack(pady=10, padx=10)
 
             self.selected_region = tk.StringVar()
@@ -1287,15 +1309,15 @@
                 if regionkey > 1:
                     self.selected_region.set(str(regionkey - 1))
 
             else:
                 print('No callback defined for:', event.keysym)
 
         class region_assignment_page(tk.Frame):
-            # View eigenbrain (same as PCpage figures)
+            # View component (same as ComponentPage figures).
             def __init__(self, parent, entryvar):
                 tk.Frame.__init__(self, parent)
                 self.entryvar = entryvar
 
                 frame = tk.Frame(self)
                 f = Figure(figsize=(9, 9), dpi=100, frameon=False)
                 f.subplots_adjust(top=1,
@@ -1327,156 +1349,154 @@
                     self.loaded = True
                     self.update()
                 else:
                     self.loaded = False
 
             def on_key_press(self, event):
 
-                if event.button == 1:  # if left click
+                if event.button == 1:  # If left click.
 
                     region = self.entryvar.get()
                     if (region != '') and self.loaded:
 
                         x = int(event.xdata)
                         y = int(event.ydata)
 
                         if roimask is not None:
                             rot_roimask = np.rot90(roimask, rotate)
                             if rot_roimask[y, x] != 1:
-                                # if click within brain
+                                # If click within brain.
                                 return
 
-                        pc_id = domain_ROIs[y, x].astype('uint16')
+                        component_id = domain_ROIs[y, x].astype('uint16')
 
-                        print('clicked on id:', pc_id)
-                        ind = np.where(domain_ROIs == pc_id)
-                        region_assignment[pc_id] = float(region)
+                        print('clicked on id:', component_id)
+                        ind = np.where(domain_ROIs == component_id)
+                        region_assignment[component_id] = float(region)
                         self.dmap[ind] = float(region)
 
                         self.update()
 
                 elif event.button == 3:
                     print('right click: save figure.')
-                    saveFigure(self.fig)
+                    save_figure(self.fig)
 
             def update(self):
                 if self.loaded:
                     print('updating!')
                     self.ax.cla()
                     self.ax.imshow(self.dmap, cmap=region_cm, vmin=1, vmax=6)
                     self.ax.imshow(self.edges, vmin=0, vmax=2, cmap='binary')
                     self.ax.axis('off')
                     self.canvas.draw()
                 else:
                     print('data not loaded.  not updating.')
 
-    class PCautocorr(tk.Frame):
-        # Page for viewing statistical information about the PC projection
+    class DomainAutoCorr(tk.Frame):
+        # Page for viewing statistical information about the PC projection.
         def __init__(self, parent, controller):
 
-            # Initialize Stats Info page
+            # Initialize Stats Info page.
             tk.Frame.__init__(self, parent)
             label = tk.Label(self,
                              text='Autocorrelation Viewer:',
                              font=LARGE_FONT)
             label.pack(pady=10, padx=10)
 
-            # Make frame for pc max value controller
-            self.xlim_max = [maxval]  # maximum x limit for figures
+            # Make frame for pc max value controller.
+            self.xlim_max = [maxval]  # Maximum x limit for figures.
             self.xlim_min = [0]
             pc_control = tk.Frame(self)
             pc_adjust = tk.Frame(pc_control)
 
-            # initialize min and max controllers
+            # Initialize min and max controllers.
             self.upper_limit = tk.StringVar()
             self.upper_limit.set(str(self.xlim_max[0]))
             self.upper_limit.trace(
                 'w',
                 lambda nm, idx, mode, var=self.upper_limit: self.updatemaxval())
 
             self.lower_limit = tk.StringVar()
             self.lower_limit.set(str(self.xlim_min[0]))
-            self.lower_limit.trace(
-                'w',
-                lambda nm, idx, mode, var=self.lower_limit: self.updateminval())
+            self.lower_limit.trace('w',
+                                   lambda nm, idx, mode, var=self.lower_limit:
+                                   self.update_min_val())
 
-            # horizontally pack label, pc_adjust into control vertically
+            # Horizontally pack label, pc_adjust into control vertically.
             tk.Label(pc_control, text='PC axes:').pack()
 
-            # pack elements in pc_adjust horizontally
+            # Pack elements in pc_adjust horizontally.
             tk.Label(pc_adjust, text='from').pack(side=tk.LEFT)
             tk.Entry(pc_adjust, textvariable=self.lower_limit,
                      width=5).pack(side=tk.LEFT)
             tk.Label(pc_adjust, text='to').pack(side=tk.LEFT)
             tk.Entry(pc_adjust, textvariable=self.upper_limit,
                      width=5).pack(side=tk.LEFT)
 
             pc_adjust.pack()
             pc_control.pack()
 
-            # statistics figures
+            # Statistics figures.
             fig_grid = tk.Frame(self)
             self.statsviewer = self.AutoCorr(fig_grid)
             self.statsviewer.grid(row=0, column=0)
 
             fig_grid.pack()
 
         def updatemaxval(self):
             # Update the maximum principal component to be
-            # included from textbox
+            # included from textbox.
             xlim_min = self.xlim_min
             xlim_max = self.xlim_max
             newvalue = self.upper_limit.get()
             print('Changing upper PC cutoff to: {0}'.format(newvalue))
 
-            if newvalue == '':  # if blank, don't reset value
+            if newvalue == '':  # If blank, don't reset value.
                 self.upper_limit.set('')
             else:
                 try:
                     assert int(
                         newvalue) <= n_components - 1, 'Index exceeds range'
                     assert int(newvalue) > xlim_min[0], 'Max index below min'
                     self.xlim_max[0] = int(newvalue)
-                    self.updateFigures(xlim_min[0], xlim_max[0])
-                except:  # not a valid number, reset to previous value
+                    self.update_figures(xlim_min[0], xlim_max[0])
+                except:  # Not a valid number, reset to previous value.
                     print('Not changing upper PC cutoff.')
-                    # self.upper_limit.set(xlim_max[0])
                     print('upper limit before', self.upper_limit.get())
                     self.upper_limit.set(str(xlim_max[0]))
                     print('upper limit after', self.upper_limit.get())
-                    # self.upper_limit.set('x')
 
-        def updateminval(self):
-            # Update the minimum principal component to be
-            # included from textbox
+        def update_min_val(self):
+            # Update the minimum component id to be
+            # included from textbox.
             xlim_min = self.xlim_min
             xlim_max = self.xlim_max
             newvalue = self.lower_limit.get()
             print('Changing lower PC cutoff to: {0}'.format(newvalue))
 
-            if newvalue == '':  # if blank, don't reset value
+            if newvalue == '':  # If blank, don't reset value.
                 self.lower_limit.set('x')
             else:
                 try:
                     assert int(newvalue) < xlim_max[0], 'Index exceeds maximum'
                     assert int(newvalue) >= 0, 'Min index below 0'
                     self.xlim_min[0] = int(newvalue)
-                    self.updateFigures(xlim_min[0], xlim_max[0])
-                except:  # not a valid number, reset to previous value
+                    self.update_figures(xlim_min[0], xlim_max[0])
+                except:  # Not a valid number, reset to previous value.
                     print('Not changing lower PC cutoff.')
                     print('lower limit before', self.lower_limit.get())
                     self.lower_limit.set('x')
                     print('lower limit after', self.lower_limit.get())
 
-        def updateFigures(self, xlim_min, xlim_max):
-            # update all figures based on limits set by text update
+        def update_figures(self, xlim_min, xlim_max):
+            # Update all figures based on limits set by text update.
             self.statsviewer.update(xlim_min, xlim_max)
 
             if type(timecourses) is np.ndarray:
-                self.pcviewer.update(xlim_min, xlim_max)
+                self.component_viewer_frame.update(xlim_min, xlim_max)
 
         def callback_manager(self, event):
             if event.keysym == 'Right':
                 newval = self.xlim_max[0] + 1
                 self.upper_limit.set(newval)
             elif event.keysym == 'Left':
                 newval = self.xlim_max[0] - 1
@@ -1487,102 +1507,132 @@
             elif event.keysym == 'Down':
                 newval = self.xlim_min[0] - 1
                 self.lower_limit.set(newval)
             else:
                 print('No callback defined for:', event.keysym)
 
         class AutoCorr(tk.Frame):
-            # View variance explained by each eigenvalue
+            # View variance explained by each 'eigenvalue'.
             def __init__(self, parent):
                 tk.Frame.__init__(self, parent)
 
-                # calculate lag autocorrelations
+                # Calculate lag autocorrelations.
                 x_grid = np.linspace(-0.2, 1.2, 1200)
 
                 frame = tk.Frame(self)
                 self.fig = Figure(figsize=(15, 8), dpi=100, frameon=False)
                 f = self.fig
 
-                self.ax = f.add_subplot(131)
+                self.ax1 = f.add_subplot(131)
                 eig_std = components['timecourses'].std(axis=1)
-                self.ax.plot(eig_std, '.r')
+                self.ax1.plot(eig_std, '.r')
                 print('cutoff:', cutoff)
-                self.ax.plot(
+                self.ax1.plot(
                     np.where(lag1[:n_components] > cutoff)[0],
                     eig_std[np.where(lag1[:n_components] > cutoff)[0]], '.b')
-                self.ax.set_xlabel('Independent Component')
-                self.ax.set_ylabel('Timecourse Standard Deviation')
+                self.ax1.set_xlabel('Independent Component')
+                self.ax1.set_ylabel('Timecourse Standard Deviation')
 
-                self.ax = f.add_subplot(132)
-                self.ax.set_ylim(-0.2, 1.2)
+                self.ax2 = f.add_subplot(132)
+                self.ax2.set_ylim(-0.2, 1.2)
                 f.subplots_adjust(left=0.2, bottom=0.15, right=0.85, top=0.85)
-                self.ax.plot(np.where(lag1 > cutoff)[0],
-                             lag1[lag1 > cutoff],
-                             'b',
-                             label='Lag-1 Signal')
-                self.ax.plot(np.where(lag1 < cutoff)[0],
-                             lag1[lag1 < cutoff],
-                             'r',
-                             label='Lag-1 Noise')
-                self.ax.set_title('PC AutoCorrelation')
-                self.ax.set_ylabel('AutoCorrelation')
-                self.ax.set_xlabel('Independent Component')
-                self.ax.legend()
-
-                self.ax = f.add_subplot(133)
-                self.ax.set_ylim(-0.2, 1.2)
-                n, _, _ = self.ax.hist(lag1, bins=50, orientation='horizontal')
-                self.ax.plot(np.exp(log_pdf) * n.max() / np.exp(log_pdf).max(),
-                             x_grid,
-                             lw=3)
+                self.ax2.plot(np.where(lag1 > cutoff)[0],
+                              lag1[lag1 > cutoff],
+                              'b',
+                              label='Lag-1 Signal')
+                self.ax2.plot(np.where(lag1 < cutoff)[0],
+                              lag1[lag1 < cutoff],
+                              'r',
+                              label='Lag-1 Noise')
+                self.ax2.set_title('Component AutoCorrelation')
+                self.ax2.set_ylabel('AutoCorrelation')
+                self.ax2.set_xlabel('Independent Component')
+                self.ax2.legend()
+
+                self.ax3 = f.add_subplot(133)
+                self.ax3.set_ylim(-0.2, 1.2)
+                n, _, _ = self.ax3.hist(lag1, bins=50, orientation='horizontal')
+                self.ax3.plot(np.exp(log_pdf) * n.max() / np.exp(log_pdf).max(),
+                              x_grid,
+                              lw=3)
                 if cutoff is not None:
-                    self.ax.axhline(cutoff, color='r', lw=3, linestyle='dashed')
-                self.ax.set_title('Lag-1 Histogram')
-                self.ax.set_xlabel('n')
+                    self.ax3.axhline(cutoff,
+                                     color='r',
+                                     lw=3,
+                                     linestyle='dashed')
+                self.ax3.set_title('Lag-1 Histogram')
+                self.ax3.set_xlabel('n')
 
                 self.canvas = FigureCanvasTkAgg(f, frame)
                 self.canvas.mpl_connect('button_press_event',
                                         lambda event: self.on_key_press(event))
                 self.canvas.draw()
                 self.canvas.get_tk_widget().pack()
                 frame.pack()
 
             def update(self, xlim_min, xlim_max):
-                self.ax.set_xlim([xlim_min, xlim_max])
+                self.ax1.set_xlim([xlim_min, xlim_max])
+                self.ax2.set_xlim([xlim_min, xlim_max])
+
+                self.ax3.cla()
+
+                if 'lag1_full' in components:
+                    lag1 = components['lag1_full']
+                    _, _, log_pdf = sort_noise(timecourses[xlim_min:xlim_max],
+                                               lag1=lag1,
+                                               return_logpdf=True)
+                else:
+                    lag1 = lag_n_autocorr(timecourses, 1, verbose=False)
+                    _, _, log_pdf = sort_noise(timecourses[xlim_min:xlim_max],
+                                               return_logpdf=True)
+
+                x_grid = np.linspace(-0.2, 1.2, 1200)
+                n, _, _ = self.ax3.hist(lag1[xlim_min:xlim_max],
+                                        bins=50,
+                                        orientation='horizontal')
+                self.ax3.plot(np.exp(log_pdf) * n.max() / np.exp(log_pdf).max(),
+                              x_grid,
+                              lw=3)
+                if cutoff is not None:
+                    self.ax3.axhline(cutoff,
+                                     color='r',
+                                     lw=3,
+                                     linestyle='dashed')
+
                 self.canvas.draw()
 
             def on_key_press(self, event):
                 if event.button == 3:
-                    saveFigure(self.fig)
+                    save_figure(self.fig)
 
-    # Run main loop
-    app = PCAgui()
+    # Run main loop.
+    app = AnalysisGui()
     app.mainloop()
     app.quit()
 
-    # Find which indices to use for reconstruction
+    # Find which indices to use for reconstruction.
     if toggle[0] == 100:
         raise Exception('Operation was cancelled')
 
     if toggle.sum() == 0:
         print('All components are classified as signal')
     else:
         print('{0} components classified as signal, {1} '
               'will be used for signal reconstruction.'.format(
                   toggle.sum(), int(toggle.size - toggle.sum())))
 
-    #update components with toggle info
+    # Update components with toggle info.
     components['artifact_components'] = toggle
     components['cutoff'] = cutoff
     components['noise_components'] = noise_components
     if 'domain_ROIs' in components:
         components['region_assignment'] = region_assignment
         components['region_labels'] = regions
 
-    if load_hdf5:  # if data came from save file, append toggle and timecourses
+    if load_hdf5:  # If data came from save file, append toggle and timecourses.
         f.save({'artifact_components': toggle})
         f.save({'noise_components': noise_components})
         f.save({'timecourses': components['timecourses']})
         if 'domain_ROIs' in components:
             f.save({
                 'region_assignment': region_assignment,
                 'region_labels': regions
```

### Comparing `seas-0.0.2/seas/ica.py` & `seas-0.0.3/seas/ica.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import os
 import re
 import numpy as np
 from datetime import datetime
 from sklearn.decomposition import FastICA
 from scipy import linalg
 from timeit import default_timer as timer
+from typing import Tuple
 
 from seas.waveletAnalysis import waveletAnalysis
 from seas.signalanalysis import butterworth, sort_noise, lag_n_autocorr
 from seas.hdf5manager import hdf5manager
-from seas.video import rotate, save, rescale, play
+from seas.video import rotate, save, rescale, play, scale_video
 
 
-def project(vector,
-            shape,
-            roimask=None,
-            n_components=None,
-            svd_multiplier=5,
-            calc_residuals=True):
+def project(vector: np.ndarray,
+            shape: Tuple[int, int, int],
+            roimask: np.ndarray = None,
+            n_components: int = None,
+            svd_multiplier: float = 5,
+            calc_residuals: bool = True):
     '''
-    Apply an ica decomposition to the first axis of the input vector.  If a roimask is provided, the flattened roimask will be used to crop the vector before decomposition.
+    Apply an ica decomposition to the first axis of the input vector.  
+    If a roimask is provided, the flattened roimask will be used to crop the vector before decomposition.
 
-    If n_components is not set, an adaptive svd threshold is used (see approximate_svd_linearity_transition), with the hyperparameter svd_mutliplier.  
+    If n_components is not set, an adaptive svd threshold is used 
+    (see approximate_svd_linearity_transition), 
+    with the hyperparameter svd_mutliplier.  
 
-    Residuals lost in the ICA projection are captured if calc_residuals == True.  This represents the signal lost by ICA compression.
+    Residuals lost in the ICA projection are captured if calc_residuals == True.  
+    This represents the signal lost by ICA compression.
 
     Arguments:
         vector: 
-            The (x*y, t) vector to be spatially ICA projected
+            The (x*y, t) vector to be spatially ICA projected.
         shape:
-            The shape of the original movie (t,x,y)
+            The shape of the original movie (t,x,y).
         roimask:
-            The roimask to crop the vectorized movie (x,y)
+            The roimask to crop the vectorized movie (x,y).
         n_components:
-            Manually request a set number of ICA components
+            Manually request a set number of ICA components.
         svd_multiplier:
-            The hyperparameter for svd adaptive thresholding
+            The hyperparameter for svd adaptive thresholding.
         calc_residuals:
             Whether to calculate spatial and temporal residuals of projection compression.
 
     Returns:
         components: A dictionary containing all the results, metadata, and information regarding the filter applied.
 
             mean: 
@@ -115,15 +120,16 @@
             # LAPACK error if matricies are too big
             u, ev, _ = linalg.svd(vector,
                                   full_matrices=False,
                                   lapack_driver='gesvd')
 
         components['svd_eigval'] = ev
 
-        # get starting point for decomposition based on svd mutliplier * the approximate point of transition to linearity in tail of ev components
+        #Get starting point for decomposition based on svd mutliplier * the approximate
+        # point of transition to linearity in tail of ev components.
         cross_1 = approximate_svd_linearity_transition(ev)
         n_components = cross_1 * svd_multiplier
 
         components['increased_cutoff'] = 0
 
         while True:
             print('\nCalculating ICA with', n_components, 'components...')
@@ -136,15 +142,15 @@
             eig_vec = ica.fit_transform(vector)
             eig_mix = ica.mixing_
 
             noise, cutoff = sort_noise(eig_mix.T)
 
             p_signal = (1 - noise.sum() / noise.size) * 100
 
-            if noise.size == shape[0]:  # all components are being used
+            if noise.size == shape[0]:  # All components are being used.
                 break
             elif p_signal < 75:
                 print('ICA components were under 75% signal ({0}% signal).'\
                     .format(p_signal))
                 break
             elif n_components >= shape[0]:
                 print('ICA components were under 75% signal ({0}% signal).'\
@@ -203,23 +209,23 @@
         ica = FastICA(n_components=n_components, random_state=1000)
 
         try:
             eig_vec = ica.fit_transform(vector)  # Eigenbrains
         except ValueError:
             print('Calculation exceeded float32 maximum.')
             print('Trying again with float64 vector...')
-            #value error if any value exceeds float32 maximum.
-            #overcome this by converting to float64
+            # Value error if any value exceeds float32 maximum.
+            # Overcome this by converting to float64.
             eig_vec = ica.fit_transform(vector.astype('float64'))
 
         t = timer() - t0
         print('Independent Component Analysis took: {0} sec'.format(t))
         eig_mix = ica.mixing_
 
-        # sort components by their eig val influence (approximated by timecourse standard deviation)
+        # Sort components by their eig val influence (approximated by timecourse standard deviation).
         ev_sort = np.argsort(eig_mix.std(axis=0))
         eig_vec = eig_vec[:, ev_sort][:, ::-1]
         eig_mix = eig_mix[:, ev_sort][:, ::-1]
 
         noise, cutoff = sort_noise(eig_mix.T)
         components['noise_components'] = noise
         components['cutoff'] = cutoff
@@ -258,34 +264,36 @@
             components['residuals_spatial'] = residuals_spatial
             components['residuals_temporal'] = residuals_temporal
 
         except Exception as e:
             print('Residual Calculation Failed!!')
             print('\t', e)
 
-    # Save filter metadata information about how and when movie was filtered in dictionary
+    # Save filter metadata information about how and when movie was filtered in dictionary.
     project_meta = {}
     project_meta['time_elapsed'] = t
     project_meta['date'] = \
         datetime.now().strftime('%Y%m%d')[2:]
     fmt = '%Y-%m-%dT%H:%M:%SZ'
     project_meta['tstmp'] = \
         datetime.now().strftime(fmt)
     project_meta['n_components'] = n_components
     components['project_meta'] = project_meta
 
     print('\n')
     return components
 
 
-def rebuild(components,
-            artifact_components=None,
-            t_start=None,
-            t_stop=None,
-            include_noise=True):
+def rebuild(components: dict,
+            artifact_components: np.ndarray = None,
+            t_start: int = None,
+            t_stop: int = None,
+            apply_mean_filter: bool = True,
+            filter_method: str = 'wavelet',
+            include_noise: bool = True):
     '''
     Rebuild original vector space based on a subset of principal 
     components of the data.  Eigenvectors to use are specified where 
     artifact_components == False.  Returns a matrix data_r, the reconstructed 
     vector projected back into its original dimensions.
 
     The filtered mean is *NOT* readded by this function.
@@ -295,24 +303,28 @@
             The components from ica_project.  artifact_components must be assigned to components before rebuilding, or passed in explicitly
         artifact_components:
             Overrides the artifact_components key in components, to rebuild all components except those specified
         t_start: 
             The frame to start rebuilding the movie at.  If none is provided, the rebuilt movie starts at the first frame
         t_stop: 
             The frame to stop rebuilding the movie at.  If none is provided, the rebuilt movie ends at the last frame
+        apply_mean_filter:
+            Whether to apply a filter to the mean signal.
+        filter_method:;
+            The filter method to apply (see filter_mean function).
         include_noise:
             Whether to include noise components when rebuilding.  If noise_components should not be included in the rebuilt movie, set this to False
 
     Returns:
         data_r: The ICA filtered video.
     '''
     print('\nRebuilding Data from Selected ICs\n-----------------------')
 
     if type(components) is str:
-        f = h5(components)
+        f = hdf5manager(components)
         components = f.load()
 
     assert type(components) is dict, 'Components were not in format expected'
 
     eig_vec = components['eig_vec']
     roimask = components['roimask']
     shape = components['shape']
@@ -343,15 +355,15 @@
         print('Returning empty matrix...')
         data_r = np.zeros((t, x, y), dtype='uint8')
         data_r = data_r[t_start:t_stop]
         return data_r
 
     n_components = reconstruct_indices.size
 
-    # make sure vector extracted properly matches the roimask given
+    # Make sure vector extracted properly matches the roimask given.
     if roimask is None:
         assert eig_vec[:, 0].size == x * y, (
             "Eigenvector size isn't compatible with the shape of the output "
             'matrix')
     else:
         maskind = np.where(roimask.flat == 1)
         assert eig_vec[:,0].size == maskind[0].size, \
@@ -375,16 +387,16 @@
     print('eig_vec:', eig_vec.shape)
     print('eig_mix:', eig_mix.shape)
 
     print('\nReconstructing....')
     data_r = np.dot(eig_vec[:, reconstruct_indices],
                     eig_mix[t_start:t_stop, reconstruct_indices].T).T
 
-    if filter_mean:
-        mean_filtered = filter_mean(mean, filter_method, low_cutoff)
+    if apply_mean_filter:
+        mean_filtered = filter_mean(mean, filter_method)
         data_r += mean_filtered[t_start:t_stop, None]
 
     else:
         print('Not filtering mean')
         mean_filtered = None
         data_r += mean[t_start:t_stop, None]
 
@@ -397,56 +409,63 @@
         reconstructed[maskind] = data_r.swapaxes(0, 1)
         reconstructed = reconstructed.swapaxes(0, 1)
         data_r = reconstructed.reshape(t, x, y)
 
     return data_r
 
 
-def approximate_svd_linearity_transition(eig_val):
+def approximate_svd_linearity_transition(eig_val: np.ndarray):
     '''
-    Approximates the transition between the svd signal distribution and the noise floor.
+    Approximates the transition between the svd signal distribution and 
+    the noise floor.
 
-    Calculates the integral of the eigenvalue 'influence' per component, fits a 2 degree polynomial to the curve, and looks for the point at which the integrated eigenvalues first overshoot the polynomial fit.  This transition point (multiplied by a hyperparameter) is used to inform the ICA n_components parameter.
+    Calculates the integral of the eigenvalue 'influence' per component, 
+    fits a 2 degree polynomial to the curve, and looks for the point at 
+    which the integrated eigenvalues first overshoot the polynomial fit.
+    This transition point (multiplied by a hyperparameter) is used to inform 
+    the ICA n_components parameter.
 
     Arguments:
         eig_val: 
-            The eigenvalues of the SVD decomposition
+            The eigenvalues of the SVD decomposition.
 
     Returns:
         transition: 
-            The estimate of the SVD noise floor cutoff
+            The estimate of the SVD noise floor cutoff.
     '''
     eig_val -= eig_val.min()
     eig_val = eig_val / eig_val.sum()
     eig_val_integrated = np.cumsum(eig_val)
     x = np.arange(eig_val.size)
 
     p = np.polyfit(x, eig_val_integrated, deg=2)
     y = np.polyval(p, x)
 
     transition = np.where(eig_val_integrated > y)[0][0]
 
     return transition
 
 
-def filter_mean(mean, filter_method='wavelet', low_cutoff=0.5):
+def filter_mean(mean: np.ndarray,
+                filter_method: str = 'wavelet',
+                low_cutoff: float = 0.5):
     '''
     Applies a high pass filtration to the ica mean signal.
 
     Arguments:
         mean: 
-            The mean timecourse signal
+            The mean timecourse signal.
         filter_method:
-            Which filtration method to apply.  Default is 'wavelet', but 'butterworth' is also accepted
+            Which filtration method to apply.  
+            Default is 'wavelet', but 'butterworth' is also accepted.
         low_cutoff:
-            The frequency cutoff to apply the high pass filter at 
+            The frequency cutoff to apply the high pass filter at.
 
     Returns:
-        mean_filtered:
-            The filtered mean
+        mean_filtered: The filtered mean.
     '''
     print('Highpass filter signal timecourse: ' + str(low_cutoff) + 'Hz')
     print('Filter method:', filter_method)
 
     if filter_method == 'butterworth':
         variance = mean.var()
         mean_filtered = butterworth(mean, low=low_cutoff)
@@ -460,32 +479,36 @@
     else:
         raise Exception("Filter method '" + str(filter_method)\
          + "' not supported!\n\t Supported methods: butterworth, wavelet")
 
     return mean_filtered
 
 
-def rebuild_mean_roi_timecourse(components,
-                                mask,
-                                include_zero=True,
-                                filter=True,
-                                invert_artifact=False,
-                                include_noise=True):
+def rebuild_mean_roi_timecourse(components: np.ndarray,
+                                mask: np.ndarray,
+                                include_zero: bool = True,
+                                filter: bool = True,
+                                invert_artifact: bool = False,
+                                include_noise: bool = True):
     '''
-    Rebuild a mean timecourse under a specific region of interest (ROI), or set of ROIs.
+    Rebuild a mean timecourse under a specific region of interest (ROI), 
+    or set of ROIs.
 
     Arguments:
         components: 
             The components result dictionary from ica.project
         mask:
-            The (x,y) mask to apply to the video for rebuilding.  If the mask has multiple unique indices (n_components), rather than just a single domain, they are all returned in an array
+            The (x,y) mask to apply to the video for rebuilding.  
+            If the mask has multiple unique indices (n_components), 
+            rather than just a single domain, they are all returned in an 
+            array.
 
     Returns:
         timecourses:
-            The set of rebuilt time courses (n_components,t)
+            The set of rebuilt time courses (n_components,t).
     '''
     eig_vec = components['eig_vec']
     roimask = components['roimask']
     eig_mix = components['eig_mix']
 
     if filter and 'artifact_components' in components.keys():
         artifact_components = components['artifact_components'].copy()
@@ -531,35 +554,39 @@
 
     if not include_zero:
         timecourses = timecourses[1:]
 
     return timecourses
 
 
-def rebuild_eigenbrain(eig_vec,
-                       index=None,
-                       roimask=None,
-                       eigb_shape=None,
-                       bulk=False):
-    '''
-    Reshape components from (n_components, xy) shape into (n_components, x, y), either through reassigning pixels where the roimask indicates, or by reshaping it into the original dimensions.
+def rebuild_eigenbrain(eig_vec: np.ndarray,
+                       index: int = None,
+                       roimask: np.ndarray = None,
+                       eigb_shape: Tuple[int, int] = None,
+                       maskind: float = 1,
+                       bulk: bool = False):
+    '''
+    Reshape components from (n_components, xy) shape into (n_components, x, y), 
+    either through reassigning pixels where the roimask indicates, or by reshaping 
+    it into the original dimensions.
 
-    If one component is requested with index, just that components is returned.  If the bulk flag is used instead, all are rebuilt and returned.
+    If one component is requested with index, just that components is returned.
+    If the bulk flag is used instead, all are rebuilt and returned.
 
     Arguments:
         eig_vec: 
-            The component eigenvectors (from components dictionary)
+            The component eigenvectors (from components dictionary).
         index:
-            Which index to rebuild
+            Which index to rebuild.
         roimask:
-            The roimask used to extract the xy coordinates (if applicable)
+            The roimask used to extract the xy coordinates (if applicable).
         eigb_shape:
-            The xy shape of the original movie (if roimask was not used)
+            The xy shape of the original movie (if roimask was not used).
         bulk:
-            Whether to rebuild all components, or just the one indicated by index
+            Whether to rebuild all components, or just the one indicated by index.
 
     Returns:
         eigenbrain:
             The reshaped eigenvector (x,y)
         OR eigenbrains:
             The array of reshaped eigenvectors (n_components, x, y)
     '''
@@ -597,90 +624,91 @@
             eigenbrain = np.empty(roimask.shape)
             eigenbrain[:] = np.NAN
             eigenbrain.flat[maskind] = eig_vec.T[index]
 
         return eigenbrain
 
 
-def filter_comparison(components,
-                      downsample=4,
-                      savepath=None,
-                      include_noise=True,
-                      t_start=None,
-                      t_stop=None,
-                      filter_mean=True,
-                      n_rotations=0):
+def filter_comparison(components: dict,
+                      downsample: int = 4,
+                      savepath: str = None,
+                      filtered_path: str = None,
+                      include_noise: bool = True,
+                      t_start: int = None,
+                      t_stop: int = None,
+                      apply_mean_filter: bool = True,
+                      n_rotations: int = 0):
     '''
-    Create a filter comparison movie, displaying the original movie, artifacts removed, and the filtered movie side by side.
+    Create a filter comparison movie, displaying the original movie, 
+    artifacts removed, and the filtered movie side by side.
 
 
     Arguments:
         components: 
-            The ICA components returned by ica.project
+            The ICA components returned by ica.project.
         downsample:
-            The factor to downsample by before writing the video
+            The factor to downsample by before writing the video.
         savepath:
-            The path to save the video at
+            The path to save the video at (mp4).
+        filtered_path:
+            The hdf5 path to save the filtered movie to. 
         include_noise:
-            Whether noise components should be included in the filtered video
+            Whether noise components should be included in the filtered video.
         t_start: 
-            The frame to start rebuilding the movie at.  If none is provided, the rebuilt movie starts at the first frame
+            The frame to start rebuilding the movie at.  If none is provided, 
+            the rebuilt movie starts at the first frame.
         t_stop: 
-            The frame to stop rebuilding the movie at.  If none is provided, the rebuilt movie ends at the last frame
+            The frame to stop rebuilding the movie at.  If none is provided, 
+            the rebuilt movie ends at the last frame.
         filter_mean:
-            Whether to filter the mean before readding
+            Whether to filter the mean before readding.
         n_rotations:
-            The number of CCW rotations to apply before saving the video
+            The number of CCW rotations to apply before saving the video.
 
     Returns:
         Nothing.
     '''
     print('\n-----------------------', '\nBuilding Filter Comparison Movies',
           '\n-----------------------')
 
-    if filterpath is not None:
-        g = h5(filterpath)
-    else:
-        g = None
-
     print('\nFiltered Movie\n-----------------------')
-    filtered = PCA_rebuild(components,
-                           returnmeta=True,
-                           include_noise=include_noise,
-                           t_start=t_start,
-                           t_stop=t_stop,
-                           filter_mean=filter_mean)
+    filtered = rebuild(components,
+                       include_noise=include_noise,
+                       t_start=t_start,
+                       t_stop=t_stop,
+                       apply_mean_filter=apply_mean_filter)
+
+    if filtered_path is not None:
+        print('Saving filtered movie to:', filtered_path)
+        f = hdf5manager(filtered_path)
+        f.save({'filtered_movie': filtered})
 
     filtered = scale_video(filtered, downsample)
     filtered = rotate(filtered, n_rotations)
 
     print('\nArtifact Movie\n-----------------------')
     artifact_index = np.where(components['artifact_components'] == 1)[0]
     components['artifact_components'] = np.ones(
         components['artifact_components'].shape)
     components['artifact_components'][artifact_index] = 0
     if not include_noise:
         components['artifact_components'][np.where(
             components['noise_components'] == 1)] = 0
-    artifact_movie = rebuild(components,
-                             returnmeta=False,
-                             t_start=t_start,
-                             t_stop=t_stop)
+    artifact_movie = rebuild(components, t_start=t_start, t_stop=t_stop)
     print('rescaling video...')
     artifact_movie = scale_video(artifact_movie, downsample)
     artifact_movie = rotate(artifact_movie, n_rotations)
 
     print('\nOriginal Movie\n-----------------------')
     components['artifact_components'] = np.zeros(
         components['artifact_components'].shape)
     raw_movie = rebuild(components,
-                        returnmeta=False,
                         t_start=t_start,
                         t_stop=t_stop,
-                        filter_mean=False)
+                        apply_mean_filter=apply_mean_filter)
     print('rescaling video...')
     raw_movie = scale_video(raw_movie, downsample)
     raw_movie = rotate(raw_movie, n_rotations)
 
     movies = np.concatenate((raw_movie, artifact_movie, filtered), axis=2)
 
     if 'roimask' in components.keys():
@@ -693,13 +721,13 @@
 
     else:
         overlay = None
 
     print('overlay', overlay.shape)
     print('movies', movies.shape)
 
-    save(savepath,
-         movies,
+    save(movies,
+         savepath,
+         rescale_range=True,
          resize_factor=1 / 2,
-         rescale=True,
          save_cbar=True,
          overlay=overlay)
```

### Comparing `seas-0.0.2/seas/rois.py` & `seas-0.0.3/seas/rois.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,118 @@
 import zipfile
 import re
 import numpy as np
 from io import BytesIO
 import cv2
+from typing import Tuple, List
 
 
-def get_masked_region(A, mask, maskval=None):
+def get_masked_region(array: np.ndarray,
+                      mask: np.ndarray,
+                      maskval: float = None):
     '''
     Extract a spatially masked array where the mask == 1 or 
     mask == maskval. Reinsert masked region using insert_masked_region function.
     
     Arguments:
-        A: a (t,x,y) numpy array or an (x,y,c) numpy array
+        array: a (t,x,y) numpy array or an (x,y,c) numpy array
 
     Returns:
-        M: the masked array in (t,xy) or (xy,c) format.
+        masked_array: the masked array in (t,xy) or (xy,c) format.
 
     Raises:
         Exception: if (x,y) mask indices did not match the shape of the input array.
     '''
-
     if maskval == None:
         maskind = np.where(mask == 1)
     else:
         maskind = np.where(mask == maskval)
 
-    if A.shape[0:2] == mask.shape:  #check if dimensions align for masking
-        M = A[maskind]
-    elif (A.shape[1], A.shape[2]) == mask.shape:
-        M = A.swapaxes(0, 1).swapaxes(1, 2)[maskind]
-        M = M.swapaxes(0, 1)
+    if array.shape[0:2] == mask.shape:  # Check if dimensions align for masking.
+        masked_array = array[maskind]
+    elif (array.shape[1], array.shape[2]) == mask.shape:
+        masked_array = array.swapaxes(0, 1).swapaxes(1, 2)[maskind]
+        masked_array = masked_array.swapaxes(0, 1)
     else:
         raise Exception(
             'Unknown mask indices with the following '
-            'dimensions:\n', 'Array: {0} Mask: {1}'.format(A.shape, mask.shape))
+            'dimensions:\n',
+            'Array: {0} Mask: {1}'.format(array.shape, mask.shape))
 
-    return M
+    return masked_array
 
 
-def insert_masked_region(A, M, mask, maskval=1):
+def insert_masked_region(array: np.ndarray,
+                         masked_array: np.ndarray,
+                         mask: np.ndarray,
+                         maskval: float = 1):
     '''
     Insert a spatially masked array from get_masked_region.  
     Masked array is inserted where the mask == 1 or mask == maskval. 
     Accepts masked array in (t,xy) or (xy,c) format.
     Accepts (t,x,y) arrays or (x,y,c) arrays, returns them in the 
     same format.
+
+    Arguments:
+        array: A (t,x,y) numpy array or an (x,y,c) numpy array
+        masked_array: The masked array in (t,xy) or (xy,c) format.
+            Usually extracted using get_masked_region.
+        mask: The mask used to extract the masked array originally, 
+            will be used for reinsertion.
+        maskval: The value used to extracted the region, if not the default of 1.
+
+    Returns:
+        array: The array with the masked values reinserted.
+
     '''
     maskind = np.where(mask == maskval)
 
-    if A.shape[0:2] == mask.shape:  #check if dimensions align for masking
-        A[maskind] = M
-    elif (A.shape[1], A.shape[2]) == mask.shape:
-        M = M.swapaxes(0, 1)
-        A = A.swapaxes(0, 1).swapaxes(1, 2)
-        A[maskind] = M
-        A = A.swapaxes(1, 2).swapaxes(0, 1)
-        # A.swapaxes(0,1).swapaxes(1,2)[maskind] = M
+    if array.shape[0:2] == mask.shape:  #check if dimensions align for masking
+        array[maskind] = masked_array
+    elif (array.shape[1], array.shape[2]) == mask.shape:
+        masked_array = masked_array.swapaxes(0, 1)
+        array = array.swapaxes(0, 1).swapaxes(1, 2)
+        array[maskind] = masked_array
+        array = array.swapaxes(1, 2).swapaxes(0, 1)
     else:
         raise Exception('Unknown mask indices with the following '
                         'dimensions:\n'
                         'Array: {0}, Mask: {1}'.format(A.shape, mask.shape))
 
-    return A
+    return array
 
 
-def roi_loader(path, verbose=True):
+def roi_loader(path: str, verbose: bool = True) -> dict:
     print('\nLoading Rois\n-----------------------')
+    '''
+    Load ROIs from a path.  
+    Rois must be in a zip file containing multiple polygon roi files, 
+    created by FIJI/ImageJ.
+
+    Arguments:
+        path: The path to the zip file of FIJI ROIs.
+        verbose: Whether to produce verbose output.
+
+    Returns:
+        rois: A dictionary containing lists of coordinates, 
+            which should be bounded polygons.
+    '''
 
     def load_roi_file(fileobj):
         '''
-        points = roiLoader(ROIfile)
+        This is based on a gist from Luis Pedro:
+        https://gist.github.com/luispedro/3437255
+
         ROIfile is a .roi file view.  
         It must first be opened as a bitstring through BytesIO to allow 
         for seeking through the bitstring.
         Read ImageJ's ROI format. Points are returned in a nx2 array. Each row
         is in (x,y) order.
         This function may not work for float32 formats, or with images that 
         have subpixel resolution.
-
-        This is based on a gist from luis pedro:
-        https://gist.github.com/luispedro/3437255
         '''
 
         def get8():
             s = fileobj.read(1)
             if not s:
                 raise IOError('readroi: Unexpected EOF')
             return ord(s)
@@ -112,157 +141,172 @@
         points[:, 1] += top
         points[:, 0] += left
 
         return points
 
     rois = dict()
 
-    # Load a .zip file of .roi files
+    # Load a .zip file of .roi files.
     if path.endswith('.zip'):
         f = zipfile.ZipFile(path)
         roifilelist = f.namelist()
 
         for roifile in roifilelist:
             if verbose:
                 print('Loading ROIs at: ', roifile)
             roiname = re.sub('.roi', '', roifile)
 
             roidata = BytesIO(f.read(roifile))
             points = load_roi_file(roidata)
             rois[roiname] = points
             roidata.close()
 
-    # Not a valid file extension
+    # Not a valid file extension.
     else:
         raise Exception('{0} does not have a valid roi '
                         'file extension.  Accepted file format is '
                         '.zip.'.format(path))
 
     return rois
 
 
-def make_mask(polylist, shape, bounding_box=None):
+def make_mask(polylist: np.ndarray, shape: Tuple[int, int], bounding_box=None):
     '''
     Makes mask from coordinates of polygon(s).  
     
-    Polylist is a list of numpy arrays, each representing a 
-    closed polygon to draw.
+    Polylist is a list of (x,y) numpy arrays, 
+
+    Arguments:
+        polylist: A list of (x,y) numpy arrays returned under a roi key by roi_loader, 
+            each representing a closed polygon to draw..
+        shape: (x,y) coordinate of shape to draw the polygons onto.
+        bounding_box: If provided, offset the polygons by this amount to take into account 
+            a previous cropping of the input image/video.
+
+    Returns:
+
     '''
     assert (len(shape) == 2), 'Shape was not 2D'
 
     if bounding_box is not None:
         polylist = polylist - bounding_box[:, 0][::-1]
 
     roimask = np.zeros(shape, dtype='uint8')
     cv2.fillPoly(roimask, [polylist.astype(np.int32).reshape((-1, 1, 2))], 1)
 
     return roimask
 
 
-def draw_bounding_box(image, required=True):
+def draw_bounding_box(image: np.ndarray,
+                      required: bool = True) -> List[List[int]]:
     '''
     Draw a bounding box on a two dimensional image.  
     Image should already be scaled to 0-255 in uint8.
-    Returns a ROI bounding box with shape [[x0,x1],[y0,y1]]
+
+    Arguments:
+        image: A numpy array to draw the bounding box on.
+        required: Whether to raise an error if the process is 
+            exited without a valid bounding box.
+
+    Returns:
+        ref_coord: An ROI bounding box with shape [[x0,x1],[y0,y1]].
     '''
     print('\nDrawing Bounding Box\n-----------------------')
 
     assert (len(image.shape) == 2), '''The image is not two dimensional.  
         Shape: '''.format(image.shape)
 
     global refPt, cropping
-    # initialize the list of reference points
-    # and boolean indicating whether cropping is being performed
+    # Initialize the list of reference points
+    # and boolean indicating whether cropping is being performed.
     window_name = "Draw bounding box on image.  \
     'r' = reset, 'a' = all, s' = save, +/- = zoom"
 
     refPt = []
     cropping = False
     zoom = 1
     zfactor = 5 / 4
 
     def click_and_crop(event, x, y, flags, param):
         global refPt, cropping
-        # if the left mouse button was clicked, record the starting
+        # If the left mouse button was clicked, record the starting
         # (x, y) coordinates and indicate that cropping is being
-        # performed
+        # performed.
         if event == cv2.EVENT_LBUTTONDOWN:
             refPt = [(x, y)]
             cropping = True
 
-        #Check to see if left mouse button was released
+        # Check to see if left mouse button was released.
         elif event == cv2.EVENT_LBUTTONUP:
-            # record the ending (x,y) coordinates and indicate that
-            # the cropping operation is finished
+            # Record the ending (x,y) coordinates and indicate that
+            # the cropping operation is finished.
             refPt.append((x, y))
             cropping = False
 
             # draw a rectangle around the point of interest
             cv2.rectangle(draw, refPt[0], refPt[1], 255, 2)
             cv2.imshow(window_name, draw)
 
     cv2.destroyAllWindows()
     for i in range(1, 5):
         cv2.waitKey(1)
 
-    # load the image, clone it to draw, and setup the mouse
-    # callback function
-
+    # Load the image, clone it to draw, and setup the mouse.
     image = image.astype('uint8')
     draw = image.copy()
     cv2.namedWindow(window_name)
     cv2.setMouseCallback(window_name, click_and_crop)
 
-    # keep looping until the 'q' key is pressed
+    # Keep looping until the 'q' key is pressed.
     while True:
-        # display the image and wait for a keypress
+        # Display the image and wait for a keypress.
         cv2.imshow(window_name, draw)
         key = cv2.waitKey(1) & 0xFF
 
-        # if the '=' key is pressed, zoom in
+        # If the '=' key is pressed, zoom in.
         if key == ord("="):
             draw = cv2.resize(draw,
                               None,
                               fx=zfactor,
                               fy=zfactor,
                               interpolation=cv2.INTER_CUBIC)
             zoom = zoom * zfactor
 
-        # if the '-' key is pressed, zoom out
+        # If the '-' key is pressed, zoom out.
         if key == ord("-"):
             draw = cv2.resize(draw,
                               None,
                               fx=1 / zfactor,
                               fy=1 / zfactor,
                               interpolation=cv2.INTER_CUBIC)
             zoom = zoom * 1 / zfactor
 
-        # if the 'r' key is pressed, reset the cropping region
+        # If the 'r' key is pressed, reset the cropping region.
         if key == ord("r"):
             draw = image.copy()
             zoom = 1
 
         if key == ord("a"):
             print('Taking entire image')
             refPt = [(0, 0), (image.shape[0], image.shape[1])]
             break
 
-        # if the 's' key is pressed, break from the loop and save ROI
+        # If the 's' key is pressed, break from the loop and save ROI.
         elif key == ord("s"):
             break
 
-    # if there are two reference points, then crop the region of interestdd
+    # If there are two reference points, then crop the region of interestd.
 
     if len(refPt) == 2:
         ref_coord = np.array([
             sorted([refPt[0][1], refPt[1][1]]),
             sorted([refPt[0][0], refPt[1][0]])
         ])
 
-        # unzoom reference coordinates
+        # Unzoom reference coordinates.
         for i in range(2):
             ref_coord[i] = [round(y / zoom) for y in ref_coord[i]]
 
     else:
         print('Exiting without bounding box')
         ref_coord = None
```

### Comparing `seas-0.0.2/seas/signalanalysis.py` & `seas-0.0.3/seas/signalanalysis.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 from sklearn.neighbors import KernelDensity
+from scipy import signal
 from scipy.signal import argrelextrema
 import numpy as np
 import math
 from itertools import compress
+from typing import Tuple, List
 
 
-def sort_noise(timecourses=None,
-               lag1=None,
-               return_logpdf=False,
-               method='KDE',
-               verbose=False):
+def sort_noise(timecourses: np.ndarray = None,
+               lag1: np.ndarray = None,
+               return_logpdf: bool = False,
+               method: str = 'KDE',
+               verbose: bool = False) -> Tuple[np.ndarray, int, np.ndarray]:
     '''
     Sorts timecourses into two clusters (signal and noise) based on 
     lag-1 autocorrelation.  
-    Timecourses should be a np array of shape (n, t).
 
-    Returns noise_components, a np array with 1 value for all noise 
-    timecourses detected, as well as the cutoff value detected
+    Arguments:
+        timecourses: Input to calculate noise threshold. 
+            Should be a np array of shape (n, t).
+        lag1: Required if the timecourses are not provided.
+            alternate input to calculate noise threshold.
+            Should be a np array of shape (n, t).
+        return_logpdf: Whether to return the KDE log density function.
+        method: The method to calculate the cutoff.  Currently only KDE is supported.
+        verbose: Whether to record a verbose output.
+
+    Returns:
+        noise_components, a np array with a value of 1 where all noise 
+            timecourses detected. as well as the cutoff value detected.
+        cutoff: The cutoff index, anything above this value is considered to be noise. 
+        log_pdf: Returned only if return_logpdf is True.  
+            The pdf function evaluated between -0.2 and 1.2.
     '''
     if method == 'KDE':
 
-        # calculate lag autocorrelations
+        # Calculate lag autocorrelations.
         if lag1 is None:
             assert timecourses is not None, 'sortNoise requires either timecourses or lag1'
             lag1 = lag_n_autocorr(timecourses, 1)
 
-        # calculate minimum between min and max peaks
+        # Calculate minimum between min and max peaks.
         kde_skl = KernelDensity(kernel='gaussian',
                                 bandwidth=0.05).fit(lag1[:, np.newaxis])
         x_grid = np.linspace(-0.2, 1.2, 1200)
 
         log_pdf = kde_skl.score_samples(x_grid[:, np.newaxis])
 
         maxima = argrelextrema(np.exp(log_pdf), np.greater)[0]
@@ -50,46 +65,81 @@
 
     if return_logpdf:
         return noise_components, cutoff, log_pdf
     else:
         return noise_components, cutoff
 
 
-def get_peak_separation(log_pdf, x_grid=None):
+def get_peak_separation(log_pdf: np.ndarray,
+                        x_grid: np.ndarray = None) -> float:
+    '''
+    Get peak to peak separation value from the log pdf.
+    This is used in 
+
+    Arguments:
+        log_pdf: The log pdf function specifying the density distribution.
+        x_grid: Optional argument specifying the coordiates matching the log_pdf.
+            If empty, -0.2 : 1.2 in 1200 points is the default.
 
+    Returns: 
+        peak_separation: The peak to peak distance of the log_pdf.
+    '''
     if x_grid is None:
         x_grid = np.linspace(-0.2, 1.2, 1200)
 
     maxima = argrelextrema(np.exp(log_pdf), np.greater)[0]
 
     if len(maxima) > 2:
         maxima = np.delete(maxima, np.argmin(np.exp(log_pdf)[maxima]))
     peak_separation = x_grid[maxima[-1]] - x_grid[maxima[0]]
 
     return peak_separation
 
 
-def lag_n_autocorr(x, n, verbose=True):
+def lag_n_autocorr(x: np.ndarray, n: int, verbose: bool = True):
+    '''
+    Calculate the lag-n autocorrelation.  Lower values are more likely to be noise.
 
+    Arguments:
+        x: The 1-D input vector to calculate lag autcorrelation from.
+        n: The integer lag to calculate.
+        verbose: Whether to print a verbose output.
+    '''
     if x.ndim == 1:
         return np.corrcoef(x[n:], x[:-n])[0, 1]
     elif x.ndim == 2:
         if verbose:
             print('calculating {0}-lag autocorrelation'.format(n),
                   'along first dimension:', x.shape)
         nt = x.shape[0]
         corrmatrix = np.corrcoef(x[:, n:], x[:, :-n])
         return np.diag(corrmatrix[:nt, nt:])
     else:
         print('Invalid input!!')
         raise AssertionError
 
 
-def butterworth(data, high=None, low=None, fps=10, order=5):
-    from scipy import signal
+def butterworth(data: np.ndarray,
+                high: float = None,
+                low: float = None,
+                fps: int = 10,
+                order: int = 5) -> np.ndarray:
+    '''
+    Apply a butterworth filter on the data.
+
+    Arguments:
+        data: A 1-D time series array to filter.
+        high: The high pass filter to apply.
+        low: The low pass filter to apply.
+        fps: The number of frames per second of the input data.
+        order: The butterworth filter order to apply.
+
+    Returns:
+        data: The filtered dataset.
+    '''
 
     def butter_highpass(cutoff, fps, order=order):
         nyq = 0.5 * fps
         normal_cutoff = cutoff / nyq
         b, a = signal.butter(order, normal_cutoff, btype='high', analog=False)
         return b, a
 
@@ -106,62 +156,117 @@
     if high is not None:
         b, a = butter_lowpass(high, fps, order=order)
         data = signal.filtfilt(b, a, data)
 
     return data
 
 
-def local_max(xvalues, array1d, sig=None):
-    # finds the local max array values and their respective position (xvalues)
+def local_max(x_values: np.ndarray, array1d: np.ndarray, sig=None):
+    '''
+    Finds the local max array values and their respective position (xvalues)
+    by giving a significance cuttoff value array of the same size as the array1d, this will also return
+    the cutoff significance at each local maxima.
+
+    TODO(@brmullen): Add documentation here.
+
+    Args:
+        x_values:
+        array1d:
+        sig:
 
-    # by giving a significance cuttoff value array of the same size as the array1d, this will also return
-    # the cutoff significance at each local maxima
+    Returns:
 
+    '''
     if sig is not None:
         i = np.r_[True, array1d[1:] > array1d[:-1]] & np.r_[
             array1d[:-1] > array1d[1:], True]
-        return list(compress(xvalues,
+        return list(compress(x_values,
                              i)), list(compress(array1d,
                                                 i)), list(compress(sig, i))
     else:
         i = np.r_[True, array1d[1:] > array1d[:-1]] & np.r_[
             array1d[:-1] > array1d[1:], True]
-        return list(compress(xvalues, i)), list(compress(array1d, i))
+        return list(compress(x_values, i)), list(compress(array1d, i))
 
 
-def local_min(xvalues, array1d, sig=None):
-    # finds the local min array values and their respective position (xvalues)
+def local_min(x_values: np.ndarray,
+              array1d: np.ndarray,
+              sig=None) -> Tuple[List[np.ndarray], List[np.ndarray]]:
+    '''
+    Finds the local min array values and their respective position (xvalues)
+    by giving a significance cutoff value array of the same size as the array1d, this will also return
+    the cutoff significance at each local minima
+
+    TODO(@brmullen): Add documentation here.
+
+    Args:
+        x_values:
+        array1d:
+        sig:
 
-    # by giving a significance cutoff value array of the same size as the array1d, this will also return
-    # the cutoff significance at each local minima
+    Returns:
 
+    '''
     if sig is not None:
         i = np.r_[True, array1d[1:] < array1d[:-1]] & np.r_[
             array1d[:-1] < array1d[1:], True]
-        return list(compress(xvalues,
+        return list(compress(x_values,
                              i)), list(compress(array1d,
                                                 i)), list(compress(sig, i))
     else:
         i = np.r_[True, array1d[1:] < array1d[:-1]] & np.r_[
             array1d[:-1] < array1d[1:], True]
-        return list(compress(xvalues, i)), list(compress(array1d, i))
+        return list(compress(x_values, i)), list(compress(array1d, i))
 
 
-def abline(slope, intercept, nframe, label=None, color=None):
-    """Plot a line from slope and intercept"""
-    x_vals = np.array((0, nframe))
+def abline(slope: float,
+           intercept: float,
+           x_max: float,
+           label: str = None,
+           color: str = None,
+           x_min: float = 0) -> None:
+    '''
+    Plot a line to the currently active plt figure based on slope and intercept.
+
+    Arguments:
+        slope: The line slope.
+        intercept: The line y intercept.
+        x_max: The maximum x value to draw the line to.
+        x_min: The minimum x value to draw the line to.
+        label: The line label, if applicable.
+        color: The matplotlib color string.  If not specified, uses the next default option.
+
+    Returns:
+        None
+    '''
+    x_vals = np.array((0, x_min))
     y_vals = intercept + slope * x_vals
     if color != None:
         plt.plot(x_vals, y_vals, label=label, color=color)
     else:
         plt.plot(x_vals, y_vals, label=label)
 
 
-def linear_regression(time, signal, verbose=True):
+def linear_regression(time: np.ndarray,
+                      signal: np.ndarray,
+                      verbose=True) -> Tuple[float, float]:
+    '''
+    Applies a linear regression to the time-series signal.
 
+    Arguments:
+        time: The time, or x axis to fit the linear regression to.
+        signal: The signal, or y axis to fit the linear regression to.
+        verbose: Whether to print a verbose output specifying the fit results.
+
+    Returns:
+        slope: The linear regression slope.
+        intercept: The linear regression intercept.
+
+    TODO(@brmullen): Check documentation.
+    '''
     regr = linear_model.LinearRegression(fit_intercept=True)
     regr.fit(time.reshape(-1, 1), signal.reshape(-1, 1))
     wsumpred = regr.predict(signal.reshape(-1, 1))
     slope = regr.coef_[0]
     intercept = regr.intercept_[0]
     if verbose:
         print('Coefficients: \n', regr.coef_)
@@ -170,16 +275,30 @@
 
     return slope, intercept
 
 
 def tdelay_correlation(vectors, n, max_offset=150, return_window=False):
     '''
     Calculates correlations of timecourses stored in an array 'vectors', of shape 
-    (n, t) against the 'n'th element of the array, or an input vector of size 't'.  
-    Returns the correlation of each vector with vector 'n', and time offset.
+    (m, t) against the 'n'th element of the array, or an input vector of size 't'.  
+    Returns 
+
+    Arguments:
+        vectors: a (m,t) numpy array containing all time series, including the one to compare to.
+        n: The element to compare each other element to.
+        max_offset: The integer maximum time offset to calculate correlation out to.
+        return_window: Whether to return the maximum correlation value in the context of the correlation window.
+
+    Returns:
+        x_corr: the correlation of each vector with vector 'n', and time offset.
+        t_delay: The time delay which maximizes the correlation value.
+        corr_window: Returns the maximum correlation at the given time delay for each time series,
+            all other values are zero.  Only returned if return_window is True.
+
+    TODO(@brmullen): Check documentation.
     '''
 
     if type(n) is int:
         tc = vectors[n].copy()
 
     elif type(n) is np.ndarray:
         if vectors.ndim == 1:
@@ -189,15 +308,14 @@
                 .format(n.size, vectors[0].size)
         tc = n
 
     tc = (tc - tc.mean()) / (tc.std() * len(tc))
 
     vectors = (vectors.copy() - vectors.mean(axis=1)[:,None]) / \
         vectors.std(axis=1)[:,None]
-    # print('vectors', vectors)
 
     n_elements = vectors[:, 0].size
     x_corr = np.zeros(n_elements)
     t_delay = np.zeros(n_elements, dtype=np.int32)
 
     if max_offset > tc.size:
         max_offset = tc.size
@@ -219,61 +337,66 @@
     if return_window:
         return x_corr, t_delay, corr_window
     else:
         return x_corr, t_delay
 
 
 def gaussian_smooth_2d(matrix, dj, dt):
+    '''
+    TODO(@brmullen): Write documentation.
+    '''
     sigma = [dj, dt]
     smooth_matrix = gaussian_filter(matrix.real, sigma=sigma)
     smooth_matrix += gaussian_filter(matrix.imag, sigma=sigma).imag
 
     return smooth_matrix
 
 
 def short_time_fourier_transform(data,
                                  fps=10,
-                                 fftLen=100,
+                                 fft_len=100,
                                  overlap=99,
                                  verbose=False):
-
-    padEndSz = fftLen
-    # the last segment can overlap the end of the data array by no more
-    # than one window size
-    nyq = fps / 2  # Nyquist frequency
+    '''
+    TODO(@brmullen): Write documentation.
+    '''
+    padEndSz = fft_len
+    # The last segment can overlap the end of the data array by no more
+    # than one window size.
+    nyq = fps / 2  # Nyquist frequency.
 
     if verbose:
         print("Calculating STFT of window size {0} and an overlap of {1}\
             \n--------------------------------------------------\
-            ".format(fftLen, overlap))
+            ".format(fft_len, overlap))
 
-    hopSz = np.int32(np.floor(fftLen - overlap))
-    # calculates the how far the next STFT is from the last
+    hopSz = np.int32(np.floor(fft_len - overlap))
+    # Calculates the how far the next STFT is from the last.
     numSeg = np.int32(np.ceil(len(data) / np.float32(hopSz)))
-    # Number of segments of through the all the data
-    window = np.hanning(fftLen)
-    # create a Hanning window of the appropriate length
-    inPad = np.zeros(fftLen)  # zeros to pad each individual segment
+    # Number of segments of through the all the data.
+    window = np.hanning(fft_len)
+    # Create a Hanning window of the appropriate length.
+    inPad = np.zeros(fft_len)  # zeros to pad each individual segment
 
     padData = np.concatenate((data, np.zeros(padEndSz)))
-    # the padded data to process
-    result = np.empty((fftLen, numSeg), dtype=np.float32)
-    # space to hold the result
+    # The padded data to process.
+    result = np.empty((fft_len, numSeg), dtype=np.float32)
+    # Space to hold the result.
 
     for i in range(numSeg):
-        hop = hopSz * i  # figure out the current segment offset
-        seg = padData[hop:hop + fftLen]  # get the current segment
-        windowed = (seg * window)  # apply a Hanning Window
+        hop = hopSz * i  # Figure out the current segment offset.
+        seg = padData[hop:hop + fft_len]  # Get the current segment.
+        windowed = (seg * window)  # Apply a Hanning Window.
         padded = np.append(windowed, inPad)
-        # add zeros to double the length of the data
-        spectrum = np.fft.fft(padded) / fftLen
-        # take the Fourier Transform and scale by the number of data points
+        # Add zeros to double the length of the data.
+        spectrum = np.fft.fft(padded) / fft_len
+        # Take the Fourier Transform and scale by the number of data points.
         autopower = np.abs(spectrum * np.conj(spectrum))
-        # find the autopower spectrum
-        result[:, i] = autopower[:fftLen]  # append to the results array
+        # Find the autopower spectrum.
+        result[:, i] = autopower[:fft_len]  # Append to the results array.
 
     result = np.flipud(result[0:math.floor(2 * nyq * fps), :]) / overlap
-    # clip values greater than the nyquist sampling rate
+    # Clip values greater than the nyquist sampling rate.
     maxData = np.amax(result)
     minData = np.amin(result)
 
     return result, fps, nyq, maxData
```

### Comparing `seas-0.0.2/seas/video.py` & `seas-0.0.3/seas/video.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,75 +6,89 @@
 from math import ceil
 import cv2
 import os
 
 from seas.rois import get_masked_region, insert_masked_region
 from seas.colormaps import DEFAULT_COLORMAP, save_colorbar
 
+from typing import Tuple, List
 
-def load(pathlist,
-         downsample=False,
-         t_downsample=False,
-         dtype=None,
-         verbose=True,
-         tiffloading=True,
-         greyscale=True):
+
+def load(pathlist: List[str],
+         downsample: int = False,
+         t_downsample: int = False,
+         dtype: str = None,
+         verbose: bool = True,
+         tiffloading: bool = True,
+         greyscale: bool = True) -> np.ndarray:
     '''
     Loads a list of tiff paths, returns concatenated arrays.
     Implemented size-aware loading for tiff arrays with pre-allocation
     Expects a list of pathnames: 
-    ex: ['./testvideo1.mat', '/home/sydney/testfile2.tif']
+
+    Arguments:
+        pathlist: List of paths to load.  Can be mixes formats, as long as dimensions match.
+            ex: ['./testvideo1.mat', '/home/sydney/testfile2.tif']
+        downsample: The spatial factor to downsample by.
+        t_downsample: The temporal factor to downsample by.
+        dtype: The data type to load into.  Must be a numpy data type string.
+        verbose: Whether to print verbose output.
+        tiffloading: Whether to preallocate array in memory based on file size expected from each tiff file.
+        greyscale: Whether the files are in color or greyscale.
+
+    Returns:
+
     Files in list must be the same xy dimensions.
     if downsample is an integer greater than one, movie will be downsampled 
     # by that factor.
     '''
     print('\nLoading Files\n-----------------------')
 
-    if type(pathlist) is str:  # if just one path got in
+    if type(pathlist) is str:  # If just one path got in.
         pathlist = [pathlist]
 
-    # make sure pathlist is a list of strings
+    # Make sure pathlist is a list of strings.
     assert type(pathlist) is list
 
-    # use tiff loading if all paths are tiffs.
+    # Use tiff loading if all paths are tiffs.
     for obj in pathlist:
         assert type(obj) is str
         if not (obj.endswith('.tif') | obj.endswith('.tiff')):
             print('Found non-tiff file to load:', obj)
             tiffloading = False
 
-    # if downsampling, explicitly state spatial and temporal factors.
+    # If downsampling, explicitly state spatial and temporal factors.
     if downsample or t_downsample:
 
         if not t_downsample:
             t_downsample = 1
         if not downsample:
             downsample = 1
 
         assert type(downsample) is int
         assert type(t_downsample) is int
 
-    # if no datatype was given, assume it's uint16
+    # If no datatype was given, assume it's uint16.
     if dtype == None:
         dtype = 'uint16'
 
-    # use size-aware tiff loading to preallocate matrix and load one at a time
+    # Use size-aware tiff loading to preallocate matrix and load one at a time.
     if tiffloading:
-        # ignore tiff warning (lots of text, unnecessary info)
+        # Ignore tiff warning (lots of text, unnecessary info).
         warnings.simplefilter('ignore', UserWarning)
         try:
 
             print('Using size-aware tiff loading.')
             nframes = 0
 
-            # loop through tiff files to determine matrix size
+            # Loop through tiff files to determine matrix size.
             for f, path in enumerate(pathlist):
                 with tifffile.TiffFile(path) as tif:
                     if (len(tif.pages) == 1) and (len(tif.pages[0].shape) == 3):
-                        # sometimes movies save as a single page
+                        # Sometimes movies save as a single page.
                         pageshape = tif.pages[0].shape[1:]
                         nframes += tif.pages[0].shape[0]
 
                     else:
                         nframes += len(tif.pages)
                         pageshape = tif.pages[0].shape
 
@@ -83,97 +97,98 @@
                     else:
                         assert pageshape == shape, \
                             'shape was not consistent for all tiff files loaded'
 
             shape = (nframes, shape[0], shape[1])
             print('shape:', shape)
 
-            # resize preallocated matrix if downsampling
+            # Resize preallocated matrix if downsampling.
             if downsample:
                 shape = (shape[0] // t_downsample, shape[1] // downsample,
                          shape[2] // downsample)
                 print('downsample size:', shape, '\n')
 
-                # initialize remainder for temporal downsampling
+                # Initialize remainder for temporal downsampling.
                 rmarray = np.zeros(shape=(0, shape[1], shape[2]), dtype='uint8')
 
-            A = np.empty(shape, dtype=dtype)
+            array = np.empty(shape, dtype=dtype)
 
-            # load video one at a time and assign to preallocated matrix
+            # Load video one at a time and assign to preallocated matrix.
             i = 0
             for f, path in enumerate(pathlist):
                 t0 = timer()
                 print('Loading file:', path)
                 with tifffile.TiffFile(path) as tif:
                     if downsample:
                         if downsample > 1:
                             print('\t spatially downsampling by {0}..'.format(
                                 downsample))
                         if t_downsample > 1:
                             print('\t temporally downsampling by {0}..'.format(
                                 t_downsample))
 
-                        array = tif.asarray()
+                        tiff_array = tif.asarray()
                         if rmarray.shape[0] > 0:
                             if verbose:
                                 print('concatenating remainder..')
-                            array = np.concatenate((rmarray, array), axis=0)
+                            tiff_array = np.concatenate((rmarray, tiff_array),
+                                                        axis=0)
 
-                        dsarray, rmarray = scale_video(array,
-                                                       downsample,
-                                                       t_downsample,
-                                                       verbose=False,
-                                                       remainder=True)
-                        npages = dsarray.shape[0]
-                        A[i:i + npages] = dsarray
+                        downsampled_array, rmarray = scale_video(tiff_array,
+                                                                 downsample,
+                                                                 t_downsample,
+                                                                 verbose=False,
+                                                                 remainder=True)
+                        npages = downsampled_array.shape[0]
+                        array[i:i + npages] = downsampled_array
 
                     else:
-                        array = tif.asarray()
-                        if array.ndim == 3:
-                            npages = array.shape[0]
-                        else:  # if a movie has only one frame, shape is only 2d
+                        tiff_array = tif.asarray()
+                        if tiff_array.ndim == 3:
+                            npages = tiff_array.shape[0]
+                        else:  # If a movie has only one frame, shape is only 2d.
                             npages = 1
-                        A[i:i + npages] = array
+                        array[i:i + npages] = tiff_array
 
                     i += npages
 
                 print("\t Loading file took: {0} sec".format(timer() - t0))
         except Exception as e:
-            # if something failed,  try again without size aware tiff loading
+            # If something failed,  try again without size aware tiff loading.
             print('Size-aware tiff-loading failed!')
             print('\tException:', e)
             tiffloading = False
 
-    # don't use tiff size-aware loading.  load each file and append to growing matrix
+    # Don't use tiff size-aware loading.  load each file and append to growing matrix.
     if not tiffloading:
         print('Not using size-aware tiff loading.')
         if t_downsample:
             remainder = True
         hdf5_loadkey = None
 
-        # general function for loading a path of any type.
-        # add if/elif statements for more file types
+        # General function for loading a path of any type.
+        # Add if/elif statements for more file types
         def loadFile(path, downsample, t_downsample, remainder=None):
             t0 = timer()
 
             if path.endswith('.tif') | path.endswith('.tiff'):
                 print("Loading tiff file at " + path)
                 with tifffile.TiffFile(path) as tif:
-                    A = tif.asarray()
+                    array = tif.asarray()
                     if type(A) is np.memmap:
-                        A = np.array(A, dtype=dtype)
+                        array = np.array(array, dtype=dtype)
 
             elif path.endswith('.hdf5') | path.endswith('.mat'):
                 print("Loading hdf5 file at", path)
                 f = h5(path)
 
                 if 'movie' in f.keys():
-                    A = f.load('movie')
+                    array = f.load('movie')
                 elif 'tr' in f.keys():
-                    A = f.load('tr')
+                    array = f.load('tr')
                 else:
                     nonlocal hdf5_loadkey
 
                     if hdf5_loadkey is None:
                         print("'movie' not found in file keys.")
                         print('Keys in file:')
                         [print('\t', key) for key in f.keys()]
@@ -182,38 +197,38 @@
                             print('Which key do you want to load?')
                             loadinput = input()
                             if loadinput in f.keys():
                                 hdf5_loadkey = loadinput
                             else:
                                 print('key:', loadinput, 'was not valid.')
 
-                    A = f.load(hdf5_loadkey)
+                    array = f.load(hdf5_loadkey)
 
             elif path.endswith('.avi') | path.endswith('.mp4'):
                 cap = cv2.VideoCapture(path)
 
                 frameCount = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
                 frameWidth = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
                 frameHeight = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
 
                 if greyscale:
-                    A = np.empty((frameCount, frameHeight, frameWidth),
-                                 np.dtype('uint8'))
+                    array = np.empty((frameCount, frameHeight, frameWidth),
+                                     np.dtype('uint8'))
                 else:
-                    A = np.empty((frameCount, frameHeight, frameWidth, 3),
-                                 np.dtype('uint8'))
+                    array = np.empty((frameCount, frameHeight, frameWidth, 3),
+                                     np.dtype('uint8'))
 
                 fc = 0
                 ret = True
                 while (fc < frameCount and ret):
                     if greyscale:
                         ret, frame = cap.read()
-                        A[fc] = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+                        array[fc] = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
                     else:
-                        ret, A[fc] = cap.read()
+                        ret, array[fc] = cap.read()
                     fc += 1
                 cap.release()
 
             else:
                 print('File path is of unknown file type!')
                 raise Exception("'{0}' does not have a supported \
                     path extension".format(path))
@@ -221,98 +236,122 @@
             if downsample is not False:
                 print('\t spatially downsampling by {0}..'.format(downsample))
                 print(
                     '\t temporally downsampling by {0}..'.format(t_downsample))
                 if remainder is not None:
                     if (type(remainder) == np.ndarray) and \
                             (remainder.shape[0] != 0):
-                        A = np.concatenate((remainder, A), axis=0)
+                        array = np.concatenate((remainder, array), axis=0)
                     A, remainder = scale_video(A,
                                                downsample,
                                                t_downsample,
                                                verbose=True,
                                                remainder=True)
                 else:
-                    A = scale_video(A, downsample, t_downsample, verbose=True)
+                    array = scale_video(A,
+                                        downsample,
+                                        t_downsample,
+                                        verbose=True)
 
             print("Loading file took: {0} sec".format(timer() - t0))
 
             if remainder is not None:
-                return remainder, A
+                return remainder, array
             else:
-                return A
+                return array
 
-        # load either one file, or load and concatenate list of files
+        # Load either one file, or load and concatenate list of files.
         if len(pathlist) == 1:
-            A = loadFile(pathlist[0], downsample, t_downsample)
+            array = loadFile(pathlist[0], downsample, t_downsample)
         else:
             remainder = None
             for i, path in enumerate(pathlist):
                 if t_downsample > 1:
-                    remainder, Atemp = loadFile(path,
-                                                downsample,
-                                                t_downsample,
-                                                remainder=remainder)
+                    remainder, temporary_array = loadFile(path,
+                                                          downsample,
+                                                          t_downsample,
+                                                          remainder=remainder)
                 else:
-                    Atemp = loadFile(path, downsample, t_downsample, remainder)
+                    temporary_array = loadFile(path, downsample, t_downsample,
+                                               remainder)
 
                 t0 = timer()
                 if i == 0:
-                    A = Atemp
+                    array = temporary_array
                 else:
                     try:
-                        A = np.concatenate([A, Atemp], axis=0)
+                        array = np.concatenate([A, temporary_array], axis=0)
                     except:
-                        A = np.concatenate([A, Atemp[None, :, :]], axis=0)
+                        array = np.concatenate([A, temporary_array[None, :, :]],
+                                               axis=0)
 
                 print("Concatenating arrays took: {0} sec\n".format(timer() -
                                                                     t0))
 
-    return A
+    return array
 
 
-def save(array,
-         path,
-         resize_factor=1,
-         apply_cmap=True,
-         rescale_range=False,
-         colormap='default',
-         speed=1,
-         fps=10,
-         codec=None,
-         mask=None,
-         overlay=None,
-         overlay_color=(0, 0, 0),
-         save_cbar=False):
+def save(array: np.ndarray,
+         path: str,
+         resize_factor: int = 1,
+         apply_cmap: bool = True,
+         rescale_range: bool = False,
+         colormap: np.ndarray = 'default',
+         speed: int = 1,
+         fps: int = 10,
+         codec: str = None,
+         mask: np.ndarray = None,
+         overlay: np.ndarray = None,
+         overlay_color: Tuple[int, int, int] = (0, 0, 0),
+         save_cbar: bool = False) -> None:
     '''
     Check what the extension of path is, and use the appropriate function
     for saving the array.  Functionality can be added for more 
     file/data types.
 
+
+    Arguments:
+        array: The (x,y,t) or (x,y,c,t) array to save to a video.
+        path: Where to save the file to.
+        resize_factor: A spatial resize factor to apply when saving
+        apply_cmap: Whether to apply a colormap.  Defaults to True.
+        rescale_range: Whether to rescale the dyanmic range of the video when saving.  Defaults to True.
+        colormap: The colormap to apply.  Defaults to the global default colormap.
+        speed: The speed factor to save the video at.  Multiplies the fps of the video.
+        fps: The video fps to save at.
+        codec: The video codec to use.  See the note below for more information.
+        mask: The mask to apply when saving.  If selected, the areas where mask == 0 will be black.
+        overlay: An overlay to draw on top of the video when saving.
+        overlay_color: The color to save the overlay as.
+        save_cbar: Whether to save an additional figure showing the color bar of the colormap applied to the video.
+
+    Returns:
+        None
+
+    
+    A note on codecs:
     For AVIs:
     Parameters (args 3+) are used for creating an avi output.  
     MJPG and XVID codecs seem to work well for linux systems, 
     so they are set as the default.
     A full list of codecs could be found at:
     http://www.fourcc.org/codecs.php.
-
-    We may need to investigate which codec gives us the best output. 
     '''
     print('\nSaving File\n-----------------------')
     assert (type(array) == np.ndarray), ('Movie to save was not a '
                                          'numpy array')
 
     if colormap == 'default':
         colormap = DEFAULT_COLORMAP
 
     if path.endswith('.tif') | path.endswith('.tiff'):
         print('Saving to: ' + path)
         t0 = timer()
         if array.shape[2] == 3:
-            # convert RGB to BGR
+            # Convert RGB to BGR.
             array = cv2.cvtColor(array, cv2.COLOR_BGR2RGB)
             print('Converted RGB image to BGR.')
         with tifffile.TiffWriter(path) as tif:
             tif.save(array)
         print("Save file: {0} sec\n".format(timer() - t0))
         save_cbar = False
 
@@ -343,26 +382,26 @@
         sz = array.shape
 
         if rescale_range:
             array, scale = rescale(array, return_scale=True)
 
         array = array.astype('uint8')
 
-        if codec == None:  # no codec specified
+        if codec == None:  # No codec specified.
             if path.endswith('.avi'):
                 codec = 'MJPG'
             elif path.endswith('.mp4'):
                 if os.name == 'posix':
                     codec = 'X264'
                 elif os.name == 'nt':
                     codec = 'XVID'
                 else:
                     raise TypeError('Unknown os type: {0}'.format(os.name))
 
-        # check codec and dimensions
+        # Check codec and dimensions.
         if array.ndim == 3:
             if apply_cmap == False:
                 sz = array.shape
                 array = array.reshape(sz[0], sz[1] * sz[2])
                 array = cv2.cvtColor(array, cv2.COLOR_GRAY2RGB)
                 array = array.reshape((sz[0], sz[1], sz[2], 3))
                 movietype = 'black and white'
@@ -377,19 +416,19 @@
                             'cannot be written in this format.'.format(
                                 array.ndim))
 
         print('Movie will be written in {0} using the {1} codec'.format(
             movietype, codec))
         print('Saving to: ' + path)
 
-        # Set up resize
+        # Set up resize.
         w = int(ceil(sz[1] * resize_factor))
         h = int(ceil(sz[2] * resize_factor))
 
-        # initialize movie writer
+        # Initialize movie writer.
         display_speed = fps * speed
         fourcc = cv2.VideoWriter_fourcc(*codec)
         out = cv2.VideoWriter(path, fourcc, display_speed, (h, w), True)
 
         if overlay is not None:
             if resize_factor != 1:
                 overlay = cv2.resize(overlay, (h, w),
@@ -415,233 +454,272 @@
     else:
         print('Save path is of unknown file type!')
         raise Exception("'{0}' does not have a supported \
             path extension".format(path))
 
     print('File saved to:' + path)
 
-    if save_cbar:
+    if save_cbar and rescale_range:
         cbarpath = os.path.splitext(path)[0] + '_colorbar.pdf'
         print('Saving Colorbar to:' + cbarpath)
         save_colorbar(scale, cbarpath, colormap=colormap)
 
 
-def dfof(A, win_size=None, win_type='box'):
+def dfof(array, win_size: int = None, win_type: str = 'box'):
     '''
     Calculates the change in fluorescence over mean 
-    fluorescense for a video.
-    If no win_size is given, it will calculate the dfof using
-    an average projection of the whole video.
+    fluorescense for a video.  If no win_size is given, 
+    it will calculate the dfof using an average projection of the whole video.
     Define window size and window type from (see function from 
     time course analysis) to calculate a rolling average dfof.
+
+    Arguments:
+        array: The input (x,y,t or xy,t) array to calculate dfof of.
+        win_size: The temporal window size to calculate rolling mean effects, if applicable.
+        win_type: The type of windowing effect applied to the movie. 
+
+    Returns:
+        array: The array after dfof is applied.
     '''
 
-    assert (type(A) == np.ndarray), 'Input was not a numpy array'
-    print(A.shape)
-    if A.ndim == 3:
+    assert (type(array) == np.ndarray), 'Input was not a numpy array'
+    if array.ndim == 3:
         reshape = True
-        sz = A.shape
-        A = np.reshape(A, (sz[0], int(A.size / sz[0])))
-    elif A.ndim == 2:
+        sz = array.shape
+        array = np.reshape(array, (sz[0], int(array.size / sz[0])))
+    elif array.ndim == 2:
         reshape = False
     else:
-        assert A.ndim == 1, ('Input was not 1-3 dimensional: {0} dim'.format(
-            A.ndim))
+        assert array.ndim == 1, (
+            'Input was not 1-3 dimensional: {0} dim'.format(array.ndim))
         reshape = False
-        A = A[:, None]
+        array = array[:, None]
         print('Reshaped to two dimensional.')
 
-    print("Array Shape (t,xy): {0}".format(A.shape))
-    print('Array Type:', A.dtype)
+    print("Array Shape (t,xy): {0}".format(array.shape))
+    print('Array Type:', array.dtype)
 
     t0 = timer()
     if win_size == None:
         print('\nCalculating dF/F\n-----------------------')
         print('Calculating dFoF based on average projection')
-        Amean = np.nanmean(A, axis=0, dtype='float32')
+        array_mean = np.nanmean(array, axis=0, dtype='float32')
         print("z mean: {0} sec".format(timer() - t0))
-        print("Amean shape (xy): {0}".format(Amean.shape))
-        print("Amean type: {0}".format(Amean.dtype))
+        print("Array mean shape (xy): {0}".format(array_mean.shape))
+        print("Array mean type: {0}".format(array_mean.dtype))
     else:
         print('\nCalculating rolling dF/F\n-----------------------')
-        lbound = int(win_size // 2)
-        ubound = int(win_size - lbound)
+        lower_bound = int(win_size // 2)
+        upper_bound = int(win_size - lower_bound)
         window = tca.windowFunc(width=win_size, win_type=win_type)[:, None]
-        window = np.repeat(window, A.shape[1], axis=1)
-        print("Upper bound frame: ", ubound, "Lower bound frame: ", lbound)
+        window = np.repeat(window, array.shape[1], axis=1)
+        print("Upper bound frame: ", upper_bound, "Lower bound frame: ",
+              lower_bound)
         print("Window shape (t,x*y): ", window.shape)
 
     t0 = timer()
-    A = A.astype('float32', copy=False)
+    array = array.astype('float32', copy=False)
     print("float32: {0} sec".format(timer() - t0))
 
     t0 = timer()
     t1 = timer()
     if win_size != None:
-        Amoving = A.copy()
-        for i in np.arange(A.shape[0]):
-            if i < lbound:
+        moving_array = array.copy()
+        for i in np.arange(array.shape[0]):
+            if i < lower_bound:
                 new_window = True
-                window = tca.windowFunc(width=ubound + i,
+                window = tca.windowFunc(width=upper_bound + i,
                                         win_type=win_type)[:, None]
-                window = np.repeat(window, A.shape[1], axis=1)
-                windprod = window * A[:i + ubound, :]
-            elif i > A.shape[0] - ubound:
+                window = np.repeat(window, array.shape[1], axis=1)
+                wind_product = window * array[:i + upper_bound, :]
+            elif i > array.shape[0] - upper_bound:
                 new_window = True
-                window = tca.windowFunc(width=lbound + A.shape[0] - i,
+                window = tca.windowFunc(width=lower_bound + array.shape[0] - i,
                                         win_type=win_type)[:, None]
-                window = np.repeat(window, A.shape[1], axis=1)
-                windprod = window * A[i - lbound:, :]
+                window = np.repeat(window, array.shape[1], axis=1)
+                wind_product = window * array[i - lower_bound:, :]
             else:
                 if new_window:
                     window = tca.windowFunc(width=win_size,
                                             win_type=win_type)[:, None]
-                    window = np.repeat(window, A.shape[1], axis=1)
+                    window = np.repeat(window, array.shape[1], axis=1)
                     new_window = False
-                windprod = np.multiply(window, A[i - lbound:i + ubound, :])
+                wind_product = np.multiply(
+                    window, array[i - lower_bound:i + upper_bound, :])
 
-            Amean = np.nansum(windprod, axis=0, dtype='float32')
+            array_mean = np.nansum(wind_product, axis=0, dtype='float32')
 
             if timer() - t1 > 300:
                 t1 = timer()
                 print(
                     '\tWorking on {0} frame, time passed: {1:.1f} secs'.format(
                         i,
                         timer() - t0))
-            Amoving[i, :] /= Amean
-            Amoving[i, :] -= 1.0
+            moving_array[i, :] /= array_mean
+            moving_array[i, :] -= 1.0
     else:
-        for i in np.arange(A.shape[0]):
-            A[i, :] /= Amean
-            A[i, :] -= 1.0
+        for i in np.arange(array.shape[0]):
+            array[i, :] /= array_mean
+            array[i, :] -= 1.0
 
     print("dfof normalization: {0} sec".format(timer() - t0))
     if reshape:
         if win_size != None:
-            A = np.reshape(Amoving, sz)
+            array = np.reshape(moving_array, sz)
         else:
-            A = np.reshape(A, sz)
-    print("A type: {0}".format(A.dtype))
-    print("A shape (t,x,y): {0}\n".format(A.shape))
-
-    return A
-
-
-def rescale(array,
-            low=3,
-            high=7,
-            cap=True,
-            mean_std=None,
-            mask=None,
-            maskval=1,
-            verbose=True,
-            min_max=None,
-            return_scale=False):
+            array = np.reshape(array, sz)
+    print("Array type: {0}".format(array.dtype))
+    print("Array shape (t,x,y): {0}\n".format(array.shape))
+
+    return array
+
+
+def rescale(array: np.ndarray,
+            low: float = 3,
+            high: float = 7,
+            cap: bool = True,
+            mean_std: Tuple[float, float] = None,
+            mask: np.ndarray = None,
+            maskval: float = 1,
+            verbose: bool = True,
+            min_max: bool = None,
+            return_scale: bool = False) -> Tuple[np.ndarray, dict]:
     '''
     determine upper and lower limits of colormap for playing movie files. 
     limits based on standard deviation from mean.  low, high are defined 
     in terms of standard deviation.  Image is updated in-place, 
     and doesn't have to be returned.
+
+    Arguments:
+        array: The array to rescale.
+        low: The number of standard deviations below to scale the range to.
+        high: The number of standard deviations above to scale the range to.
+        cap: If the dynamic range would be reduced, 
+            instead cap range to the minimum/maximum values present within the array.
+        mean_std: Use a given mean and standard deviation to apply the transformation, 
+            rather than gathering from the video.
+        mask: A mask to apply to the video when calculating the min/max range to scale by.
+        maskval: The value of the mask to include as signal.
+        verbose: Whether to print a verbose output.
+        min_max: Apply a specific min/max as the range, rather than calculating dyamically.
+        return_scale: Whether to return the resize scale which was applied.
+
+    Returns:
+        array: The rescaled array.
+            The original array should be updated in place as well.
+        scale: A dictionary containing all the scaling parameters.
+            Only returned if return_scale = True.
     '''
 
     if verbose:
         print('\nRescaling Movie\n-----------------------')
 
-    # Mask the region if mask provided
+    # Mask the region if mask provided.
     if mask is not None:
         copy = array.copy()
         array = get_masked_region(array, mask, maskval)
 
     if np.isnan(array).any():
         array[np.where(np.isnan(array))] = 0
 
-    # if unmasked color image, add extra temporary first dimension
+    # If unmasked color image, add extra temporary first dimension.
     if array.ndim == 3:
         if array.shape[2] == 3:
             array = array[None, :]
 
     if min_max is None:
         if mean_std is None:
             mean = np.nanmean(array, dtype=np.float64)
             std = np.nanstd(array, dtype=np.float64)
         else:
             mean = mean_std[0]
             std = mean_std[1]
 
-        newMin = mean - low * std
-        newMax = mean + high * std
+        new_min = mean - low * std
+        new_max = mean + high * std
         if verbose:
             print('mean:', mean, 'low:', low, 'high:', high, 'std:', std)
     else:
         assert len(min_max) == 2
-        newMin = min_max[0]
-        newMax = min_max[1]
+        new_min = min_max[0]
+        new_max = min_max[1]
 
     if verbose:
-        print('newMin:', newMin)
-        print('newMax', newMax)
+        print('new_min:', new_min)
+        print('new_max', new_max)
 
-    if cap:  # don't reduce dynamic range
+    if cap:  # Don't reduce dynamic range.
         if verbose:
             print('array min', np.nanmin(array))
-        if newMin < array.min():
-            newMin = array.min()
+        if new_min < array.min():
+            new_min = array.min()
             if verbose:
-                print('array min scaled', newMin)
+                print('array min scaled', new_min)
 
         if verbose:
             print('amax', np.nanmax(array))
-        if newMax > array.max():
-            newMax = array.max()
+        if new_max > array.max():
+            new_max = array.max()
             if verbose:
-                print('amax scaled', newMax)
+                print('amax scaled', new_max)
 
-    newSlope = 255.0 / (newMax - newMin)
+    new_slope = 255.0 / (new_max - new_min)
     if verbose:
-        print('newSlope:', newSlope)
-    array = array - newMin
-    array = array * newSlope
+        print('new_slope:', new_slope)
+    array = array - new_min
+    array = array * new_slope
 
     if mask is not None:
         array = insert_masked_region(copy, A, mask, maskval)
 
     array[np.where(array > 255)] = 255
     array[np.where(array < 0)] = 0
 
-    if array.shape[0] == 1:  #if was converted to one higher dimension
+    if array.shape[0] == 1:  # If was converted to one higher dimension.
         array = array[0, :]
 
     if verbose:
         print('\n')
 
     if not return_scale:
         return array
     else:
-        return array, {'scale': newSlope, 'min': newMin, 'max': newMax}
+        return array, {'scale': new_slope, 'min': new_min, 'max': new_max}
 
 
-def play(array,
-         textsavepath=None,
-         min_max=None,
-         preprocess=True,
-         overlay=None,
-         toolbarsMinMax=False,
-         rescale_movie=True,
-         cmap='default',
-         loop=True):
-    '''
-    play movie in opencv after normalizing display range
-    array is a numpy 3-dimensional movie
-    newMinMax is an optional tuple of length 2, the new display range
+def play(array: np.ndarray,
+         textsavepath: str = None,
+         min_max: Tuple[float, float] = None,
+         preprocess: bool = True,
+         overlay: np.ndarray = None,
+         min_max_toolbars: bool = False,
+         rescale_movie: bool = True,
+         cmap: np.ndarray = 'default',
+         loop: bool = True) -> None:
+    '''
+    Play movie in opencv after normalizing display range.
+
+    Arguments:
+        array: The (x,y,t or x,y,c,t) array to play as a movie.
+        textsavepath: An output to save time points to.
+        min_max: A specific min max value to scale the video to.
+        preprocess: Whether to preprocess the video, or calculate ranges dynamically.
+        overlay: An overlay frame to put on top of the video.
+        min_max_toolbars: Whether to display min/max slider toolbars for adjusting color range.
+        rescale_movie: Whether to rescale the movie.
+        cmap: The color map to apply.
+        loop: Whether to loop the video.
+
+    Returns:
+        None.
 
     Note: if preprocess is set to true, the array normalization is done 
     in place, thus the array will be rescaled outside scope of 
-    this function
+    this function.
     '''
-
     if colormap == 'default':
         colormap = DEFAULT_COLORMAP
 
     sz = array.shape
 
     def frameWrite(w, savepath=textsavepath):
         update = open(savepath, 'a', buffering=1)
@@ -653,27 +731,27 @@
         frameWrite(w='Start index, End index', savepath=textsavepath)
 
     if overlay is not None:
         o_values = np.unique(overlay)
         for val in o_values:
             if val not in [0, 1, 255]:
                 raise AssertionError('Overlay must be a 3d binary image.')
-        #create negative image
+        # Create negative image.
         overlay = overlay == 0
         overlay = overlay.astype(np.uint8)
 
     print('\nPlaying Movie\n-----------------------')
     assert (type(array) == np.ndarray), 'array was not a numpy array'
     assert (array.ndim == 3) | (array.ndim == 4), ('array was not three or '
                                                    'four-dimensional array')
 
     windowname = "Press Esc to Close"
     cv2.namedWindow(windowname, cv2.WINDOW_NORMAL)
     print('preprocessing data...')
-    #Create a resizable window
+    # Create a resizable window.
 
     sz = array.shape
 
     if array.ndim == 3:
         if min_max == None:
             # if min/max aren't set, default to 3 and 7
             lowB = [3]
@@ -681,37 +759,37 @@
         else:
             # otherwise, use values given
             lowB = min_max[0]
             highB = min_max[1]
 
         if rescale_movie == False:
             # if the movie shouldn't be rescaled, don't display rescaling toolbars
-            toolbarsMinMax = False
+            min_max_toolbars = False
         else:
             # mean, std not required if not rescaling
             mean = np.nanmean(A, dtype=np.float64)
             std = np.nanstd(A, dtype=np.float64)
 
         if preprocess:
             print('Pre-processing movie rescaling...')
             #Normalize movie range and change to uint8 before display
-            if toolbarsMinMax:
+            if min_max_toolbars:
                 imgclone = array.copy()
             t0 = timer()
             array = np.reshape(array, (sz[0], int(array.size / sz[0])))
             array = rescale(array,
                             low=lowB[0],
                             high=highB[0],
                             mean_std=(mean, std))
 
             array = np.reshape(array, sz)
             array = array.astype('uint8', copy=False)
             print("Movie range normalization: {0}".format(timer() - t0))
 
-        if toolbarsMinMax:
+        if min_max_toolbars:
 
             def updateColormap(array):
                 lowB[0] = 0.5 * (8 -
                                  cv2.getTrackbarPos("Low Limit", windowname))
                 highB[0] = 0.5 * cv2.getTrackbarPos("High Limit", windowname)
 
                 if preprocess:
@@ -752,36 +830,34 @@
                              high=highB[0],
                              mean_std=(mean, std),
                              verbose=False,
                              cap=False)
             color = np.zeros((im.shape[0], im.shape[1], 3))
             color = cv2.applyColorMap(im.astype('uint8'), cmap, color)
             if overlay is not None:
-                im *= overlay  # black:
-                # im[overlay==0]=255 # white
+                im *= overlay  # Black:
             cv2.putText(color, str(i), (5, 25), cv2.FONT_HERSHEY_SIMPLEX, 1.0,
-                        (255, 255, 255))  #draw frame text
+                        (255, 255, 255))  # Draw frame text.
             cv2.imshow(windowname, color)
 
         elif A.ndim == 4:
             if overlay is not None:
-                im *= overlay  # black:
-                # im[overlay==0]=255 # white
+                im *= overlay
             cv2.putText(im, str(i), (5, 25), cv2.FONT_HERSHEY_SIMPLEX, 1.0,
-                        (255, 255, 255))  #draw frame text
+                        (255, 255, 255))  #D raw frame text.
             cv2.imshow(windowname, im.astype('uint8'))
 
         k = cv2.waitKey(10)
-        if k == 27:  #if esc is pressed
+        if k == 27:  # If esc is pressed.
             break
         elif (k == ord(' ')) and (toggleNext == True):
             tf = False
         elif (k == ord(' ')) and (toggleNext == False):
             tf = True
-        toggleNext = tf  #toggle the switch
+        toggleNext = tf  # Toggle the switch.
 
         if k == ord("="):
             zoom = zoom * 1 / zfactor
         if k == ord("-"):
             zoom = zoom * zfactor
 
         if k == ord('b') and toggleNext:
@@ -819,41 +895,68 @@
             else:
                 print('Not a valid index. Try again.')
 
         elif toggleNext:
             i += 1
 
         if (i > (A.shape[0] - 1)) or (i < -1):
-            # reset to 0 if looping, otherwise break the while loop
+            # Reset to 0 if looping, otherwise break the while loop.
             if loop:
                 i = 0
             else:
                 break
 
     cv2.destroyAllWindows()
     for i in range(5):
         cv2.waitKey(1)
 
     print('\n')
 
-    if toolbarsMinMax:
+    if min_max_toolbars:
         return (lowB[0], highB[0])
 
 
-def scale_video(array, s_factor=1, t_factor=1, verbose=True, remainder=False):
+def scale_video(array: np.ndarray,
+                s_factor: int = 1,
+                t_factor: int = 1,
+                verbose: bool = True,
+                remainder: np.ndarray = False) -> Tuple[np.ndarray, np.ndarray]:
+    '''
+    Scale a video according to spatial and temporal resizing factors.
+
+    Arguments:
+        array: The array to rescale.
+        s_factor: The spatial factor to downsize by.
+        t_factor: The temporal factor to downsize by.
+        verbose: Whether to produce verbose print statements.
+        remainder: Whether to return a temporal remainder array.
+
+    Returns:
+        dsarray: The downsampled array.
+        remainder: A tempora remainder, 
+            in the dimensions and scale of the orignal video.
+    '''
+
     if verbose:
         print('\nRescaling Video\n-----------------------')
     assert array.ndim == 3, 'Input was not a video'
     shape = array.shape
 
     if s_factor == None:
         s_factor = 1
     if t_factor == None:
         t_factor = 1
 
+    if s_factor == 0:
+        print('WARNING: Spatial scaling factor was 0.  Reverting to 1.')
+        s_factor = 1
+    if t_factor == 0:
+        print('WARNING: Temporaldef  scaling factor was 0.  Reverting to 1.')
+        t_factor = 1
+
     if (s_factor == 1) and (t_factor == 1):
         print('No downsample factor given.')
         print('Returning array.')
 
         if remainder:
             return array, np.zeros(shape=(0, shape[1], shape[2]),
                                    dtype=array.dtype)
@@ -891,18 +994,35 @@
 
     if remainder:
         return dsarray, rmarray
     else:
         return dsarray
 
 
-def downsample(array, new_shape, keepdims=False):
-    # reshape m by n matrix by factor f by reshaping matrix into
-    # m f n f matricies, then applying sum across mxf, nxf matrices
-    # if keepdims, video is downsampled, but number of pixels remains the same.
+def downsample(array: np.ndarray,
+               new_shape: Tuple[int, int, int],
+               keepdims: bool = False) -> np.ndarray:
+    '''
+    Reshape m by n matrix by factor f by reshaping matrix into
+    m f n f matricies, then applying sum across mxf, nxf matrices
+    if keepdims, video is downsampled, but number of pixels remains the same.
+
+    The scale_video function is an application of this function, 
+    is more user friendly, and should be used in most cases.
+
+    Arguments:
+        array: The array to downsample.
+        new_shape: The new array shape to convert array to.
+        keepdims: Whether to keep the orignal dimensions.  
+            Only useful to differentiating whether downsample 
+            differences are just due to number of samples.
+
+    Returns:
+        array: The downsampled array.
+    '''
 
     if array.ndim != len(new_shape):
         raise ValueError("Shape mismatch: {} -> {}".format(
             array.shape, new_shape))
 
     array_shape = array.shape
 
@@ -920,18 +1040,28 @@
             ax = -1 * (2 * i + 1)
             n = array.shape[ax]
             array = array.mean(ax, keepdims=True)
             array = np.repeat(array, n, axis=ax)
 
         array = array.reshape(array_shape)
 
-    return (array)
+    return array
 
 
-def rotate(array, n):
+def rotate(array: np.ndarray, n: int) -> np.ndarray:
+    '''
+    Rotate an image or video n times counterclockwise.
+
+    Arguments:
+        array: The array to rotate.
+        n: The number of counterclockwise rotations.
+
+    Returns:
+        array: The array after rotation.
+    '''
 
     assert type(array) == np.ndarray
 
     if n > 0:
         ndim = array.ndim
 
         if ndim == 3:
```

### Comparing `seas-0.0.2/seas/waveletAnalysis.py` & `seas-0.0.3/seas/waveletAnalysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/usr/bin/env python3
-
+# TODO(@brmullen): Write documentation for this file.
 import sys
-#sys.path.insert(0, '/home/mike/Dropbox/0_firebird_research/fit_peaks/single_fits/')
 import numpy as np
 from seas.waveletFunctions import *
 import matplotlib.pylab as plt
 import matplotlib
 import math
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.gridspec import GridSpec
 from datetime import datetime
 from seas.signalanalysis import local_max, linear_regression, abline, gaussian_smooth_2d, lag_n_autocorr
-#sys.path.insert(0, '/home/mike/Dropbox/0_firebird_research/microburst_characterization/')
-#from src import remove_dropouts
+
 import operator
 
 #Adapted from __author__ = 'Mykhaylo Shumko' : __init__, waveletTransform, plotPower, lagNAutoCorr
-#All other functions written by Brian Mullen
+#All other functions written by Brian Mullen.
 '''
 To find the global wavelet spectrum run these two scripts:
     waveletAnalysis.globalWaveletSpectrum()
 
 To find events:
     Need to work on this. Depending on which range of frequencies, you get varying results
     waveletAnalysis.averageWaveletPower(periodLim =[0.25, 8])
@@ -36,47 +34,47 @@
 
     tc1 = np.asarray(np.squeeze(tc1))
     tc2 = np.asarray(np.squeeze(tc2))
 
     assert tc1.ndim == 1 and tc2.ndim == 1, 'Timecouses should only be one dimension'
     assert tc1.shape[0] == tc2.shape[0], 'Timecourses are not the same shape'
 
-    #run wavelet transform
+    # Run wavelet transform.
     w1 = waveletAnalysis(tc1, fps=fps)
     w2 = waveletAnalysis(tc2, fps=fps)
 
-    # cross wavelet transform
+    # Cross wavelet transform.
     w1w2 = w1.wave * np.conj(
         w2.wave)  #/ (np.ones([1, tc1.size]) * w1.scale[:, None])
     xwt = np.sqrt(w1w2.real**2 + w1w2.imag**2)
 
-    # calculate phase
+    # Calculate phase.
     phase = np.angle(w1w2)
 
-    # #set up smoothing window
+    # #et up smoothing window.
     # win_s = np.floor(w1.wave.shape[1]/w1.dj)+1
     # win_t = 2*np.floor(w1.wave.shape[0]/w1.cadence)+1
 
     # win_s = 10
     # win_t = 10
 
     # window2D = np.dot(windowFunc(win_t, win_type = 'ham')[:,np.newaxis] , windowFunc(win_s, win_type = 'ham')[:,np.newaxis].T)
 
-    #smooth
+    # Smooth.
     s1 = gaussian_smooth_2d(w1.power, w1.dj, w1.cadence)
     s2 = gaussian_smooth_2d(w2.power, w2.dj, w2.cadence)
     s1s2 = gaussian_smooth_2d(w1w2, w1.dj, w1.cadence)
 
-    #calculate coherency
+    # Calculate coherency.
     coherency = s1s2 / np.sqrt(s1 * s2)
 
-    #calculate coherence
+    # Calculate coherence.
     coherence = (s1s2.real**2 + s1s2.imag**2) / (s1 * s2)
 
-    # significance?
+    # Significance?
     acor1 = 0.5 * (lag_n_autocorr(tc1, 1) + lag_n_autocorr(tc1, 2))
     acor2 = 0.5 * (lag_n_autocorr(tc2, 1) + lag_n_autocorr(tc2, 2))
 
     xwt_signif = wave_cohere_signif(([1.0]), ([1.0]),
                                     dt=1 / fps,
                                     sigtest=sigtest,
                                     scale=w1.scale,
@@ -128,15 +126,15 @@
     if y_lag1 == -1:
         y_lag1 = 0.0
     if siglvl == -1:
         siglvl = 0.95
     if mother == -1:
         mother = 'MORLET'
 
-    # get the appropriate parameters [see Table(2)]
+    # Get the appropriate parameters [see Table(2)]
     if mother == 'MORLET':  #----------------------------------  Morlet
         empir = ([2, -1, -1, -1])
         if param == -1 or param == 6:
             param = 6.
             empir[1:] = ([0.776, 2.39, 0.60])
         if param == 4:
             empir[1:] = ([1.151, 2.5, 0.60])
@@ -159,166 +157,166 @@
             empir[1:] = ([1.966, 1.37, 0.97])
         m = param
         fourier_factor = 2 * np.pi * np.sqrt(2. / (2 * m + 1))
     else:
         print('Mother must be one of MORLET, PAUL, DOG')
 
     period = scale * fourier_factor
-    dofmin = empir[0]  # Degrees of freedom with no smoothing
-    Cdelta = empir[1]  # reconstruction factor
-    gamma_fac = empir[2]  # time-decorrelation factor
-    dj0 = empir[3]  # scale-decorrelation factor
-    freq = dt / period  # normalized frequency
+    dofmin = empir[0]  # Degrees of freedom with no smoothing.
+    Cdelta = empir[1]  # Reconstruction factor.
+    gamma_fac = empir[2]  # Time-decorrelation factor.
+    dj0 = empir[3]  # Scale-decorrelation factor.
+    freq = dt / period  # Normalized frequency.
 
     y_fft_theor = (1 - y_lag1**2) / (
         1 - 2 * y_lag1 * np.cos(freq * 2 * np.pi) + y_lag1**2)  # [Eqn(16)]
-    y_fft_theor = y_variance * y_fft_theor  # include time-series variance
+    y_fft_theor = y_variance * y_fft_theor  # Include time-series variance.
 
     x_fft_theor = (1 - x_lag1**2) / (
         1 - 2 * x_lag1 * np.cos(freq * 2 * np.pi) + x_lag1**2)  # [Eqn(16)]
-    x_fft_theor = x_variance * x_fft_theor  # include time-series variance
+    x_fft_theor = x_variance * x_fft_theor  # Include time-series variance.
 
     fft_theor = np.sqrt(y_fft_theor * x_fft_theor)
     signif = fft_theor
 
     if len(np.atleast_1d(dof)) == 1:
         if dof == -1:
             dof = dofmin
-    if sigtest == 0:  # no smoothing, DOF=dofmin [Sec.4]
+    if sigtest == 0:  # No smoothing, DOF=dofmin [Sec.4].
         dof = dofmin
         chisquare = chisquare_inv(siglvl, dof) / dof
         signif = fft_theor * chisquare  # [Eqn(18)]
-    elif sigtest == 1:  # time-averaged significance
+    elif sigtest == 1:  # Time-averaged significance.
         if len(np.atleast_1d(dof)) == 1:
             dof = np.zeros(J1) + dof
         dof[dof < 1] = 1
         dof = dofmin * np.sqrt(1 +
                                (dof * dt / gamma_fac / scale)**2)  # [Eqn(23)]
-        dof[dof < dofmin] = dofmin  # minimum DOF is dofmin
+        dof[dof < dofmin] = dofmin  # Minimum DOF is dofmin.
         for a1 in range(0, J1 + 1):
             chisquare = chisquare_inv(siglvl, dof[a1]) / dof[a1]
             signif[a1] = fft_theor[a1] * chisquare
-        # print("Chi squared: %e " % chisquare)
-    elif sigtest == 2:  # time-averaged significance
+    elif sigtest == 2:  # Time-averaged significance.
         if len(dof) != 2:
             print(
                 'ERROR: DOF must be set to [S1,S2], the range of scale-averages'
             )
         if Cdelta == -1:
             print('ERROR: Cdelta & dj0 not defined for ' + mother +
                   ' with param = ' + str(param))
 
         s1 = dof[0]
         s2 = dof[1]
-        avg = np.logical_and(scale >= s1, scale < s2)  # scales between S1 & S2
+        avg = np.logical_and(scale >= s1, scale < s2)  # Scales between S1 & S2.
         navg = np.sum(
             np.array(np.logical_and(scale >= s1, scale < s2), dtype=int))
         if navg == 0:
             print('ERROR: No valid scales between ' + str(s1) + ' and ' +
                   str(s2))
         Savg = 1. / np.sum(1. / scale[avg])  # [Eqn(25)]
-        Smid = np.exp((np.log(s1) + np.log(s2)) / 2.)  # power-of-two midpoint
+        Smid = np.exp((np.log(s1) + np.log(s2)) / 2.)  # Power-of-two midpoint.
         dof = (dofmin * navg * Savg / Smid) * np.sqrt(
             1 + (navg * dj / dj0)**2)  # [Eqn(28)]
         fft_theor = Savg * np.sum(fft_theor[avg] / scale[avg])  # [Eqn(27)]
         chisquare = chisquare_inv(siglvl, dof) / dof
         signif = (dj * dt / Cdelta / Savg) * fft_theor * chisquare  # [Eqn(26)]
     else:
         print('ERROR: sigtest must be either 0, 1, or 2')
 
     return signif
 
 
 def lagWaveletCoherency(tc1, tc2, fps=10, lag=5):
     for i in np.arange(0, lag + 1):
         if i == 0:
-            #initialize for proper shape
+            # Initialize for proper shape.
             cor, coh, xwt, phase, xwt_sig = waveletCoherence(tc1, tc2)
 
-            # create ouputs
+            # Create ouputs.
             lag_cor = np.zeros(
                 (2 * lag + 1, cor.shape[0], cor.shape[1])) * np.nan
             lag_coh = np.zeros(
                 (2 * lag + 1, cor.shape[0], cor.shape[1])) * np.nan
             lag_xwt = np.zeros(
                 (2 * lag + 1, cor.shape[0], cor.shape[1])) * np.nan
             lag_phase = np.zeros(
                 (2 * lag + 1, cor.shape[0], cor.shape[1])) * np.nan
             lag_xwt_sig = np.zeros(
                 (2 * lag + 1, cor.shape[0], cor.shape[1])) * np.nan
 
-            #store in the proper index
+            # Store in the proper index.
             lag_cor[lag] = cor
             lag_coh[lag] = coh
             lag_xwt[lag] = xwt
             lag_phase[lag] = phase
             lag_xwt_sig[lag] = xwt_sig
         else:
-            #finish up the remaining lags (right shifted)
+            # Finish up the remaining lags (right shifted).
             lag_cor[lag + i, : , i:], lag_coh[lag + i, : , i:], lag_xwt[lag + i, : , i:],\
             lag_phase[lag + i, : , i:], lag_xwt_sig[lag + i, : , i:] = waveletCoherence(tc1[i:],tc2[:-i], fps = fps)
 
-            #(left shifted)
+            # (Left shifted).
             lag_cor[lag - i, : , :-i],lag_coh[lag - i, : , :-i],lag_xwt[lag - i, : , :-i],\
             lag_phase[lag - i, : , :-i],lag_xwt_sig[lag - i, : , :-i] = waveletCoherence(tc1[:-i],tc2[i:], fps = fps)
 
     return lag_cor, lag_coh, lag_xwt, lag_phase, lag_xwt_sig
 
 
 class waveletAnalysis:
 
     def __init__(self, data, fps, **kwargs):
         """
-        Initialize the wavelet parameters
+        Initialize the wavelet parameters.
         """
 
         assert data.ndim == 1, 'Time series is the wrong shape. It should be a 1-dim vector'
 
         self.dataCopy = data
         self.data = (data - np.mean(data)) / np.std(data, ddof=1)
         self.n = len(self.data)
         self.cadence = 1 / fps
         self.time = np.arange(self.n) * self.cadence
 
-        #default parameters
-        #print/ plot statements
+        # Default parameters.
+        # Print/ plot statements.
         self.verbose = kwargs.get('verbose', False)
         self.plot = kwargs.get('plot', False)
 
-        #wavelet parameters
+        # Wavelet parameters.
         self.mother = kwargs.get('mother', 'MORLET')
         self.param = kwargs.get('param', 4)
         self.j1 = kwargs.get('j1', 80)
         self.pad = kwargs.get('pad', 1)
         self.dj = kwargs.get('dj', 0.125)
         self.s0 = kwargs.get('s0', 2 * self.cadence)
 
-        #noies modeling parameter
+        # Noise modeling parameter.
         self.siglvl = kwargs.get('siglvl', 0.95)
         self.lag1 = 0.5 * (lag_n_autocorr(data, 1) + lag_n_autocorr(data, 2))
         # self.lag1 = self.lagNAutoCorr(data, 1)
 
         self.waveletTransform()
 
     def waveletTransform(self):
         # Wavelet transform:
         self.wave, self.period, self.scale, self.coi = \
             wavelet(self.data, self.cadence, self.pad, self.dj, self.s0, self.j1, self.mother, self.param)
 
         if len(self.time) != len(self.coi):
             self.coi = self.coi[1:]
 
-        self.power = (np.abs(self.wave))**2  # compute wavelet power spectrum
+        self.power = (np.abs(self.wave))**2  # Compute wavelet power spectrum.
 
-        # Significance levels: (variance=1 for the normalized data)
+        # Significance levels: (variance=1 for the normalized data).
         self.signif = wave_signif(([1.0]), dt=self.cadence, sigtest=0, scale=self.scale, \
             lag1=self.lag1, mother=self.mother, siglvl = self.siglvl)
         self.sig95 = self.signif[:, np.newaxis].dot(
-            np.ones(self.n)[np.newaxis, :])  # expand signif --> (J+1)x(N) array
-        self.sig95 = self.power / self.sig95  # where ratio > 1, power is significant
+            np.ones(
+                self.n)[np.newaxis, :])  # Expand signif --> (J+1)x(N) array.
+        self.sig95 = self.power / self.sig95  # Where ratio > 1, power is significant.
         return
 
     def inverseWaveletTransform(self,
                                 waveFlt=None,
                                 C_d=1.151,
                                 psi0=np.pi**(-0.25) * 0.85):
         """
@@ -349,49 +347,49 @@
 
         if ax == None:
             f = plt.figure()
             f, ax = plt.subplots(1)
         else:
             ax = np.ravel(ax)[0]
 
-        # Max period is fourier_factor*S0*2^(j1*dj), fourier_factor = 3.97383530632
+        # Max period is fourier_factor*S0*2^(j1*dj), fourier_factor = 3.97383530632.
         CS = ax.contourf(self.time,
                          self.period,
                          np.log2(self.power),
                          len(self.levels),
                          colors=colors)
         im = ax.contourf(CS, levels=np.log2(self.levels), colors=colors)
         ax.set_xlabel('Time (s)')
         ax.set_ylabel('Period (s)')
         ax.set_title('Wavelet Power Spectrum')
-        # 95 significance contour, levels at -99 (fake) and 1 (95# signif)
+        # 95 significance contour, levels at -99 (fake) and 1 (95# signif).
         ax.contour(self.time, self.period, self.sig95, [-99, 1], colors='k')
-        # # cone-of-influence, anything "below" is dubious
+        # Cone-of-influence, anything "below" is dubious.
         ax.fill_between(self.time,
                         np.max(self.period),
                         self.coi,
                         alpha=0.5,
                         facecolor='white',
                         zorder=3)
         ax.plot(self.time, self.coi, 'k')
-        # # format y-scale
+        # Format y-scale.
 
-        # different matplotlib versions available for python < 3.8.
+        # Different matplotlib versions available for python < 3.8.
         try:
             ax.set_yscale('log', base=2, subs=None)
         except ValueError:
             ax.set_yscale('log', basey=2, subsy=None)
 
         ax.set_ylim([np.min(self.period), np.max(self.period)])
         axy = ax.yaxis
         axy.set_major_formatter(matplotlib.ticker.ScalarFormatter())
         ax.ticklabel_format(
             axis='y', style='plain')  ## causes issues with tkinter mpl canvas
         ax.invert_yaxis()
-        # set up the size and location of the colorbar
+        # Set up the size and location of the colorbar.
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("bottom", size="5%", pad=0.5)
         plt.colorbar(im, cax=cax, orientation='horizontal')
 
     def waveletFilter(self,
                       lowerPeriod=None,
                       upperPeriod=None,
@@ -405,17 +403,17 @@
         
         # WAVELET SCALE CALCULATOR ################# 
         # jth scale indicie = ln(S/S0)/(dJ * ln(2))
         ##################################    
         """
         self.waveFlt = self.wave.copy()
 
-        # Band pass filter
-        # Proporionally decreases power in specific wavelengths with respect to a 'motion vector'
-        # More motion, more severe the filtration of power in the given frequencies
+        # Band pass filter:
+        # Proporionally decreases power in specific wavelengths with respect to a 'motion vector'.
+        # More motion, more severe the filtration of power in the given frequencies.
         if movement_vector is not None:
             movement_vector -= movement_vector.min()
             movement_vector /= movement_vector.max()
             movement_vector = (1. - movement_vector)
 
             if lowerPeriod != None:
                 if lowerPeriod > self.period[0]:
@@ -426,68 +424,68 @@
             if upperPeriod != None:
                 if upperPeriod < self.period[-1]:
                     upper_ind = np.where(self.period > upperPeriod)[0][0]
                     #print('Upper Period: ', self.period[upper_ind], 'Lower Freq: ', 1/self.period[upper_ind])
                     self.waveFlt[upper_ind:, :] = self.waveFlt[
                         upper_ind:, :] * movement_vector
 
-        # Band pass filter
+        # Band pass filter:
         # Zero out parts of the wavlet space that we don't want to reconstruct.
         else:
             if lowerPeriod != None:
                 if lowerPeriod > self.period[0]:
                     lower_ind = np.where(self.period < lowerPeriod)[0][-1]
                     #print('Lower Period: ', self.period[lower_ind], 'Lower Freq: ', 1/self.period[lower_ind])
                     self.waveFlt[:lower_ind, :] = 0
             if upperPeriod != None:
                 if upperPeriod < self.period[-1]:
                     upper_ind = np.where(self.period > upperPeriod)[0][0]
                     #print('Upper Period: ', self.period[upper_ind], 'Upper Freq: ', 1/self.period[upper_ind])
                     self.waveFlt[upper_ind:, :] = 0
 
-        # Significance filter
+        # Significance filter:
         notSigInd = np.where(
             self.sig95 < sigLevel
         )  # Only pass data that has power of (100% - sigThreshold). Usually sigThreshold is 95%. Was 0.25.
         self.waveFlt[notSigInd] = 0
 
     ############################################
 
     def nanCOI(self):
-        # get rid of all values outside the cone of influence
+        # Get rid of all values outside the cone of influence.
         #   wave = np.log2(wave)
         self.nanCOImat = self.power.copy()
         for i in range(self.power.shape[1]):
             cutoff = np.where(self.coi[i] < self.period)
             self.nanCOImat[cutoff, i] = np.nan
 
     def nanSig(self):
-        # get rid of all values that are not significant
+        # Get rid of all values that are not significant.
         self.nanSigmat = self.wave
         self.nanSigmat[np.where(wavelet.sig95 < 1)] = np.nan
 
     def sigLost(self, slope, intercept):
         loss = 1 - (intercept + slope * self.n * self.cadence) / intercept
         if self.verbose:
             print('We have lost approximately {0:.2f} % power over the movie'.
                   format(loss[0] * 100))
 
         return loss
 
-    def binSignal(self, binsz=30):  # binsz in seconds
+    def binSignal(self, binsz=30):  # Bins in seconds.
         binnum = (self.n * self.cadence) // binsz
         padsz = math.ceil(float(self.n) / binnum) * binnum - self.n
         binsignal = np.append(self.signal, np.zeros(int(padsz)) * np.nan)
         binsignal = np.nanmean(binsignal.reshape(int(binnum), -1), axis=1)
         bintime = np.arange(binsz, self.n * self.cadence + 1, binsz) - binsz / 2
 
         return bintime, binsignal
 
     def familySig(self, sigList=[0.9, 0.95, 0.99, 0.999], dof=-1, sigtest=0):
-        # plot a family of significance curves for visualization and analysis
+        # Plot a family of significance curves for visualization and analysis.
 
         if isinstance(sigList, float):
             if sigtest < 2:
                 fam_signif = np.zeros((1, self.scale.shape[0])) * np.nan
             if sigtest == 2:
                 fam_signif = np.nan
             fam_signif = wave_signif([1.0],
@@ -517,15 +515,15 @@
                                             dof=dof,
                                             mother=self.mother,
                                             param=self.param)
 
         return np.squeeze(fam_signif), np.squeeze(sigList)
 
     def sumAcrossPeriod(self, perLim=[0, 100]):
-        #sum wavelet power across select periods
+        # Sum wavelet power across select periods.
 
         if self.verbose:
             print('Summing across {0} to {1} periods on wavelet run with mother {2} at paramter {3}'.\
                   format(perLim[0], perLim[1], self.mother, self.param) )
 
         cdelta = None
         if self.mother == 'MORLET' and self.param == 6:
@@ -553,17 +551,17 @@
         return np.squeeze(period_sum)
 
     def globalWaveletSpectrum(self):
         if self.verbose:
             print('Assessing wavelet mother {0} at paramter {1}'.format(
                 self.mother, self.param))
 
-        # calulate the global self spectrum
+        # Calulate the global self spectrum.
         self.nanCOI()
-        # if np.sum(~np.isnan(self.nanCOImat))!=0:
+        # If np.sum(~np.isnan(self.nanCOImat))!=0:.
         self.period_size = np.sum(~np.isnan(self.nanCOImat), axis=1)
         nan_ind = np.where(self.period_size == 0)[0]
         self.gws = np.zeros_like(self.period) * np.nan
         if nan_ind.any():
             self.gws[:nan_ind[0]] = np.nanmean(self.nanCOImat[:nan_ind[0], :],
                                                axis=1)
             self.gws[nan_ind] = 0
@@ -574,22 +572,22 @@
             dif = self.period_size.shape[0] - self.period.shape[0]
             if dif < 0:
                 self.period_size = np.append(self.period_size,
                                              np.zeros(np.abs(dif)))
             else:
                 self.period_size = self.period_size[:self.period.shape[0]]
 
-        # calculate the average significance
+        # Calculate the average significance.
         self.gws_sig, self.gws_sigList = self.familySig(sigList=[0.95],
                                                         dof=self.period_size,
                                                         sigtest=1)
 
         if self.verbose:
             print('Auto-correlation value: {0:.4g}'.format(self.lag1))
-        # determine fourier wavelength
+        # Determine fourier wavelength.
         if self.mother == 'DOG':
             self.flambda = (2 * np.pi * 1 / self.period) / np.sqrt(self.param +
                                                                    .5)
         if self.mother == 'MORLET':
             self.flambda = (4 * np.pi * 1 / self.period) / (
                 self.param + np.sqrt(2 + np.square(self.param)))
 
@@ -605,15 +603,15 @@
                 lgws.append(mx_gws[i])
                 lfl.append(fl_wav[i])
         lwav_inv = [x**(-1) for x in lwav]
 
         self.gws_localmax_power = lgws
         self.gws_localmax_freq = lfl
 
-        #find the lowest and highest frequencies that are still significant
+        # Find the lowest and highest frequencies that are still significant.
         hiwav = np.nan
         hival = np.nan
         lowav = np.nan
         loval = np.nan
 
         if np.where(self.gws > self.gws_sig)[0].shape[0] > 0:
             hival = self.gws[np.where(self.gws > self.gws_sig)][0]
@@ -634,15 +632,15 @@
         if self.plot:
             fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(8, 4), sharey=True)
             nyq = 0.5 * 1 / self.cadence
             linetype = ['-', '-.', '--', ':']
             fam_signif, sigList = self.familySig(dof=self.period_size,
                                                  sigtest=1)
 
-            #self period graph
+            # Self period graph.
             ax1.plot(self.period, self.gws)
             ax1.plot(lwav, lgws, 'ro')
 
             for i in range(len(sigList)):
                 if i >= len(linetype) - 1:
                     j = len(linetype) - 1
                 else:
@@ -688,15 +686,15 @@
             #         else:
             #             plt.xlim([0, np.ceil(max(lwav_inv))])
             #         plt.xlabel(self.mother + ' frequency')
             #         plt.ylabel('normalized power (to variance)')
             #         plt.legend()
             #         plt.show()
 
-            #Fourier space lambda
+            # Fourier space lambda.
             ax2.plot(self.flambda, self.gws)
             for i in range(len(sigList)):
                 if i >= len(linetype) - 1:
                     j = len(linetype) - 1
                 else:
                     j = i
                 ax2.plot(self.flambda,
@@ -749,18 +747,18 @@
         # calculate the average significance
 
     #     sig = wavelet.signif/np.sqrt(1+((self.period_size * wavelet.cadence)/(gamma * wavelet.period)))
         self.sig_period_sum, _ = self.familySig(sigList=[0.95],
                                                 dof=periodLim,
                                                 sigtest=2)
 
-        #find coordinates of local max values
+        # Find coordinates of local max values.
         mx_wav, mx_gws = local_max(self.time, self.period_sum)
 
-        #Return only those above significance threshold
+        # Return only those above significance threshold.
         ltime = []
         lgws = []
         for i in range(len(mx_wav)):
             if mx_gws[i] > self.sig_period_sum:
                 ltime.append(mx_wav[i])
                 lgws.append(mx_gws[i])
         if self.plot:
@@ -778,20 +776,20 @@
 
         self.events = ltime
         self.events_value = lgws
 
     def tsSignal(self, binSig=False, periodLim=[0.5, 4]):
         '''
         Using wavelet transforms to assess how the power of signal changes 
-        over time
+        over time.
         '''
         self.binSig = binSig
         assert len(periodLim) == 2, 'Period limits are wrong size'
 
-        #determine the time and power across neural signal periods
+        # Determine the time and power across neural signal periods.
         self.signal = self.sumAcrossPeriod(perLim=periodLim)
         self.signal_sig, _ = self.familySig(sigList=[0.95],
                                             dof=periodLim,
                                             sigtest=2)
 
         if self.binSig:
             bintime, binsignal = self.binSignal()
@@ -827,15 +825,15 @@
     def noiseFilter(self,
                     lowerPeriod=None,
                     upperPeriod=10,
                     movement_vector=None,
                     sigLevel=0.25):
 
         if lowerPeriod is None:
-            lowerPeriod = 2 * self.cadence  #nyquist sampling rate
+            lowerPeriod = 2 * self.cadence  # Nyquist sampling rate.
 
         if movement_vector is not None:
             movement_vector = np.array(np.squeeze(movement_vector),
                                        dtype='float64')
             assert movement_vector.shape[
                 0] == self.n, 'Movement vector is not the same size as the data'
```

### Comparing `seas-0.0.2/seas/waveletFunctions.py` & `seas-0.0.3/seas/waveletFunctions.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.2/seas.egg-info/PKG-INFO` & `seas-0.0.3/seas.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: seas
-Version: 0.0.2
+Version: 0.0.3
 Summary: python Signal Extraction and Segmentation
 Home-page: https://github.com/ackmanlab/pySEAS
 Author: Sydney Weiser
 Author-email: scweiser@ucsc.edu
 License: UNKNOWN
-Description: Data-driven filtration and segmentation of mesoscale neural dynamics
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Data-driven filtration and segmentation of mesoscale neural dynamics
+
```

### Comparing `seas-0.0.2/seas.egg-info/SOURCES.txt` & `seas-0.0.3/seas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 seas/__init__.py
 seas/colormaps.py
 seas/defaults.py
 seas/domains.py
```

### Comparing `seas-0.0.2/setup.py` & `seas-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seas",
-    version="0.0.2",
+    version="0.0.3",
     author="Sydney Weiser",
     author_email="scweiser@ucsc.edu",
     description="python Signal Extraction and Segmentation",
     long_description="Data-driven filtration and segmentation of mesoscale neural dynamics",
     long_description_content_type="text/markdown",
     url="https://github.com/ackmanlab/pySEAS",
     packages=setuptools.find_packages(),
@@ -24,11 +24,11 @@
         'numpy',
         'opencv-python',
         'PyYAML',
         'scikit-learn',
         'scipy',
         'sklearn',
         'tifffile',
-        'tk'
+        'tk',
     ],
     python_requires='>=3.5',
 )
```

### Comparing `seas-0.0.2/tests/colormaps_test.py` & `seas-0.0.3/tests/colormaps_test.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.2/tests/experiment_test.py` & `seas-0.0.3/tests/experiment_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,12 +65,13 @@
     exp = seas.experiment.Experiment(pathlist=test_video_path)
     exp.load_rois('fake_roi_path')
     exp.define_mask_boundaries()
     results = exp.ica_project(n_components=10)
 
     assert 'eig_mix' in results
 
+
 def test_ica_decompose_without_rois_n_components():
     exp = seas.experiment.Experiment(pathlist=test_video_path)
     results = exp.ica_project(n_components=10)
 
     assert 'eig_mix' in results
```

### Comparing `seas-0.0.2/tests/filemanager_test.py` & `seas-0.0.3/tests/filemanager_test.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.2/tests/video_test.py` & `seas-0.0.3/tests/video_test.py`

 * *Files identical despite different names*

