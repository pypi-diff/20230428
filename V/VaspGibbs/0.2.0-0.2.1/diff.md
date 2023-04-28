# Comparing `tmp/VaspGibbs-0.2.0.tar.gz` & `tmp/VaspGibbs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VaspGibbs-0.2.0.tar", last modified: Fri Apr 28 01:38:32 2023, max compression
+gzip compressed data, was "VaspGibbs-0.2.1.tar", last modified: Fri Apr 28 03:14:12 2023, max compression
```

## Comparing `VaspGibbs-0.2.0.tar` & `VaspGibbs-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 felixt    (1000) felixt    (1000)        0 2023-04-28 01:38:32.388309 VaspGibbs-0.2.0/
--rw-r--r--   0 felixt    (1000) felixt    (1000)     1071 2023-04-27 22:59:45.000000 VaspGibbs-0.2.0/LICENSE.md
--rw-r--r--   0 felixt    (1000) felixt    (1000)      298 2023-04-28 01:38:32.388309 VaspGibbs-0.2.0/PKG-INFO
--rw-rw-r--   0 felixt    (1000) felixt    (1000)     3746 2023-04-28 01:34:59.000000 VaspGibbs-0.2.0/README.md
-drwxr-xr-x   0 felixt    (1000) felixt    (1000)        0 2023-04-28 01:38:32.387309 VaspGibbs-0.2.0/VaspGibbs.egg-info/
--rw-r--r--   0 felixt    (1000) felixt    (1000)      298 2023-04-28 01:38:32.000000 VaspGibbs-0.2.0/VaspGibbs.egg-info/PKG-INFO
--rw-r--r--   0 felixt    (1000) felixt    (1000)      275 2023-04-28 01:38:32.000000 VaspGibbs-0.2.0/VaspGibbs.egg-info/SOURCES.txt
--rw-r--r--   0 felixt    (1000) felixt    (1000)        1 2023-04-28 01:38:32.000000 VaspGibbs-0.2.0/VaspGibbs.egg-info/dependency_links.txt
--rw-r--r--   0 felixt    (1000) felixt    (1000)        6 2023-04-28 01:38:32.000000 VaspGibbs-0.2.0/VaspGibbs.egg-info/requires.txt
--rw-r--r--   0 felixt    (1000) felixt    (1000)       10 2023-04-28 01:38:32.000000 VaspGibbs-0.2.0/VaspGibbs.egg-info/top_level.txt
--rw-r--r--   0 felixt    (1000) felixt    (1000)      106 2023-04-28 01:38:32.388309 VaspGibbs-0.2.0/setup.cfg
--rw-rw-r--   0 felixt    (1000) felixt    (1000)      457 2022-09-09 18:37:44.000000 VaspGibbs-0.2.0/setup.py
--rwxrwxr-x   0 felixt    (1000) felixt    (1000)     7135 2022-09-28 20:48:48.000000 VaspGibbs-0.2.0/vasp_gibbs
-drwxr-xr-x   0 felixt    (1000) felixt    (1000)        0 2023-04-28 01:38:32.387309 VaspGibbs-0.2.0/vaspgibbs/
--rw-rw-r--   0 felixt    (1000) felixt    (1000)      215 2022-08-04 22:53:27.000000 VaspGibbs-0.2.0/vaspgibbs/__init__.py
--rw-rw-r--   0 felixt    (1000) felixt    (1000)     6069 2022-09-28 20:50:37.000000 VaspGibbs-0.2.0/vaspgibbs/thermo.py
--rw-rw-r--   0 felixt    (1000) felixt    (1000)     5399 2022-09-09 18:37:44.000000 VaspGibbs-0.2.0/vaspgibbs/utils.py
+drwxr-xr-x   0 felixt    (1000) felixt    (1000)        0 2023-04-28 03:14:12.859236 VaspGibbs-0.2.1/
+-rw-r--r--   0 felixt    (1000) felixt    (1000)     1071 2023-04-27 22:59:45.000000 VaspGibbs-0.2.1/LICENSE.md
+-rw-r--r--   0 felixt    (1000) felixt    (1000)      298 2023-04-28 03:14:12.859236 VaspGibbs-0.2.1/PKG-INFO
+-rw-rw-r--   0 felixt    (1000) felixt    (1000)     3772 2023-04-28 02:14:44.000000 VaspGibbs-0.2.1/README.md
+drwxr-xr-x   0 felixt    (1000) felixt    (1000)        0 2023-04-28 03:14:12.859236 VaspGibbs-0.2.1/VaspGibbs.egg-info/
+-rw-r--r--   0 felixt    (1000) felixt    (1000)      298 2023-04-28 03:14:12.000000 VaspGibbs-0.2.1/VaspGibbs.egg-info/PKG-INFO
+-rw-r--r--   0 felixt    (1000) felixt    (1000)      275 2023-04-28 03:14:12.000000 VaspGibbs-0.2.1/VaspGibbs.egg-info/SOURCES.txt
+-rw-r--r--   0 felixt    (1000) felixt    (1000)        1 2023-04-28 03:14:12.000000 VaspGibbs-0.2.1/VaspGibbs.egg-info/dependency_links.txt
+-rw-r--r--   0 felixt    (1000) felixt    (1000)        6 2023-04-28 03:14:12.000000 VaspGibbs-0.2.1/VaspGibbs.egg-info/requires.txt
+-rw-r--r--   0 felixt    (1000) felixt    (1000)       10 2023-04-28 03:14:12.000000 VaspGibbs-0.2.1/VaspGibbs.egg-info/top_level.txt
+-rw-r--r--   0 felixt    (1000) felixt    (1000)      106 2023-04-28 03:14:12.860236 VaspGibbs-0.2.1/setup.cfg
+-rw-rw-r--   0 felixt    (1000) felixt    (1000)      457 2023-04-28 02:18:54.000000 VaspGibbs-0.2.1/setup.py
+-rwxrwxr-x   0 felixt    (1000) felixt    (1000)     7135 2022-09-28 20:48:48.000000 VaspGibbs-0.2.1/vasp_gibbs
+drwxr-xr-x   0 felixt    (1000) felixt    (1000)        0 2023-04-28 03:14:12.859236 VaspGibbs-0.2.1/vaspgibbs/
+-rw-rw-r--   0 felixt    (1000) felixt    (1000)      215 2022-08-04 22:53:27.000000 VaspGibbs-0.2.1/vaspgibbs/__init__.py
+-rw-rw-r--   0 felixt    (1000) felixt    (1000)     6069 2022-09-28 20:50:37.000000 VaspGibbs-0.2.1/vaspgibbs/thermo.py
+-rw-rw-r--   0 felixt    (1000) felixt    (1000)     5399 2022-09-09 18:37:44.000000 VaspGibbs-0.2.1/vaspgibbs/utils.py
```

### Comparing `VaspGibbs-0.2.0/LICENSE.md` & `VaspGibbs-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VaspGibbs-0.2.0/README.md` & `VaspGibbs-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VaspGibbs
 
 A simple way to get Gibbs free energy from Vasp calculations
 
 ## Installation
 
 ```
-pip install vasp_gibbs
+pip install vaspgibbs
 ```
 
 *Latest version:* 0.2.0 (beta)
 
 ## Usage
 
 In a folder with a finished vasp calculation, run
