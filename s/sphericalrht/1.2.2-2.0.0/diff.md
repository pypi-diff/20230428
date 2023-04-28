# Comparing `tmp/sphericalrht-1.2.2.tar.gz` & `tmp/sphericalrht-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/users/georgech/sphericalrht/dist/tmp17ql3doc/sphericalrht-1.2.2.tar", last modified: Thu Jul  7 01:13:48 2022, max compression
+gzip compressed data, was "/home/users/georgech/sphericalrht/dist/.tmp-fl9m5toc/sphericalrht-2.0.0.tar", last modified: Fri Apr 28 01:32:07 2023, max compression
```

## Comparing `sphericalrht-1.2.2.tar` & `sphericalrht-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.529955 sphericalrht-1.2.2/
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.257736 sphericalrht-1.2.2/.github/
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.361058 sphericalrht-1.2.2/.github/workflows/
--rw-r--r--   0 georgech (355130) seclark1 (377337)      969 2021-11-09 19:57:02.000000 sphericalrht-1.2.2/.github/workflows/tests.yml
--rw-r--r--   0 georgech (355130) seclark1 (377337)     1056 2021-11-04 19:06:51.000000 sphericalrht-1.2.2/LICENSE
--rw-r--r--   0 georgech (355130) seclark1 (377337)      196 2021-11-09 22:55:35.000000 sphericalrht-1.2.2/MANIFEST.in
--rw-r--r--   0 georgech (355130) seclark1 (377337)     2923 2022-07-07 01:13:48.531583 sphericalrht-1.2.2/PKG-INFO
--rw-r--r--   0 georgech (355130) seclark1 (377337)     2100 2021-11-12 01:13:46.000000 sphericalrht-1.2.2/README.md
--rw-r--r--   0 georgech (355130) seclark1 (377337)     6899 2022-07-07 01:04:26.000000 sphericalrht-1.2.2/README.rst
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.382014 sphericalrht-1.2.2/docs/
--rw-r--r--   0 georgech (355130) seclark1 (377337)      638 2021-11-08 16:39:26.000000 sphericalrht-1.2.2/docs/Makefile
--rw-r--r--   0 georgech (355130) seclark1 (377337)      834 2021-11-08 16:39:52.000000 sphericalrht-1.2.2/docs/make.bat
--rw-r--r--   0 georgech (355130) seclark1 (377337)      538 2022-03-04 19:57:24.000000 sphericalrht-1.2.2/pyproject.toml
--rw-r--r--   0 georgech (355130) seclark1 (377337)       69 2021-11-05 18:58:31.000000 sphericalrht-1.2.2/requirements.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)      110 2021-11-09 05:49:42.000000 sphericalrht-1.2.2/requirements_dev.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)     1164 2022-07-07 01:13:48.538371 sphericalrht-1.2.2/setup.cfg
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.267937 sphericalrht-1.2.2/src/
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.416682 sphericalrht-1.2.2/src/sphericalrht/
--rw-r--r--   0 georgech (355130) seclark1 (377337)      891 2022-07-07 01:12:12.000000 sphericalrht-1.2.2/src/sphericalrht/__init__.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-04 20:48:45.000000 sphericalrht-1.2.2/src/sphericalrht/py.typed
--rw-r--r--   0 georgech (355130) seclark1 (377337)    19708 2022-07-07 01:12:21.000000 sphericalrht-1.2.2/src/sphericalrht/spherical_rht.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)      900 2022-07-07 01:12:00.000000 sphericalrht-1.2.2/src/sphericalrht/utils.py
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.461310 sphericalrht-1.2.2/src/sphericalrht.egg-info/
--rw-r--r--   0 georgech (355130) seclark1 (377337)     2923 2022-07-07 01:13:48.000000 sphericalrht-1.2.2/src/sphericalrht.egg-info/PKG-INFO
--rw-r--r--   0 georgech (355130) seclark1 (377337)      636 2022-07-07 01:13:48.000000 sphericalrht-1.2.2/src/sphericalrht.egg-info/SOURCES.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)        1 2022-07-07 01:13:48.000000 sphericalrht-1.2.2/src/sphericalrht.egg-info/dependency_links.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)      132 2022-07-07 01:13:48.000000 sphericalrht-1.2.2/src/sphericalrht.egg-info/requires.txt
--rw-r--r--   0 georgech (355130) seclark1 (377337)       13 2022-07-07 01:13:48.000000 sphericalrht-1.2.2/src/sphericalrht.egg-info/top_level.txt
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.495614 sphericalrht-1.2.2/tests/
--rw-r--r--   0 georgech (355130) seclark1 (377337)       86 2022-07-07 01:12:34.000000 sphericalrht-1.2.2/tests/__init__.py
-drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2022-07-07 01:13:48.521672 sphericalrht-1.2.2/tests/data/
--rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-11 23:22:43.000000 sphericalrht-1.2.2/tests/data/__init__.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)     8640 2021-11-11 23:12:34.000000 sphericalrht-1.2.2/tests/data/test_map.fits
--rw-r--r--   0 georgech (355130) seclark1 (377337)     8640 2022-03-04 04:47:55.000000 sphericalrht-1.2.2/tests/data/test_map2.fits
--rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-07 01:49:54.000000 sphericalrht-1.2.2/tests/py.typed
--rw-r--r--   0 georgech (355130) seclark1 (377337)     6090 2022-03-04 19:48:27.000000 sphericalrht-1.2.2/tests/test_spherical_rht.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)      754 2021-11-12 01:46:19.000000 sphericalrht-1.2.2/tests/test_utils.py
--rw-r--r--   0 georgech (355130) seclark1 (377337)      486 2021-11-09 19:56:12.000000 sphericalrht-1.2.2/tox.ini
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.847927 sphericalrht-2.0.0/
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.566987 sphericalrht-2.0.0/.github/
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.672497 sphericalrht-2.0.0/.github/workflows/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      969 2021-11-09 19:57:02.000000 sphericalrht-2.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     1056 2021-11-04 19:06:51.000000 sphericalrht-2.0.0/LICENSE
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      196 2021-11-09 22:55:35.000000 sphericalrht-2.0.0/MANIFEST.in
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     2923 2023-04-28 01:32:07.849035 sphericalrht-2.0.0/PKG-INFO
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     2100 2021-11-12 01:13:46.000000 sphericalrht-2.0.0/README.md
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     7108 2023-04-28 01:05:27.000000 sphericalrht-2.0.0/README.rst
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.735565 sphericalrht-2.0.0/docs/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      638 2021-11-08 16:39:26.000000 sphericalrht-2.0.0/docs/Makefile
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      834 2021-11-08 16:39:52.000000 sphericalrht-2.0.0/docs/make.bat
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      538 2022-03-04 19:57:24.000000 sphericalrht-2.0.0/pyproject.toml
+-rw-r--r--   0 georgech (355130) seclark1 (377337)       69 2021-11-05 18:58:31.000000 sphericalrht-2.0.0/requirements.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      110 2021-11-09 05:49:42.000000 sphericalrht-2.0.0/requirements_dev.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     1164 2023-04-28 01:32:07.853917 sphericalrht-2.0.0/setup.cfg
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.572491 sphericalrht-2.0.0/src/
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.771396 sphericalrht-2.0.0/src/sphericalrht/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      891 2023-04-28 01:24:05.000000 sphericalrht-2.0.0/src/sphericalrht/__init__.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-04 20:48:45.000000 sphericalrht-2.0.0/src/sphericalrht/py.typed
+-rw-r--r--   0 georgech (355130) seclark1 (377337)    20597 2023-04-28 01:26:53.000000 sphericalrht-2.0.0/src/sphericalrht/spherical_rht.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      900 2023-04-28 01:24:47.000000 sphericalrht-2.0.0/src/sphericalrht/utils.py
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.797264 sphericalrht-2.0.0/src/sphericalrht.egg-info/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     2923 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/PKG-INFO
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      636 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/SOURCES.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)        1 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/dependency_links.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      132 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/requires.txt
+-rw-r--r--   0 georgech (355130) seclark1 (377337)       13 2023-04-28 01:32:07.000000 sphericalrht-2.0.0/src/sphericalrht.egg-info/top_level.txt
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.818540 sphericalrht-2.0.0/tests/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)       86 2023-04-28 01:25:10.000000 sphericalrht-2.0.0/tests/__init__.py
+drwxr-xr-x   0 georgech (355130) seclark1 (377337)        0 2023-04-28 01:32:07.840874 sphericalrht-2.0.0/tests/data/
+-rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-11 23:22:43.000000 sphericalrht-2.0.0/tests/data/__init__.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     8640 2021-11-11 23:12:34.000000 sphericalrht-2.0.0/tests/data/test_map.fits
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     8640 2023-04-28 01:22:20.000000 sphericalrht-2.0.0/tests/data/test_map2.fits
+-rw-r--r--   0 georgech (355130) seclark1 (377337)        0 2021-11-07 01:49:54.000000 sphericalrht-2.0.0/tests/py.typed
+-rw-r--r--   0 georgech (355130) seclark1 (377337)     6185 2023-04-28 01:03:00.000000 sphericalrht-2.0.0/tests/test_spherical_rht.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      754 2021-11-12 01:46:19.000000 sphericalrht-2.0.0/tests/test_utils.py
+-rw-r--r--   0 georgech (355130) seclark1 (377337)      486 2021-11-09 19:56:12.000000 sphericalrht-2.0.0/tox.ini
```

### Comparing `sphericalrht-1.2.2/.github/workflows/tests.yml` & `sphericalrht-2.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/LICENSE` & `sphericalrht-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/PKG-INFO` & `sphericalrht-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphericalrht
-Version: 1.2.2
+Version: 2.0.0
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
-Metadata-Version: 2.1 Name: sphericalrht Version: 1.2.2 Summary: Spherical
+Metadata-Version: 2.1 Name: sphericalrht Version: 2.0.0 Summary: Spherical
 implementation of the Rolling Hough Transform Home-page: https://github.com/
 georgehalal/sphericalrht Author: George Halal Author-email:
 halalgeorge@gmail.com Project-URL: Bug Tracker, https://github.com/georgehalal/
 sphericalrht/issues Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `sphericalrht-1.2.2/README.md` & `sphericalrht-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/README.rst` & `sphericalrht-2.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,19 @@
   account, weighted by their intensity.
 
 ``norients``: int
   angular resolution given by the number of orientations to consider. We
   have found empirically that ``norients`` = 25 is sufficient for most
   applications.
 
+``mask``: Union[str, np.ndarray]
+  either a path to the map or an array of the map pixels. This defines
+  the mask for maps that are not defined over the entire sky. The map
+  ordering is assumed to be RING.
+
 ``weighting``: Union[str, np.ndarray]
   either a path to the map or an array of the map pixels. This is used as the
   weight for the output Stokes Q/U maps. The map ordering is assumed to be RING.
 
 ``overwrite``: bool
   whether to overwrite outputs of same name if they already exist.
```

