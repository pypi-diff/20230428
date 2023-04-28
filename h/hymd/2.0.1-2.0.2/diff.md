# Comparing `tmp/hymd-2.0.1.tar.gz` & `tmp/hymd-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hymd-2.0.1.tar", last modified: Wed Apr  5 15:34:58 2023, max compression
+gzip compressed data, was "hymd-2.0.2.tar", last modified: Fri Apr 28 15:24:00 2023, max compression
```

## Comparing `hymd-2.0.1.tar` & `hymd-2.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:34:58.060209 hymd-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-05 15:29:23.000000 hymd-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-04-05 15:34:58.060209 hymd-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-05 15:29:23.000000 hymd-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:34:58.060209 hymd-2.0.1/hymd/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/barostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/barostat_scr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_angle_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_angle_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_bond_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_bond_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_dihedral_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_dihedral_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/configure_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/dipole_reconstruction.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/dipole_reconstruction__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)    46365 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    26666 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    29848 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/force.py
--rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/gaussian_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    52393 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    50045 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:34:58.060209 hymd-2.0.1/hymd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-05 15:29:23.000000 hymd-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:34:58.060209 hymd-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-05 15:29:23.000000 hymd-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:34:58.060209 hymd-2.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_configure_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_distribute_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_force.py
--rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    33165 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:00.478704 hymd-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-28 15:17:50.000000 hymd-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-28 15:24:00.478704 hymd-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-28 15:17:50.000000 hymd-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:00.474704 hymd-2.0.2/hymd/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/barostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/barostat_scr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_angle_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_angle_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_bond_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_bond_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_dihedral_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_dihedral_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/configure_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/dipole_reconstruction.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/dipole_reconstruction__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    46365 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26666 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29848 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/gaussian_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52393 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50045 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:00.474704 hymd-2.0.2/hymd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 15:17:50.000000 hymd-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 15:24:00.478704 hymd-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-28 15:17:50.000000 hymd-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:00.474704 hymd-2.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_configure_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_distribute_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33165 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_thermostat.py
```

### Comparing `hymd-2.0.1/LICENSE.txt` & `hymd-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/PKG-INFO` & `hymd-2.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hymd
-Version: 2.0.1
+Version: 2.0.2
 Summary: Massively parallel hybrid particle-field MD
 Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum
 Author-email: morten.ledum@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -24,26 +24,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <a href="https://cascella-group-uio.github.io/HyMD/">
   <img src="https://github.com/Cascella-Group-UiO/HyMD/blob/main/docs/img/hymd_logo_text_black.png?raw=true" width="500" title="HylleraasMD">
 </a>
 
