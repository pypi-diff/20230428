# Comparing `tmp/pyp_beagle-0.9.8.tar.gz` & `tmp/pyp_beagle-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyp_beagle-0.9.8.tar", last modified: Fri Nov 11 13:19:57 2022, max compression
+gzip compressed data, was "dist/pyp_beagle-0.9.9.tar", last modified: Fri Nov 11 14:41:19 2022, max compression
```

## Comparing `pyp_beagle-0.9.8.tar` & `pyp_beagle-0.9.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10140 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/PyP-BEAGLE/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_calibration_correction.py
--rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    31186 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_mock_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)     6954 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_multinest_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_observed_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)     9675 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11764 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    35681 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_photometry.py
--rw-r--r--   0 runner    (1001) docker     (121)    19430 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_posterior_predictive_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     7004 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_residual_photometry.py
--rw-r--r--   0 runner    (1001) docker     (121)    39552 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_spectra.py
--rw-r--r--   0 runner    (1001) docker     (121)    12195 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_spectral_indices.py
--rw-r--r--   0 runner    (1001) docker     (121)    17870 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_summary_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)    19156 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/beagle_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10664 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/command_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/FillBetweenStep.py
--rw-r--r--   0 runner    (1001) docker     (121)    11445 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/WeightedKDE.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/autoscale.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/set_shared_labels.py
--rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/walker_random_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/PyP-BEAGLE/files/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/files/calibration_correction.json
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/files/emission_lines.json
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/files/params_names.json
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/files/params_names_latex_table.json
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/files/params_names_mock.json
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/files/summary_config.json
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/PyP-BEAGLE/significant_digits.py
--rw-r--r--   0 runner    (1001) docker     (121)     8410 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/pyp_beagle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10140 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/pyp_beagle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/pyp_beagle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/pyp_beagle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/pyp_beagle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/pyp_beagle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/pyp_beagle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 13:19:57.000000 pyp_beagle-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3901 2022-11-11 13:19:49.000000 pyp_beagle-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10140 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/PyP-BEAGLE/
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_calibration_correction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31186 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_mock_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6954 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_multinest_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_observed_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9675 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11764 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35681 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19430 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_posterior_predictive_checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7004 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_residual_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39929 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12195 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_spectral_indices.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17870 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_summary_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19156 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/beagle_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10664 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/FillBetweenStep.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11445 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/WeightedKDE.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/autoscale.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/set_shared_labels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/walker_random_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/PyP-BEAGLE/files/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/files/calibration_correction.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/files/emission_lines.json
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/files/params_names.json
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/files/params_names_latex_table.json
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/files/params_names_mock.json
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/files/summary_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/PyP-BEAGLE/significant_digits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8410 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/pyp_beagle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10140 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/pyp_beagle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/pyp_beagle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/pyp_beagle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/pyp_beagle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/pyp_beagle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/pyp_beagle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 14:41:19.000000 pyp_beagle-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3901 2022-11-11 14:41:07.000000 pyp_beagle-0.9.9/setup.py
```

### Comparing `pyp_beagle-0.9.8/PKG-INFO` & `pyp_beagle-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp_beagle
-Version: 0.9.8
+Version: 0.9.9
 Summary: Package for post-processing of results obtained with the Beagle SED fitting tool
 Home-page: https://github.com/jacopo-chevallard/PyP-BEAGLE
 Author: Jacopo Chevallard
 Author-email: jacopo.chevallard@mailfence.com
 License: MIT
 Description: [![Upload Python Package](https://github.com/jacopo-chevallard/PyP-BEAGLE/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jacopo-chevallard/PyP-BEAGLE/actions/workflows/python-publish.yml)
```

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/__init__.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/__init__.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_calibration_correction.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_calibration_correction.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_filters.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_filters.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_mock_catalogue.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_mock_catalogue.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_multinest_catalogue.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_multinest_catalogue.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_multiprocess.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_multiprocess.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_observed_catalogue.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_observed_catalogue.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_parsers.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_parsers.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_pdf.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_pdf.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_photometry.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_photometry.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_posterior_predictive_checks.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_posterior_predictive_checks.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_residual_photometry.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_residual_photometry.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_spectra.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,31 +313,27 @@
 
         hdulist = fits.open(fits_file)
 
         # Read the template wl array, and the 2D flux array
         model_wl = hdulist['marginal sed wl'].data['wl'][0,:]
         model_fluxes = hdulist['marginal sed'].data
         
-
-            
-
         # Read the posterior probability
         # to use random.choice you need the probabilities to very high precision and to
         # sum to 1
         probability = np.array(hdulist['posterior pdf'].data['probability'], np.float64)
         probability = probability/probability.sum().astype(np.float64)
 
         # Now compute for each wl bin the sorted fluxes, you will need this to
         # calculate the median and percentiles for each wl bin
         sort_indices = np.argsort(model_fluxes, axis=0)
 
         # Now it's time to compute the median (observed-frame) SED and its percentiles
         n_wl = model_fluxes.shape[1]
         
-
         # If plotting the calibration correction, create calibration_correction fluxes
         if self.show_calibration_correction:
             #Sample 100 from the output
 #            nSamp = 100
 #            idx = np.random.choice(np.fromiter((x for x in range(model_fluxes.shape[0])),np.int),\
 #                                               size=nSamp,p=probability)
             calibration_correction_arr = np.zeros([model_fluxes.shape[0],n_wl])
@@ -402,28 +398,31 @@
 #        pylab.plot(model_wl, upper_calibration)
 #        pylab.show()
                 
     
         # Set the plot limits from the minimum and maximum wl_eff
         axs = list()
         residual_axs = list()
+        multiple_redshifts = False
         if observation.data['redshift'] is not None:
             redshift = observation.data['redshift']
         else:
             _redshifts =  hdulist['galaxy properties'].data['redshift']
             _, _counts = np.unique(_redshifts, return_counts=True)
             if len(_counts) > 1:
                 logging.warning("The `redshift` of the object is not unique!")
+                multiple_redshifts = True
 
             # Take the MAP redshift
             redshift = hdulist['galaxy properties'].data['redshift'][np.argmax(probability)]
 
-        z1 = 1. + redshift
-
         if self.wl_rest:
+            if multiple_redshifts:
+                raise ValueError('Cannot plot in the rest-frame since redshift is an adjustable parameter of the model!')
+            z1 = 1. + redshift
             data_wl = observation.data['wl'] / z1
             data_flux = observation.data['flux'] * z1
             data_flux_err = observation.data['fluxerr'] * z1
 
             model_wl /= z1
             median_flux *= z1
             lower_flux *= z1
@@ -433,18 +432,14 @@
             data_flux = observation.data['flux']
             data_flux_err = observation.data['fluxerr']
 
         # Convert to correct wl units
         model_wl /= wl_factor
         data_wl /= wl_factor
         
-
-                
-
-
         # Load the mask spectrum if exists
         mask_color = "grey"
         has_mask = False
         data_mask = np.ones(len(data_wl), dtype=bool)
         if "mask" in observation.data:
             data_mask = observation.data['mask']
             has_mask = True
@@ -782,24 +777,23 @@
 
             # Extract and plot full SED
             if 'full sed wl' in hdulist and self.plot_full_SED:
                 indices = np.arange(len(probability))
                 wrand = WalkerRandomSampling(probability, keys=indices)
                 rand_indices = wrand.random(self.n_SED_to_plot)
 
-                if self.wl_rest:
-                    wl_obs = hdulist['full sed wl'].data['wl'][0,:]
-
-                    for i in rand_indices:
-                        SED = hdulist['full sed'].data[i,:]
-                else:
-                    wl_obs = hdulist['full sed wl'].data['wl'][0,:] * z1
+                for i in rand_indices:
 
-                    for i in rand_indices:
-                        SED = hdulist['full sed'].data[i,:] / z1
+                    if self.wl_rest:
+                        wl_obs = hdulist['full sed wl'].data['wl'][0,:]
+                        flux_obs = hdulist['full sed'].data[i,:]
+                    else:
+                        _z1 = 1. + hdulist['galaxy properties'].data['redshift'][i]
+                        wl_obs = hdulist['full sed wl'].data['wl'][0,:] * _z1
+                        flux_obs = hdulist['full sed'].data[i,:] / _z1
 
                     ax.plot(wl_obs, 
                             flux_obs,
                             color="black",
                             ls="-",
                             lw=0.5,
                             alpha=0.5)
@@ -811,26 +805,30 @@
             yl = autoscale.get_autoscale_y(ax, ylog=self.log_flux, top_margin=0.2, bottom_margin=0.1)
             ylim = [min(ylim[0], yl[0]), max(ylim[1], yl[1])]
 
         for ax in axs:
             ax.set_ylim(ylim)
 
         if self.show_residual:
-            data_flux_ = data_flux[np.isclose(data_wl, model_wl, rtol=1e-6, atol=0.0, equal_nan=False)]
-            data_mask_ = data_mask[np.isclose(data_wl, model_wl, rtol=1e-6, atol=0.0, equal_nan=False)]
-            data_flux_err_ = data_flux_err[np.isclose(data_wl, model_wl, rtol=1e-6, atol=0.0, equal_nan=False)]
+            arr1 = np.pad(model_wl, (3, 2), 'constant', constant_values=(8,0))                 
+            len_diff = len(data_wl)-len(model_wl)
+            is_close = np.isclose(data_wl, np.pad(model_wl, (0, len_diff), constant_values=(0.,0.)), rtol=1e-6, atol=0.0, equal_nan=False)
+            data_flux_ = data_flux[is_close]
+            data_mask_ = data_mask[is_close]
+            data_flux_err_ = data_flux_err[is_close]
+
             residual = (data_flux_-median_flux)/data_flux_
             residual_err = (1./data_flux_ - (data_flux_-median_flux)/data_flux_**2) * data_flux_err_
 
             ymax = np.amax(abs(residual))
             ymax += 0.2*ymax
             ymax = 1.1
 
             colors = ["darkgreen"]
-            indices = np.arange(len(data_wl))
+            indices = np.arange(len(data_flux_))
             if has_mask:
                 colors = ["darkgreen", mask_color]
 
             for ax in residual_axs:
                 ax.set_ylim([-ymax, ymax])
                 kwargs = {'alpha':0.7}
```

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_spectral_indices.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_spectral_indices.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_summary_catalogue.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_summary_catalogue.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/beagle_utils.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/beagle_utils.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/command_line.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/command_line.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/conftest.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/conftest.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/FillBetweenStep.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/FillBetweenStep.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/WeightedKDE.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/WeightedKDE.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/autoscale.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/autoscale.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/set_shared_labels.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/set_shared_labels.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/dependencies/walker_random_sampling.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/dependencies/walker_random_sampling.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/files/emission_lines.json` & `pyp_beagle-0.9.9/PyP-BEAGLE/files/emission_lines.json`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/files/params_names.json` & `pyp_beagle-0.9.9/PyP-BEAGLE/files/params_names.json`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/files/params_names_mock.json` & `pyp_beagle-0.9.9/PyP-BEAGLE/files/params_names_mock.json`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/files/summary_config.json` & `pyp_beagle-0.9.9/PyP-BEAGLE/files/summary_config.json`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/PyP-BEAGLE/significant_digits.py` & `pyp_beagle-0.9.9/PyP-BEAGLE/significant_digits.py`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/README.md` & `pyp_beagle-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/pyp_beagle.egg-info/PKG-INFO` & `pyp_beagle-0.9.9/pyp_beagle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp-beagle
-Version: 0.9.8
+Version: 0.9.9
 Summary: Package for post-processing of results obtained with the Beagle SED fitting tool
 Home-page: https://github.com/jacopo-chevallard/PyP-BEAGLE
 Author: Jacopo Chevallard
 Author-email: jacopo.chevallard@mailfence.com
 License: MIT
 Description: [![Upload Python Package](https://github.com/jacopo-chevallard/PyP-BEAGLE/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jacopo-chevallard/PyP-BEAGLE/actions/workflows/python-publish.yml)
```

### Comparing `pyp_beagle-0.9.8/pyp_beagle.egg-info/SOURCES.txt` & `pyp_beagle-0.9.9/pyp_beagle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyp_beagle-0.9.8/setup.py` & `pyp_beagle-0.9.9/setup.py`

 * *Files identical despite different names*