#### html2text {}

```diff
@@ -29,47 +29,50 @@
 the orientation). ``fwhm``: float scale [arcmins] for the unsharp mask applied
 to pick out filamentary structure. ``thresh``: float threshold fraction of the
 window diameter between 0-1 applied to the result of the convolution. Higher
 thresholds focus on the main orientations only, while lower thresholds take
 more orientations into account, weighted by their intensity. ``norients``: int
 angular resolution given by the number of orientations to consider. We have
 found empirically that ``norients`` = 25 is sufficient for most applications.
-``weighting``: Union[str, np.ndarray] either a path to the map or an array of
-the map pixels. This is used as the weight for the output Stokes Q/U maps. The
-map ordering is assumed to be RING. ``overwrite``: bool whether to overwrite
-outputs of same name if they already exist. ``split_factor``: int number of
-data splits to save on runtime memory usage. Default value is based on the
-requested NSIDE (1 for NSIDE < 4096). If your job runs out of memory and you
-can't request more memory per job, increase the split factor. ===== Usage =====
-The code runs in parallel on as many CPUs as available, so feel free to request
-many CPUs when submitting a job. The runtime and memory increase as O
-(``nside``\ :sup:`2` * ``norients``). The ``split_factor`` can be used to
-decrease the memory complexity and increase the time complexity as O
-(``split_factor``). The other input parameters have a negligible effect on the
-time and memory complexity. The polarization convention is COSMO with the
-polarization being perpendicular to the filaments in the map in the plane of
-the sky. To obtain polarization maps corresponding to the IAU convention,
-multiply U by -1. To obtain polarization maps parallel to the orientation of
-the filaments (e.g. magnetic field orientation) in the COSMO convention,
-multiply both Q and U by -1. Example 1 --------- Here's one way to run the
-algorithm with all the input parameters: .. code-block:: python from
-sphericalrht import CubeAndStokes cube_and_stokes = CubeAndStokes( in_map="/
-path/to/map_name.fits", nside=1024, out_dir="/path/to/output_dir", wlen=75,
-fwhm=30, thresh=0.7, norients=25, weighting="/path/to/weighting_map.fits"
-overwrite=False, split_factor=1) cube_and_stokes.build_and_save() Example 2 ---
------- If your input map is an array instead of a .fits file, you can enter a
-tuple with the array in the first entry and the name as the second entry as
-shown in this example that uses only the required input parameters: .. code-
-block:: python import h5py with h5py.File("/path/to/map_name.h5", "r") as f:
-intensity = f["I"][:, 0] from sphericalrht import CubeAndStokes cube_and_stokes
-= CubeAndStokes( in_map=(intensity, "map_name"), nside=1024, out_dir="/path/to/
-output_dir") cube_and_stokes.build_and_save() Reading the results -------------
------- .. code-block:: python # Load the output maps import healpy as hp
-out_name = "map_name_nside1024_wlen75_fwhm30_thresh0.7_norients25" I, Q, U =
-hp.read_map( f"/path/to/output_dir/IQU_{out_name}.fits", field=(0,1,2)) # If
-you'd like, you can also load the output of # all orientation angles for each
-pixel import h5py with h5py.File("/path/to/output_dir/{out_name}.h5") as
-cube_file: spherical_rht_out = cube_file["spherical_rht_cube"][:, PIXEL_INDEX]
+``mask``: Union[str, np.ndarray] either a path to the map or an array of the
+map pixels. This defines the mask for maps that are not defined over the entire
+sky. The map ordering is assumed to be RING. ``weighting``: Union[str,
+np.ndarray] either a path to the map or an array of the map pixels. This is
+used as the weight for the output Stokes Q/U maps. The map ordering is assumed
+to be RING. ``overwrite``: bool whether to overwrite outputs of same name if
+they already exist. ``split_factor``: int number of data splits to save on
+runtime memory usage. Default value is based on the requested NSIDE (1 for
+NSIDE < 4096). If your job runs out of memory and you can't request more memory
+per job, increase the split factor. ===== Usage ===== The code runs in parallel
+on as many CPUs as available, so feel free to request many CPUs when submitting
+a job. The runtime and memory increase as O(``nside``\ :sup:`2` *
+``norients``). The ``split_factor`` can be used to decrease the memory
+complexity and increase the time complexity as O(``split_factor``). The other
+input parameters have a negligible effect on the time and memory complexity.
+The polarization convention is COSMO with the polarization being perpendicular
+to the filaments in the map in the plane of the sky. To obtain polarization
+maps corresponding to the IAU convention, multiply U by -1. To obtain
+polarization maps parallel to the orientation of the filaments (e.g. magnetic
+field orientation) in the COSMO convention, multiply both Q and U by -1.
+Example 1 --------- Here's one way to run the algorithm with all the input
+parameters: .. code-block:: python from sphericalrht import CubeAndStokes
+cube_and_stokes = CubeAndStokes( in_map="/path/to/map_name.fits", nside=1024,
+out_dir="/path/to/output_dir", wlen=75, fwhm=30, thresh=0.7, norients=25,
+weighting="/path/to/weighting_map.fits" overwrite=False, split_factor=1)
+cube_and_stokes.build_and_save() Example 2 --------- If your input map is an
+array instead of a .fits file, you can enter a tuple with the array in the
+first entry and the name as the second entry as shown in this example that uses
+only the required input parameters: .. code-block:: python import h5py with
+h5py.File("/path/to/map_name.h5", "r") as f: intensity = f["I"][:, 0] from
+sphericalrht import CubeAndStokes cube_and_stokes = CubeAndStokes( in_map=
+(intensity, "map_name"), nside=1024, out_dir="/path/to/output_dir")
+cube_and_stokes.build_and_save() Reading the results ------------------- ..
+code-block:: python # Load the output maps import healpy as hp out_name =
+"map_name_nside1024_wlen75_fwhm30_thresh0.7_norients25" I, Q, U = hp.read_map
+( f"/path/to/output_dir/IQU_{out_name}.fits", field=(0,1,2)) # If you'd like,
+you can also load the output of # all orientation angles for each pixel import
+h5py with h5py.File("/path/to/output_dir/{out_name}.h5") as cube_file:
+spherical_rht_out = cube_file["spherical_rht_cube"][:, PIXEL_INDEX]
 ======================== References & Attribution ======================== The
 paper introducing this package is in preparation. If you make use of this code
 in your research, please contact halalgeorge@gmail.com for discussing proper
 citations.
```

