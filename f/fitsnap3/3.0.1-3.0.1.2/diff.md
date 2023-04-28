# Comparing `tmp/fitsnap3-3.0.1.tar.gz` & `tmp/fitsnap3-3.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsnap3-3.0.1.tar", last modified: Fri Apr 28 14:41:58 2023, max compression
+gzip compressed data, was "fitsnap3-3.0.1.2.tar", last modified: Fri Apr 28 14:54:37 2023, max compression
```

## Comparing `fitsnap3-3.0.1.tar` & `fitsnap3-3.0.1.2.tar`

### file list

```diff
@@ -1,168 +1,171 @@
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.458765 fitsnap3-3.0.1/
--rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.0.1/LICENSE
--rw-rw-r--   0 drew      (1000) drew      (1000)    24953 2023-04-28 14:41:58.458765 fitsnap3-3.0.1/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     3819 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/README.md
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.410764 fitsnap3-3.0.1/fitsnap3/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1799 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3/__main__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3/fitsnap.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.410764 fitsnap3-3.0.1/fitsnap3.egg-info/
--rw-rw-r--   0 drew      (1000) drew      (1000)    24953 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     5209 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/SOURCES.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/dependency_links.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/requires.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-04-28 14:41:58.000000 fitsnap3-3.0.1/fitsnap3.egg-info/top_level.txt
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.410764 fitsnap3-3.0.1/fitsnap3lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.418764 fitsnap3-3.0.1/fitsnap3lib/calculators/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2060 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/basic_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    16381 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1191 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/calculator_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8511 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_base.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11541 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    17979 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19992 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      433 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/calculators/template_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6496 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/fitsnap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3670 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/initialize.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.418764 fitsnap3-3.0.1/fitsnap3lib/io/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/error.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6468 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/input.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      313 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.422764 fitsnap3-3.0.1/fitsnap3lib/io/outputs/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1712 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      746 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/output_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8305 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/outputs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7156 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14246 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      263 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/outputs/template_output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.426764 fitsnap3-3.0.1/fitsnap3lib/io/sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.430765 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8204 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      322 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7382 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2183 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1033 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      902 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/eshift.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2267 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/extras.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4832 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/groups.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      855 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/memory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      996 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/outfile.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      717 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/path.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1223 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/reference.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1607 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2039 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/section_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6731 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/sections.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.430765 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1112 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3152 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      473 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4578 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5629 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      482 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/ridge.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1587 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      364 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/template.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      960 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/io/sections/trainshift.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.430765 fitsnap3-3.0.1/fitsnap3lib/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.434764 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.434764 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pairwise.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pas.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12046 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/write.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.434764 fitsnap3-3.0.1/fitsnap3lib/lib/pace/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/pace/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13217 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/pace/pace.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.434764 fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/setup.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.438764 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.438764 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/gen_labels.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/genlib.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.438764 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/tree_method.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.442765 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/young.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      349 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/parallel_output.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    35256 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/parallel_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.442765 fitsnap3-3.0.1/fitsnap3lib/scrapers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4345 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/json_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    17413 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/scrape.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      759 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/scraper_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/template_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    27314 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/vasp_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19146 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/scrapers/xyz_scraper.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.450765 fitsnap3-3.0.1/fitsnap3lib/solvers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3082 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/anl.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3169 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10164 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/bcs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8565 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1786 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/lreg.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5291 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/mcmc.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4994 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/merr.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    39513 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2329 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/opt.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    42023 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2161 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/ridge.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3005 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    24006 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1091 2023-04-28 14:39:05.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/solver_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1559 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/svd.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      388 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/template_solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1793 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/solvers/tensorflowsvd.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.454765 fitsnap3-3.0.1/fitsnap3lib/tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/configuration.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/tools/dataframe_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/dataloaders.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/lammps_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/nn_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/tools/test_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.454765 fitsnap3-3.0.1/fitsnap3lib/units/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/units/conversion_finder.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/energy.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/force.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/length.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/mass.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/pressure.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/temperature.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/fitsnap3lib/units/time.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.0.1/fitsnap3lib/units/units.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1092 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/pyproject.toml
--rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-04-28 14:41:58.458765 fitsnap3-3.0.1/setup.cfg
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:41:58.458765 fitsnap3-3.0.1/tests/
--rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/tests/test_examples.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12841 2023-04-28 14:38:35.000000 fitsnap3-3.0.1/tests/test_pytorch.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.0.1.2/LICENSE
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24955 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3819 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/README.md
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.947444 fitsnap3-3.0.1.2/fitsnap3/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1799 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3/__main__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3/fitsnap.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.947444 fitsnap3-3.0.1.2/fitsnap3.egg-info/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24955 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5292 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/SOURCES.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/dependency_links.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/requires.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/top_level.txt
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.947444 fitsnap3-3.0.1.2/fitsnap3lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.951444 fitsnap3-3.0.1.2/fitsnap3lib/calculators/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2060 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/basic_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    16381 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1191 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/calculator_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8511 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_base.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    11541 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17979 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19992 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      433 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/template_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6496 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/fitsnap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3670 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/initialize.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.951444 fitsnap3-3.0.1.2/fitsnap3lib/io/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/error.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6468 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/input.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      313 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.951444 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1712 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      746 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/output_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8305 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/outputs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7156 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14246 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      263 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/template_output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.955444 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.959444 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8204 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/ace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      322 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7382 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2183 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1033 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      902 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/eshift.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2267 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/extras.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4832 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/groups.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      855 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/memory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      996 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/outfile.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      717 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/path.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1223 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/reference.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1607 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2039 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/section_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6731 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/sections.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.959444 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1112 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3152 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      473 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4578 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5629 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      482 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1587 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      364 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/template.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      960 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/trainshift.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.959444 fitsnap3-3.0.1.2/fitsnap3lib/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.959444 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pairwise.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pas.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12046 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/write.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/pace/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/pace/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13217 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/pace/pace.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/ridge_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:51:51.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/ridge_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      664 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/ridge_solver/regressor.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/setup.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.967444 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/gen_labels.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/genlib.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.967444 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/rpi_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/tree_method.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/wigner_couple.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.967444 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/young.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      349 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/parallel_output.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    35256 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/parallel_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.967444 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4345 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/json_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17413 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/scrape.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      759 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/scraper_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/template_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    27314 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/vasp_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19146 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/xyz_scraper.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.971444 fitsnap3-3.0.1.2/fitsnap3lib/solvers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3082 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/anl.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3169 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10164 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/bcs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8565 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1786 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/lreg.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5291 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/mcmc.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4994 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/merr.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    39513 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2329 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/opt.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    42023 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2161 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3005 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24006 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1091 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/solver_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1559 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/svd.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      388 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/template_solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1793 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/tensorflowsvd.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/fitsnap3lib/tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/configuration.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/dataframe_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/dataloaders.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/lammps_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/nn_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/test_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/fitsnap3lib/units/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/conversion_finder.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/energy.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/force.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/length.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/mass.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/pressure.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/temperature.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/time.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/units.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1095 2023-04-28 14:54:30.000000 fitsnap3-3.0.1.2/pyproject.toml
+-rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/setup.cfg
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/tests/
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/tests/test_examples.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12841 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/tests/test_pytorch.py
```

### Comparing `fitsnap3-3.0.1/LICENSE` & `fitsnap3-3.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/PKG-INFO` & `fitsnap3-3.0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.0.1
+Version: 3.0.1.2
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991
```

### Comparing `fitsnap3-3.0.1/README.md` & `fitsnap3-3.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3/__main__.py` & `fitsnap3-3.0.1.2/fitsnap3/__main__.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3.egg-info/PKG-INFO` & `fitsnap3-3.0.1.2/fitsnap3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.0.1
+Version: 3.0.1.2
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991
```

### Comparing `fitsnap3-3.0.1/fitsnap3.egg-info/SOURCES.txt` & `fitsnap3-3.0.1.2/fitsnap3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 fitsnap3lib/lib/neural_networks/pytorch.py
 fitsnap3lib/lib/neural_networks/write.py
 fitsnap3lib/lib/neural_networks/descriptors/__init__.py
 fitsnap3lib/lib/neural_networks/descriptors/bessel.py
 fitsnap3lib/lib/neural_networks/descriptors/g3b.py
 fitsnap3lib/lib/pace/__init__.py
 fitsnap3lib/lib/pace/pace.py