-[![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd)
+[![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd) [![status](https://joss.theoj.org/papers/5ea61fe1ad1657834b9efb30c66bc64d/status.svg)](https://joss.theoj.org/papers/5ea61fe1ad1657834b9efb30c66bc64d)
+
 
 ---------
 **HylleraasMD** (HyMD) is a massively parallel Python package for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter systems.
 
 HyMD can run canonical hPF-MD simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic interactions. It includes all standard intramolecular interactions,
 including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics.
 It can run simulations in constant energy (NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [[4]](#4).
 
 HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python).
 File IO is done via HDF5 formats to allow MPI parallel reads.
 
+If you use HyMD, [please cite our paper(s)](#citehead). 
+
 ## User Guide
 Detailed installation and user guide, together with comprehensive example simulations are located in the [HylleraasMD documentation](https://cascella-group-uio.github.io/HyMD/index.html).
 
 Run simulations by
 ```bash
 python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--OPTIONAL_ARGS)
 ```
@@ -83,43 +86,77 @@
 /app$ # Grab example input files
 /app$ curl -O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/ideal_chain/ideal_chain.toml
 /app$ curl -O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/ideal_chain/ideal_chain.HDF5
 /app$
 /app$ # Run simulation
 /app$ python3 -m hymd ideal_chain.toml ideal_chain.HDF5 --verbose
 ```
-
 ## Run tests
 Clone the repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash
 git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd
 cd hymd
 python3 -m pip install pytest pytest-mpi
 pytest
 ```
+
 Running MPI enabled pytest tests is simplified with a convenient script
 ```bash
 chmod +x pytest-mpi
 pytest-mpi -oo -n 2 -ns
 ```
 
-## Please cite our work
-If you use HyMD for your purposes, please cite the appropriate references from the section below.  
-If you cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4). 
+## Contributions and issues
+We welcome contributions to our code and provide a set of guidelines to follow in [CONTRIBUTING.md](CONTRIBUTING.md).  
+To seek support in case of any issues and bugs, we welcome you to post them using the [issue tracker](https://github.com/Cascella-Group-UiO/HyMD/issues). 
+
+## <a name="citehead"></a>Please cite our work
+You will find information about our publications and archived data since 2023 at the open repository: [Publications](https://github.com/Cascella-Group-UiO/Publications).  
+If you use HyMD, please cite:  
+```bibtex
+@article{
+  Ledum_HylleraasMD_Massively_parallel_2023,
+  author = {Ledum, Morten and Carrer, Manuel and Sen, Samiran and Li, Xinmeng and Cascella, Michele and Bore, Sigbjørn Løland},
+  doi = {10.21105/joss.04149},
+  journal = {Journal of Open Source Software},
+  month = {apr},
+  number = {84},
+  pages = {4149},
+  title = {{HylleraasMD: Massively parallel hybrid particle-field molecular dynamics in Python}},
+  url = {https://joss.theoj.org/papers/10.21105/joss.04149},
+  volume = {8},
+  year = {2023}
+}
+
+@article{
+   Sen_HylleraasMD_2023,
+   author = {Sen, Samiran and Ledum, Morten and Bore, Sigbjørn Løland and Cascella, Michele},
+   title = {Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble},
+   doi = {10.1021/acs.jcim.3c00186},
+   journal = {Journal of Chemical Information and Modeling},
+   month= mar,
+   year = {2023},
+   volume = {63},
+   number = {7},
+   pages = {2207-2217},
+   URL = {https://doi.org/10.1021/acs.jcim.3c00186},
+}
+
+```
 
 ---------
 
 ### References
 <a id="1">[1]</a>
 Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv 2021
 
 <a id="2">[2]</a>
-Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
+Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python. Journal of Open Source Software (JOSS) 2023, 8(84), 2475-9066, 4149.
 
 <a id="3">[3]</a>
 Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
 
 <a id="4">[4]</a>
-Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023
+Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. J Chem Inf Model 2023, 63(7), 1549-9596.
 
 <a id="5">[5]</a>
 Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213–C236.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hymd Version: 2.0.1 Summary: Massively parallel
+Metadata-Version: 2.1 Name: hymd Version: 2.0.2 Summary: Massively parallel
 hybrid particle-field MD Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum Author-email: morten.ledum@gmail.com License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -17,30 +17,33 @@
 badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) !
 [build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/
 badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/
 workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/
 ) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/
 badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [!
 [PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/
-hymd) --------- **HylleraasMD** (HyMD) is a massively parallel Python package
-for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations
-of coarse-grained bio- and soft-matter systems. HyMD can run canonical hPF-MD
-simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]]
-(#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic
-interactions. It includes all standard intramolecular interactions, including
-stretching, bending, torsional, and combined bending-dihedral potentials.
-Additionally, topological reconstruction of permanent peptide chain backbone
-dipoles is possible for accurate recreation of protein conformational dynamics.
-It can run simulations in constant energy (NVE), constant volume (NVT) [[1]]
-(#1) or constant pressure (NPT) conditions [[4]](#4). HyMD uses the [pmesh]
-(github.com/rainwoodman/pmesh) library for particle-mesh operations, with the
-PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/
-rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI
-parallel reads. ## User Guide Detailed installation and user guide, together
-with comprehensive example simulations are located in the [HylleraasMD
+hymd) [![status](https://joss.theoj.org/papers/
+5ea61fe1ad1657834b9efb30c66bc64d/status.svg)](https://joss.theoj.org/papers/
+5ea61fe1ad1657834b9efb30c66bc64d) --------- **HylleraasMD** (HyMD) is a
+massively parallel Python package for Hamiltonian hybrid particle-field
+molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter
+systems. HyMD can run canonical hPF-MD simulations, or filtered density
+Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or
+without explicit PME electrostatic interactions. It includes all standard
+intramolecular interactions, including stretching, bending, torsional, and
+combined bending-dihedral potentials. Additionally, topological reconstruction
+of permanent peptide chain backbone dipoles is possible for accurate recreation
+of protein conformational dynamics. It can run simulations in constant energy
+(NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [
+[4]](#4). HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for
+particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the
+[pfft-python bindings](github.com/rainwoodman/pfft-python). File IO is done via
+HDF5 formats to allow MPI parallel reads. If you use HyMD, [please cite our
+paper(s)](#citehead). ## User Guide Detailed installation and user guide,
+together with comprehensive example simulations are located in the [HylleraasMD
 documentation](https://cascella-group-uio.github.io/HyMD/index.html). Run
 simulations by ```bash python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--
 OPTIONAL_ARGS) ``` #### Run interactively in Google Colaboratory A [Google
 Colaboratory](https://colab.research.google.com/) jupyter notebook is setup
 [here](https://colab.research.google.com/drive/
 1jfzRaXjL3q53J4U8OrCgADepmf_HuCOh?usp=sharing) with a working HyMD fully
 installed and executable in the browser. ## Installation #### Non-Python
@@ -65,21 +68,39 @@
 O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/
 ideal_chain/ideal_chain.HDF5 /app$ /app$ # Run simulation /app$ python3 -m hymd
 ideal_chain.toml ideal_chain.HDF5 --verbose ``` ## Run tests Clone the
 repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd cd hymd
 python3 -m pip install pytest pytest-mpi pytest ``` Running MPI enabled pytest
 tests is simplified with a convenient script ```bash chmod +x pytest-mpi
-pytest-mpi -oo -n 2 -ns ``` ## Please cite our work If you use HyMD for your
-purposes, please cite the appropriate references from the section below. If you
-cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4).
---------- ### References [1] Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.;
-Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid
-Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv
-2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L.
-HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
-[3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid
-particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106. [4] Sen,
-S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing
-ParticleâField Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023 [5]
-Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM
-J. Sci. Comput. 2013, 35, C213âC236.
+pytest-mpi -oo -n 2 -ns ``` ## Contributions and issues We welcome
+contributions to our code and provide a set of guidelines to follow in
+[CONTRIBUTING.md](CONTRIBUTING.md). To seek support in case of any issues and
+bugs, we welcome you to post them using the [issue tracker](https://github.com/
+Cascella-Group-UiO/HyMD/issues). ## Please cite our work You will find
+information about our publications and archived data since 2023 at the open
+repository: [Publications](https://github.com/Cascella-Group-UiO/Publications).
+If you use HyMD, please cite: ```bibtex @article
+{ Ledum_HylleraasMD_Massively_parallel_2023, author = {Ledum, Morten and
+Carrer, Manuel and Sen, Samiran and Li, Xinmeng and Cascella, Michele and Bore,
+SigbjÃ¸rn LÃ¸land}, doi = {10.21105/joss.04149}, journal = {Journal of Open
+Source Software}, month = {apr}, number = {84}, pages = {4149}, title = {
+{HylleraasMD: Massively parallel hybrid particle-field molecular dynamics in
+Python}}, url = {https://joss.theoj.org/papers/10.21105/joss.04149}, volume =
+{8}, year = {2023} } @article{ Sen_HylleraasMD_2023, author = {Sen, Samiran and
+Ledum, Morten and Bore, SigbjÃ¸rn LÃ¸land and Cascella, Michele}, title = {Soft
+Matter under Pressure: Pushing ParticleâField Molecular Dynamics to the
+Isobaric Ensemble}, doi = {10.1021/acs.jcim.3c00186}, journal = {Journal of
+Chemical Information and Modeling}, month= mar, year = {2023}, volume = {63},
+number = {7}, pages = {2207-2217}, URL = {https://doi.org/10.1021/
+acs.jcim.3c00186}, } ``` --------- ### References [1] Ledum, M.; Sen, S.; Li,
+X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain
+Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations
+of Soft Matter. ChemRxiv 2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.;
+Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field
+molecular dynamics in Python. Journal of Open Source Software (JOSS) 2023, 8
+(84), 2475-9066, 4149. [3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free
+hybrid particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
+[4] Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure:
+Pushing ParticleâField Molecular Dynamics to the Isobaric Ensemble. J Chem
+Inf Model 2023, 63(7), 1549-9596. [5] Pippig, M. PFFT: An extension of FFTW to
+massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213âC236.
```

### Comparing `hymd-2.0.1/README.md` & `hymd-2.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 <a href="https://cascella-group-uio.github.io/HyMD/">
   <img src="https://github.com/Cascella-Group-UiO/HyMD/blob/main/docs/img/hymd_logo_text_black.png?raw=true" width="500" title="HylleraasMD">
 </a>
 
-[![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd)
+[![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd) [![status](https://joss.theoj.org/papers/5ea61fe1ad1657834b9efb30c66bc64d/status.svg)](https://joss.theoj.org/papers/5ea61fe1ad1657834b9efb30c66bc64d)
+
 
 ---------
 **HylleraasMD** (HyMD) is a massively parallel Python package for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter systems.
 
 HyMD can run canonical hPF-MD simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic interactions. It includes all standard intramolecular interactions,
 including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics.
 It can run simulations in constant energy (NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [[4]](#4).
 
 HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python).
 File IO is done via HDF5 formats to allow MPI parallel reads.
 
+If you use HyMD, [please cite our paper(s)](#citehead). 
+
 ## User Guide
 Detailed installation and user guide, together with comprehensive example simulations are located in the [HylleraasMD documentation](https://cascella-group-uio.github.io/HyMD/index.html).
 
 Run simulations by
 ```bash
 python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--OPTIONAL_ARGS)
 ```
@@ -57,43 +60,77 @@
 /app$ # Grab example input files
 /app$ curl -O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/ideal_chain/ideal_chain.toml
 /app$ curl -O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/ideal_chain/ideal_chain.HDF5
 /app$
 /app$ # Run simulation
 /app$ python3 -m hymd ideal_chain.toml ideal_chain.HDF5 --verbose
 ```
-
 ## Run tests
 Clone the repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash
 git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd
 cd hymd
 python3 -m pip install pytest pytest-mpi
 pytest
 ```
+
 Running MPI enabled pytest tests is simplified with a convenient script
 ```bash
 chmod +x pytest-mpi
 pytest-mpi -oo -n 2 -ns
 ```
 
-## Please cite our work
-If you use HyMD for your purposes, please cite the appropriate references from the section below.  
-If you cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4). 
+## Contributions and issues
+We welcome contributions to our code and provide a set of guidelines to follow in [CONTRIBUTING.md](CONTRIBUTING.md).  
+To seek support in case of any issues and bugs, we welcome you to post them using the [issue tracker](https://github.com/Cascella-Group-UiO/HyMD/issues). 
+
+## <a name="citehead"></a>Please cite our work
+You will find information about our publications and archived data since 2023 at the open repository: [Publications](https://github.com/Cascella-Group-UiO/Publications).  
+If you use HyMD, please cite:  
+```bibtex
+@article{
+  Ledum_HylleraasMD_Massively_parallel_2023,
+  author = {Ledum, Morten and Carrer, Manuel and Sen, Samiran and Li, Xinmeng and Cascella, Michele and Bore, Sigbjørn Løland},
+  doi = {10.21105/joss.04149},
+  journal = {Journal of Open Source Software},
+  month = {apr},
+  number = {84},
+  pages = {4149},
+  title = {{HylleraasMD: Massively parallel hybrid particle-field molecular dynamics in Python}},
+  url = {https://joss.theoj.org/papers/10.21105/joss.04149},
+  volume = {8},
+  year = {2023}
+}
+
+@article{
+   Sen_HylleraasMD_2023,
+   author = {Sen, Samiran and Ledum, Morten and Bore, Sigbjørn Løland and Cascella, Michele},
+   title = {Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble},
+   doi = {10.1021/acs.jcim.3c00186},
+   journal = {Journal of Chemical Information and Modeling},
+   month= mar,
+   year = {2023},
+   volume = {63},
+   number = {7},
+   pages = {2207-2217},
+   URL = {https://doi.org/10.1021/acs.jcim.3c00186},
+}
+
+```
 
 ---------
 
 ### References
 <a id="1">[1]</a>
 Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv 2021
 
 <a id="2">[2]</a>
-Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
+Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python. Journal of Open Source Software (JOSS) 2023, 8(84), 2475-9066, 4149.
 
 <a id="3">[3]</a>
 Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
 
 <a id="4">[4]</a>
-Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023
+Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. J Chem Inf Model 2023, 63(7), 1549-9596.
 
 <a id="5">[5]</a>
 Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213–C236.
```

#### html2text {}

```diff
@@ -3,30 +3,33 @@
 badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) !
 [build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/
 badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/
 workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/
 ) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/
 badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [!
 [PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/
-hymd) --------- **HylleraasMD** (HyMD) is a massively parallel Python package
-for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations
-of coarse-grained bio- and soft-matter systems. HyMD can run canonical hPF-MD
-simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]]
-(#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic
-interactions. It includes all standard intramolecular interactions, including
-stretching, bending, torsional, and combined bending-dihedral potentials.
-Additionally, topological reconstruction of permanent peptide chain backbone
-dipoles is possible for accurate recreation of protein conformational dynamics.
-It can run simulations in constant energy (NVE), constant volume (NVT) [[1]]
-(#1) or constant pressure (NPT) conditions [[4]](#4). HyMD uses the [pmesh]
-(github.com/rainwoodman/pmesh) library for particle-mesh operations, with the
-PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/
-rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI
-parallel reads. ## User Guide Detailed installation and user guide, together
-with comprehensive example simulations are located in the [HylleraasMD
+hymd) [![status](https://joss.theoj.org/papers/
+5ea61fe1ad1657834b9efb30c66bc64d/status.svg)](https://joss.theoj.org/papers/
+5ea61fe1ad1657834b9efb30c66bc64d) --------- **HylleraasMD** (HyMD) is a
+massively parallel Python package for Hamiltonian hybrid particle-field
+molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter
+systems. HyMD can run canonical hPF-MD simulations, or filtered density
+Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or
+without explicit PME electrostatic interactions. It includes all standard
+intramolecular interactions, including stretching, bending, torsional, and
+combined bending-dihedral potentials. Additionally, topological reconstruction
+of permanent peptide chain backbone dipoles is possible for accurate recreation
+of protein conformational dynamics. It can run simulations in constant energy
+(NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [
+[4]](#4). HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for
+particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the
+[pfft-python bindings](github.com/rainwoodman/pfft-python). File IO is done via
+HDF5 formats to allow MPI parallel reads. If you use HyMD, [please cite our
+paper(s)](#citehead). ## User Guide Detailed installation and user guide,
+together with comprehensive example simulations are located in the [HylleraasMD
 documentation](https://cascella-group-uio.github.io/HyMD/index.html). Run
 simulations by ```bash python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--
 OPTIONAL_ARGS) ``` #### Run interactively in Google Colaboratory A [Google
 Colaboratory](https://colab.research.google.com/) jupyter notebook is setup
 [here](https://colab.research.google.com/drive/
 1jfzRaXjL3q53J4U8OrCgADepmf_HuCOh?usp=sharing) with a working HyMD fully
 installed and executable in the browser. ## Installation #### Non-Python
@@ -51,21 +54,39 @@
 O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/
 ideal_chain/ideal_chain.HDF5 /app$ /app$ # Run simulation /app$ python3 -m hymd
 ideal_chain.toml ideal_chain.HDF5 --verbose ``` ## Run tests Clone the
 repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd cd hymd
 python3 -m pip install pytest pytest-mpi pytest ``` Running MPI enabled pytest
 tests is simplified with a convenient script ```bash chmod +x pytest-mpi
-pytest-mpi -oo -n 2 -ns ``` ## Please cite our work If you use HyMD for your
-purposes, please cite the appropriate references from the section below. If you
-cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4).
---------- ### References [1] Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.;
-Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid
-Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv
-2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L.
-HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
-[3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid
-particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106. [4] Sen,
-S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing
-ParticleâField Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023 [5]
-Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM
-J. Sci. Comput. 2013, 35, C213âC236.
+pytest-mpi -oo -n 2 -ns ``` ## Contributions and issues We welcome
+contributions to our code and provide a set of guidelines to follow in
+[CONTRIBUTING.md](CONTRIBUTING.md). To seek support in case of any issues and
+bugs, we welcome you to post them using the [issue tracker](https://github.com/
+Cascella-Group-UiO/HyMD/issues). ## Please cite our work You will find
+information about our publications and archived data since 2023 at the open
+repository: [Publications](https://github.com/Cascella-Group-UiO/Publications).
+If you use HyMD, please cite: ```bibtex @article
+{ Ledum_HylleraasMD_Massively_parallel_2023, author = {Ledum, Morten and
+Carrer, Manuel and Sen, Samiran and Li, Xinmeng and Cascella, Michele and Bore,
+SigbjÃ¸rn LÃ¸land}, doi = {10.21105/joss.04149}, journal = {Journal of Open
+Source Software}, month = {apr}, number = {84}, pages = {4149}, title = {
+{HylleraasMD: Massively parallel hybrid particle-field molecular dynamics in
+Python}}, url = {https://joss.theoj.org/papers/10.21105/joss.04149}, volume =
+{8}, year = {2023} } @article{ Sen_HylleraasMD_2023, author = {Sen, Samiran and
+Ledum, Morten and Bore, SigbjÃ¸rn LÃ¸land and Cascella, Michele}, title = {Soft
+Matter under Pressure: Pushing ParticleâField Molecular Dynamics to the
+Isobaric Ensemble}, doi = {10.1021/acs.jcim.3c00186}, journal = {Journal of
+Chemical Information and Modeling}, month= mar, year = {2023}, volume = {63},
+number = {7}, pages = {2207-2217}, URL = {https://doi.org/10.1021/
+acs.jcim.3c00186}, } ``` --------- ### References [1] Ledum, M.; Sen, S.; Li,
+X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain
+Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations
+of Soft Matter. ChemRxiv 2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.;
+Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field
+molecular dynamics in Python. Journal of Open Source Software (JOSS) 2023, 8
+(84), 2475-9066, 4149. [3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free
+hybrid particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
+[4] Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure:
+Pushing ParticleâField Molecular Dynamics to the Isobaric Ensemble. J Chem
+Inf Model 2023, 63(7), 1549-9596. [5] Pippig, M. PFFT: An extension of FFTW to
+massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213âC236.
```

### Comparing `hymd-2.0.1/hymd/barostat.py` & `hymd-2.0.2/hymd/barostat.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/barostat_scr.py` & `hymd-2.0.2/hymd/barostat_scr.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/compute_angle_forces.f90` & `hymd-2.0.2/hymd/compute_angle_forces.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/compute_angle_forces__double.f90` & `hymd-2.0.2/hymd/compute_angle_forces__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/compute_bond_forces.f90` & `hymd-2.0.2/hymd/compute_bond_forces.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/compute_bond_forces__double.f90` & `hymd-2.0.2/hymd/compute_bond_forces__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/compute_dihedral_forces.f90` & `hymd-2.0.2/hymd/compute_dihedral_forces.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/compute_dihedral_forces__double.f90` & `hymd-2.0.2/hymd/compute_dihedral_forces__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/configure_runtime.py` & `hymd-2.0.2/hymd/configure_runtime.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/dipole_reconstruction.f90` & `hymd-2.0.2/hymd/dipole_reconstruction.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/dipole_reconstruction__double.f90` & `hymd-2.0.2/hymd/dipole_reconstruction__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/field.py` & `hymd-2.0.2/hymd/field.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/file_io.py` & `hymd-2.0.2/hymd/file_io.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/force.py` & `hymd-2.0.2/hymd/force.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/gaussian_core.py` & `hymd-2.0.2/hymd/gaussian_core.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/hamiltonian.py` & `hymd-2.0.2/hymd/hamiltonian.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,14 +167,21 @@
         def V_bar_elec(
             psi,
             t,
             type_charges=self.config.type_charges,
         ):
             return type_charges[t] * psi
 
+        self.V_bar_0 = [
+            sympy.lambdify(
+                [(self.phi)], V_bar_0(self.phi, t)
+            )
+            for t in range(self.config.n_types)
+        ]
+
         self.V_bar = [
             sympy.lambdify(
                 [(self.phi, self.psi)], V_bar_0(self.phi, t) + V_bar_elec(self.psi, t)
             )
             for t in range(self.config.n_types)
         ]
 
@@ -275,14 +282,21 @@
         def V_bar_elec(
             psi,
             t,
             type_charges=self.config.type_charges,
         ):
             return type_charges[t] * psi
 
+        self.V_bar_0 = [
+            sympy.lambdify(
+                [(self.phi)], V_bar_0(self.phi, t)
+            )
+            for t in range(self.config.n_types)
+        ]
+
         self.V_bar = [
             sympy.lambdify(
                 [(self.phi, self.psi)], V_bar_0(self.phi, t) + V_bar_elec(self.psi, t)
             )
             for t in range(self.config.n_types)
         ]
 
@@ -435,14 +449,21 @@
         def V_bar_elec(
             psi,
             t,
             type_charges=self.config.type_charges,
         ):
             return type_charges[t] * psi
 
+        self.V_bar_0 = [
+            sympy.lambdify(
+                [(self.phi)], V_bar_0(self.phi, t)
+            )
+            for t in range(self.config.n_types)
+        ]
+
         self.V_bar = [
             sympy.lambdify(
                 [(self.phi, self.psi)], V_bar_0(self.phi, t) + V_bar_elec(self.psi, t)
             )
             for t in range(self.config.n_types)
         ]
```

### Comparing `hymd-2.0.1/hymd/input_parser.py` & `hymd-2.0.2/hymd/input_parser.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/integrator.py` & `hymd-2.0.2/hymd/integrator.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/logger.py` & `hymd-2.0.2/hymd/logger.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/main.py` & `hymd-2.0.2/hymd/main.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd/pressure.py` & `hymd-2.0.2/hymd/pressure.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,18 @@
     kinetic_energy = 0.5 * config.mass * np.sum(velocities**2)
     p_kin = 2 / (3 * V) * kinetic_energy
 
     # Term 1
     p0 = -1 / V * np.sum(w)
 
     # Term 2
-    V_bar = np.array([hamiltonian.V_bar[k]([phi, psi]) for k in range(config.n_types)])
+    if psi is not None: # if using electrostatics
+        V_bar = np.array([hamiltonian.V_bar[k]([phi, psi]) for k in range(config.n_types)])
+    else:
+        V_bar = np.array([hamiltonian.V_bar_0[k](phi) for k in range(config.n_types)])
 
     p1 = np.sum((volume_per_cell / V) * V_bar * phi)
 
     # Term 3
     comp_laplacian(
         phi_fourier,
         phi_transfer,
```

### Comparing `hymd-2.0.1/hymd/thermostat.py` & `hymd-2.0.2/hymd/thermostat.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/hymd.egg-info/PKG-INFO` & `hymd-2.0.2/hymd.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hymd
-Version: 2.0.1
+Version: 2.0.2
 Summary: Massively parallel hybrid particle-field MD
 Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum
 Author-email: morten.ledum@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -24,26 +24,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <a href="https://cascella-group-uio.github.io/HyMD/">
   <img src="https://github.com/Cascella-Group-UiO/HyMD/blob/main/docs/img/hymd_logo_text_black.png?raw=true" width="500" title="HylleraasMD">
 </a>
 
-[![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd)
+[![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd) [![status](https://joss.theoj.org/papers/5ea61fe1ad1657834b9efb30c66bc64d/status.svg)](https://joss.theoj.org/papers/5ea61fe1ad1657834b9efb30c66bc64d)
+
 
 ---------
 **HylleraasMD** (HyMD) is a massively parallel Python package for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter systems.
 
 HyMD can run canonical hPF-MD simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic interactions. It includes all standard intramolecular interactions,
 including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics.
 It can run simulations in constant energy (NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [[4]](#4).
 
 HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python).
 File IO is done via HDF5 formats to allow MPI parallel reads.
 
+If you use HyMD, [please cite our paper(s)](#citehead). 
+
 ## User Guide
 Detailed installation and user guide, together with comprehensive example simulations are located in the [HylleraasMD documentation](https://cascella-group-uio.github.io/HyMD/index.html).
 
 Run simulations by
 ```bash
 python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--OPTIONAL_ARGS)
 ```
@@ -83,43 +86,77 @@
 /app$ # Grab example input files
 /app$ curl -O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/ideal_chain/ideal_chain.toml
 /app$ curl -O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/ideal_chain/ideal_chain.HDF5
 /app$
 /app$ # Run simulation
 /app$ python3 -m hymd ideal_chain.toml ideal_chain.HDF5 --verbose
 ```
-
 ## Run tests
 Clone the repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash
 git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd
 cd hymd
 python3 -m pip install pytest pytest-mpi
 pytest
 ```
+
 Running MPI enabled pytest tests is simplified with a convenient script
 ```bash
 chmod +x pytest-mpi
 pytest-mpi -oo -n 2 -ns
 ```
 
-## Please cite our work
-If you use HyMD for your purposes, please cite the appropriate references from the section below.  
-If you cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4). 
+## Contributions and issues
+We welcome contributions to our code and provide a set of guidelines to follow in [CONTRIBUTING.md](CONTRIBUTING.md).  
+To seek support in case of any issues and bugs, we welcome you to post them using the [issue tracker](https://github.com/Cascella-Group-UiO/HyMD/issues). 
+
+## <a name="citehead"></a>Please cite our work
+You will find information about our publications and archived data since 2023 at the open repository: [Publications](https://github.com/Cascella-Group-UiO/Publications).  
+If you use HyMD, please cite:  
+```bibtex
+@article{
+  Ledum_HylleraasMD_Massively_parallel_2023,
+  author = {Ledum, Morten and Carrer, Manuel and Sen, Samiran and Li, Xinmeng and Cascella, Michele and Bore, Sigbjørn Løland},
+  doi = {10.21105/joss.04149},
+  journal = {Journal of Open Source Software},
+  month = {apr},
+  number = {84},
+  pages = {4149},
+  title = {{HylleraasMD: Massively parallel hybrid particle-field molecular dynamics in Python}},
+  url = {https://joss.theoj.org/papers/10.21105/joss.04149},
+  volume = {8},
+  year = {2023}
+}
+
+@article{
+   Sen_HylleraasMD_2023,
+   author = {Sen, Samiran and Ledum, Morten and Bore, Sigbjørn Løland and Cascella, Michele},
+   title = {Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble},
+   doi = {10.1021/acs.jcim.3c00186},
+   journal = {Journal of Chemical Information and Modeling},
+   month= mar,
+   year = {2023},
+   volume = {63},
+   number = {7},
+   pages = {2207-2217},
+   URL = {https://doi.org/10.1021/acs.jcim.3c00186},
+}
+
+```
 
 ---------
 
 ### References
 <a id="1">[1]</a>
 Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv 2021
 
 <a id="2">[2]</a>
-Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
+Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python. Journal of Open Source Software (JOSS) 2023, 8(84), 2475-9066, 4149.
 
 <a id="3">[3]</a>
 Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
 
 <a id="4">[4]</a>
-Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023
+Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. J Chem Inf Model 2023, 63(7), 1549-9596.
 
 <a id="5">[5]</a>
 Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213–C236.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hymd Version: 2.0.1 Summary: Massively parallel
+Metadata-Version: 2.1 Name: hymd Version: 2.0.2 Summary: Massively parallel
 hybrid particle-field MD Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum Author-email: morten.ledum@gmail.com License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -17,30 +17,33 @@
 badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) !
 [build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/
 badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/
 workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/
 ) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/
 badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [!
 [PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/
-hymd) --------- **HylleraasMD** (HyMD) is a massively parallel Python package
-for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations
-of coarse-grained bio- and soft-matter systems. HyMD can run canonical hPF-MD
-simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]]
-(#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic
-interactions. It includes all standard intramolecular interactions, including
-stretching, bending, torsional, and combined bending-dihedral potentials.
-Additionally, topological reconstruction of permanent peptide chain backbone
-dipoles is possible for accurate recreation of protein conformational dynamics.
-It can run simulations in constant energy (NVE), constant volume (NVT) [[1]]
-(#1) or constant pressure (NPT) conditions [[4]](#4). HyMD uses the [pmesh]
-(github.com/rainwoodman/pmesh) library for particle-mesh operations, with the
-PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/
-rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI
-parallel reads. ## User Guide Detailed installation and user guide, together
-with comprehensive example simulations are located in the [HylleraasMD
+hymd) [![status](https://joss.theoj.org/papers/
+5ea61fe1ad1657834b9efb30c66bc64d/status.svg)](https://joss.theoj.org/papers/
+5ea61fe1ad1657834b9efb30c66bc64d) --------- **HylleraasMD** (HyMD) is a
+massively parallel Python package for Hamiltonian hybrid particle-field
+molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter
+systems. HyMD can run canonical hPF-MD simulations, or filtered density
+Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or
+without explicit PME electrostatic interactions. It includes all standard
+intramolecular interactions, including stretching, bending, torsional, and
+combined bending-dihedral potentials. Additionally, topological reconstruction
+of permanent peptide chain backbone dipoles is possible for accurate recreation
+of protein conformational dynamics. It can run simulations in constant energy
+(NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [
+[4]](#4). HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for
+particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the
+[pfft-python bindings](github.com/rainwoodman/pfft-python). File IO is done via
+HDF5 formats to allow MPI parallel reads. If you use HyMD, [please cite our
+paper(s)](#citehead). ## User Guide Detailed installation and user guide,
+together with comprehensive example simulations are located in the [HylleraasMD
 documentation](https://cascella-group-uio.github.io/HyMD/index.html). Run
 simulations by ```bash python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--
 OPTIONAL_ARGS) ``` #### Run interactively in Google Colaboratory A [Google
 Colaboratory](https://colab.research.google.com/) jupyter notebook is setup
 [here](https://colab.research.google.com/drive/
 1jfzRaXjL3q53J4U8OrCgADepmf_HuCOh?usp=sharing) with a working HyMD fully
 installed and executable in the browser. ## Installation #### Non-Python
@@ -65,21 +68,39 @@
 O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/
 ideal_chain/ideal_chain.HDF5 /app$ /app$ # Run simulation /app$ python3 -m hymd
 ideal_chain.toml ideal_chain.HDF5 --verbose ``` ## Run tests Clone the
 repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd cd hymd
 python3 -m pip install pytest pytest-mpi pytest ``` Running MPI enabled pytest
 tests is simplified with a convenient script ```bash chmod +x pytest-mpi
-pytest-mpi -oo -n 2 -ns ``` ## Please cite our work If you use HyMD for your
-purposes, please cite the appropriate references from the section below. If you
-cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4).
---------- ### References [1] Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.;
-Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid
-Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv
-2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L.
-HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
-[3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid
-particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106. [4] Sen,
-S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing
-ParticleâField Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023 [5]
-Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM
-J. Sci. Comput. 2013, 35, C213âC236.
+pytest-mpi -oo -n 2 -ns ``` ## Contributions and issues We welcome
+contributions to our code and provide a set of guidelines to follow in
+[CONTRIBUTING.md](CONTRIBUTING.md). To seek support in case of any issues and
+bugs, we welcome you to post them using the [issue tracker](https://github.com/
+Cascella-Group-UiO/HyMD/issues). ## Please cite our work You will find
+information about our publications and archived data since 2023 at the open
+repository: [Publications](https://github.com/Cascella-Group-UiO/Publications).
+If you use HyMD, please cite: ```bibtex @article
+{ Ledum_HylleraasMD_Massively_parallel_2023, author = {Ledum, Morten and
+Carrer, Manuel and Sen, Samiran and Li, Xinmeng and Cascella, Michele and Bore,
+SigbjÃ¸rn LÃ¸land}, doi = {10.21105/joss.04149}, journal = {Journal of Open
+Source Software}, month = {apr}, number = {84}, pages = {4149}, title = {
+{HylleraasMD: Massively parallel hybrid particle-field molecular dynamics in
+Python}}, url = {https://joss.theoj.org/papers/10.21105/joss.04149}, volume =
+{8}, year = {2023} } @article{ Sen_HylleraasMD_2023, author = {Sen, Samiran and
+Ledum, Morten and Bore, SigbjÃ¸rn LÃ¸land and Cascella, Michele}, title = {Soft
+Matter under Pressure: Pushing ParticleâField Molecular Dynamics to the
+Isobaric Ensemble}, doi = {10.1021/acs.jcim.3c00186}, journal = {Journal of
+Chemical Information and Modeling}, month= mar, year = {2023}, volume = {63},
+number = {7}, pages = {2207-2217}, URL = {https://doi.org/10.1021/
+acs.jcim.3c00186}, } ``` --------- ### References [1] Ledum, M.; Sen, S.; Li,
+X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain
+Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations
+of Soft Matter. ChemRxiv 2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.;
+Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field
+molecular dynamics in Python. Journal of Open Source Software (JOSS) 2023, 8
+(84), 2475-9066, 4149. [3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free
+hybrid particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
+[4] Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure:
+Pushing ParticleâField Molecular Dynamics to the Isobaric Ensemble. J Chem
+Inf Model 2023, 63(7), 1549-9596. [5] Pippig, M. PFFT: An extension of FFTW to
+massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213âC236.
```

### Comparing `hymd-2.0.1/hymd.egg-info/SOURCES.txt` & `hymd-2.0.2/hymd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/setup.py` & `hymd-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,22 @@
         return version_match.group(1)
     raise RuntimeError("Version not found")
 
 
 with open('README.md', 'r') as in_file:
     readme = in_file.read()
 
+with open('requirements.txt', 'r') as f:
+    requirements = [
+        s for s in [
+            line.split('#', 1)[0].strip(' \t\n') for line in f
+        ] if s != ''
+    ]
+
+
 force_kernels = Extension(
     name="force_kernels",
     sources=[
         "hymd/compute_bond_forces.f90",
         "hymd/compute_bond_forces__double.f90",
         "hymd/compute_angle_forces.f90",
         "hymd/compute_angle_forces__double.f90",
@@ -39,29 +47,18 @@
     long_description_content_type="text/markdown",
     license="LGPLv3",
     packages=["hymd"],
     version=find_version("hymd/version.py"),
     ext_modules=[force_kernels],
     setup_requires=[
         "cython",
-        "numpy<1.24",
-        "mpi4py",
-    ],
-    install_requires=[
-        "cython",
-        "h5py",
+        "numpy",
         "mpi4py",
-        "mpsort",
-        "networkx",
-        "numpy<1.24",
-        "pfft-python",
-        "pmesh",
-        "sympy",
-        "tomli",
     ],
+    install_requires=requirements,
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",  # noqa: E501
         "Intended Audience :: Science/Research",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `hymd-2.0.1/test/test_configure_runtime.py` & `hymd-2.0.2/test/test_configure_runtime.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_distribute_input.py` & `hymd-2.0.2/test/test_distribute_input.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_field.py` & `hymd-2.0.2/test/test_field.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_file_io.py` & `hymd-2.0.2/test/test_file_io.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_force.py` & `hymd-2.0.2/test/test_force.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_hamiltonian.py` & `hymd-2.0.2/test/test_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_input_parser.py` & `hymd-2.0.2/test/test_input_parser.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_integrator.py` & `hymd-2.0.2/test/test_integrator.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_logger.py` & `hymd-2.0.2/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.1/test/test_thermostat.py` & `hymd-2.0.2/test/test_thermostat.py`

 * *Files identical despite different names*

