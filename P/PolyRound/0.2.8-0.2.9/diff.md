# Comparing `tmp/PolyRound-0.2.8.tar.gz` & `tmp/PolyRound-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PolyRound-0.2.8.tar", last modified: Thu Apr 13 08:52:16 2023, max compression
+gzip compressed data, was "PolyRound-0.2.9.tar", last modified: Fri Apr 28 13:56:27 2023, max compression
```

## Comparing `PolyRound-0.2.8.tar` & `PolyRound-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.964647 PolyRound-0.2.8/
--rw-rw-rw-   0 root         (0) root         (0)    34667 2023-04-13 08:52:08.000000 PolyRound-0.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5811 2023-04-13 08:52:16.961647 PolyRound-0.2.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.944646 PolyRound-0.2.8/PolyRound/
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-04-13 08:52:08.000000 PolyRound-0.2.8/PolyRound/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6769 2023-04-13 08:52:08.000000 PolyRound-0.2.8/PolyRound/api.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-04-13 08:52:08.000000 PolyRound-0.2.8/PolyRound/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-04-13 08:52:08.000000 PolyRound-0.2.8/PolyRound/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.951646 PolyRound-0.2.8/PolyRound/mutable_classes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/mutable_classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5190 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/mutable_classes/polytope.py
--rw-rw-rw-   0 root         (0) root         (0)     3916 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.956647 PolyRound-0.2.8/PolyRound/static_classes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7488 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/constraint_removal_reduction.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/csv_io.py
--rw-rw-rw-   0 root         (0) root         (0)    12846 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/lp_interfacing.py
--rw-rw-rw-   0 root         (0) root         (0)     2501 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/lp_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/parse_sbml_stoichiometry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.961647 PolyRound-0.2.8/PolyRound/static_classes/rounding/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/rounding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3138 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/rounding/geometric_mean_scaling.py
--rw-rw-rw-   0 root         (0) root         (0)    10569 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py
--rw-rw-rw-   0 root         (0) root         (0)    20225 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/unit_tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.949646 PolyRound-0.2.8/PolyRound.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5811 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5310 2023-04-13 08:52:09.000000 PolyRound-0.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 08:52:16.964647 PolyRound-0.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-04-13 08:52:09.000000 PolyRound-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.443999 PolyRound-0.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)    34667 2023-04-28 13:56:13.000000 PolyRound-0.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5054 2023-04-28 13:56:27.441999 PolyRound-0.2.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.423997 PolyRound-0.2.9/PolyRound/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6769 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.431998 PolyRound-0.2.9/PolyRound/mutable_classes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/mutable_classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5190 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/mutable_classes/polytope.py
+-rw-rw-rw-   0 root         (0) root         (0)     3916 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.436998 PolyRound-0.2.9/PolyRound/static_classes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7488 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/constraint_removal_reduction.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/csv_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    12846 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/lp_interfacing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2501 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/lp_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/parse_sbml_stoichiometry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.441999 PolyRound-0.2.9/PolyRound/static_classes/rounding/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/rounding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3138 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/rounding/geometric_mean_scaling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10569 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py
+-rw-rw-rw-   0 root         (0) root         (0)    20225 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/unit_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.429998 PolyRound-0.2.9/PolyRound.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5054 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4553 2023-04-28 13:56:13.000000 PolyRound-0.2.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 13:56:27.443999 PolyRound-0.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-04-28 13:56:13.000000 PolyRound-0.2.9/setup.py
```

### Comparing `PolyRound-0.2.8/LICENSE` & `PolyRound-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/__init__.py` & `PolyRound-0.2.9/PolyRound/__init__.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/api.py` & `PolyRound-0.2.9/PolyRound/api.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/main.py` & `PolyRound-0.2.9/PolyRound/main.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/mutable_classes/polytope.py` & `PolyRound-0.2.9/PolyRound/mutable_classes/polytope.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/settings.py` & `PolyRound-0.2.9/PolyRound/settings.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/static_classes/constraint_removal_reduction.py` & `PolyRound-0.2.9/PolyRound/static_classes/constraint_removal_reduction.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/static_classes/csv_io.py` & `PolyRound-0.2.9/PolyRound/static_classes/csv_io.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/static_classes/lp_interfacing.py` & `PolyRound-0.2.9/PolyRound/static_classes/lp_interfacing.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/static_classes/lp_utils.py` & `PolyRound-0.2.9/PolyRound/static_classes/lp_utils.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/static_classes/parse_sbml_stoichiometry.py` & `PolyRound-0.2.9/PolyRound/static_classes/parse_sbml_stoichiometry.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/static_classes/rounding/geometric_mean_scaling.py` & `PolyRound-0.2.9/PolyRound/static_classes/rounding/geometric_mean_scaling.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py` & `PolyRound-0.2.9/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py` & `PolyRound-0.2.9/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound/unit_tests.py` & `PolyRound-0.2.9/PolyRound/unit_tests.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.8/PolyRound.egg-info/SOURCES.txt` & `PolyRound-0.2.9/PolyRound.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 PolyRound/__init__.py
 PolyRound/api.py
 PolyRound/default_settings.py
 PolyRound/main.py
 PolyRound/settings.py
 PolyRound/unit_tests.py