### Comparing `sphericalrht-1.2.2/docs/Makefile` & `sphericalrht-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/docs/make.bat` & `sphericalrht-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/pyproject.toml` & `sphericalrht-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/setup.cfg` & `sphericalrht-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sphericalrht
-version = 1.2.2
+version = 2.0.0
 author = George Halal
 author_email = halalgeorge@gmail.com
 description = Spherical implementation of the Rolling Hough Transform
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/georgehalal/sphericalrht
 project_urls =
```

### Comparing `sphericalrht-1.2.2/src/sphericalrht/__init__.py` & `sphericalrht-2.0.0/src/sphericalrht/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
 from .spherical_rht import StokesQU, CubeAndStokes
 from .utils import set_logger
 
 
 __author__ = "George Halal"
 __email__ = "halalgeorge@gmail.com"
-__version__ = "1.2.1"
+__version__ = "2.0.0"
 __all__ = ["StokesQU", "CubeAndStokes", "set_logger"]
```

### Comparing `sphericalrht-1.2.2/src/sphericalrht/spherical_rht.py` & `sphericalrht-2.0.0/src/sphericalrht/spherical_rht.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,22 @@
         if necessary).
     CubeAndStokes: Define an instance of this class with input
         parameters, then use the build_and_save method to run
         the algorthm.
 
 Author: George Halal
 Email: halalgeorge@gmail.com
