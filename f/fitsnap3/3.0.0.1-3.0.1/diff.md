# Comparing `tmp/fitsnap3-3.0.0.1.tar.gz` & `tmp/fitsnap3-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsnap3-3.0.0.1.tar", last modified: Tue Feb 28 06:44:32 2023, max compression
+gzip compressed data, was "fitsnap3-3.0.1.tar", last modified: Fri Apr 28 14:41:58 2023, max compression
```

## Comparing `fitsnap3-3.0.0.1.tar` & `fitsnap3-3.0.1.tar`

### file list

```diff
@@ -1,166 +1,168 @@
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.387994 fitsnap3-3.0.0.1/
--rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.0.0.1/LICENSE
--rw-rw-r--   0 drew      (1000) drew      (1000)    25080 2023-02-28 06:44:32.387994 fitsnap3-3.0.0.1/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     3944 2023-02-27 06:32:59.000000 fitsnap3-3.0.0.1/README.md
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.363994 fitsnap3-3.0.0.1/fitsnap3/
--rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1799 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3/__main__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3/fitsnap.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.363994 fitsnap3-3.0.0.1/fitsnap3.egg-info/
--rw-rw-r--   0 drew      (1000) drew      (1000)    25080 2023-02-28 06:44:32.000000 fitsnap3-3.0.0.1/fitsnap3.egg-info/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     5121 2023-02-28 06:44:32.000000 fitsnap3-3.0.0.1/fitsnap3.egg-info/SOURCES.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-02-28 06:44:32.000000 fitsnap3-3.0.0.1/fitsnap3.egg-info/dependency_links.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-02-28 06:44:32.000000 fitsnap3-3.0.0.1/fitsnap3.egg-info/requires.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-02-28 06:44:32.000000 fitsnap3-3.0.0.1/fitsnap3.egg-info/top_level.txt
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.363994 fitsnap3-3.0.0.1/fitsnap3lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.367994 fitsnap3-3.0.0.1/fitsnap3lib/calculators/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2060 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/basic_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    16381 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1191 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/calculator_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8511 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/lammps_base.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11651 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/lammps_custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    18273 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/lammps_pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    20142 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/lammps_snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      433 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/calculators/template_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6303 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/fitsnap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3670 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/initialize.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.367994 fitsnap3-3.0.0.1/fitsnap3lib/io/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/error.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6468 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/input.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      313 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.367994 fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1712 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      746 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/output_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8237 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/outputs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7139 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14169 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      263 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/template_output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.371994 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.371994 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7191 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      322 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7382 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2183 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1033 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      902 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/eshift.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1935 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/extras.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4832 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/groups.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      855 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/memory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1016 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/outfile.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      717 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/path.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1223 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/reference.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1607 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1975 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/section_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6731 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/sections.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.375994 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      804 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3152 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      475 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4578 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5629 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1837 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      364 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/template.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      960 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/io/sections/trainshift.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.375994 fitsnap3-3.0.0.1/fitsnap3lib/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.375994 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.375994 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/descriptors/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4747 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/pairwise.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6732 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/pas.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12044 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    16102 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/write.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.375994 fitsnap3-3.0.0.1/fitsnap3lib/lib/pace/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/pace/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13217 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/pace/pace.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.375994 fitsnap3-3.0.0.1/fitsnap3lib/lib/scalapack_solver/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/scalapack_solver/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3682 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/scalapack_solver/setup.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.379994 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4484 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.379994 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2527 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    16056 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/gen_labels.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      701 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/genlib.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.379994 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/lib/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11314 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13571 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11077 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10257 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/tree_method.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4681 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.379994 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3026 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2734 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11117 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1055 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12433 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/young.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      349 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/parallel_output.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    35098 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/parallel_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.379994 fitsnap3-3.0.0.1/fitsnap3lib/scrapers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/scrapers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3736 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/scrapers/json_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    17413 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/scrapers/scrape.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      759 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/scrapers/scraper_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      495 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/scrapers/template_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    26979 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/scrapers/vasp_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    18930 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/scrapers/xyz_scraper.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.383994 fitsnap3-3.0.0.1/fitsnap3lib/solvers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3083 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/anl.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3277 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10165 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/bcs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8565 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1534 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/lreg.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5292 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/mcmc.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4995 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/merr.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    34877 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2329 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/opt.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    39931 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2670 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    22614 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1047 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/solver_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1559 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/svd.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      388 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/template_solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1793 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/solvers/tensorflowsvd.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.383994 fitsnap3-3.0.0.1/fitsnap3lib/tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1027 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/tools/configuration.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/tools/dataframe_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8083 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/tools/dataloaders.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5688 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/tools/lammps_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8716 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/tools/nn_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6358 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/tools/test_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.387994 fitsnap3-3.0.0.1/fitsnap3lib/units/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1617 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/conversion_finder.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/energy.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/force.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/length.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/mass.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/pressure.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/temperature.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      273 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/time.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/fitsnap3lib/units/units.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1253 2023-02-28 06:43:16.000000 fitsnap3-3.0.0.1/pyproject.toml
--rw-rw-r--   0 drew      (1000) drew      (1000)       38 2023-02-28 06:44:32.387994 fitsnap3-3.0.0.1/setup.cfg
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-02-28 06:44:32.387994 fitsnap3-3.0.0.1/tests/
--rw-rw-r--   0 drew      (1000) drew      (1000)     3998 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/tests/test_examples.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13030 2023-02-27 06:33:02.000000 fitsnap3-3.0.0.1/tests/test_pytorch.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.458765 fitsnap3-3.0.1/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.0.1/LICENSE
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24953 2023-04-28 14:41:58.458765 fitsnap3-3.0.1/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3819 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/README.md
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.410764 fitsnap3-3.0.1/fitsnap3/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1799 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3/__main__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3/fitsnap.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.410764 fitsnap3-3.0.1/fitsnap3.egg-info/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24953 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5209 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/SOURCES.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/dependency_links.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/requires.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/top_level.txt
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.410764 fitsnap3-3.0.1/fitsnap3lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.418764 fitsnap3-3.0.1/fitsnap3lib/calculators/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2060 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/basic_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    16381 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1191 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/calculator_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8511 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_base.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    11541 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17979 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19992 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      433 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/template_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6496 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/fitsnap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3670 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/initialize.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.418764 fitsnap3-3.0.1/fitsnap3lib/io/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/error.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6468 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/input.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      313 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.422764 fitsnap3-3.0.1/fitsnap3lib/io/outputs/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1712 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      746 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/output_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8305 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/outputs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7156 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14246 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      263 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/template_output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.426764 fitsnap3-3.0.1/fitsnap3lib/io/sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.430765 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8204 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      322 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7382 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2183 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1033 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      902 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/eshift.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2267 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/extras.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4832 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/groups.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      855 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/memory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      996 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/outfile.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      717 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/path.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1223 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/reference.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1607 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2039 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/section_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6731 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/sections.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.430765 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1112 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3152 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      473 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4578 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5629 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      482 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1587 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      364 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/template.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      960 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/trainshift.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.430765 fitsnap3-3.0.1/fitsnap3lib/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.434764 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.434764 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pairwise.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pas.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12046 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/write.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.434764 fitsnap3-3.0.1/fitsnap3lib/lib/pace/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/pace/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13217 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/pace/pace.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.434764 fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/setup.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.438764 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.438764 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/gen_labels.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/genlib.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.438764 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/tree_method.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.442765 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/young.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      349 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/parallel_output.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    35256 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/parallel_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.442765 fitsnap3-3.0.1/fitsnap3lib/scrapers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4345 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/json_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17413 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/scrape.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      759 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/scraper_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/template_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    27314 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/vasp_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19146 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/xyz_scraper.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.450765 fitsnap3-3.0.1/fitsnap3lib/solvers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3082 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/anl.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3169 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10164 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/bcs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8565 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1786 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/lreg.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5291 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/mcmc.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4994 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/merr.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    39513 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2329 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/opt.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    42023 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2161 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3005 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24006 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1091 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/solver_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1559 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/svd.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      388 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/template_solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1793 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/tensorflowsvd.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.454765 fitsnap3-3.0.1/fitsnap3lib/tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/configuration.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/tools/dataframe_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/dataloaders.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/lammps_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/nn_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/test_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.454765 fitsnap3-3.0.1/fitsnap3lib/units/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/units/conversion_finder.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/energy.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/force.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/length.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/mass.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/pressure.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/temperature.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/units/time.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/units.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1092 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/pyproject.toml
+-rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-04-28 14:41:58.458765 fitsnap3-3.0.1/setup.cfg
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.458765 fitsnap3-3.0.1/tests/
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/tests/test_examples.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12841 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/tests/test_pytorch.py
```

### Comparing `fitsnap3-3.0.0.1/LICENSE` & `fitsnap3-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/PKG-INFO` & `fitsnap3-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.0.0.1
+Version: 3.0.1
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991 
         
