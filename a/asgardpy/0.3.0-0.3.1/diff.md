# Comparing `tmp/asgardpy-0.3.0.tar.gz` & `tmp/asgardpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgardpy-0.3.0.tar", last modified: Fri Apr 28 13:42:17 2023, max compression
+gzip compressed data, was "asgardpy-0.3.1.tar", last modified: Fri Apr 28 15:07:30 2023, max compression
```

## Comparing `asgardpy-0.3.0.tar` & `asgardpy-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-28 13:41:56.000000 asgardpy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-28 13:42:17.950912 asgardpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-28 13:41:56.000000 asgardpy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.946911 asgardpy-0.3.0/asgardpy/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/analysis/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/base/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/base/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/config/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/dataset_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/dl4.py
--rw-r--r--   0 runner    (1001) docker     (123)    32909 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/data/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-28 13:41:56.000000 asgardpy-0.3.0/asgardpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:42:17.950912 asgardpy-0.3.0/asgardpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 13:42:17.000000 asgardpy-0.3.0/asgardpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 13:41:56.000000 asgardpy-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 13:42:17.950912 asgardpy-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-28 13:41:56.000000 asgardpy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:30.441226 asgardpy-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-28 15:07:09.000000 asgardpy-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-28 15:07:30.441226 asgardpy-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-28 15:07:09.000000 asgardpy-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:30.437226 asgardpy-0.3.1/asgardpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:30.437226 asgardpy-0.3.1/asgardpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/analysis/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:30.437226 asgardpy-0.3.1/asgardpy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/base/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/base/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:30.437226 asgardpy-0.3.1/asgardpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/config/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:30.441226 asgardpy-0.3.1/asgardpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/data/dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/data/dataset_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/data/dl4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32909 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/data/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:30.441226 asgardpy-0.3.1/asgardpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-28 15:07:09.000000 asgardpy-0.3.1/asgardpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:07:30.437226 asgardpy-0.3.1/asgardpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-28 15:07:30.000000 asgardpy-0.3.1/asgardpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 15:07:30.000000 asgardpy-0.3.1/asgardpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:07:30.000000 asgardpy-0.3.1/asgardpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 15:07:30.000000 asgardpy-0.3.1/asgardpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 15:07:30.000000 asgardpy-0.3.1/asgardpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 15:07:09.000000 asgardpy-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-28 15:07:30.441226 asgardpy-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-28 15:07:09.000000 asgardpy-0.3.1/setup.py
```

### Comparing `asgardpy-0.3.0/LICENSE` & `asgardpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/PKG-INFO` & `asgardpy-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
-Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.2.0.tar.gz
+Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
```

### Comparing `asgardpy-0.3.0/README.md` & `asgardpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/analysis/analysis.py` & `asgardpy-0.3.1/asgardpy/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/base/__init__.py` & `asgardpy-0.3.1/asgardpy/base/__init__.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/base/base.py` & `asgardpy-0.3.1/asgardpy/base/base.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/base/geom.py` & `asgardpy-0.3.1/asgardpy/base/geom.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/base/reduction.py` & `asgardpy-0.3.1/asgardpy/base/reduction.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/config/generator.py` & `asgardpy-0.3.1/asgardpy/config/generator.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/data/__init__.py` & `asgardpy-0.3.1/asgardpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/data/dataset_1d.py` & `asgardpy-0.3.1/asgardpy/data/dataset_1d.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/data/dataset_3d.py` & `asgardpy-0.3.1/asgardpy/data/dataset_3d.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/data/dl4.py` & `asgardpy-0.3.1/asgardpy/data/dl4.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/data/target.py` & `asgardpy-0.3.1/asgardpy/data/target.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy/io/io.py` & `asgardpy-0.3.1/asgardpy/io/io.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/asgardpy.egg-info/PKG-INFO` & `asgardpy-0.3.1/asgardpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
-Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.2.0.tar.gz
+Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
```

### Comparing `asgardpy-0.3.0/asgardpy.egg-info/SOURCES.txt` & `asgardpy-0.3.1/asgardpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.0/setup.py` & `asgardpy-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,19 +41,19 @@
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords="",
     url="https://github.com/chaimain/asgardpy",
-    download_url="https://github.com/chaimain/asgardpy/archive/refs/tags/v0.2.0.tar.gz",
+    download_url="https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz",
     author="Chaitanya Priyadarshi",
     author_email="chaitanya.p.astrphys@gmail.com",
     license="Apache",
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"],
     ),
     package_data={"asgardpy": ["py.typed"]},
     install_requires=read_requirements("requirements.txt"),
     extras_require={"dev": read_requirements("dev-requirements.txt")},
-    python_requires=">=3.8",
+    python_requires=">=3.10",
 )
```

