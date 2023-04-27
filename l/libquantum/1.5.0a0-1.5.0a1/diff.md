# Comparing `tmp/libquantum-1.5.0a0.tar.gz` & `tmp/libquantum-1.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libquantum-1.5.0a0.tar", last modified: Thu Apr 27 23:23:45 2023, max compression
+gzip compressed data, was "libquantum-1.5.0a1.tar", last modified: Thu Apr 27 23:39:57 2023, max compression
```

## Comparing `libquantum-1.5.0a0.tar` & `libquantum-1.5.0a1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.519237 libquantum-1.5.0a0/
--rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.0a0/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    15457 2023-04-27 23:23:45.519237 libquantum-1.5.0a0/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     2070 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/README.md
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.517237 libquantum-1.5.0a0/libquantum/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.0a0/libquantum/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    20391 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/libquantum/atoms.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/atoms_inverse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/blast_pulse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/doppler.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/entropy.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/export.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.518237 libquantum-1.5.0a0/libquantum/plot_templates/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.0a0/libquantum/plot_templates/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/plot_templates/plot_time_frequency_picks.py
--rw-r--r--   0 opq       (1000) opq       (1000)    40958 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/libquantum/plot_templates/plot_time_frequency_reps.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/scales.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.0a0/libquantum/spectra.py
--rw-r--r--   0 opq       (1000) opq       (1000)    12802 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/libquantum/synthetics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/tfr_gate_pick.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14988 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/libquantum/utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.518237 libquantum-1.5.0a0/libquantum.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    15457 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)      722 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      104 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       11 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      866 2023-04-27 23:22:39.000000 libquantum-1.5.0a0/pyproject.toml
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:23:45.519237 libquantum-1.5.0a0/setup.cfg
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.518237 libquantum-1.5.0a0/tests/
--rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.0a0/tests/test_quantum.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/tests/test_spectra.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.584776 libquantum-1.5.0a1/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.0a1/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    15457 2023-04-27 23:39:57.584776 libquantum-1.5.0a1/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     2070 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/README.md
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.582776 libquantum-1.5.0a1/libquantum/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.0a1/libquantum/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    20391 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/libquantum/atoms.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/atoms_inverse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/blast_pulse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/doppler.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/entropy.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/export.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.583776 libquantum-1.5.0a1/libquantum/plot_templates/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.0a1/libquantum/plot_templates/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/plot_templates/plot_time_frequency_picks.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    40958 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/libquantum/plot_templates/plot_time_frequency_reps.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/scales.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.0a1/libquantum/spectra.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    12802 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/libquantum/synthetics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/tfr_gate_pick.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14988 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/libquantum/utils.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.583776 libquantum-1.5.0a1/libquantum.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    15457 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)      722 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      108 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       11 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      870 2023-04-27 23:39:41.000000 libquantum-1.5.0a1/pyproject.toml
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:39:57.584776 libquantum-1.5.0a1/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.584776 libquantum-1.5.0a1/tests/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.0a1/tests/test_quantum.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/tests/test_spectra.py
```

### Comparing `libquantum-1.5.0a0/LICENSE` & `libquantum-1.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/PKG-INFO` & `libquantum-1.5.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.0a0
+Version: 1.5.0a1
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libquantum-1.5.0a0/README.md` & `libquantum-1.5.0a1/README.md`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/atoms.py` & `libquantum-1.5.0a1/libquantum/atoms.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/atoms_inverse.py` & `libquantum-1.5.0a1/libquantum/atoms_inverse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/blast_pulse.py` & `libquantum-1.5.0a1/libquantum/blast_pulse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/doppler.py` & `libquantum-1.5.0a1/libquantum/doppler.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/entropy.py` & `libquantum-1.5.0a1/libquantum/entropy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/export.py` & `libquantum-1.5.0a1/libquantum/export.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/plot_templates/plot_geo_scatter_2d_3d.py` & `libquantum-1.5.0a1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/plot_templates/plot_time_frequency_picks.py` & `libquantum-1.5.0a1/libquantum/plot_templates/plot_time_frequency_picks.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/plot_templates/plot_time_frequency_reps.py` & `libquantum-1.5.0a1/libquantum/plot_templates/plot_time_frequency_reps.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/scales.py` & `libquantum-1.5.0a1/libquantum/scales.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/spectra.py` & `libquantum-1.5.0a1/libquantum/spectra.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/synthetics.py` & `libquantum-1.5.0a1/libquantum/synthetics.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/tfr_gate_pick.py` & `libquantum-1.5.0a1/libquantum/tfr_gate_pick.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum/utils.py` & `libquantum-1.5.0a1/libquantum/utils.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/libquantum.egg-info/PKG-INFO` & `libquantum-1.5.0a1/libquantum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.0a0
+Version: 1.5.0a1
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libquantum-1.5.0a0/libquantum.egg-info/SOURCES.txt` & `libquantum-1.5.0a1/libquantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a0/pyproject.toml` & `libquantum-1.5.0a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # See:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "libquantum"
-version = "1.5.0a0"
+version = "1.5.0a1"
 authors = [
     { name = "RedVox, Inc", email = "support@redvox.io" }
 ]
 description = "Library for implementing standardized time-frequency representations."
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file = "LICENSE" }
 
 dependencies = [
     "librosa==0.10.0.post2",
-    "redvox==3.4.0",
-    "libwwz==1.3.0",
-    "redvox-base[matplotlib,numpy,pandas,scipy]==2023.4.25"
+    "redvox==3.4.0a3",
+    "libwwz==1.3.0a1",
+    "redvox-base[matplotlib,numpy,pandas,scipy]==2023.4.27"
 ]
 
 [project.urls]
 homepage = "https://github.com/RedVoxInc/libquantum"
 PyPI = "https://pypi.org/project/libquantum/"
 
 [build-system]
```

### Comparing `libquantum-1.5.0a0/tests/test_spectra.py` & `libquantum-1.5.0a1/tests/test_spectra.py`

 * *Files identical despite different names*

