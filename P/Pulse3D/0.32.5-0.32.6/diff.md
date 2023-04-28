# Comparing `tmp/Pulse3D-0.32.5.tar.gz` & `tmp/Pulse3D-0.32.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.32.5.tar", last modified: Thu Apr 27 01:50:44 2023, max compression
+gzip compressed data, was "Pulse3D-0.32.6.tar", last modified: Fri Apr 28 20:20:34 2023, max compression
```

## Comparing `Pulse3D-0.32.5.tar` & `Pulse3D-0.32.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.598796 Pulse3D-0.32.5/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-27 01:50:44.606796 Pulse3D-0.32.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-27 01:50:44.000000 Pulse3D-0.32.5/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-27 01:50:44.000000 Pulse3D-0.32.5/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:50:29.000000 Pulse3D-0.32.5/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 01:50:08.000000 Pulse3D-0.32.5/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 01:50:08.000000 Pulse3D-0.32.5/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-27 01:50:08.000000 Pulse3D-0.32.5/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-27 01:50:08.000000 Pulse3D-0.32.5/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    45167 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.292044 Pulse3D-0.32.6/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 20:20:34.300044 Pulse3D-0.32.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 20:20:34.000000 Pulse3D-0.32.6/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-28 20:20:34.000000 Pulse3D-0.32.6/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:20:17.000000 Pulse3D-0.32.6/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 20:19:57.000000 Pulse3D-0.32.6/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 20:19:57.000000 Pulse3D-0.32.6/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-28 20:19:57.000000 Pulse3D-0.32.6/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-28 20:19:57.000000 Pulse3D-0.32.6/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45310 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.32.5/LICENSE` & `Pulse3D-0.32.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/PKG-INFO` & `Pulse3D-0.32.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.32.5
+Version: 0.32.6
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.32.5/mantarray-magnet-finding/setup.py` & `Pulse3D-0.32.6/mantarray-magnet-finding/setup.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/setup.py` & `Pulse3D-0.32.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.32.5",
+    version="0.32.6",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.32.5/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.32.6/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.32.5
+Version: 0.32.6
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.32.5/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.32.6/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.32.6/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.32.6/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.32.6/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/constants.py` & `Pulse3D-0.32.6/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/excel_writer.py` & `Pulse3D-0.32.6/src/pulse3D/excel_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,26 +617,26 @@
         if stim_plotting_info:
             _write_stim_waveforms(writer, stim_plotting_info["stim_waveform_df"])
 
         # waveform snapshot/full
         wb = writer.book
         snapshot_sheet = wb.add_worksheet("continuous-waveform-snapshot")
         full_sheet = wb.add_worksheet("full-continuous-waveform-plots")
-
-        for well_info in recording_plotting_info:
+        for rec_info_idx, well_info in enumerate(recording_plotting_info):
             log.info(f'Creating waveform charts for well {well_info["well_name"]}')
             create_waveform_charts(
                 y_axis_bounds,
                 well_info,
                 continuous_waveforms_df,
                 wb,
                 continuous_waveforms_sheet,
                 snapshot_sheet,
                 full_sheet,
                 stim_plotting_info,
+                rec_info_idx,  # used to remove whitespace in full-continuous-waveform-plots
             )
 
         _write_aggregate_metrics(
             writer, recording_plotting_info, twitch_widths, baseline_widths_to_use, group_metrics_list
         )
 
         num_metrics = _write_per_twitch_metrics(
@@ -750,14 +750,15 @@
     well_info,
     continuous_waveforms_df,
     wb,
     continuous_waveforms_sheet,
     snapshot_sheet,
     full_sheet,
     stim_plotting_info,
+    rec_info_idx,
 ):
     well_idx = well_info["well_index"]
     well_name = well_info["well_name"]
 
     # maximum snapshot size is 10 seconds
     snapshot_lower_x_bound = well_info["tissue_data"][0, 0]
     snapshot_upper_x_bound = min(
@@ -897,17 +898,17 @@
         well_row * (CHART_HEIGHT_CELLS + 1), well_col * (CHART_FIXED_WIDTH_CELLS + 1), snapshot_chart
     )
 
     cells_per_well = CHART_HEIGHT_CELLS + 1
     if stim_chart_format == "stacked":
         cells_per_well += STIM_CHART_HEIGHT_CELLS
         if stim_chart.series:
-            full_sheet.insert_chart(1 + CHART_HEIGHT_CELLS + well_idx * cells_per_well, 1, stim_chart)
+            full_sheet.insert_chart(1 + CHART_HEIGHT_CELLS + rec_info_idx * cells_per_well, 1, stim_chart)
 