@@ -374,57 +374,54 @@
 A Python package for machine learning potentials with [LAMMPS](https://github.com/lammps/lammps).
 
 **Documentation page:** [https://fitsnap.github.io](https://fitsnap.github.io)
 
 **Colab Python notebook tutorial:** [https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb](https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb)
 
 #### How to cite 
-We are currently working on an overview of the code in its current state, stay tuned!
+Rohskopf et al., (2023). FitSNAP: Atomistic machine learning with LAMMPS. Journal of Open Source Software, 8(84), 5118, https://doi.org/10.21105/joss.05118
 
 #### Dependencies:
 
-* This package expects Python 3.6+ 
-* Python dependencies: `numpy pandas scipy psutil tabulate`
+* This package expects Python 3.8+ 
+* Python dependencies: See `pyproject.toml`
 * [Compile LAMMPS as a shared library with python support](https://docs.lammps.org/Python_head.html). 
 If you can run `import lammps; lmp = lammps.lammps()` without errors in your Python interpreter, 
 you're good to go!
 * [Optional] To use neural network fitting functionality, install PyTorch with `pip install torch`. 
 * [Optional] For optimal performance, also install your favorite flavor of MPI (OpenMPI, MPICH) and 
 the Python package `mpi4py`. If installing mpi4py with a Python package manager, we recommend using 
 pip over conda as pip will auto-configure your package to your system's defaut MPI version 
 (usually what you used to build LAMMPS).
 * [Optional] For atomic cluster expansion (ACE) capabilities, build LAMMPS with the ML-PACE package, 
 along with the `compute_pace` files from [https://github.com/jmgoff/lammps-user-pace](https://github.com/jmgoff/lammps-user-pace)
 
 #### Quick install (minimal working environment) using Conda:
 
-WARNING: Conda LAMMPS installation does NOT include ACE, SPIN, or neural network functionality. See 
-the docs for details on how to install the current LAMMPS which has these functionalities.
+WARNING: Conda LAMMPS installation does NOT include ACE. See the docs for details on how to install the current LAMMPS which has these functionalities.
 
-* Clone this repository to get a FitSNAP directory:\
-    `git clone https://github.com/FitSNAP/FitSNAP`
-* Add `path/to/FitSNAP` path to your `PYTHONPATH` environment variable.
-* Add conda-forge to your Conda install, if not already added:\
+* Add conda-forge to your conda install, if not already added:\
     `conda config --add channels conda-forge` 
-* Create a new Conda environment:\
+* Create a new conda environment:\
     `conda create -n fitsnap python=3.9; conda activate fitsnap;`
 * Install the following packages:\
-    `conda install lammps psutil pandas tabulate sphinx sphinx_rtd_theme mpi4py`
-* Periodically `git pull` for code updates
+    `conda install -c conda-forge lammps fitsnap3`
 
 #### Running:
 
 * `(mpirun -np #) python -m fitsnap3 [options] infile`
 * Command line options can be seen with `python -m fitsnap3 -h`
 * Examples of published SNAP interatomic potentials are found in `examples/`
 * Examples of running FitSNAP via the library interface are found in `examples/library`
 
 #### Contributing:
 
 * See our [Programmer Guide](https://fitsnap.github.io/Executable.html) on how to add new features.
+* Abide by our code standards by installing `flake8` and running `flake8 --statistics` in the top 
+directory.
 * Get Sphinx with `pip install sphinx sphinx_rtd_theme` for adding new documentation, and see `docs/README.md` 
 for how to build docs for your features. 
 * **Feel free to ask for help!**
 
 #### About
 * Mitchell Wood and Aidan Thompson co-lead development of FitSNAP since 2016.
 * The FitSNAP Development Team is the set of all contributors to the FitSNAP project, including all subprojects.
```

### Comparing `fitsnap3-3.0.0.1/README.md` & `fitsnap3-3.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,57 +8,54 @@
 A Python package for machine learning potentials with [LAMMPS](https://github.com/lammps/lammps).
 
 **Documentation page:** [https://fitsnap.github.io](https://fitsnap.github.io)
 
 **Colab Python notebook tutorial:** [https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb](https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb)
 
 #### How to cite 
-We are currently working on an overview of the code in its current state, stay tuned!
+Rohskopf et al., (2023). FitSNAP: Atomistic machine learning with LAMMPS. Journal of Open Source Software, 8(84), 5118, https://doi.org/10.21105/joss.05118
 
 #### Dependencies:
 
-* This package expects Python 3.6+ 
-* Python dependencies: `numpy pandas scipy psutil tabulate`
+* This package expects Python 3.8+ 
+* Python dependencies: See `pyproject.toml`
 * [Compile LAMMPS as a shared library with python support](https://docs.lammps.org/Python_head.html). 
 If you can run `import lammps; lmp = lammps.lammps()` without errors in your Python interpreter, 
 you're good to go!
 * [Optional] To use neural network fitting functionality, install PyTorch with `pip install torch`. 
 * [Optional] For optimal performance, also install your favorite flavor of MPI (OpenMPI, MPICH) and 
 the Python package `mpi4py`. If installing mpi4py with a Python package manager, we recommend using 
 pip over conda as pip will auto-configure your package to your system's defaut MPI version 
 (usually what you used to build LAMMPS).
 * [Optional] For atomic cluster expansion (ACE) capabilities, build LAMMPS with the ML-PACE package, 
 along with the `compute_pace` files from [https://github.com/jmgoff/lammps-user-pace](https://github.com/jmgoff/lammps-user-pace)
 
 #### Quick install (minimal working environment) using Conda:
 
-WARNING: Conda LAMMPS installation does NOT include ACE, SPIN, or neural network functionality. See 
-the docs for details on how to install the current LAMMPS which has these functionalities.
+WARNING: Conda LAMMPS installation does NOT include ACE. See the docs for details on how to install the current LAMMPS which has these functionalities.
 
-* Clone this repository to get a FitSNAP directory:\
-    `git clone https://github.com/FitSNAP/FitSNAP`
-* Add `path/to/FitSNAP` path to your `PYTHONPATH` environment variable.
-* Add conda-forge to your Conda install, if not already added:\
+* Add conda-forge to your conda install, if not already added:\
     `conda config --add channels conda-forge` 
-* Create a new Conda environment:\
+* Create a new conda environment:\
     `conda create -n fitsnap python=3.9; conda activate fitsnap;`
 * Install the following packages:\
-    `conda install lammps psutil pandas tabulate sphinx sphinx_rtd_theme mpi4py`
-* Periodically `git pull` for code updates
+    `conda install -c conda-forge lammps fitsnap3`
 
 #### Running:
 
 * `(mpirun -np #) python -m fitsnap3 [options] infile`
 * Command line options can be seen with `python -m fitsnap3 -h`
 * Examples of published SNAP interatomic potentials are found in `examples/`
 * Examples of running FitSNAP via the library interface are found in `examples/library`
 
 #### Contributing:
 
 * See our [Programmer Guide](https://fitsnap.github.io/Executable.html) on how to add new features.
+* Abide by our code standards by installing `flake8` and running `flake8 --statistics` in the top 
+directory.
 * Get Sphinx with `pip install sphinx sphinx_rtd_theme` for adding new documentation, and see `docs/README.md` 
 for how to build docs for your features. 
 * **Feel free to ask for help!**
 
 #### About
 * Mitchell Wood and Aidan Thompson co-lead development of FitSNAP since 2016.
 * The FitSNAP Development Team is the set of all contributors to the FitSNAP project, including all subprojects.
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3/__main__.py` & `fitsnap3-3.0.1/fitsnap3/__main__.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3.egg-info/PKG-INFO` & `fitsnap3-3.0.1/fitsnap3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.0.0.1
+Version: 3.0.1
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991 
         
@@ -374,57 +374,54 @@
 A Python package for machine learning potentials with [LAMMPS](https://github.com/lammps/lammps).
 
 **Documentation page:** [https://fitsnap.github.io](https://fitsnap.github.io)
 
 **Colab Python notebook tutorial:** [https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb](https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb)
 
 #### How to cite 
-We are currently working on an overview of the code in its current state, stay tuned!
+Rohskopf et al., (2023). FitSNAP: Atomistic machine learning with LAMMPS. Journal of Open Source Software, 8(84), 5118, https://doi.org/10.21105/joss.05118
 
 #### Dependencies:
 
-* This package expects Python 3.6+ 
-* Python dependencies: `numpy pandas scipy psutil tabulate`
+* This package expects Python 3.8+ 
+* Python dependencies: See `pyproject.toml`
 * [Compile LAMMPS as a shared library with python support](https://docs.lammps.org/Python_head.html). 
 If you can run `import lammps; lmp = lammps.lammps()` without errors in your Python interpreter, 
 you're good to go!
 * [Optional] To use neural network fitting functionality, install PyTorch with `pip install torch`. 
 * [Optional] For optimal performance, also install your favorite flavor of MPI (OpenMPI, MPICH) and 
 the Python package `mpi4py`. If installing mpi4py with a Python package manager, we recommend using 
 pip over conda as pip will auto-configure your package to your system's defaut MPI version 
 (usually what you used to build LAMMPS).
 * [Optional] For atomic cluster expansion (ACE) capabilities, build LAMMPS with the ML-PACE package, 
 along with the `compute_pace` files from [https://github.com/jmgoff/lammps-user-pace](https://github.com/jmgoff/lammps-user-pace)
 
 #### Quick install (minimal working environment) using Conda:
 
-WARNING: Conda LAMMPS installation does NOT include ACE, SPIN, or neural network functionality. See 
-the docs for details on how to install the current LAMMPS which has these functionalities.
+WARNING: Conda LAMMPS installation does NOT include ACE. See the docs for details on how to install the current LAMMPS which has these functionalities.
 
-* Clone this repository to get a FitSNAP directory:\
-    `git clone https://github.com/FitSNAP/FitSNAP`
-* Add `path/to/FitSNAP` path to your `PYTHONPATH` environment variable.
-* Add conda-forge to your Conda install, if not already added:\
+* Add conda-forge to your conda install, if not already added:\
     `conda config --add channels conda-forge` 
-* Create a new Conda environment:\
+* Create a new conda environment:\
     `conda create -n fitsnap python=3.9; conda activate fitsnap;`
 * Install the following packages:\
-    `conda install lammps psutil pandas tabulate sphinx sphinx_rtd_theme mpi4py`
-* Periodically `git pull` for code updates
+    `conda install -c conda-forge lammps fitsnap3`
 
 #### Running:
 
 * `(mpirun -np #) python -m fitsnap3 [options] infile`
 * Command line options can be seen with `python -m fitsnap3 -h`
 * Examples of published SNAP interatomic potentials are found in `examples/`
 * Examples of running FitSNAP via the library interface are found in `examples/library`
 
 #### Contributing:
 
 * See our [Programmer Guide](https://fitsnap.github.io/Executable.html) on how to add new features.
+* Abide by our code standards by installing `flake8` and running `flake8 --statistics` in the top 
+directory.
 * Get Sphinx with `pip install sphinx sphinx_rtd_theme` for adding new documentation, and see `docs/README.md` 
 for how to build docs for your features. 
 * **Feel free to ask for help!**
 
 #### About
 * Mitchell Wood and Aidan Thompson co-lead development of FitSNAP since 2016.
 * The FitSNAP Development Team is the set of all contributors to the FitSNAP project, including all subprojects.
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3.egg-info/SOURCES.txt` & `fitsnap3-3.0.1/fitsnap3.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 fitsnap3/__init__.py
 fitsnap3/__main__.py
 fitsnap3/fitsnap.py
 fitsnap3.egg-info/PKG-INFO
 fitsnap3.egg-info/SOURCES.txt
 fitsnap3.egg-info/dependency_links.txt
 fitsnap3.egg-info/requires.txt
@@ -55,14 +56,15 @@
 fitsnap3lib/io/sections/calculator_sections/custom.py
 fitsnap3lib/io/sections/solver_sections/__init__.py
 fitsnap3lib/io/sections/solver_sections/ard.py
 fitsnap3lib/io/sections/solver_sections/jax.py
 fitsnap3lib/io/sections/solver_sections/lasso.py
 fitsnap3lib/io/sections/solver_sections/network.py
 fitsnap3lib/io/sections/solver_sections/pytorch.py
+fitsnap3lib/io/sections/solver_sections/ridge.py
 fitsnap3lib/io/sections/solver_sections/solver.py
 fitsnap3lib/lib/__init__.py
 fitsnap3lib/lib/neural_networks/__init__.py
 fitsnap3lib/lib/neural_networks/jax.py
 fitsnap3lib/lib/neural_networks/pairwise.py
 fitsnap3lib/lib/neural_networks/pas.py
 fitsnap3lib/lib/neural_networks/pytorch.py
@@ -109,14 +111,15 @@
 fitsnap3lib/solvers/lasso.py
 fitsnap3lib/solvers/lreg.py
 fitsnap3lib/solvers/mcmc.py
 fitsnap3lib/solvers/merr.py
 fitsnap3lib/solvers/network.py
 fitsnap3lib/solvers/opt.py
 fitsnap3lib/solvers/pytorch.py
+fitsnap3lib/solvers/ridge.py
 fitsnap3lib/solvers/scalapack.py
 fitsnap3lib/solvers/solver.py
 fitsnap3lib/solvers/solver_factory.py
 fitsnap3lib/solvers/svd.py
 fitsnap3lib/solvers/template_solver.py
 fitsnap3lib/solvers/tensorflowsvd.py
 fitsnap3lib/tools/__init__.py
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/calculators/basic_calculator.py` & `fitsnap3-3.0.1/fitsnap3lib/calculators/basic_calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/calculators/calculator.py` & `fitsnap3-3.0.1/fitsnap3lib/calculators/calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/calculators/calculator_factory.py` & `fitsnap3-3.0.1/fitsnap3lib/calculators/calculator_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/calculators/lammps_base.py` & `fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_base.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/calculators/lammps_custom.py` & `fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_custom.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,20 +123,23 @@
         # extract other quantities (no reference forces for this calculator yet!)
 
         ref_forces = np.zeros(3*num_atoms)
         ref_energy = 0
 
         # set indices for populating shared arrays
 
-        index = self.shared_index # Index telling where to start in the shared arrays on this proc.
-                                  # Currently this is an index for the 'a' array (natoms*nconfigs rows).
-                                  # This is also an index for the 't' array of types (natoms*nconfigs rows).
-                                  # Also made indices for:
-                                  # - the 'b' array (nconfigs rows)
-                                  # - the 'neighlist' array (natoms)*nneigh*nconfigs rows.
+        """
+        Index telling where to start in the shared arrays on this proc.
+        Currently this is an index for the 'a' array (natoms*nconfigs rows).
+        This is also an index for the 't' array of types (natoms*nconfigs rows).
+        Also made indices for:
+        - the 'b' array (nconfigs rows)
+        - the 'neighlist' array (natoms)*nneigh*nconfigs rows.
+        """
+        index = self.shared_index
         dindex = self.distributed_index
         index_b = self.shared_index_b
         index_c = self.shared_index_c
         index_neighlist = self.shared_index_neighlist
 
         # look up the neighbor list
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/calculators/lammps_pace.py` & `fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_pace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from fitsnap3lib.calculators.lammps_base import LammpsBase, _extract_compute_np, _extract_commands
+from fitsnap3lib.calculators.lammps_base import LammpsBase, _extract_compute_np
 from fitsnap3lib.parallel_tools import ParallelTools
-import ctypes
-from fitsnap3lib.calculators.calculator import Calculator
-from fitsnap3lib.parallel_tools import ParallelTools, DistributedList
 from fitsnap3lib.io.input import Config
 import numpy as np
 
 
 #config = Config()
 #pt = ParallelTools()
 
@@ -117,21 +114,24 @@
         # number of columns in the pace array, add 3 to include indices and Cartesian components.
 
         ncols = n_coeff + 3
         ncols_reference = 0
         nrows_dgrad = np.shape(lmp_pace)[0]-nrows_energy-1
         nrows_pace = nrows_energy + nrows_dgrad + 1
         assert nrows_pace == np.shape(lmp_pace)[0]
-        index = self.shared_index # Index telling where to start in the shared arrays on this proc.
-                                  # Currently this is an index for the 'a' array (natoms*nconfigs rows).
-                                  # This is also an index for the 't' array of types (natoms*nconfigs rows).
-                                  # Also made indices for:
-                                  # - the 'b' array (3*natoms+1)*nconfigs rows.
-                                  # - the 'dgrad' array (natoms+1)*nneigh*3*nconfigs rows.
-                                  # - the 'dgrad_indices' array which has same number of rows as 'dgrad'
+        """
+        Shared index tells where to start in the shared arrays on this proc.
+        Currently this is an index for the 'a' array (natoms*nconfigs rows).
+        This is also an index for the 't' array of types (natoms*nconfigs rows).
+        Also made indices for:
+        - the 'b' array (3*natoms+1)*nconfigs rows.
+        - the 'dgrad' array (natoms+1)*nneigh*3*nconfigs rows.
+        - the 'dgrad_indices' array which has same number of rows as 'dgrad'
+        """
+        index = self.shared_index
         dindex = self.distributed_index
         index_b = self.shared_index_b
         index_c = self.shared_index_c
         index_dgrad = self.shared_index_dgrad
 
         # extract the useful parts of the pace array
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/calculators/lammps_snap.py` & `fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_snap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fitsnap3lib.calculators.lammps_base import LammpsBase, _extract_compute_np
-from fitsnap3lib.parallel_tools import ParallelTools, DistributedList
+from fitsnap3lib.parallel_tools import ParallelTools
 from fitsnap3lib.io.input import Config
 import numpy as np
 
 
 #config = Config()
 #pt = ParallelTools()
 
@@ -138,21 +138,24 @@
         # number of columns in the snap array, add 3 to include indices and Cartesian components.
 
         ncols_snap = n_coeff + 3
         ncols_reference = 0
         nrows_dgrad = np.shape(lmp_snap)[0]-nrows_energy-1
         nrows_snap = nrows_energy + nrows_dgrad + 1
         assert nrows_snap == np.shape(lmp_snap)[0]
-        index = self.shared_index # Index telling where to start in the shared arrays on this proc.
-                                  # Currently this is an index for the 'a' array (natoms*nconfigs rows).
-                                  # This is also an index for the 't' array of types (natoms*nconfigs rows).
-                                  # Also made indices for:
-                                  # - the 'b' array (3*natoms+1)*nconfigs rows.
-                                  # - the 'dgrad' array (natoms+1)*nneigh*3*nconfigs rows.
-                                  # - the 'dgrad_indices' array which has same number of rows as 'dgrad'
+        """
+        Shared index tells where to start in the shared arrays on this proc.
+        Currently this is an index for the 'a' array (natoms*nconfigs rows).
+        This is also an index for the 't' array of types (natoms*nconfigs rows).
+        Also made indices for:
+        - the 'b' array (3*natoms+1)*nconfigs rows.
+        - the 'dgrad' array (natoms+1)*nneigh*3*nconfigs rows.
+        - the 'dgrad_indices' array which has same number of rows as 'dgrad'
+        """
+        index = self.shared_index
         dindex = self.distributed_index
         index_b = self.shared_index_b
         index_c = self.shared_index_c
         index_dgrad = self.shared_index_dgrad
 
         # extract the useful parts of the snap array
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/fitsnap.py` & `fitsnap3-3.0.1/fitsnap3lib/fitsnap.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,22 +59,25 @@
 
         self.scraper = scraper(self.config.sections["SCRAPER"].scraper)
         self.data = []
         self.calculator = calculator(self.config.sections["CALCULATOR"].calculator)
         self.solver = solver(self.config.sections["SOLVER"].solver)
         self.fit = None
         self.multinode = 0
-        self.delete_data = True # make False if don't want to delete data object
-                                # useful for using library to loop over fits
+        """
+        Make False if don't want to delete data object.
+        Useful for using library to loop over fits.
+        """
+        self.delete_data = True
         if self.config.sections["EXTRAS"].only_test:
             self.fit = output.read_fit()
 
         if (hasattr(self.pt, "lammps_version")):
-          if (self.config.sections['CALCULATOR'].nonlinear and (self.pt.lammps_version < 20220915) ):
-              raise Exception(f"Please upgrade LAMMPS to 2022-09-15 or later to use nonlinear solvers.")
+            if (self.config.sections['CALCULATOR'].nonlinear and (self.pt.lammps_version < 20220915) ):
+                raise Exception(f"Please upgrade LAMMPS to 2022-09-15 or later to use nonlinear solvers.")
        
     #@pt.single_timeit 
     def scrape_configs(self):
         """Scrapes configurations of atoms and creates a list of configurations called `data`."""
 
         @self.pt.single_timeit
         def decorated_scrape_configs():
@@ -135,14 +138,18 @@
                 else:
                     # Perform nonlinear fitting on 1 proc only
                     if(self.pt._rank==0):
                         self.solver.perform_fit()
             else:
                 self.solver.fit = self.fit
                 
+        # If not performing a fit, keep in mind that the `configs` list is None 
+        # for nonlinear models. Keep this in mind when performing error 
+        # analysis.
+        
         @self.pt.single_timeit
         def fit_gather():
             self.solver.fit_gather()
         @self.pt.single_timeit
         def error_analysis():
             self.solver.error_analysis()
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/initialize.py` & `fitsnap3-3.0.1/fitsnap3lib/initialize.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/input.py` & `fitsnap3-3.0.1/fitsnap3lib/io/input.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/custom.py` & `fitsnap3-3.0.1/fitsnap3lib/io/outputs/custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/output_factory.py` & `fitsnap3-3.0.1/fitsnap3lib/io/outputs/output_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/outputs.py` & `fitsnap3-3.0.1/fitsnap3lib/io/outputs/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,17 @@
                 function = errors.to_pickle
                 write_type = 'wb'
             else:
                 raise NotImplementedError("Metric style {} not implemented".format(
                     self.config.sections["OUTFILE"].metrics_style))
             with optional_open(fname, write_type) as file:
                 function(file, **arguments)
-        decorated_write_errors()
+
+        if not self.config.sections["SOLVER"].true_multinode: 
+            decorated_write_errors()
 
     def write_errors_nn(self, errors):
         """ 
         Write errors for nonlinear fits. 
         
         Args:
             errors : sequence of dictionaries (mae_f, mae_e, rmse_e, rmse_f, count_train, count_test)
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/pace.py` & `fitsnap3-3.0.1/fitsnap3lib/io/outputs/pace.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 drcinnervals = self.drcinner
             if len(self.lmbda) > 1:
                 lmbdavals = {bondstr:lmb for bondstr,lmb in zip(bondstrs,self.lmbda)}
                 rcvals = {bondstr:lmb for bondstr,lmb in zip(bondstrs,self.rcutfac)}
                 rcinnervals = {bondstr:lmb for bondstr,lmb in zip(bondstrs,self.rcinner)}
                 drcinnervals = {bondstr:lmb for bondstr,lmb in zip(bondstrs,self.drcinner)}
 
-            apot = AcePot(self.types, reference_ens, [int(k) for k in self.ranks], [int(k) for k in self.nmax],  [int(k) for k in self.lmax], self.nmaxbase, rcvals, lmbdavals, rcinnervals, drcinnervals, self.lmin, self.RPI_heuristic)
+            apot = AcePot(self.types, reference_ens, [int(k) for k in self.ranks], [int(k) for k in self.nmax],  [int(k) for k in self.lmax], self.nmaxbase, rcvals, lmbdavals, rcinnervals, drcinnervals, [int(k) for k in self.lmin], self.RPI_heuristic)
             apot.set_betas(coeffs,has_zeros=True)
             apot.set_funcs()
             apot.write_pot(self.config.sections["OUTFILE"].potential_name)
             # Append metadata to .yace file
             unit = f"# units {self.config.sections['REFERENCE'].units}\n"
             atom = f"# atom_style {self.config.sections['REFERENCE'].atom_style}\n"
             pair = "\n".join(["# " + s for s in self.config.sections["REFERENCE"].lmp_pairdecl]) + "\n"
@@ -131,15 +131,14 @@
 
 def _to_coeff_string(coeffs):
     """
     Convert a set of coefficients along with bispec options into a .snapparam file
     """
     config = Config()
     desc_str = "ACE"
-
     coeffs = coeffs.reshape((config.sections[desc_str].numtypes, -1))
     blank2Js = config.sections[desc_str].blank2J.reshape((config.sections[desc_str].numtypes, -1))
     if config.sections[desc_str].bzeroflag:
         blank2Js = np.insert(blank2Js, 0, [1.0], axis=1)
     coeffs = np.multiply(coeffs, blank2Js)
     coeff_names = [[0]]+config.sections[desc_str].blist
     type_names = config.sections[desc_str].types
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/outputs/snap.py` & `fitsnap3-3.0.1/fitsnap3lib/io/outputs/snap.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
     out += f"rfac0 {config.sections['BISPECTRUM'].rfac0}\n"
     out += f"rmin0 {config.sections['BISPECTRUM'].rmin0}\n"
     out += f"bzeroflag {config.sections['BISPECTRUM'].bzeroflag}\n"
     out += f"wselfallflag {config.sections['BISPECTRUM'].wselfallflag}\n"
     out += f"chemflag {chemflag_int}\n"
     out += f"bnormflag {config.sections['BISPECTRUM'].bnormflag}\n"
     out += f"switchinnerflag {config.sections['BISPECTRUM'].switchinnerflag}\n"
+    out += f"quadraticflag {config.sections['BISPECTRUM'].quadraticflag}\n"
     if config.sections["BISPECTRUM"].switchinnerflag:
         out += f"sinner {config.sections['BISPECTRUM'].sinner}\n"
         out += f"dinner {config.sections['BISPECTRUM'].dinner}\n"
     out += "\n"
     out += "# This file was generated by FitSNAP.\n"
     out += f"# Hash: {config.hash}\n"
     out += "# FitSNAP REFERENCE section settings:\n"
@@ -329,8 +330,8 @@
     else:
         out += f"pair_style mliap model mliappy FitTorch_Pytorch.pt descriptor sna {snap_filename}.mliap.descriptor\n"
         pc_snap = f"pair_coeff * *"
         for t in config.sections["BISPECTRUM"].types:
             pc_snap += f" {t}"
         out += pc_snap
 
-    return out
+    return out
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,21 +20,21 @@
                           'bikflag', 'dgradflag']
             for value_name in config['ACE']:
                 if value_name in allowedkeys: continue
                 else:
                     raise RuntimeError(">>> Found unmatched variable in ACE section of input: ",value_name)
             self.numtypes = self.get_value("ACE", "numTypes", "1", "int")
             self.ranks = self.get_value("ACE","ranks","3").split()
-            self.lmin = self.get_value("ACE", "lmin", "1", "int")
+            self.lmin = self.get_value("ACE", "lmin", "0").split() 
             self.lmax = self.get_value("ACE", "lmax", "2").split()
             self.nmax = self.get_value("ACE", "nmax", "2").split() 
             self.mumax = self.get_value("ACE","mumax", "1")
             self.nmaxbase = self.get_value("ACE", "nmaxbase", "16","int")
-            self.rcutfac = self.get_value("ACE", "rcutfac", "7.5").split()
-            self.lmbda = self.get_value("ACE","lambda",'5.0').split()
+            self.rcutfac = self.get_value("ACE", "rcutfac", "4.5").split()
+            self.lmbda = self.get_value("ACE","lambda",'1.35').split()
             self.rcinner = self.get_value("ACE","rcinner",'0.0').split()
             self.drcinner = self.get_value("ACE","drcinner",'0.01').split()
             self.types = self.get_value("ACE", "type", "H").split()
             self.erefs = self.get_value("ACE", "erefs", "0.0").split() 
             self.bikflag = self.get_value("ACE", "bikflag", "0", "bool")
             self.dgradflag = self.get_value("ACE", "dgradflag", "0", "bool")
             self.RPI_heuristic = self.get_value("ACE" , "RPI_heuristic" , 'root_SO3_span')
@@ -43,31 +43,43 @@
                 self.type_mapping[atom_type] = i+1
 
             self.bzeroflag = self.get_value("ACE", "bzeroflag", "0", "bool")
             self.wigner_flag = self.get_value("ACE", "wigner_flag", "1", "bool")
 
             if self.bikflag:
                 self._assert_dependency('bikflag', "CALCULATOR", "per_atom_energy", True)
-
+            self.lmax_dct = {int(rnk):int(lmx) for rnk,lmx in zip(self.ranks,self.lmax)}
             self.pt = ParallelTools()
+            if self.RPI_heuristic != 'root_SO3_span':
+                self.pt.single_print('WARNING: do not change RPI flags unless you know what you are doing!')
             self._generate_b_list()
             self._write_couple()
             Section.num_desc = len(self.blist)
             self.delete()
 
         def _generate_b_list(self):
             self.blist = []
             self.blank2J = []
             prefac = 1.0
             i = 0
 
             if self.RPI_heuristic == 'lexicographic':
                 ranked_chem_nus = [generate_nl(int(rnk), int(self.nmax[ind]), int(self.lmax[ind]), int(self.mumax)) for ind,rnk in enumerate(self.ranks)]
             else:
-                ranked_chem_nus = [descriptor_labels_YSG(int(rnk), int(self.nmax[ind]), int(self.lmax[ind]), int(self.mumax),lmin = self.lmin ) for ind,rnk in enumerate(self.ranks)]
+                if type(self.lmin) == list:
+                    if len(self.lmin) == 1:
+                        self.lmin = self.lmin * len(self.ranks)
+                    ranked_chem_nus = [descriptor_labels_YSG(int(rnk), int(self.nmax[ind]), int(self.lmax[ind]), int(self.mumax),lmin = int(self.lmin[ind]) ) for ind,rnk in enumerate(self.ranks)]
+                else:
+                    ranked_chem_nus = [descriptor_labels_YSG(int(rnk), int(self.nmax[ind]), int(self.lmax[ind]), int(self.mumax),lmin = int(self.lmin) ) for ind,rnk in enumerate(self.ranks)]
+
+            highranks = [int(r) for r in self.ranks if int(r) >= 4]
+            warnflag = any([ self.lmax_dct[rank] >= 3 for ind,rank in enumerate(highranks)])
+            if warnflag:
+                self.pt.single_print('WARNING: lmax of %d will generate descriptors that cannot be entered into LAMMPS_PACE - try a lower lmax for ranks >= 4' % warnflag[0])
             nus_unsort = [item for sublist in ranked_chem_nus for item in sublist]
             nus = nus_unsort.copy()
             mu0s = []
             mus =[]
             ns = []
             ls = []
             for nu in nus_unsort:
@@ -123,19 +135,19 @@
             if len(self.lmbda) > 1:
                 lmbdavals = {bondstr:lmb for bondstr,lmb in zip(bondstrs,self.lmbda)}
                 rcvals = {bondstr:lmb for bondstr,lmb in zip(bondstrs,self.rcutfac)}
                 rcinnervals = {bondstr:lmb for bondstr,lmb in zip(bondstrs,self.rcinner)}
                 drcinnervals = {bondstr:lmb for bondstr,lmb in zip(bondstrs,self.drcinner)}
                     
 
-            apot = AcePot(self.types, reference_ens, [int(k) for k in self.ranks], [int(k) for k in self.nmax],  [int(k) for k in self.lmax], self.nmaxbase, rcvals, lmbdavals, rcinnervals, drcinnervals, self.lmin, self.RPI_heuristic)
+            apot = AcePot(self.types, reference_ens, [int(k) for k in self.ranks], [int(k) for k in self.nmax],  [int(k) for k in self.lmax], self.nmaxbase, rcvals, lmbdavals, rcinnervals, drcinnervals, [int(k) for k in self.lmin], self.RPI_heuristic)
             apot.write_pot('coupling_coefficients')
 
 except ModuleNotFoundError:
 
     class Ace(Section):
         """
         Dummy class for factory to read if torch is not available for import.
         """
         def __init__(self, name, config, args):
             super().__init__(name, config, args)
-            raise ModuleNotFoundError("Missing sympy or pyyaml modules.")
+            raise ModuleNotFoundError("Missing sympy or pyyaml modules.")
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/eshift.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/eshift.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/extras.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/extras.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,36 +5,43 @@
 pt = ParallelTools()
 
 
 class Extras(Section):
 
     def __init__(self, name, config, args):
         super().__init__(name, config, args)
-        self.allowedkeys = ['multinode_testing', 'apply_transpose', 'only_test', 'dump_descriptors', 'dump_truth',
-                            'dump_weights', 'dump_dataframe', 'dump_peratom', 'dump_perconfig']
+        self.allowedkeys = ['multinode_testing', 'apply_transpose', 'only_test', \
+                            'dump_descriptors', 'dump_truth', 'dump_weights', 'dump_dataframe', \
+                            'dump_peratom', 'dump_perconfig', 'dump_configs']
         self._check_section()
 
+        # Set EXTRAS section file dump flags.
+
         self.multinode_testing = self.get_value("EXTRAS", "multinode_testing", "0", "bool")
         self.apply_transpose = self.get_value("EXTRAS", "apply_transpose", "0", "bool")
         self.only_test = self.get_value("EXTRAS", "only_test", "0", "bool")
         self.dump_a = self.get_value("EXTRAS", "dump_descriptors", "0", "bool")
         self.dump_b = self.get_value("EXTRAS", "dump_truth", "0", "bool")
         self.dump_w = self.get_value("EXTRAS", "dump_weights", "0", "bool")
         self.dump_dataframe = self.get_value("EXTRAS", "dump_dataframe", "0", "bool")
         self.dump_peratom = self.get_value("EXTRAS", "dump_peratom", "0", "bool")
         self.dump_perconfig = self.get_value("EXTRAS", "dump_perconfig", "0", "bool")
+        self.dump_configs = self.get_value("EXTRAS", "dump_configs", "0", "bool")
 
+        # Set OUTFILE section filenames.
 
         self.descriptor_file = \
             self.check_path(self.get_value("OUTFILE", "descriptors", "Descriptors.npy"))
         self.truth_file = \
             self.check_path(self.get_value("OUTFILE", "truth", "Truth-Ref.npy"))
         self.weights_file = \
             self.check_path(self.get_value("OUTFILE", "weights", "Weights.npy"))
         self.dataframe_file = \
             self.check_path(self.get_value("OUTFILE", "dataframe", "FitSNAP.df"))
         self.peratom_file = \
             self.check_path(self.get_value("OUTFILE", "peratom", "peratom.dat"))
         self.perconfig_file = \
             self.check_path(self.get_value("OUTFILE", "perconfig", "perconfig.dat"))
+        self.configs_file = \
+            self.check_path(self.get_value("OUTFILE", "configs", "configs.pickle"))
 
         self.delete()
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/groups.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/groups.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/memory.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/memory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/outfile.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/outfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from os import path
 from fitsnap3lib.io.sections.sections import Section
 from fitsnap3lib.parallel_tools import ParallelTools
-from os import path
 
 
 #pt = ParallelTools()
 
 
 class Outfile(Section):
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/path.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/path.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/reference.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/reference.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/scraper.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/section_factory.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/section_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from fitsnap3lib.io.sections.outfile import Outfile
 from fitsnap3lib.io.sections.path import Path
 from fitsnap3lib.io.sections.reference import Reference
 from fitsnap3lib.io.sections.scraper import Scraper
 from fitsnap3lib.io.sections.solver_sections.solver import Solver
 from fitsnap3lib.io.sections.solver_sections.ard import Ard
 from fitsnap3lib.io.sections.solver_sections.lasso import Lasso
+from fitsnap3lib.io.sections.solver_sections.ridge import Ridge
 from fitsnap3lib.io.sections.solver_sections.jax import JAX
 from fitsnap3lib.io.sections.solver_sections.pytorch import PYTORCH
 from fitsnap3lib.io.sections.solver_sections.network import NETWORK
 from fitsnap3lib.io.sections.template import Default
 
 
 pt = ParallelTools()
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/sections.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/sections.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/jax.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/network.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/network.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/io/sections/trainshift.py` & `fitsnap3-3.0.1/fitsnap3lib/io/sections/trainshift.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,13 +99,13 @@
             c = self.cutoff
             function = 0.5 + 0.5*torch.cos(self.pi*(rij-0)/(c-0))
 
             return function[:,0]
             
 except ModuleNotFoundError:
 
-    class Bessel():
+    class Gaussian3Body():
         """
         Dummy class for factory to read if torch is not available for import.
         """
         def __init__(self):
             raise ModuleNotFoundError("No module named 'torch'")
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/jax.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/pairwise.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pairwise.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/pas.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pas.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 It's similar to the basic pytorch.py used for fitting energies/forces, but convenient to separate 
 into a separate file because there are many differences in the forward pass.
 
 We use the `create_networks` function in pytorch.py since the structure is the same.
 """
 
 import torch
-from torch import from_numpy
-from torch.nn import Parameter
+
 """
 Try to import mliap package after: https://github.com/lammps/lammps/pull/3388
 See related bug: https://github.com/lammps/lammps/issues/3204
 For now we only use the following two MLIAP features for writing LAMMPS-ready pytorch models.
 """
 
 class FitTorchPAS(torch.nn.Module):
@@ -82,15 +81,15 @@
             #                                 for i in range(self.n_elem)])[types,atom_indices]
 
             # Slightly slower, but more general
 
             per_atom_scalars = torch.zeros(types.size(dim=0), dtype=dtype).to(device)
             given_elems, elem_indices = torch.unique(types, return_inverse=True)
             for i, elem in enumerate(given_elems): 
-              per_atom_scalars[elem_indices == i] = self.networks[elem](x[elem_indices == i]).flatten()
+                per_atom_scalars[elem_indices == i] = self.networks[elem](x[elem_indices == i]).flatten()
 
         return per_atom_scalars
 
     def import_wb(self, weights, bias):
         """
         Imports weights and bias into FitTorch model
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/pytorch.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             #                                 for i in range(self.n_elem)])[types,atom_indices]
 
             # Slightly slower, but more general
 
             per_atom_energies = torch.zeros(types.size(dim=0), dtype=dtype).to(device)
             given_elems, elem_indices = torch.unique(types, return_inverse=True)
             for i, elem in enumerate(given_elems):
-              per_atom_energies[elem_indices == i] = self.networks[elem](x[elem_indices == i]).flatten()
+                per_atom_energies[elem_indices == i] = self.networks[elem](x[elem_indices == i]).flatten()
 
         # calculate energies
 
         if (self.energy_bool):
             predicted_energy_total = torch.zeros(atoms_per_structure.size(), dtype=dtype).to(device)
             predicted_energy_total.index_add_(0, indices, per_atom_energies.squeeze())
         else:
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/neural_networks/write.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,18 +370,18 @@
         tag_j = torch.from_numpy(tag_j).to(dtype=torch.long, device=self.device) #.requires_grad_(True)
 
         #print(unique_i)
         #print(tag_i)
         #print(unique_j)
         #print(tag_j)
 
-        diff_norm = torch.nn.functional.normalize(rij, dim=1) # need for g3b
-                                                              # size (npairs, 3)
-        distance_ij = torch.linalg.norm(rij, dim=1).unsqueeze(1)  # need for cutoff and various other functions
-                                                                  # size (npairs, 1)
+        # need for g3b, size (npairs, 3)
+        diff_norm = torch.nn.functional.normalize(rij, dim=1)
+        # need for cutoff and various other functions, size (npairs, 1)
+        distance_ij = torch.linalg.norm(rij, dim=1).unsqueeze(1)
 
         #print(distance_ij)
 
         # max pairwise distance is good for debugging match with fitting code
         #maxr = torch.max(distance_ij)
         #print(f"Max pairwise distance: {maxr}")
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/pace/pace.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/pace/pace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/scalapack_solver/setup.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,21 +61,24 @@
 
 if mpiversion == 'openmpi':
     # Fetch the arguments for linking and compiling.
     mpilinkargs = runcommand('mpicc -showme:link').split()
     mpicompileargs = runcommand('mpicc -showme:compile').split()
 
 if scalapackversion == 'intelmkl':
-    # Set library includes (taking into account which MPI library we are using)."
-    scl_lib = ['mkl_scalapack_ilp64', 'mkl_intel_ilp64', 'mkl_intel_thread', 'mkl_core',
-               'mkl_blacs_'+mpiversion+'_ilp64', 'iomp5', 'pthread', 'mkl_avx512', 'mkl_def']
+    # Set library includes taking into account which MPI library we are using.
+    # Includes for specific machines are suggested by the Intel MKL link advisor online tool.
+    # For example if using Intel compilers instead of GNU, one might switch
+    # `mkl_gnu_thread` to `mkl_intel_thread` and `gomp` to `iomp5`.
+    scl_lib = ['mkl_scalapack_ilp64', 'mkl_intel_ilp64', 'mkl_gnu_thread', 'mkl_core',
+               'mkl_blacs_'+mpiversion+'_ilp64', 'gomp', 'pthread', 'mkl_avx512', 'mkl_def',
+               'm', 'dl']
     scl_incl = os.environ['MKLROOT']+'/include'
-    # scl_lib = ['mkl_blacs_'+mpiversion+'_lp64', 'iomp5', 'pthread']
-    scl_libdir = [os.environ['MKLROOT']+'/lib' if 'MKLROOT' in os.environ else '']
-    # scl_libdir = ['/Users/casieve/anaconda3/lib']
+    # The library directory also comes from the Intel MKL link advisor online tool.
+    scl_libdir = [os.environ['MKLROOT']+'/lib/intel64' if 'MKLROOT' in os.environ else '']
 elif scalapackversion == 'netlib':
     scl_lib = ['scalapack', 'gfortran']
     scl_libdir = [ os.path.dirname(runcommand('gfortran -print-file-name=libgfortran.a')) ]
 else:
     raise Exception("Scalapack distribution unsupported. Please modify setup.py manually.")
 
 
@@ -83,18 +86,16 @@
                          'scalapack_funcs',
                          # source file:
                          sources=['scalapack.pyx'],
                          # Needed if building with NumPy. This includes the NumPy headers when compiling.
                          include_dirs=[get_include(), mpi4py.get_include(), scl_incl],
                          #include libraries 
                          library_dirs=scl_libdir, libraries=scl_lib,
-                         #libraries=["scalapack"],
-                         #library_dirs=[library_dirs],
                          # other compile args for gcc
                          extra_compile_args=["-DMKL_ILP64", "-m64"],
                          # other files to link to
                          extra_link_args=["-lm", "-ldl"] + mpilinkargs)]
 
-setup(
-      cmdclass = {'build_ext': build_ext},
-      ext_modules = ext_modules
+setup (
+          cmdclass = {'build_ext': build_ext},
+          ext_modules = ext_modules
       )
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,129 @@
 from scipy import special
 import pickle
 import numpy as np
 from fitsnap3lib.lib.sym_ACE.sym_ACE_settings import *
 
 
 def Clebsch_gordan(j1,m1,j2,m2,j3,m3):
-	# Clebsch-gordan coefficient calculator based on eqs. 4-5 of:
-	# https://hal.inria.fr/hal-01851097/document
-	# and christoph ortner's julia code ACE.jl
-
-	#VERIFIED: test non-zero indices in Wolfram using format ClebschGordan[{j1,m1},{j2,m2},{j3,m3}]
-	#rules:
-	rule1 = np.abs(j1-j2) <= j3
-	rule2 = j3 <= j1+j2
-	rule3 = m3 == m1 + m2
-	rule4 = np.abs(m3) <= j3
-
-	#rules assumed by input
-	#assert np.abs(m1) <= j1, 'm1 must be \in {-j1,j1}'
-	#assert np.abs(m2) <= j2, 'm2 must be \in {-j2,j2}'
-
-	if rule1 and rule2 and rule3 and rule4:
-		#attempting binomial representation
-		N1 = np.longdouble((2*j3) + 1 )
-		N2 =  np.longdouble(special.factorial(j1 + m1, exact=True)) \
-		* np.longdouble(special.factorial(j1 - m1, exact=True)) \
-		* np.longdouble(special.factorial(j2 + m2, exact=True)) \
-		* np.longdouble(special.factorial(j2 - m2, exact=True)) \
-		* np.longdouble(special.factorial(j3 + m3, exact=True)) \
-		* np.longdouble(special.factorial(j3 - m3, exact=True))
-
-		N3 = np.longdouble(special.factorial(j1 + j2 - j3, exact=True)) \
-		* np.longdouble(special.factorial(j1 - j2 + j3, exact=True)) \
-		* np.longdouble(special.factorial(-j1 + j2 + j3, exact=True)) \
-		* np.longdouble(special.factorial(j1 + j2 + j3 + 1, exact=True))
-
-		#N = np.longdouble((N1*N2))/np.longdouble((N3))
-		N = np.longdouble(0.)
-		N += np.divide((N1*N2),N3)
-
-		G = np.longdouble(0.0)
-
-		#k conditions (see eq.5 of https://hal.inria.fr/hal-01851097/document)
-		# k  >= 0
-		# k <= j1 - m1
-		# k <= j2 + m2
-
-		for k in range(0, min([j1-m1, j2+m2]) + 1  ):
-			G1 = np.longdouble((-1)**k)
-			G2 = np.longdouble(special.comb(j1 + j2 - j3, k,exact=True))
-			G3 = np.longdouble(special.comb(j1 - j2 + j3, j1 - m1 - k,exact=True))
-			G4 = np.longdouble(special.comb(-j1 +j2 + j3, j2 + m2 - k,exact=True))
-			G += np.longdouble(G1*G2*G3*G4)
-		Nsqrt = np.longdouble(0)
-		Nsqrt += np.sqrt(N)
-		return np.float32(Nsqrt*G)
+    # Clebsch-gordan coefficient calculator based on eqs. 4-5 of:
+    # https://hal.inria.fr/hal-01851097/document
+    # and christoph ortner's julia code ACE.jl
+
+    #VERIFIED: test non-zero indices in Wolfram using format ClebschGordan[{j1,m1},{j2,m2},{j3,m3}]
+    #rules:
+    rule1 = np.abs(j1-j2) <= j3
+    rule2 = j3 <= j1+j2
+    rule3 = m3 == m1 + m2
+    rule4 = np.abs(m3) <= j3
+
+    #rules assumed by input
+    #assert np.abs(m1) <= j1, 'm1 must be \in {-j1,j1}'
+    #assert np.abs(m2) <= j2, 'm2 must be \in {-j2,j2}'
+
+    if rule1 and rule2 and rule3 and rule4:
+        #attempting binomial representation
+        N1 = np.longdouble((2*j3) + 1 )
+        N2 =  np.longdouble(special.factorial(j1 + m1, exact=True)) \
+        * np.longdouble(special.factorial(j1 - m1, exact=True)) \
+        * np.longdouble(special.factorial(j2 + m2, exact=True)) \
+        * np.longdouble(special.factorial(j2 - m2, exact=True)) \
+        * np.longdouble(special.factorial(j3 + m3, exact=True)) \
+        * np.longdouble(special.factorial(j3 - m3, exact=True))
+
+        N3 = np.longdouble(special.factorial(j1 + j2 - j3, exact=True)) \
+        * np.longdouble(special.factorial(j1 - j2 + j3, exact=True)) \
+        * np.longdouble(special.factorial(-j1 + j2 + j3, exact=True)) \
+        * np.longdouble(special.factorial(j1 + j2 + j3 + 1, exact=True))
+
+        #N = np.longdouble((N1*N2))/np.longdouble((N3))
+        N = np.longdouble(0.)
+        N += np.divide((N1*N2),N3)
+
+        G = np.longdouble(0.0)
+
+        #k conditions (see eq.5 of https://hal.inria.fr/hal-01851097/document)
+        # k  >= 0
+        # k <= j1 - m1
+        # k <= j2 + m2
+
+        for k in range(0, min([j1-m1, j2+m2]) + 1  ):
+            G1 = np.longdouble((-1)**k)
+            G2 = np.longdouble(special.comb(j1 + j2 - j3, k,exact=True))
+            G3 = np.longdouble(special.comb(j1 - j2 + j3, j1 - m1 - k,exact=True))
+            G4 = np.longdouble(special.comb(-j1 +j2 + j3, j2 + m2 - k,exact=True))
+            G += np.longdouble(G1*G2*G3*G4)
+        Nsqrt = np.longdouble(0)
+        Nsqrt += np.sqrt(N)
+        return np.float32(Nsqrt*G)
 
-	else:
-		return 0.
+    else:
+        return 0.
 
 def clebsch_gordan(l1,m1,l2,m2,l3,m3):
-	# try to load c library for calculating cg coefficients
-	if cglib:
-		return lib.Clebsch_Gordan(l1,m1,l2,m2,l3,m3)
-	else:
-		return Clebsch_gordan(l1,m1,l2,m2,l3,m3)
+    # try to load c library for calculating cg coefficients
+    if cglib:
+        return lib.Clebsch_Gordan(l1,m1,l2,m2,l3,m3)
+    else:
+        return Clebsch_gordan(l1,m1,l2,m2,l3,m3)
 
 def wigner_3j(j1,m1,j2,m2,j3,m3):
-	# uses relation between Clebsch-Gordann coefficients and W-3j symbols to evaluate W-3j
-	#VERIFIED - wolframalpha.com
-	cg = clebsch_gordan(j1,m1,j2,m2,j3,-m3)
+    # uses relation between Clebsch-Gordann coefficients and W-3j symbols to evaluate W-3j
+    #VERIFIED - wolframalpha.com
+    cg = clebsch_gordan(j1,m1,j2,m2,j3,-m3)
 
-	num = np.longdouble((-1)**(j1-j2-m3))
-	denom = np.longdouble(((2*j3) +1)**(1/2))
+    num = np.longdouble((-1)**(j1-j2-m3))
+    denom = np.longdouble(((2*j3) +1)**(1/2))
 
-	return np.float32(cg*np.longdouble(num/denom))
+    return np.float32(cg*np.longdouble(num/denom))
 
 
 def init_clebsch_gordan(lmax):
-	#returns dictionary of all cg coefficients to be used at a given value of lmax
-	cg = {}
-	for l1 in range(lmax+1):
-		for l2 in range(lmax+1):
-			for l3 in range(lmax+1):
-				for m1 in range(-l1,l1+1):
-					for m2 in range(-l2,l2+1):
-						for m3 in range(-l3,l3+1):
-							key = '%d,%d,%d,%d,%d,%d' % (l1,m1,l2,m2,l3,m3)
-							cg[key] = clebsch_gordan(l1,m1,l2,m2,l3,m3)
-	return cg
+    #returns dictionary of all cg coefficients to be used at a given value of lmax
+    cg = {}
+    for l1 in range(lmax+1):
+        for l2 in range(lmax+1):
+            for l3 in range(lmax+1):
+                for m1 in range(-l1,l1+1):
+                    for m2 in range(-l2,l2+1):
+                        for m3 in range(-l3,l3+1):
+                            key = '%d,%d,%d,%d,%d,%d' % (l1,m1,l2,m2,l3,m3)
+                            cg[key] = clebsch_gordan(l1,m1,l2,m2,l3,m3)
+    return cg
 
 
 def init_wigner_3j(lmax):
-	#returns dictionary of all cg coefficients to be used at a given value of lmax
-	cg = {}
-	for l1 in range(lmax+1):
-		for l2 in range(lmax+1):
-			for l3 in range(lmax+1):
-				for m1 in range(-l1,l1+1):
-					for m2 in range(-l2,l2+1):
-						for m3 in range(-l3,l3+1):
-							key = '%d,%d,%d,%d,%d,%d' % (l1,m1,l2,m2,l3,m3)
-							cg[key] = wigner_3j(l1,m1,l2,m2,l3,m3)
-	return cg
+    #returns dictionary of all cg coefficients to be used at a given value of lmax
+    cg = {}
+    for l1 in range(lmax+1):
+        for l2 in range(lmax+1):
+            for l3 in range(lmax+1):
+                for m1 in range(-l1,l1+1):
+                    for m2 in range(-l2,l2+1):
+                        for m3 in range(-l3,l3+1):
+                            key = '%d,%d,%d,%d,%d,%d' % (l1,m1,l2,m2,l3,m3)
+                            cg[key] = wigner_3j(l1,m1,l2,m2,l3,m3)
+    return cg
 
 
 def get_w3j_and_cg():
-  # store a large dictionary of clebsch gordan coefficients
-  if cglib:
+    # store a large dictionary of clebsch gordan coefficients
+    if cglib:
+        try:
+            with open('%s/Clebsch_Gordan.pickle' %lib_path, 'rb') as handle:
+                Clebsch_Gordan = pickle.load(handle)
+        except FileNotFoundError:
+            print ("Generating your first pickled library of CG coefficients. This will take a few moments...")
+            Clebsch_Gordan = init_clebsch_gordan(10)
+            with open('%s/Clebsch_Gordan.pickle' %lib_path, 'wb') as handle:
+                pickle.dump(Clebsch_Gordan, handle, protocol=pickle.HIGHEST_PROTOCOL)
+    # do the same thing for the traditional wigner_3j symbols
     try:
-      with open('%s/Clebsch_Gordan.pickle' %lib_path, 'rb') as handle:
-        Clebsch_Gordan = pickle.load(handle)
+        with open('%s/Wigner_3j.pickle' % lib_path, 'rb') as handle:
+            Wigner_3j = pickle.load(handle)
     except FileNotFoundError:
-      print ("Generating your first pickled library of CG coefficients. This will take a few moments...")
-      Clebsch_Gordan = init_clebsch_gordan(10)
-      with open('%s/Clebsch_Gordan.pickle' %lib_path, 'wb') as handle:
-        pickle.dump(Clebsch_Gordan, handle, protocol=pickle.HIGHEST_PROTOCOL)
-  # do the same thing for the traditional wigner_3j symbols
-  try:
-    with open('%s/Wigner_3j.pickle' % lib_path, 'rb') as handle:
-      Wigner_3j = pickle.load(handle)
-  except FileNotFoundError:
-    print ("Generating your first pickled library of Wigner 3j coefficients. This will take a few moments...")
-    Wigner_3j = init_wigner_3j(lmax_traditional)
-    with open('%s/Wigner_3j.pickle' % lib_path, 'wb') as handle:
-      pickle.dump(Wigner_3j, handle, protocol=pickle.HIGHEST_PROTOCOL)
+        print ("Generating your first pickled library of Wigner 3j coefficients. This will take a few moments...")
+        Wigner_3j = init_wigner_3j(lmax_traditional)
+        with open('%s/Wigner_3j.pickle' % lib_path, 'wb') as handle:
+            pickle.dump(Wigner_3j, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
-  return Wigner_3j
+    return Wigner_3j
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/genlib.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/genlib.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # global settings for the sym_ACE library
 from fitsnap3lib.lib.sym_ACE.sym_ACE_settings import *
 import sys
 
 try:
-	flag = sys.argv[1]
+    flag = sys.argv[1]
 except IndexError:
-	flag = None
+    flag = None
 if flag != None:
-	#   list of ranks
-	print ('!!! IMPORTANT !!! lmax per rank:')
-	for rank in ranks:
-		print(rank,lmax_dict_G[rank])
-	print ('Attempting to use descriptors with larger lmax values than this per rank will result in KeyError')
-	print ('  To use larger values, edit lmax_dict_G in the sym_ACE_settings.py file. Using larger values \n may result in long times to load libraries.')
-
-	print ('Prompting generation for first library of coupling coefficients:')
-	from wigner_couple import *
-	print (global_ccs)
-	print ('sent')
+    #   list of ranks
+    print ('!!! IMPORTANT !!! lmax per rank:')
+    for rank in ranks:
+        print(rank,lmax_dict_G[rank])
+    print ('Attempting to use descriptors with larger lmax values than this per rank will result in KeyError')
+    print ('  To use larger values, edit lmax_dict_G in the sym_ACE_settings.py file. Using larger values \n may result in long times to load libraries.')
 
+    print ('Prompting generation for first library of coupling coefficients:')
+    from wigner_couple import *
+    print (global_ccs)
+    print ('sent')
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py`

 * *Files 17% similar despite different names*

```diff
@@ -324,90 +324,89 @@
  ((0, 7, 1, 6), (2, 3)),
  ((0, 7), (1, 6), (2, 3)),
  ((0, 7, 1, 6), (2, 3), (4, 5)),
  ((0, 7), (1, 6), (2, 3), (4, 5))]
 
 
 def filled_perm(tups,rank):
-	allinds = list(range(rank))
-	try:
-		remainders = [ i for i in allinds if i not in flatten(tups)]
-		alltups = tups + tuple([tuple([k]) for k in remainders])
-	except TypeError:
-		remainders = [ i for i in allinds if i not in flatten(flatten(tups))]
-		alltups = tups + tuple([tuple([k]) for k in remainders])
-	return alltups
+    allinds = list(range(rank))
+    try:
+        remainders = [ i for i in allinds if i not in flatten(tups)]
+        alltups = tups + tuple([tuple([k]) for k in remainders])
+    except TypeError:
+        remainders = [ i for i in allinds if i not in flatten(flatten(tups))]
+        alltups = tups + tuple([tuple([k]) for k in remainders])
+    return alltups
 
 def base_automorphisms(l,subtree=False):
-	# base automorphism groups for most practical descriptor labels.
-	if len(l) == 4 or len(l) == 5:
-		if not subtree:
-			all_ops = sylow_2_s4
-		else:
-			all_ops = s4_subtree_syms
-	elif len(l) == 6 or len(l) == 7:
-		if not subtree:
-			all_ops = sylow_2_s6
-		else:
-			all_ops = s6_subtree_syms
-	elif len(l) == 8 or len(l) == 9:
-		if not subtree:
-			all_ops = sylow_2_s8
-		else:
-			all_ops = s8_subtree_syms
-	else:
-		raise ValueError()
-
-	all_ops.sort(key=lambda x: x,reverse=True)
-	all_ops.sort(key=lambda x: tuple([len(k) for k in x]),reverse=True)
-
-	all_ops = [filled_perm(op,len(l)) for op in all_ops]
-
-	all_parts = []
-	for op in all_ops:
-		orbits = [len(x) for x in op]
-		partition = tuple(orbits)
-		all_parts.append(partition)
-	unique_parts = list(set(all_parts))
-	unique_parts.sort(key=lambda x: len(x),reverse=True)
-	unique_parts.sort(key=lambda x: x,reverse=True)
-	op_per_part = {p:[] for p in unique_parts}
-	for op_part in zip(all_ops,all_parts):
-		this_op,this_part = op_part
-		op_per_part[this_part].append(this_op)
-
-	if tuple([len(l)]) not in unique_parts:
-		unique_parts = [tuple([len(l)])] + unique_parts
-		op_per_part[tuple([len(l)])] = [  tuple([ tuple([i]) for i in  range(len(l))]) ]
-	organized_automorphisms = {p: sorted(op_per_part[p]) for p in unique_parts} 
-	return organized_automorphisms
+    # base automorphism groups for most practical descriptor labels.
+    if len(l) == 4 or len(l) == 5:
+        if not subtree:
+            all_ops = sylow_2_s4
+        else:
+            all_ops = s4_subtree_syms
+    elif len(l) == 6 or len(l) == 7:
+        if not subtree:
+            all_ops = sylow_2_s6
+        else:
+            all_ops = s6_subtree_syms
+    elif len(l) == 8 or len(l) == 9:
+        if not subtree:
+            all_ops = sylow_2_s8
+        else:
+            all_ops = s8_subtree_syms
+    else:
+        raise ValueError()
+
+    all_ops.sort(key=lambda x: x,reverse=True)
+    all_ops.sort(key=lambda x: tuple([len(k) for k in x]),reverse=True)
+
+    all_ops = [filled_perm(op,len(l)) for op in all_ops]
+
+    all_parts = []
+    for op in all_ops:
+        orbits = [len(x) for x in op]
+        partition = tuple(orbits)
+        all_parts.append(partition)
+    unique_parts = list(set(all_parts))
+    unique_parts.sort(key=lambda x: len(x),reverse=True)
+    unique_parts.sort(key=lambda x: x,reverse=True)
+    op_per_part = {p:[] for p in unique_parts}
+    for op_part in zip(all_ops,all_parts):
+        this_op,this_part = op_part
+        op_per_part[this_part].append(this_op)
+
+    if tuple([len(l)]) not in unique_parts:
+        unique_parts = [tuple([len(l)])] + unique_parts
+        op_per_part[tuple([len(l)])] = [  tuple([ tuple([i]) for i in  range(len(l))]) ]
+    organized_automorphisms = {p: sorted(op_per_part[p]) for p in unique_parts} 
+    return organized_automorphisms
 
 def get_auto_part(l,part,add_degen_autos=False,part_only=False,subtree=False):
-	
-	# grows the automorphism group for a given l vector,
-	#   and returns permutation operations belonging to specific set of orbits
-	#   in the partition 'part' 
-	#   add_degen_autos (logical) : flag to grow automorphism group based on degeneracy
-	#   part_only (logical) : flag to return automorphisms within one set of orbits
-
-	N = len(l)
-	G_N_per_part = base_automorphisms(l,subtree)
-	if part_only:
-		applied_perms = [tuple(Permutation(filled_perm(pi,len(l)))(l)) for pi in G_N_per_part[part]]
-	elif not part_only:
-		applied_perms = [tuple(Permutation(filled_perm(pi,len(l)))(l)) for pi in flatten(G_N_per_part.values())]
-	autos = []
-	if add_degen_autos:
-		perms = [p for p in itertools.permutations(range(N))]	
-		for perm in perms:
-			P = Permutation(perm)
-			cyc = P.full_cyclic_form
-			cyc = tuple([tuple(k) for k in cyc])
-			this_applied = P(l)
-			if tuple(this_applied) in applied_perms:
-				autos.append(cyc)
-	if part_only:
-		return_lst = sorted(list(set(G_N_per_part[part] + autos)))
-	elif not part_only:
-		return_lst = sorted(list(set(flatten(G_N_per_part.values()) + autos)))
-	return return_lst
-
+    
+    # grows the automorphism group for a given l vector,
+    #   and returns permutation operations belonging to specific set of orbits
+    #   in the partition 'part' 
+    #   add_degen_autos (logical) : flag to grow automorphism group based on degeneracy
+    #   part_only (logical) : flag to return automorphisms within one set of orbits
+
+    N = len(l)
+    G_N_per_part = base_automorphisms(l,subtree)
+    if part_only:
+        applied_perms = [tuple(Permutation(filled_perm(pi,len(l)))(l)) for pi in G_N_per_part[part]]
+    elif not part_only:
+        applied_perms = [tuple(Permutation(filled_perm(pi,len(l)))(l)) for pi in flatten(G_N_per_part.values())]
+    autos = []
+    if add_degen_autos:
+        perms = [p for p in itertools.permutations(range(N))]   
+        for perm in perms:
+            P = Permutation(perm)
+            cyc = P.full_cyclic_form
+            cyc = tuple([tuple(k) for k in cyc])
+            this_applied = P(l)
+            if tuple(this_applied) in applied_perms:
+                autos.append(cyc)
+    if part_only:
+        return_lst = sorted(list(set(G_N_per_part[part] + autos)))
+    elif not part_only:
+        return_lst = sorted(list(set(flatten(G_N_per_part.values()) + autos)))
+    return return_lst
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,318 +7,318 @@
 global_lsyms = {}
 global_lsemi = {}
 global_parts = {}
 global_orbits = {}
 
 
 def permutation_adapted_lL(l,semistandardflag=True):
-	# This is a function to return the permutation-adapted angular 
-	#  basis labels. It finds the varsigma(l) permutations for a 
-	#  provided block of l_i (as a list)
-	
-	#----------------------------------------------------------------
-	# Define the identity l_o based on degeneracy and the coupling 
-	# scheme. (This is no longer necessary but it makes for smaller
-	# amounts of permutations to sift over to find the full set of
-	#  { \varsigma(l) }
-	#----------------------------------------------------------------
-	N = len(l)
-	uniques = list(set(l))
-	tmp = l.copy()
-	tmp.sort(key=Counter(l).get,reverse=True)
-	uniques.sort(key=Counter(tmp).get,reverse=True)
-	count_uniques =[l.count(u) for u in uniques]
-	mp = {uniques[i]:i for i in range(len(uniques))}
-	mprev = {i:uniques[i] for i in range(len(uniques))}
-	mapped = [mp[t] for t in tmp]
-	
-	if len(uniques) == math.floor(len(l)/2):# and 0 in uniques:
-		l.sort(key=Counter(l).get,reverse=True)
-		mapped.sort(key=Counter(mapped).get,reverse=True)
-	else:
-		l = sort_pair(l)
-		mapped = sort_pair(mapped)
-	assert len(l) <= 6, "symmetry reduction is only needed for rank 4 + descriptors. Use a rank between 4 and 6, automorphism groups for rank >= 7 to be added soon."
-	N = len(l)
-	if verbose:
-		print ('lrep',l)
-	#----------------------------------------------------------------
-	# End definition of the identity
-	#----------------------------------------------------------------
-
-
-	#----------------------------------------------------------------
-	# Use young subgroup fillings to reduce a full search over S_N
-	#  to obtain \varsigma(l) and irrep. The young subgroup used is
-	#  S_2 \otimes S_2 \otimes ... S_2  - for N/2 iterations if N is
-	#  even and
-	#  S_2 \otimes S_2 \otimes ... \otimes S_1 - for floor(N/2) 
-	#  iterations if N is odd.
-	#----------------------------------------------------------------
-	
-	try:
-		sigma_c_parts = global_parts[N]
-	except KeyError:
-		
-		ysgi = Young_Subgroup(N)
-		sigma_c_parts = ysgi.sigma_c_partitions(max_orbit=N)
-		sigma_c_parts.sort(key=lambda x: x.count(2),reverse=True)
-		sigma_c_parts.sort(key=lambda x: tuple([i%2==0 for i in x]),reverse=True)
-		sigma_c_parts.sort(key=lambda x: max(x),reverse=True)
-		global_parts[N] = sigma_c_parts
-		if verbose:
-			print (sigma_c_parts)
-	try:
-		lperms = global_lsyms[tuple(mapped)]
-		part_per_fill = global_orbits[tuple(mapped)]
-		lperms_semistandard = global_lsemi[tuple(mapped)]
-	except KeyError:
-		ysgi = Young_Subgroup(N)
-		ysgi.subgroup_fill(mapped,sigma_c_parts,sigma_c_symmetric=True,semistandard=False)
-		lperms = ysgi.fills.copy()
-		lperms = ysgi.reduce_list(mapped,lperms)
-		part_per_fill = ysgi.partitions_per_fill
-		ysgi.subgroup_fill(mapped,sigma_c_parts,sigma_c_symmetric=True,semistandard=True)
-		lperms_semistandard = ysgi.fills.copy()
-		standard_part_per_fill = ysgi.partitions_per_fill
-		global_lsyms[tuple(mapped)] = lperms
-		global_orbits[tuple(mapped)] = part_per_fill
-		global_lsemi[tuple(mapped)] = lperms_semistandard
-		if verbose:
-			print ('lperms_ysg_not',lperms)
-			print ('lperms_ysg_semistandard',lperms_semistandard)
-			print ('highest symmetry orbits per filling', part_per_fill)
-	myvarsigma_l = [tuple([mprev[k] for k in lp]) for lp in lperms]
-	myvarsigma_l = sorted(myvarsigma_l)
-	varsigma_l = []
-
-	L_per_varsigma = {}
-
-	for vsl in myvarsigma_l:
-		#print ('vsl in loop',vsl)
-		varsigma_l.append(vsl)
-		L_lp = tree_l_inters(vsl)
-		nodes,remainder = tree(vsl)
-		lnodes_lp = group_vec_by_node(vsl,nodes,remainder)
-		L_lp_filtered = parity_filter(lnodes_lp,L_lp)
-		L_per_varsigma[ vsl]=L_lp_filtered
-
-	reps_per_varsigma = {}
-	for fill,irreps in part_per_fill.items():
-		lmp = tuple([mprev[k] for k in fill])
-		reps_per_varsigma[lmp] = irreps
-	
-	# the following loop eliminates dependent labels due to
-	#  degeneracies in internal nodes. (e.g. removes trees with
-	#  equivalent branch structures once intermediates are applied)
-	quick_build = []
-	orbids = []
-	leafids = []
-	used_l = []
-	all_autos = []
-	ysg = Young_Subgroup(N)
-	for lp, Lp_lst in L_per_varsigma.items():
-		ti = Tree_ID(lp,Lp_lst[-1])
-		orbi = ti.return_orbit_l_ID()
-		leafi = ti.return_leaf_l_ID()
-		ysg.set_inds(lp)
-		automorphisms = get_auto_part(tuple(lp),tuple([len(lp)]),add_degen_autos=False,part_only=False)
-		conj1, applied_conj,conj_list = ysg.apply_automorphism_conjugation(my_automorphisms=automorphisms)
-		# first catch any binary trees that share the same
-		#  leaf structure as the coupling permutation, \sigma_c
-		if leafi not in leafids:
-			quick_build.append( (lp,Lp_lst[-1]))
-			orbids.append(orbi)
-			leafids.append(leafi)
-			all_autos.extend(conj_list)
-		# secondly, catch binary trees that share more symmetry
-		#  even if it has a leaf structure compatible with \sigma_c
-		#  as well. (Needed for degenerate l_i)
-		if orbi not in orbids:
-			quick_build.append( (lp,Lp_lst[-1]))
-			orbids.append(orbi)
-			leafids.append(leafi)
-			all_autos.extend(conj_list)
-
-	varsigma_lL = quick_build.copy()
-	# for each varsigma(l) - provide the highest symmetry partition
-	#  (isomorphic to an irrep in S_N) it is compatible with
-	highest_sym_reps = {}
-	for lL in varsigma_lL:
-		varsigmali,intersi = lL
-		reps = reps_per_varsigma[varsigmali]
-		highest_sym_reps[lL] = reps[0]
-			
-	return varsigma_lL, highest_sym_reps
+    # This is a function to return the permutation-adapted angular 
+    #  basis labels. It finds the varsigma(l) permutations for a 
+    #  provided block of l_i (as a list)
+    
+    #----------------------------------------------------------------
+    # Define the identity l_o based on degeneracy and the coupling 
+    # scheme. (This is no longer necessary but it makes for smaller
+    # amounts of permutations to sift over to find the full set of
+    #  { \varsigma(l) }
+    #----------------------------------------------------------------
+    N = len(l)
+    uniques = list(set(l))
+    tmp = l.copy()
+    tmp.sort(key=Counter(l).get,reverse=True)
+    uniques.sort(key=Counter(tmp).get,reverse=True)
+    count_uniques =[l.count(u) for u in uniques]
+    mp = {uniques[i]:i for i in range(len(uniques))}
+    mprev = {i:uniques[i] for i in range(len(uniques))}
+    mapped = [mp[t] for t in tmp]
+    
+    if len(uniques) == math.floor(len(l)/2):# and 0 in uniques:
+        l.sort(key=Counter(l).get,reverse=True)
+        mapped.sort(key=Counter(mapped).get,reverse=True)
+    else:
+        l = sort_pair(l)
+        mapped = sort_pair(mapped)
+    assert len(l) <= 6, "symmetry reduction is only needed for rank 4 + descriptors. Use a rank between 4 and 6, automorphism groups for rank >= 7 to be added soon."
+    N = len(l)
+    if verbose:
+        print ('lrep',l)
+    #----------------------------------------------------------------
+    # End definition of the identity
+    #----------------------------------------------------------------
+
+
+    #----------------------------------------------------------------
+    # Use young subgroup fillings to reduce a full search over S_N
+    #  to obtain \varsigma(l) and irrep. The young subgroup used is
+    #  S_2 \otimes S_2 \otimes ... S_2  - for N/2 iterations if N is
+    #  even and
+    #  S_2 \otimes S_2 \otimes ... \otimes S_1 - for floor(N/2) 
+    #  iterations if N is odd.
+    #----------------------------------------------------------------
+    
+    try:
+        sigma_c_parts = global_parts[N]
+    except KeyError:
+        
+        ysgi = Young_Subgroup(N)
+        sigma_c_parts = ysgi.sigma_c_partitions(max_orbit=N)
+        sigma_c_parts.sort(key=lambda x: x.count(2),reverse=True)
+        sigma_c_parts.sort(key=lambda x: tuple([i%2==0 for i in x]),reverse=True)
+        sigma_c_parts.sort(key=lambda x: max(x),reverse=True)
+        global_parts[N] = sigma_c_parts
+        if verbose:
+            print (sigma_c_parts)
+    try:
+        lperms = global_lsyms[tuple(mapped)]
+        part_per_fill = global_orbits[tuple(mapped)]
+        lperms_semistandard = global_lsemi[tuple(mapped)]
+    except KeyError:
+        ysgi = Young_Subgroup(N)
+        ysgi.subgroup_fill(mapped,sigma_c_parts,sigma_c_symmetric=True,semistandard=False)
+        lperms = ysgi.fills.copy()
+        lperms = ysgi.reduce_list(mapped,lperms)
+        part_per_fill = ysgi.partitions_per_fill
+        ysgi.subgroup_fill(mapped,sigma_c_parts,sigma_c_symmetric=True,semistandard=True)
+        lperms_semistandard = ysgi.fills.copy()
+        standard_part_per_fill = ysgi.partitions_per_fill
+        global_lsyms[tuple(mapped)] = lperms
+        global_orbits[tuple(mapped)] = part_per_fill
+        global_lsemi[tuple(mapped)] = lperms_semistandard
+        if verbose:
+            print ('lperms_ysg_not',lperms)
+            print ('lperms_ysg_semistandard',lperms_semistandard)
+            print ('highest symmetry orbits per filling', part_per_fill)
+    myvarsigma_l = [tuple([mprev[k] for k in lp]) for lp in lperms]
+    myvarsigma_l = sorted(myvarsigma_l)
+    varsigma_l = []
+
+    L_per_varsigma = {}
+
+    for vsl in myvarsigma_l:
+        #print ('vsl in loop',vsl)
+        varsigma_l.append(vsl)
+        L_lp = tree_l_inters(vsl)
+        nodes,remainder = tree(vsl)
+        lnodes_lp = group_vec_by_node(vsl,nodes,remainder)
+        L_lp_filtered = parity_filter(lnodes_lp,L_lp)
+        L_per_varsigma[ vsl]=L_lp_filtered
+
+    reps_per_varsigma = {}
+    for fill,irreps in part_per_fill.items():
+        lmp = tuple([mprev[k] for k in fill])
+        reps_per_varsigma[lmp] = irreps
+    
+    # the following loop eliminates dependent labels due to
+    #  degeneracies in internal nodes. (e.g. removes trees with
+    #  equivalent branch structures once intermediates are applied)
+    quick_build = []
+    orbids = []
+    leafids = []
+    used_l = []
+    all_autos = []
+    ysg = Young_Subgroup(N)
+    for lp, Lp_lst in L_per_varsigma.items():
+        ti = Tree_ID(lp,Lp_lst[-1])
+        orbi = ti.return_orbit_l_ID()
+        leafi = ti.return_leaf_l_ID()
+        ysg.set_inds(lp)
+        automorphisms = get_auto_part(tuple(lp),tuple([len(lp)]),add_degen_autos=False,part_only=False)
+        conj1, applied_conj,conj_list = ysg.apply_automorphism_conjugation(my_automorphisms=automorphisms)
+        # first catch any binary trees that share the same
+        #  leaf structure as the coupling permutation, \sigma_c
+        if leafi not in leafids:
+            quick_build.append( (lp,Lp_lst[-1]))
+            orbids.append(orbi)
+            leafids.append(leafi)
+            all_autos.extend(conj_list)
+        # secondly, catch binary trees that share more symmetry
+        #  even if it has a leaf structure compatible with \sigma_c
+        #  as well. (Needed for degenerate l_i)
+        if orbi not in orbids:
+            quick_build.append( (lp,Lp_lst[-1]))
+            orbids.append(orbi)
+            leafids.append(leafi)
+            all_autos.extend(conj_list)
+
+    varsigma_lL = quick_build.copy()
+    # for each varsigma(l) - provide the highest symmetry partition
+    #  (isomorphic to an irrep in S_N) it is compatible with
+    highest_sym_reps = {}
+    for lL in varsigma_lL:
+        varsigmali,intersi = lL
+        reps = reps_per_varsigma[varsigmali]
+        highest_sym_reps[lL] = reps[0]
+            
+    return varsigma_lL, highest_sym_reps
 
 def permutation_adapted_nlL(n,l,semistandardflag=True):
-	# flag to return in descriptor label format for FitSNAP
-	return_desclabels = True
+    # flag to return in descriptor label format for FitSNAP
+    return_desclabels = True
 
-	#------------------------------------------------------------------
-	# generate PA-RI basis and corresponding irreps of SN
-	lLs, SN_irreps = permutation_adapted_lL(l,semistandardflag)
-
-	# initialize lists for permutation adapted nl labels
-	#  and used binary trees, respectively
-	varsigma_nls = []
-	used_nl_reps = []
-
-	# make all permutations of n ( the function below removes explicit
-	#  redundancies such as n_1=(1111), n_2=(1111) that are generated
-	#  when using python-native enumerations (e.g. itertools.permutations)
-	ns = unique_perms(n)
-	
-	# using the set { \varsigma_l } and the corresponding highest symmetry
-	#  set of orbits used to generate \varsigma_l, find all unique nl
-	#  nl trees. (To go from permutation-adapted angular indices to 
-	#  permutation-adapted radial + angular indices, we add more leaves to the
-	#  tree.
-	for lL,irrep in SN_irreps.items():
-		li,Li = lL
-		ti = Tree_ID(li,Li)
-		loid = ti.return_orbit_l_ID(orbit=irrep)
-		for nperm in ns:
-			nloid = ti.return_orbit_nl_ID(nperm,orbit=irrep)
-			if verbose:
-				print (nloid)
-			if nloid not in used_nl_reps:
-				used_nl_reps.append(nloid)
-				varsigma_nls.append((nperm,li,Li))
-
-	
-
-	#------------------------------------------------------------------
-
-	# Remaining code in this function is to return descriptor labels in 
-	#  fitsnap format.
-	descriptor_labels = []
-	# enforce single element in lite version
-	nelements=1
-	N = len(l)
-	for mu0 in range(nelements):
-		for munlL in varsigma_nls:
-			munlL = tuple([ tuple([0]*N)  ]) + munlL
-			st='%d_' % mu0
-			tmp=  ','.join([b for b in ['%d']*N*(3)])
-			tmp = tmp % tuple(flatten(munlL[:-1]))
-			st +=tmp
-			st+=  '_'
-			st+= '-'.join(str(b) for b in munlL[3])
-			descriptor_labels.append(st)
-	if return_desclabels:
-		return descriptor_labels
-	else:
-		return varsigma_nls
+    #------------------------------------------------------------------
+    # generate PA-RI basis and corresponding irreps of SN
+    lLs, SN_irreps = permutation_adapted_lL(l,semistandardflag)
+
+    # initialize lists for permutation adapted nl labels
+    #  and used binary trees, respectively
+    varsigma_nls = []
+    used_nl_reps = []
+
+    # make all permutations of n ( the function below removes explicit
+    #  redundancies such as n_1=(1111), n_2=(1111) that are generated
+    #  when using python-native enumerations (e.g. itertools.permutations)
+    ns = unique_perms(n)
+    
+    # using the set { \varsigma_l } and the corresponding highest symmetry
+    #  set of orbits used to generate \varsigma_l, find all unique nl
+    #  nl trees. (To go from permutation-adapted angular indices to 
+    #  permutation-adapted radial + angular indices, we add more leaves to the
+    #  tree.
+    for lL,irrep in SN_irreps.items():
+        li,Li = lL
+        ti = Tree_ID(li,Li)
+        loid = ti.return_orbit_l_ID(orbit=irrep)
+        for nperm in ns:
+            nloid = ti.return_orbit_nl_ID(nperm,orbit=irrep)
+            if verbose:
+                print (nloid)
+            if nloid not in used_nl_reps:
+                used_nl_reps.append(nloid)
+                varsigma_nls.append((nperm,li,Li))
+
+    
+
+    #------------------------------------------------------------------
+
+    # Remaining code in this function is to return descriptor labels in 
+    #  fitsnap format.
+    descriptor_labels = []
+    # enforce single element in lite version
+    nelements=1
+    N = len(l)
+    for mu0 in range(nelements):
+        for munlL in varsigma_nls:
+            munlL = tuple([ tuple([0]*N)  ]) + munlL
+            st='%d_' % mu0
+            tmp=  ','.join([b for b in ['%d']*N*(3)])
+            tmp = tmp % tuple(flatten(munlL[:-1]))
+            st +=tmp
+            st+=  '_'
+            st+= '-'.join(str(b) for b in munlL[3])
+            descriptor_labels.append(st)
+    if return_desclabels:
+        return descriptor_labels
+    else:
+        return varsigma_nls
 
 
 def permutation_adapted_munlL(mu,n,l,nelements=1,semistandardflag=True):
-	# flag to return in descriptor label format for FitSNAP
-	return_desclabels = True
+    # flag to return in descriptor label format for FitSNAP
+    return_desclabels = True
 
-	#------------------------------------------------------------------
-	# generate PA-RI basis and corresponding irreps of SN
-	lLs, SN_irreps = permutation_adapted_lL(l,semistandardflag)
-
-	# initialize lists for permutation adapted nl labels
-	#  and used binary trees, respectively
-	varsigma_nls = []
-	used_nl_reps = []
-
-	# make all permutations of n ( the function below removes explicit
-	#  redundancies such as n_1=(1111), n_2=(1111) that are generated
-	#  when using python-native enumerations (e.g. itertools.permutations)
-	ns = unique_perms(n)
-	mus = unique_perms(mu)
-	
-	# using the set { \varsigma_l } and the corresponding highest symmetry
-	#  set of orbits used to generate \varsigma_l, find all unique nl
-	#  nl trees. (To go from permutation-adapted angular indices to 
-	#  permutation-adapted radial + angular indices, we add more leaves to the
-	#  tree.
-	for lL,irrep in SN_irreps.items():
-		li,Li = lL
-		ti = Tree_ID(li,Li)
-		loid = ti.return_orbit_l_ID(orbit=irrep)
-		for nperm in ns:
-			for muperm in mus:
-				nloid = ti.return_orbit_munl_ID(muperm,nperm,orbit=irrep)
-				if verbose:
-					print (nloid)
-				if nloid not in used_nl_reps:
-					used_nl_reps.append(nloid)
-					varsigma_nls.append((muperm,nperm,li,Li))
-
-	
-
-	#------------------------------------------------------------------
-
-	# Remaining code in this function is to return descriptor labels in 
-	#  fitsnap format.
-	descriptor_labels = []
-	N = len(l)
-	for mu0 in range(nelements):
-		for munlL in varsigma_nls:
-			munlL = munlL
-			st='%d_' % mu0
-			tmp=  ','.join([b for b in ['%d']*N*(3)])
-			tmp = tmp % tuple(flatten(munlL[:-1]))
-			st +=tmp
-			st +=  '_'
-			st += '-'.join(str(b) for b in munlL[3])
-			descriptor_labels.append(st)
-	if return_desclabels:
-		return descriptor_labels
-	else:
-		return varsigma_nls
+    #------------------------------------------------------------------
+    # generate PA-RI basis and corresponding irreps of SN
+    lLs, SN_irreps = permutation_adapted_lL(l,semistandardflag)
+
+    # initialize lists for permutation adapted nl labels
+    #  and used binary trees, respectively
+    varsigma_nls = []
+    used_nl_reps = []
+
+    # make all permutations of n ( the function below removes explicit
+    #  redundancies such as n_1=(1111), n_2=(1111) that are generated
+    #  when using python-native enumerations (e.g. itertools.permutations)
+    ns = unique_perms(n)
+    mus = unique_perms(mu)
+    
+    # using the set { \varsigma_l } and the corresponding highest symmetry
+    #  set of orbits used to generate \varsigma_l, find all unique nl
+    #  nl trees. (To go from permutation-adapted angular indices to 
+    #  permutation-adapted radial + angular indices, we add more leaves to the
+    #  tree.
+    for lL,irrep in SN_irreps.items():
+        li,Li = lL
+        ti = Tree_ID(li,Li)
+        loid = ti.return_orbit_l_ID(orbit=irrep)
+        for nperm in ns:
+            for muperm in mus:
+                nloid = ti.return_orbit_munl_ID(muperm,nperm,orbit=irrep)
+                if verbose:
+                    print (nloid)
+                if nloid not in used_nl_reps:
+                    used_nl_reps.append(nloid)
+                    varsigma_nls.append((muperm,nperm,li,Li))
+
+    
+
+    #------------------------------------------------------------------
+
+    # Remaining code in this function is to return descriptor labels in 
+    #  fitsnap format.
+    descriptor_labels = []
+    N = len(l)
+    for mu0 in range(nelements):
+        for munlL in varsigma_nls:
+            munlL = munlL
+            st='%d_' % mu0
+            tmp=  ','.join([b for b in ['%d']*N*(3)])
+            tmp = tmp % tuple(flatten(munlL[:-1]))
+            st +=tmp
+            st +=  '_'
+            st += '-'.join(str(b) for b in munlL[3])
+            descriptor_labels.append(st)
+    if return_desclabels:
+        return descriptor_labels
+    else:
+        return varsigma_nls
 
 
 
 def descriptor_labels_YSG(rank,nmax,lmax,mumax=1,lmin=1):
-	if mumax ==0:
-		mumax = 1
-		
-	if rank >= 4:
-		lrng = list(range(lmin,lmax+1))
-		nrng = list(range(1,nmax+1))
-		murng = list(range(mumax))
-		# function to return all l vectors obeying angular momentum
-		#  N-dimensional polygon conditions for coupling scheme in
-		#  paper.
-		lstrs = generate_l_LR(lrng , rank , L_R = 0)
-
-		ns = [i for i in itertools.combinations_with_replacement(nrng,rank)]
-		mus = [i for i in itertools.combinations_with_replacement(murng,rank)]
-		used_ls = []
-		labels = []
-		
-		# loop over n and l vectors and build permutation-adapted blocks
-		#  for all combinations of these vectors
-		if mumax ==0 or mumax==1:
-			for lstr in sorted(list(set(lstrs))):
-				l = [int(k) for k in lstr.split(',')]
-				N = len(l)
-				for n in ns:
-					lrep = tuple([ tuple(sorted(l)), tuple(sorted(n))])
-					if lrep not in used_ls:
-						nls = permutation_adapted_nlL(n,l)
-						used_ls.append(lrep)
-						labels.extend(nls)
-		else:
-			for lstr in sorted(list(set(lstrs))):
-				l = [int(k) for k in lstr.split(',')]
-				N = len(l)
-				for n in ns:
-					for mu in mus:
-						lrep = tuple([ tuple(sorted(l)), tuple(sorted(n)), tuple(sorted(mu))])
-						if lrep not in used_ls:
-							munls = permutation_adapted_munlL(mu,n,l,nelements=mumax)
-							used_ls.append(lrep)
-							labels.extend(munls)
-			
-
-	elif rank < 4:
-		# no symmetry reduction required for rank <= 3
-		# use typical lexicographical ordering for such cases 
-		labels = generate_nl(rank,nmax,lmax,mumax=mumax,lmin=lmin,L_R=0,M_R=0,all_perms=False)	
-	munltups = [get_mu_n_l(nu,return_L=True) for nu in labels]
-	return labels
+    if mumax ==0:
+        mumax = 1
+        
+    if rank >= 4:
+        lrng = list(range(lmin,lmax+1))
+        nrng = list(range(1,nmax+1))
+        murng = list(range(mumax))
+        # function to return all l vectors obeying angular momentum
+        #  N-dimensional polygon conditions for coupling scheme in
+        #  paper.
+        lstrs = generate_l_LR(lrng , rank , L_R = 0)
+
+        ns = [i for i in itertools.combinations_with_replacement(nrng,rank)]
+        mus = [i for i in itertools.combinations_with_replacement(murng,rank)]
+        used_ls = []
+        labels = []
+        
+        # loop over n and l vectors and build permutation-adapted blocks
+        #  for all combinations of these vectors
+        if mumax ==0 or mumax==1:
+            for lstr in sorted(list(set(lstrs))):
+                l = [int(k) for k in lstr.split(',')]
+                N = len(l)
+                for n in ns:
+                    lrep = tuple([ tuple(sorted(l)), tuple(sorted(n))])
+                    if lrep not in used_ls:
+                        nls = permutation_adapted_nlL(n,l)
+                        used_ls.append(lrep)
+                        labels.extend(nls)
+        else:
+            for lstr in sorted(list(set(lstrs))):
+                l = [int(k) for k in lstr.split(',')]
+                N = len(l)
+                for n in ns:
+                    for mu in mus:
+                        lrep = tuple([ tuple(sorted(l)), tuple(sorted(n)), tuple(sorted(mu))])
+                        if lrep not in used_ls:
+                            munls = permutation_adapted_munlL(mu,n,l,nelements=mumax)
+                            used_ls.append(lrep)
+                            labels.extend(munls)
+            
+
+    elif rank < 4:
+        # no symmetry reduction required for rank <= 3
+        # use typical lexicographical ordering for such cases 
+        labels = generate_nl(rank,nmax,lmax,mumax=mumax,lmin=lmin,L_R=0,M_R=0,all_perms=False)  
+    munltups = [get_mu_n_l(nu,return_L=True) for nu in labels]
+    return labels
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,121 +11,121 @@
 from fitsnap3lib.lib.sym_ACE.tree_method import *
 from fitsnap3lib.lib.sym_ACE.gen_labels import *
 from sympy.combinatorics import Permutation
 from functools import partial
 
 
 def get_coupling(ldict, Wigner_3j, L_R=0,**kwargs):
-	M_Rs = list(range(-L_R,L_R+1))
-	#generic coupling for any L_R - support must be added to call 
-	ranks = list(ldict.keys())
-	coupling = {M_R : {rank:{} for rank in ranks} for M_R in M_Rs}
-
-	#weights are only necessary when generating linear combinations of wigner coefficients
-	weights = None
-	for M_R in M_Rs:
-		for rank in ranks:
-			rnk = rank
-			ls_per_rnk = generate_l_LR(range(ldict[rank]+1),rank,L_R,M_R)
-			for lstr in ls_per_rnk:
-				l = [int(k) for k in lstr.split(',')]
-				if rank ==1:
-					decomped = rank_1_tree(l,Wigner_3j, L_R,M_R)
-					coupling[M_R][rnk][lstr] = decomped
-				elif rank ==2:
-					decomped = rank_2_tree(l,Wigner_3j,L_R,M_R)
-					coupling[M_R][rnk][lstr] = decomped
-				elif rank ==3:
-					decomped = rank_3_tree(l,Wigner_3j,L_R,M_R)
-					coupling[M_R][rnk][lstr] = decomped
-				elif rank ==4:
-					decomped = rank_4_tree(l,Wigner_3j,L_R,M_R)
-					coupling[M_R][rnk][lstr] = decomped
-				elif rank ==5:
-					decomped = rank_5_tree(l,Wigner_3j,L_R,M_R)
-					coupling[M_R][rnk][lstr] = decomped
-				elif rank ==6:
-					decomped = rank_6_tree(l,Wigner_3j,L_R,M_R)
-					coupling[M_R][rnk][lstr] = decomped
-				elif rank ==7:
-					decomped = rank_7_tree(l,Wigner_3j,L_R,M_R)
-					coupling[M_R][rnk][lstr] = decomped
-				elif rank ==8:
-					decomped = rank_8_tree(l,Wigner_3j,L_R,M_R)
-					coupling[M_R][rnk][lstr] = decomped
-				elif rank > 8:
-					raise ValueError("Cannot generate couplings for rank %d. symmetric L_R couplings up to rank 6 have been implemented" % rank)
-	return coupling,weights
+    M_Rs = list(range(-L_R,L_R+1))
+    #generic coupling for any L_R - support must be added to call 
+    ranks = list(ldict.keys())
+    coupling = {M_R : {rank:{} for rank in ranks} for M_R in M_Rs}
+
+    #weights are only necessary when generating linear combinations of wigner coefficients
+    weights = None
+    for M_R in M_Rs:
+        for rank in ranks:
+            rnk = rank
+            ls_per_rnk = generate_l_LR(range(ldict[rank]+1),rank,L_R,M_R)
+            for lstr in ls_per_rnk:
+                l = [int(k) for k in lstr.split(',')]
+                if rank ==1:
+                    decomped = rank_1_tree(l,Wigner_3j, L_R,M_R)
+                    coupling[M_R][rnk][lstr] = decomped
+                elif rank ==2:
+                    decomped = rank_2_tree(l,Wigner_3j,L_R,M_R)
+                    coupling[M_R][rnk][lstr] = decomped
+                elif rank ==3:
+                    decomped = rank_3_tree(l,Wigner_3j,L_R,M_R)
+                    coupling[M_R][rnk][lstr] = decomped
+                elif rank ==4:
+                    decomped = rank_4_tree(l,Wigner_3j,L_R,M_R)
+                    coupling[M_R][rnk][lstr] = decomped
+                elif rank ==5:
+                    decomped = rank_5_tree(l,Wigner_3j,L_R,M_R)
+                    coupling[M_R][rnk][lstr] = decomped
+                elif rank ==6:
+                    decomped = rank_6_tree(l,Wigner_3j,L_R,M_R)
+                    coupling[M_R][rnk][lstr] = decomped
+                elif rank ==7:
+                    decomped = rank_7_tree(l,Wigner_3j,L_R,M_R)
+                    coupling[M_R][rnk][lstr] = decomped
+                elif rank ==8:
+                    decomped = rank_8_tree(l,Wigner_3j,L_R,M_R)
+                    coupling[M_R][rnk][lstr] = decomped
+                elif rank > 8:
+                    raise ValueError("Cannot generate couplings for rank %d. symmetric L_R couplings up to rank 6 have been implemented" % rank)
+    return coupling,weights
 
 
 
 def local_coupling(l,L_R=0,**kwargs):
-	M_Rs = list(range(-L_R,L_R+1))
-	#generic coupling for any L_R - support must be added to call 
-	ranks = [len(l)]
-	coupling = {M_R : {rank:{} for rank in ranks} for M_R in M_Rs}
-
-	#weights are only necessary when generating linear combinations of wigner coefficients
-	weights = None
-	for M_R in M_Rs:
-		rank = len(l)
-		rnk = rank
-		lstr = ','.join([str(li) for li in l])
-		if type(l) == str:
-			l = [int(k) for k in l.split(',')]
-		if rank ==1:
-			decomped = rank_1_tree(l,L_R,M_R)
-			coupling[M_R][rnk][lstr] = decomped
-		elif rank ==2:
-			decomped = rank_2_tree(l,L_R,M_R)
-			coupling[M_R][rnk][lstr] = decomped
-		elif rank ==3:
-			decomped = rank_3_tree(l,L_R,M_R)
-			coupling[M_R][rnk][lstr] = decomped
-		elif rank ==4:
-			decomped = rank_4_tree(l,L_R,M_R)
-			coupling[M_R][rnk][lstr] = decomped
-		elif rank ==5:
-			decomped = rank_5_tree(l,L_R,M_R)
-			coupling[M_R][rnk][lstr] = decomped
-		elif rank ==6:
-			decomped = rank_6_tree(l,L_R,M_R)
-			coupling[M_R][rnk][lstr] = decomped
-		elif rank ==7:
-			decomped = rank_7_tree(l,L_R,M_R)
-			coupling[M_R][rnk][lstr] = decomped
-		elif rank ==8:
-			decomped = rank_8_tree(l,L_R,M_R)
-			coupling[M_R][rnk][lstr] = decomped
-		elif rank > 8:
-			raise ValueError("Cannot generate couplings for rank %d. symmetric L_R couplings up to rank 6 have been implemented" % rank)
-	return coupling,weights
+    M_Rs = list(range(-L_R,L_R+1))
+    #generic coupling for any L_R - support must be added to call 
+    ranks = [len(l)]
+    coupling = {M_R : {rank:{} for rank in ranks} for M_R in M_Rs}
+
+    #weights are only necessary when generating linear combinations of wigner coefficients
+    weights = None
+    for M_R in M_Rs:
+        rank = len(l)
+        rnk = rank
+        lstr = ','.join([str(li) for li in l])
+        if type(l) == str:
+            l = [int(k) for k in l.split(',')]
+        if rank ==1:
+            decomped = rank_1_tree(l,L_R,M_R)
+            coupling[M_R][rnk][lstr] = decomped
+        elif rank ==2:
+            decomped = rank_2_tree(l,L_R,M_R)
+            coupling[M_R][rnk][lstr] = decomped
+        elif rank ==3:
+            decomped = rank_3_tree(l,L_R,M_R)
+            coupling[M_R][rnk][lstr] = decomped
+        elif rank ==4:
+            decomped = rank_4_tree(l,L_R,M_R)
+            coupling[M_R][rnk][lstr] = decomped
+        elif rank ==5:
+            decomped = rank_5_tree(l,L_R,M_R)
+            coupling[M_R][rnk][lstr] = decomped
+        elif rank ==6:
+            decomped = rank_6_tree(l,L_R,M_R)
+            coupling[M_R][rnk][lstr] = decomped
+        elif rank ==7:
+            decomped = rank_7_tree(l,L_R,M_R)
+            coupling[M_R][rnk][lstr] = decomped
+        elif rank ==8:
+            decomped = rank_8_tree(l,L_R,M_R)
+            coupling[M_R][rnk][lstr] = decomped
+        elif rank > 8:
+            raise ValueError("Cannot generate couplings for rank %d. symmetric L_R couplings up to rank 6 have been implemented" % rank)
+    return coupling,weights
 
 def generate_ccs():
     """
     Define and return coupling coefficients, called by AcePot initializer in potential.py
     """
     Wigner_3j = get_w3j_and_cg() # from coupling_coeffs.py
 
     import time
     t1 =time.time()
     try:
-      with open('%s/global_ccs_LR_0_MR_0.pickle' % lib_path, 'rb') as handle:
-        global_ccs = pickle.load(handle)
+        with open('%s/global_ccs_LR_0_MR_0.pickle' % lib_path, 'rb') as handle:
+            global_ccs = pickle.load(handle)
     except FileNotFoundError:
-      global_ccs_all,global_weights = get_coupling(lmax_dict_G, Wigner_3j)
-      global_ccs = global_ccs_all[0]
-      with open('%s/global_ccs_LR_0_MR_0.pickle' % lib_path, 'wb') as handle:
-        pickle.dump(global_ccs, handle, protocol=pickle.HIGHEST_PROTOCOL)
+        global_ccs_all,global_weights = get_coupling(lmax_dict_G, Wigner_3j)
+        global_ccs = global_ccs_all[0]
+        with open('%s/global_ccs_LR_0_MR_0.pickle' % lib_path, 'wb') as handle:
+            pickle.dump(global_ccs, handle, protocol=pickle.HIGHEST_PROTOCOL)
     if gen_LR1:
-      try:
-        with open('%s/global_ccs_LR_1.pickle' % lib_path, 'rb') as handle:
-          global_ccs_l1 = pickle.load(handle)
-      except FileNotFoundError:
-        global_ccs_l1,global_weights = get_coupling(lmax_dict_G, Wigner_3j, L_R=1)
-        with open('%s/global_ccs_LR_1.pickle' % lib_path, 'wb') as handle:
-          pickle.dump(global_ccs_l1, handle, protocol=pickle.HIGHEST_PROTOCOL)
-    t2 = time.time()
+        try:
+            with open('%s/global_ccs_LR_1.pickle' % lib_path, 'rb') as handle:
+                global_ccs_l1 = pickle.load(handle)
+        except FileNotFoundError:
+            global_ccs_l1,global_weights = get_coupling(lmax_dict_G, Wigner_3j, L_R=1)
+            with open('%s/global_ccs_LR_1.pickle' % lib_path, 'wb') as handle:
+                pickle.dump(global_ccs_l1, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
+    # t2 = time.time()
     #print ('Time to generate/load global generalized couplings:', (t2-t1)*1000, 'ms', '\n', 'global lmax per descriptor rank:', lmax_dict_G)
 
     return global_ccs
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py` & `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,270 +1,319 @@
-import yaml
 import itertools
 from fitsnap3lib.lib.sym_ACE.wigner_couple import *
 from fitsnap3lib.lib.sym_ACE.rpi_lib import *
 from fitsnap3lib.lib.sym_ACE.yamlpace_tools.acecoeff_tools import *
 import json
 
 
 class AcePot():
-  def __init__(self,
-        elements,
-        reference_ens,
-        ranks,
-        nmax,
-        lmax,
-        nradbase,
-        rcut,
-        lmbda,
-        rcutinner=0.0,
-        drcutinner=0.01,
-        lmin = 1,
-        RPI_heuristic='root_SO3_span',
-        **kwargs):
-    if kwargs != None:
-      self.__dict__.update(kwargs)
-    
-    self.global_ccs = generate_ccs()
-    self.E0 = reference_ens
-    self.ranks =ranks
-    self.elements = elements
-    self.betas = None
-    self.nus = None
-    self.deltaSplineBins=0.001
-    self.global_ndensity=1
-    self.global_FSparams=[1.0, 1.0]
-    self.global_rhocut = 100000
-    self.global_drhocut = 250
-    #assert the same nmax,lmax,nradbase (e.g. same basis) for each bond type
-    self.radbasetype = 'ChebExpCos'
-    self.global_nmax=nmax
-    self.global_lmax=lmax
-    assert len(nmax) == len(lmax),'nmax and lmax arrays must be same size'
-    self.global_nradbase=nradbase
-    if type(rcut) != dict and type(rcut) != list:
-      self.global_rcut = rcut
-      self.global_lmbda = lmbda
-      self.global_rcutinner = rcutinner
-      self.global_drcutinner = drcutinner
-    else:
-      self.rcut = rcut
-      self.lmbda = lmbda
-      self.rcutinner = rcutinner
-      self.drcutinner = drcutinner
-    self.RPI_heuristic = RPI_heuristic
-    self.set_embeddings()
-    self.set_bonds()
-    self.set_bond_base()
-
-    lmax_dict = {rank:lv for rank,lv in zip(self.ranks,self.global_lmax)}
-    nradmax_dict = {rank:nv for rank,nv in zip(self.ranks,self.global_nmax)}
-    mumax_dict={rank:len(self.elements) for rank in self.ranks}
-    if self.RPI_heuristic == 'lexicographic':
-      nulst_1 = [generate_nl(rank,nradmax_dict[rank],lmax_dict[rank],mumax_dict[rank]) for rank in self.ranks]
-    else:
-      nulst_1 = [descriptor_labels_YSG(rank,nradmax_dict[rank],lmax_dict[rank],mumax_dict[rank],lmin) for rank in self.ranks]
-    nus_unsort = [item for sublist in nulst_1 for item in sublist]
-    nus = nus_unsort.copy()
-    mu0s = []
-    mus =[]
-    ns = []
-    ls = []
-    for nu in nus_unsort:
-      mu0ii,muii,nii,lii = get_mu_n_l(nu)
-      mu0s.append(mu0ii)
-      mus.append(tuple(muii))
-      ns.append(tuple(nii))
-      ls.append(tuple(lii))
-    nus.sort(key = lambda x : mus[nus_unsort.index(x)],reverse = False)
-    nus.sort(key = lambda x : ns[nus_unsort.index(x)],reverse = False)
-    nus.sort(key = lambda x : ls[nus_unsort.index(x)],reverse = False)
-    nus.sort(key = lambda x : mu0s[nus_unsort.index(x)],reverse = False)
-    nus.sort(key = lambda x : len(x),reverse = False)
-    nus.sort(key = lambda x : mu0s[nus_unsort.index(x)],reverse = False)
-    self.nus = nus
-    self.set_funcs(nus)
-
-    return None
-
-
-  def set_embeddings(self,npoti='FinnisSinclair',FSparams=[1.0,1.0]):#default for linear models in lammps PACE
-    #embeddings =dict()#OrderedDict() #{ind:None for ind in range(len(self.elements))}
-    embeddings ={ind:None for ind in range(len(self.elements))}
-    for elemind in range(len(self.elements)):
-      embeddings[elemind] = {'ndensity':self.global_ndensity, 'FS_parameters':FSparams,'npoti':npoti, 'rho_core_cutoff':self.global_rhocut, 'drho_core_cutoff':self.global_drhocut}
-    self.embeddings = embeddings
-
-  def set_bonds(self):
-    bondinds=range(len(self.elements))
-    bond_lsts = [list(b) for b in itertools.product(bondinds,bondinds)]
-    self.bondlsts = bond_lsts
-
-  def set_bond_base(self):
-    bondstrs = ['[%d, %d]' %(b[0],b[1]) for b in self.bondlsts]
-    bonds = {bondstr:None for bondstr in bondstrs}
-
-    #radial basis function expansion coefficients
-    #saved in n,l,k shape
-    # defaults to orthogonal delta function [g(n,k)] basis of drautz 2019	
-    try:
-      nradmax = max(self.global_nmax[:])
-    except ValueError:
-      nradmax = max(self.global_nmax)
-    lmax= max(self.global_lmax)
-    nradbase = self.global_nradbase
-    crad = np.zeros((nradmax,lmax+1,nradbase),dtype=int)
-    for n in range(nradmax):
-      for l in range(lmax+1):
-        crad[n][l] = np.array([1 if k==n else 0 for k in range(nradbase)]) 
-
-    cnew = np.zeros((nradbase,nradmax,lmax+1))
-    for n in range(1,nradmax+1):
-      for l in range(lmax+1):
-        for k in range(1,nradbase+1):
-          cnew[k-1][n-1][l] = crad[n-1][l][k-1]
-
-    for bondind,bondlst in enumerate(self.bondlsts):
-      bstr = '[%d, %d]' %(bondlst[0],bondlst[1])
-      
-      try:
-        bonds[bstr] = {'nradmax':nradmax, 'lmax':max(self.global_lmax), 'nradbasemax':self.global_nradbase,'radbasename':self.radbasetype,'radparameters':[self.global_lmbda], 'radcoefficients':crad.tolist(), 'prehc':0, 'lambdahc':self.global_lmbda,'rcut':self.global_rcut, 'dcut':0.01, 'rcut_in':self.global_rcutinner, 'dcut_in':self.global_drcutinner, 'inner_cutoff_type':'distance'}
-      except AttributeError:
-        if type(self.rcut) == dict:
-          bonds[bstr] = {'nradmax':nradmax, 'lmax':max(self.global_lmax), 'nradbasemax':self.global_nradbase,'radbasename':self.radbasetype,'radparameters':[self.lmbda[bstr]], 'radcoefficients':crad.tolist(), 'prehc':0, 'lambdahc':self.lmbda[bstr],'rcut':self.rcut[bstr], 'dcut':0.01, 'rcut_in':self.rcutinner[bstr], 'dcut_in':self.drcutinner[bstr], 'inner_cutoff_type':'distance'}
-        elif type(self.rcut) == list:
-          bonds[bstr] = {'nradmax':nradmax, 'lmax':max(self.global_lmax), 'nradbasemax':self.global_nradbase,'radbasename':self.radbasetype,'radparameters':[self.lmbda[bondind]], 'radcoefficients':crad.tolist(), 'prehc':0, 'lambdahc':self.lmbda[bondind],'rcut':self.rcut[bondind], 'dcut':0.01, 'rcut_in':self.rcutinner[bondind], 'dcut_in':self.drcutinner[bondind], 'inner_cutoff_type':'distance'}
+    def __init__(self,
+            elements,
+            reference_ens,
+            ranks,
+            nmax,
+            lmax,
+            nradbase,
+            rcut,
+            lmbda,
+            rcutinner=0.0,
+            drcutinner=0.01,
+            lmin = 1,
+            RPI_heuristic='root_SO3_span',
+            **kwargs):
+        if kwargs != None:
+            self.__dict__.update(kwargs)
       
-    self.bonds = bonds
+        self.global_ccs = generate_ccs()
+        self.E0 = reference_ens
+        self.ranks =ranks
+        self.elements = elements
+        self.betas = None
+        self.nus = None
+        self.deltaSplineBins=0.001
+        self.global_ndensity=1
+        self.global_FSparams=[1.0, 1.0]
+        self.global_rhocut = 100000
+        self.global_drhocut = 250
+        #assert the same nmax,lmax,nradbase (e.g. same basis) for each bond type
+        self.radbasetype = 'ChebExpCos'
+        self.global_nmax=nmax
+        self.global_lmax=lmax
+        assert len(nmax) == len(lmax),'nmax and lmax arrays must be same size'
+        self.global_nradbase=nradbase
+        if type(rcut) != dict and type(rcut) != list:
+            self.global_rcut = rcut
+            self.global_lmbda = lmbda
+            self.global_rcutinner = rcutinner
+            self.global_drcutinner = drcutinner
+            self.global_lmin = lmin
+        else:
+            self.rcut = rcut
+            self.lmbda = lmbda
+            self.rcutinner = rcutinner
+            self.drcutinner = drcutinner
+            self.lmin = lmin
+        self.RPI_heuristic = RPI_heuristic
+        self.set_embeddings()
+        self.set_bonds()
+        self.set_bond_base()
 
-  def set_funcs(self,nulst=None,muflg=True,print_0s=True):
-    if nulst == None:
-      if self.nus != None:
-        nulst = self.nus.copy()
-      else:
-        raise AttributeError("No list of descriptors found/specified")
-      
-    muflg = True
-    permu0 = {b:[] for b in range(len(self.elements))}
-    permunu = {b:[] for b in range(len(self.elements))}
-    if self.betas != None:
-      betas = self.betas
-    else:
-      #betas = {ind:{nu:1.0 for nu in nulst} for ind in range(len(self.elements))}
-      betas = {ind:{} for ind in range(len(self.elements))}
-      for nu in nulst:
-        mu0,mu,n,l,L = get_mu_n_l(nu,return_L=True)
-        betas[mu0][nu] = 1.0
-    for nu in nulst:
-      mu0,mu,n,l,L = get_mu_n_l(nu,return_L=True)
-      rank = get_mu_nu_rank(nu)
-
-      llst = ['%d']*rank
-      #print (nu,l,oldfmt,muflg)
-      lstr = ','.join(b for b in llst) % tuple(l)
-      if L != None:
-        ccs = self.global_ccs[rank][lstr][tuple(L)]
-      elif L == None:
+        lmax_dict = {rank:lv for rank,lv in zip(self.ranks,self.global_lmax)}
         try:
-          ccs = self.global_ccs[rank][lstr][()]
-        except KeyError:
-          ccs = self.global_ccs[rank][lstr]
-      ms = list(ccs.keys())
-      mslsts = [[int(k) for k in m.split(',')] for m in ms]
-      msflat= [item for sublist in mslsts for item in sublist]
-      if print_0s or betas[mu0][nu] != 0.:
-        ccoeffs =  list ( np.array(list(ccs.values())) * betas[mu0][nu] )
-        permu0[mu0].append({'mu0':mu0,'rank':rank,'ndensity':self.global_ndensity,'num_ms_combs':len(ms),'mus':mu, 'ns':n,'ls':l,'ms_combs':msflat, 'ctildes':ccoeffs})
-        permunu[mu0].append(nu)
-      elif betas[mu0][nu] == 0. and not print_0s:
-        print ('Not printing descriptor: %s, coefficient is 0' % nu)
-        #ccoeffs =  list ( np.array(list(ccs.values())) * betas[mu0][nu] )
-        #permu0[mu0].append({'mu0':mu0,'rank':rank,'ndensity':self.global_ndensity,'num_ms_combs':len(ms),'mus':mu, 'ns':n,'ls':l,'ms_combs':msflat, 'ctildes':ccoeffs})
-        #permunu[mu0].append(nu)
-        
-    #for b in range(len(self.elements)):
-    #	for i in permunu[b]:
-    #		print (b,i)
-    #for b in range(len(self.elements)):
-    #	print (b,len(permu0[b]))
-    self.funcs = permu0
-    self.permunu = permunu
-
-  def set_betas(self,betas,has_zeros=False):
-    if type(betas) != dict:
-      if not has_zeros:
-        assert len(betas) == len(self.nus), "list of betas must be the same size as list of descriptors (0th order coefficient should NOT be included in this list"
-      elif has_zeros:
-        with_nu_inds = len(self.nus) + len(self.elements)
-        base_N_nu_per_ind = int(len(self.nus)/len(self.elements))
-        e0inds =[]
-        for i in range(len(self.elements)):
-          e0ind = (i*base_N_nu_per_ind)  + i 
-          e0inds.append(e0ind)
-        e0s = [betas[e0ind] for e0ind in e0inds]
-        self.E0 = e0s
-        betas = [b for i,b in enumerate(betas) if i not in e0inds]
-  
-      betas_dict = {ind:{} for ind in range(len(self.elements))}
-      for nu,beta in zip(self.nus,betas):
-        mu0,mu,n,l,L = get_mu_n_l(nu,return_L=True)
-        betas_dict[mu0][nu] = beta
-      self.betas = betas_dict
-    elif type(betas) == dict:
-      self.betas = betas
-
-  def read_acecoeff(self,name,remove_0s=False):
-    f = '%s.acecoeff' % name
-    coeff_dict = process_acepot(f,self.elements)
-    e0s = []
-    beta_dict = {mu0: {} for mu0 in range(len(self.elements))}
-    remove_keys = {mu0: [] for mu0 in range(len(self.elements))}
-    for ind,element in enumerate(self.elements):
-      for key  in coeff_dict.keys():
-        if key == '%d_0' % ind:
-          e0s.append(coeff_dict[key])
-          remove_keys[ind].append(key)
+            lmin_dict = {rank:lv for rank,lv in zip(self.ranks,self.lmin)}
+        except AttributeError:
+            lmin_dict = {rank:lv for rank,lv in zip(self.ranks,self.global_lmin*len(self.ranks))}
+        nradmax_dict = {rank:nv for rank,nv in zip(self.ranks,self.global_nmax)}
+        mumax_dict={rank:len(self.elements) for rank in self.ranks}
+        if self.RPI_heuristic == 'lexicographic':
+            nulst_1 = [generate_nl(rank,nradmax_dict[rank],lmax_dict[rank],mumax_dict[rank]) for rank in self.ranks]
         else:
-          mu0,mu,n,l = get_mu_n_l(key)
-          beta_dict[mu0][key] = coeff_dict[key]
-  
-    for ind,element in enumerate(self.elements):
-      for key in remove_keys[ind]:
+            nulst_1 = [descriptor_labels_YSG(rank,nradmax_dict[rank],lmax_dict[rank],mumax_dict[rank],lmin_dict[rank]) for rank in self.ranks]
+        nus_unsort = [item for sublist in nulst_1 for item in sublist]
+        nus = nus_unsort.copy()
+        mu0s = []
+        mus =[]
+        ns = []
+        ls = []
+        for nu in nus_unsort:
+            mu0ii,muii,nii,lii = get_mu_n_l(nu)
+            mu0s.append(mu0ii)
+            mus.append(tuple(muii))
+            ns.append(tuple(nii))
+            ls.append(tuple(lii))
+        nus.sort(key = lambda x : mus[nus_unsort.index(x)],reverse = False)
+        nus.sort(key = lambda x : ns[nus_unsort.index(x)],reverse = False)
+        nus.sort(key = lambda x : ls[nus_unsort.index(x)],reverse = False)
+        nus.sort(key = lambda x : mu0s[nus_unsort.index(x)],reverse = False)
+        nus.sort(key = lambda x : len(x),reverse = False)
+        nus.sort(key = lambda x : mu0s[nus_unsort.index(x)],reverse = False)
+        self.nus = nus
+        self.set_funcs(nus)
+
+        return None
+
+
+    def set_embeddings(self,npoti='FinnisSinclair',FSparams=[1.0,1.0]):#default for linear models in lammps PACE
+        #embeddings =dict()#OrderedDict() #{ind:None for ind in range(len(self.elements))}
+        embeddings ={ind:None for ind in range(len(self.elements))}
+        for elemind in range(len(self.elements)):
+            embeddings[elemind] = {'ndensity':self.global_ndensity,
+                                   'FS_parameters':FSparams,'npoti':npoti, 
+                                   'rho_core_cutoff':self.global_rhocut, 
+                                   'drho_core_cutoff':self.global_drhocut}
+        self.embeddings = embeddings
+
+    def set_bonds(self):
+        bondinds=range(len(self.elements))
+        bond_lsts = [list(b) for b in itertools.product(bondinds,bondinds)]
+        self.bondlsts = bond_lsts
+
+    def set_bond_base(self):
+        bondstrs = ['[%d, %d]' %(b[0],b[1]) for b in self.bondlsts]
+        bonds = {bondstr:None for bondstr in bondstrs}
+
+        #radial basis function expansion coefficients
+        #saved in n,l,k shape
+        # defaults to orthogonal delta function [g(n,k)] basis of drautz 2019   
         try:
-          del beta_dict[ind][key]
-        except KeyError:
-          pass
-
-    self.E0 = e0s
-    return beta_dict
+            nradmax = max(self.global_nmax[:])
+        except ValueError:
+            nradmax = max(self.global_nmax)
+        lmax= max(self.global_lmax)
+        nradbase = self.global_nradbase
+        crad = np.zeros((nradmax,lmax+1,nradbase),dtype=int)
+        for n in range(nradmax):
+            for l in range(lmax+1):
+                crad[n][l] = np.array([1 if k==n else 0 for k in range(nradbase)]) 
+
+        cnew = np.zeros((nradbase,nradmax,lmax+1))
+        for n in range(1,nradmax+1):
+            for l in range(lmax+1):
+                for k in range(1,nradbase+1):
+                    cnew[k-1][n-1][l] = crad[n-1][l][k-1]
+
+        for bondind,bondlst in enumerate(self.bondlsts):
+            bstr = '[%d, %d]' %(bondlst[0],bondlst[1])
+            
+            try:
+                bonds[bstr] = {'nradmax':nradmax, 
+                               'lmax':max(self.global_lmax), 
+                               'nradbasemax':self.global_nradbase,
+                               'radbasename':self.radbasetype,
+                               'radparameters':[self.global_lmbda], 
+                               'radcoefficients':crad.tolist(), 
+                               'prehc':0, 
+                               'lambdahc':self.global_lmbda,
+                               'rcut':self.global_rcut, 
+                               'dcut':0.01, 
+                               'rcut_in':self.global_rcutinner, 
+                               'dcut_in':self.global_drcutinner, 
+                               'inner_cutoff_type':'distance'}
+            except AttributeError:
+                if type(self.rcut) == dict:
+                    bonds[bstr] = {'nradmax':nradmax, 
+                                   'lmax':max(self.global_lmax), 
+                                   'nradbasemax':self.global_nradbase,
+                                   'radbasename':self.radbasetype,
+                                   'radparameters':[self.lmbda[bstr]], 
+                                   'radcoefficients':crad.tolist(), 
+                                   'prehc':0, 
+                                   'lambdahc':self.lmbda[bstr],
+                                   'rcut':self.rcut[bstr], 
+                                   'dcut':0.01, 
+                                   'rcut_in':self.rcutinner[bstr], 
+                                   'dcut_in':self.drcutinner[bstr], 
+                                   'inner_cutoff_type':'distance'}
+                elif type(self.rcut) == list:
+                    bonds[bstr] = {'nradmax':nradmax, 
+                                   'lmax':max(self.global_lmax), 
+                                   'nradbasemax':self.global_nradbase,
+                                   'radbasename':self.radbasetype,
+                                   'radparameters':[self.lmbda[bondind]], 
+                                   'radcoefficients':crad.tolist(), 
+                                   'prehc':0, 
+                                   'lambdahc':self.lmbda[bondind],
+                                   'rcut':self.rcut[bondind], 
+                                   'dcut':0.01, 
+                                   'rcut_in':self.rcutinner[bondind], 
+                                   'dcut_in':self.drcutinner[bondind], 
+                                   'inner_cutoff_type':'distance'}
+          
+        self.bonds = bonds
+
+    def set_funcs(self,nulst=None,muflg=True,print_0s=True):
+        if nulst == None:
+            if self.nus != None:
+                nulst = self.nus.copy()
+            else:
+                raise AttributeError("No list of descriptors found/specified")
+          
+        muflg = True
+        permu0 = {b:[] for b in range(len(self.elements))}
+        permunu = {b:[] for b in range(len(self.elements))}
+        if self.betas != None:
+            betas = self.betas
+        else:
+            #betas = {ind:{nu:1.0 for nu in nulst} for ind in range(len(self.elements))}
+            betas = {ind:{} for ind in range(len(self.elements))}
+            for nu in nulst:
+                mu0,mu,n,l,L = get_mu_n_l(nu,return_L=True)
+                betas[mu0][nu] = 1.0
+        for nu in nulst:
+            mu0,mu,n,l,L = get_mu_n_l(nu,return_L=True)
+            rank = get_mu_nu_rank(nu)
+
+            llst = ['%d']*rank
+            #print (nu,l,oldfmt,muflg)
+            lstr = ','.join(b for b in llst) % tuple(l)
+            if L != None:
+                ccs = self.global_ccs[rank][lstr][tuple(L)]
+            elif L == None:
+                try:
+                    ccs = self.global_ccs[rank][lstr][()]
+                except KeyError:
+                    ccs = self.global_ccs[rank][lstr]
+            ms = list(ccs.keys())
+            mslsts = [[int(k) for k in m.split(',')] for m in ms]
+            msflat= [item for sublist in mslsts for item in sublist]
+            if print_0s or betas[mu0][nu] != 0.:
+                ccoeffs =  list ( np.array(list(ccs.values())) * betas[mu0][nu] )
+                permu0[mu0].append({'mu0':mu0,
+                                    'rank':rank,
+                                    'ndensity':self.global_ndensity,
+                                    'num_ms_combs':len(ms),
+                                    'mus':mu, 
+                                    'ns':n,
+                                    'ls':l,
+                                    'ms_combs':msflat, 
+                                    'ctildes':ccoeffs})
+                permunu[mu0].append(nu)
+            elif betas[mu0][nu] == 0. and not print_0s:
+                print ('Not printing descriptor: %s, coefficient is 0' % nu)
+            
+        #for b in range(len(self.elements)):
+        #   for i in permunu[b]:
+        #       print (b,i)
+        #for b in range(len(self.elements)):
+        #   print (b,len(permu0[b]))
+        self.funcs = permu0
+        self.permunu = permunu
+
+    def set_betas(self,betas,has_zeros=False):
+        if type(betas) != dict:
+            if not has_zeros:
+                assert len(betas) == len(self.nus), "list of betas must be the same size as list of descriptors (0th order coefficient should NOT be included in this list"
+            elif has_zeros:
+                with_nu_inds = len(self.nus) + len(self.elements)
+                base_N_nu_per_ind = int(len(self.nus)/len(self.elements))
+                e0inds =[]
+                for i in range(len(self.elements)):
+                    e0ind = (i*base_N_nu_per_ind)  + i 
+                    e0inds.append(e0ind)
+                e0s = [betas[e0ind] for e0ind in e0inds]
+                self.E0 = e0s
+                betas = [b for i,b in enumerate(betas) if i not in e0inds]
         
-  def write_pot(self,name):
-    srt_nus = []
-    with open('%s.yace'%name,'w') as writeout:
-      e0lst = ['%f']*len(self.elements)
-      e0str = ', '.join(b for b in e0lst) % tuple(self.E0)
-      elemlst =['%s']*len(self.elements)
-      elemstr = ', '.join(b for b in elemlst) % tuple(self.elements)
-      writeout.write('elements: [%s] \n' % elemstr)
-      writeout.write('E0: [%s] \n' % e0str)
-      writeout.write('deltaSplineBins: %f \n' % self.deltaSplineBins)
-      writeout.write('embeddings:\n')
-      for mu0, embed in self.embeddings.items():
-        writeout.write('  %d: ' % mu0)
-        ystr = json.dumps(embed) + '\n'
-        ystr = ystr.replace('"','')
-        writeout.write(ystr)
-      writeout.write('bonds:\n')
-      bondstrs=['[%d, %d]' %(b[0],b[1]) for b in self.bondlsts]
-      for bondstr in bondstrs:
-        writeout.write('  %s: ' % bondstr)
-        bstr = json.dumps(self.bonds[bondstr]) + '\n'
-        bstr = bstr.replace('"','')
-        writeout.write(bstr)
-      writeout.write('functions:\n')
-      for mu0 in range(len(self.elements)):
-        writeout.write('  %d:\n'%(mu0))
-        mufuncs = self.funcs[mu0]
-        for mufunc in mufuncs:
-          mufuncstr = '    - ' +json.dumps(mufunc) + '\n'
-          mufuncstr = mufuncstr.replace('"','')
-          writeout.write(mufuncstr)
+            betas_dict = {ind:{} for ind in range(len(self.elements))}
+            for nu,beta in zip(self.nus,betas):
+                mu0,mu,n,l,L = get_mu_n_l(nu,return_L=True)
+                betas_dict[mu0][nu] = beta
+            self.betas = betas_dict
+        elif type(betas) == dict:
+            self.betas = betas
+
+    def read_acecoeff(self,name,remove_0s=False):
+        f = '%s.acecoeff' % name
+        coeff_dict = process_acepot(f,self.elements)
+        e0s = []
+        beta_dict = {mu0: {} for mu0 in range(len(self.elements))}
+        remove_keys = {mu0: [] for mu0 in range(len(self.elements))}
+        for ind,element in enumerate(self.elements):
+            for key  in coeff_dict.keys():
+                if key == '%d_0' % ind:
+                    e0s.append(coeff_dict[key])
+                    remove_keys[ind].append(key)
+                else:
+                    mu0,mu,n,l = get_mu_n_l(key)
+                    beta_dict[mu0][key] = coeff_dict[key]
+      
+        for ind,element in enumerate(self.elements):
+            for key in remove_keys[ind]:
+                try:
+                    del beta_dict[ind][key]
+                except KeyError:
+                    pass
+
+        self.E0 = e0s
+        return beta_dict
+          
+    def write_pot(self,name):
+        srt_nus = []
+        with open('%s.yace'%name,'w') as writeout:
+            e0lst = ['%f']*len(self.elements)
+            e0str = ', '.join(b for b in e0lst) % tuple(self.E0)
+            elemlst =['%s']*len(self.elements)
+            elemstr = ', '.join(b for b in elemlst) % tuple(self.elements)
+            writeout.write('elements: [%s] \n' % elemstr)
+            writeout.write('E0: [%s] \n' % e0str)
+            writeout.write('deltaSplineBins: %f \n' % self.deltaSplineBins)
+            writeout.write('embeddings:\n')
+            for mu0, embed in self.embeddings.items():
+                writeout.write('  %d: ' % mu0)
+                ystr = json.dumps(embed) + '\n'
+                ystr = ystr.replace('"','')
+                writeout.write(ystr)
+            writeout.write('bonds:\n')
+            bondstrs=['[%d, %d]' %(b[0],b[1]) for b in self.bondlsts]
+            for bondstr in bondstrs:
+                writeout.write('  %s: ' % bondstr)
+                bstr = json.dumps(self.bonds[bondstr]) + '\n'
+                bstr = bstr.replace('"','')
+                writeout.write(bstr)
+            writeout.write('functions:\n')
+            for mu0 in range(len(self.elements)):
+                writeout.write('  %d:\n'%(mu0))
+                mufuncs = self.funcs[mu0]
+                for mufunc in mufuncs:
+                    mufuncstr = '    - ' +json.dumps(mufunc) + '\n'
+                    mufuncstr = mufuncstr.replace('"','')
+                    writeout.write(mufuncstr)
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/parallel_tools.py` & `fitsnap3-3.0.1/fitsnap3lib/parallel_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,17 +172,19 @@
 
         if stubs == 0:
             if comm is None:
                 comm = MPI.COMM_WORLD
             self._comm = comm
             self._rank = self._comm.Get_rank()
             self._size = self._comm.Get_size()
-            self.create_shared_bool = True # set to False if want to avoid shared array
-                                           # this is helpful when using the library to loop over
-                                           # functions that create shared arrays, to avoid mem leaks
+            """
+            Set this to False if want to avoid shared arrays. This is helpful when using the library 
+            to loop over functions that create shared arrays, to avoid mem leaks.
+            """
+            self.create_shared_bool = True
 
         if stubs == 1:
             self._rank = 0
             self._size = 1
             self._comm = None
             self._sub_rank = 0
             self._sub_size = 1
@@ -528,15 +530,19 @@
                 sub_a_sizes[proc_number] += 6
 
             # if fitting to per-atom scalar, arrays are same as using per atom energies
 
             if self.fitsnap_dict["per_atom_scalar"]:
                 sub_a_sizes[proc_number] += self.shared_arrays["number_of_atoms"].array[i]
 
-        assert sum(sub_a_sizes) == len(self.shared_arrays['a'].array)
+        # This assert only works on a single node.
+        # TODO: Should be way to generalize for all nodes, take closer look at variables.
+        if self._number_of_nodes == 1:
+            assert sum(sub_a_sizes) == len(self.shared_arrays['a'].array)
+
         self.add_2_fitsnap("sub_a_size", sub_a_sizes)
         self._bcast_fitsnap("sub_a_size")
         self.fitsnap_dict["sub_a_size"] = sub_a_sizes[self._sub_rank]
 
         count = 0
         indices = np.zeros((self._sub_size, 2), dtype=int)
         for i, value in enumerate(sub_a_sizes):
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/scrapers/json_scraper.py` & `fitsnap3-3.0.1/fitsnap3lib/scrapers/json_scraper.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,75 +20,85 @@
     def scrape_groups(self):
         super().scrape_groups()
         self.configs = self.files
 
     def scrape_configs(self):
         self.files = self.configs
         self.conversions = copy(self.default_conversions)
+        data_path = self.config.sections["PATH"].datapath
         for i, file_name in enumerate(self.files):
-            with open(file_name) as file:
-                if file.readline()[0]=="{":
-                    file.seek(0)
-                try:
-                    self.data = loads(file.read(), parse_constant=True)
-                except Exception as e:
-                    output.screen("Trouble Parsing Training Data: ", file_name)
-                    output.exception(e)
-
-                assert len(self.data) == 1, "More than one object (dataset) is in this file"
-
-                self.data = self.data['Dataset']
-
-                assert len(self.data['Data']) == 1, "More than one configuration in this dataset"
-
-                self.data['Group'] = file_name.split("/")[-2]
-                self.data['File'] = file_name.split("/")[-1]
-
-                assert all(k not in self.data for k in self.data["Data"][0].keys()), \
-                    "Duplicate keys in dataset and data"
-
-                self.data.update(self.data.pop('Data')[0])  # Move data up one level
-
-                for key in self.data:
-                    if "Style" in key:
-                        if key.replace("Style", "") in self.conversions:
-                            temp = config.sections["SCRAPER"].properties[key.replace("Style", "")]
-                            temp[1] = self.data[key]
-                            self.conversions[key.replace("Style", "")] = convert(temp)
-
-                for key in config.sections["SCRAPER"].properties:
-                    if key in self.data:
-                        self.data[key] = np.asarray(self.data[key])
-
-                natoms = np.shape(self.data["Positions"])[0]
-                pt.shared_arrays["number_of_atoms"].sliced_array[i] = natoms
-                self.data["QMLattice"] = (self.data["Lattice"] * self.conversions["Lattice"]).T
-                del self.data["Lattice"]  # We will populate this with the lammps-normalized lattice.
-                if "Label" in self.data:
-                    del self.data["Label"]  # This comment line is not that useful to keep around.
-
-                if not isinstance(self.data["Energy"], float):
-                    self.data["Energy"] = float(self.data["Energy"])
-
-                # insert electronegativities, which are per-atom scalars
-
-                if (self.config.sections["CALCULATOR"].per_atom_scalar):
-                  if not isinstance(self.data["Chis"], float):
-                      self.data["Chis"] = self.data["Chis"]
-
-                # Currently, ESHIFT should be in units of your training data (note there is no conversion)
-                if hasattr(config.sections["ESHIFT"], 'eshift'):
-                    for atom in self.data["AtomTypes"]:
-                        self.data["Energy"] += config.sections["ESHIFT"].eshift[atom]
-
-                self.data["test_bool"] = self.test_bool[i]
-
-                self.data["Energy"] *= self.conversions["Energy"]
-
-                self._rotate_coords()
-                self._translate_coords()
-
-                self._weighting(natoms)
-
-                self.all_data.append(self.data)
+            if file_name.endswith('.json'):
+                with open(file_name) as file:
+                    if file.readline()[0]=="{":
+                        file.seek(0)
+                    try:
+                        self.data = loads(file.read(), parse_constant=True)
+                    except Exception as e:
+                        output.screen("Trouble Parsing Training Data: ", file_name)
+                        output.exception(e)
+
+                    assert len(self.data) == 1, "More than one object (dataset) is in this file"
+
+                    self.data = self.data['Dataset']
+
+                    assert len(self.data['Data']) == 1, "More than one configuration in this dataset"
+                    
+                    training_file = file_name.split("/")[-1]
+                    self.data['File'] = training_file
+                    group_name = file_name.replace(data_path,'').replace(training_file,'')[1:-1] 
+                    self.data['Group'] = group_name
+                    
+                    assert all(k not in self.data for k in self.data["Data"][0].keys()), \
+                        "Duplicate keys in dataset and data"
+
+                    # Move data up one level
+                    self.data.update(self.data.pop('Data')[0])  
+
+                    for key in self.data:
+                        if "Style" in key:
+                            if key.replace("Style", "") in self.conversions:
+                                temp = config.sections["SCRAPER"].properties[key.replace("Style", "")]
+                                temp[1] = self.data[key]
+                                self.conversions[key.replace("Style", "")] = convert(temp)
+
+                    for key in config.sections["SCRAPER"].properties:
+                        if key in self.data:
+                            self.data[key] = np.asarray(self.data[key])
+
+                    natoms = np.shape(self.data["Positions"])[0]
+                    pt.shared_arrays["number_of_atoms"].sliced_array[i] = natoms
+                    self.data["QMLattice"] = (self.data["Lattice"] * self.conversions["Lattice"]).T
+
+                    # Populate with LAMMPS-normalized lattice
+                    del self.data["Lattice"]  
+
+                    # TODO Check whether "Label" container useful to keep around
+                    if "Label" in self.data:
+                        del self.data["Label"] 
+
+                    if not isinstance(self.data["Energy"], float):
+                        self.data["Energy"] = float(self.data["Energy"])
+
+                    # Insert electronegativities, which are per-atom scalars
+                    if (self.config.sections["CALCULATOR"].per_atom_scalar):
+                        if not isinstance(self.data["Chis"], float):
+                            self.data["Chis"] = self.data["Chis"]
+
+                    # Currently, ESHIFT should be in units of your training data (note there is no conversion)
+                    if hasattr(config.sections["ESHIFT"], 'eshift'):
+                        for atom in self.data["AtomTypes"]:
+                            self.data["Energy"] += config.sections["ESHIFT"].eshift[atom]
+
+                    self.data["test_bool"] = self.test_bool[i]
+
+                    self.data["Energy"] *= self.conversions["Energy"]
+
+                    self._rotate_coords()
+                    self._translate_coords()
+
+                    self._weighting(natoms)
+
+                    self.all_data.append(self.data)
+            else:
+                pt.single_print("Non-json file found: ", file_name)    
 
         return self.all_data
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/scrapers/scrape.py` & `fitsnap3-3.0.1/fitsnap3lib/scrapers/scrape.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/scrapers/scraper_factory.py` & `fitsnap3-3.0.1/fitsnap3lib/scrapers/scraper_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/scrapers/vasp_scraper.py` & `fitsnap3-3.0.1/fitsnap3lib/scrapers/vasp_scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,26 @@
             self.trainshift = config.sections['TRAINSHIFT'].trainshift
             output.screen("!WARNING: 'TRAINSHIFT' is in input file!\n!WARNING: This section is used to shift (and clearly document) per-atom energies between VASP datasets.\n!WARNING: . \n!WARNING: Only use this section if you know what you're doing!")
         else:
             self.trainshift = {}
 
 
     def scrape_groups(self):
-        ### Locate all OUTCARs in datapath
+        # Locate all OUTCARs in datapath
         glob_asterisks = '/**/*'
         outcars_base = os.path.join(self.vasp_path, *glob_asterisks.split('/'))
 
-        ## TODO make this search user-specify-able (e.g., OUTCARs have labels/prefixes etc.)
+        # TODO make this search user-specify-able (e.g., OUTCARs have labels/prefixes etc.)
         all_outcars = [f for f in glob(outcars_base,recursive=True) if f.endswith('OUTCAR')]
 
-        ## Grab test|train split
+        # Grab test|train split
         self.group_dict = {k: config.sections['GROUPS'].group_types[i] for i, k in enumerate(config.sections['GROUPS'].group_sections)}
 
         for group in self.group_table:
-            ## First, check that all group folders exist
+            # First, check that all group folders exist
             group_vasp_path = f'{self.vasp_path}/{group}'
             if not os.path.exists(group_vasp_path):
                 raise Exception('!!ERROR: group folder not detected!!' 
                     '\n!!Please check that all groups in the input file have an associated group folder' 
                     f'\n!!\tInput file: {self.infile}'
                     f'\n!!\tMissing group folder: {group_vasp_path}'
                     '\n')
@@ -73,91 +73,91 @@
                 testing_size = self.group_table[group]['testing_size']
                 testing_size_type = self.group_dict['testing_size']
             else:
                 testing_size = 0
             if training_size is None:
                 raise ValueError('Please set training size for {}'.format(group))
             
-            ## Grab OUTCARS for this training group
-            ## Test filepath to be sure that unique group name is being matched
+            # Grab OUTCARS for this training group
+            # Test filepath to be sure that unique group name is being matched
             group_outcars = [f for f in all_outcars if group_vasp_path + '/' in f]
             if len(group_outcars) == 0:
                 raise Exception('!!ERROR: no OUTCARs found in group!!' 
                     '\n!!Please check that all groups in the input file have at least one file named "OUTCAR"' 
                     '\n!!in at least one subdirectory of the group folder' 
                     f'\n!!\tMissing group data root: {group_vasp_path}'
                     '\n')
 
             file_base = os.path.join(config.sections['PATH'].datapath, group)
             self.files[file_base] = group_outcars
             self.configs[group] = []  
 
             for outcar in self.files[file_base]:
-                ## Open file
+                # Open file
                 with open(outcar, 'r') as fp:
                     lines = fp.readlines()
                 nlines = len(lines)
 
-                ## Use ion loop text to partition ionic steps
+                # Use ion loop text to partition ionic steps
                 ion_loop_text = 'aborting loop'
                 start_idx_loops = [i for i, line in enumerate(lines) if ion_loop_text in line]
                 converged_list = [False if 'unconverged' in lines[i] else True for i in start_idx_loops]
                 end_idx_loops = [i for i in start_idx_loops[1:]] + [nlines]
 
-                ## Grab potcar and element info
+                # Grab potcar and element info
                 header_lines = lines[:start_idx_loops[0]]
                 potcar_list, potcar_elements, ions_per_type, is_duplicated = self.parse_outcar_header(header_lines)
 
-                ## Each config in a single OUTCAR is assigned the same
-                ## parent data (i.e. filename, potcar and ion data)
-                ## but separated for each iteration (idx loops on 'lines')
-                ## Tuple data: outcar file name str, config number int, starting line number (for debug)  int, 
-                ## potcar list, potcar elements list, number ions per element list, configuration lines list 
+                # Each config in a single OUTCAR is assigned the same
+                # parent data (i.e. filename, potcar and ion data)
+                # but separated for each iteration (idx loops on 'lines')
+                # Tuple data: outcar file name str, config number int, starting line number (for debug)  int, 
+                # potcar list, potcar elements list, number ions per element list, configuration lines list 
                 unique_configs = [(outcar, i, start_idx_loops[i], potcar_list, potcar_elements, ions_per_type, converged_list[i],
                                     lines[start_idx_loops[i]:end_idx_loops[i]])
                                     for i in range(0, len(start_idx_loops))]
                 
-                ## Avoid adding degenerate structures (for different energies) to training set
-                ## Take only final one for JSON
-                ## See 'parse_outcar_header' method, the IBRION and NSW check, for more details
+                # Avoid adding degenerate structures (for different energies) to training set
+                # Take only final one for JSON
+                # See 'parse_outcar_header' method, the IBRION and NSW check, for more details
                 if is_duplicated:
                     unique_configs = unique_configs[-1:]
 
-                ## Parse and process OUTCAR data per configuration
+                # Parse and process OUTCAR data per configuration
                 for uc in unique_configs:
                     config_dict = self.generate_config_dict(group, uc)
                     if config_dict != -1: 
                         self.configs[group].append(config_dict)
                 del lines
 
-            ## If random_sampling toggled on, shuffle training and testing data
+            # If random_sampling toggled on, shuffle training and testing data
             if config.sections["GROUPS"].random_sampling:
                 shuffle(self.configs[group], pt.get_seed)
             nconfigs = len(self.configs[group])
 
-            ## Assign configurations to train/test groups
+            # Assign configurations to train/test groups
             if training_size == 1:
                 training_configs = nconfigs
                 testing_configs = 0
             else:
                 training_configs = max(1, int(round(training_size * nconfigs)))
                 if training_configs == nconfigs:
-                    ## If training_size is not exactly 1.0, add at least 1 testing config
+                    # If training_size is not exactly 1.0, add at least 1 testing config
                     training_configs -= 1
                     testing_configs = 1
                 else:
                     testing_configs = nconfigs - training_configs
 
             if nconfigs - testing_configs - training_configs < 0:
                 raise ValueError("training configs: {} + testing configs: {} is greater than files in folder: {}".format(
                     training_configs, testing_configs, nconfigs))
 
             output.screen(f"{group}: Detected {nconfigs}, fitting on {training_configs}, testing on {testing_configs}")
 
-            ## Populate tests dictionary
+            # Populate tests dictionary
             if self.tests is None:
                 self.tests = {}
             self.tests[group] = []
 
             for i in range(testing_configs):
                 self.tests[group].append(self.configs[group].pop())
 
@@ -175,16 +175,17 @@
 
             self.data = data['Dataset']
 
             assert len(self.data['Data']) == 1, "More than one configuration in this dataset"
 
             assert all(k not in self.data for k in self.data["Data"][0].keys()), \
                 "Duplicate keys in dataset and data"
-
-            self.data.update(self.data.pop('Data')[0])  # Move self.data up one level
+            
+            # Move self.data up one level
+            self.data.update(self.data.pop('Data')[0])  
 
             for key in self.data:
                 if "Style" in key:
                     if key.replace("Style", "") in self.conversions:
                         temp = config.sections["SCRAPER"].properties[key.replace("Style", "")]
                         temp[1] = self.data[key]
                         self.conversions[key.replace("Style", "")] = convert(temp)
@@ -192,17 +193,27 @@
             for key in config.sections["SCRAPER"].properties:
                 if key in self.data:
                     self.data[key] = np.asarray(self.data[key])
 
             natoms = np.shape(self.data["Positions"])[0]
             pt.shared_arrays["number_of_atoms"].sliced_array[i] = natoms
             self.data["QMLattice"] = (self.data["Lattice"] * self.conversions["Lattice"]).T
-            del self.data["Lattice"]  # We will populate this with the lammps-normalized lattice.
+
+            # Populate with LAMMPS-normalized lattice
+            del self.data["Lattice"]  
+
+            # TODO Check whether "Label" container useful to keep around
             if "Label" in self.data:
-                del self.data["Label"]  # This comment line is not that useful to keep around.
+                del self.data["Label"] 
+
+            # TODO test this with VASP files (taken from JSON scraper)
+            # Insert electronegativities, which are per-atom scalars
+            # if (self.config.sections["CALCULATOR"].per_atom_scalar):
+            #    if not isinstance(self.data["Chis"], float):
+            #        self.data["Chis"] = self.data["Chis"]
 
             if not isinstance(self.data["Energy"], float):
                 self.data["Energy"] = float(self.data["Energy"])
 
             # Currently, ESHIFT should be in units of your training data (note there is no conversion)
             if hasattr(config.sections["ESHIFT"], 'eshift'):
                 for atom in self.data["AtomTypes"]:
@@ -220,33 +231,33 @@
             self.all_data.append(self.data)
 
         return self.all_data
 
     def generate_config_dict(self, group, outcar_config):
         """If no JSON has been created, create dictionary for each configuration contained in a single OUTCAR"""
         """Otherwise, read existing JSON (unless input file variable 'vasp_overwrite_jsons' is toggled to True)"""
-        ## TODO future: create CSV of converted files and check that (instead of loading full OUTCAR again)
+        # TODO future: create CSV of converted files and check that (instead of loading full OUTCAR again)
         config_dict = {}
         is_bad_config = False
         has_json = None
         outcar_filename, config_num, start_idx, potcar_list, potcar_elements, ions_per_type, converged, lines = outcar_config
         file_num = config_num + 1
 
-        ## JSON read/write setup
+        # JSON read/write setup
         json_path = f'{self.jsonpath}/{group}'
         json_filestem = outcar_filename.replace('/','_').replace('_OUTCAR','') #.replace(f'_{group}','')
         if converged:
             json_filename = f"{json_path}/{json_filestem}_{file_num}.json"
         else:
             if self.unconverged_label != '\'\'':
                 json_filename = f"{json_path}/{json_filestem}_{file_num}_{self.unconverged_label}.json"
             else:
                 json_filename = f"{json_path}/{json_filestem}_{file_num}.json"
 
-        ## Check if JSON was already created from this OUTCAR
+        # Check if JSON was already created from this OUTCAR
         if not os.path.exists(json_path):
             os.makedirs(json_path)
             has_json = False
         else:
             has_json = os.path.exists(json_filename)
 
         if has_json and not self.vasp_ignore_jsons:
@@ -297,113 +308,113 @@
             if not is_bad_config:
                 self.write_json(json_filename, outcar_filename, config_dict)
                 return config_dict
             else:
                 return -1
 
     def parse_outcar_config(self,lines,potcar_list,potcar_elements,ions_per_type):
-        ## Many thanks to Mary Alice Cusentino and Logan Williams for parts of the following code
-        ## Based on the VASP2JSON.py script in the 'tools' directory
-        ## LIST SECTION_MARKERS AND RELATED FUNCTIONS ARE HARD-CODED!!
-        ## DO NOT CHANGE UNLESS YOU KNOW WHAT YOU'RE DOING!!
+        # Many thanks to Mary Alice Cusentino and Logan Williams for parts of the following code
+        # Based on the VASP2JSON.py script in the 'tools' directory
+        # LIST SECTION_MARKERS AND RELATED FUNCTIONS ARE HARD-CODED!!
+        # DO NOT CHANGE UNLESS YOU KNOW WHAT YOU'RE DOING!!
         section_markers = [
             'FORCE on cell',
             'direct lattice vectors',
             'TOTAL-FORCE (eV/Angst)',
             'FREE ENERGIE OF THE ION-ELECTRON SYSTEM (eV)',
         ]
 
         section_names = [
             'stresses',
             'lattice',
             'coords & forces',
             'energie',
         ]
 
-        idx_stress_vects = 0 # 4
-        idx_lattice_vects = 1 # 5
-        idx_force_vects = 2 # 6
-        idx_energie = 3 # 7
+        idx_stress_vects = 0
+        idx_lattice_vects = 1 
+        idx_force_vects = 2 
+        idx_energie = 3
 
-        ## Index lines of file containing JSON data
+        # Index lines of file containing JSON data
         section_idxs = [None,None,None,None]
         atom_coords, atom_forces, stress_component, all_lattice, total_energie  = None, None, None, None, None
 
         list_atom_types = []
         for i, elem in enumerate(potcar_elements):
             num_repeats = ions_per_type[i]
             elem_list = [elem.strip()]*num_repeats
             list_atom_types.extend(elem_list)
         natoms = sum(ions_per_type)
 
-        ## Search entire config/ionic step to create indices for each section
+        # Search entire config/ionic step to create indices for each section
         for i, line in enumerate(lines):
             line_test = [True if sm in line else False for sm in section_markers]
             if any(line_test):
                 test_idx = [n for n, b in enumerate(line_test) if b][0]
                 section_idxs[test_idx] = i
         
-        ## If this config has any sections missing, it is incomplete, return crash
+        # If this config has any sections missing, it is incomplete, return crash
         missing_sections = [True if i == None else False for i in section_idxs]
         if any(missing_sections):
             crash_type = '4 sections'
             missing_sections_str = 'missing sections: '
             missing_sections_str += ', '.join([section_names[i] for i, b in enumerate(missing_sections) if b])
             del lines
             return (crash_type, missing_sections_str)
 
-        ## Create data dict for this config, with global information already included
+        # Create data dict for this config, with global information already included
         data = {}
-        data['AtomTypes'] = list_atom_types  ## orig in poscar, done
-        data['NumAtoms'] = natoms  ## orig in poscar, done
+        data['AtomTypes'] = list_atom_types  # orig in poscar, done
+        data['NumAtoms'] = natoms  # orig in poscar, done
 
-        ## Lattice vectors in real space
-        ## Note: index to initial lattice vector output (POSCAR) in OUTCAR has already been removed.
-        ## Actual vector starts one line after that, and has 3 lines
+        # Lattice vectors in real space
+        # Note: index to initial lattice vector output (POSCAR) in OUTCAR has already been removed.
+        # Actual vector starts one line after that, and has 3 lines
         lidx_last_lattice0 = section_idxs[idx_lattice_vects] + 1
         lidx_last_lattice1 = lidx_last_lattice0 + 3
         lines_last_lattice = lines[lidx_last_lattice0:lidx_last_lattice1]
         all_lattice = self.get_direct_lattice(lines_last_lattice)
 
-        ## Stresses
+        # Stresses
         lidx_stresses = section_idxs[idx_stress_vects] + 14
         line_stresses = lines[lidx_stresses]
         stress_component = self.get_stresses(line_stresses)
 
-        ## Atom coordinates and forces
+        # Atom coordinates and forces
         lidx_forces0 = section_idxs[idx_force_vects] + 2
         lidx_forces1 = lidx_forces0 + natoms
         lines_forces = lines[lidx_forces0:lidx_forces1]
         atom_coords, atom_forces = self.get_forces(lines_forces)
         if type(atom_coords) == str:
             crash_type = 'atom coords, atom forces'
             crash_atom_coord_line = 'found bad line: ' + atom_coords
             del lines
             return (crash_type, crash_atom_coord_line)
 
-        ## Energie WITH entropy (TOTEN)
+        # Energie WITH entropy (TOTEN)
         lidx_TOTEN = section_idxs[idx_energie] + 2
         line_TOTEN = lines[lidx_TOTEN]
         total_energie_with_entropy = self.get_energie_with_entropy(line_TOTEN)
 
-        ## Energie without entropy
+        # Energie without entropy
         lidx_energie = section_idxs[idx_energie] + 4
         line_energie = lines[lidx_energie]
         total_energie_without_entropy = self.get_energie_without_entropy(line_energie)
 
-        ## Check if we should use the default without entropy, or use TOTEN 
-        ## (when vasp_use_TOTEN = True in [GROUPS])
+        # Check if we should use the default without entropy, or use TOTEN 
+        # (when vasp_use_TOTEN = True in [GROUPS])
         if self.use_TOTEN:
             total_energie = total_energie_with_entropy
         else:
             total_energie = total_energie_without_entropy
 
-        ## Special toggled shift in energie if converting training data
+        # Special toggled shift in energie if converting training data
         if self.trainshift:
-            ## Shift energies
+            # Shift energies
             shifted_energies = [self.trainshift[element] for element in potcar_elements]
             energy_shifts = [ions_per_type[i]*shifted_energies[i] for i in range(len(potcar_elements))]
             total_energie += sum(energy_shifts)
 
         # Here is where all the data is put together since the energy value is the last
         # one listed in each configuration.  After this, all these values will be overwritten
         # once the next configuration appears in the sequence when parsing
@@ -411,39 +422,41 @@
         data['Forces'] = atom_forces
         data['Stress'] = stress_component
         data['Lattice'] = all_lattice
         data['Energy'] = total_energie
         data["computation_code"] = "VASP"
         data["pseudopotential_information"] = potcar_list
 
-        ## Clean up (othewrise we get memory errors)
+        # Clean up (othewrise we get memory errors)
         del lines
 
         return data
 
     def parse_outcar_header(self, header):
-        ## These searches replace the POSCAR and POTCAR, and can also check IBRION for AIMD runs (commented out now)
+        # These searches replace the POSCAR and POTCAR, and can also check IBRION for AIMD runs (commented out now)
         lines_potcar, lines_vrhfin, lines_ions_per_type = [], [],[]
         potcar_list, potcar_elements, ions_per_type = [], [], []
         ibrion, nsw = None, None 
         is_duplicated = False
-        ## scf: self-consistent framework - ions don't move, electrons 'moved' until convergence criterion reached
-        ## if IBRION = -1 and NSW > 0, VASP sometimes prints duplicate structures, check for this
+        # scf: self-consistent framework - ions don't move, electrons 'moved' until convergence criterion reached
+        # if IBRION = -1 and NSW > 0, VASP sometimes prints duplicate structures, check for this
 
         for line in header:
             if "VRHFIN" in line:
                 lines_vrhfin.append(line)
             elif "ions per type" in line:
                 lines_ions_per_type.append(line)
             elif "POTCAR" in line:
                 lines_potcar.append(line)
                 # Look for the ordering of the atom types - grabbing POTCAR filenames first, then atom labels separately because VASP has terribly inconsistent formatting
-                if line.split()[1:] not in potcar_list:  # VASP will have these lines in the OUTCAR twice, and we don't need to append them the second time
-                    potcar_list.append(line.split()[1:])  # each line will look something like ['PAW_PBE', 'Zr_sv_GW', '05Dec2013']
-            ## TODO add check that warns user if POSCAR elements and POTCAR order are not the same (if possible)
+                # OUTCARs have the following lines printed twice, and we don't need to append them the second time
+                if line.split()[1:] not in potcar_list:  
+                    potcar_list.append(line.split()[1:])  
+
+            # TODO add check that warns user if POSCAR elements and POTCAR order are not the same (if possible)
             elif 'IBRION' in line:
                 ibrion = self.get_ibrion(line)
             elif 'NSW' in line:
                 nsw = self.get_nsw(line)
 
         if ibrion == -1 and nsw > 0:
             output.screen('!WARNING: degenerate energies on same structure!\n'
@@ -460,17 +473,17 @@
         for line in lines_ions_per_type:
             str0 = line.replace("ions per type = ","").strip()
             ions_per_type = [int(s) for s in str0.split()]
 
         return potcar_list, potcar_elements, ions_per_type, is_duplicated
 
     def get_vrhfin(self, lines):
-        ## Scrapes vrhfin lines to get elements
-        ## These lines appear only once per element in OUTCARs
-        ## Format: VRHFIN =W: 5p6s5d
+        # Scrapes vrhfin lines to get elements
+        # These lines appear only once per element in OUTCARs
+        # Format: VRHFIN =W: 5p6s5d
         elem_list = []
         for line in lines:
             str0 = line.strip().replace("VRHFIN =", "")
             str1 = str0[:str0.find(":")]
             elem_list.append(str1)
         return elem_list
 
@@ -478,53 +491,54 @@
         ions_per_type = []
         for line in lines:
             str0 = line.replace("ions per type = ","").strip()
             ions_per_type = [int(s) for s in str0.split()]
         return ions_per_type
 
     def get_ibrion(self, line):
-        ## There should be only one of these lines (from INCAR print)
-        ## IBRION value should always be first number < 10 to appear after "="
+        # There should be only one of these lines (from INCAR print)
+        # IBRION value should always be first number < 10 to appear after "="
         line1 = line.split()
         idx_equals = line1.index("=")
         probably_ibrion = line1[idx_equals+1]
         return int(probably_ibrion)
     
     def get_nsw(self, line):
-        ## There should be only one of these lines (from INCAR print)
-        ## Format:   >NSW    =    100    number of steps for IOM
+        # There should be only one of these lines (from INCAR print)
+        # Format:   >NSW    =    100    number of steps for IOM
         line1 = line.split()
         idx_equals = line1.index("=")
         probably_nsw = line1[idx_equals+1]
         return int(probably_nsw)
 
     def get_direct_lattice(self, lines):
         lattice_coords = []
         for i in range(0, 3):
             lattice_coords.append([float(v) for v in lines[i].split()[:3]])
         return lattice_coords
 
     def get_stresses(self, line):
-        ## TODO check that we can assume symmetric stress tensors
-        ## TODO where do we set the cell type (Bravais)
+        # TODO check that we can assume symmetric stress tensors
+        # TODO where do we set the cell type (Bravais)
         columns = line.split()
         stress_xx, stress_yy, stress_zz = [float(c) for c in columns[2:5]]
         stress_xy, stress_yz, stress_zx = [float(c) for c in columns[5:8]]
         stresses = [[stress_xx, stress_xy, stress_zx],
                     [stress_xy, stress_yy, stress_yz],
                     [stress_zx, stress_yz, stress_zz]]
         return stresses
 
     def get_forces(self, lines):
         coords, forces = [], []
         try:
             [float(v) for v in lines[-1].split()[:6]]
         except:
             print('OUTCAR config did not run to completion! Discarding configuration')
-            return lines[-1],-1 ## returning faulty string for error message
+            # Return faulty string for error message
+            return lines[-1],-1 
 
         for line in lines:
             x, y, z, fx, fy, fz = [float(v) for v in line.split()[:6]]
             coords.append([x, y, z])
             forces.append([fx, fy, fz])
         return coords, forces
 
@@ -538,38 +552,39 @@
     def get_energie_with_entropy(self, line):
         energie_with_entropy = float(line.split()[4])
         return energie_with_entropy
     
     def write_json(self, json_filename, outcar_filename, config_dict):
         dt = datetime.now().strftime('%B %d %Y %I:%M%p')
 
-        ## TODO future versions, include generation metadata in JSON file
+        # TODO future versions, include generation metadata in JSON file
         comment_line = f'# Generated on {dt} from: {os.getcwd()}/{outcar_filename}'
 
-        ## Write JSON object
-        # with open(json_filename, "a+") as f: ## with comment line
-        with open(json_filename, "w") as f:
+        # Write JSON object
+        # Note: older versions of FitSNAP wrote JSONs with a leading comment line
+        # If you need that, use append mode ('a+') instead of write mode below
+        with open(json_filename, 'w') as f:
             json.dump(config_dict, f, indent=2, sort_keys=True)
         return
 
 
-## ------------------------ Ideas/plans for future versions ------------------------ ##
+# ------------------------ Ideas/plans for future versions ------------------------ #
     def scrape_incar(self):
-        ## Might be able to add this info to FitSNAP JSONs easily, will need to check compatibility
+        # Might be able to add this info to FitSNAP JSONs easily, will need to check compatibility
         pass
 
 
     def only_read_JSONs_if_OUTCAR_already_converted(self):
-        ## Many OUTCARs (esp. for AIMD) are HUGE and take a long time to parse. Design a user-friendly and elegant way to confirm that OUTCAR has already been parsed and only read available JSON data (see above)
+        # Many OUTCARs (esp. for AIMD) are HUGE and take a long time to parse. Design a user-friendly and elegant way to confirm that OUTCAR has already been parsed and only read available JSON data (see above)
         pass
 
     def check_OUTCAR_filesizes(self):
-        ## Many OUTCARs (esp. for AIMD) are HUGE and take a long time to parse. In these cases, strongly recommend to user to toggle vasp2json on, and then use JSONs only, or have an elegant way to only read available JSON data (see above)
+        # Many OUTCARs (esp. for AIMD) are HUGE and take a long time to parse. In these cases, strongly recommend to user to toggle vasp2json on, and then use JSONs only, or have an elegant way to only read available JSON data (see above)
         pass
 
     def generate_lammps_test(self):
-        ## Maybe create option where we can take scraped OUTCARs and make LAMMPS-compatible *dat files right away
+        # Maybe create option where we can take scraped OUTCARs and make LAMMPS-compatible *dat files right away
         pass
 
     def vasp_namer(self):
-        ## Tryiing to think of a clever naming scheme so that users can trace back where they got the file
+        # Trying to think of a clever naming scheme so that users can trace back where they got the file
         return
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/scrapers/xyz_scraper.py` & `fitsnap3-3.0.1/fitsnap3lib/scrapers/xyz_scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,60 +46,75 @@
         '"': '"',
         '(': ')',
         '{': '}',
         '[': ']',
     }
 
     # Make pairs and process afterwards
+    # List of characters for each entry, add a new list for new value
     kv_pairs = [
-        [[]]]  # List of characters for each entry, add a new list for new value
-    delimiter_stack = []  # push and pop closing delimiters
-    escaped = False  # add escaped sequences verbatim
+        [[]]]  
+    # push and pop closing delimiters
+    delimiter_stack = []  
+    # add escaped sequences verbatim
+    escaped = False  
 
     # parse character-by-character unless someone can do nested brackets
     # and escape sequences in a regex
     for char in string.strip():
-        if escaped:  # bypass everything if escaped
+        # bypass everything if escaped
+        if escaped:  
             kv_pairs[-1][-1].extend(['\\', char])
             escaped = False
-        elif delimiter_stack:  # inside brackets
-            if char == delimiter_stack[-1]:  # find matching delimiter
+        # inside brackets
+        elif delimiter_stack:  
+            # find matching delimiter
+            if char == delimiter_stack[-1]:  
                 delimiter_stack.pop()
             elif char in delimiters:
-                delimiter_stack.append(delimiters[char])  # nested brackets
+                # nested brackets
+                delimiter_stack.append(delimiters[char])  
             elif char == '\\':
-                escaped = True  # so escaped quotes can be ignored
+                # so escaped quotes can be ignored
+                escaped = True  
             else:
-                kv_pairs[-1][-1].append(char)  # inside quotes, add verbatim
+                # inside quotes, add verbatim
+                kv_pairs[-1][-1].append(char)  
         elif char == '\\':
             escaped = True
         elif char in delimiters:
-            delimiter_stack.append(delimiters[char])  # brackets or quotes
+            # brackets or quotes
+            delimiter_stack.append(delimiters[char])  
         elif (sep is None and char.isspace()) or char == sep:
-            if kv_pairs == [[[]]]:  # empty, beginning of string
+            # empty, beginning of string
+            if kv_pairs == [[[]]]:  
                 continue
             elif kv_pairs[-1][-1] == []:
                 continue
             else:
                 kv_pairs.append([[]])
         elif char == '=':
             if kv_pairs[-1] == [[]]:
                 del kv_pairs[-1]
-            kv_pairs[-1].append([])  # value
+            # value
+            kv_pairs[-1].append([])  
         else:
             kv_pairs[-1][-1].append(char)
 
     kv_dict = {}
 
     for kv_pair in kv_pairs:
-        if len(kv_pair) == 0:  # empty line
+        # empty line
+        if len(kv_pair) == 0:  
             continue
-        elif len(kv_pair) == 1:  # default to True
+        # default to True
+        elif len(kv_pair) == 1:  
             key, value = ''.join(kv_pair[0]), 'T'
-        else:  # Smush anything else with kv-splitter '=' between them
+        # Smush anything else with kv-splitter '=' between them
+        else:  
             key, value = ''.join(kv_pair[0]), '='.join(
                 ''.join(x) for x in kv_pair[1:])
 
         if key.lower() not in UNPROCESSED_KEYS:
             # Try to convert to (arrays of) floats, ints
             split_value = re.findall(r'[^\s,]+', value)
             try:
@@ -126,15 +141,16 @@
                     boolvalue = [str_to_bool[vpart] for vpart in
                                  re.findall(r'[^\s,]+', value)]
                     if len(boolvalue) == 1:
                         value = boolvalue[0]
                     else:
                         value = boolvalue
                 except KeyError:
-                    pass  # value is unchanged
+                    # value is unchanged
+                    pass  
 
         kv_dict[key] = value
 
     return kv_dict
 
 
 def parse_properties(prop_str):
@@ -431,17 +447,21 @@
 
                     self.data['Group'] = ".".join(filename.split("/")[-1].split(".")[:-1])
                     self.data['File'] = filename.split("/")[-1]
 
                     pt.shared_arrays["number_of_atoms"].sliced_array[i] = self.data['NumAtoms']
 
                     self.data["QMLattice"] = self.data["Lattice"] * self.conversions["Lattice"]
-                    del self.data["Lattice"]  # We will populate this with the lammps-normalized lattice.
+
+                    # Populate with LAMMPS-normalized lattice
+                    del self.data["Lattice"]  
+
+                    # TODO Check whether "Label" container useful to keep around
                     if "Label" in self.data:
-                        del self.data["Label"]  # This comment line is not that useful to keep around.
+                        del self.data["Label"]  
 
                     # possibly due to JSON, some configurations have integer energy values.
                     if not isinstance(self.data["Energy"], float):
                         # pt.print(f"Warning: Configuration {all_index}
                         # ({group_name}/{fname_end}) gives energy as an integer")
                         self.data["Energy"] = float(self.data["Energy"])
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/anl.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/anl.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,8 +74,7 @@
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
         pt = self.pt
         b = pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
-
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/ard.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/ard.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from fitsnap3lib.solvers.solver import Solver
 from fitsnap3lib.parallel_tools import ParallelTools
 from fitsnap3lib.io.input import Config
 import numpy as np
 
 
-config = Config()
-pt = ParallelTools()
+#config = Config()
+#pt = ParallelTools()
 
 
 try:
     from sklearn.linear_model import ARDRegression
 
 
     class ARD(Solver):
@@ -19,60 +19,56 @@
             self.pt = ParallelTools()
             self.config = Config()
 
         #@pt.sub_rank_zero
         def perform_fit(self):
             @self.pt.sub_rank_zero
             def decorated_perform_fit():
-                training = [not elem for elem in pt.fitsnap_dict['Testing']]
-                pt.single_print(training)
-                w = pt.shared_arrays['w'].array[training]
-                aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[training], w * pt.shared_arrays['b'].array[training]
-                if config.sections['EXTRAS'].apply_transpose:
+                training = [not elem for elem in self.pt.fitsnap_dict['Testing']]
+                w = self.pt.shared_arrays['w'].array[training]
+                aw, bw = w[:, np.newaxis] * self.pt.shared_arrays['a'].array[training], w * self.pt.shared_arrays['b'].array[training]
+
+                if  self.config.sections['EXTRAS'].apply_transpose:
                     bw = aw.T@bw
                     aw = aw.T@aw
-                # alval_small = config.sections['ARD'].alphasmall
-                alval_big = config.sections['ARD'].alphabig
-                lmbval_small = config.sections['ARD'].lambdasmall
-                # lmbval_big = config.sections['ARD'].lambdabig
-                thresh = config.sections['ARD'].threshold_lambda
-                reg = ARDRegression(n_iter=300, tol=0.001, threshold_lambda=thresh, alpha_1=alval_big, alpha_2=alval_big,
-                                    lambda_1=lmbval_small, lambda_2=lmbval_small, fit_intercept=False)
+
+                ap = (1/(np.var(bw)))
+                self.pt.single_print('inverse variance in training data: %f, logscale for threshold_lambda: %f' %(ap, (np.log10(ap))))
+
+                alval_small = self.config.sections['ARD'].alphasmall
+                alval_big = self.config.sections['ARD'].alphabig
+                lmbval_small = self.config.sections['ARD'].lambdasmall
+                lmbval_big = self.config.sections['ARD'].lambdabig
+                thresh = self.config.sections['ARD'].threshold_lambda
+                directmethod = self.config.sections['ARD'].directmethod
+                scap = self.config.sections['ARD'].scap
+                scai = self.config.sections['ARD'].scai
+                logcut = self.config.sections['ARD'].logcut
+                self.pt.single_print('automated threshold_lambda will be 10**(%f + %1.3f)' % (logcut , np.abs(np.log10(ap)) ) )
+                if directmethod:
+                    reg = ARDRegression(n_iter=1000, threshold_lambda=thresh, alpha_1=alval_big, alpha_2=alval_big,
+                                        lambda_1=lmbval_small, lambda_2=lmbval_small, fit_intercept=False)
+                elif not directmethod:
+                    reg = ARDRegression(n_iter=1000,alpha_1=scap*ap, alpha_2=scap*ap, lambda_1=ap*scai,lambda_2=ap*scai,fit_intercept=False,threshold_lambda= 10**(int(np.abs(np.log10(ap)))+logcut) )
+                else:
+                    reg = ARDRegression(n_iter=1000,alpha_1=scap*ap, alpha_2=scap*ap, lambda_1=ap*scai,lambda_2=ap*scai,fit_intercept=False,threshold_lambda= 10**(int(np.abs(np.log10(ap)))+logcut) )
+
                 reg.fit(aw, bw)
                 self.fit = reg.coef_
-                residues = reg.predict(aw) - bw
             decorated_perform_fit()
-            for key in pt.fitsnap_dict.keys():
-                pt.single_print(key,pt.fitsnap_dict[key])
-            training = [not elem for elem in pt.fitsnap_dict['Testing']]
-            w = pt.shared_arrays['w'].array[training]
-            aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[training], w * pt.shared_arrays['b'].array[training]
-            if config.sections['EXTRAS'].apply_transpose:
-                bw = aw.T@bw
-                aw = aw.T@aw
-            alval_small = config.sections['ARD'].alphasmall
-            alval_big = config.sections['ARD'].alphabig
-            lmbval_small = config.sections['ARD'].lambdasmall
-            lmbval_big = config.sections['ARD'].lambdabig
-            thresh = config.sections['ARD'].threshold_lambda
-            reg = ARDRegression(n_iter=300, tol=0.001, threshold_lambda=thresh, alpha_1=alval_big, alpha_2=alval_big,
-                                lambda_1=lmbval_small, lambda_2=lmbval_small, fit_intercept=False)
-            reg.fit(aw, bw)
-            self.fit = reg.coef_
-            residues = reg.predict(aw) - bw
-
-        def _dump_a(self):
-            np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
-
-        def _dump_x(self):
-            np.savez_compressed('x.npz', x=self.fit)
-
-        def _dump_b(self):
-            b = pt.shared_arrays['a'].array @ self.fit
-            np.savez_compressed('b.npz', b=b)
+
+    def _dump_a(self):
+        np.savez_compressed('a.npz', a=self.pt.shared_arrays['a'].array)
+
+    def _dump_x(self):
+        np.savez_compressed('x.npz', x=self.fit)
+
+    def _dump_b(self):
+        b = self.pt.shared_arrays['a'].array @ self.fit
+        np.savez_compressed('b.npz', b=b)
 
 except ModuleNotFoundError:
 
     class ARD(Solver):
 
         def __init__(self, name):
             super().__init__(name)
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/bcs.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/bcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,8 +245,7 @@
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
         b = pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
-
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/jax.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/lasso.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/opt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 from fitsnap3lib.solvers.solver import Solver
 from fitsnap3lib.parallel_tools import ParallelTools
 from fitsnap3lib.io.input import Config
+from scipy.optimize import minimize
 import numpy as np
 
+#pt = ParallelTools()
+#config = Config()
 
-config = Config()
-pt = ParallelTools()
+def distance(x, aw, bw):
+    return np.linalg.norm(np.dot(aw, x) - bw)
 
 
-try:
-    from sklearn.linear_model import Lasso
+def distance_grad(x, aw, bw):
+    # get analytical gradient:
+    return np.dot(aw.T, np.dot(aw, x) - bw)
+
+
+class OPT(Solver):
+
+    def __init__(self, name):
+        super().__init__(name)
+        self.pt = ParallelTools()
+        self.config = Config()
+
+    @self.pt.sub_rank_zero
+    def perform_fit(self):
+        @self.pt.sub_rank_zero
+        def decorated_perform_fit():
+            pt = self.pt
+            config = self.config
+            if pt.shared_arrays['configs_per_group'].testing_elements != 0:
+                testing = -1*pt.shared_arrays['configs_per_group'].testing_elements
+            else:
+                testing = len(pt.shared_arrays['w'].array)
+            w = pt.shared_arrays['w'].array[:testing]
+            aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[:testing], w * pt.shared_arrays['b'].array[:testing]
+            #        Transpose method does not work with Quadratic SNAP (why?)
+            #        We need to revisit this preconditioning of the linear problem, we can make this a bit more elegant.
+            #        Since this breaks some examples this will stay as a 'secret' feature.
+            #        Need to chat with some mathy people on how we can profile A and find good preconditioners.
+            #        Will help when we want to try gradient based linear solvers as well.
+            if config.sections['EXTRAS'].apply_transpose:
+                bw = aw.T@bw
+                aw = aw.T@aw
 
+            param_ini = np.random.randn(aw.shape[1], )
+            res = minimize(distance, param_ini, args=(aw, bw), method='BFGS', options={'gtol': 1e-13}, jac=distance_grad)
+            self.fit = res.x
+            np.save('mean.npy', self.fit)
 
-    class LASSO(Solver):
+        decorated_perform_fit()
 
-        def __init__(self, name):
-            super().__init__(name)
+    def _dump_a(self):
+        np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
 
-        @pt.sub_rank_zero
-        def perform_fit(self):
-            training = [not elem for elem in pt.fitsnap_dict['Testing']]
-            w = pt.shared_arrays['w'].array[training]
-            aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[training], w * pt.shared_arrays['b'].array[training]
-            if config.sections['EXTRAS'].apply_transpose:
-                bw = aw.T @ bw
-                aw = aw.T @ aw
-            alval = config.sections['LASSO'].alpha
-            maxitr = config.sections['LASSO'].max_iter
-            reg = Lasso(alpha=alval, fit_intercept=False, max_iter=maxitr)
-            reg.fit(aw, bw)
-            self.fit = reg.coef_
-
-        @staticmethod
-        def _dump_a():
-            np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
-
-        def _dump_x(self):
-            np.savez_compressed('x.npz', x=self.fit)
-
-        def _dump_b(self):
-            b = pt.shared_arrays['a'].array @ self.fit
-            np.savez_compressed('b.npz', b=b)
-
-except ModuleNotFoundError:
-
-    class LASSO(Solver):
-
-        def __init__(self, name):
-            super().__init__(name)
-            raise ModuleNotFoundError("No module named 'sklearn'")
+    def _dump_x(self):
+        np.savez_compressed('x.npz', x=self.fit)
+
+    def _dump_b(self):
+        b = pt.shared_arrays['a'].array @ self.fit
+        np.savez_compressed('b.npz', b=b)
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/lreg.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/lreg.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/mcmc.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/mcmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,8 +131,7 @@
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
         b = pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
-
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/merr.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/merr.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,8 +104,7 @@
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
         b = pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
-
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/network.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -493,26 +493,29 @@
 
             self.pt.single_print("Average loss over batches is", np.mean(np.asarray(train_losses_step)))
             
             self.model.write_lammps_torch(self.config.sections['NETWORK'].output_file)
             
             self.fit = None
 
-        def evaluate_configs(self, config_index=0, option = 1, evaluate_all = False, standardize_bool = True, dtype=torch.float64):
+        def evaluate_configs(self, config_idx = 0, standardize_bool = True, dtype=torch.float64, eval_device='cpu'):
             """
             Evaluates energies and forces on configs for testing purposes. 
 
             Args:
-            config_index (int): index of config to evaluate
-            option (int): 1 if evaluating energies/forces for all configs separately.
-                2 if evaluating energies/forces using the dataloader/batch procedure
-            standardize_bool (bool): True will standardize the weights. Not standardizing is useful 
-                if comparing inputs on a previously trained standardized model, such as when doing 
-                finite difference checks. 
-            dtype (torch.dtype): Optional override of the global dtype.
+                config_idx (int): Index of config to evaluate. None if evaluating all configs.
+                standardize_bool (bool): True to standardize weights, False otherwise. Useful if 
+                    comparing inputs with a previously standardized model.
+                dtype (torch.dtype): Optional override of the global dtype.
+                eval_device (torch.device): Optional device to evaluate on, defaults to CPU to
+                    prevent device mismatch when training on GPU.
+
+            Returns:
+                A tuple (energy, force) for the config given by `config_idx`. The tuple will contain 
+                lists of energy/force for each config if `config_idx` is None.
             """
 
             @self.pt.sub_rank_zero
             def decorated_evaluate_configs():
 
                 if (standardize_bool):
                     if self.config.sections['NETWORK'].save_state_input is None:
@@ -547,16 +550,94 @@
                         
                         self.model.load_state_dict(state_dict)
 
                 # only evaluate, no weight gradients
 
                 self.model.eval()
 
-                # for evaluating single configs separately
+                if (config_idx is not None):
+                    # Evaluate a single config.
+                    config = self.configs[config_idx]
+                      
+                    #positions = torch.tensor(config.positions).requires_grad_(True)
+                    positions = torch.tensor(config.x).requires_grad_(True)
+                    xneigh = torch.tensor(config.xneigh)
+                    transform_x = torch.tensor(config.transform_x)
+                    atom_types = torch.tensor(config.types).long()
+                    target = torch.tensor(config.energy).reshape(-1)
+                    # indexing 0th axis with None reshapes the tensor to be 2D for stacking later
+                    weights = torch.tensor(config.weights[None,:])
+                    target_forces = torch.tensor(config.forces)
+                    num_atoms = torch.tensor(config.natoms)
+                    neighlist = torch.tensor(config.neighlist).long()
+
+                    # convert quantities to desired dtype
+              
+                    positions = positions.to(dtype)
+                    transform_x = transform_x.to(dtype)
+                    target = target.to(dtype)
+                    weights = weights.to(dtype)
+                    target_forces = target_forces.to(dtype)
+
+                    # make indices upon which to contract per-atom energies for this config
+
+                    config_indices = torch.arange(1).long() # this usually has len(batch) as arg in dataloader
+                    indices = torch.repeat_interleave(config_indices, neighlist.size()[0]) # config indices for each pair
+                    unique_i = neighlist[:,0]
+                    unique_j = neighlist[:,1]
+                    
+                    # need to unsqueeze num_atoms to get a tensor of definable size
+
+                    (energies,forces) = self.model(positions, neighlist, transform_x, 
+                                                  indices, num_atoms.unsqueeze(0), 
+                                                  atom_types, unique_i, unique_j, self.device, dtype)
+                    
+                else:
+                    # Evaluate all configs and store energy/force in list.
+                    energies = []
+                    forces = []
+                    for config in self.configs:
+                        #positions = torch.tensor(config.positions).requires_grad_(True)
+                        positions = torch.tensor(config.x).requires_grad_(True)
+                        xneigh = torch.tensor(config.xneigh)
+                        transform_x = torch.tensor(config.transform_x)
+                        atom_types = torch.tensor(config.types).long()
+                        target = torch.tensor(config.energy).reshape(-1)
+                        # indexing 0th axis with None reshapes the tensor to be 2D for stacking later
+                        weights = torch.tensor(config.weights[None,:])
+                        target_forces = torch.tensor(config.forces)
+                        num_atoms = torch.tensor(config.natoms)
+                        neighlist = torch.tensor(config.neighlist).long()
+
+                        # convert quantities to desired dtype
+                  
+                        positions = positions.to(dtype)
+                        transform_x = transform_x.to(dtype)
+                        target = target.to(dtype)
+                        weights = weights.to(dtype)
+                        target_forces = target_forces.to(dtype)
+
+                        # make indices upon which to contract per-atom energies for this config
+
+                        config_indices = torch.arange(1).long() # this usually has len(batch) as arg in dataloader
+                        indices = torch.repeat_interleave(config_indices, neighlist.size()[0]) # config indices for each pair
+                        unique_i = neighlist[:,0]
+                        unique_j = neighlist[:,1]
+                        
+                        # need to unsqueeze num_atoms to get a tensor of definable size
 
+                        (e_model,f_model) = self.model(positions, neighlist, transform_x, 
+                                                      indices, num_atoms.unsqueeze(0), 
+                                                      atom_types, unique_i, unique_j, self.device, dtype)
+
+                        energies.append(e_model)
+                        forces.append(f_model)
+                    
+                return (energies, forces)
+                """
                 if (option==1):
 
                     if (evaluate_all):
 
                         energies_configs = []
                         forces_configs = []
                         for config in self.configs:
@@ -637,14 +718,15 @@
                                                        indices, num_atoms.unsqueeze(0), 
                                                        atom_types, unique_i, unique_j, self.device, dtype)
 
                         energies_configs.append(energies)
                         forces_configs.append(forces)
 
                         return(energies_configs, forces_configs)
+                        """
 
             (energies, forces) = decorated_evaluate_configs()
 
             return(energies, forces)
             
 except ModuleNotFoundError:
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/opt.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/ridge.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 from fitsnap3lib.solvers.solver import Solver
 from fitsnap3lib.parallel_tools import ParallelTools
 from fitsnap3lib.io.input import Config
-from scipy.optimize import minimize
+from fitsnap3lib.lib.ridge_solver.regressor import Local_Ridge
 import numpy as np
 
-#pt = ParallelTools()
-#config = Config()
-
-def distance(x, aw, bw):
-    return np.linalg.norm(np.dot(aw, x) - bw)
-
-
-def distance_grad(x, aw, bw):
-    # get analytical gradient:
-    return np.dot(aw.T, np.dot(aw, x) - bw)
 
+#config = Config()
+#pt = ParallelTools()
 
-class OPT(Solver):
+class RIDGE(Solver):
 
     def __init__(self, name):
         super().__init__(name)
         self.pt = ParallelTools()
         self.config = Config()
 
-    @self.pt.sub_rank_zero
     def perform_fit(self):
         @self.pt.sub_rank_zero
         def decorated_perform_fit():
-            pt = self.pt
-            config = self.config
-            if pt.shared_arrays['configs_per_group'].testing_elements != 0:
-                testing = -1*pt.shared_arrays['configs_per_group'].testing_elements
-            else:
-                testing = len(pt.shared_arrays['w'].array)
-            w = pt.shared_arrays['w'].array[:testing]
-            aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[:testing], w * pt.shared_arrays['b'].array[:testing]
-            #        Transpose method does not work with Quadratic SNAP (why?)
-            #        We need to revisit this preconditioning of the linear problem, we can make this a bit more elegant.
-            #        Since this breaks some examples this will stay as a 'secret' feature.
-            #        Need to chat with some mathy people on how we can profile A and find good preconditioners.
-            #        Will help when we want to try gradient based linear solvers as well.
-            if config.sections['EXTRAS'].apply_transpose:
-                bw = aw.T@bw
-                aw = aw.T@aw
-
-            param_ini = np.random.randn(aw.shape[1], )
-            res = minimize(distance, param_ini, args=(aw, bw), method='BFGS', options={'gtol': 1e-13}, jac=distance_grad)
-            self.fit = res.x
-            np.save('mean.npy', self.fit)
 
+            training = [not elem for elem in self.pt.fitsnap_dict['Testing']]
+            w = self.pt.shared_arrays['w'].array[training]
+            aw, bw = w[:, np.newaxis] * self.pt.shared_arrays['a'].array[training], w * self.pt.shared_arrays['b'].array[training]
+            if self.config.sections['EXTRAS'].apply_transpose:
+                bw = aw.T @ bw
+                aw = aw.T @ aw
+            alval = self.config.sections['RIDGE'].alpha
+            #print (self.config.sections['RIDGE'].local_solver, type(self.config.sections['RIDGE'].local_solver))
+            if not self.config.sections['RIDGE'].local_solver:
+                try:
+                    from sklearn.linear_model import Ridge
+                    reg = Ridge(alpha = alval, fit_intercept = False)
+                except ModuleNotFoundError:
+                    self.pt.single_print('Cannot find sklearn module, using local ridge solver anyway')
+                    reg = Local_Ridge(alpha = alval, fit_intercept = False)
+            elif self.config.sections['RIDGE'].local_solver:
+                reg = Local_Ridge(alpha = alval, fit_intercept = False)
+
+            reg.fit(aw, bw)
+            self.pt.single_print('printing fit: ', reg.coef_)
+            self.fit = reg.coef_
+            residues = np.matmul(aw,reg.coef_) - bw
         decorated_perform_fit()
 
-    def _dump_a(self):
-        np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
+
+    #@staticmethod
+    def _dump_a():
+        np.savez_compressed('a.npz', a= self.pt.shared_arrays['a'].array)
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
-        b = pt.shared_arrays['a'].array @ self.fit
+        b = self.pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
+
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/pytorch.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -576,144 +576,198 @@
                 #    print("Warning: FitSNAP will continue without ML-IAP")
                 
                 self.fit = None
 
             decorated_perform_fit()
 
         #@pt.sub_rank_zero
-        def evaluate_configs(self, option = 1, standardize_bool = True, dtype=torch.float64, eval_device='cpu'):
+        def evaluate_configs(self, config_idx = 0, standardize_bool = True, dtype=torch.float64, eval_device='cpu'):
             """
             Evaluates energies and forces on configs for testing purposes. 
 
             Args:
-                option (int): 1 to evaluate energies/forces for all configs separately, 2 for using 
-                    dataloader/batch procedure. Currently only 1 is implemented.
+                config_idx (int): Index of config to evaluate. None if evaluating all configs.
                 standardize_bool (bool): True to standardize weights, False otherwise. Useful if 
                     comparing inputs with a previously standardized model.
                 dtype (torch.dtype): Optional override of the global dtype.
                 eval_device (torch.device): Optional device to evaluate on, defaults to CPU to
                     prevent device mismatch when training on GPU.
+
+            Returns:
+                A tuple (energy, force) for the config given by `config_idx`. The tuple will contain 
+                lists of energy/force for each config if `config_idx` is None.
             """
 
             @self.pt.sub_rank_zero
             def decorated_evaluate_configs():
                 #self.create_datasets()
                 # Convert model to dtype
                 self.model.to(dtype)
                 # Send model to device
                 self.model.to(eval_device)
 
                 if (standardize_bool):
-                  if self.config.sections['PYTORCH'].save_state_input is None:
-
-                      # standardization
-                      # need to perform on all network types in the model
+                    if self.config.sections['PYTORCH'].save_state_input is None:
 
-                      inv_std = 1/np.std(self.pt.shared_arrays['a'].array, axis=0)
-                      mean_inv_std = np.mean(self.pt.shared_arrays['a'].array, axis=0) * inv_std
-                      state_dict = self.model.state_dict()
-
-                      # look for the first layer for all types of networks, these are keys like
-                      # network_architecture0.0.weight and network_architecture0.0.bias
-                      # for the first network, and
-                      # network_architecture1.0.weight and network_architecture0.1.bias for the next,
-                      # and so forth
-
-                      ntypes = self.num_elements
-                      num_networks = len(self.networks)
-                      keys = [*state_dict.keys()]
-                      #for t in range(0,ntypes):
-                      for t in range(0,num_networks):
-                          first_layer_weight = "network_architecture"+str(t)+".0.weight"
-                          first_layer_bias = "network_architecture"+str(t)+".0.bias"
-                          state_dict[first_layer_weight] = torch.tensor(inv_std)*torch.eye(len(inv_std))
-                          state_dict[first_layer_bias] = torch.tensor(mean_inv_std)
+                        # standardization
+                        # need to perform on all network types in the model
 
-                      # load the new state_dict with the standardized weights
-                      
-                      self.model.load_state_dict(state_dict)
+                        inv_std = 1/np.std(self.pt.shared_arrays['a'].array, axis=0)
+                        mean_inv_std = np.mean(self.pt.shared_arrays['a'].array, axis=0) * inv_std
+                        state_dict = self.model.state_dict()
+
+                        # look for the first layer for all types of networks, these are keys like
+                        # network_architecture0.0.weight and network_architecture0.0.bias
+                        # for the first network, and
+                        # network_architecture1.0.weight and network_architecture0.1.bias for the next,
+                        # and so forth
+
+                        ntypes = self.num_elements
+                        num_networks = len(self.networks)
+                        keys = [*state_dict.keys()]
+                        #for t in range(0,ntypes):
+                        for t in range(0,num_networks):
+                            first_layer_weight = "network_architecture"+str(t)+".0.weight"
+                            first_layer_bias = "network_architecture"+str(t)+".0.bias"
+                            state_dict[first_layer_weight] = torch.tensor(inv_std)*torch.eye(len(inv_std))
+                            state_dict[first_layer_bias] = torch.tensor(mean_inv_std)
+
+                        # load the new state_dict with the standardized weights
+                        
+                        self.model.load_state_dict(state_dict)
 
                 # only evaluate, no weight gradients
 
                 self.model.eval()
 
-                # for evaluating on single config:
+                # Evaluate a single config:
+
+                if (config_idx is not None):
+                    config = self.configs[config_idx]
+                    descriptors = torch.tensor(config.descriptors).requires_grad_(True)
+                    atom_types = torch.tensor(config.types).long()
+                    target = torch.tensor(config.energy).reshape(-1)
+                    # indexing 0th axis with None reshapes the tensor to be 2D for stacking later
+                    weights = torch.tensor(config.weights[None,:])
+                    num_atoms = torch.tensor(config.natoms)
+                    """
+                    target_forces = torch.tensor(config.forces)
+                    num_atoms = torch.tensor(config.natoms)
+                    dgrad = torch.tensor(config.dgrad)
+                    dbdrindx = torch.tensor(config.dgrad_indices).long()
+                    """
+                    if (self.pt.fitsnap_dict['force']):
+                        target_forces = torch.tensor(config.forces)
+                        dgrad = torch.tensor(config.dgrad)
+                        dbdrindx = torch.tensor(config.dgrad_indices).long()
+
+                        # illustrate what unique_i and unique_j are
+
+                        unique_i = dbdrindx[:,0]
+                        unique_j = dbdrindx[:,1]
+
+                        # convert quantities to desired type
 
-                if (option==1):
+                        target_forces = target_forces.to(dtype)
+                        dgrad = dgrad.to(dtype)
+                    else:
+                        target_forces = None
+                        dgrad = None
+                        dbdrindx = None
+                        unique_j = None
+                        unique_i = None
+
+                    # convert quantities to desired dtype
+              
+                    descriptors = descriptors.to(dtype)
+                    target = target.to(dtype)
+                    weights = weights.to(dtype)
+                    #target_forces = target_forces.to(dtype)
+                    #dgrad = dgrad.to(dtype)
+
+                    # make indices upon which to contract per-atom energies for this config
+
+                    config_indices = torch.arange(1).long() # this usually has len(batch) as arg in dataloader
+                    indices = torch.repeat_interleave(config_indices, num_atoms)
+                    
+                    # illustrate what unique_i and unique_j are
+
+                    #unique_i = dbdrindx[:,0]
+                    #unique_j = dbdrindx[:,1]
+
+                    (energies,forces) = self.model(descriptors, dgrad, indices, num_atoms, 
+                                                  atom_types, dbdrindx, unique_j, unique_i, 
+                                                  eval_device, dtype)
+
+                else:
+                    
+                    # Evaluate all configs.
 
-                    energies_configs = []
-                    forces_configs = []
+                    energies = []
+                    forces = []
                     for config in self.configs:
                       
                         descriptors = torch.tensor(config.descriptors).requires_grad_(True)
                         atom_types = torch.tensor(config.types).long()
                         target = torch.tensor(config.energy).reshape(-1)
                         # indexing 0th axis with None reshapes the tensor to be 2D for stacking later
                         weights = torch.tensor(config.weights[None,:])
+                        num_atoms = torch.tensor(config.natoms)
+                        """
                         target_forces = torch.tensor(config.forces)
                         num_atoms = torch.tensor(config.natoms)
                         dgrad = torch.tensor(config.dgrad)
                         dbdrindx = torch.tensor(config.dgrad_indices).long()
+                        """
+                        if (self.pt.fitsnap_dict['force']):
+                            target_forces = torch.tensor(config.forces)
+                            dgrad = torch.tensor(config.dgrad)
+                            dbdrindx = torch.tensor(config.dgrad_indices).long()
+
+                            # illustrate what unique_i and unique_j are
+
+                            unique_i = dbdrindx[:,0]
+                            unique_j = dbdrindx[:,1]
+
+                            # convert quantities to desired type
+
+                            target_forces = target_forces.to(dtype)
+                            dgrad = dgrad.to(dtype)
+                        else:
+                            target_forces = None
+                            dgrad = None
+                            dbdrindx = None
+                            unique_j = None
+                            unique_i = None
 
                         # convert quantities to desired dtype
                   
                         descriptors = descriptors.to(dtype)
                         target = target.to(dtype)
                         weights = weights.to(dtype)
-                        target_forces = target_forces.to(dtype)
-                        dgrad = dgrad.to(dtype)
+                        #target_forces = target_forces.to(dtype)
+                        #dgrad = dgrad.to(dtype)
 
                         # make indices upon which to contract per-atom energies for this config
 
                         config_indices = torch.arange(1).long() # this usually has len(batch) as arg in dataloader
                         indices = torch.repeat_interleave(config_indices, num_atoms)
 
                         # illustrate what unique_j and unique_i are
 
-                        unique_i = dbdrindx[:,0]
-                        unique_j = dbdrindx[:,1]
+                        #unique_i = dbdrindx[:,0]
+                        #unique_j = dbdrindx[:,1]
 
-                        (energies,forces) = self.model(descriptors, dgrad, indices, num_atoms, 
+                        (e_model,f_model) = self.model(descriptors, dgrad, indices, num_atoms, 
                                                       atom_types, dbdrindx, unique_j, unique_i, 
                                                       eval_device, dtype)
-                        energies_configs.append(energies)
-                        forces_configs.append(forces)
+                        energies.append(e_model)
+                        forces.append(f_model)
 
-                    return(energies_configs, forces_configs)
-
-                else:
-                    print("Other options not implemented yet, see example below")
-
-                    """
-                    for epoch in range(self.config.sections["PYTORCH"].num_epochs):
-                        print(f"----- epoch: {epoch}")
-                        start = time()
-
-                        # loop over training data
-
-                        train_losses_step = []
-                        loss = None
-                        self.model.eval() # don't calculate gradients for simple evaluating
-                        for i, batch in enumerate(self.training_loader):
-                            descriptors = batch['x'].to(self.device).requires_grad_(True)
-                            atom_types = batch['t'].to(self.device)
-                            targets = batch['y'].to(self.device) #.requires_grad_(True)
-                            target_forces = batch['y_forces'].to(self.device) #.requires_grad_(True)
-                            indices = batch['i'].to(self.device)
-                            num_atoms = batch['noa'].to(self.device)
-                            weights = batch['w'].to(self.device)
-                            dgrad = batch['dgrad'].to(self.device) #.requires_grad_(True)
-                            dbdrindx = batch['dbdrindx'].to(self.device)
-                            unique_j = batch['unique_j'].to(self.device)
-                            unique_i = batch['unique_i'].to(self.device)
-                            testing_bools = batch['testing_bools']
-                            (energies,forces) = self.model(descriptors, dgrad, indices, num_atoms, atom_types, dbdrindx, unique_j, unique_i, self.device)
-                            energies = torch.div(energies,num_atoms)
-                            print(forces)
-                    """
+                return(energies, forces)
 
             (energies,forces) = decorated_evaluate_configs()
 
             return(energies,forces)
 
 
 except ModuleNotFoundError:
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/solver.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from fitsnap3lib.io.input import Config
 from fitsnap3lib.parallel_tools import ParallelTools
 import numpy as np
 from pandas import DataFrame, Series, concat
+import pickle
 
 #pt = ParallelTools()
 #config = Config()
 
 class Solver:
     """
     This class declares the method to solve the machine learning problem, e.g. linear regression,
@@ -106,16 +107,20 @@
     def error_analysis(self):
         """
         Extracts and stores fitting data, such as descriptor values, truths, and predictions, into
         a Pandas dataframe.
         """
         @self.pt.rank_zero
         def decorated_error_analysis():
-            if not self.linear:
-                import torch
+            
+            # Proceed with nonlinear error analysis, if doing a fit.
+            # If doing a fit, then self.configs is not None.
+
+            if not self.linear and self.configs is not None:
+                import torch # Needed to declare dtype. TODO: Move this into NN evaluate function.
                 mae_f = {} # Force MAE of each group, train and test.
                 mae_e = {} # Test energy MAE of each group, train and test.
                 rmse_f = {} # Test force RMSE of each group, train and test.
                 rmse_e = {} # Test energy RMSE of each group, train and test.
 
                 count_train = {} # Nested dictionary with number of configs and atoms per group for training data.
                 count_test = {} # Nested dictionary with number of configs and atoms per group for testing data.
@@ -150,32 +155,29 @@
                 count_test['*ALL'] = {}
                 count_test['*ALL']["nconfigs"] = 0 # Total number test configs in group.
                 count_test['*ALL']["natoms"] = 0 # Total number test atoms in group.
                 count_train['*ALL'] = {}
                 count_train['*ALL']["nconfigs"] = 0 # Total number test configs in group.
                 count_train['*ALL']["natoms"] = 0 # Total number test atoms in group.
 
-                # Evaluate errors with float64 dtype since this is what we use in production.
-
-                if (self.config.sections["CALCULATOR"].calculator == "LAMMPSCUSTOM"):
-                    (energies_model, forces_model) = self.evaluate_configs(option=1, evaluate_all = True, standardize_bool=False, dtype=torch.float64)
-                else:
-                    (energies_model, forces_model) = self.evaluate_configs(option=1, standardize_bool=False, dtype=torch.float64)
                 if (self.config.sections["EXTRAS"].dump_peratom):
                     fha = open(self.config.sections["EXTRAS"].peratom_file, 'w')
                     line = f"Filename Group AtomID Type Fx_Truth Fy_Truth Fz_Truth Fx_Pred Fy_Pred Fz_Pred Testing_Bool"
                     fha.write(line + "\n")
                 if (self.config.sections["EXTRAS"].dump_perconfig):
                     fhc = open(self.config.sections["EXTRAS"].perconfig_file, 'w')
                     line = f"Filename Group Natoms Energy_Truth Energy_Pred Testing_Bool"
                     fhc.write(line + "\n")
                 atom_indx = 0
                 m = 0
-                for c in self.configs:
-                    e_pred = energies_model[m].detach().numpy()/c.natoms # Model per-atom energy.
+                for idx, c in enumerate(self.configs):
+                    (energies_model, forces_model) = self.evaluate_configs(config_idx=idx, \
+                                                                           standardize_bool=False, \
+                                                                           dtype=torch.float64)
+                    e_pred = energies_model.detach().numpy()/c.natoms # Model per-atom energy.
                     # Custom networks need a further index.
                     if (self.config.sections["CALCULATOR"].calculator == "LAMMPSCUSTOM"):
                         e_pred = e_pred[0]
 
                     ae = abs(c.energy - e_pred)
                     se = (c.energy - e_pred)**2
                     
@@ -190,60 +192,60 @@
                         mae_e[c.group]["train"] += ae
                         rmse_e[c.group]["train"] += se
                         count_train[c.group]["nconfigs"] += 1
                         mae_e['*ALL']["train"] += ae
                         rmse_e['*ALL']["train"] += se
                         count_train['*ALL']["nconfigs"] += 1
 
-                    f_pred = forces_model[m].detach().numpy()
-                    # Custom calculator returns Nx3 force array but we need 3*N here.
-                    if (self.config.sections["CALCULATOR"].calculator == "LAMMPSCUSTOM"):
-                        f_pred = f_pred.flatten()
-
-
                     if (self.config.sections["EXTRAS"].dump_perconfig):
                         line = f"{c.filename} {c.group} {c.natoms} {c.energy} {e_pred} {c.testing_bool}\n"
                         fhc.write(line)
-                    for i in range(c.natoms):
-                        fx_truth = c.forces[3*i+0]
-                        fy_truth = c.forces[3*i+1]
-                        fz_truth = c.forces[3*i+2]
-                        fx_pred = f_pred[3*i+0]
-                        fy_pred = f_pred[3*i+1]
-                        fz_pred = f_pred[3*i+2]
-
-                        ae = abs(fx_truth - fx_pred) + \
-                             abs(fy_truth - fy_pred) + \
-                             abs(fz_truth - fz_pred)
-                        se = ((fx_truth - fx_pred)**2 + \
-                              (fy_truth - fy_pred)**2 + \
-                              (fz_truth - fz_pred)**2)
-
-                        if (c.testing_bool):
-                            mae_f[c.group]["test"] += ae
-                            rmse_f[c.group]["test"] += se
-                            count_test[c.group]["natoms"] += 1
-                            mae_f['*ALL']["test"] += ae
-                            rmse_f['*ALL']["test"] += se
-                            count_test['*ALL']["natoms"] += 1
-                        else:
-                            mae_f[c.group]["train"] += ae
-                            rmse_f[c.group]["train"] += se
-                            count_train[c.group]["natoms"] += 1
-                            mae_f['*ALL']["train"] += ae
-                            rmse_f['*ALL']["train"] += se
-                            count_train['*ALL']["natoms"] += 1
-                        
-                        if (self.config.sections["EXTRAS"].dump_peratom):
-                            line = f"{c.filename} {c.group} {i+1} {int(c.types[i]+1)} "
-                            line += f"{fx_truth} {fy_truth} {fz_truth} "
-                            line += f"{fx_pred} {fy_pred} {fz_pred} "
-                            line += f"{c.testing_bool}"
-                            fha.write(line + "\n")
-                        atom_indx += 1
+
+                    if (forces_model is not None):
+                        f_pred = forces_model.detach().numpy()
+                        # Custom calculator returns Nx3 force array but we need 3*N here.
+                        if (self.config.sections["CALCULATOR"].calculator == "LAMMPSCUSTOM"):
+                            f_pred = f_pred.flatten()
+                        for i in range(c.natoms):
+                            fx_truth = c.forces[3*i+0]
+                            fy_truth = c.forces[3*i+1]
+                            fz_truth = c.forces[3*i+2]
+                            fx_pred = f_pred[3*i+0]
+                            fy_pred = f_pred[3*i+1]
+                            fz_pred = f_pred[3*i+2]
+
+                            ae = abs(fx_truth - fx_pred) + \
+                                abs(fy_truth - fy_pred) + \
+                                abs(fz_truth - fz_pred)
+                            se = ((fx_truth - fx_pred)**2 + \
+                                  (fy_truth - fy_pred)**2 + \
+                                  (fz_truth - fz_pred)**2)
+
+                            if (c.testing_bool):
+                                mae_f[c.group]["test"] += ae
+                                rmse_f[c.group]["test"] += se
+                                count_test[c.group]["natoms"] += 1
+                                mae_f['*ALL']["test"] += ae
+                                rmse_f['*ALL']["test"] += se
+                                count_test['*ALL']["natoms"] += 1
+                            else:
+                                mae_f[c.group]["train"] += ae
+                                rmse_f[c.group]["train"] += se
+                                count_train[c.group]["natoms"] += 1
+                                mae_f['*ALL']["train"] += ae
+                                rmse_f['*ALL']["train"] += se
+                                count_train['*ALL']["natoms"] += 1
+                            
+                            if (self.config.sections["EXTRAS"].dump_peratom):
+                                line = f"{c.filename} {c.group} {i+1} {int(c.types[i]+1)} "
+                                line += f"{fx_truth} {fy_truth} {fz_truth} "
+                                line += f"{fx_pred} {fy_pred} {fz_pred} "
+                                line += f"{c.testing_bool}"
+                                fha.write(line + "\n")
+                            atom_indx += 1
                     m += 1
                 if (self.config.sections["EXTRAS"].dump_perconfig):
                     fhc.close()
                 if (self.config.sections["EXTRAS"].dump_peratom):
                     fha.close()
 
                 # Normalize to get average errors.
@@ -280,17 +282,42 @@
                     rmse_e[group]["test"]  /= count_test[group]["nconfigs"]  if count_test[group]["nconfigs"]  > 0  else np.nan
                     rmse_e[group]["test"]   = np.sqrt(rmse_e[group]["test"])
                     rmse_e[group]["train"] /= count_train[group]["nconfigs"] if count_train[group]["nconfigs"] > 0  else np.nan
                     rmse_e[group]["train"]  = np.sqrt(rmse_e[group]["train"])
 
                 self.errors = (mae_f, mae_e, rmse_f, rmse_e, count_train, count_test)
 
+                # Write pickled list of configs.
+
+                if self.config.sections["EXTRAS"].dump_configs:
+                    configs_file = self.config.sections['EXTRAS'].configs_file
+                    with open(configs_file, 'wb') as f:
+                        pickle.dump(self.configs, f)
+
+                return
+            
+            # If nonlinear and not doing a fit, just create configs.
+
+            elif not self.linear and self.configs is None:
+                
+                # Create list of Configuration objects.
+                
+                self.create_datasets()
+                
+                # Save a pickled list of Configuration objects.
+
+                if self.config.sections["EXTRAS"].dump_configs:
+                    configs_file = self.config.sections['EXTRAS'].configs_file
+                    with open(configs_file, 'wb') as f:
+                        pickle.dump(self.configs, f)
+
                 return
 
-            # collect remaining arrays to write dataframe
+            # Proceed with linear error analysis.
+            # Collect remaining arrays to write dataframe.
 
             self.df = DataFrame(self.pt.shared_arrays['a'].array)
             self.df['truths'] = self.pt.shared_arrays['b'].array.tolist()
             if self.fit is not None:
                 self.df['preds'] = self.pt.shared_arrays['a'].array @ self.fit
             self.df['weights'] = self.pt.shared_arrays['w'].array.tolist()
             for key in self.pt.fitsnap_dict.keys():
@@ -298,18 +325,19 @@
                     len(self.pt.fitsnap_dict[key]) == len(self.df.index):
                     self.df[key] = self.pt.fitsnap_dict[key]
             if self.config.sections["EXTRAS"].dump_dataframe:
                 self.df.to_pickle(self.config.sections['EXTRAS'].dataframe_file)
 
             # proceed with error analysis if doing a fit
 
-            if self.fit is not None:
+            if self.fit is not None and not self.config.sections["SOLVER"].true_multinode:
 
                 # return data for each group
-
+                #print(f"^^^ {self.pt._rank}")
+                #print(self.df)
                 grouped = self.df.groupby(['Groups', \
                     'Testing', \
                     'Row_Type']).apply(self._ncount_mae_rmse_rsq_unweighted_and_weighted)
 
                 # reformat the weighted and unweighted data into separate rows
 
                 grouped = concat({'Unweighted':grouped[['ncount', 'mae', 'rmse', 'rsq']], \
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/solver_factory.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/solver_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from fitsnap3lib.parallel_tools import ParallelTools
 from fitsnap3lib.solvers.solver import Solver
 from fitsnap3lib.solvers.ard import ARD
 from fitsnap3lib.solvers.jax import JAX
 from fitsnap3lib.solvers.lasso import LASSO
+from fitsnap3lib.solvers.ridge import RIDGE
 from fitsnap3lib.solvers.pytorch import PYTORCH
 from fitsnap3lib.solvers.scalapack import ScaLAPACK
 from fitsnap3lib.solvers.svd import SVD
 from fitsnap3lib.solvers.tensorflowsvd import TensorflowSVD
 from fitsnap3lib.solvers.anl import ANL
 from fitsnap3lib.solvers.merr import MERR
 from fitsnap3lib.solvers.network import NETWORK
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/svd.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/svd.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/solvers/tensorflowsvd.py` & `fitsnap3-3.0.1/fitsnap3lib/solvers/tensorflowsvd.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/tools/dataframe_tools.py` & `fitsnap3-3.0.1/fitsnap3lib/tools/dataframe_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/tools/dataloaders.py` & `fitsnap3-3.0.1/fitsnap3lib/tools/dataloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import torch.utils.data
-from torch.utils.data import DataLoader
 from sys import float_info
 import numpy as np
-import itertools, operator
-
+from torch.utils.data import DataLoader
 
 class InRAMDataset(torch.utils.data.Dataset):
     """
     Parent class for storing and shuffling data, depending on the specific solver used. Child 
     classes are InRAMDatasetPyTorch and InRAMDatasetJAX, which process the list of Configuration 
     objects appropriately for their own solver methods.
     """
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/tools/lammps_tools.py` & `fitsnap3-3.0.1/fitsnap3lib/tools/lammps_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 import numpy as np
-import pandas as pd
 from itertools import compress
 import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
 from fitsnap3lib.parallel_tools import ParallelTools
 from fitsnap3lib.io.input import Config
 
 SMALL_SIZE = 10
 MEDIUM_SIZE = 12
 BIGGER_SIZE = 12
 plt.rc('font', size=SMALL_SIZE)          # controls default text sizes
@@ -54,26 +52,23 @@
         from fitsnap3lib.fitsnap import FitSnap
         self.snap = FitSnap()
 
         # scrape the configs
 
         self.snap.scrape_configs()
 
-        # 
-
     def calc_mae(self, arr1, arr2):
         arr1 = np.array(arr1)
         arr2 = np.array(arr2)
         abs_diff = np.abs(arr1-arr2)
         mae = np.mean(abs_diff)
         return mae
 
     def calculate(self):
-        from fitsnap3lib.calculators.lammps_snap import LammpsSnap, _extract_compute_np
-        from fitsnap3lib.calculators.lammps_snap import _extract_compute_np
+        from fitsnap3lib.calculators.lammps_snap import LammpsSnap
         calc = LammpsSnap(name='LAMMPSSNAP')
         calc.shared_index = self.snap.calculator.shared_index
 
         energies_all = []
         forces_all = []
         energies_test_all = []
         forces_test_all = []
@@ -150,9 +145,8 @@
             preds = list(compress(forces_all, group_mask))
             truths = list(compress(forces_test_all, group_mask))
 
             mae_forces = self.calc_mae(preds, truths)
 
             errors[group]["mae_force"]=mae_forces
 
-        return errors
-
+        return errors
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/tools/nn_tools.py` & `fitsnap3-3.0.1/fitsnap3lib/tools/nn_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import numpy as np
 import pandas as pd
-from itertools import compress
 import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
 
 SMALL_SIZE = 10
 MEDIUM_SIZE = 12
 BIGGER_SIZE = 12
 plt.rc('font', size=SMALL_SIZE)          # controls default text sizes
 plt.rc('axes', titlesize=SMALL_SIZE)     # fontsize of the axes title
 plt.rc('axes', labelsize=MEDIUM_SIZE)    # fontsize of the x and y labels
@@ -168,8 +166,8 @@
             # Plot absolute error vs. target magnitude.
             plt.plot(abs(true_train), abs(true_train-pred_train), 'bo', markersize=5)
             plt.plot(abs(true_test), abs(true_test-pred_test), 'ro', markersize=5)
             plt.legend(["Train", "Validation"])
             plt.xlabel(xlabel)
             plt.ylabel(ylabel)
             plt.savefig(filename, dpi=500)
-            plt.clf()
+            plt.clf()
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/tools/test_tools.py` & `fitsnap3-3.0.1/fitsnap3lib/tools/test_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-import os
 import numpy as np
-import pandas as pd
-import random
 import torch
-from itertools import compress
 import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 
 SMALL_SIZE = 10
 MEDIUM_SIZE = 12
 BIGGER_SIZE = 12
 plt.rc('font', size=SMALL_SIZE)          # controls default text sizes
 plt.rc('axes', titlesize=SMALL_SIZE)     # fontsize of the axes title
 plt.rc('axes', labelsize=MEDIUM_SIZE)    # fontsize of the x and y labels
@@ -34,21 +27,21 @@
         option for which test to run, e.g. "FiniteDifference"
     
     """
     def __init__(self, input_script):
 
         # import parallel tools and create pt object
         from fitsnap3lib.parallel_tools import ParallelTools
-        #pt = ParallelTools(comm=comm)
+        # pt = ParallelTools(comm=comm)
         self.pt = ParallelTools()
         # don't check for existing fitsnap objects since we'll be overwriting things
         self.pt.check_fitsnap_exist = False
         from fitsnap3lib.io.input import Config
-        #fitsnap_in = "../examples/Ta_Pytorch_NN/Ta-example.in"
-        #fitsnap_in = "Ta-example.in" #ta_example_file.as_posix()
+        # fitsnap_in = "../examples/Ta_Pytorch_NN/Ta-example.in"
+        # fitsnap_in = "Ta-example.in" #ta_example_file.as_posix()
         self.config = Config(arguments_lst = [input_script, "--overwrite"])
 
     def finite_difference(self, group, config_index=0):
         """
         Calculate finite difference forces for the given group, and compare with model forces.
 
         Attributes
@@ -56,109 +49,101 @@
 
         config_index: int
             index of configuration to test finite difference on
         """
 
         h = 1e-4 # size of finite difference
 
-        #config.sections['BISPECTRUM'].switchflag = 1 # required for smooth finite difference
+        # config.sections['BISPECTRUM'].switchflag = 1 # required for smooth finite difference
         self.config.sections['NETWORK'].manual_seed_flag = 1
         self.config.sections['NETWORK'].dtype = torch.float64
         # only perform calculations on displaced BCC structures
-        self.config.sections['GROUPS'].group_table = {group: \
-            {'training_size': 1.0, \
-            'testing_size': 0.0, \
-            'eweight': 100.0, \
-            'fweight': 1.0, \
-            'vweight': 1e-08}}
+        self.config.sections['GROUPS'].group_table = {group:
+                                                     {'training_size': 1.0,
+                                                      'testing_size': 0.0,
+                                                      'eweight': 100.0,
+                                                      'fweight': 1.0,
+                                                      'vweight': 1e-08}}
         # create a fitsnap object
         from fitsnap3lib.fitsnap import FitSnap
         self.snap = FitSnap()
 
         # get config positions
         self.snap.scrape_configs()
         # don't delete the data since we'll use it many times with finite difference
         self.snap.delete_data = False 
 
         # calculate model forces
 
         self.snap.process_configs()
         self.pt.all_barrier()
         self.snap.solver.create_datasets()
-        (energies_model, forces_model) = self.snap.solver.evaluate_configs(option=1, evaluate_all=True, standardize_bool=True)
+        (energies_model, forces_model) = self.snap.solver.evaluate_configs(config_idx=None, standardize_bool=True)
 
         start_indx = config_index
 
         assert (start_indx < len(self.snap.data)-1)
 
         errors = []
         for m in range(start_indx,start_indx+1):
             for i in range(0,self.snap.data[m]['NumAtoms']):
-                  for a in range(0,3):
-                      natoms = self.snap.data[m]['NumAtoms']
+                for a in range(0,3):
+                    # natoms = self.snap.data[m]['NumAtoms']
+                    # calculate model energy with +h (energy1)
+
+                    self.snap.data[m]['Positions'][i,a] += h
+                    self.snap.calculator.distributed_index = 0
+                    self.snap.calculator.shared_index = 0
+                    self.snap.calculator.shared_index_b = 0
+                    self.snap.calculator.shared_index_c = 0
+                    self.snap.calculator.shared_index_dgrad = 0
+                    self.snap.process_configs()
+                    self.snap.solver.create_datasets()
+                    (energies1, forces1) = self.snap.solver.evaluate_configs(config_idx=m, standardize_bool=False)
+
+                    # calculate model energy with -h (energy2)
+
+                    self.snap.data[m]['Positions'][i,a] -= 2.*h
+                    #print(f"position: {snap.data[m]['Positions'][i,a]}")
+                    self.snap.calculator.distributed_index = 0
+                    self.snap.calculator.shared_index = 0
+                    self.snap.calculator.shared_index_b = 0
+                    self.snap.calculator.shared_index_c = 0
+                    self.snap.calculator.shared_index_dgrad = 0
+                    self.snap.process_configs()
+                    self.snap.solver.create_datasets()
+                    (energies2, forces2) = self.snap.solver.evaluate_configs(config_idx=m, standardize_bool=False)
+
+                    # calculate and compare finite difference force
+
+                    force_fd = -1.0*(energies1[0] - energies2[0])/(2.*h)
+                    force_fd = force_fd.item()
+                    force_model = forces_model[m][i][a].item()
+
+                    error = force_model - force_fd
+                    if (abs(error) > 1e-1):
+                        print(f"m i a f_fd f_model: {m} {i} {a} {force_fd} {force_model}")
+                        assert(False)
+                    errors.append(error)
 
-                      # calculate model energy with +h (energy1)
+                    # return position back to normal
 
-                      self.snap.data[m]['Positions'][i,a] += h
-                      #print(f"position: {snap.data[m]['Positions'][i,a]}")
-                      self.snap.calculator.distributed_index = 0
-                      self.snap.calculator.shared_index = 0
-                      self.snap.calculator.shared_index_b = 0
-                      self.snap.calculator.shared_index_c = 0
-                      self.snap.calculator.shared_index_dgrad = 0
-                      self.snap.process_configs()
-                      self.snap.solver.create_datasets()
-                      (energies1, forces1) = self.snap.solver.evaluate_configs(config_index=m, option=1, standardize_bool=False)
-
-                      # calculate model energy with -h (energy2)
-
-                      self.snap.data[m]['Positions'][i,a] -= 2.*h
-                      #print(f"position: {snap.data[m]['Positions'][i,a]}")
-                      self.snap.calculator.distributed_index = 0
-                      self.snap.calculator.shared_index = 0
-                      self.snap.calculator.shared_index_b = 0
-                      self.snap.calculator.shared_index_c = 0
-                      self.snap.calculator.shared_index_dgrad = 0
-                      self.snap.process_configs()
-                      self.snap.solver.create_datasets()
-                      (energies2, forces2) = self.snap.solver.evaluate_configs(config_index=m, option=1, standardize_bool=False)
-
-                      # calculate and compare finite difference force
-
-                      force_fd = -1.0*(energies1[0] - energies2[0])/(2.*h)
-                      force_fd = force_fd.item()
-                      force_model = forces_model[m][i][a].item()
-
-                      error = force_model - force_fd
-                      if (abs(error) > 1e-1):
-                          print(f"m i a f_fd f_model: {m} {i} {a} {force_fd} {force_model}")
-                          assert(False)
-                      errors.append(error)
-
-                      # return position back to normal
-
-                      self.snap.data[m]['Positions'][i,a] += h
+                    self.snap.data[m]['Positions'][i,a] += h
 
         mean_err = np.mean(np.abs(errors))
         max_err = np.max(np.abs(errors))
 
         print(f"mean max: {mean_err} {max_err}")
 
         errors = np.abs(errors)
-        
+
         hist, bins = np.histogram(errors, bins=10)
         logbins = np.logspace(np.log10(bins[0]),np.log10(bins[-1]),len(bins))
         plt.hist(errors, bins=logbins)
         plt.xscale('log')
         plt.xlim((1e-12,1e4))
         plt.xlabel(r'Absolute difference (eV/$\AA$)')
         plt.ylabel("Distribution")
         plt.yticks([])
         plt.savefig("fd-force-check.png", dpi=500)
-        
-
-        assert(mean_err < 0.001 and max_err < 0.1)
 
-        #del pt
-        #del config
-        #del snap.data
-        #del snap
+        assert (mean_err < 0.001 and max_err < 0.1)
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/units/conversion_finder.py` & `fitsnap3-3.0.1/fitsnap3lib/units/conversion_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,9 +46,8 @@
         raise AttributeError("{} was not found in unit type {}".format(unit_a, a_unit_type))
 
     try:
         denominator = getattr(the_unit_type, unit_b)
     except AttributeError:
         raise AttributeError("{} was not found in unit type {}".format(unit_b, a_unit_type))
 
-    return numerator/denominator
-
+    return numerator/denominator
```

### Comparing `fitsnap3-3.0.0.1/fitsnap3lib/units/units.py` & `fitsnap3-3.0.1/fitsnap3lib/units/units.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.0.1/pyproject.toml` & `fitsnap3-3.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
-#requires = ['setuptools>=42', 'numpy', 'scipy', 'scikit-learn', 'virtualenv', 'psutil', 'pandas', 'tabulate', 'mpi4py', 'Cython', 'torch', 'sympy', 'pyyaml']
 requires = [
     "setuptools>=42",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "fitsnap3"
-version = "3.0.0.1"
+version = "3.0.1"
 description = "Molecular Machine Learning Interface"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `fitsnap3-3.0.0.1/tests/test_examples.py` & `fitsnap3-3.0.1/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-import sys
 from pathlib import Path
 import os
 import importlib.util
 
 
 """Resolve Pathing and load ExampleChecker"""
 this_path = Path(__file__).parent.resolve()
```

### Comparing `fitsnap3-3.0.0.1/tests/test_pytorch.py` & `fitsnap3-3.0.1/tests/test_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,65 +54,64 @@
     snap.delete_data = False 
 
     # calculate model forces
 
     snap.process_configs()
     pt.all_barrier()
     snap.solver.create_datasets()
-    (energies_model, forces_model) = snap.solver.evaluate_configs(option=1, standardize_bool=True)
+    (energies_model, forces_model) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=True)
 
     print(f"Length of data: {len(snap.data)}")
 
     # chose a random config to test against
 
     random_indx = 0 #random.randint(0, len(snap.data)-1)
 
     percent_errors = []
     for m in range(random_indx,random_indx+1):
         for i in range(0,snap.data[m]['NumAtoms']):
-        #for i in range(0,1):
-              for a in range(0,3):
-                  natoms = snap.data[m]['NumAtoms']
-
-                  # calculate model energy with +h (energy1)
-
-                  snap.data[m]['Positions'][i,a] += h
-                  snap.calculator.distributed_index = 0
-                  snap.calculator.shared_index = 0
-                  snap.calculator.shared_index_b = 0
-                  snap.calculator.shared_index_c = 0
-                  snap.calculator.shared_index_dgrad = 0
-                  snap.process_configs()
-                  snap.solver.create_datasets()
-                  (energies1, forces1) = snap.solver.evaluate_configs(option=1, standardize_bool=False)
-
-                  # calculate model energy with -h (energy2)
-
-                  snap.data[m]['Positions'][i,a] -= 2.*h
-                  snap.calculator.distributed_index = 0
-                  snap.calculator.shared_index = 0
-                  snap.calculator.shared_index_b = 0
-                  snap.calculator.shared_index_c = 0
-                  snap.calculator.shared_index_dgrad = 0
-                  snap.process_configs()
-                  snap.solver.create_datasets()
-                  (energies2, forces2) = snap.solver.evaluate_configs(option=1, standardize_bool=False)
-
-                  # calculate and compare finite difference force
-
-                  force_fd = -1.0*(energies1[m] - energies2[m])/(2.*h)
-                  force_fd = force_fd.item()
-                  force_indx = 3*i + a 
-                  force_model = forces_model[m][force_indx].item()
-                  percent_error = abs(force_model - force_fd) #((force_model - force_fd)/force_model)*100.
-                  percent_errors.append(percent_error)
+            for a in range(0,3):
+                natoms = snap.data[m]['NumAtoms']
 
-                  # return position back to normal
+                # calculate model energy with +h (energy1)
 
-                  snap.data[m]['Positions'][i,a] += h
+                snap.data[m]['Positions'][i,a] += h
+                snap.calculator.distributed_index = 0
+                snap.calculator.shared_index = 0
+                snap.calculator.shared_index_b = 0
+                snap.calculator.shared_index_c = 0
+                snap.calculator.shared_index_dgrad = 0
+                snap.process_configs()
+                snap.solver.create_datasets()
+                (energies1, forces1) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=False)
+
+                # calculate model energy with -h (energy2)
+
+                snap.data[m]['Positions'][i,a] -= 2.*h
+                snap.calculator.distributed_index = 0
+                snap.calculator.shared_index = 0
+                snap.calculator.shared_index_b = 0
+                snap.calculator.shared_index_c = 0
+                snap.calculator.shared_index_dgrad = 0
+                snap.process_configs()
+                snap.solver.create_datasets()
+                (energies2, forces2) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=False)
+
+                # calculate and compare finite difference force
+
+                force_fd = -1.0*(energies1[m] - energies2[m])/(2.*h)
+                force_fd = force_fd.item()
+                force_indx = 3*i + a 
+                force_model = forces_model[m][force_indx].item()
+                percent_error = abs(force_model - force_fd) #((force_model - force_fd)/force_model)*100.
+                percent_errors.append(percent_error)
+
+                # return position back to normal
+
+                snap.data[m]['Positions'][i,a] += h
 
     percent_errors = np.array(percent_errors)
     mean_err = np.mean(np.abs(percent_errors))
     max_err = np.max(np.abs(percent_errors))
 
     # mean and max percent error should be < 0.001 %
     # max percent error should be < 0.1 %
@@ -161,66 +160,66 @@
     snap.delete_data = False 
 
     # calculate model forces
 
     snap.process_configs()
     pt.all_barrier()
     snap.solver.create_datasets()
-    (energies_model, forces_model) = snap.solver.evaluate_configs(option=1, standardize_bool=True)
+    (energies_model, forces_model) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=True)
 
     print(f"Length of data: {len(snap.data)}")
 
     # chose a random config to test against
 
     random_indx = 0 #random.randint(0, len(snap.data)-1)
 
     percent_errors = []
     for m in range(random_indx,random_indx+1):
         for i in range(0,snap.data[m]['NumAtoms']):
-              for a in range(0,3):
-                  natoms = snap.data[m]['NumAtoms']
+            for a in range(0,3):
+                natoms = snap.data[m]['NumAtoms']
 
-                  # calculate model energy with +h (energy1)
+                # calculate model energy with +h (energy1)
 
-                  snap.data[m]['Positions'][i,a] += h
-                  snap.calculator.distributed_index = 0
-                  snap.calculator.shared_index = 0
-                  snap.calculator.shared_index_b = 0
-                  snap.calculator.shared_index_c = 0
-                  snap.calculator.shared_index_dgrad = 0
-                  snap.process_configs()
-                  snap.solver.create_datasets()
-                  (energies1, forces1) = snap.solver.evaluate_configs(option=1, standardize_bool=False)
-
-                  # calculate model energy with -h (energy2)
-
-                  snap.data[m]['Positions'][i,a] -= 2.*h
-                  snap.calculator.distributed_index = 0
-                  snap.calculator.shared_index = 0
-                  snap.calculator.shared_index_b = 0
-                  snap.calculator.shared_index_c = 0
-                  snap.calculator.shared_index_dgrad = 0
-                  snap.process_configs()
-                  snap.solver.create_datasets()
-                  (energies2, forces2) = snap.solver.evaluate_configs(option=1, standardize_bool=False)
-
-                  # calculate and compare finite difference force
-
-                  force_fd = -1.0*(energies1[m] - energies2[m])/(2.*h)
-                  force_fd = force_fd.item()
-                  force_indx = 3*i + a 
-                  force_model = forces_model[m][force_indx].item()
-                  percent_error = abs(force_model - force_fd) #((force_model - force_fd)/force_model)*100.
-                  print(f"absolute error: {percent_error}")
-                  assert(percent_error < 0.1) # nice assertion to have for all forces
-                  percent_errors.append(percent_error)
+                snap.data[m]['Positions'][i,a] += h
+                snap.calculator.distributed_index = 0
+                snap.calculator.shared_index = 0
+                snap.calculator.shared_index_b = 0
+                snap.calculator.shared_index_c = 0
+                snap.calculator.shared_index_dgrad = 0
+                snap.process_configs()
+                snap.solver.create_datasets()
+                (energies1, forces1) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=False)
+
+                # calculate model energy with -h (energy2)
+
+                snap.data[m]['Positions'][i,a] -= 2.*h
+                snap.calculator.distributed_index = 0
+                snap.calculator.shared_index = 0
+                snap.calculator.shared_index_b = 0
+                snap.calculator.shared_index_c = 0
+                snap.calculator.shared_index_dgrad = 0
+                snap.process_configs()
+                snap.solver.create_datasets()
+                (energies2, forces2) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=False)
+
+                # calculate and compare finite difference force
+
+                force_fd = -1.0*(energies1[m] - energies2[m])/(2.*h)
+                force_fd = force_fd.item()
+                force_indx = 3*i + a 
+                force_model = forces_model[m][force_indx].item()
+                percent_error = abs(force_model - force_fd) #((force_model - force_fd)/force_model)*100.
+                print(f"absolute error: {percent_error}")
+                assert(percent_error < 0.1) # nice assertion to have for all forces
+                percent_errors.append(percent_error)
 
-                  # return position back to normal
+                # return position back to normal
 
-                  snap.data[m]['Positions'][i,a] += h
+                snap.data[m]['Positions'][i,a] += h
 
     percent_errors = np.array(percent_errors)
     mean_err = np.mean(np.abs(percent_errors))
     max_err = np.max(np.abs(percent_errors))
 
     # mean and max percent error should be < 0.001 %
     # max percent error should be < 0.1 %
@@ -271,66 +270,65 @@
     snap.delete_data = False 
 
     # calculate model forces
 
     snap.process_configs()
     pt.all_barrier()
     snap.solver.create_datasets()
-    (energies_model, forces_model) = snap.solver.evaluate_configs(option=1, standardize_bool=True)
+    (energies_model, forces_model) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=True)
 
     print(f"Length of data: {len(snap.data)}")
 
     # chose a random config to test against
 
     random_indx = 0 #random.randint(0, len(snap.data)-1)
 
     percent_errors = []
     for m in range(random_indx,random_indx+1):
         for i in range(0,snap.data[m]['NumAtoms']):
-        #for i in range(0,1):
-              for a in range(0,3):
-                  natoms = snap.data[m]['NumAtoms']
-
-                  # calculate model energy with +h (energy1)
-
-                  snap.data[m]['Positions'][i,a] += h
-                  snap.calculator.distributed_index = 0
-                  snap.calculator.shared_index = 0
-                  snap.calculator.shared_index_b = 0
-                  snap.calculator.shared_index_c = 0
-                  snap.calculator.shared_index_dgrad = 0
-                  snap.process_configs()
-                  snap.solver.create_datasets()
-                  (energies1, forces1) = snap.solver.evaluate_configs(option=1, standardize_bool=False)
-
-                  # calculate model energy with -h (energy2)
-
-                  snap.data[m]['Positions'][i,a] -= 2.*h
-                  snap.calculator.distributed_index = 0
-                  snap.calculator.shared_index = 0
-                  snap.calculator.shared_index_b = 0
-                  snap.calculator.shared_index_c = 0
-                  snap.calculator.shared_index_dgrad = 0
-                  snap.process_configs()
-                  snap.solver.create_datasets()
-                  (energies2, forces2) = snap.solver.evaluate_configs(option=1, standardize_bool=False)
-
-                  # calculate and compare finite difference force
-
-                  force_fd = -1.0*(energies1[m] - energies2[m])/(2.*h)
-                  force_fd = force_fd.item()
-                  force_indx = 3*i + a 
-                  force_model = forces_model[m][force_indx].item()
-                  percent_error = abs(force_model - force_fd) #((force_model - force_fd)/force_model)*100.
-                  #print(percent_error)
-                  percent_errors.append(percent_error)
+            for a in range(0,3):
+                natoms = snap.data[m]['NumAtoms']
+
+                # calculate model energy with +h (energy1)
+
+                snap.data[m]['Positions'][i,a] += h
+                snap.calculator.distributed_index = 0
+                snap.calculator.shared_index = 0
+                snap.calculator.shared_index_b = 0
+                snap.calculator.shared_index_c = 0
+                snap.calculator.shared_index_dgrad = 0
+                snap.process_configs()
+                snap.solver.create_datasets()
+                (energies1, forces1) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=False)
+
+                # calculate model energy with -h (energy2)
+
+                snap.data[m]['Positions'][i,a] -= 2.*h
+                snap.calculator.distributed_index = 0
+                snap.calculator.shared_index = 0
+                snap.calculator.shared_index_b = 0
+                snap.calculator.shared_index_c = 0
+                snap.calculator.shared_index_dgrad = 0
+                snap.process_configs()
+                snap.solver.create_datasets()
+                (energies2, forces2) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=False)
+
+                # calculate and compare finite difference force
+
+                force_fd = -1.0*(energies1[m] - energies2[m])/(2.*h)
+                force_fd = force_fd.item()
+                force_indx = 3*i + a 
+                force_model = forces_model[m][force_indx].item()
+                percent_error = abs(force_model - force_fd) #((force_model - force_fd)/force_model)*100.
+                #print(percent_error)
+                percent_errors.append(percent_error)
 
-                  # return position back to normal
+                # return position back to normal
 
-                  snap.data[m]['Positions'][i,a] += h
+                snap.data[m]['Positions'][i,a] += h
 
     percent_errors = np.array(percent_errors)
     mean_err = np.mean(np.abs(percent_errors))
     max_err = np.max(np.abs(percent_errors))
 
     # mean and max percent error should be < 0.001 %
     # max percent error should be < 0.1 %
```