+PolyRound/version.py
 PolyRound.egg-info/PKG-INFO
 PolyRound.egg-info/SOURCES.txt
 PolyRound.egg-info/dependency_links.txt
 PolyRound.egg-info/requires.txt
 PolyRound.egg-info/top_level.txt
 PolyRound/mutable_classes/__init__.py
 PolyRound/mutable_classes/polytope.py
```

### Comparing `PolyRound-0.2.8/README.md` & `PolyRound-0.2.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # PolyRound
 [![PyPI version](https://badge.fury.io/py/PolyRound.svg)](https://badge.fury.io/py/PolyRound)
 
 Efficient random sampling in convex polytopes relies on a 'rounding' preprocessing step, in which the polytope is rescaled so that the width is as uniform as possible across different dimensions.
 PolyRound rounds polytopes on the general form:
 
-![equation](https://latex.codecogs.com/gif.latex?P&space;:=&space;\{x&space;\in&space;\mathcal{R}^n:&space;A_{eq}x&space;=&space;b_{eq},&space;A_{ineq}x&space;\leq&space;b_{ineq}\}) with matrices ![equation](https://latex.codecogs.com/gif.latex?A_{eq}&space;\in&space;\mathcal{R}^{m,n}) and ![equation](https://latex.codecogs.com/gif.latex?A_{ineq}\in&space;\mathcal{R}^{k,n}) and vectors ![equation](https://latex.codecogs.com/gif.latex?b_{eq}&space;\in&space;\mathcal{R}^{m}) and ![equation](https://latex.codecogs.com/gif.latex?b_{ineq}\in&space;\mathcal{R}^{k}).
+$`P:=\{x \in \mathcal{R}^n: A_{eq} x = b_{eq}, A_{ineq} x \leq b_{ineq}\}`$ with matrices $`A_{eq} \in \mathcal{R}^{m,n}`$ and $`A_{ineq} \in \mathcal{R}^{k,n}`$ and vectors $`b_{eq} \in \mathcal{R}^{m}`$ and $`b_{ineq} \in \mathcal{R}^{k}`$.
 
 This formulation often arises in Systems Biology as the flux space of a metabolic network.
 
-As output, PolyRound produces a polytope on the form ![equation](https://latex.codecogs.com/gif.latex?P^{r}&space;:=&space;\{v&space;\in&space;\mathcal{R}^l:&space;A^{r}_{ineq}v&space;\leq&space;b^{r}_{ineq}\}) where ![equation](https://latex.codecogs.com/gif.latex?l&space;\leq&space;n) and the zero vector is a stricly interior point. For transforming points back to the original space, it also provides a matrix ![equation](https://latex.codecogs.com/gif.latex?S&space;\in&space;\mathcal{R}^{n,l}) and a vector ![equation](https://latex.codecogs.com/gif.latex?t&space;\in&space;\mathcal{R}^{n}), so that ![equation](https://latex.codecogs.com/gif.latex?x&space;=&space;Sv&space;&plus;&space;t).
+As output, PolyRound produces a polytope on the form $`P^{r}:=\{v \in \mathcal{R}^l: A^{r}_{ineq}v \leq b^{r}_{ineq}\}`$ where $`l \leq n`$ and the zero vector is a stricly interior point. For transforming points back to the original space, it also provides a matrix $`S \in \mathcal{R}^{n,l}`$ and a vector $`t \in \mathcal{R}^{n}`$, so that $`x=Sv + t`$.
 
 Currently, PolyRound is supported for python 3.7 to 3.9.
 
 PolyRound no longer depends on a Gurobi installation and uses optlang (https://github.com/opencobra/optlang) to delegate linear programs to GLPK in case Gurobi is not installed. However, PolyRound is more reliable with Gurobi. Free Gurobi licenses for academic use can be obtained at https://www.gurobi.com/. Once the license is installed, gurobipy can be installed directly through pip, or by getting the optional requirements by 'pip install -r optional_requirements.txt'.
 
 An easy example of how to get started is presented in the jupyter notebook cells below.
 
 
 They show how to: <br>
 1) create a polytope object from a file path <br>
 2) simplify, reduce, and round a polytope in separate steps, togehter with some printed checks <br>
 3) simplify, reduce and round a polytope in one step <br>
-4) save the rounded polytope in various formats
+4) save the rounded polytope
 
 ``` python
 import os
 from PolyRound.api import PolyRoundApi
 from PolyRound.static_classes.lp_utils import ChebyshevFinder
 from PolyRound.settings import PolyRoundSettings
 from pathlib import Path
+
 model_path = os.path.join("PolyRound", "models", "e_coli_core.xml")
 ```
 
 ``` python
 # Create a settings object with the default settings.
 settings = PolyRoundSettings()
 ```