-    full_sheet.insert_chart(1 + well_idx * cells_per_well, 1, full_chart)
+    full_sheet.insert_chart(1 + rec_info_idx * cells_per_well, 1, full_chart)
 
 
 def aggregate_metrics_df(
     recording_plotting_info: List[Dict[Any, Any]],
     widths: Tuple[int, ...] = DEFAULT_TWITCH_WIDTHS,
     baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS,
     group_metrics_list: List[Dict[str, Any]] = [],
```

### Comparing `Pulse3D-0.32.5/src/pulse3D/magnet_finding.py` & `Pulse3D-0.32.6/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/metrics.py` & `Pulse3D-0.32.6/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/peak_detection.py` & `Pulse3D-0.32.6/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/plate_recording.py` & `Pulse3D-0.32.6/src/pulse3D/plate_recording.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import pandas as pd
 from scipy import interpolate
 from semver import VersionInfo
 from xlsxwriter.utility import xl_cell_to_rowcol
 
 from .compression_cy import compress_filtered_magnetic_data
 from .constants import *
+from .exceptions import DuplicateWellsFoundError
+from .exceptions import IncorrectOpticalFileFormatError
 from .exceptions import NoRecordingFilesLoadedError
 from .exceptions import SubprotocolFormatIncompatibleWithInterpolationError
 from .magnet_finding import find_magnet_positions
 from .magnet_finding import fix_dropped_samples
 from .magnet_finding import format_well_file_data
 from .stimulation import aggregate_timepoints
 from .stimulation import create_stim_session_waveforms
@@ -51,17 +53,15 @@
 log = logging.getLogger(__name__)
 
 
 class MantarrayH5FileCreator(h5py.File):
     """Creates an H5 file with the basic format/layout."""
 
     def __init__(
-        self,
-        file_name: str,
-        file_format_version: str = CURRENT_BETA2_HDF5_FILE_FORMAT_VERSION,
+        self, file_name: str, file_format_version: str = CURRENT_BETA2_HDF5_FILE_FORMAT_VERSION
     ) -> None:
         super().__init__(
             file_name,
             "w",
             # tried to specify this ('earliest', 'v110') to be more backward compatible
             # but it didn't work for unknown reasons (gave error when trying to set swmr_mode=True)
             libver="latest",
@@ -335,15 +335,14 @@
         stiffness_factor: Optional[int] = None,
         inverted_post_magnet_wells: Optional[List[str]] = None,
         well_groups: Optional[Dict[str, List[str]]] = None,
     ):
         self.path = path
         self.wells = []
         self._iter = 0
-
         # this may get overwritten later
         self.is_optical_recording = False
 
         # Tanner (11/16/22): due to the needs of the scientists for the full analysis,
         # these params should only be used in the recording snapshot.
         # These params also have no effect on Beta 1 data.
         if start_time < 0:
@@ -355,22 +354,23 @@
 
         self._created_from_dataframe = recording_df is not None
 
         if self.path.endswith(".zip"):
             with tempfile.TemporaryDirectory() as tmpdir:
                 zf = zipfile.ZipFile(path)
                 zf.extractall(path=tmpdir)
-                self.wells, calibration_recordings = load_files(
-                    tmpdir, stiffness_factor, inverted_post_magnet_wells
-                )
+
+                if glob.glob(os.path.join(tmpdir, "**", "*.h5"), recursive=True):
+                    self.wells, calibration_recordings = load_files(
+                        tmpdir, stiffness_factor, inverted_post_magnet_wells
+                    )
+                elif xlsx_files := glob.glob(os.path.join(tmpdir, "*.xlsx"), recursive=True):
+                    self._load_optical_well_files(xlsx_files, stiffness_factor)
         elif self.path.endswith(".xlsx"):  # optical file
-            self.is_optical_recording = True
-            well_file = WellFile(self.path, stiffness_factor=stiffness_factor)
-            self.wells = [None] * (well_file[WELL_INDEX_UUID] + 1)
-            self.wells[well_file[WELL_INDEX_UUID]] = well_file
+            self._load_optical_well_files([self.path], stiffness_factor)
         else:  # .h5 files
             self.wells, calibration_recordings = load_files(
                 self.path, stiffness_factor, inverted_post_magnet_wells
             )
 
         # make sure at least one WellFile was loaded
         if not any(self.wells):
@@ -522,14 +522,34 @@
             stim_col_titles = sorted([col for col in df if f"{well_name}__stim" in col])
 
             for col_title in stim_col_titles:
                 stim_session_raw = np.array([stim_timepoints, df[col_title]])
                 stim_session = stim_session_raw[:, ~np.isnan(stim_session_raw[1])].astype(int)
                 wf.stim_sessions.append(stim_session)
 
+    def _load_optical_well_files(self, file_paths: List[str], stiffness_factor: Union[int, None]):
+        self.is_optical_recording = True
+        if not self.wells:
+            # TODO parameterize number of wells here, set to 24 max for now
+            self.wells = [None] * 24
+
+        for xlsx_path in file_paths:
+            # check if xlsx is correct format and not pulse3d output file
+            if _get_num_of_sheets(xlsx_path) > 1:
+                raise IncorrectOpticalFileFormatError(
+                    f"Incorrect number of sheets found for file {os.path.basename(xlsx_path)}"
+                )
+
+            well_file = WellFile(xlsx_path, stiffness_factor=stiffness_factor)
+            # check if user attempts to upload multiple files for the same well
+            if self.wells[well_file[WELL_INDEX_UUID]] is not None:
+                raise DuplicateWellsFoundError(f"Duplicate well found for {well_file[WELL_NAME_UUID]}")
+
+            self.wells[well_file[WELL_INDEX_UUID]] = well_file
+
     def to_dataframe(self, include_stim_data=True) -> pd.DataFrame:
         """Creates DataFrame from PlateRecording with all the data
         interpolated, normalized, and scaled. The returned dataframe contains
         one column for time in ms and one column for each well.
 
         The dataframe returned by this method can be used in calls to peak_detector by selecting the
         'time' column and the well column that peak detection should be run on after transposing the
@@ -622,22 +642,14 @@
         log.info(f"Loading recording from file {os.path.basename(path)}")
         yield PlateRecording(path, **kwargs)
 
     @staticmethod
     def from_directory(path, **kwargs):
         # multi zip files
         for zf in glob.glob(os.path.join(path, "*.zip"), recursive=True):
-            zip_file = zipfile.ZipFile(zf)
-            # check if this is a zip of optical files
-            if ".xlsx" in zip_file.namelist()[0]:
-                with tempfile.TemporaryDirectory() as tmpdir:
-                    zip_file.extractall(path=tmpdir)
-                    for optical_file in os.scandir(tmpdir):
-                        yield PlateRecording(optical_file.path, **kwargs)
-                return
             log.info(f"Loading recording from file {zf}")
             yield PlateRecording(zf, **kwargs)
 
         # multi optical files
         for of in glob.glob(os.path.join(path, "*.xlsx"), recursive=True):
             log.info(f"Loading optical data from file {of}")
             yield PlateRecording(of, **kwargs)
@@ -707,14 +719,19 @@
 
 
 def _get_single_sheet(file_name: str) -> Any:
     work_book = load_workbook(file_name)
     return work_book[work_book.sheetnames[0]]
 
 
+def _get_num_of_sheets(file_path: str) -> Any:
+    work_book = load_workbook(file_path)
+    return len(work_book.sheetnames)
+
+
 def _get_cell_value(sheet: Worksheet, zero_based_row: int, zero_based_col: int) -> Optional[str]:
     result = sheet.cell(row=zero_based_row + 1, column=zero_based_col + 1).value
     if result is None:
         return result
     return str(result)
 
 
@@ -748,14 +765,18 @@
 
     begin_recording = _get_excel_metadata_value(sheet, UTC_BEGINNING_RECORDING_UUID)
     begin_recording = datetime.datetime.strptime(begin_recording, "%Y-%m-%d %H:%M:%S")  # type: ignore
 
     twenty_four_well = LabwareDefinition(row_count=4, column_count=6)
     well_name = _get_excel_metadata_value(sheet, WELL_NAME_UUID)
 
+    # some provided sample xlsx files contained well names like A001 and B001
+    if well_name is not None:
+        well_name = well_name.replace("0", "")
+
     attrs = {
         FILE_FORMAT_VERSION_METADATA_KEY: NOT_APPLICABLE_LABEL,
         TISSUE_SENSOR_READINGS: raw_tissue_reading,
         REFERENCE_SENSOR_READINGS: np.zeros(raw_tissue_reading.shape),
         str(INTERPOLATION_VALUE_UUID): interpolation_value,
         str(TISSUE_SAMPLING_PERIOD_UUID): sampling_period,
         str(UTC_BEGINNING_RECORDING_UUID): begin_recording,
```

### Comparing `Pulse3D-0.32.5/src/pulse3D/plotting.py` & `Pulse3D-0.32.6/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/stimulation.py` & `Pulse3D-0.32.6/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/transforms.py` & `Pulse3D-0.32.6/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.5/src/pulse3D/utils.py` & `Pulse3D-0.32.6/src/pulse3D/utils.py`

 * *Files identical despite different names*