@@ -76,14 +76,18 @@
 * https://pubs.acs.org/doi/abs/10.1021/jp407468t (Supporting Information)
 * https://gaussian.com/thermo/
 * https://wiki.fysik.dtu.dk/ase/ase/thermochemistry/thermochemistry.html
 * https://chem.libretexts.org/Bookshelves/Physical_and_Theoretical_Chemistry_Textbook_Maps/Statistical_Thermodynamics_(Jeschke)/06%3A_Partition_Functions_of_Gases/6.04%3A_Rotational_Partition_Function
 * https://vaspkit.com/tutorials.html#thermo-energy-correction
 * https://uregina.ca/~eastalla/entropy.pdf (https://doi.org/10.1063/1.473958)
 
+## Citation
+
+Coming Soon!
+
 ## Under development
 
 Results have been checked with [J. Phys. Chem. C 2013, 117, 49](https://pubs.acs.org/doi/abs/10.1021/jp407468t). More validation needs to be done; use with care.
 
 *Next steps:* more testing, add to pypi, PV term for solids with Murnaghan equation, hindered translator and rotor?
 
 Let me know if you would like new features to be added!
```

### Comparing `VaspGibbs-0.2.0/vasp_gibbs` & `VaspGibbs-0.2.1/vasp_gibbs`

 * *Files identical despite different names*

### Comparing `VaspGibbs-0.2.0/vaspgibbs/thermo.py` & `VaspGibbs-0.2.1/vaspgibbs/thermo.py`

 * *Files identical despite different names*

### Comparing `VaspGibbs-0.2.0/vaspgibbs/utils.py` & `VaspGibbs-0.2.1/vaspgibbs/utils.py`

 * *Files identical despite different names*