@@ -50,42 +51,40 @@
 simplified_polytope = PolyRoundApi.simplify_polytope(polytope)
 # The simplified polytope has non-zero border distance
 x, dist = ChebyshevFinder.chebyshev_center(simplified_polytope, settings)
 print(dist)
 ```
 
 ``` python
+# Embed the polytope in a space where it has non-zero volume
 transformed_polytope = PolyRoundApi.transform_polytope(simplified_polytope)
 # The distance from the chebyshev center to the boundary changes in the new coordinate system
 x, dist = ChebyshevFinder.chebyshev_center(transformed_polytope, settings)
 print(dist)
 ```
 
 ``` python
+# Round the polytope
 rounded_polytope = PolyRoundApi.round_polytope(transformed_polytope)
 # After rounding, the distance from the chebyshev center to the boundary is set to be close to 1
 x, dist = ChebyshevFinder.chebyshev_center(rounded_polytope, settings)
 print(dist)
 
 # The chebyshev center can be back transformed into an interior point in the simplified space.
 print(simplified_polytope.border_distance(rounded_polytope.back_transform(x)))
-
 ```
 
 ``` python
 # simplify, transform and round in one call
 one_step_rounded_polytope = PolyRoundApi.simplify_transform_and_round(polytope)
 ```
 
 ``` python
-#save to hdf5
-out_hdf5 = os.path.join("PolyRound", 'output', 'rounded_e_coli_core.hdf5')
-PolyRoundApi.polytope_to_hdf5(one_step_rounded_polytope, out_hdf5)
-#save to csv
-out_csv_dir = os.path.join("PolyRound", 'output', 'e_coli_core')
+# save to csv
+out_csv_dir = os.path.join("PolyRound", "output", "e_coli_core")
 Path(out_csv_dir).mkdir(parents=True, exist_ok=True)
 PolyRoundApi.polytope_to_csvs(one_step_rounded_polytope, out_csv_dir)
 ```
 
 ``` python
 # Special use case: remove redundant constraints without removing zero facettes. This will leave th polytope with its original border distance.
 x, dist = ChebyshevFinder.chebyshev_center(polytope, settings)
```