-Date: 07/06/2022
-Version: 1.2.2
+Date: 04/27/2023
+Version: 2.0.0
 """
 
 
 __author__ = "George Halal"
 __email__ = "halalgeorge@gmail.com"
-__version__ = "1.2.1"
+__version__ = "2.0.0"
 __all__ = ["StokesQU", "CubeAndStokes"]
 
 
 import os
 import time
 from collections import deque
 import logging
@@ -127,14 +127,15 @@
             and saving the resulting cube and maps.
     """
 
     def __init__(self, in_map: Union[str, Tuple[np.ndarray, str]], nside: int,
                  out_dir: str, wlen: int = 75, fwhm: float = 30.,
                  thresh: float = 0.7, norients: int = 25,
                  weighting: Optional[Union[str, np.ndarray]] = None,
+                 mask: Optional[Union[str, np.ndarray]] = None,
                  overwrite: bool = False,
                  split_factor: Optional[int] = None) -> None:
         """Define necessary variables based on the input arguments and
         make necessary directories.
 
         Parameters:
             in_map (str or tuple(np.ndarray((Npix,)), str)): either
@@ -154,14 +155,17 @@
             thresh (float): threshold fraction of the window diameter
                 between 0-1 applied to the result of the convolution.
                 Higher thresholds focus on the main orientations only,
                 while lower thresholds take more orientations into
                 account, weighted by their intensity.
             norients (int): angular resolution given by the number of
                 orientations to consider.
+            mask (str or np.ndarray((Npix,))): either a path to the map
+                or an array of the map pixels. This defines the mask for
+                maps that are not defined over the entire sky. 
             weighting (str or np.ndarray((Npix,))): either a path to the
                 map or an array of the map pixels. This is used as the
                 weight for the output Stokes Q/U maps. The map ordering
                 is assumed to be RING.
             overwrite (bool): whether to overwrite outputs of same name
                 if they already exist.
             split_factor (int): number of convolution splits to save on
@@ -179,14 +183,28 @@
             self.name = in_map.split("/")[-1].split(".fits")[0]
         else:
             self.in_map = in_map[0]
             self.name = in_map[1]
             assert np.sqrt(self.in_map.shape[0]/12) % 1 == 0, (
                "Input map has the wrong shape or number of pixels.")
 
+        if mask is not None:
+            assert isinstance(mask, str) or isinstance(mask, np.ndarray), (
+                "Mask must be a path or a np.ndarray")
+            if isinstance(mask, str):
+                assert os.path.exists(mask), (
+                    "Mask does not exist. Check path and try again.")
+                self.mask = hp.read_map(mask, field=(0))
+            else:
+                self.mask = mask
+                assert self.mask.shape[0] == self.in_map.shape[0], (
+                   "Mask has the wrong number of pixels.")
+        else:
+            self.mask = np.ones_like(self.in_map)
+
         assert nside % 1 == 0 and nside > 0, "NSIDE must be a positive integer"
         self.nside = int(nside)
 
         assert isinstance(out_dir, str), "Output directory must be a str"
         if not os.path.exists(out_dir):
             os.makedirs(out_dir)
         self.out_dir = out_dir
@@ -219,16 +237,16 @@
                     self.weighting = self.in_map
                 else:
                     self.weighting = hp.read_map(weighting, field=(0))
             else:
                 assert np.sqrt(weighting.shape[0]/12) % 1 == 0, (
                     "Weighting map has the wrong shape or number of pixels.")
                 self.weighting = weighting
-        else:
-            self.weighting = self.in_map
+            if hp.get_nside(self.weighting) != self.nside:
+                self.weighting = hp.ud_grade(self.weighting, self.nside)
 
         self.overwrite = overwrite
 
         if split_factor is not None:
             assert split_factor % 1 == 0 and split_factor > 0, (
                 "Split factor must be a positive integer")
             self.split_factor = int(split_factor)
@@ -259,55 +277,53 @@
         Parameters:
             original_map (np.ndarray((Npix,))): map to
                 high-pass filter
 
         Returns:
             high-pass filtered map of 1s and 0s (np.ndarray)
         """
