# Comparing `tmp/SeaFreeze-0.9.2.post2.tar.gz` & `tmp/SeaFreeze-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SeaFreeze-0.9.2.post2.tar", last modified: Tue Nov 12 02:59:40 2019, max compression
+gzip compressed data, was "SeaFreeze-0.9.3.tar", last modified: Thu Apr 27 22:38:41 2023, max compression
```

## Comparing `SeaFreeze-0.9.2.post2.tar` & `SeaFreeze-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxr-xr-x   0 penny      (501) staff       (20)        0 2019-11-12 02:59:40.000000 SeaFreeze-0.9.2.post2/
--rw-r--r--   0 penny      (501) staff       (20)     1074 2019-11-12 02:59:36.000000 SeaFreeze-0.9.2.post2/LICENSE.txt
--rw-r--r--   0 penny      (501) staff       (20)       20 2019-08-08 20:30:48.000000 SeaFreeze-0.9.2.post2/MANIFEST.in
--rw-r--r--   0 penny      (501) staff       (20)    10102 2019-11-12 02:59:40.000000 SeaFreeze-0.9.2.post2/PKG-INFO
--rw-r--r--   0 penny      (501) staff       (20)     8147 2019-11-12 02:58:57.000000 SeaFreeze-0.9.2.post2/README.md
-drwxr-xr-x   0 penny      (501) staff       (20)        0 2019-11-12 02:59:40.000000 SeaFreeze-0.9.2.post2/seafreeze/
-drwxr-xr-x   0 penny      (501) staff       (20)        0 2019-11-12 02:59:40.000000 SeaFreeze-0.9.2.post2/seafreeze/SeaFreeze.egg-info/
--rw-r--r--   0 penny      (501) staff       (20)    10102 2019-11-12 02:59:39.000000 SeaFreeze-0.9.2.post2/seafreeze/SeaFreeze.egg-info/PKG-INFO
--rw-r--r--   0 penny      (501) staff       (20)      301 2019-11-12 02:59:39.000000 SeaFreeze-0.9.2.post2/seafreeze/SeaFreeze.egg-info/SOURCES.txt
--rw-r--r--   0 penny      (501) staff       (20)        1 2019-11-12 02:59:39.000000 SeaFreeze-0.9.2.post2/seafreeze/SeaFreeze.egg-info/dependency_links.txt
--rw-r--r--   0 penny      (501) staff       (20)       31 2019-11-12 02:59:39.000000 SeaFreeze-0.9.2.post2/seafreeze/SeaFreeze.egg-info/requires.txt
--rw-r--r--   0 penny      (501) staff       (20)        1 2019-11-12 02:59:39.000000 SeaFreeze-0.9.2.post2/seafreeze/SeaFreeze.egg-info/top_level.txt
--rw-r--r--   0 penny      (501) staff       (20)        0 2019-08-08 20:30:48.000000 SeaFreeze-0.9.2.post2/seafreeze/__init__.py
--rw-r--r--   0 penny      (501) staff       (20)     9329 2019-11-11 01:26:41.000000 SeaFreeze-0.9.2.post2/seafreeze/seafreeze.py
--rw-r--r--   0 penny      (501) staff       (20)       38 2019-11-12 02:59:40.000000 SeaFreeze-0.9.2.post2/setup.cfg
--rw-r--r--   0 penny      (501) staff       (20)      828 2019-11-12 02:53:51.000000 SeaFreeze-0.9.2.post2/setup.py
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-04-27 22:38:41.949582 SeaFreeze-0.9.3/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    35129 2023-04-27 22:38:31.000000 SeaFreeze-0.9.3/LICENSE.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       20 2023-04-27 22:34:31.000000 SeaFreeze-0.9.3/MANIFEST.in
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     8681 2023-04-27 22:38:41.949179 SeaFreeze-0.9.3/PKG-INFO
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     8202 2023-04-27 19:34:03.000000 SeaFreeze-0.9.3/README.md
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-04-27 22:38:41.943550 SeaFreeze-0.9.3/SeaFreeze.egg-info/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     8681 2023-04-27 22:38:41.000000 SeaFreeze-0.9.3/SeaFreeze.egg-info/PKG-INFO
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      440 2023-04-27 22:38:41.000000 SeaFreeze-0.9.3/SeaFreeze.egg-info/SOURCES.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)        1 2023-04-27 22:38:41.000000 SeaFreeze-0.9.3/SeaFreeze.egg-info/dependency_links.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       42 2023-04-27 22:38:41.000000 SeaFreeze-0.9.3/SeaFreeze.egg-info/requires.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       26 2023-04-27 22:38:41.000000 SeaFreeze-0.9.3/SeaFreeze.egg-info/top_level.txt
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-04-27 22:38:41.945228 SeaFreeze-0.9.3/lbftd/
+-rw-rw-r--   0 mjstyczi   (503) staff       (20)     3694 2019-08-14 21:37:49.000000 SeaFreeze-0.9.3/lbftd/README.md
+-rw-rw-r--   0 mjstyczi   (503) staff       (20)       84 2019-08-14 21:37:49.000000 SeaFreeze-0.9.3/lbftd/__init__.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    20694 2023-04-27 21:43:55.000000 SeaFreeze-0.9.3/lbftd/evalGibbs.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     2882 2023-04-27 21:36:28.000000 SeaFreeze-0.9.3/lbftd/loadGibbs.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    15885 2023-04-27 21:15:19.000000 SeaFreeze-0.9.3/lbftd/statevars.py
+-rwxr-xr-x   0 mjstyczi   (503) staff       (20)      699 2023-04-27 22:32:58.000000 SeaFreeze-0.9.3/make_dist
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-04-27 22:38:41.946155 SeaFreeze-0.9.3/mlbspline/
+-rw-rw-r--   0 mjstyczi   (503) staff       (20)       72 2019-08-14 21:37:49.000000 SeaFreeze-0.9.3/mlbspline/__init__.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     4182 2023-04-27 21:07:26.000000 SeaFreeze-0.9.3/mlbspline/eval.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5098 2023-04-27 21:08:48.000000 SeaFreeze-0.9.3/mlbspline/load.py
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-04-27 22:38:41.948603 SeaFreeze-0.9.3/seafreeze/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)  1349296 2023-04-27 22:38:31.000000 SeaFreeze-0.9.3/seafreeze/SeaFreeze_Gibbs.mat
+-rw-r--r--   0 mjstyczi   (503) staff       (20)        0 2023-01-07 22:22:07.000000 SeaFreeze-0.9.3/seafreeze/__init__.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     9455 2023-04-27 21:48:58.000000 SeaFreeze-0.9.3/seafreeze/seafreeze.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       38 2023-04-27 22:38:41.949654 SeaFreeze-0.9.3/setup.cfg
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      921 2023-04-27 22:38:15.000000 SeaFreeze-0.9.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SeaFreeze-0.9.2.post2/README.md` & `SeaFreeze-0.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SeaFreeze
 
 V0.9.2
 