+fitsnap3lib/lib/ridge_solver/__init__.py
+fitsnap3lib/lib/ridge_solver/regressor.py
 fitsnap3lib/lib/scalapack_solver/__init__.py
 fitsnap3lib/lib/scalapack_solver/scalapack.py
 fitsnap3lib/lib/scalapack_solver/setup.py
 fitsnap3lib/lib/sym_ACE/__init__.py
 fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
 fitsnap3lib/lib/sym_ACE/gen_labels.py
 fitsnap3lib/lib/sym_ACE/genlib.py
```

### Comparing `fitsnap3-3.0.1/fitsnap3lib/calculators/basic_calculator.py` & `fitsnap3-3.0.1.2/fitsnap3lib/calculators/basic_calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/calculators/calculator.py` & `fitsnap3-3.0.1.2/fitsnap3lib/calculators/calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/calculators/calculator_factory.py` & `fitsnap3-3.0.1.2/fitsnap3lib/calculators/calculator_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_base.py` & `fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_base.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_custom.py` & `fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_pace.py` & `fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_pace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/calculators/lammps_snap.py` & `fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_snap.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/fitsnap.py` & `fitsnap3-3.0.1.2/fitsnap3lib/fitsnap.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/initialize.py` & `fitsnap3-3.0.1.2/fitsnap3lib/initialize.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/input.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/input.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/outputs/custom.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/outputs/output_factory.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/output_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/outputs/outputs.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/outputs/pace.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/pace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/outputs/snap.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/snap.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/ace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/bispectrum.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/eshift.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/eshift.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/extras.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/extras.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/groups.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/groups.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/memory.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/memory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/outfile.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/outfile.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/path.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/path.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/reference.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/reference.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/scraper.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/section_factory.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/section_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/sections.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/sections.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/ard.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/ard.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/jax.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/network.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/network.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/solver_sections/solver.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/solver.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/io/sections/trainshift.py` & `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/trainshift.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/bessel.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/g3b.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/jax.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pairwise.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pairwise.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pas.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pas.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/pytorch.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/neural_networks/write.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/write.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/pace/pace.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/pace/pace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/scalapack.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/scalapack_solver/setup.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/setup.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/gen_labels.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/gen_labels.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/genlib.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/genlib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/rpi_lib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/tree_method.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/tree_method.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/wigner_couple.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/lib/sym_ACE/young.py` & `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/young.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/parallel_tools.py` & `fitsnap3-3.0.1.2/fitsnap3lib/parallel_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/scrapers/json_scraper.py` & `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/json_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/scrapers/scrape.py` & `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/scrape.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/scrapers/scraper_factory.py` & `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/scraper_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/scrapers/vasp_scraper.py` & `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/vasp_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/scrapers/xyz_scraper.py` & `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/xyz_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/anl.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/anl.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/ard.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/ard.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/bcs.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/bcs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/jax.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/lasso.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/lasso.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/lreg.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/lreg.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/mcmc.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/mcmc.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/merr.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/merr.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/network.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/network.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/opt.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/opt.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/pytorch.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/ridge.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/ridge.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/scalapack.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/scalapack.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/solver.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/solver_factory.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/solver_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/svd.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/svd.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/solvers/tensorflowsvd.py` & `fitsnap3-3.0.1.2/fitsnap3lib/solvers/tensorflowsvd.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/tools/configuration.py` & `fitsnap3-3.0.1.2/fitsnap3lib/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/tools/dataframe_tools.py` & `fitsnap3-3.0.1.2/fitsnap3lib/tools/dataframe_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/tools/dataloaders.py` & `fitsnap3-3.0.1.2/fitsnap3lib/tools/dataloaders.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/tools/lammps_tools.py` & `fitsnap3-3.0.1.2/fitsnap3lib/tools/lammps_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/tools/nn_tools.py` & `fitsnap3-3.0.1.2/fitsnap3lib/tools/nn_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/tools/test_tools.py` & `fitsnap3-3.0.1.2/fitsnap3lib/tools/test_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/units/conversion_finder.py` & `fitsnap3-3.0.1.2/fitsnap3lib/units/conversion_finder.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/fitsnap3lib/units/units.py` & `fitsnap3-3.0.1.2/fitsnap3lib/units/units.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/pyproject.toml` & `fitsnap3-3.0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "fitsnap3"
-version = "3.0.1"
+version = "3.0.1.2"
 description = "Molecular Machine Learning Interface"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -45,8 +45,8 @@
 #packages = [
 #    "fitsnap3",
 #    "fitsnap3lib",
 #]
 
 [tool.setuptools.packages.find]
 include = ["fitsnap3*", "fitsnap3lib*"]  # alternatively: `exclude = ["additional*"]`
-namespaces = false
+namespaces = false
```

### Comparing `fitsnap3-3.0.1/tests/test_examples.py` & `fitsnap3-3.0.1.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1/tests/test_pytorch.py` & `fitsnap3-3.0.1.2/tests/test_pytorch.py`

 * *Files identical despite different names*

