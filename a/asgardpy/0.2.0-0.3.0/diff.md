# Comparing `tmp/asgardpy-0.2.0.tar.gz` & `tmp/asgardpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgardpy-0.2.0.tar", last modified: Mon Apr 24 11:30:37 2023, max compression
+gzip compressed data, was "asgardpy-0.3.0.tar", last modified: Fri Apr 28 13:42:17 2023, max compression
```

## Comparing `asgardpy-0.2.0.tar` & `asgardpy-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        0 2023-04-24 11:30:37.000000 asgardpy-0.2.0/
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)    11353 2023-02-18 06:29:57.000000 asgardpy-0.2.0/LICENSE
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     2852 2023-04-24 11:30:37.000000 asgardpy-0.2.0/PKG-INFO
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     2108 2023-04-24 11:15:26.000000 asgardpy-0.2.0/README.md
-drwxr-xr-x   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        0 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy/
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)      161 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/__init__.py
-drwxr-xr-x   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        0 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy/analysis/
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)       88 2023-02-18 06:29:57.000000 asgardpy-0.2.0/asgardpy/analysis/__init__.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     7864 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/analysis/analysis.py
-drwxr-xr-x   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        0 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy/config/
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)       83 2023-02-18 06:29:57.000000 asgardpy-0.2.0/asgardpy/config/__init__.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     3834 2023-04-10 22:23:12.000000 asgardpy-0.2.0/asgardpy/config/generator.py
-drwxr-xr-x   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        0 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy/data/
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     2874 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/data/__init__.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     4105 2023-03-06 21:07:33.000000 asgardpy-0.2.0/asgardpy/data/base.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)    15071 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/data/dataset_1d.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)    24864 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/data/dataset_3d.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     4751 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/data/dl4.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     2964 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/data/geom.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     2903 2023-02-18 06:29:57.000000 asgardpy-0.2.0/asgardpy/data/reduction.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)    30793 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/data/target.py
-drwxr-xr-x   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        0 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy/io/
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)      128 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/io/__init__.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     6512 2023-04-10 21:51:58.000000 asgardpy-0.2.0/asgardpy/io/io.py
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        0 2023-02-18 06:29:57.000000 asgardpy-0.2.0/asgardpy/py.typed
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)      407 2023-04-19 00:57:32.000000 asgardpy-0.2.0/asgardpy/version.py
-drwxr-xr-x   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        0 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy.egg-info/
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     2852 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy.egg-info/PKG-INFO
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)      626 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy.egg-info/SOURCES.txt
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        1 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy.egg-info/dependency_links.txt
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)      402 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy.egg-info/requires.txt
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)        9 2023-04-24 11:30:37.000000 asgardpy-0.2.0/asgardpy.egg-info/top_level.txt
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)      347 2023-02-18 06:29:57.000000 asgardpy-0.2.0/pyproject.toml
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)      447 2023-04-24 11:30:37.000000 asgardpy-0.2.0/setup.cfg
--rw-r--r--   0 chaitanya.priyadarshi  (2679) ctan-onsite-it  (1772)     2190 2023-04-24 11:29:39.000000 asgardpy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-28 13:41:56.000000 asgardpy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-28 13:42:17.950912 asgardpy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-28 13:41:56.000000 asgardpy-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.946911 asgardpy-0.3.0/asgardpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/analysis/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/base/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/base/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/config/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/dataset_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/dl4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32909 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 13:41:56.000000 asgardpy-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 13:42:17.950912 asgardpy-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-28 13:41:56.000000 asgardpy-0.3.0/setup.py
```

### Comparing `asgardpy-0.2.0/LICENSE` & `asgardpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgardpy-0.2.0/PKG-INFO` & `asgardpy-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.2.0
+Version: 0.3.0
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
 Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.2.0.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)] [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
-Follow the `Gammapy v1.0 <https://docs.gammapy.org/1.0/>`_ documentation for understanding the core Gammapy objects.
+Follow the [Gammapy v1.0](https://docs.gammapy.org/1.0/) documentation for understanding the core Gammapy objects.
 
-The various Data Levels	used here follow the descriptions suggested by `GADF v0.3 <https://gamma-astro-data-formats.readthedocs.io/en/latest/>`_ and CTAO Data Model
+The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT (`enrico <https://enrico.readthedocs.io/en/latest/>`_ and `fermipy <https://fermipy.readthedocs.io/en/latest/>`_) files and LST-1 (`cta-lstchain <https://cta-observatory.github.io/cta-lstchain/>`_) DL3 files (with energy-dependent selection cuts) for point-like sources. 
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources. 
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.2.0/README.md` & `asgardpy-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)] [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
-Follow the `Gammapy v1.0 <https://docs.gammapy.org/1.0/>`_ documentation for understanding the core Gammapy objects.
+Follow the [Gammapy v1.0](https://docs.gammapy.org/1.0/) documentation for understanding the core Gammapy objects.
 
-The various Data Levels	used here follow the descriptions suggested by `GADF v0.3 <https://gamma-astro-data-formats.readthedocs.io/en/latest/>`_ and CTAO Data Model
+The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT (`enrico <https://enrico.readthedocs.io/en/latest/>`_ and `fermipy <https://fermipy.readthedocs.io/en/latest/>`_) files and LST-1 (`cta-lstchain <https://cta-observatory.github.io/cta-lstchain/>`_) DL3 files (with energy-dependent selection cuts) for point-like sources. 
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources. 
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.2.0/asgardpy/analysis/analysis.py` & `asgardpy-0.3.0/asgardpy/analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Config-driven high level analysis interface.
 """
 import logging
 
 from gammapy.datasets import Datasets
 from gammapy.modeling.models import Models
 
-from asgardpy.config.generator import AsgardpyConfig
-from asgardpy.data.base import AnalysisStep
-from asgardpy.data.target import apply_selection_mask_to_models, set_models
+from asgardpy.base import AnalysisStep
+from asgardpy.config import AsgardpyConfig
+from asgardpy.data import apply_selection_mask_to_models, set_models
 
 log = logging.getLogger(__name__)
 
 __all__ = ["AsgardpyAnalysis"]
 
 
 class AsgardpyAnalysis:
```

### Comparing `asgardpy-0.2.0/asgardpy/data/base.py` & `asgardpy-0.3.0/asgardpy/base/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 
 from astropy import units as u
 from astropy.coordinates import Angle
 from astropy.time import Time
 from pydantic import BaseModel
 
 __all__ = [
+    "AnalysisStep",
+    "AnalysisStepBase",
+    "AnalysisStepEnum",
     "AngleType",
+    "BaseConfig",
+    "EnergyRangeConfig",
     "EnergyType",
-    "TimeType",
     "FrameEnum",
+    "PathType",
     "TimeFormatEnum",
-    "AnalysisStepBase",
-    "AnalysisStep",
-    "BaseConfig",
-    "TimeRangeConfig",
     "TimeIntervalsConfig",
-    "EnergyRangeConfig",
+    "TimeRangeConfig",
+    "TimeType",
 ]
 
 
 # Basic Quantities Type for building the Config
 class AngleType(Angle):
     @classmethod
     def __get_validators__(cls):
@@ -143,15 +145,15 @@
 class AnalysisStep:
     """
     Create one of the Analysis Step class listed in the Registry.
     """
 
     @staticmethod
     def create(tag, config, **kwargs):
-        from . import ANALYSIS_STEP_REGISTRY
+        from asgardpy.data import ANALYSIS_STEP_REGISTRY
 
         cls = ANALYSIS_STEP_REGISTRY.get_cls(tag)
         return cls(config, **kwargs)
 
 
 class AnalysisStepEnum(str, Enum):
     datasets_1d = "datasets-1d"
```

### Comparing `asgardpy-0.2.0/asgardpy/data/dataset_1d.py` & `asgardpy-0.3.0/asgardpy/data/dataset_1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,36 +20,34 @@
     SafeMaskMaker,
     SpectrumDatasetMaker,
     WobbleRegionsFinder,
 )
 from gammapy.maps import RegionGeom, WcsGeom
 from regions import CircleAnnulusSkyRegion, CircleSkyRegion, PointSkyRegion
 
-from asgardpy.data.base import AnalysisStepBase, BaseConfig
-from asgardpy.data.geom import (
+from asgardpy.base import (
+    AnalysisStepBase,
+    BackgroundConfig,
+    BaseConfig,
     GeomConfig,
     MapAxesConfig,
-    SpatialPointConfig,
-    get_energy_axis,
-)
-from asgardpy.data.reduction import (
-    BackgroundConfig,
     MapSelectionEnum,
     ObservationsConfig,
     ReductionTypeEnum,
     SafeMaskConfig,
+    SpatialPointConfig,
+    get_energy_axis,
 )
-from asgardpy.io.io import DL3Files, InputConfig
+from asgardpy.io import DL3Files, InputConfig
 
 __all__ = [
-    "Dataset1DConfig",
+    "Datasets1DAnalysisStep",
     "Dataset1DBaseConfig",
     "Dataset1DConfig",
     "Dataset1DGeneration",
-    "Datasets1DAnalysisStep",
 ]
 
 log = logging.getLogger(__name__)
 
 
 # Defining various components of 1D Dataset Config section
 class Dataset1DInfoConfig(BaseConfig):
@@ -353,27 +351,15 @@
         the config.
         """
         safe_config = self.config_1d_dataset_info.safe_mask
         pars = safe_config.parameters
 
         if len(safe_config.methods) != 0:
             if "custom-mask" not in safe_config.methods:
-                pos = SkyCoord(
-                    u.Quantity(pars.position["lon"]),
-                    u.Quantity(pars.position["lat"]),
-                    frame=pars.position["frame"],
-                )
-                safe_maker = SafeMaskMaker(
-                    methods=safe_config.methods,
-                    aeff_percent=pars.aeff_percent,
-                    bias_percent=pars.bias_percent,
-                    position=pos,
-                    fixed_offset=pars.fixed_offset,
-                    offset_max=pars.offset_max,
-                )
+                safe_maker = SafeMaskMaker(methods=safe_config.methods, **pars)
             else:
                 safe_maker = None
         else:
             safe_maker = None
 
         return safe_maker
```

### Comparing `asgardpy-0.2.0/asgardpy/data/dataset_3d.py` & `asgardpy-0.3.0/asgardpy/data/dataset_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,41 +23,40 @@
     Models,
     PowerLawNormSpectralModel,
     SkyModel,
     TemplateSpatialModel,
 )
 from regions import CircleAnnulusSkyRegion, CircleSkyRegion
 
-from asgardpy.data.base import AnalysisStepBase, BaseConfig
-from asgardpy.data.geom import (
+from asgardpy.base import (
+    AnalysisStepBase,
+    BackgroundConfig,
+    BaseConfig,
     GeomConfig,
     MapAxesConfig,
-    SpatialCircleConfig,
-    get_energy_axis,
-)
-from asgardpy.data.reduction import (
-    BackgroundConfig,
     MapSelectionEnum,
     ReductionTypeEnum,
     SafeMaskConfig,
+    SpatialCircleConfig,
+    get_energy_axis,
 )
 from asgardpy.data.target import (
     apply_selection_mask_to_models,
     create_gal_diffuse_skymodel,
     create_iso_diffuse_skymodel,
     create_source_skymodel,
 )
 from asgardpy.io import DL3Files, InputConfig
 
 __all__ = [
-    "Dataset3DInfoConfig",
+    "Datasets3DAnalysisStep",
     "Dataset3DBaseConfig",
     "Dataset3DConfig",
     "Dataset3DGeneration",
-    "Datasets3DAnalysisStep",
+    "Dataset3DInfoConfig",
 ]
 
 log = logging.getLogger(__name__)
 
 
 # Defining various components of 3D Dataset Config section
 class Dataset3DInfoConfig(BaseConfig):
```

### Comparing `asgardpy-0.2.0/asgardpy/data/dl4.py` & `asgardpy-0.3.0/asgardpy/data/dl4.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from enum import Enum
 
 from astropy import units as u
 from gammapy.datasets import Datasets
 from gammapy.estimators import FluxPointsEstimator
 from gammapy.modeling import Fit
 
-from asgardpy.data.base import AnalysisStepBase, BaseConfig, EnergyRangeConfig
+from asgardpy.base import AnalysisStepBase, BaseConfig, EnergyRangeConfig
 
 __all__ = [
-    "FluxPointsConfig",
-    "FitConfig",
     "FitAnalysisStep",
+    "FitConfig",
     "FluxPointsAnalysisStep",
+    "FluxPointsConfig",
 ]
 
 
 # Defining various components of High-level Analysis Config
 class BackendEnum(str, Enum):
     minuit = "minuit"
     scipy = "scipy"
```

### Comparing `asgardpy-0.2.0/asgardpy/data/geom.py` & `asgardpy-0.3.0/asgardpy/base/geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 from enum import Enum
 from typing import List
 
 from astropy import units as u
 from gammapy.maps import MapAxis
 
-from asgardpy.data.base import AngleType, BaseConfig, EnergyType, FrameEnum
+from asgardpy.base import AngleType, BaseConfig, EnergyType, FrameEnum
 
 __all__ = [
-    "SpatialCircleConfig",
-    "SpatialPointConfig",
     "EnergyAxisConfig",
-    "MapAxesConfig",
     "EnergyEdgesCustomConfig",
-    "SelectionConfig",
+    "GeomConfig",
+    "MapAxesConfig",
     "MapFrameShapeConfig",
-    "SkyCoordConfig",
     "ProjectionEnum",
+    "SelectionConfig",
+    "SkyCoordConfig",
+    "SpatialCircleConfig",
+    "SpatialPointConfig",
     "WcsConfig",
-    "GeomConfig",
     "get_energy_axis",
 ]
 
 
 # Basic Components to define the main GeomConfig
 class SpatialCircleConfig(BaseConfig):
     frame: FrameEnum = FrameEnum.icrs
```

### Comparing `asgardpy-0.2.0/asgardpy/data/reduction.py` & `asgardpy-0.3.0/asgardpy/base/reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 """
 
 from enum import Enum
 from typing import List
 
 from astropy import units as u
 
-from asgardpy.data.base import AngleType, BaseConfig, PathType, TimeIntervalsConfig
-from asgardpy.data.geom import SkyCoordConfig
+from asgardpy.base import (
+    AngleType,
+    BaseConfig,
+    PathType,
+    SkyCoordConfig,
+    TimeIntervalsConfig,
+)
 
 __all__ = [
-    "ReductionTypeEnum",
-    "RequiredHDUEnum",
-    "ObservationsConfig",
-    "BackgroundRegionFinderMethodEnum",
-    "ReflectedRegionFinderConfig",
-    "WobbleRegionsFinderConfig",
+    "BackgroundConfig",
     "BackgroundMethodEnum",
+    "BackgroundRegionFinderMethodEnum",
     "ExclusionRegionsConfig",
-    "RegionsConfig",
-    "SafeMaskMethodsEnum",
     "MapSelectionEnum",
-    "BackgroundConfig",
+    "ObservationsConfig",
+    "ReductionTypeEnum",
+    "ReflectedRegionFinderConfig",
+    "RegionsConfig",
+    "RequiredHDUEnum",
     "SafeMaskConfig",
+    "SafeMaskMethodsEnum",
+    "WobbleRegionsFinderConfig",
 ]
 
 
 # Basic Components to define the various Dataset Reduction Maker Config
 class ReductionTypeEnum(str, Enum):
     spectrum = "1d"
     cube = "3d"
```

### Comparing `asgardpy-0.2.0/asgardpy/data/target.py` & `asgardpy-0.3.0/asgardpy/data/target.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,35 +17,35 @@
     EBLAbsorptionNormSpectralModel,
     Models,
     SkyModel,
     SpectralModel,
     create_fermi_isotropic_diffuse_model,
 )
 
-from asgardpy.data.base import AngleType, BaseConfig, PathType
-from asgardpy.data.geom import SkyCoordConfig
+from asgardpy.base import AngleType, BaseConfig, PathType, SkyCoordConfig
 
 __all__ = [
+    "BrokenPowerLaw2SpectralModel",
     "EBLAbsorptionModel",
-    "SpectralModelConfig",
-    "SpatialModelConfig",
+    "ExpCutoffLogParabolaSpectralModel",
     "RoISelectionConfig",
+    "SpatialModelConfig",
+    "SpectralModelConfig",
     "Target",
-    "ExpCutoffLogParabolaSpectralModel",
-    "set_models",
     "apply_selection_mask_to_models",
     "config_to_dict",
+    "create_gal_diffuse_skymodel",
+    "create_iso_diffuse_skymodel",
+    "create_source_skymodel",
     "params_renaming_to_gammapy",
     "params_rescale_to_gammapy",
     "read_models_from_asgardpy_config",
-    "xml_spectral_model_to_gammapy_params",
+    "set_models",
     "xml_spatial_model_to_gammapy",
-    "create_source_skymodel",
-    "create_iso_diffuse_skymodel",
-    "create_gal_diffuse_skymodel",
+    "xml_spectral_model_to_gammapy_params",
 ]
 
 
 # Basic components to define the Target Config and any Models Config
 class EBLAbsorptionModel(BaseConfig):
     filename: PathType = PathType(".")
     reference: str = "dominguez"
@@ -140,14 +140,67 @@
         xx = energy / reference
         exponent = -alpha_1 - beta * np.log(xx)
         cutoff = np.exp(-np.power(energy * lambda_, alpha_2))
 
         return amplitude * np.power(xx, exponent) * cutoff
 
 
+class BrokenPowerLaw2SpectralModel(SpectralModel):
+    r"""Spectral broken power-law 2 model.
+
+    In this slightly modified Broken Power Law, instead of having the second index
+    as a distinct parameter, the difference in the spectral indices around the
+    Break Energy is used, to try for some assumptions on the different physical
+    processes that define the full spectrum, where the second process is dependent
+    on the first process.
+
+    For more information see :ref:`broken-powerlaw-spectral-model`.
+
+    Parameters
+    ----------
+    index1 : `~astropy.units.Quantity`
+        :math:`\Gamma1`
+    index_diff : `~astropy.units.Quantity`
+        :math:`\Delta\Gamma`
+    amplitude : `~astropy.units.Quantity`
+        :math:`\phi_0`
+    ebreak : `~astropy.units.Quantity`
+        :math:`E_{break}`
+
+    See Also
+    --------
+    SmoothBrokenPowerLawSpectralModel
+    """
+
+    tag = ["BrokenPowerLaw2SpectralModel", "bpl2"]
+    index1 = Parameter("index1", 2.0)
+    index_diff = Parameter("index_diff", 1.0)
+    amplitude = Parameter(
+        name="amplitude",
+        value="1e-12 cm-2 s-1 TeV-1",
+        scale_method="scale10",
+        interp="log",
+        is_norm=True,
+    )
+    ebreak = Parameter("ebreak", "1 TeV")
+
+    @staticmethod
+    def evaluate(energy, index1, index_diff, amplitude, ebreak):
+        """Evaluate the model (static function)."""
+        energy = np.atleast_1d(energy)
+        cond = energy < ebreak
+        bpwl2 = amplitude * np.ones(energy.shape)
+
+        index2 = index1 + index_diff
+        bpwl2[cond] *= (energy[cond] / ebreak) ** (-index1)
+        bpwl2[~cond] *= (energy[~cond] / ebreak) ** (-index2)
+
+        return bpwl2
+
+
 # Function for Models assignment
 def set_models(
     config, datasets, datasets_name_list=None, models=None, target_source_name=None, extend=False
 ):
     """
     Set models on given Datasets.
 
@@ -322,14 +375,18 @@
 
     # Spectral Model
     if model_config.spectral.ebl_abs.reference != "":
         if model_config.spectral.type == "ExpCutoffLogParabolaSpectralModel":
             model1 = ExpCutoffLogParabolaSpectralModel().from_dict(
                 {"spectral": config_to_dict(model_config.spectral)}
             )
+        elif model_config.spectral.type == "BrokenPowerLaw2SpectralModel":
+            model1 = BrokenPowerLaw2SpectralModel().from_dict(
+                {"spectral": config_to_dict(model_config.spectral)}
+            )
         else:
             model1 = SPECTRAL_MODEL_REGISTRY.get_cls(model_config.spectral.type)().from_dict(
                 {"spectral": config_to_dict(model_config.spectral)}
             )
 
         ebl_model = model_config.spectral.ebl_abs
 
@@ -348,14 +405,18 @@
             model2.alpha_norm.value = ebl_model.alpha_norm
         spectral_model = model1 * model2
     else:
         if model_config.spectral.type == "ExpCutoffLogParabolaSpectralModel":
             spectral_model = ExpCutoffLogParabolaSpectralModel().from_dict(
                 {"spectral": config_to_dict(model_config.spectral)}
             )
+        elif model_config.spectral.type == "BrokenPowerLaw2SpectralModel":
+            model1 = BrokenPowerLaw2SpectralModel().from_dict(
+                {"spectral": config_to_dict(model_config.spectral)}
+            )
         else:
             spectral_model = SPECTRAL_MODEL_REGISTRY.get_cls(
                 model_config.spectral.type
             )().from_dict({"spectral": config_to_dict(model_config.spectral)})
     spectral_model.name = config.source_name
 
     # Spatial model if provided
```

### Comparing `asgardpy-0.2.0/asgardpy/io/io.py` & `asgardpy-0.3.0/asgardpy/io/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,20 @@
 Dataset and DL3 files that follow GADF v0.3 and can be directly read by Gammapy,
 for 1D Dataset.
 """
 
 import logging
 from pathlib import Path
 
-from asgardpy.data.base import BaseConfig, PathType
+from asgardpy.base import BaseConfig, PathType
 
 __all__ = ["InputFilePatterns", "InputConfig", "DL3Files"]
 
 EXPECTED_DL3_RANGE = ["gadf-dl3", "lat", "lat-aux"]
 
-glob_dict_std = {
-    "events": "*events.fits*",
-    "edisp": "*DRM.fits*",
-    "exposure": "*BinnedMap.fits*",
-    "xml_model": "*out.xml",
-    "psf": "*psf.fits*",
-    "diffuse": "gll_iem_v*.fits*",
-    "iso": "iso_P8R3_SOURCE_V*_*.txt",
-    "dl3": "dl3*fits",
-}
-
 
 # Basic Components for the Input Config
 class InputFilePatterns(BaseConfig):
     events: str = "*events.fits*"
     edisp: str = "*DRM.fits*"
     exposure: str = "*BinnedMap.fits*"
     xml_model: str = "*out.xml"
@@ -65,19 +54,15 @@
             self.dl3_path = Path(dir_dict.input_dir)
         else:
             self.log.error(f"{dir_dict.input_dir} is not a valid file location")
 
         self.dl3_type = dir_dict.type
         self._check_dl3_type()
 
-        glob_dict = dir_dict.glob_pattern
-        if glob_dict is None:
-            self.glob_dict = glob_dict_std
-        else:
-            self.glob_dict = glob_dict
+        self.glob_dict = dir_dict.glob_pattern
 
         self.events_files = None
         self.edrm_files = None
         self.xml_files = None
         self.expmap_files = None
         self.psf_files = None
         self.gal_diff_files = None
```

### Comparing `asgardpy-0.2.0/asgardpy.egg-info/PKG-INFO` & `asgardpy-0.3.0/asgardpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.2.0
+Version: 0.3.0
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
 Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.2.0.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)] [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
-Follow the `Gammapy v1.0 <https://docs.gammapy.org/1.0/>`_ documentation for understanding the core Gammapy objects.
+Follow the [Gammapy v1.0](https://docs.gammapy.org/1.0/) documentation for understanding the core Gammapy objects.
 
-The various Data Levels	used here follow the descriptions suggested by `GADF v0.3 <https://gamma-astro-data-formats.readthedocs.io/en/latest/>`_ and CTAO Data Model
+The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT (`enrico <https://enrico.readthedocs.io/en/latest/>`_ and `fermipy <https://fermipy.readthedocs.io/en/latest/>`_) files and LST-1 (`cta-lstchain <https://cta-observatory.github.io/cta-lstchain/>`_) DL3 files (with energy-dependent selection cuts) for point-like sources. 
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources. 
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.2.0/asgardpy.egg-info/SOURCES.txt` & `asgardpy-0.3.0/asgardpy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 asgardpy.egg-info/PKG-INFO
 asgardpy.egg-info/SOURCES.txt
 asgardpy.egg-info/dependency_links.txt
 asgardpy.egg-info/requires.txt
 asgardpy.egg-info/top_level.txt
 asgardpy/analysis/__init__.py
 asgardpy/analysis/analysis.py
+asgardpy/base/__init__.py
+asgardpy/base/base.py
+asgardpy/base/geom.py
+asgardpy/base/reduction.py
 asgardpy/config/__init__.py
 asgardpy/config/generator.py
 asgardpy/data/__init__.py
-asgardpy/data/base.py
 asgardpy/data/dataset_1d.py
 asgardpy/data/dataset_3d.py
 asgardpy/data/dl4.py
-asgardpy/data/geom.py
-asgardpy/data/reduction.py
 asgardpy/data/target.py
 asgardpy/io/__init__.py
 asgardpy/io/io.py
```

### Comparing `asgardpy-0.2.0/setup.py` & `asgardpy-0.3.0/setup.py`

 * *Files identical despite different names*