+        original_map[original_map != original_map] = 0
+
         smoothed_map = hp.smoothing(
-            original_map, fwhm=np.radians(self.fwhm / 60.))
-        subtracted_map = original_map - smoothed_map
+            original_map * self.mask, fwhm=np.radians(self.fwhm / 60.))
+        
+        subtracted_map = original_map*self.mask - smoothed_map
 
         return (subtracted_map > 0.).astype(int)
 
     def prep_intensity(self, return_alm: bool = False) -> Union[
-            np.ndarray, Tuple[np.ndarray, np.ndarray]]:
+            np.ndarray, None]:
         """Process the intensity map for saving with the Stokes Q/U
         maps and optionally calculate alms for the convolution.
 
         Parameters:
             return_alm (bool): whether to calculate and return alms
 
         Returns:
-            intensity_out (np.ndarray((Npix,))): intensity map to
-                save
             (optional) intensity_alm (np.ndarray((1, Nalms))):
                 processed alms used for convolution
         """
         intensity_nside = hp.get_nside(self.in_map)
 
-        if self.nside == intensity_nside:
-            intensity_out = self.in_map
-        else:
-            intensity_out = hp.ud_grade(self.in_map, self.nside)
+        if self.nside != intensity_nside:
+            self.in_map = hp.ud_grade(self.in_map, self.nside)
 
         if return_alm:
-            if self.ker_nside == intensity_nside:
+            if self.ker_nside == self.nside:
                 intensity_in = self.in_map
-            elif self.ker_nside == self.nside:
-                intensity_in = intensity_out
             else:
                 intensity_in = hp.ud_grade(self.in_map, self.ker_nside)
+                self.mask = hp.ud_grade(self.mask, self.ker_nside)
 
             intensity_in = self.unsharp_mask(intensity_in)
             intensity_alm = hp.map2alm(
                 intensity_in, self.lmax).reshape((1, -1))
-            return intensity_out, intensity_alm
+            return intensity_alm
 
-        return intensity_out
+        return None
 
     def make_ker(self):
         """Select line of pixels defining the kernel at the North Pole.
 
         Returns:
             line (collections.deque): double-ended queue of pixel
                 indices defining the kernel
@@ -378,20 +394,19 @@
         psis = np.repeat(orients, phis.shape[0])
         phis = np.tile(phis, orients.shape[0])
         thetas = np.tile(thetas, orients.shape[0])
 
         return np.vstack((thetas, phis, psis)).T
 
     def save_cube_and_stokes(
-            self, intensity: np.ndarray,
+            self, 
             interpolator: ducc0.totalconvolve.Interpolator) -> None:
         """Run the convolution and save the resulting cube and maps.
 
         Parameters:
-            intensity (np.ndarray((Npix,)): intensity map to save
             interpolator (ducc0.totalconvolve.Interpolator): object
                 encapsulating the convolution functionality
         """
         npix = 12 * self.nside**2
         stokes = StokesQU(npix)
         norm = np.zeros((npix))
 
@@ -432,18 +447,22 @@
             norm += spherical_rht_temp.sum(axis=0)
             process = psutil.Process(os.getpid())
             logging.info(f"* Using {process.memory_info().rss / 1e9}GB of"
                          " memory to make spherical RHT cube.")
 
         f.close()
 
-        stokes.normalize_and_weight(norm, self.weighting)
+        if self.weighting is not None:
+            stokes.normalize_and_weight(norm, self.weighting)
+        else:
+            stokes.normalize_and_weight(norm, self.in_map)
 
         hp.write_map(os.path.join(self.out_dir, "IQU_" + self.out_name
-                     + ".fits"), (intensity, stokes.stokes_q, stokes.stokes_u),
+                     + ".fits"), (self.in_map, stokes.stokes_q,
+                     stokes.stokes_u), dtype=["float32", "float32", "float32"],
                      coord="G", column_names=["I", "Q", "U"], overwrite=True)
 
         return None
 
     def build_and_save(self) -> None:
         """Run the algorithm and save the resulting orientation cube and
         Stokes maps.
@@ -462,17 +481,17 @@
 
         intensity_alm_file = os.path.join(
             self.out_dir, self.name
             + f"_alms_nside{self.ker_nside}_fwhm{self.fwhm}.npy")
         if os.path.exists(intensity_alm_file) and not self.overwrite:
             logging.info("* Input map alms exist.")
             intensity_alm = np.load(intensity_alm_file)
-            intensity = self.prep_intensity()
+            self.prep_intensity()
         else:
-            intensity, intensity_alm = self.prep_intensity(return_alm=True)
+            intensity_alm = self.prep_intensity(return_alm=True)
             np.save(intensity_alm_file, intensity_alm)
             logging.info("* Created input map alms.")
 
         ker_alm_file = os.path.join(
             self.kernel_alms_dir, f"alms_nside{self.ker_nside}_"
             f"wlen{self.wlen}.npy")
         if os.path.exists(ker_alm_file):
@@ -491,15 +510,15 @@
                                                         epsilon=1e-4,
                                                         ofactor=1.5,
                                                         nthreads=0)
 
         logging.info("* Interpolator configured.")
         del intensity_alm, ker_alm
 
-        self.save_cube_and_stokes(intensity, interpolator)
+        self.save_cube_and_stokes(interpolator)
 
         logging.info("* Saved cube and maps in output directory.")
         logging.info(
             f"* Total run time = {(time.perf_counter()-start_time) / 60.}"
             " mins.")
 
         return None
```

### Comparing `sphericalrht-1.2.2/src/sphericalrht.egg-info/PKG-INFO` & `sphericalrht-2.0.0/src/sphericalrht.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphericalrht
-Version: 1.2.2
+Version: 2.0.0
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
-Metadata-Version: 2.1 Name: sphericalrht Version: 1.2.2 Summary: Spherical
+Metadata-Version: 2.1 Name: sphericalrht Version: 2.0.0 Summary: Spherical
 implementation of the Rolling Hough Transform Home-page: https://github.com/
 georgehalal/sphericalrht Author: George Halal Author-email:
 halalgeorge@gmail.com Project-URL: Bug Tracker, https://github.com/georgehalal/
 sphericalrht/issues Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `sphericalrht-1.2.2/src/sphericalrht.egg-info/SOURCES.txt` & `sphericalrht-2.0.0/src/sphericalrht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/tests/data/test_map.fits` & `sphericalrht-2.0.0/tests/data/test_map.fits`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/tests/data/test_map2.fits` & `sphericalrht-2.0.0/tests/data/test_map2.fits`

 * *Files identical despite different names*

### Comparing `sphericalrht-1.2.2/tests/test_spherical_rht.py` & `sphericalrht-2.0.0/tests/test_spherical_rht.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Quantitative tests of the classes and functions in the sphericalrht
 package.
 
 Qualitative tests have been performed separately on toy models.
 
 Author: George Halal
 Email: halalgeorge@gmail.com
