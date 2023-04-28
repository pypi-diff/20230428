# Comparing `tmp/multidimio-0.2.8.tar.gz` & `tmp/multidimio-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidimio-0.2.8.tar", max compression
+gzip compressed data, was "multidimio-0.2.9.tar", max compression
```

## Comparing `multidimio-0.2.8.tar` & `multidimio-0.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    10203 2023-03-04 14:30:10.755033 multidimio-0.2.8/LICENSE
--rw-r--r--   0        0        0     6043 2023-03-04 14:30:10.755033 multidimio-0.2.8/README.md
--rw-r--r--   0        0        0     2855 2023-03-04 14:30:26.131072 multidimio-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      474 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/__init__.py
--rw-r--r--   0        0        0     2697 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/__main__.py
--rw-r--r--   0        0        0      127 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/api/__init__.py
--rw-r--r--   0        0        0    24779 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/api/accessor.py
--rw-r--r--   0        0        0     2322 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/api/convenience.py
--rw-r--r--   0        0        0     4451 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/api/io_utils.py
--rw-r--r--   0        0        0      105 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/commands/__init__.py
--rw-r--r--   0        0        0    10623 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/commands/segy.py
--rw-r--r--   0        0        0      529 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/constants.py
--rw-r--r--   0        0        0      141 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/converters/__init__.py
--rw-r--r--   0        0        0      597 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/converters/exceptions.py
--rw-r--r--   0        0        0     6349 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/converters/mdio.py
--rw-r--r--   0        0        0    12386 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/converters/segy.py
--rw-r--r--   0        0        0      143 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/core/__init__.py
--rw-r--r--   0        0        0     3811 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/core/dimension.py
--rw-r--r--   0        0        0      268 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/core/exceptions.py
--rw-r--r--   0        0        0     3765 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/core/grid.py
--rw-r--r--   0        0        0     2917 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/core/indexing.py
--rw-r--r--   0        0        0     2727 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/core/serialization.py
--rw-r--r--   0        0        0      429 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/core/utils_write.py
--rw-r--r--   0        0        0     1646 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/py.typed
--rw-r--r--   0        0        0       44 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/__init__.py
--rw-r--r--   0        0        0      636 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/_standards_common.py
--rw-r--r--   0        0        0     9384 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/_standards_rev0.py
--rw-r--r--   0        0        0     8023 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/_workers.py
--rw-r--r--   0        0        0    11362 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/blocked_io.py
--rw-r--r--   0        0        0     1760 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/byte_utils.py
--rw-r--r--   0        0        0     9396 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/creation.py
--rw-r--r--   0        0        0     4856 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/ebcdic.py
--rw-r--r--   0        0        0      181 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/exceptions.py
--rw-r--r--   0        0        0     2748 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/headers.py
--rw-r--r--   0        0        0     3561 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/headers_text.py
--rw-r--r--   0        0        0     3232 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/helpers_segy.py
--rw-r--r--   0        0        0     5785 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/ibm_float.py
--rw-r--r--   0        0        0     4540 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/parsers.py
--rw-r--r--   0        0        0     6160 2023-03-04 14:30:10.771033 multidimio-0.2.8/src/mdio/segy/utilities.py
--rw-r--r--   0        0        0     7710 1970-01-01 00:00:00.000000 multidimio-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    10203 2023-03-10 15:18:05.939740 multidimio-0.2.9/LICENSE
+-rw-r--r--   0        0        0     6043 2023-03-10 15:18:05.939740 multidimio-0.2.9/README.md
+-rw-r--r--   0        0        0     2860 2023-03-10 15:18:19.051646 multidimio-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/__init__.py
+-rw-r--r--   0        0        0     2697 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/__main__.py
+-rw-r--r--   0        0        0      127 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/api/__init__.py
+-rw-r--r--   0        0        0    24779 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/api/accessor.py
+-rw-r--r--   0        0        0     2322 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/api/convenience.py
+-rw-r--r--   0        0        0     4451 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/api/io_utils.py
+-rw-r--r--   0        0        0      105 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/commands/__init__.py
+-rw-r--r--   0        0        0    10623 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/commands/segy.py
+-rw-r--r--   0        0        0      529 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/constants.py
+-rw-r--r--   0        0        0      141 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/converters/__init__.py
+-rw-r--r--   0        0        0      597 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/converters/exceptions.py
+-rw-r--r--   0        0        0     6349 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/converters/mdio.py
+-rw-r--r--   0        0        0    12386 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/converters/segy.py
+-rw-r--r--   0        0        0      143 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/__init__.py
+-rw-r--r--   0        0        0     3811 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/dimension.py
+-rw-r--r--   0        0        0      268 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/exceptions.py
+-rw-r--r--   0        0        0     3765 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/grid.py
+-rw-r--r--   0        0        0     2917 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/indexing.py
+-rw-r--r--   0        0        0     2727 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/serialization.py
+-rw-r--r--   0        0        0      429 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/utils_write.py
+-rw-r--r--   0        0        0     1646 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/py.typed
+-rw-r--r--   0        0        0       44 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/__init__.py
+-rw-r--r--   0        0        0      636 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/_standards_common.py
+-rw-r--r--   0        0        0     9384 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/_standards_rev0.py
+-rw-r--r--   0        0        0     8023 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/_workers.py
+-rw-r--r--   0        0        0    11362 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/blocked_io.py
+-rw-r--r--   0        0        0     1760 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/byte_utils.py
+-rw-r--r--   0        0        0     9396 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/creation.py
+-rw-r--r--   0        0        0     4856 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/ebcdic.py
+-rw-r--r--   0        0        0      181 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/exceptions.py
+-rw-r--r--   0        0        0     2748 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/headers.py
+-rw-r--r--   0        0        0     3561 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/headers_text.py
+-rw-r--r--   0        0        0     3232 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/helpers_segy.py
+-rw-r--r--   0        0        0     5785 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/ibm_float.py
+-rw-r--r--   0        0        0     4540 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/parsers.py
+-rw-r--r--   0        0        0     6160 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/utilities.py
+-rw-r--r--   0        0        0     7680 1970-01-01 00:00:00.000000 multidimio-0.2.9/PKG-INFO
```

### Comparing `multidimio-0.2.8/LICENSE` & `multidimio-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/README.md` & `multidimio-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/pyproject.toml` & `multidimio-0.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidimio"
-version = "0.2.8"
+version = "0.2.9"
 description = "Cloud-native, scalable, and user-friendly multi dimensional energy data!"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
     "Sri Kainkaryam <sribharath.kainkaryam@tgs.com>",
 ]
 license = "Apache-2.0"