-The SeaFreeze package allows computation of the thermodynamic and elastic properties of water and ice polymorphs Ih, III, V and VI in the 0-2300 MPa and 220-500 K range. It is based on the evaluation of Local Basis Functions for each phase. The formalism is described in more details in Brown (2018), Journaux et al. (2019), and in the liquid water Gibbs parameterization by Bollengier, Brown, and Shaw (2019).
+The SeaFreeze package allows computation of the thermodynamic and elastic properties of water and ice polymorphs Ih, II, III, V and VI in the 0-2300 MPa and 220-500 K range. It is based on the evaluation of Local Basis Functions for each phase. The formalism is described in more details in Brown (2018), Journaux et al. (2019), and in the liquid water Gibbs parameterization by Bollengier, Brown, and Shaw (2019).
 
 
 ## Installation
 This package will install [uw-highP-geophysics-tools](https://pypi.org/project/uw-highP-geophysics-tools/) and its dependencies.
 
 Run the following command to install
 
@@ -168,15 +168,16 @@
 * **Penny Espinoza** - *University of Washington, Earth and Space Sciences Department, Seattle, USA* 
 * **Baptiste Journaux** - *University of Washington, Earth and Space Sciences Department, Seattle, USA* 
 * **J. Michael Brown** - *University of Washington, Earth and Space Sciences Department, Seattle, USA* 
 
 ## Change log
 
 ### Changes since 0.9.0
-- `0.9.2`: `whichphase` returns `numpy.nan` if PT is outside the regime of all phases
+- `0.9.2.post2`: `whichphase` returns `numpy.nan` if PT is outside the regime of all phases
+- `0.9.2`: add ice II to the representation.
 - `0.9.1`: add `whichphase` function
 
 ### Changes from 0.8
 - rename function get_phase_thermodynamics to seafreeze
 - reverse order of PT and phase in function signature
 - remove a layer of nesting (`seafreeze.seafreeze` rather than `seafreeze.seafreeze.seafreeze`)
```

### Comparing `SeaFreeze-0.9.2.post2/seafreeze/seafreeze.py` & `SeaFreeze-0.9.3/seafreeze/seafreeze.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from collections import namedtuple
 from itertools import repeat
 import warnings
+import logging
 import os.path as op
 import numpy as np
 from mlbspline import load
 from lbftd import evalGibbs as eg
 from lbftd.statevars import iP, iT
 
+log = logging.getLogger('seafreeze')
+stream = logging.StreamHandler()
+stream.setFormatter(logging.Formatter('[SeaFreeze %(levelname)s] %(message)s'))
 defpath = op.join(op.dirname(op.abspath(__file__)), 'SeaFreeze_Gibbs.mat')
 
 def seafreeze(PT, phase, path=defpath):
     """ Calculates thermodynamic quantities for H2O water or ice polymorphs Ih, III, V, and VI for all phases
         (see lbftd documentation for full list)
         for solid phases only:
             - Vp (compressional wave velocity, in m/s)
@@ -19,107 +23,107 @@
     Requires the SeaFreeze_Gibbs.mat library containing the Gibbs LBF parametrization (installed with this module).
 
     NOTE:  The authors recommend the use of 'water1' for any application in the 200-355 K range and up to 2300 MPa.
     The ice Gibbs parametrizations are optimized for use with the 'water1' phase for phase equilibrium calculations.
     Using other water parametrizations will lead to incorrect melting curves -- 'water2' and 'water_IAPWS95'
     parametrizations are provided for HP extension up to 100 GPa and comparison only.
 
-    :param PT:      the pressure (MPa) and temperature (K) conditions at which the thermodynamic quantities should be
+    :param PT:      The pressure (MPa) and temperature (K) conditions at which the thermodynamic quantities should be
                     calculated -- the specified units are required, as conversions are built into several calculations.
                     This parameter can have one of the following formats:
-                        - a 1-dimensional numpy array of tuples with one or more scattered (P,T) tuples, e.g.
+                        - A 1-dimensional numpy array of tuples with one or more scattered (P,T) tuples, e.g.
                                 PT = np.empty((3,), np.object)
                                 PT[0] = (441.0858, 313.95)
                                 PT[1] = (478.7415, 313.96)
                                 PT[2] = (444.8285, 313.78)
-                        - a numpy array with 2 nested numpy arrays, the first with pressures and the second
+                        - A numpy array with 2 nested numpy arrays, the first with pressures and the second
                           with temperatures -- each inner array must be sorted from low to high values
-                          a grid will be constructed from the P and T arrays such that each row of the output
+                          A grid will be constructed from the P and T arrays such that each row of the output
                           will correspond to a pressure and each column to a temperature, e.g.
                                 P = np.arange(0.1, 1000.2, 10)
                                 T = np.arange(240, 501, 2)
                                 PT = np.array([P, T])
-    :param phase:   one of the keys of the phases dict, indicating the phase of H2O to be evaluated
-    :param path:    an optional path to the SeaFreeze_Gibbs.mat file
+    :param phase:   One of the keys of the phases dict, indicating the phase of H2O to be evaluated
+    :param path:    An optional path to the SeaFreeze_Gibbs.mat file
                     default value assumes the spline distributed along with the project
     :return:        object containing the calculated thermodynamic quantities (as named properties), as well as
-                    a PTM property (a copy of PT)
+                    A PTM property (a copy of PT)
     """
     try:
         phasedesc = phases[phase]
     except KeyError:
-        raise ValueError('The specified phase is not recognized.  Supported phases are ' +
+        raise ValueError('The specified phase is not recognized. Supported phases are ' +
                          ', '.join(phases.keys())+'.')
     sp = load.loadSpline(path, phasedesc.sp_name)
-    # calc density and isentropic bulk modulus
+    # Calc density and isentropic bulk modulus
     isscatter = _is_scatter(PT)
     tdvs = _get_tdvs(sp, PT, isscatter)
     if phasedesc.shear_mod_parms:
         smg = _get_shear_mod_GPa(phasedesc.shear_mod_parms, tdvs.rho, _get_T(PT, isscatter))
-        tdvs.shear = 1e3 * smg  # convert to MPa for consistency with other measures
+        tdvs.shear = 1e3 * smg  # Convert to MPa for consistency with other measures
         tdvs.Vp = _get_Vp(smg, tdvs.rho, tdvs.Ks)
         tdvs.Vs = _get_Vs(smg, tdvs.rho)
     return tdvs
 
 
 def whichphase(PT, path=defpath):
     """ Determines the most likely phase of water at each pressure/temperature
 
-    :param PT:      the pressure (MPa) and temperature (K) conditions at which the phase should be determined --
+    :param PT:      The pressure (MPa) and temperature (K) conditions at which the phase should be determined --
                     the specified units are required, as conversions are built into several calculations.
                     This parameter can have one of the following formats:
                         - a 1-dimensional numpy array of tuples with one or more scattered (P,T) tuples, e.g.
                                 PT = np.empty((3,), np.object)
                                 PT[0] = (441.0858, 313.95)
                                 PT[1] = (478.7415, 313.96)
                                 PT[2] = (444.8285, 313.78)
                         - a numpy array with 2 nested numpy arrays, the first with pressures and the second
                           with temperatures -- each inner array must be sorted from low to high values
                           a grid will be constructed from the P and T arrays such that each row of the output
                           will correspond to a pressure and each column to a temperature, e.g.
                                 P = np.arange(0.1, 1000.2, 10)
                                 T = np.arange(240, 501, 2)
                                 PT = np.array([P, T])
-    :param path:    an optional path to the SeaFreeze_Gibbs.mat file --
+    :param path:    An optional path to the SeaFreeze_Gibbs.mat file --
                     default value assumes the spline distributed along with the project
     :return:        A numpy.ndarray the same size as PT, with the phase of each pressure/temperature represented by
                     an integer, as shown in phasenum2phase
     """
     isscatter = _is_scatter(PT)
     phase_sp = {v.phase_num: load.loadSpline(path, v.sp_name) for v in phases.values() if not np.isnan(v.phase_num)}
-    ptsh = ((PT.size,) if isscatter else (PT[0].size, PT[1].size))      # reference shape based on PT
-    comp = np.full(ptsh + (max_phase_num+1,), np.nan)                   # comparison matrix
+    ptsh = ((PT.size,) if isscatter else (PT[0].size, PT[1].size))  # Reference shape based on PT
+    comp = np.full(ptsh + (max_phase_num+1,), np.nan)  # Comparison matrix
     for p in phase_sp.keys():
-        sl = tuple(repeat(slice(None), 1 if isscatter else 2))+(p,)     # slice for this phase
+        sl = tuple(repeat(slice(None), 1 if isscatter else 2))+(p,)  # Slice for this phase
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             sp = phase_sp[p]
             tdvs = _get_tdvs(sp, PT, isscatter, 'G').G
-            # wipe out G for PT values that fall outside the knot sequence
+            # Wipe out G for PT values that fall outside the knot sequence
             if isscatter:
                 extrap = [(pt[iP] < sp['knots'][iP].min()) + (pt[iP] > sp['knots'][iP].max()) +
                           (pt[iT] < sp['knots'][iT].min()) + (pt[iT] > sp['knots'][iT].max()) for pt in PT]
             else:
                 pt = np.logical_or(PT[iP] < sp['knots'][iP].min(), PT[iP] > sp['knots'][iP].max())
                 tt = np.logical_or(PT[iT] < sp['knots'][iT].min(), PT[iT] > sp['knots'][iT].max())
                 extrap = np.logical_or(*np.meshgrid(pt, tt, indexing='ij'))
             tdvs[extrap] = np.nan
             comp[sl] = tdvs
-    # output for all-nan slices should be nan
-    all_nan_sl = np.all(np.isnan(comp), -1)     # find slices where all values are nan along the innermost axis
-    out = np.full(ptsh, np.nan)        # initialize output to nan
-    out[~all_nan_sl] = np.nanargmin(comp[~all_nan_sl],-1)      # find min values for other slices
+    # Output for all-nan slices should be nan
+    all_nan_sl = np.all(np.isnan(comp), -1)  # Find slices where all values are nan along the innermost axis
+    out = np.full(ptsh, np.nan)  # Initialize output to nan
+    out[~all_nan_sl] = np.nanargmin(comp[~all_nan_sl],-1)  # Find min values for other slices
     return out
 
 
 def _get_tdvs(sp, PT, is_scatter, *tdvSpec):
-    """ peeks into PT to see if the PT data is for grid or scatter and calls the appropriate evalGibbs function
+    """ Peeks into PT to see if the PT data is for grid or scatter and calls the appropriate evalGibbs function
 
-    :param sp:          the Gibbs LBF
-    :param PT:          the PT data
+    :param sp:          The Gibbs LBF
+    :param PT:          The PT data
     :param is_scatter:  Boolean indicating whether the PT data is scatter or not (if not, it is a grid)
     :param tdvSpec:     optional list of thermodynamic variables to calculate (see lbftd documentation)
     :return:            tdv object (see lbftd documentation)
     """
     fn = eg.evalSolutionGibbsScatter if is_scatter else eg.evalSolutionGibbsGrid
     return fn(sp, PT, *tdvSpec, failOnExtrapolate=False)
 
@@ -144,15 +148,15 @@
     return np.array([T for P,T in PT]) if is_scatter else PT[1]
 
 
 #########################################
 ## Constants
 #########################################
 PhaseDesc = namedtuple('PhaseDesc', 'sp_name shear_mod_parms phase_num')
-phases = {"Ih": PhaseDesc("G_iceIh", [3.04, -0.00462, 0, -0.00607, 1000, 273.15], 1),  # Feistel and Wagner, 2006
+phases = {"Ih": PhaseDesc("G_iceIh", [3.1, -0.00462, 0, -0.00657, 1000, 273.15], 1),  # Feistel and Wagner, 2006
           "II": PhaseDesc("G_iceII", [4.1, 0.0175, 0, -0.014, 1100, 273], 2),          # Journaux et al, 2019
           "III": PhaseDesc("G_iceIII", [2.57, 0.0175, 0, -0.014, 1100, 273], 3),       # Journaux et al, 2019
           "V": PhaseDesc("G_iceV", [2.57, 0.0175, 0, -0.014, 1100, 273], 5),           # Journaux et al, 2019
           "VI": PhaseDesc("G_iceVI", [2.57, 0.0175, 0, -0.014, 1100, 273], 6),         # Journaux et al, 2019
           "water1": PhaseDesc("G_H2O_2GPa_500K", None, 0),              # extends to 500 K and 2300 MPa; Bollengier et al 2019
           "water2": PhaseDesc("G_H2O_100GPa_10000K", None, np.nan),     # extends to 100 GPa; Brown 2018
           "water_IAPWS95": PhaseDesc("G_H2O_IAPWS", None, np.nan)       # LBF representation of IAPWS 95; Wagner and Pruß, 2002
```