-Date: 11/11/2021
+Date: 04/27/2023
 """
 
 
 import os
 import shutil
 
 import ducc0
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
@@ -59,30 +59,32 @@
     """Test of the CubeAndStokes class.
     """
 
     def test_unsharp_mask(self):
         """Test of the CubeAndStokes.unsharp_mask method.
         """
         c_a_s = CubeAndStokes(
-            TEST_MAP_PATH, NSIDE, OUT_DIR, weighting=TEST_MAP2_PATH)
+            TEST_MAP_PATH, NSIDE, OUT_DIR, weighting=TEST_MAP_PATH,
+            mask=TEST_MAP_PATH)
         test_map = np.ones((NPIX))
         umask_map = c_a_s.unsharp_mask(test_map)
 
+        # we expect the ones to become halves
         self.assertEqual(np.sum(umask_map), NPIX/2)
 
     def test_prep_intensity(self):
         """Test of the CubeAndStokes.prep_intensity method.
         """
         c_a_s = CubeAndStokes(TEST_MAP_PATH, 4, OUT_DIR)
-        out_map = c_a_s.prep_intensity()
-        self.assertEqual(out_map.shape[0], 12 * 4**2)
+        c_a_s.prep_intensity()
+        self.assertEqual(c_a_s.in_map.shape[0], 12 * 4**2)
 
         c_a_s = CubeAndStokes(TEST_MAP_PATH, 1024, OUT_DIR)
-        out_map = c_a_s.prep_intensity()
-        self.assertEqual(out_map.shape[0], 12 * 1024**2)
+        c_a_s.prep_intensity()
+        self.assertEqual(c_a_s.in_map.shape[0], 12 * 1024**2)
 
     def test_make_ker(self):
         """Test of the CubeAndStokes.make_ker method.
         """
         c_a_s = CubeAndStokes(TEST_MAP_PATH, NSIDE, OUT_DIR)
         ker = c_a_s.make_ker()
 
@@ -111,15 +113,15 @@
         self.assertEqual(ptg[0, 2], 0)
 
     def test_save_cube_and_stokes(self):
         """Test of the CubeAndStokes.save_cube_and_stokes method.
         """
         c_a_s = CubeAndStokes(
             TEST_MAP_PATH, NSIDE, OUT_DIR, norients=NORIENTS,
-            weighting=TEST_MAP_PATH)
+            weighting=TEST_MAP2_PATH, mask=np.ones((NPIX)))
         lmax = c_a_s.lmax
         mmax = min(c_a_s.mmax, lmax)
 
         nalm_ker = (((mmax+1)*(mmax+2))//2 + (mmax+1)*(lmax-mmax))
         nalm_map = ((lmax+1)*(lmax+2)) // 2
 
         alm_ker = (np.random.uniform(-1., 1., (1, nalm_ker))
@@ -134,27 +136,27 @@
         interpolator = ducc0.totalconvolve.Interpolator(alm_map, alm_ker,
                                                         separate=True,
                                                         lmax=lmax,
                                                         kmax=mmax,
                                                         epsilon=1e-4,
                                                         ofactor=1.5,
                                                         nthreads=0)
-        intensity = np.ones((NPIX))
-        c_a_s.save_cube_and_stokes(intensity, interpolator)
+
+        c_a_s.save_cube_and_stokes(interpolator)
 
         cube_name = os.path.join(OUT_DIR, c_a_s.out_name + ".h5")
         map_name = os.path.join(OUT_DIR, "IQU_" + c_a_s.out_name + ".fits")
         self.assertTrue(os.path.exists(cube_name))
         self.assertTrue(os.path.exists(map_name))
 
     def test_build_and_save(self):
         """Test of the CubeAndStokes.build_and_save method.
         """
-        c_a_s = CubeAndStokes(
-            TEST_MAP_PATH, NSIDE, OUT_DIR, norients=NORIENTS, split_factor=1)
+        c_a_s = CubeAndStokes(TEST_MAP_PATH, NSIDE, OUT_DIR, norients=NORIENTS,
+                              weighting=np.ones((12 * 4**2)), split_factor=1)
         c_a_s.build_and_save()
 
         cube_name = os.path.join(OUT_DIR, c_a_s.out_name + ".h5")
         map_name = os.path.join(
             OUT_DIR, "IQU_" + c_a_s.out_name + ".fits")
         self.assertTrue(os.path.exists(cube_name))
         self.assertTrue(os.path.exists(map_name))
```

### Comparing `sphericalrht-1.2.2/tests/test_utils.py` & `sphericalrht-2.0.0/tests/test_utils.py`

 * *Files identical despite different names*