@@ -31,17 +31,17 @@
 dask = ">=2022.11.0"
 tqdm = "^4.64.0"
 segyio = "^1.9.3"
 numba = ">=0.55.2,<1.0.0"
 psutil = "^5.9.1"
 distributed = {version = ">=2022.11.0", optional = true}
 bokeh = {version = "^2.4.3", optional = true}
-s3fs = {version = "^2022.7.0", optional = true}
-gcsfs = {version = "^2022.7.0", optional = true}
-adlfs = {version = "^2022.7.0", optional = true}
+s3fs = {version = ">=2022.7.0", optional = true}
+gcsfs = {version = ">=2022.7.0", optional = true}
+adlfs = {version = ">=2022.7.0", optional = true}
 zfpy = {version = "^1.0.0", optional = true}
 
 [tool.poetry.extras]
 distributed = ["distributed", "bokeh"]
 cloud = ["s3fs", "gcsfs", "adlfs"]
 lossy = ["zfpy"]
 
@@ -50,24 +50,24 @@
 coverage = {version = "^6.4.4", extras = ["toml"]}
 darglint = "^1.8.1"
 flake8 = "^5.0.0"
 flake8-bandit = "^4.0.0"
 flake8-bugbear = "^22.8.22"
 flake8-docstrings = "^1.6.0"
 flake8-rst-docstrings = "^0.2.7"
-furo = "^2022.6.21"
+furo = ">=2022.6.21"
 isort = "^5.10.1"
 mypy = "^0.971"
 pep8-naming = "^0.13.2"
 pre-commit = "^2.20.0"
 pre-commit-hooks = "^4.3.0"
 pytest = "^7.1.2"
 pyupgrade = "^2.37.3"
 safety = "^2.1.1"
-sphinx-autobuild = "^2021.3.14"
+sphinx-autobuild = ">=2021.3.14"
 sphinx-click = "^4.3.0"
 sphinx-copybutton = "^0.5.0"
 typeguard = "^2.13.3"
 xdoctest = {version = "^1.0.2", extras = ["colors"]}
 myst-parser = "^0.18.0"
 Pygments = "^2.13.0"
 Sphinx = "^5.1.1"
```

### Comparing `multidimio-0.2.8/src/mdio/__main__.py` & `multidimio-0.2.9/src/mdio/__main__.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/api/accessor.py` & `multidimio-0.2.9/src/mdio/api/accessor.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/api/convenience.py` & `multidimio-0.2.9/src/mdio/api/convenience.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/api/io_utils.py` & `multidimio-0.2.9/src/mdio/api/io_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/commands/segy.py` & `multidimio-0.2.9/src/mdio/commands/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/constants.py` & `multidimio-0.2.9/src/mdio/constants.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/converters/exceptions.py` & `multidimio-0.2.9/src/mdio/converters/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/converters/mdio.py` & `multidimio-0.2.9/src/mdio/converters/mdio.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/converters/segy.py` & `multidimio-0.2.9/src/mdio/converters/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/core/dimension.py` & `multidimio-0.2.9/src/mdio/core/dimension.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/core/grid.py` & `multidimio-0.2.9/src/mdio/core/grid.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/core/indexing.py` & `multidimio-0.2.9/src/mdio/core/indexing.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/core/serialization.py` & `multidimio-0.2.9/src/mdio/core/serialization.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/exceptions.py` & `multidimio-0.2.9/src/mdio/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/_standards_common.py` & `multidimio-0.2.9/src/mdio/segy/_standards_common.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/_standards_rev0.py` & `multidimio-0.2.9/src/mdio/segy/_standards_rev0.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/_workers.py` & `multidimio-0.2.9/src/mdio/segy/_workers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/blocked_io.py` & `multidimio-0.2.9/src/mdio/segy/blocked_io.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/byte_utils.py` & `multidimio-0.2.9/src/mdio/segy/byte_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/creation.py` & `multidimio-0.2.9/src/mdio/segy/creation.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/ebcdic.py` & `multidimio-0.2.9/src/mdio/segy/ebcdic.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/headers.py` & `multidimio-0.2.9/src/mdio/segy/headers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/headers_text.py` & `multidimio-0.2.9/src/mdio/segy/headers_text.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/helpers_segy.py` & `multidimio-0.2.9/src/mdio/segy/helpers_segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/ibm_float.py` & `multidimio-0.2.9/src/mdio/segy/ibm_float.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/parsers.py` & `multidimio-0.2.9/src/mdio/segy/parsers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/src/mdio/segy/utilities.py` & `multidimio-0.2.9/src/mdio/segy/utilities.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.8/PKG-INFO` & `multidimio-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidimio
-Version: 0.2.8
+Version: 0.2.9
 Summary: Cloud-native, scalable, and user-friendly multi dimensional energy data!
 Home-page: https://mdio.dev
 License: Apache-2.0
 Keywords: mdio,multidimio,seismic,wind,data
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
@@ -15,24 +15,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cloud
 Provides-Extra: distributed
 Provides-Extra: lossy
-Requires-Dist: adlfs (>=2022.7.0,<2023.0.0) ; extra == "cloud"
+Requires-Dist: adlfs (>=2022.7.0) ; extra == "cloud"
 Requires-Dist: bokeh (>=2.4.3,<3.0.0) ; extra == "distributed"
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-params (>=0.3.0,<0.4.0)
 Requires-Dist: dask (>=2022.11.0)
 Requires-Dist: distributed (>=2022.11.0) ; extra == "distributed"
-Requires-Dist: gcsfs (>=2022.7.0,<2023.0.0) ; extra == "cloud"
+Requires-Dist: gcsfs (>=2022.7.0) ; extra == "cloud"
 Requires-Dist: numba (>=0.55.2,<1.0.0)
 Requires-Dist: psutil (>=5.9.1,<6.0.0)
-Requires-Dist: s3fs (>=2022.7.0,<2023.0.0) ; extra == "cloud"
+Requires-Dist: s3fs (>=2022.7.0) ; extra == "cloud"
 Requires-Dist: segyio (>=1.9.3,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: zarr (>=2.12.0,<3.0.0)
 Requires-Dist: zfpy (>=1.0.0,<2.0.0) ; extra == "lossy"
 Project-URL: Changelog, https://github.com/TGSAI/mdio-python/releases
 Project-URL: Documentation, https://mdio-python.readthedocs.io
 Project-URL: Repository, https://github.com/TGSAI/mdio-python
```

