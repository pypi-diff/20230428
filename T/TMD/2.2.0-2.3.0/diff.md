# Comparing `tmp/tmd-2.2.0.tar.gz` & `tmp/TMD-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmd-2.2.0.tar", last modified: Mon Aug 22 11:37:29 2022, max compression
+gzip compressed data, was "TMD-2.3.0.tar", last modified: Fri Apr 28 11:43:56 2023, max compression
```

## Comparing `tmd-2.2.0.tar` & `TMD-2.3.0.tar`

### file list

```diff
@@ -1,118 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.551731 tmd-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.539731 tmd-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.543731 tmd-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-08-22 11:37:24.000000 tmd-2.2.0/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-08-22 11:37:24.000000 tmd-2.2.0/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-22 11:37:24.000000 tmd-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-22 11:37:24.000000 tmd-2.2.0/.pep8rc
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-22 11:37:24.000000 tmd-2.2.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-08-22 11:37:24.000000 tmd-2.2.0/COPYING-BSD
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-08-22 11:37:24.000000 tmd-2.2.0/COPYING-LGPL
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-08-22 11:37:24.000000 tmd-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-22 11:37:29.551731 tmd-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-08-22 11:37:24.000000 tmd-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.543731 tmd-2.2.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-22 11:37:24.000000 tmd-2.2.0/doc/Installation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-08-22 11:37:24.000000 tmd-2.2.0/doc/Readme.txt
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-08-22 11:37:24.000000 tmd-2.2.0/doc/Tutorial.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.543731 tmd-2.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.543731 tmd-2.2.0/examples/Advanced/
--rw-r--r--   0 runner    (1001) docker     (121)    34431 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/Advanced/advanced_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     6988 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/Advanced/classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/Advanced/diversity_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     3039 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/Advanced/matching.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/Advanced/polar_plot_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7329 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/Advanced/time_series_tmd.py
--rw-r--r--   0 runner    (1001) docker     (121)    18803 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/Advanced/variability.py
--rw-r--r--   0 runner    (1001) docker     (121)     3228 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/classifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/distances_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/extract_ph.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-08-22 11:37:24.000000 tmd-2.2.0/examples/write_swc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-08-22 11:37:24.000000 tmd-2.2.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 11:37:29.551731 tmd-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-08-22 11:37:24.000000 tmd-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.543731 tmd-2.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/basic.swc
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/basic_exotic_section_types.swc
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/basic_no_comments.swc
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/basic_no_sec_ids.swc
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/basic_options.swc
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/neuron.swc
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/neuron_ph_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/neuron_ph_2.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/sample.swc
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/sample_disordered.swc
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/sample_disordered_v1.h5
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/sample_ph_0.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/sample_ph_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/sample_v0.h5
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/sample_v1.h5
--rw-r--r--   0 runner    (1001) docker     (121)     7264 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/sample_v2.h5
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/test_morph.swc
--rw-r--r--   0 runner    (1001) docker     (121)     4240 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/test_morph_v1.h5
--rw-r--r--   0 runner    (1001) docker     (121)     8552 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/test_morph_v2.h5
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tests/data/valid/
--rw-r--r--   0 runner    (1001) docker     (121)    48881 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/valid/C010398B-P2.CNG.swc
--rwxr-xr-x   0 runner    (1001) docker     (121)    33168 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/valid/C010398B-P2.h5
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/valid/sample.swc
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/valid/sample_v1.h5
--rw-r--r--   0 runner    (1001) docker     (121)     7264 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/data/valid/sample_v2.h5
--rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_h5.py
--rw-r--r--   0 runner    (1001) docker     (121)     3854 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_neuron.py
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_neuron_conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_neuron_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_population.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_soma.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_soma_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_swc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7612 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_topology_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    10241 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_topology_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     4975 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_topology_persistent_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     7361 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-22 11:37:24.000000 tmd-2.2.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tmd/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tmd/Neuron/
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Neuron/Neuron.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Neuron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Neuron/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tmd/Population/
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Population/Population.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Population/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tmd/Soma/
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Soma/Soma.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Soma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Soma/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tmd/Topology/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13142 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Topology/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Topology/methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     5925 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Topology/persistent_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Topology/statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Topology/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tmd/Tree/
--rw-r--r--   0 runner    (1001) docker     (121)     5782 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Tree/Tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9857 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/Tree/methods.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.551731 tmd-2.2.0/tmd/io/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/io/conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/io/h5.py
--rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/io/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     4333 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/io/swc.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.551731 tmd-2.2.0/tmd/view/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21237 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/view/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    10843 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/view/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    29120 2022-08-22 11:37:24.000000 tmd-2.2.0/tmd/view/view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 11:37:29.547731 tmd-2.2.0/tmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-22 11:37:29.000000 tmd-2.2.0/tmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-08-22 11:37:29.000000 tmd-2.2.0/tmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 11:37:29.000000 tmd-2.2.0/tmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-08-22 11:37:29.000000 tmd-2.2.0/tmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-22 11:37:29.000000 tmd-2.2.0/tmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-08-22 11:37:24.000000 tmd-2.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.051457 TMD-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-28 11:43:44.000000 TMD-2.3.0/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-28 11:43:44.000000 TMD-2.3.0/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:44.000000 TMD-2.3.0/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 11:43:44.000000 TMD-2.3.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-28 11:43:44.000000 TMD-2.3.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 11:43:44.000000 TMD-2.3.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 11:43:44.000000 TMD-2.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 11:43:44.000000 TMD-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-28 11:43:44.000000 TMD-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-28 11:43:44.000000 TMD-2.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-28 11:43:44.000000 TMD-2.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-28 11:43:44.000000 TMD-2.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-28 11:43:44.000000 TMD-2.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-28 11:43:44.000000 TMD-2.3.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-28 11:43:44.000000 TMD-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-28 11:43:44.000000 TMD-2.3.0/COPYRIGHT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-28 11:43:44.000000 TMD-2.3.0/LICENSE-BSD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-28 11:43:44.000000 TMD-2.3.0/LICENSE-LGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 11:43:44.000000 TMD-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-28 11:43:56.051457 TMD-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-28 11:43:44.000000 TMD-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/TMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-28 11:43:55.000000 TMD-2.3.0/TMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 11:43:56.000000 TMD-2.3.0/TMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:43:55.000000 TMD-2.3.0/TMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 11:43:55.000000 TMD-2.3.0/TMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 11:43:55.000000 TMD-2.3.0/TMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-28 11:43:44.000000 TMD-2.3.0/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.035457 TMD-2.3.0/examples/Advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)    34102 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/advanced_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/diversity_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/polar_plot_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/time_series_tmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20425 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/distances_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/extract_ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/write_swc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 11:43:44.000000 TMD-2.3.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 11:43:44.000000 TMD-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:43:56.051457 TMD-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-28 11:43:44.000000 TMD-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.039457 TMD-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic_exotic_section_types.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic_no_comments.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic_no_sec_ids.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic_options.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/neuron.swc
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/neuron_ph_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/neuron_ph_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_disordered.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_disordered_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_ph_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_ph_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_v0.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_v2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/test_morph.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/test_morph_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/test_morph_v2.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tests/data/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/C010398B-P2.CNG.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33168 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/C010398B-P2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/sample.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/sample_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/sample_v2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_neuron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_neuron_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_neuron_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_soma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_soma_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_swc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_topology_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_topology_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_topology_persistent_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/Neuron/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Neuron/Neuron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Neuron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Neuron/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/Population/
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Population/Population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Population/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/Soma/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Soma/Soma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Soma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Soma/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/Topology/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/persistent_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.051457 TMD-2.3.0/tmd/Tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Tree/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Tree/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.051457 TMD-2.3.0/tmd/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/swc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.051457 TMD-2.3.0/tmd/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/view/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/view/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40938 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/view/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-28 11:43:44.000000 TMD-2.3.0/tox.ini
```

### Comparing `tmd-2.2.0/COPYING-BSD` & `TMD-2.3.0/LICENSE-BSD.txt`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/COPYING-LGPL` & `TMD-2.3.0/LICENSE-LGPL.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-                   GNU LESSER GENERAL PUBLIC LICENSE
+                  GNU LESSER GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
 
   This version of the GNU Lesser General Public License incorporates
 the terms and conditions of version 3 of the GNU General Public
 License, supplemented by the additional permissions listed below.
```

### Comparing `tmd-2.2.0/LICENSE.txt` & `TMD-2.3.0/tmd/Soma/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-TMD - Topological Morphology Descriptor Python library
+"""TMD: Soma class."""
 
-TMD is licensed under the LGPL, unless noted otherwise, e.g., for external
-dependencies. See files COPYING-LGPL and COPYING-BSD for the full licenses.
-Examples and test are BSD-licensed.
-External dependencies are either LGPL or BSD-licensed.
-See file ACKNOWLEDGEMENTS.txt and AUTHORS.txt for further details.
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-Copyright (c) 2016-2022 Blue Brain Project/EPFL
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU Lesser General Public License as published by the
-Free Software Foundation, either version 3 of the License, or (at your option)
-any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY;
-without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
-
-See the GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General Public License
-along with this program. If not, see <http://www.gnu.org/licenses/>.
+import tmd.Soma.Soma  # noqa
```

### Comparing `tmd-2.2.0/README.md` & `TMD-2.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,79 @@
-TMD: Topological Morphology Descriptor
-========================================
+# TMD
 
-The TMD performs the topological analysis of neuronal morphologies and extracts the persistence barcodes of trees.
+A python package for the topological analysis of neurons.
 
-©Blue Brain Project/EPFL 2005 – 2019. All rights reserved
+The TMD performs the topological analysis of neuronal morphologies and extracts the persistence
+barcodes of trees.
 
-Details
----------
-Author: Lida Kanari
+This Python module includes:
 
-Contributors: Pawel Dlotko, Benoit Coste
+* Basic loading of neuronal morphologies in swc and h5 file format.
+* Extraction of the topological descriptors of tree morphologies.
+* Visualization of neuronal trees and neurons.
+* Plotting persistence diagrams, barcodes and images.
 
-Publication:
 
+## Installation
 
-A Topological Representation of Branching Neuronal Morphologies
+This package should be installed using pip:
 
-_Cite this article as:_
-    Kanari, L., Dłotko, P., Scolamiero, M. et al. Neuroinform (2018) 16:3.
-    DOI: <https://doi.org/10.1007/s12021-017-9341-1>
+```bash
+pip install TMD
+```
 
-Related publications:
+For installation of optional viewers:
 
+```bash
+pip install TMD[viewer]
+```
 
-Comprehensive Morpho-Electrotonic Analysis Shows 2 Distinct Classes of L2 and L3 Pyramidal Neurons in Human Temporal Cortex.
 
-_Cite this article as:_
-   Deitcher Y., Eyal G., Kanari L., et al. Cerebral Cortex (2017) 27:11
-   DOI: <https://doi.org/10.1093/cercor/bhx226>
+## Usage
 
-Objective Classification of Neocortical Pyramidal Cells
-    DOI: <http://dx.doi.org/10.1101/349977>
+```python
+# Import the TMD toolkit in IPython
+import tmd
 
-Developed in Blue Brain Project
+# Load a neuron
+neuron = tmd.io.load_neuron('input_path_to_file/input_file.swc')
 
-Funding
----------
-This project/research was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
+# Extract the tmd of a neurite, i.e., neuronal tree
+pd = tmd.methods.get_persistence_diagram(neuron.neurites[0])
+```
 
-Sotware description
----------------------
+## Citation
 
-This Python module includes:
+If you use this software or method for your research, we kindly ask you to cite the following publication associated to this repository:
 
-* Basic loading of neuronal morphologies in swc and h5 file format.
-* Extraction of the topological descriptors of tree morphologies.
-* Visualization of neuronal trees and neurons.
-* Ploting persistence diagrams, barcodes and images.
+**A Topological Representation of Branching Neuronal Morphologies**
 
-Supported OS
---------------
+_Cite this article as:_
 
-Ubuntu : 12.0, 14.04, 16.04
+Kanari, L., Dłotko P., Scolamiero M., et al., A Topological Representation of Branching Neuronal Morphologies, Neuroinformatics 16, nᵒ 1 (2018): 3‑13. https://doi.org/10.1007/s12021-017-9341-1.
 
-macOS: Sierra 10.13.3
 
-Required Dependencies
----------------------
+## Related publications
 
-Python : 2.7+
+**Comprehensive Morpho-Electrotonic Analysis Shows 2 Distinct Classes of L2 and L3 Pyramidal Neurons in Human Temporal Cortex, Cerebral Cortex**
 
-numpy : 1.8.1+,
-scipy : 0.13.3+,
-enum34 : 1.0.4+,
-scikit-learn : 0.19.1+,
-munkres: 1.0.12+
+_Cite this article as:_
 
-Optional Dependencies
-----------------------
-h5py : 2.8.0+ (optional),
-matplotlib : 1.3.1+ (required for viewer mode)
+Deitcher Y., Eyal G., Kanari L., et al., Comprehensive Morpho-Electrotonic Analysis Shows 2 Distinct Classes of L2 and L3 Pyramidal Neurons in Human Temporal Cortex, Cerebral Cortex, Volume 27, Issue 11, November 2017, Pages 5398–5414, https://doi.org/10.1093/cercor/bhx226
 
-Instalation instructions
---------------------------------
+**Objective Morphological Classification of Neocortical Pyramidal Cells**:
 
-```bash
-virtualenv test_tmd
-source ./test_tmd/bin/activate
-git clone https://github.com/BlueBrain/TMD
-pip install ./TMD
-```
+_Cite this article as:_
 
-For installation of viewers (only works in Python2)
+Lida Kanari, Srikanth Ramaswamy, Ying Shi, Sebastien Morand, Julie Meystre, Rodrigo Perin, Marwan Abdellah, Yun Wang, Kathryn Hess, Henry Markram, Objective Morphological Classification of Neocortical Pyramidal Cells, Cerebral Cortex, Volume 29, Issue 4, April 2019, Pages 1719-1735, https://doi.org/10.1093/cercor/bhy339
 
-```bash
-pip install ./TMD[viewer]
-```
+Developed in Blue Brain Project.
+
+## Funding & Acknowledgment
+
+The development of this software was supported by funding to the Blue Brain Project, a research
+center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH
+Board of the Swiss Federal Institutes of Technology.
 
+For license and authors, see `LICENSE.txt` and `AUTHORS.md` respectively.
 
-Copyright (c) 2016-2022 Blue Brain Project/EPFL
+Copyright © 2021-2022 Blue Brain Project/EPFL
```

### Comparing `tmd-2.2.0/examples/Advanced/advanced_plot.py` & `TMD-2.3.0/examples/Advanced/advanced_plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,374 +1,413 @@
-"""Plotting functions of tmd (untested and more complex ploting)"""
-
+"""Example script of plotting functions of tmd (untested and more complex plotting)."""
+import common as _cm
+import matplotlib.colors as mcolors
+import matplotlib.pyplot as plt
 import numpy as _np
-from tmd import Topology as _tm
 import view as _view
-import common as _cm
+from scipy import stats
+
+from tmd import Topology as _tm
+from tmd import utils as _utils
+from tmd import view
 from tmd.analysis import sort_ph
+from tmd.view.plot import barcode
+from tmd.view.plot import diagram
+from tmd.view.plot import persistence_image
 
 
 def _sort_ph_radii(ph):
-    """
-    Sorts barcode according to length of bars.
-    """
+    """Sorts barcode according to length of bars."""
     ph_sort = [[p[0], p[1], p[2], _np.abs(p[0] - p[1])] for p in ph]
     ph_sort.sort(key=lambda x: x[3])
     return ph_sort
 
 
 def _sort_ph_initial(ph):
-    """
-    Sorts barcode according to length of bars.
-    """
+    """Sorts barcode according to length of bars."""
     ph_sort = [[p[0], p[1], p[2], _np.abs(p[0] - p[1])] for p in ph]
     ph_sort.sort(key=lambda x: x[2])
     return [p[:2] for p in ph_sort]
 
 
 def _mirror_ph(ph):
-    """
-    Sorts barcode according to length of bars.
-    """
+    """Sorts barcode according to length of bars."""
     ph_mirror = [[p[0], p[1], p[0] - p[1]] for p in ph]
     ph_mirror.sort(key=lambda x: x[2])
     return ph_mirror
 
 
-def tree_all(tree, plane='xy', feature='radial_distances', title='',
-             diameter=True, treecol='b', xlims=None, ylims=None, **kwargs):
-    '''Subplot with ph, barcode and tree
-    '''
-    from tmd import utils as _utils
-    from matplotlib.collections import LineCollection
-
-    kwargs['output_path'] = kwargs.get('output_path', None)
-
-    fig1, ax1 = _view.tree(tree, new_fig=True, subplot=221, plane='xy',
-                           title=title, treecolor=treecol, diameter=diameter)
+def tree_all(
+    tree,
+    plane="xy",
+    feature="radial_distances",
+    title="",
+    diameter=True,
+    treecol="b",
+    xlim=None,
+    ylim=None,
+    **kwargs,
+):
+    """Subplot with ph, barcode and tree."""
+    kwargs["output_path"] = kwargs.get("output_path", None)
+
+    fig1, ax1 = _view.tree(
+        tree,
+        new_fig=True,
+        subplot=221,
+        plane="xy",
+        title=title,
+        treecolor=treecol,
+        diameter=diameter,
+    )
 
-    feat = getattr(tree, 'get_section_' + feature)()
-    segs = tree.get_segments()
+    # feat = getattr(tree, "get_section_" + feature)()
+    # segs = tree.get_segments()
 
     def _seg_2d(seg):
-        """2d coordinates required for the plotting of a segment"""
-
+        """2d coordinates required for the plotting of a segment."""
         horz = _utils.term_dict[plane[0]]
         vert = _utils.term_dict[plane[1]]
 
         horz1 = seg[0][horz]
         horz2 = seg[1][horz]
         vert1 = seg[0][vert]
         vert2 = seg[1][vert]
 
         return ((horz1, vert1), (horz2, vert2))
 
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, feature=feature)
     else:
-        raise Exception('Plane value not recognised')
+        raise Exception("Plane value not recognised")
 
-    bounds = max(max(ph))
-    fig1, ax2 = ph_diagram(ph, new_fig=False, subplot=222, color=treecol)
+    # bounds = max(max(ph))
+    fig1, ax2 = diagram(ph, new_fig=False, subplot=222, color=treecol)
     fig1, ax3 = barcode(ph, new_fig=False, subplot=223, color=treecol)
-    fig1, ax4 = ph_image(ph, new_fig=False, subplot=224, xlims=xlims, ylims=ylims)
+    fig1, ax4 = persistence_image(ph, new_fig=False, subplot=224, xlim=xlim, ylim=ylim)
     _cm.plt.tight_layout(True)
 
-    if kwargs['output_path'] is not None:
-        fig = _cm.save_plot(fig=ax1, **kwargs)
-
-    return fig1, ax1
-
+    if kwargs["output_path"] is not None:
+        _cm.save_plot(fig=ax1, **kwargs)
 
-def neu_all(neuron, plane='xy', feature='radial_distances', title='',
-            diameter=True, treecol='b', xlims=None, ylims=None, neurite_type='basal', **kwargs):
-    '''Subplot with ph, barcode
-       and tree within spheres
-    '''
-    from tmd import utils as _utils
-    from matplotlib.collections import LineCollection
+    return fig1, ax1, ax2, ax3, ax4
 
-    kwargs['output_path'] = kwargs.get('output_path', None)
 
-    fig1, ax1 = _view.neuron(neuron, new_fig=True, subplot=221, plane='xy', neurite_type=[neurite_type],
-                             title=title, treecolor=treecol, diameter=diameter)
+def neu_all(
+    neuron,
+    plane="xy",
+    feature="radial_distances",
+    title="",
+    diameter=True,
+    treecol="b",
+    xlim=None,
+    ylim=None,
+    neurite_type="basal_dendrite",
+    **kwargs,
+):
+    """Subplot with ph, barcode and tree within spheres."""
+    kwargs["output_path"] = kwargs.get("output_path", None)
+
+    fig1, ax1 = _view.neuron(
+        neuron,
+        new_fig=True,
+        subplot=221,
+        plane="xy",
+        neurite_type=[neurite_type],
+        title=title,
+        treecolor=treecol,
+        diameter=diameter,
+    )
 
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_ph_neuron(neuron, feature=feature, neurite_type=neurite_type)
     else:
-        raise Exception('Plane value not recognised')
+        raise Exception("Plane value not recognised")
 
-    bounds = max(max(ph))
-    fig1, ax2 = ph_diagram(ph, new_fig=False, subplot=222, color=treecol)
+    # bounds = max(max(ph))
+    fig1, ax2 = diagram(ph, new_fig=False, subplot=222, color=treecol)
     fig1, ax3 = barcode(ph, new_fig=False, subplot=223, color=treecol)
-    fig1, ax4 = ph_image(ph, new_fig=False, subplot=224, xlims=xlims, ylims=ylims)
+    fig1, ax4 = persistence_image(ph, new_fig=False, subplot=224, xlim=xlim, ylim=ylim)
     _cm.plt.tight_layout(True)
 
-    if kwargs['output_path'] is not None:
-        fig = _cm.save_plot(fig=ax1, **kwargs)
+    if kwargs["output_path"] is not None:
+        _cm.save_plot(fig=ax1, **kwargs)
 
     return fig1, ax1
 
 
 def barcode_radii(ph, new_fig=True, subplot=False, linewidth=1.2, diam_max=2.0, **kwargs):
-    """
-    Generates a 2d figure (barcode) of the persistent homology
-    """
+    """Generate a 2d figure (barcode) of the persistent homology."""
     from pylab import cm
 
     # Initialization of matplotlib figure and axes.
     fig, ax = _view.common.get_figure(new_fig=new_fig, subplot=subplot)
 
-    # Hach for colorbar creation
-    Z = [[0,0],[0,0]]
-    levels = _np.linspace(0.0,diam_max,200)
+    # Colorbar creation
+    Z = [[0, 0], [0, 0]]
+    levels = _np.linspace(0.0, diam_max, 200)
     CS3 = _view.common.plt.contourf(Z, levels, cmap=cm.jet)
-    ph_sort = sort_ph_radii(ph)
+    ph_sort = _sort_ph_radii(ph)
 
     for ip, p in enumerate(ph_sort):
-        ax.plot(p[:2], [ip, ip], c=cm.jet(p[2]/diam_max), linewidth=linewidth)
+        ax.plot(p[:2], [ip, ip], c=cm.jet(p[2] / diam_max), linewidth=linewidth)
 
-    kwargs['title'] = kwargs.get('title', 'Barcode of p.h.')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'Lifetime')
+    all_kwargs = {
+        "title": "Barcode of p.h.",
+        "xlabel": "Lifetime",
+    }
+    all_kwargs.update(kwargs)
 
     _view.common.plt.ylim([-1, len(ph_sort)])
     _view.common.plt.colorbar(CS3)
 
-    return _view.common.plot_style(fig=fig, ax=ax, **kwargs)
+    return _view.common.plot_style(fig=fig, ax=ax, **all_kwargs)
 
 
-def barcode_mirror(ph, new_fig=True, subplot=False, color='b', **kwargs):
-    """
-    Generates a mirrored 2d figure (barcode) of the persistent homology
-    """
+def barcode_mirror(ph, new_fig=True, subplot=False, color="b", **kwargs):
+    """Generate a mirrored 2d figure (barcode) of the persistent homology."""
     # Initialization of matplotlib figure and axes.
     fig, ax = _view.common.get_figure(new_fig=new_fig, subplot=subplot)
 
     ph_mirror = _mirror_ph(ph)
 
     for ip, p in enumerate(ph_mirror):
         if p[2] >= 0:
             ax.plot(p[:2], [ip, ip], c=color)
         if p[2] < 0:
-            ax.plot(_np.subtract([0,0],p[:2]), [ip, ip], c=color)
+            ax.plot(_np.subtract([0, 0], p[:2]), [ip, ip], c=color)
 
-    kwargs['title'] = kwargs.get('title', 'Mirror Barcode of p.h.')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'Lifetime')
+    all_kwargs = {
+        "title": "Mirror persistence barcode",
+        "xlabel": "Lifetime",
+    }
+    all_kwargs.update(kwargs)
     _view.common.plt.ylim([-len(ph_mirror), len(ph_mirror)])
 
-    return _view.common.plot_style(fig=fig, ax=ax, **kwargs)
+    return _view.common.plot_style(fig=fig, ax=ax, **all_kwargs)
 
 
-def ph_birth_length(ph, new_fig=True, subplot=False, color='b', **kwargs):
-    """
-    Generates a 2d figure (ph diagram) of the persistent homology
-    """
+def ph_birth_length(ph, new_fig=True, subplot=False, color="b", **kwargs):
+    """Generate a 2d figure (ph diagram) of the persistent homology."""
     # Initialization of matplotlib figure and axes.
     fig, ax = _view.common.get_figure(new_fig=new_fig, subplot=subplot)
 
     ph_sort = sort_ph(ph)
 
-    bounds = _np.max(_np.max(ph))
-
     for p in ph_sort:
-
         ax.scatter(p[0], p[2], c=color)
 
-    #_view.common.plt.plot([0, bounds], [0, bounds], c=color)
+    # bounds = _np.max(_np.max(ph))
+    # _view.common.plt.plot([0, bounds], [0, bounds], c=color)
 
-    kwargs['title'] = kwargs.get('title', 'Birth-Length diagram')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'Birth')
-    kwargs['ylabel'] = kwargs.get('ylabel', 'Length')
+    all_kwargs = {
+        "title": "Birth-Length diagram",
+        "xlabel": "Birth",
+        "ylabel": "Length",
+    }
+    all_kwargs.update(kwargs)
 
-    return _view.common.plot_style(fig=fig, ax=ax, **kwargs)
+    return _view.common.plot_style(fig=fig, ax=ax, **all_kwargs)
 
 
-def ph_on_tree(tree, new_fig=True, subplot=False, plane='xy', alpha=0.05, **kwargs):
-    """
-    Generates a 3d figure of the tree and adds
-    the corresponding spheres that represent
-    important events in the persistent homology
+def ph_on_tree(tree, new_fig=True, subplot=False, plane="xy", alpha=0.05, **kwargs):
+    """Generate a 3d figure of the tree.
+
+    Also adds the corresponding spheres that represent important events in the persistent homology
     diagram (birth and death of components).
     """
     # Initialization of matplotlib figure and axes.
     fig, ax = _view.tree(tree, new_fig=new_fig, subplot=subplot, plane=plane, **kwargs)
 
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, dim=plane)
     else:
-        raise Exception('Plane value not recognised')
+        raise Exception("Plane value not recognised")
 
     for p in ph:
+        c1 = _view.common.plt.Circle([tree.x[0], tree.y[0], tree.z[0]], p[0], alpha=alpha)
+        c2 = _view.common.plt.Circle([tree.x[0], tree.y[0], tree.z[0]], p[1], alpha=alpha)
 
-        c1 = _view.common.plt.Circle([tree.x[0], tree.y[0],
-                                      tree.z[0]], p[0], alpha=alpha)
-        c2 = _view.common.plt.Circle([tree.x[0], tree.y[0],
-                                      tree.z[0]], p[1], alpha=alpha)
-
-        ax.add_patch(c1) # pylint: disable=no-member
-        ax.add_patch(c2) # pylint: disable=no-member
+        ax.add_patch(c1)  # pylint: disable=no-member
+        ax.add_patch(c2)  # pylint: disable=no-member
 
     return _view.common.plot_style(fig=fig, ax=ax, **kwargs)
 
 
-def barcode_tree(tree, new_fig=True, plane='xy', output_dir=None, **kwargs):
-    """
-    Generates a 2d figure (barcode) of the persistent homology
-    of a tree as it has been computed by
-    Topology.get_persistent_homology method.
+def barcode_tree(tree, new_fig=True, plane="xy", output_dir=None, **kwargs):
+    """Generate a 2d figure (barcode) of the persistent homology of a tree.
+
+    This persistent homology is supposed to be computed by the Topology.get_persistent_homology()
+    method.
     """
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, dim=plane)
     else:
-        raise Exception('Plane value not recognised')
+        raise Exception("Plane value not recognised")
 
     for ip, p in enumerate(ph):
-
         ph[ip].append(_np.abs(p[0] - p[1]))
 
     ph.sort(key=lambda x: x[2])
 
     for ip, p in enumerate(ph):
-
         fig, ax = _view.tree(tree, new_fig=new_fig, subplot=121, plane=plane)
 
         c1 = _view.common.plt.Circle([tree.x[0], tree.y[0]], p[0], alpha=0.2)
         c2 = _view.common.plt.Circle([tree.x[0], tree.y[0]], p[1], alpha=0.2)
 
-        ax.add_patch(c1) # pylint: disable=no-member
-        ax.add_patch(c2) # pylint: disable=no-member
+        ax.add_patch(c1)  # pylint: disable=no-member
+        ax.add_patch(c2)  # pylint: disable=no-member
 
         fig, ax = _view.common.get_figure(new_fig=False, subplot=122)
 
         for ip1, p1 in enumerate(ph):
             if ip1 != ip:
-                ax.plot(p1[:2], [ip1, ip1], c='b')
+                ax.plot(p1[:2], [ip1, ip1], c="b")
             else:
-                ax.plot(p1[:2], [ip1, ip1], c='r')
+                ax.plot(p1[:2], [ip1, ip1], c="r")
 
-        kwargs['title'] = kwargs.get('title', 'Barcode of p.h.')
-        kwargs['xlabel'] = kwargs.get('xlabel', 'Lifetime')
-        kwargs['ylabel'] = kwargs.get('ylabel', '')
+        all_kwargs = {
+            "title": "Persistence barcode",
+            "xlabel": "Lifetime",
+            "ylabel": "",
+        }
+        all_kwargs.update(kwargs)
 
         _view.common.plt.ylim([-1, len(ph)])
 
-        _view.common.plot_style(fig, ax, **kwargs)
+        _view.common.plot_style(fig, ax, **all_kwargs)
 
         if output_dir is not None:
-            kwargs['output_path'] = output_dir
-            kwargs['output_name'] = 'barcode_' + '0'*(2-len(str(len(tree.get_bifurcations()) - ip))) + str(len(tree.get_bifurcations()) - ip)
+            all_kwargs["output_path"] = output_dir
+            all_kwargs["output_name"] = (
+                "barcode_"
+                + "0" * (2 - len(str(len(tree.get_bifurcations()) - ip)))
+                + str(len(tree.get_bifurcations()) - ip)
+            )
 
-        _view.common.save_plot(fig, **kwargs)     
+        _view.common.save_plot(fig, **all_kwargs)
 
-        if output_dir is not None:
-            kwargs['output_path'] = None
-            kwargs['output_name'] = None
 
+def ph_diagram_tree(tree, new_fig=True, plane="xy", output_dir=None, **kwargs):
+    """Generate a 2d figure (barcode) of the persistent homology of a tree.
 
-def ph_diagram_tree(tree, new_fig=True, plane='xy', output_dir=None, **kwargs):
+    This persistent homology is supposed to be computed by the Topology.get_persistent_homology()
+    method.
     """
-    Generates a 2d figure (barcode) of the persistent homology
-    of a tree as it has been computed by
-    Topology.get_persistent_homology method.
-    """
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, dim=plane)
     else:
-        raise Exception('Plane value not recognised')
+        raise Exception("Plane value not recognised")
 
     bounds = max(max(ph))
 
     for ip, p in enumerate(ph):
-
         ph[ip].append(_np.abs(p[0] - p[1]))
 
     ph.sort(key=lambda x: x[2])
 
     for ip, p in enumerate(ph):
-
         fig, ax = _view.tree(tree, new_fig=new_fig, subplot=121, plane=plane)
 
         c1 = _view.common.plt.Circle([tree.x[0], tree.y[0]], p[0], alpha=0.2)
         c2 = _view.common.plt.Circle([tree.x[0], tree.y[0]], p[1], alpha=0.2)
 
-        ax.add_patch(c1) # pylint: disable=no-member
-        ax.add_patch(c2) # pylint: disable=no-member
+        ax.add_patch(c1)  # pylint: disable=no-member
+        ax.add_patch(c2)  # pylint: disable=no-member
 
         fig, ax = _view.common.get_figure(new_fig=False, subplot=122)
 
         for ip1, p1 in enumerate(ph):
             if ip1 != ip:
-                ax.scatter(p1[0], p1[1], c='b')
+                ax.scatter(p1[0], p1[1], c="b")
             else:
-                ax.scatter(p1[0], p1[1], c='r', s=50)
+                ax.scatter(p1[0], p1[1], c="r", s=50)
 
-        kwargs['title'] = kwargs.get('title', 'P.H. diagram')
-        kwargs['xlabel'] = kwargs.get('xlabel', 'Birth')
-        kwargs['ylabel'] = kwargs.get('ylabel', 'Death')
+        all_kwargs = {
+            "title": "P.H. diagram",
+            "xlabel": "Birth",
+            "ylabel": "Death",
+        }
+        all_kwargs.update(kwargs)
 
-        _view.common.plot_style(fig, ax, **kwargs)
+        _view.common.plot_style(fig, ax, **all_kwargs)
 
         _view.common.plt.plot([0, bounds], [0, bounds])
 
         if output_dir is not None:
-            kwargs['output_path'] = output_dir
-            kwargs['output_name'] = 'ph_' + '0'*(2-len(str(len(tree.get_bifurcations()) - ip))) + str(len(tree.get_bifurcations()) - ip) + '.png'
-
-        _view.common.save_plot(fig, **kwargs)     
-
-        if output_dir is not None:
-            kwargs['output_path'] = None
-            kwargs['output_name'] = None
-
-
-def tree_instance(tree, new_fig=True, plane='xy', component_num=1, feature='radial_distances', diameter=True, col='r', treecol='b', **kwargs):
-    '''Subplot with ph, barcode and tree within spheres
-    '''
-    from tmd import utils as _utils
+            all_kwargs["output_path"] = output_dir
+            all_kwargs["output_name"] = (
+                "ph_"
+                + "0" * (2 - len(str(len(tree.get_bifurcations()) - ip)))
+                + str(len(tree.get_bifurcations()) - ip)
+                + ".png"
+            )
+
+        _view.common.save_plot(fig, **all_kwargs)
+
+
+def tree_instance(
+    tree,
+    new_fig=True,
+    plane="xy",
+    component_num=1,
+    feature="radial_distances",
+    diameter=True,
+    col="r",
+    treecol="b",
+    **kwargs,
+):
+    """Subplot with ph, barcode and tree within spheres."""
     from matplotlib.collections import LineCollection
 
     if new_fig:
-        fig1, ax1 = _view.tree(tree, new_fig=new_fig, subplot=121, plane='xy', title='', treecolor=treecol, diameter=diameter)
+        fig1, ax1 = _view.tree(
+            tree,
+            new_fig=new_fig,
+            subplot=121,
+            plane="xy",
+            title="",
+            treecolor=treecol,
+            diameter=diameter,
+        )
     else:
         fig1, ax1 = _view.common.get_figure(new_fig=new_fig, subplot=121)
-    feat = getattr(tree, 'get_section_' + feature)()
+    feat = getattr(tree, "get_section_" + feature)()
     segs = tree.get_segments()
 
     def _seg_2d(seg):
-        """2d coordinates required for the plotting of a segment"""
-
+        """2d coordinates required for the plotting of a segment."""
         horz = _utils.term_dict[plane[0]]
         vert = _utils.term_dict[plane[1]]
 
         horz1 = seg[0][horz]
         horz2 = seg[1][horz]
         vert1 = seg[0][vert]
         vert2 = seg[1][vert]
 
         return ((horz1, vert1), (horz2, vert2))
 
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, feature=feature)
     else:
-        raise Exception('Plane value not recognised')
-
-    bounds = max(max(ph))
+        raise Exception("Plane value not recognised")
 
     if new_fig:
         fig1, ax2 = barcode(ph, new_fig=False, subplot=222, color=treecol)
-        fig1, ax3 = ph_diagram(ph, new_fig=False, subplot=224, color=treecol)
+        fig1, ax3 = diagram(ph, new_fig=False, subplot=224, color=treecol)
     else:
         fig1, ax2 = _view.common.get_figure(new_fig=new_fig, subplot=222)
         fig1, ax3 = _view.common.get_figure(new_fig=new_fig, subplot=224)
 
     ph = sort_ph(ph)
     select_section = ph[component_num]
 
-    ax2.plot(select_section[:-1], [component_num, component_num], color=col, linewidth=2.)
-    ax3.scatter(select_section[0], select_section[1], color=col, s=50.)
+    ax2.plot(select_section[:-1], [component_num, component_num], color=col, linewidth=2.0)
+    ax3.scatter(select_section[0], select_section[1], color=col, s=50.0)
 
     initial = _np.transpose(tree.get_sections())[_np.where(feat == select_section[0])[0]]
     all_way = _np.array(tree.get_way_to_root(initial[0][1]))
 
     if select_section[1] != -1:
         final = _np.transpose(tree.get_sections())[_np.where(feat == select_section[1])[0]]
         until = _np.array(tree.get_way_to_root(final[0][1]))
@@ -377,490 +416,549 @@
 
     between = _np.setxor1d(all_way, until)
 
     tmp_segs = _np.array(segs)[between]
     toplot_segs = [_seg_2d(seg) for seg in tmp_segs]
     linewidth = [2 * d * 2 for d in _np.array(tree.d)[between]]
 
-    collection = LineCollection(toplot_segs, color=col, linewidth=linewidth, alpha=1.)
+    collection = LineCollection(toplot_segs, color=col, linewidth=linewidth, alpha=1.0)
     ax1.add_collection(collection)
     _view.common.plt.tight_layout(True)
 
     return ax1, collection
 
 
 def customized_cmap():
-    '''Returns a custom cmap'''
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import matplotlib.colors as mcolors
+    """Returns a custom cmap."""
 
     def make_colormap(seq):
-        """Return a LinearSegmentedColormap
+        """Return a LinearSegmentedColormap.
+
         seq: a sequence of floats and RGB-tuples. The floats should be increasing
         and in the interval (0,1).
         """
         seq = [(None,) * 3, 0.0] + list(seq) + [1.0, (None,) * 3]
-        cdict = {'red': [], 'green': [], 'blue': []}
+        cdict = {"red": [], "green": [], "blue": []}
         for i, item in enumerate(seq):
             if isinstance(item, float):
                 r1, g1, b1 = seq[i - 1]
                 r2, g2, b2 = seq[i + 1]
-                cdict['red'].append([item, r1, r2])
-                cdict['green'].append([item, g1, g2])
-                cdict['blue'].append([item, b1, b2])
-        return mcolors.LinearSegmentedColormap('CustomMap', cdict)
-
-    c = mcolors.ColorConverter().to_rgb
+                cdict["red"].append([item, r1, r2])
+                cdict["green"].append([item, g1, g2])
+                cdict["blue"].append([item, b1, b2])
+        return mcolors.LinearSegmentedColormap("CustomMap", cdict)
 
     rvb = make_colormap(
-            [(0.9, 0.9, 0.98), 0.01, (0.8, 0.8, 0.98), 0.05,
-             (0.7, 0.7, 0.98), 0.10, (0.6, 0.6, 0.98), 0.12,
-             (0.5, 0.5, 0.98), 0.15, (0.2, 0.2, 1.0), 0.18,
-             (0.0, 0.5, 1.0), 0.20, (0.0, 0.8, 0.8), 0.25,
-             (0.0, 0.9, 0.5), 0.33, (0.0, 0.95, 0.2), 0.35,
-             (0.4, 0.95, 0.2), 0.4, (0.6, 0.95, 0.1), 0.45,
-             (0.98, 0.95, 0.0), 0.5, (0.99, 0.99, 0.0), 0.55,
-             (0.99, 0.8, 0.0), 0.60, (0.99, 0.65, 0.0), 0.67,
-             (0.99, 0.45, 0.0), 0.7, (0.99, 0.15, 0.0), 0.75,
-             (1.0, 0.0, 0.0), 0.8, (0.9, 0.0, 0.0), 0.85,
-             (0.75, 0.0, 0.0), 0.999, (0.55, 0.0, 0.0)])
+        [
+            (0.9, 0.9, 0.98),
+            0.01,
+            (0.8, 0.8, 0.98),
+            0.05,
+            (0.7, 0.7, 0.98),
+            0.10,
+            (0.6, 0.6, 0.98),
+            0.12,
+            (0.5, 0.5, 0.98),
+            0.15,
+            (0.2, 0.2, 1.0),
+            0.18,
+            (0.0, 0.5, 1.0),
+            0.20,
+            (0.0, 0.8, 0.8),
+            0.25,
+            (0.0, 0.9, 0.5),
+            0.33,
+            (0.0, 0.95, 0.2),
+            0.35,
+            (0.4, 0.95, 0.2),
+            0.4,
+            (0.6, 0.95, 0.1),
+            0.45,
+            (0.98, 0.95, 0.0),
+            0.5,
+            (0.99, 0.99, 0.0),
+            0.55,
+            (0.99, 0.8, 0.0),
+            0.60,
+            (0.99, 0.65, 0.0),
+            0.67,
+            (0.99, 0.45, 0.0),
+            0.7,
+            (0.99, 0.15, 0.0),
+            0.75,
+            (1.0, 0.0, 0.0),
+            0.8,
+            (0.9, 0.0, 0.0),
+            0.85,
+            (0.75, 0.0, 0.0),
+            0.999,
+            (0.55, 0.0, 0.0),
+        ]
+    )
 
     return rvb
 
 
 def gaussian_kernel_resample(ph, num_samples=None, scale_persistent_comp=10):
-    '''Plots the gaussian kernel of the ph diagram that is given.
-    '''
-    from scipy import stats
-    from numpy.random import multivariate_normal
-    import numpy as _np
-
+    """Plot the gaussian kernel of the ph diagram that is given."""
     values = _np.transpose(ph)
     kernel = stats.gaussian_kde(values)
 
     if num_samples is None:
         num_samples = len(ph)
 
     return _np.transpose(kernel.resample(size=num_samples))
 
 
-def gaussian_kernel_rot(ph, new_fig=True, subplot=111, xlims=None, ylims=None, angle=0, **kwargs):
-    '''Plots the gaussian kernel of the ph diagram that is given.
-    '''
-    from scipy import stats
+def gaussian_kernel_rot(ph, new_fig=True, subplot=111, xlim=None, ylim=None, angle=0, **kwargs):
+    """Plot the gaussian kernel of the ph diagram that is given."""
 
     def rotation(x, y, angle=0.0):
-        return [_np.cos(angle)*x - _np.sin(angle)*y,
-                _np.sin(angle)*x + _np.cos(angle)*y]
+        return [_np.cos(angle) * x - _np.sin(angle) * y, _np.sin(angle) * x + _np.cos(angle) * y]
 
     ph_r = [rotation(i[0], i[1], angle=angle) for i in ph]
 
     xmin = min(_np.transpose(ph_r)[0])
     xmax = max(_np.transpose(ph_r)[0])
     ymin = min(_np.transpose(ph_r)[1])
     ymax = max(_np.transpose(ph_r)[1])
 
-    if xlims is None:
-        xlims = [xmin, xmax]
-    if ylims is None:
-        ylims = [ymin, ymax]
+    if xlim is None:
+        xlim = [xmin, xmax]
+    if ylim is None:
+        ylim = [ymin, ymax]
 
-    X, Y = _np.mgrid[xlims[0]:xlims[1]:100j, ylims[0]:ylims[1]:100j]
+    X, Y = _np.mgrid[xlim[0] : xlim[1] : 100j, ylim[0] : ylim[1] : 100j]
 
     values = _np.transpose(ph_r)
     kernel = stats.gaussian_kde(values)
     positions = _np.vstack([X.ravel(), Y.ravel()])
     Z = _np.reshape(kernel(positions).T, X.shape)
     Zn = Z / _np.max(Z)
 
     fig, ax = _view.common.get_figure(new_fig=new_fig, subplot=subplot)
 
-    ax.pcolor(Zn, vmin=0., vmax=1., cmap=_view.common.plt.cm.inferno)
+    ax.pcolor(Zn, vmin=0.0, vmax=1.0, cmap=_view.common.plt.cm.inferno)
 
     return Z, _view.common.plot_style(fig=fig, ax=ax, **kwargs)
 
 
-def gaussian_kernel_weighted(ph, new_fig=True, subplot=111, xlims=None, ylims=None, **kwargs):
-    '''Plots the gaussian kernel of the ph diagram that is given.
-    '''
-    from scipy import stats
+def gaussian_kernel_weighted(ph, new_fig=True, subplot=111, xlim=None, ylim=None, **kwargs):
+    """Plot the gaussian kernel of the ph diagram that is given."""
     xmin = min(_np.transpose(ph)[0])
     xmax = max(_np.transpose(ph)[0])
     ymin = min(_np.transpose(ph)[1])
     ymax = max(_np.transpose(ph)[1])
 
-    if xlims is None:
-        xlims = [xmin, xmax]
-    if ylims is None:
-        ylims = [ymin, ymax]
+    if xlim is None:
+        xlim = [xmin, xmax]
+    if ylim is None:
+        ylim = [ymin, ymax]
 
-    X, Y = _np.mgrid[xlims[0]:xlims[1]:100j, ylims[0]:ylims[1]:100j]
+    X, Y = _np.mgrid[xlim[0] : xlim[1] : 100j, ylim[0] : ylim[1] : 100j]
 
     values = _np.transpose(ph)
     kernel = stats.gaussian_kde(values)
     positions = _np.vstack([X.ravel(), Y.ravel()])
     Z = _np.reshape(kernel(positions).T, X.shape)
     Zn = Z / _np.max(Z)
 
     fig, ax = _view.common.get_figure(new_fig=new_fig, subplot=subplot)
 
-    ax.pcolor(Zn, vmin=0., vmax=1., cmap=_view.common.plt.cm.inferno)
+    ax.pcolor(Zn, vmin=0.0, vmax=1.0, cmap=_view.common.plt.cm.inferno)
 
     return Z, _view.common.plot_style(fig=fig, ax=ax, **kwargs)
 
 
-def gaussian_kernel_superposition(ph, new_fig=True, subplot=111, xlims=None, ylims=None, color='r', **kwargs):
-    '''Plots the gaussian kernel
-       of the ph diagram that is given.
-    '''
-    from scipy import stats
+def gaussian_kernel_superposition(
+    ph, new_fig=True, subplot=111, xlim=None, ylim=None, color="r", **kwargs
+):
+    """Plot the gaussian kernel of the ph diagram that is given."""
     xmin = min(_np.transpose(ph)[0])
     xmax = max(_np.transpose(ph)[0])
     ymin = min(_np.transpose(ph)[1])
     ymax = max(_np.transpose(ph)[1])
 
-    if xlims is None:
-        xlims = [xmin, xmax]
-    if ylims is None:
-        ylims = [ymin, ymax]
+    if xlim is None:
+        xlim = [xmin, xmax]
+    if ylim is None:
+        ylim = [ymin, ymax]
 
-    X, Y = _np.mgrid[xlims[0]:xlims[1]:100j, ylims[0]:ylims[1]:100j]
+    X, Y = _np.mgrid[xlim[0] : xlim[1] : 100j, ylim[0] : ylim[1] : 100j]
 
     values = _np.transpose(ph)
     kernel = stats.gaussian_kde(values)
     positions = _np.vstack([X.ravel(), Y.ravel()])
     Z = _np.reshape(kernel(positions).T, X.shape)
     Zn = Z / _np.max(Z)
-                                                      
+
     fig, ax = _view.common.get_figure(new_fig=new_fig, subplot=subplot)
 
-    ax.pcolor(Zn, vmin=0., vmax=1., cmap=_view.common.plt.cm.inferno)
-    #ax.contour(Z, extent=xlims+ylims)
+    ax.pcolor(Zn, vmin=0.0, vmax=1.0, cmap=_view.common.plt.cm.inferno)
 
     for p in ph:
-
         ax.scatter(p[0], p[1], c=color)
 
-    return _view.common.plot_style(fig=fig, ax=ax, xlim=xlims, ylim=ylims, **kwargs)
-
-
-def tree_br(tree, plane='xy', feature='radial_distances', title='', diameter=True, treecol='b', **kwargs):
-    '''Subplot with ph, barcode
-       and tree within spheres
-    '''
-    from tmd import utils as _utils
-    from matplotlib.collections import LineCollection
-
-    kwargs['output_path'] = kwargs.get('output_path', None)
+    return _view.common.plot_style(fig=fig, ax=ax, xlim=xlim, ylim=ylim, **kwargs)
 
-    fig1, ax1 = _view.tree(tree, new_fig=True, subplot=121, plane='xy',
-                           title=title, treecolor=treecol, diameter=diameter)
 
-    feat = getattr(tree, 'get_section_' + feature)()
-    segs = tree.get_segments()
+def tree_br(
+    tree, plane="xy", feature="radial_distances", title="", diameter=True, treecol="b", **kwargs
+):
+    """Subplot with ph, barcode and tree within spheres."""
+    kwargs["output_path"] = kwargs.get("output_path", None)
+
+    fig1, ax1 = _view.tree(
+        tree,
+        new_fig=True,
+        subplot=121,
+        plane="xy",
+        title=title,
+        treecolor=treecol,
+        diameter=diameter,
+    )
 
     def _seg_2d(seg):
-        """2d coordinates required for the plotting of a segment"""
-
+        """2d coordinates required for the plotting of a segment."""
         horz = _utils.term_dict[plane[0]]
         vert = _utils.term_dict[plane[1]]
 
         horz1 = seg[0][horz]
         horz2 = seg[1][horz]
         vert1 = seg[0][vert]
         vert2 = seg[1][vert]
 
         return ((horz1, vert1), (horz2, vert2))
 
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, feature=feature)
     else:
-        raise Exception('Plane value not recognised')
-
-    bounds = max(max(ph))
+        raise Exception("Plane value not recognised")
 
-    fig1, ax2 = barcode(ph, new_fig=False, subplot=122, color=treecol, ylabel='')
+    fig1, ax2 = barcode(ph, new_fig=False, subplot=122, color=treecol, ylabel="")
 
     _view.common.plt.tight_layout(True)
 
-    if kwargs['output_path'] is not None:
-        fig = _view.common.save_plot(fig=ax1, **kwargs)
+    if kwargs["output_path"] is not None:
+        _view.common.save_plot(fig=ax1, **kwargs)
 
     return fig1, ax1
 
 
-def tree_gaussian_kernel(tree, plane='xy', feature='radial_distances', title='', diameter=True, treecol='b', xlims=None, ylims=None, **kwargs):
-    '''Subplot with ph, barcode
-       and tree within spheres
-    '''
-    from tmd import utils as _utils
-    from matplotlib.collections import LineCollection
-
-    kwargs['output_path'] = kwargs.get('output_path', None)
-
-    fig1, ax1 = _view.tree(tree, new_fig=True, subplot=121, plane='xy',
-                           title=title, treecolor=treecol, diameter=diameter)
-
-    feat = getattr(tree, 'get_section_' + feature)()
-    segs = tree.get_segments()
+def tree_gaussian_kernel(
+    tree,
+    plane="xy",
+    feature="radial_distances",
+    title="",
+    diameter=True,
+    treecol="b",
+    xlim=None,
+    ylim=None,
+    **kwargs,
+):
+    """Subplot with ph, barcode and tree within spheres."""
+    kwargs["output_path"] = kwargs.get("output_path", None)
+
+    fig1, ax1 = _view.tree(
+        tree,
+        new_fig=True,
+        subplot=121,
+        plane="xy",
+        title=title,
+        treecolor=treecol,
+        diameter=diameter,
+    )
 
     def _seg_2d(seg):
-        """2d coordinates required for the plotting of a segment"""
-
+        """2d coordinates required for the plotting of a segment."""
         horz = _utils.term_dict[plane[0]]
         vert = _utils.term_dict[plane[1]]
 
         horz1 = seg[0][horz]
         horz2 = seg[1][horz]
         vert1 = seg[0][vert]
         vert2 = seg[1][vert]
 
         return ((horz1, vert1), (horz2, vert2))
 
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, feature=feature)
     else:
-        raise Exception('Plane value not recognised')
+        raise Exception("Plane value not recognised")
 
-    bounds = max(max(ph))
-
-    fig1, ax2 = gaussian_kernel(ph, new_fig=False, subplot=122, xlims=xlims, ylims=ylims)
+    fig1, ax2 = gaussian_kernel_weighted(ph, new_fig=False, subplot=122, xlim=xlim, ylim=ylim)
 
     _view.common.plt.tight_layout(True)
 
-    if kwargs['output_path'] is not None:
-        fig = _view.common.save_plot(fig=ax1, **kwargs)
+    if kwargs["output_path"] is not None:
+        _view.common.save_plot(fig=ax1, **kwargs)
 
     return fig1, ax1
 
 
-def tree_ph(tree, plane='xy', feature='radial_distances', title='', diameter=True, treecol='b', xlims=None, ylims=None, **kwargs):
-    '''Subplot with ph, barcode
-       and tree within spheres
-    '''
-    from tmd import utils as _utils
-    from matplotlib.collections import LineCollection
-
-    kwargs['output_path'] = kwargs.get('output_path', None)
-
-    fig1, ax1 = _view.tree(tree, new_fig=True, subplot=121, plane='xy',
-                           title=title, treecolor=treecol, diameter=diameter)
-
-    feat = getattr(tree, 'get_section_' + feature)()
-    segs = tree.get_segments()
+def tree_ph(
+    tree,
+    plane="xy",
+    feature="radial_distances",
+    title="",
+    diameter=True,
+    treecol="b",
+    **kwargs,
+):
+    """Subplot with ph, barcode and tree within spheres."""
+    kwargs["output_path"] = kwargs.get("output_path", None)
+
+    fig1, ax1 = _view.tree(
+        tree,
+        new_fig=True,
+        subplot=121,
+        plane="xy",
+        title=title,
+        treecolor=treecol,
+        diameter=diameter,
+    )
 
     def _seg_2d(seg):
-        """2d coordinates required for the plotting of a segment"""
-
+        """2d coordinates required for the plotting of a segment."""
         horz = _utils.term_dict[plane[0]]
         vert = _utils.term_dict[plane[1]]
 
         horz1 = seg[0][horz]
         horz2 = seg[1][horz]
         vert1 = seg[0][vert]
         vert2 = seg[1][vert]
 
         return ((horz1, vert1), (horz2, vert2))
 
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, feature=feature)
     else:
-        raise Exception('Plane value not recognised')
-
-    bounds = max(max(ph))
+        raise Exception("Plane value not recognised")
 
-    fig1, ax2 = ph_diagram(ph, new_fig=False, subplot=122, color=treecol)
+    fig1, ax2 = diagram(ph, new_fig=False, subplot=122, color=treecol)
 
     _view.common.plt.tight_layout(True)
 
-    if kwargs['output_path'] is not None:
-        fig = _view.common.save_plot(fig=ax1, **kwargs)
+    if kwargs["output_path"] is not None:
+        _view.common.save_plot(fig=ax1, **kwargs)
 
     return fig1, ax1
 
 
-def tree_evol(tree, plane='xy', feature='radial_distances', title='', diameter=True, treecol='b', xlims=None, ylims=None, xlim=None, ylim=None, **kwargs):
-    '''Subplot with ph, barcode
-       and tree within spheres
-    '''
-    from tmd import utils as _utils
-    from matplotlib.collections import LineCollection
-
-    kwargs['output_path'] = kwargs.get('output_path', None)
-
-    fig1, ax1 = _view.tree(tree, new_fig=True, subplot=121, plane='xy',
-                           title=title, treecolor=treecol, diameter=diameter)
-
-    feat = getattr(tree, 'get_section_' + feature)()
-    segs = tree.get_segments()
+def tree_evol(
+    tree,
+    plane="xy",
+    feature="radial_distances",
+    title="",
+    diameter=True,
+    treecol="b",
+    barcode_xlim=None,
+    barcode_ylim=None,
+    kernel_xlim=None,
+    kernel_ylim=None,
+    **kwargs,
+):
+    """Subplot with ph, barcode and tree within spheres."""
+    kwargs["output_path"] = kwargs.get("output_path", None)
+
+    fig1, ax1 = _view.tree(
+        tree,
+        new_fig=True,
+        subplot=121,
+        plane="xy",
+        title=title,
+        treecolor=treecol,
+        diameter=diameter,
+    )
 
     def _seg_2d(seg):
-        """2d coordinates required for the plotting of a segment"""
-
+        """2d coordinates required for the plotting of a segment."""
         horz = _utils.term_dict[plane[0]]
         vert = _utils.term_dict[plane[1]]
 
         horz1 = seg[0][horz]
         horz2 = seg[1][horz]
         vert1 = seg[0][vert]
         vert2 = seg[1][vert]
 
         return ((horz1, vert1), (horz2, vert2))
 
-    if plane in ['xy', 'yx', 'zx', 'xz', 'yz', 'zy']:
+    if plane in ["xy", "yx", "zx", "xz", "yz", "zy"]:
         ph = _tm.methods.get_persistence_diagram(tree, feature=feature)
     else:
-        raise Exception('Plane value not recognised')
-
-    bounds = max(max(ph))
-
-    fig1, ax3 = barcode(ph, new_fig=False, subplot=222, color=treecol, xlim=xlim, ylim=ylim)
+        raise Exception("Plane value not recognised")
 
-    fig1, ax4 = gaussian_kernel(ph, new_fig=False, subplot=224, xlims=xlims, ylims=ylims)
+    fig1, ax3 = barcode(
+        ph, new_fig=False, subplot=222, color=treecol, xlim=barcode_xlim, ylim=barcode_ylim
+    )
+
+    fig1, ax4 = gaussian_kernel_weighted(
+        ph, new_fig=False, subplot=224, xlim=kernel_xlim, ylim=kernel_ylim
+    )
 
     _view.common.plt.tight_layout(True)
 
-    if kwargs['output_path'] is not None:
-        fig = _view.common.save_plot(fig=ax1, **kwargs)
+    if kwargs["output_path"] is not None:
+        _view.common.save_plot(fig=ax1, **kwargs)
 
     return fig1, ax1
 
 
-def image_diff_time(Z_sequence, time_steps=100, new_fig=True, subplot=111, xlims=None, ylims=None, **kwargs):
-    """Takes as input a set of images
-       as exported from the gaussian kernel
-       plotting function, and plots
-       their difference.
-    """
-    
-
+def image_diff_time(
+    Z1, Z2, time_steps=100, new_fig=True, subplot=111, xlim=None, ylim=None, **kwargs
+):
+    """Take as input a set of images and plots their difference."""
     xmin = min(Z1[1][1].get_xlim() + Z2[1][1].get_xlim())
     xmax = max(Z1[1][1].get_xlim() + Z2[1][1].get_xlim())
     ymin = min(Z1[1][1].get_ylim() + Z2[1][1].get_ylim())
     ymax = max(Z1[1][1].get_ylim() + Z2[1][1].get_ylim())
 
-    if xlims is None:
-        xlims = [xmin, xmax]
-    if ylims is None:
-        ylims = [ymin, ymax]
+    if xlim is None:
+        xlim = [xmin, xmax]
+    if ylim is None:
+        ylim = [ymin, ymax]
 
-    X, Y = _np.mgrid[xlims[0]:xlims[1]:100j, ylims[0]:ylims[1]:100j]
+    X, Y = _np.mgrid[xlim[0] : xlim[1] : 100j, ylim[0] : ylim[1] : 100j]
 
-    img1 = Z1[0]/Z1[0].max()
-    img2 = Z2[0]/Z2[0].max()
+    img1 = Z1[0] / Z1[0].max()
+    img2 = Z2[0] / Z2[0].max()
 
     fig, ax = _view.common.get_figure(new_fig=new_fig, subplot=subplot)
 
     _view.common.plt.pcolor(X, Y, img2 - img1, vmin=-1.0, vmax=1.0)
 
     _view.common.plt.colorbar()
 
-    kwargs['xlim'] = xlims
-    kwargs['ylim'] = ylims
+    kwargs["xlim"] = xlim
+    kwargs["ylim"] = ylim
 
     return _view.common.plot_style(fig=fig, ax=ax, **kwargs)
 
 
-def plot_simple_tree(tr, plane='xy', new_fig=True, subplot=False, hadd=0.0, vadd=0.0, treecolor='b', alpha=1.0, **kwargs):
-    '''Generates a 2d figure of the tree.
-    '''
+def plot_simple_tree(
+    tr,
+    plane="xy",
+    new_fig=True,
+    subplot=False,
+    hadd=0.0,
+    vadd=0.0,
+    treecolor="b",
+    alpha=1.0,
+    **kwargs,
+):
+    """Generate a 2d figure of the tree."""
     from matplotlib.collections import LineCollection
-    from tmd import utils as _utils
 
     # Initialization of matplotlib figure and axes.
     fig, ax = _view.common.get_figure(new_fig=new_fig, subplot=subplot)
 
     # Data needed for the viewer: x,y,z,r
     bounding_box = tr.get_bounding_box()
 
     def _seg_2d(seg, x_add=0.0, y_add=0.0):
-
-        """2d coordinates required for the plotting of a segment"""
-
+        """2d coordinates required for the plotting of a segment."""
         horz = _utils.term_dict[plane[0]]
         vert = _utils.term_dict[plane[1]]
 
         horz1 = seg[0][horz] + x_add
         horz2 = seg[1][horz] + x_add
         vert1 = seg[0][vert] + y_add
         vert2 = seg[1][vert] + y_add
 
         return ((horz1, vert1), (horz2, vert2))
 
     segs = [_seg_2d(seg, hadd, vadd) for seg in tr.get_segments()]
 
     linewidth = [2 * d * 1.0 for d in tr.d]
 
-    #treecolor = 'b'
-
     # Plot the collection of lines.
-    collection = LineCollection(segs, color=treecolor, linewidth=linewidth,
-                                alpha=alpha)
+    collection = LineCollection(segs, color=treecolor, linewidth=linewidth, alpha=alpha)
 
     ax.add_collection(collection)
 
-    kwargs['xlim'] = kwargs.get('xlim', [bounding_box[0][_utils.term_dict[plane[0]]] - 20,
-                                         bounding_box[1][_utils.term_dict[plane[0]]] + 20])
-    kwargs['ylim'] = kwargs.get('ylim', [bounding_box[0][_utils.term_dict[plane[1]]] - 20,
-                                         bounding_box[1][_utils.term_dict[plane[1]]] + 20])
-
-    return _view.common.plot_style(fig=fig, ax=ax, **kwargs)
+    all_kwargs = {
+        "xlim": [
+            bounding_box[0][_utils.term_dict[plane[0]]] - 20,
+            bounding_box[1][_utils.term_dict[plane[0]]] + 20,
+        ],
+        "ylim": [
+            bounding_box[0][_utils.term_dict[plane[1]]] - 20,
+            bounding_box[1][_utils.term_dict[plane[1]]] + 20,
+        ],
+    }
+    all_kwargs.update(kwargs)
 
+    return _view.common.plot_style(fig=fig, ax=ax, **all_kwargs)
 
-def plot_intermediate(ph_all, colors_bar, tree, colors, counter, linewidth=1., output_path='./'):
-    '''plots the tree and the barcode with defined colors'''
 
+def plot_intermediate(ph_all, colors_bar, tree, colors, counter, linewidth=1.0, output_path="./"):
+    """Plot the tree and the barcode with defined colors."""
     fig, ax1 = _view.common.get_figure(new_fig=True, subplot=122)
 
     for ipers, pers in enumerate(ph_all):
         ax1.plot(pers[:2], [ipers, ipers], c=colors_bar[ipers], linewidth=linewidth)
-        ax1.set_title('Barcode', fontsize=14)
+        ax1.set_title("Barcode", fontsize=14)
 
     ax1.set_ylim([-1, len(ph_all)])
     ax1.set_xlim([-10, _np.max(ph_all)])
 
-    ax1.set_xlabel('Distance from soma', fontsize=14)
+    ax1.set_xlabel("Distance from soma", fontsize=14)
 
-    ax1.spines['right'].set_visible(False)
-    ax1.spines['top'].set_visible(False)
+    ax1.spines["right"].set_visible(False)
+    ax1.spines["top"].set_visible(False)
     # ax1.spines['left'].set_visible(False)
-    ax1.yaxis.set_ticks_position('left')
-    ax1.xaxis.set_ticks_position('bottom')
+    ax1.yaxis.set_ticks_position("left")
+    ax1.xaxis.set_ticks_position("bottom")
     ax1.set_yticks([])
 
     fig, ax2 = plot_simple_tree(tree, new_fig=False, subplot=121, treecolor=colors, diameter=False)
 
-    ax2.spines['right'].set_visible(False)
-    ax2.spines['top'].set_visible(False)
-    ax2.spines['left'].set_visible(False)
-    ax2.yaxis.set_ticks_position('left')
-    ax2.xaxis.set_ticks_position('bottom')
+    ax2.spines["right"].set_visible(False)
+    ax2.spines["top"].set_visible(False)
+    ax2.spines["left"].set_visible(False)
+    ax2.yaxis.set_ticks_position("left")
+    ax2.xaxis.set_ticks_position("bottom")
     ax2.set_yticks([])
 
-    _view.common.plot_style(fig=fig, ax=ax2, output_path=output_path,
-                            title='Morphology', tight=True, xlabel='Length (um)', ylabel='',
-                            output_name=str(0)*(3 - len(str(counter))) + str(counter))
-
-
-def plot_persistent_homology_video(tree, feature='radial_distances', linewidth=1.0, c1='b', c2='w', c3='w', c4='b', c5='r', output_path='./', **kwargs):
-    '''Method to extract ph from tree that contains mutlifurcations
-    and generate a video of the process'''
-
+    _view.common.plot_style(
+        fig=fig,
+        ax=ax2,
+        output_path=output_path,
+        title="Morphology",
+        tight=True,
+        xlabel="Length (um)",
+        ylabel="",
+        output_name=str(0) * (3 - len(str(counter))) + str(counter),
+    )
+
+
+def plot_persistent_homology_video(
+    tree,
+    feature="radial_distances",
+    linewidth=1.0,
+    c1="b",
+    c2="w",
+    c3="w",
+    c4="b",
+    c5="r",
+    output_path="./",
+    **kwargs,
+):
+    """Extract ph from tree that contains mutlifurcations and generate a video of the process."""
     ph_all = _tm.methods.get_persistence_diagram(tree)
 
     ph_all = _sort_ph_initial(ph_all)
 
-    colors_bar = _np.array([c4 for s in xrange(len(ph_all))])
+    colors_bar = _np.array([c4 for s in range(len(ph_all))])
 
     ph = []
 
-    rd = getattr(tree, 'get_point_' + feature)(**kwargs)
+    rd = getattr(tree, "get_point_" + feature)(**kwargs)
 
-    colors = _np.array([c1 for s in xrange(len(tree.x) - 1)])
+    colors = _np.array([c1 for s in range(len(tree.x) - 1)])
 
     counter = 5
 
     plot_intermediate(ph_all, colors_bar, tree, colors, counter, output_path=output_path)
 
     counter = counter + 1
 
@@ -870,62 +968,61 @@
 
     beg = _np.array(beg)
     end = _np.array(end)
 
     parents = {e: b for b, e in zip(beg, end)}
     children = {b: end[_np.where(beg == b)[0]] for b in _np.unique(beg)}
 
-    colors_bar = _np.array([c3 for s in xrange(len(ph_all))])
+    colors_bar = _np.array([c3 for s in range(len(ph_all))])
 
     plot_intermediate(ph_all, colors_bar, tree, colors, counter, output_path=output_path)
 
     counter = counter + 1
 
     active_paths = {}
 
     while len(_np.where(active)[0]) > 1:
         alive = list(_np.where(active)[0])
 
-        for l in alive:
-
-            p = parents[l]
+        for i in alive:
+            p = parents[i]
             c = children[p]
 
             if _np.alltrue(active[c]):
-
                 to_modify = []
                 to_modify_bars = []
 
                 active[p] = True
                 active[c] = False
 
                 mx = _np.argmax(abs(rd[c]))
                 mx_id = c[mx]
 
                 alive.remove(mx_id)
                 c = _np.delete(c, mx)
 
                 for ci in c:
                     ph.append([rd[ci], rd[p]])
-                    #colors_bar[_np.where(_np.array(ph_all) == [rd[ci], rd[p]])[0][1]] = c4
-                    to_modify_bars = to_modify_bars + [_np.where(_np.array(ph_all) == [rd[ci], rd[p]])[0][1]]
+                    # colors_bar[_np.where(_np.array(ph_all) == [rd[ci], rd[p]])[0][1]] = c4
+                    to_modify_bars = to_modify_bars + [
+                        _np.where(_np.array(ph_all) == [rd[ci], rd[p]])[0][1]
+                    ]
 
                     alive.remove(ci)
-                    
+
                     # colors[tree.get_way_to_section_start(ci - 1)] = c2
                     to_modify = to_modify + tree.get_way_to_section_start(ci - 1)
 
                     if ci < len(colors):
                         # colors[ci] = c2
                         to_modify = to_modify + [ci]
 
                     key = int(ci)
 
                     while key in active_paths:
-
                         # colors[tree.get_way_to_section_start(active_paths[key] - 1)] = c2
                         to_modify = to_modify + tree.get_way_to_section_start(active_paths[key] - 1)
                         if active_paths[key] < len(colors):
                             # colors[active_paths[key]] = c2
                             to_modify = to_modify + [active_paths[key]]
                         key = active_paths.pop(key)
 
@@ -934,28 +1031,32 @@
                 alive.append(p)
 
                 rd[p] = rd[mx_id]
 
                 colors[to_modify] = c5
                 colors_bar[to_modify_bars] = c5
 
-                plot_intermediate(ph_all, colors_bar, tree, colors, counter, output_path=output_path)
+                plot_intermediate(
+                    ph_all, colors_bar, tree, colors, counter, output_path=output_path
+                )
 
                 counter = counter + 1
 
                 colors[to_modify] = c2
                 colors_bar[to_modify_bars] = c4
 
-                plot_intermediate(ph_all, colors_bar, tree, colors, counter, output_path=output_path)
+                plot_intermediate(
+                    ph_all, colors_bar, tree, colors, counter, output_path=output_path
+                )
 
                 counter = counter + 1
 
     to_modify = []
 
-    ph.append([rd[_np.where(active)[0][0]], 0]) # Add the last alive component
+    ph.append([rd[_np.where(active)[0][0]], 0])  # Add the last alive component
 
     key = int(_np.where(active)[0][0])
     way = tree.get_way_to_section_start(key - 1)
     way.remove(-1)
     # colors[way] = c2
     to_modify = to_modify + way
 
@@ -985,44 +1086,57 @@
 
     plot_intermediate(ph_all, colors_bar, tree, colors, counter, output_path=output_path)
 
     # plot_intermediate(ph_all, colors_bar, tree, colors, counter)
 
     return ph
 
-def multiple_trees_plot(trees, phs, xlim=None, ylim=None, title_1='Asymmetry'):
-    fig = plt.figure()
-    N = len(trees)
-    lims = [np.min(np.min(phs)) - 5 , np.max(np.max(phs)) + 5]
-
-    for i,tr in enumerate(trees):
-        view.view.tree(tr, new_fig=False, subplot=(3,N,i+1),
-                       title=title_1, plane='xy',
-                       diameter=False, linewidth=0.8, treecolor='black')
-
-        view.plot.barcode(phs[i], new_fig=False, subplot=(3,N,i+1+N) , title='', xlim=lims)
-        view.plot.ph_image(phs[i], new_fig=False, subplot=(3,N,i+1+2*N) , title='', xlims=lims, ylims=lims)
 
+def multiple_trees_plot(trees, phs, title_1="Asymmetry"):
+    """Plot multiple trees."""
+    plt.figure()
+    N = len(trees)
+    lims = [_np.min(_np.min(phs)) - 5, _np.max(_np.max(phs)) + 5]
 
-def polar_plot_custom_color(population, bins=25, apical_color='purple', basal_color='r',
-                            edgecolor=None, alpha=0.8):
-    '''
-    '''
+    for i, tr in enumerate(trees):
+        view.view.tree(
+            tr,
+            new_fig=False,
+            subplot=(3, N, i + 1),
+            title=title_1,
+            plane="xy",
+            diameter=False,
+            linewidth=0.8,
+            treecolor="black",
+        )
+
+        view.plot.barcode(phs[i], new_fig=False, subplot=(3, N, i + 1 + N), title="", xlim=lims)
+        view.plot.persistence_image(
+            phs[i], new_fig=False, subplot=(3, N, i + 1 + 2 * N), title="", xlim=lims, ylim=lims
+        )
+
+
+def polar_plot_custom_color(
+    population, bins=25, apical_color="purple", basal_color="r", edgecolor=None, alpha=0.8
+):
+    """Plot a population."""
     fig = _cm.plt.figure()
     ax = fig.add_axes([0.1, 0.1, 0.8, 0.8], polar=True)
 
-    input_data1 = _get_polar_data(population, neurite_type='basal', bins=bins)
-    input_data2 = _get_polar_data(population, neurite_type='apical', bins=bins)
+    input_data1 = view.view._get_polar_data(population, neurite_type="basal_dendrite", bins=bins)
+    input_data2 = view.view._get_polar_data(population, neurite_type="apical_dendrite", bins=bins)
 
-    maximum = _np.max(_np.array(input_data1)[:,2].tolist() + _np.array(input_data2)[:,2].tolist())
+    maximum = _np.max(_np.array(input_data1)[:, 2].tolist() + _np.array(input_data2)[:, 2].tolist())
 
-    theta = _np.array(input_data1)[:,0]
-    radii = _np.array(input_data1)[:,2] / maximum
+    theta = _np.array(input_data1)[:, 0]
+    radii = _np.array(input_data1)[:, 2] / maximum
     width = 2 * _np.pi / len(input_data1)
-    bars = ax.bar(theta, radii, width=width, edgecolor=edgecolor,
-                  bottom=0.0, alpha=alpha, color=basal_color)
+    ax.bar(
+        theta, radii, width=width, edgecolor=edgecolor, bottom=0.0, alpha=alpha, color=basal_color
+    )
 
-    theta = _np.array(input_data2)[:,0]
-    radii = _np.array(input_data2)[:,2] / maximum
+    theta = _np.array(input_data2)[:, 0]
+    radii = _np.array(input_data2)[:, 2] / maximum
     width = 2 * _np.pi / len(input_data2)
-    bars = ax.bar(theta, radii, width=width, edgecolor=edgecolor,
-                  bottom=0.0, alpha=alpha, color=apical_color)
+    ax.bar(
+        theta, radii, width=width, edgecolor=edgecolor, bottom=0.0, alpha=alpha, color=apical_color
+    )
```

### Comparing `tmd-2.2.0/examples/Advanced/classification.py` & `TMD-2.3.0/examples/Advanced/classification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,210 +1,215 @@
-list_of_modules = ['discriminant_analysis', 'discriminant_analysis', 'tree']
+"""Example script of classification."""
+import numpy as np
 
-list_of_classifiers = ['LinearDiscriminantAnalysis',
-                       'QuadraticDiscriminantAnalysis', 'DecisionTreeClassifier']
+list_of_modules = ["discriminant_analysis", "discriminant_analysis", "tree"]
+
+list_of_classifiers = [
+    "LinearDiscriminantAnalysis",
+    "QuadraticDiscriminantAnalysis",
+    "DecisionTreeClassifier",
+]
 
 
 def train(mod, classifier, data, labels, **kwargs):
-    '''Trains the classifier from mod of sklearn
-       with data and targets.
-       Returns a fited classifier.
-    '''
+    """Trains the classifier from mod of sklearn with data and targets.
+
+    Returns a fited classifier.
+    """
     import importlib
 
-    clas_mod = importlib.import_module('sklearn.' + mod)
+    clas_mod = importlib.import_module("sklearn." + mod)
     clf = getattr(clas_mod, classifier)()
     clf.set_params(**kwargs)
 
     clf.fit(data, labels)
 
     return clf
 
 
 def predict(clf, data):
-    '''Predict label for data for the trained classifier clf.
-       Returns the index of the predicted class
-       for each datapoint in data.
-    '''
+    """Predict label for data for the trained classifier clf.
+
+    Returns the index of the predicted class for each datapoint in data.
+    """
     predict_label = clf.predict([data])
 
     return predict_label[0]
 
 
 def leave_one_out(mod, classifier, data, labels, **kwargs):
-    '''Leaves one individual out, trains classifier
-       with the rest of the data and returns the score
-       of matching ids between proposed and predicted labels.
-       Score defines how many trials were successful
-       as a percentage over the total number of trials.
-    '''
+    """Leaves one individual out and trains classifier with the rest of the data.
+
+    Returns the score of matching ids between proposed and predicted labels.
+    Score defines how many trials were successful as a percentage over the total number of trials.
+    """
     sample_size = len(labels)
     scores = np.zeros(sample_size)
 
     for ed in range(sample_size):
-
-        # print 'Testing ' + str(ed) + ' ...'
+        # print('Testing ' + str(ed) + ' ...')
 
         train_data = data[np.delete(range(sample_size), ed)]
         train_labels = labels[np.delete(range(sample_size), ed)]
 
         clf = train(mod, classifier, train_data, train_labels, **kwargs)
         predict_label = predict(clf, data[ed])
 
-        # print 'The individual ' + str(ed) + ' is of type ' + str(predict_label)
+        # print('The individual ' + str(ed) + ' is of type ' + str(predict_label))
 
         scores[ed] = predict_label == labels[ed]
 
     return np.float(np.count_nonzero(scores)) / sample_size
 
 
 def leave_one_out_statistics(mod, classifier, data, labels, N=10, **kwargs):
-    '''Leaves one individual out, trains classifier
-       with the rest of the data and returns the score
-       of matching ids between proposed and predicted labels.
-       Score defines how many trials were successful
-       as a percentage over the total number of trials.
-    '''
+    """Leaves one individual out and trains classifier with the rest of the data.
+
+    Returns the score of matching ids between proposed and predicted labels.
+    Score defines how many trials were successful
+    as a percentage over the total number of trials.
+    """
     sample_size = len(labels)
     scores = np.zeros(sample_size)
 
     for ed in range(sample_size):
-
-        # print 'Testing ' + str(ed) + ' ...'
+        # print('Testing ' + str(ed) + ' ...')
 
         train_data = data[np.delete(range(sample_size), ed)]
         train_labels = labels[np.delete(range(sample_size), ed)]
 
         clf = train(mod, classifier, train_data, train_labels, **kwargs)
 
         all_results = []
         for i in range(N):
             all_results.append(predict(clf, data[ed]))
 
         predict_label = predict(clf, data[ed])
-        print 'The individual ', str(ed), ' is of type ', all_results
+        print("The individual ", str(ed), " is of type ", all_results)
 
         scores[ed] = predict_label == labels[ed]
 
     return np.float(np.count_nonzero(scores)) / sample_size
 
 
 def leave_perc_out(mod, classifier, data, labels, iterations=10, percent=10, **kwargs):
-    '''Leaves one individual out, trains classifier
-       with the rest of the data and returns the score
-       of matching ids between proposed and predicted labels.
-       Score defines how many trials were successful
-       as a percentage over the total number of trials.
-       Iteration defines the number of trials.
-       Percent defines the percentage of the data that will
-       define the test set of the classifier.
-    '''
+    """Leaves one individual out and trains classifier with the rest of the data.
+
+    Returns the score of matching ids between proposed and predicted labels.
+    Score defines how many trials were successful
+    as a percentage over the total number of trials.
+    Iteration defines the number of trials.
+    Percent defines the percentage of the data that will
+    define the test set of the classifier.
+    """
     import random
 
     sample_size = len(labels)
-    test_size = int(sample_size * percent / 100.)
+    test_size = int(sample_size * percent / 100.0)
     scores = np.zeros(iterations)
 
-    # print sample_size, test_size
+    # print(sample_size, test_size)
 
     for i in range(iterations):
-
         random_inds = random.sample(range(0, sample_size), test_size)
         kept = np.delete(range(sample_size), random_inds)
 
         clf = train(mod, classifier, data[kept], labels[kept], **kwargs)
 
         sc = 0.0
         for ed in random_inds:
             predict_label = predict(clf, data[ed])
             sc = sc + float(predict_label == labels[ed])
 
         scores[i] = float(sc) / float(test_size)
 
-    # print len(random_inds), len(kept), len(random_inds) + len(kept)
+    # print(len(random_inds), len(kept), len(random_inds) + len(kept))
 
     return scores  # np.mean(np.count_nonzero(scores))/sample_size
 
 
 def leave_one_out_mixing(mod, classifier, data, labels, **kwargs):
-    '''Leaves one individual out, trains classifier
-       with the rest of the data and returns the score
-       of matching ids between proposed and predicted labels.
-       Score defines how many trials were successful
-       as a percentage over the total number of trials.
-    '''
+    """Leaves one individual out and trains classifier with the rest of the data.
+
+    Returns the score of matching ids between proposed and predicted labels.
+    Score defines how many trials were successful
+    as a percentage over the total number of trials.
+    """
     sample_size = len(labels)
     scores = np.zeros(sample_size)
 
     separation = np.zeros([len(np.unique(labels)), len(np.unique(labels))])
 
     sizes = np.zeros(len(np.unique(labels)))
 
     for i in np.unique(labels):
         sizes[int(i - 1)] = len(np.where(labels == i)[0])
 
     for ed in range(sample_size):
-
-        # print 'Testing ' + str(ed) + ' ...'
+        # print('Testing ' + str(ed) + ' ...')
 
         train_data = data[np.delete(range(sample_size), ed)]
         train_labels = labels[np.delete(range(sample_size), ed)]
 
         clf = train(mod, classifier, train_data, train_labels, **kwargs)
         predict_label = predict(clf, data[ed])
 
-        # print predict_label, labels[ed]
-        separation[int(labels[ed] - 1)][int(predict_label - 1)] = separation[int(labels[ed] - 1)
-                                                                             ][int(predict_label - 1)] + 1. / sizes[int(labels[ed] - 1)]
+        # print(predict_label, labels[ed])
+        separation[int(labels[ed] - 1)][int(predict_label - 1)] = (
+            separation[int(labels[ed] - 1)][int(predict_label - 1)]
+            + 1.0 / sizes[int(labels[ed] - 1)]
+        )
 
-        # print 'The individual ' + str(ed) + ' is of type ' + str(predict_label)
+        # print('The individual ' + str(ed) + ' is of type ' + str(predict_label))
 
         scores[ed] = predict_label == labels[ed]
 
     return np.float(np.count_nonzero(scores)) / sample_size, separation
 
 
 def leave_one_out_multiple(mod, classifier, data, labels, n=10, **kwargs):
-    '''Leaves one individual out, trains classifier
-       with the rest of the data and returns the score
-       of matching ids between proposed and predicted labels.
-       Score defines how many trials were successful
-       as a percentage over the total number of trials.
-    '''
+    """Leaves one individual out and trains classifier with the rest of the data.
+
+    Returns the score of matching ids between proposed and predicted labels.
+    Score defines how many trials were successful
+    as a percentage over the total number of trials.
+    """
     sample_size = len(labels)
     scores = np.zeros(sample_size)
 
     for ed in range(sample_size):
+        # print('Testing ' + str(ed) + ' ...')
 
-        # print 'Testing ' + str(ed) + ' ...'
-
-        print 'The individual ' + str(ed) + ' is of type ',
+        print("The individual " + str(ed) + " is of type ")
 
         for ni in range(n):
-
             train_data = data[np.delete(range(sample_size), ed)]
             train_labels = labels[np.delete(range(sample_size), ed)]
 
             clf = train(mod, classifier, train_data, train_labels, **kwargs)
 
             predict_label = predict(clf, data[ed])
 
-            print str(predict_label),
+            print(
+                str(predict_label),
+            )
 
-        print ' !'
+        print(" !")
 
         scores[ed] = predict_label == labels[ed]
 
     return np.float(np.count_nonzero(scores)) / sample_size
 
 
-def multi(dat, tar, m='tree', cl='DecisionTreeClassifier', n=10, randomize=False):
+def multi(dat, tar, m="tree", cl="DecisionTreeClassifier", n=10, randomize=False):
+    """TODO: Add docstring."""
     score = np.zeros(n)
     if not randomize:
         for i in range(n):
             score[i] = leave_one_out(m, cl, dat, tar)
     else:
         for i in range(n):
-            score[i] = leave_one_out(m, cl, dat, np.random.randint(
-                min(tar), max(tar) + 1, size=len(tar)))
+            score[i] = leave_one_out(
+                m, cl, dat, np.random.randint(min(tar), max(tar) + 1, size=len(tar))
+            )
 
-    return mean(score), std(score)
+    return np.mean(score), np.std(score)
```

### Comparing `tmd-2.2.0/examples/Advanced/diversity_index.py` & `TMD-2.3.0/examples/Advanced/diversity_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,120 @@
-# Example script to compute the diversity index from a set of classes.
+"""Example script to compute the diversity index from a set of classes."""
+import numpy as np
 
 
 def diversity_index(perc, simil, q):
-    """Computes the generalized diversity index
-       as described in http://onlinelibrary.wiley.com/doi/10.1890/10-2402.1/abstract
-       Inputs:
-            perc: list of percentages of species distribution
-            of size S.
-            simil: confusion matrix indicating the similarity
-            between species of size SxS.
-            q: the order of diversity index.
-    """
-    import numpy as np
+    """Computes the generalized diversity index.
+
+    The diversity index is described in
+    http://onlinelibrary.wiley.com/doi/10.1890/10-2402.1/abstract
 
+    Inputs:
+         perc: list of percentages of species distribution
+         of size S.
+         simil: confusion matrix indicating the similarity
+         between species of size SxS.
+         q: the order of diversity index.
+    """
     perc = np.array(perc, dtype=float) / sum(perc)
 
     diq = 0.0
 
     for i in range(len(perc)):
         zpi = np.dot(simil[i], perc)
-        diq = diq + np.power(perc[i], q) * np.power(zpi, q - 1.)
+        diq = diq + np.power(perc[i], q) * np.power(zpi, q - 1.0)
 
-    return np.power(diq, 1. / (1. - q))
+    return np.power(diq, 1.0 / (1.0 - q))
 
 
 def diversity_index_inf(perc, simil):
-    """Computes the generalized diversity index
-       as described in http://onlinelibrary.wiley.com/doi/10.1890/10-2402.1/abstract
-       Inputs:
-            perc: list of percentages of species distribution
-            of size S.
-            simil: confusion matrix indicating the similarity
-            between species of size SxS.
-            q: the order of diversity index is set to inf
-    """
-    import numpy as np
+    """Computes the generalized diversity index.
 
+    The diversity index is described in
+    http://onlinelibrary.wiley.com/doi/10.1890/10-2402.1/abstract
+
+    Inputs:
+         perc: list of percentages of species distribution
+         of size S.
+         simil: confusion matrix indicating the similarity
+         between species of size SxS.
+         q: the order of diversity index is set to inf
+    """
     diq = np.inf
 
     perc = np.array(perc, dtype=float) / sum(perc)
 
     for i in range(len(perc)):
         zpi = np.dot(simil[i], perc)
         diq = min(diq, zpi)
 
-    return np.float(1.) / diq
+    return np.float(1.0) / diq
 
 
 def diversity_index_one(perc, simil):
-    """Computes the generalized diversity index
-       as described in http://onlinelibrary.wiley.com/doi/10.1890/10-2402.1/abstract
-       Inputs:
-            perc: list of percentages of species distribution
-            of size S.
-            simil: confusion matrix indicating the similarity
-            between species of size SxS.
-            q: the order of diversity index is set to one
-    """
-    import numpy as np
+    """Computes the generalized diversity index.
 
+    The diversity index is described in
+    http://onlinelibrary.wiley.com/doi/10.1890/10-2402.1/abstract
+
+    Inputs:
+         perc: list of percentages of species distribution
+         of size S.
+         simil: confusion matrix indicating the similarity
+         between species of size SxS.
+         q: the order of diversity index is set to one
+    """
     diq = 1.0
 
     perc = np.array(perc, dtype=float) / sum(perc)
 
     for i in range(len(perc)):
         zpi = np.dot(simil[i], perc)
         diq = diq * np.power(zpi, perc[i])
 
-    return np.float(1.) / diq
+    return np.float(1.0) / diq
 
 
 def diversity_index_zero(perc, simil):
-    """Computes the generalized diversity index
-       as described in http://onlinelibrary.wiley.com/doi/10.1890/10-2402.1/abstract
-       Inputs:
-            perc: list of percentages of species distribution
-            of size S.
-            simil: confusion matrix indicating the similarity
-            between species of size SxS.
-            q: the order of diversity index is set to one
-    """
-    import numpy as np
+    """Computes the generalized diversity index.
 
+    The diversity index is described in
+    http://onlinelibrary.wiley.com/doi/10.1890/10-2402.1/abstract
+
+    Inputs:
+         perc: list of percentages of species distribution
+         of size S.
+         simil: confusion matrix indicating the similarity
+         between species of size SxS.
+         q: the order of diversity index is set to one
+    """
     diq = 1.0
 
     perc = np.array(perc, dtype=float) / sum(perc)
 
     for i in range(len(perc)):
         zpi = np.dot(simil[i], perc)
         diq = diq * np.power(zpi, perc[i])
 
-    return np.float(1.) / diq
+    return np.float(1.0) / diq
 
     perc = np.array(perc, dtype=float) / sum(perc)
 
     diq = 0.0
 
     for i in range(len(perc)):
         zpi = np.dot(simil[i], perc)
         if not np.close(zpi, 0.0):
             diq = diq + perc[i] / zpi
 
     return diq
 
 
 def diversity_vary_q(perc, simil, dep=np.linspace(0.05, 0.95, 20).tolist() + range(2, 10)):
-    """Computes the diversity index
-       with different q values:
-       from q=0 to q=infinity
-    """
+    """Computes the diversity index with different q values: from q=0 to q=infinity."""
     # div_index = [diversity_index_zero(perc, simil), diversity_index_one(perc, simil)]
 
     div_index = [diversity_index(perc, simil, q) for q in dep]
 
     # div_index = div_index + [diversity_index_inf(perc, simil)]
 
     return dep, div_index
```

### Comparing `tmd-2.2.0/examples/Advanced/matching.py` & `TMD-2.3.0/examples/Advanced/matching.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-'''
-tmd matching algorithms implementation
-'''
+"""TMD matching algorithms implementation."""
+import numpy as np
 
 
 def marriage_problem(women_preferences, men_preferences):
-    '''Matches N women to M men so that max(M, N)
-    are coupled to their preferred choice that is available
+    """Matches N women to M men so that max(M, N) are coupled to their preferred available choice.
+
     See https://en.wikipedia.org/wiki/Stable_marriage_problem
-    '''
+    """
     N = len(women_preferences)
     M = len(men_preferences)
 
     swapped = False
 
     if M > N:
         swap = women_preferences
@@ -45,57 +44,56 @@
     if swapped:
         return [(couples[k], k) for k in couples]
 
     return [(k, couples[k]) for k in couples]
 
 
 def symmetric(p):
-    '''Returns the symmetric point of a PD point on the diagonal
-    '''
-    return [(p[0] + p[1]) / 2., (p[0] + p[1]) / 2]
+    """Return the symmetric point of a PD point on the diagonal."""
+    return [(p[0] + p[1]) / 2.0, (p[0] + p[1]) / 2]
+
 
+def matching_diagrams(
+    p1, p2, plot=False, method="munkres", use_diag=True, new_fig=True, subplot=(111)
+):
+    """Return a list of matching components.
 
-def matching_diagrams(p1, p2, plot=False, method='munkres', use_diag=True, new_fig=True, subplot=(111)):
-    '''Returns a list of matching components
     Possible matching methods:
     - munkress
     - marriage problem
-    '''
-    from scipy.spatial.distance import cdist
+    """
     import munkres
+    from scipy.spatial.distance import cdist
+
     from tmd.view import common as _cm
 
     def plot_matching(p1, p2, indices, new_fig=True, subplot=(111)):
-        '''Plots matching between p1, p2
-        for the corresponding indices
-        '''
-        import pylab as plt
+        """Plots matching between p1, p2 for the corresponding indices."""
         fig, ax = _cm.get_figure(new_fig=new_fig, subplot=subplot)
         for i, j in indices:
-            ax.plot((p1[i][0], p2[j][0]), (p1[i][1], p2[j][1]), color='black')
-            ax.scatter(p1[i][0], p1[i][1], c='r')
-            ax.scatter(p2[j][0], p2[j][1], c='b')
+            ax.plot((p1[i][0], p2[j][0]), (p1[i][1], p2[j][1]), color="black")
+            ax.scatter(p1[i][0], p1[i][1], c="r")
+            ax.scatter(p2[j][0], p2[j][1], c="b")
 
     if use_diag:
         p1_enh = p1 + [symmetric(i) for i in p2]
         p2_enh = p2 + [symmetric(i) for i in p1]
     else:
         p1_enh = p1
         p2_enh = p2
 
     D = cdist(p1_enh, p2_enh)
 
-    if method == 'munkres':
+    if method == "munkres":
         m = munkres.Munkres()
         indices = m.compute(np.copy(D))
-    elif method == 'marriage':
+    elif method == "marriage":
         first_pref = [np.argsort(k).tolist() for k in cdist(p1_enh, p2_enh)]
         second_pref = [np.argsort(k).tolist() for k in cdist(p2_enh, p1_enh)]
         indices = marriage_problem(first_pref, second_pref)
 
     if plot:
         plot_matching(p1_enh, p2_enh, indices, new_fig=new_fig, subplot=subplot)
 
     ssum = np.sum([D[i][j] for (i, j) in indices])
 
     return indices, ssum
-
```

### Comparing `tmd-2.2.0/examples/Advanced/polar_plot_generation.py` & `TMD-2.3.0/examples/Advanced/polar_plot_generation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+"""Example for polar plots."""
+import matplotlib.pyplot as plt
+
 import tmd
-from view import polar_plots
+from tmd.view import polar_plots
 
-filename = './'
+filename = "./"
 
 pop = tmd.io.load_population(filename)
 
 # Get the data for a single cell
-res = polar_plots.get_histogram_polar_coordinates(pop.neurons[0], neurite_type='basal', N=30)
+res = polar_plots.get_histogram_polar_coordinates(
+    pop.neurons[0], neurite_type="basal_dendrite", N=30
+)
 
 # Plot the data for a single cell
 polar_plots.plot_polar_coordinates(res)
 
 # Extract the polar plots of all neurons in the population and save images
 # in a selected directory
 for n in pop.neurons:
-    res = polar_plots.get_histogram_polar_coordinates(n, neurite_type='basal', N=30)
-    polar_plots.plot_polar_coordinates(res, output_path='./PolarPlots/', output_name=n.name.split('/')[-1])
+    res = polar_plots.get_histogram_polar_coordinates(n, neurite_type="basal_dendrite", N=30)
+    polar_plots.plot_polar_coordinates(
+        res, output_path="./PolarPlots/", output_name=n.name.split("/")[-1]
+    )
     plt.close()
```

### Comparing `tmd-2.2.0/examples/Advanced/time_series_tmd.py` & `TMD-2.3.0/examples/Advanced/time_series_tmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,90 @@
+"""Example script for time series."""
+import matplotlib.pyplot as plt
+import numpy as np
+
+from tmd.Topology.analysis import sort_ph
+from tmd.view import plot
+
 
 def find_matching(p1, p2):
-    '''Finds the best matching between two
-    persistent diagrams and returns a list
-    of matched indices. The difference is
+    """Finds the best matching between two persistent diagrams.
+
+    Returns a list of matched indices. The difference is
     computed between p2 from p1, and
     the matching starts from the longest
-    components.    
-    '''
-    from scipy.spatial import distance
-    from view import plot
-
+    components.
+    """
     p2 = sort_ph(p2)
-    p2_symm = [((p[0] + p[1]) / 2., (p[0] + p[1]) / 2.) for p in p2]
+    p2_symm = [((p[0] + p[1]) / 2.0, (p[0] + p[1]) / 2.0) for p in p2]
     avail = range(len(p1))
     avail_symm = range(len(p2_symm))
 
     plot.ph_diagram(p1)
-    plot.ph_diagram(p2, new_fig=False, color='r')
+    plot.ph_diagram(p2, new_fig=False, color="r")
 
     for p in p2:
         if avail:
-            index = np.argmin( [np.linalg.norm(np.subtract(p[:2], pi)) for pi in np.array(p1)[avail]])
+            index = np.argmin(
+                [np.linalg.norm(np.subtract(p[:2], pi)) for pi in np.array(p1)[avail]]
+            )
             value = np.array(p1)[avail][index]
-            print p[:2], value, np.where(p1 == value)[0][0]
-            plt.plot([p[:2][0], value[0]], [p[:2][1], value[1]], c='b')
+            print(p[:2], value, np.where(p1 == value)[0][0])
+            plt.plot([p[:2][0], value[0]], [p[:2][1], value[1]], c="b")
             avail.remove(np.where(p1 == value)[0][0])
         else:
-            index = np.argmin( [np.linalg.norm(np.subtract(p[:2], pi)) for pi in np.array(p2_symm)[avail_symm]])
+            index = np.argmin(
+                [np.linalg.norm(np.subtract(p[:2], pi)) for pi in np.array(p2_symm)[avail_symm]]
+            )
             value = np.array(p2_symm)[avail_symm][index]
-            print p[:2], value, np.where(p2_symm == value)[0][0]
-            plt.plot([p[:2][0], value[0]], [p[:2][1], value[1]], c='b')
+            print(p[:2], value, np.where(p2_symm == value)[0][0])
+            plt.plot([p[:2][0], value[0]], [p[:2][1], value[1]], c="b")
             avail_symm.remove(np.where(p2_symm == value)[0][0])
 
-    
-def find_matching_time_series(p_list):
-    '''Finds the best matching between two
-    persistent diagrams and returns a list
-    of matched indices. The difference is
+
+def find_matching_time_series(p1, p2):
+    """Finds the best matching between two persistent diagrams.
+
+    Returns a list of matched indices. The difference is
     computed between p2 from p1, and
     the matching starts from the longest
-    components.    
-    '''
-    from scipy.spatial import distance
-    from view import plot
-
+    components.
+    """
     p2 = sort_ph(p2)
-    p1_symm = [((p[0] + p[1]) / 2., (p[0] + p[1]) / 2.) for p in p1]
+    p1_symm = [((p[0] + p[1]) / 2.0, (p[0] + p[1]) / 2.0) for p in p1]
     avail = range(len(p1))
     avail_symm = range(len(p1_symm))
 
     plot.ph_diagram(p1)
-    plot.ph_diagram(p2, new_fig=False, color='r')
+    plot.ph_diagram(p2, new_fig=False, color="r")
 
     for p in p2:
         if avail:
-            index = np.argmin( [np.linalg.norm(np.subtract(p[:2], pi)) for pi in np.array(p1)[avail]])
+            index = np.argmin(
+                [np.linalg.norm(np.subtract(p[:2], pi)) for pi in np.array(p1)[avail]]
+            )
             value = np.array(p1)[avail][index]
-            print p[:2], value, np.where(p1 == value)[0][0]
-            plt.plot([p[:2][0], value[0]], [p[:2][1], value[1]], c='b')
+            print(p[:2], value, np.where(p1 == value)[0][0])
+            plt.plot([p[:2][0], value[0]], [p[:2][1], value[1]], c="b")
             avail.remove(np.where(p1 == value)[0][0])
         else:
-            index = np.argmin( [np.linalg.norm(np.subtract(p[:2], pi)) for pi in np.array(p1_symm)[avail_symm]])
+            index = np.argmin(
+                [np.linalg.norm(np.subtract(p[:2], pi)) for pi in np.array(p1_symm)[avail_symm]]
+            )
             value = np.array(p1_symm)[avail_symm][index]
-            print p[:2], value, np.where(p1_symm == value)[0][0]
-            plt.plot([p[:2][0], value[0]], [p[:2][1], value[1]], c='b')
+            print(p[:2], value, np.where(p1_symm == value)[0][0])
+            plt.plot([p[:2][0], value[0]], [p[:2][1], value[1]], c="b")
             avail_symm.remove(np.where(p1_symm == value)[0][0])
 
 
 def marriage_problem(women_preferences, men_preferences):
-    '''Matches N women to M men so that max(M, N)
-    are coupled to their preferred choice that is available
+    """Matches N women to M men so that max(M, N) are coupled to their preferred available choice.
+
     See https://en.wikipedia.org/wiki/Stable_marriage_problem
-    '''
+    """
     N = len(women_preferences)
     M = len(men_preferences)
 
     swapped = False
 
     if M > N:
         swap = women_preferences
@@ -84,124 +93,120 @@
         N = len(women_preferences)
         M = len(men_preferences)
         swapped = True
 
     free_women = range(N)
     free_men = range(M)
 
-    couples = {x: None for x in xrange(N)} # woman first, then current husband
-
-    count = 0
+    couples = {x: None for x in range(N)}  # woman first, then current husband
 
     while len(free_men) > 0:
         m = free_men.pop()
         choice = men_preferences[m].pop(0)
 
         if choice in free_women:
             couples[choice] = m
             free_women.remove(choice)
         else:
             current = np.where(np.array(women_preferences)[choice] == couples[choice])[0][0]
             tobe = np.where(np.array(women_preferences)[choice] == m)[0][0]
-            if  current < tobe:
+            if current < tobe:
                 free_men.append(couples[choice])
                 couples[choice] = m
             else:
                 free_men.append(m)
 
     if swapped:
         return {couples[k]: k for k in couples}
 
     return couples
 
 
 def marry_components(p1, p2, ax=None, z1=0, z2=0.2):
-    '''Returns a list of matching components
-    '''
+    """Returns a list of matching components."""
     from scipy.spatial.distance import cdist
-    from mpl_toolkits.mplot3d.art3d import Line3DCollection
 
-    #if ax is None:
-        #fig = plt.figure()
-        #ax = fig.add_subplot(111, projection='3d')
+    # if ax is None:
+    # fig = plt.figure()
+    # ax = fig.add_subplot(111, projection='3d')
 
     first_distances = cdist(p1, p2)
     second_distances = cdist(p2, p1)
 
     first_pref = [np.argsort(k).tolist() for k in first_distances]
     second_pref = [np.argsort(k).tolist() for k in second_distances]
 
     church = marriage_problem(first_pref, second_pref)
 
-    #ax.scatter3D(np.transpose(p1)[0], np.transpose(p1)[1], z1)
-    #ax.scatter3D(np.transpose(p2)[0], np.transpose(p2)[1], z2, c='r')
-    #ax.plot3D([0,200], [0,200], z1, c='g')
-    #ax.plot3D([0,200], [0,200], z2, c='g')
+    # ax.scatter3D(np.transpose(p1)[0], np.transpose(p1)[1], z1)
+    # ax.scatter3D(np.transpose(p2)[0], np.transpose(p2)[1], z2, c='r')
+    # ax.plot3D([0,200], [0,200], z1, c='g')
+    # ax.plot3D([0,200], [0,200], z2, c='g')
 
     def symmetric(i, j):
-        return ((i + j) / 2., (i + j) / 2.)
+        return ((i + j) / 2.0, (i + j) / 2.0)
 
     speed = []
 
     for c in church:
         if c is None:
             x, y = symmetric(p2[church[c]][0], p2[church[c]][1])
-            #ax.plot3D([x, p2[church[c]][0]], [y, p2[church[c]][1]], [z1,z2], c='b')
+            # ax.plot3D([x, p2[church[c]][0]], [y, p2[church[c]][1]], [z1,z2], c='b')
             sp = np.linalg.norm(np.subtract([x, p2[church[c]][0]], [y, p2[church[c]][1]]))
         elif church[c] is not None:
-            #ax.plot3D([p1[c][0], p2[church[c]][0]], [p1[c][1], p2[church[c]][1]], [z1,z2], c='b')
-            sp = np.linalg.norm(np.subtract([p1[c][0], p2[church[c]][0]], [p1[c][1], p2[church[c]][1]]))
+            # ax.plot3D([p1[c][0], p2[church[c]][0]], [p1[c][1], p2[church[c]][1]], [z1,z2], c='b')
+            sp = np.linalg.norm(
+                np.subtract([p1[c][0], p2[church[c]][0]], [p1[c][1], p2[church[c]][1]])
+            )
         else:
             x, y = symmetric(p1[c][0], p1[c][1])
-            #ax.plot3D([p1[c][0], x], [p1[c][1], y], [z1,z2], c='b')
+            # ax.plot3D([p1[c][0], x], [p1[c][1], y], [z1,z2], c='b')
             sp = np.linalg.norm(np.subtract([p1[c][0], x], [p1[c][1], y]))
 
         speed.append(sp)
 
     return speed
 
-def vineyards(ph_list):
-    from matplotlib import pylab as plt
-    from mpl_toolkits.mplot3d import Axes3D
 
-    #fig = plt.figure()
-    #ax = fig.add_subplot(111, projection='3d')
+def vineyards(ph_list):
+    """TODO: Add relevant docstring."""
+    # fig = plt.figure()
+    # ax = fig.add_subplot(111, projection='3d')
 
     speeds = []
 
     for ip, p in enumerate(ph_list[:-1]):
-        sp = marry_components(ph_list[ip], ph_list[ip+1], z1=ip*0.2, z2=(ip + 1)*0.2)
+        sp = marry_components(ph_list[ip], ph_list[ip + 1], z1=ip * 0.2, z2=(ip + 1) * 0.2)
         speeds.append(sp)
-        #ax = plt.gca()
+        # ax = plt.gca()
 
     return speeds
 
 
 def get_persistence_diagram_timelapse(trees, **kwargs):
-    '''Method to extract ph from tree that contains mutlifurcations'''
+    """Method to extract ph from tree that contains mutlifurcations."""
     ph = []
 
     for itr, tree in enumerate(trees):
-        rd = getattr(tree, 'get_point_radial_distances_time')(time=itr, **kwargs)
+        rd = getattr(tree, "get_point_radial_distances_time")(time=itr, **kwargs)
 
         active = tree.get_bif_term() == 0
 
         beg, end = tree.get_sections_3()
 
         beg = np.array(beg)
         end = np.array(end)
 
         parents = {e: b for b, e in zip(beg, end)}
         children = {b: end[np.where(beg == b)[0]] for b in np.unique(beg)}
 
         while len(np.where(active)[0]) > 1:
             alive = list(np.where(active)[0])
-            for l in alive:
-
-                p = parents[l]
+            for i in alive:
+                p = parents[i]
                 c = children[p]
 
                 if np.alltrue(active[c]):
                     active[p] = True
                     active[c] = False
 
                     mx = np.argmax(abs(rd[c]))
@@ -214,10 +219,10 @@
                         ph.append([rd[ci], rd[p]])
                         alive.remove(ci)
 
                     alive.append(p)
 
                     rd[p] = rd[mx_id]
 
-        ph.append([rd[np.where(active)[0][0]], 0]) # Add the last alive component
+        ph.append([rd[np.where(active)[0][0]], 0])  # Add the last alive component
 
     return ph
```

### Comparing `tmd-2.2.0/examples/Advanced/variability.py` & `TMD-2.3.0/examples/Advanced/variability.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,79 @@
-import tmd
+"""Examples for variability compputation."""
+import matplotlib.pyplot as plt
+import numpy as np
 import view
+from matplotlib import cm
+
+import tmd
+
+# Defining average images
 
-### Defining average images
 
 def img_diff_distance(Z1, Z2, norm=True):
-    """Takes as input two images
-       as exported from the gaussian kernel
-       plotting function, and returns
-       their absolute difference:
-       diff(abs(Z1 - Z2))
+    """Return the absolute difference of 2 images from the gaussian kernel plotting function.
+
+    The absolute difference is computed as: diff(abs(Z1 - Z2))
     """
     if norm:
         Z1 = Z1 / Z1.max()
         Z2 = Z2 / Z2.max()
 
-    diff = np.sum(np.abs(Z2 - Z2))
+    diff = np.sum(np.abs(Z1 - Z2))
 
     # Normalize the difference to % of #pixels
     diff = diff / np.prod(np.shape(Z1))
 
     return diff
 
+
 def img_diff(Z1, Z2, norm=True):
-    """Takes as input two images
-       as exported from the gaussian kernel
-       plotting function, and returns
-       their absolute difference:
-       diff(abs(Z1 - Z2))
+    """Return the difference of 2 images from the gaussian kernel plotting function.
+
+    The difference is computed as: diff(Z1 - Z2)
     """
     if norm:
         Z1 = Z1 / Z1.max()
         Z2 = Z2 / Z2.max()
 
     return Z1 - Z2
 
 
 def number_of_bars(phs_list):
-    '''Returns the length of each ph_diagram of a list
-    '''
+    """Return the length of each ph_diagram of a list."""
     return [len(p) for p in phs_list]
 
 
 def weight_bars(phs_list, max_norm=None):
-    '''Returns weights according to the number of branches.
+    """Return weights according to the number of branches.
+
     If max not defined the maximum within a group will be used.
-    '''
+    """
     lengths = number_of_bars(phs_list)
     if max_norm is None:
         max_norm = np.max(lengths)
     return np.array(lengths, dtype=np.float) / max_norm
 
 
-def persistence_image(ph, norm_factor=None, xlims=None, ylims=None):
-    '''Create the data for the generation of the persistence image.
+def persistence_image(ph, norm_factor=None, xlim=None, ylim=None):
+    """Create the data for the generation of the persistence image.
+
     If norm_factor is provided the data will be normalized based on this,
     otherwise they will be normalized to 1.
-    If xlims, ylims are provided the data will be scaled accordingly.   
-    '''
-    from scipy import stats
+    If xlim, ylim are provided the data will be scaled accordingly.
+    """
     import numpy as np
+    from scipy import stats
 
-    if xlims is None:
-        xlims = [min(np.transpose(ph)[0]), max(np.transpose(ph)[0])]
-    if ylims is None:
-        ylims = [min(np.transpose(ph)[1]), max(np.transpose(ph)[1])]
+    if xlim is None:
+        xlim = [min(np.transpose(ph)[0]), max(np.transpose(ph)[0])]
+    if ylim is None:
+        ylim = [min(np.transpose(ph)[1]), max(np.transpose(ph)[1])]
 
-    X, Y = np.mgrid[xlims[0]:xlims[1]:100j, ylims[0]:ylims[1]:100j]
+    X, Y = np.mgrid[xlim[0] : xlim[1] : 100j, ylim[0] : ylim[1] : 100j]
 
     values = np.transpose(ph)
     kernel = stats.gaussian_kde(values)
     positions = np.vstack([X.ravel(), Y.ravel()])
     Z = np.reshape(kernel(positions).T, X.shape)
 
     if norm_factor is None:
@@ -77,474 +81,674 @@
 
     Zn = Z / norm_factor
 
     return Zn
 
 
 def average_ph_image(images_list):
-    '''Generates a normalized average image
-    from a list of images. Careful: images should be
-    at the same scale (x-y) for appropriate comparison.
-    '''
+    """Generates a normalized average image from a list of images.
+
+    .. warning::
+
+        Images should be at the same scale (x-y) for appropriate comparison.
+    """
     average_imgs = images_list[0]
 
     for im in images_list[1:]:
         average_imgs = np.add(average_imgs, im)
 
     average_imgs = average_imgs / len(images_list)
 
     return average_imgs
 
 
 def average_ph_image_weighted(images_list, weights):
-    '''Generates a normalized average image
-    from a list of images. Careful: images should be
-    at the same scale (x-y) for appropriate comparison.
-    '''
+    """Generates a normalized average image from a list of images.
+
+    .. warning::
+
+        Images should be at the same scale (x-y) for appropriate comparison.
+    """
     average_imgs = weights[0] * images_list[0]
 
-    for i,im in enumerate(images_list[1:]):
+    for i, im in enumerate(images_list[1:]):
         average_imgs = np.add(average_imgs, weights[i] * im)
 
     average_imgs = average_imgs / len(images_list)
 
     return average_imgs / np.max(average_imgs)
 
-def average_ph_from_list(phs_list, xlims=None, ylims=None, norm_factor=None):
-    '''Generates average image from list of phs'''
-    imgs = [persistence_image(p, norm_factor=norm_factor, xlims=xlims, ylims=ylims) for p in phs_list]
+
+def average_ph_from_list(phs_list, xlim=None, ylim=None, norm_factor=None):
+    """Generates average image from list of phs."""
+    imgs = [persistence_image(p, norm_factor=norm_factor, xlim=xlim, ylim=ylim) for p in phs_list]
     return average_ph_image(imgs)
 
 
-def average_weighted_ph_from_list(phs_list, xlims=None, ylims=None, norm_factor=None, max_norm=None):
-    '''Generates average image from list of phs'''
+def average_weighted_ph_from_list(phs_list, xlim=None, ylim=None, norm_factor=None, max_norm=None):
+    """Generates average image from list of phs."""
     weights = weight_bars(phs_list, max_norm=max_norm)
-    imgs = [persistence_image(p, norm_factor=norm_factor, xlims=xlims, ylims=ylims) for p in phs_list]
+    imgs = [persistence_image(p, norm_factor=norm_factor, xlim=xlim, ylim=ylim) for p in phs_list]
     return average_ph_image_weighted(imgs, weights=weights)
 
 
 def define_limits(phs_list):
-    '''Returns the x-y coordinates limits (min, max)
-    for a list of persistence diagrams
-    '''
+    """Return the x-y coordinates limits (min, max) for a list of persistence diagrams."""
     ph = view.plot.collapse(phs_list)
-    xlims = [min(np.transpose(ph)[0]), max(np.transpose(ph)[0])]
-    ylims = [min(np.transpose(ph)[1]), max(np.transpose(ph)[1])]
+    xlim = [min(np.transpose(ph)[0]), max(np.transpose(ph)[0])]
+    ylim = [min(np.transpose(ph)[1]), max(np.transpose(ph)[1])]
 
-    return xlims, ylims
+    return xlim, ylim
 
 
-### Ploting functions
+# Plotting functions
 
-def plot_imgs(img, new_fig=True, subplot=111, title='', xlims=None, ylims=None, cmap=cm.jet, vmin=0, vmax=1., masked=False, threshold=0.01):
-    '''Plots the gaussian kernel of the input image.
-    '''
-    from scipy import stats
-    from view import common
+
+def plot_imgs(
+    img,
+    new_fig=True,
+    subplot=111,
+    title="",
+    xlim=None,
+    ylim=None,
+    cmap=cm.jet,
+    vmin=0,
+    vmax=1.0,
+    masked=False,
+    threshold=0.01,
+):
+    """Plots the gaussian kernel of the input image."""
     import numpy as np
+    from view import common
 
-    if xlims is None:
-        xlims = (0,100)
-    if ylims is None:
-        ylims = (0,100)
+    if xlim is None:
+        xlim = (0, 100)
+    if ylim is None:
+        ylim = (0, 100)
 
     fig, ax = common.get_figure(new_fig=new_fig, subplot=subplot)
 
     if masked:
         img = np.ma.masked_where((threshold > np.abs(img)), img)
 
-    cax= ax.imshow(np.rot90(img), vmin=vmin, vmax=vmax, cmap=cmap, interpolation='bilinear', extent=xlims+ylims)
+    cax = ax.imshow(
+        np.rot90(img),
+        vmin=vmin,
+        vmax=vmax,
+        cmap=cmap,
+        interpolation="bilinear",
+        extent=xlim + ylim,
+    )
 
     kwargs = {}
 
-    kwargs['xlim'] = xlims
-    kwargs['ylim'] = ylims
-    kwargs['title'] = title
+    kwargs["xlim"] = xlim
+    kwargs["ylim"] = ylim
+    kwargs["title"] = title
 
     plt.colorbar(cax)
 
-    ax.set_aspect('equal')
+    ax.set_aspect("equal")
 
-    return common.plot_style(fig=fig, ax=ax, aspect='equal', **kwargs)
+    return common.plot_style(fig=fig, ax=ax, aspect="equal", **kwargs)
 
 
-def plot_av(phs1, title=''):
-    '''Generates and plots the average images from input phs'''
-    xlims, ylims = define_limits(phs1)
-    imgs1 = [persistence_image(p, xlims=xlims, ylims=ylims) for p in phs1]
+def plot_av(phs1, title=""):
+    """Generates and plots the average images from input phs."""
+    xlim, ylim = define_limits(phs1)
+    imgs1 = [persistence_image(p, xlim=xlim, ylim=ylim) for p in phs1]
     IMG = average_ph_image(imgs1)
-    return plot_imgs(IMG, xlims=xlims, ylims=ylims, title=title)
-
+    return plot_imgs(IMG, xlim=xlim, ylim=ylim, title=title)
 
-def multiplot(phs1, title=''):
-    '''Plots distances, average image and an example from the population'''
 
-    xlims, ylims = define_limits(phs1)
-    imgs1 = [persistence_image(p, xlims=xlims, ylims=ylims) for p in phs1]
+def multiplot(phs1, title=""):
+    """Plots distances, average image and an example from the population."""
+    xlim, ylim = define_limits(phs1)
+    imgs1 = [persistence_image(p, xlim=xlim, ylim=ylim) for p in phs1]
 
     IMG = average_ph_image(imgs1)
 
     distances = [img_diff_distance(IMG, im) for im in imgs1]
     ID = np.argmax(distances)
-    
+
     fig = plt.figure()
-    ax = fig.add_subplot(1,3,1)
+    ax = fig.add_subplot(1, 3, 1)
     ax.hist(distances, bins=20)
     plt.title(title)
 
-    plot_imgs(IMG, xlims=xlims, ylims=ylims, new_fig=False, subplot=132)
-    plot_imgs(imgs1[ID], xlims=xlims, ylims=ylims, new_fig=False, subplot=133)
+    plot_imgs(IMG, xlim=xlim, ylim=ylim, new_fig=False, subplot=132)
+    plot_imgs(imgs1[ID], xlim=xlim, ylim=ylim, new_fig=False, subplot=133)
 
     return distances
 
 
-def multiplot_outliers(phs1, title=''):
-    '''Plots distances, average image and an example from the population'''
-
-    xlims, ylims = define_limits(phs1)
-    imgs1 = [persistence_image(p, xlims=xlims, ylims=ylims) for p in phs1]
+def multiplot_outliers(phs1, title=""):
+    """Plots distances, average image and an example from the population."""
+    xlim, ylim = define_limits(phs1)
+    imgs1 = [persistence_image(p, xlim=xlim, ylim=ylim) for p in phs1]
 
     IMG = average_ph_image(imgs1)
 
     distances = [img_diff_distance(IMG, im) for im in imgs1]
 
     d_mean = np.mean(distances)
     d_std = np.std(distances)
-    outliers = np.where((np.array(distances) > d_mean + 2*d_std))[0]
+    outliers = np.where((np.array(distances) > d_mean + 2 * d_std))[0]
     no_outliers = np.delete(np.arange(len(distances)), outliers)
 
     IMG_out = average_ph_image(np.array(imgs1)[outliers])
     IMG_without = average_ph_image(np.array(imgs1)[no_outliers])
 
     fig = plt.figure()
-    ax = fig.add_subplot(2,2,1)
+    ax = fig.add_subplot(2, 2, 1)
     ax.hist(distances, bins=20)
     plt.title(title)
 
-    plot_imgs(IMG, xlims=xlims, ylims=ylims, new_fig=False, subplot=222)
-    plt.title('All')
-    plot_imgs(IMG_out, xlims=xlims, ylims=ylims, new_fig=False, subplot=223)
-    plt.title('Outliers')
-    plot_imgs(IMG_without, xlims=xlims, ylims=ylims, new_fig=False, subplot=224)
-    plt.title('No_outliers')
+    plot_imgs(IMG, xlim=xlim, ylim=ylim, new_fig=False, subplot=222)
+    plt.title("All")
+    plot_imgs(IMG_out, xlim=xlim, ylim=ylim, new_fig=False, subplot=223)
+    plt.title("Outliers")
+    plot_imgs(IMG_without, xlim=xlim, ylim=ylim, new_fig=False, subplot=224)
+    plt.title("No_outliers")
 
     return distances
 
 
 def outliers_distances(dist_list, n=2):
-    '''Outputs the number of cells
-    that are outside the n*sigma regime.
-    '''
+    """Outputs the number of cells that are outside the n*sigma regime."""
     d_mean = np.mean(dist_list)
     d_std = np.std(dist_list)
 
-    outliers = np.where((np.array(dist_list) > d_mean + n*d_std))[0]
+    outliers = np.where((np.array(dist_list) > d_mean + n * d_std))[0]
 
     return outliers, len(outliers), len(dist_list)
 
 
 def representatives_distances(dist_list, n=3):
-    '''Outputs the number of cells
-    that are outside the n*sigma regime.
-    '''
+    """Outputs the number of cells that are outside the n*sigma regime."""
     return np.argsort(dist_list)[:n]
 
+
 # Functions using the previous basics, customized for Sandra's datasets
 
-def example_run_outliers(filename='./Female/control 4h/IPL/', title=''):
-    '''Special funct'''
-    pop = tmd.io.load_population(filename, tree_types={0:'basal'})
+
+def example_run_outliers(filename="./Female/control 4h/IPL/", title=""):
+    """Special funct."""
+    pop = tmd.io.load_population(filename, tree_types={0: "basal_dendrite"})
 
     phs1 = []
     pids = []
 
-    for i,n in enumerate(pop.neurons):
+    for i, n in enumerate(pop.neurons):
         try:
             p = tmd.methods.get_ph_neuron(n)
             if len(p) > 4:
                 phs1.append(p)
                 pids.append(i)
-        except:
-            print n.name
+        except Exception:
+            print(n.name)
 
     distances = multiplot_outliers(phs1, title=title)
 
     return distances
 
 
-def example_run(filename='./Female/control 4h/IPL/', title=''):
-    '''Special funct'''
-    pop = tmd.io.load_population(filename, tree_types={0:'basal'})
+def example_run(filename="./Female/control 4h/IPL/", title=""):
+    """Special funct."""
+    pop = tmd.io.load_population(filename, tree_types={0: "basal_dendrite"})
 
     phs1 = []
 
-    for i,n in enumerate(pop.neurons):
+    for i, n in enumerate(pop.neurons):
         try:
             p = tmd.methods.get_ph_neuron(n)
             if len(p) > 4:
                 phs1.append(p)
-        except:
-            #print n.name
+        except Exception:
+            # print(n.name)
             pass
 
     distances = multiplot(phs1, title=title)
 
     return distances
 
 
-def get_phs_clean(filename='./Female/control 4h/IPL/'):
-    '''Special funct'''
-    pop = tmd.io.load_population(filename, tree_types={0:'basal'})
+def get_phs_clean(filename="./Female/control 4h/IPL/"):
+    """Special funct."""
+    pop = tmd.io.load_population(filename, tree_types={0: "basal_dendrite"})
 
     phs1 = []
 
-    for i,n in enumerate(pop.neurons):
+    for i, n in enumerate(pop.neurons):
         try:
             p = tmd.methods.get_ph_neuron(n)
             if len(p) > 4:
                 phs1.append(p)
-        except:
-            #print n.name
+        except Exception:
             pass
 
     return phs1
 
 
 def norm_limits(ph_list):
-    '''Normalizes the limits and the intensity of ph_images
-    in order to compare all the ph of a list.
-    '''
+    """Compute the limits of ph_images in order to compare all the ph of a list."""
     # Normalization of limits
     pp = []
     for ph in ph_list:
         pp = pp + ph
-    xlims, ylims = define_limits(pp)
+    xlim, ylim = define_limits(pp)
 
-    return xlims, ylims
+    return xlim, ylim
 
 
 def norm_intensity(ph_list):
-    '''Normalizes the limits and the intensity of ph_images
-    in order to compare all the ph of a list.
-    '''
+    """Normalize the intensity of ph_images in order to compare all the ph of a list."""
     # Normalization of intensity
     intensities = []
     for ph in ph_list:
-        Z = average_ph_from_list(ph, norm_factor=1.0, xlims=xlims, ylims=ylims)
+        xlim, ylim = define_limits([ph])
+        Z = average_ph_from_list([ph], norm_factor=1.0, xlim=xlim, ylim=ylim)
         intensities.append(np.max(Z))
     M = np.max(intensities)
 
     return M
 
 
-def multiplot_comparison(ph_list, norm=True, diff=1., thresh=0.1, masked=True):
-
-    xlims, ylims = norm_limits(ph_list)
+def multiplot_comparison(ph_list, norm=True, diff=1.0, thresh=0.1, masked=True):
+    """Compare multiple plots."""
+    xlim, ylim = norm_limits(ph_list)
 
     if norm:
         M = norm_intensity(ph_list)
     else:
         M = None
 
     # Generate normalized averages
     Zns = []
     for ph in ph_list:
-        Z = average_ph_from_list(ph, norm_factor=M, xlims=xlims, ylims=ylims)
+        Z = average_ph_from_list(ph, norm_factor=M, xlim=xlim, ylim=ylim)
         Zns.append(Z)
 
-    plot_imgs(Zns[0], new_fig=True, subplot=331, xlims=xlims, ylims=ylims)
-    plot_imgs(Zns[1], new_fig=False, subplot=332, xlims=xlims, ylims=ylims)
-    plot_imgs(Zns[2], new_fig=False, subplot=334, xlims=xlims, ylims=ylims)
-    plot_imgs(Zns[3], new_fig=False, subplot=335, xlims=xlims, ylims=ylims)
+    plot_imgs(Zns[0], new_fig=True, subplot=331, xlim=xlim, ylim=ylim)
+    plot_imgs(Zns[1], new_fig=False, subplot=332, xlim=xlim, ylim=ylim)
+    plot_imgs(Zns[2], new_fig=False, subplot=334, xlim=xlim, ylim=ylim)
+    plot_imgs(Zns[3], new_fig=False, subplot=335, xlim=xlim, ylim=ylim)
 
     D1 = img_diff(Zns[0], Zns[2], norm=False)
     D2 = img_diff(Zns[1], Zns[3], norm=False)
     D3 = img_diff(Zns[0], Zns[1], norm=False)
     D4 = img_diff(Zns[2], Zns[3], norm=False)
 
-    plot_imgs(D1, new_fig=False, subplot=337, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh)
-    plot_imgs(D2, new_fig=False, subplot=338, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh)
-    plot_imgs(D3, new_fig=False, subplot=333, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh)
-    plot_imgs(D4, new_fig=False, subplot=336, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh)
+    plot_imgs(
+        D1,
+        new_fig=False,
+        subplot=337,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+    )
+    plot_imgs(
+        D2,
+        new_fig=False,
+        subplot=338,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+    )
+    plot_imgs(
+        D3,
+        new_fig=False,
+        subplot=333,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+    )
+    plot_imgs(
+        D4,
+        new_fig=False,
+        subplot=336,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+    )
 
     return Zns
 
 
-def multiplot_weighted_comparison_naive(ph_list, diff=1., thresh=0.1, masked=True, title='', xlims=None, ylims=None):
-
-    if xlims is None and ylims is None:    
-        xlims, ylims = norm_limits(ph_list)
+def multiplot_weighted_comparison_naive(
+    ph_list, diff=1.0, thresh=0.1, masked=True, title="", xlim=None, ylim=None
+):
+    """Compare multiple weighted plot in a naive way."""
+    if xlim is None and ylim is None:
+        xlim, ylim = norm_limits(ph_list)
 
     # Generate normalized averages
     Zns = []
     for ph in ph_list:
-        Z = average_weighted_ph_from_list(ph, norm_factor=None, xlims=xlims, ylims=ylims)
+        Z = average_weighted_ph_from_list(ph, norm_factor=None, xlim=xlim, ylim=ylim)
         Zns.append(Z)
 
-    plot_imgs(Zns[0], new_fig=True, subplot=331, xlims=xlims, ylims=ylims, title='Control 4h')
-    plot_imgs(Zns[1], new_fig=False, subplot=332, xlims=xlims, ylims=ylims, title='Control 48h')
-    plot_imgs(Zns[2], new_fig=False, subplot=334, xlims=xlims, ylims=ylims, title='Naive 4h')
-    plot_imgs(Zns[3], new_fig=False, subplot=335, xlims=xlims, ylims=ylims, title='Naive 48h')
+    plot_imgs(Zns[0], new_fig=True, subplot=331, xlim=xlim, ylim=ylim, title="Control 4h")
+    plot_imgs(Zns[1], new_fig=False, subplot=332, xlim=xlim, ylim=ylim, title="Control 48h")
+    plot_imgs(Zns[2], new_fig=False, subplot=334, xlim=xlim, ylim=ylim, title="Naive 4h")
+    plot_imgs(Zns[3], new_fig=False, subplot=335, xlim=xlim, ylim=ylim, title="Naive 48h")
 
     D1 = img_diff(Zns[0], Zns[2], norm=False)
     D2 = img_diff(Zns[1], Zns[3], norm=False)
     D3 = img_diff(Zns[0], Zns[1], norm=False)
     D4 = img_diff(Zns[2], Zns[3], norm=False)
 
-    plot_imgs(D1, new_fig=False, subplot=337, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control - Naive 4h')
-    print 'Control - Naive 4h :', np.sum(np.abs(D1))
-    plot_imgs(D2, new_fig=False, subplot=338, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control - Naive 48h')
-    print 'Control - Naive 48h :', np.sum(np.abs(D2))
-    plot_imgs(D3, new_fig=False, subplot=333, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control 4h-48h')
-    print 'Control 4h-48h :', np.sum(np.abs(D3))
-    plot_imgs(D4, new_fig=False, subplot=336, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Naive 4h-48h')
-    print 'Naive 4h-48h :', np.sum(np.abs(D4))
+    plot_imgs(
+        D1,
+        new_fig=False,
+        subplot=337,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control - Naive 4h",
+    )
+    print("Control - Naive 4h :", np.sum(np.abs(D1)))
+    plot_imgs(
+        D2,
+        new_fig=False,
+        subplot=338,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control - Naive 48h",
+    )
+    print("Control - Naive 48h :", np.sum(np.abs(D2)))
+    plot_imgs(
+        D3,
+        new_fig=False,
+        subplot=333,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control 4h-48h",
+    )
+    print("Control 4h-48h :", np.sum(np.abs(D3)))
+    plot_imgs(
+        D4,
+        new_fig=False,
+        subplot=336,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Naive 4h-48h",
+    )
+    print("Naive 4h-48h :", np.sum(np.abs(D4)))
 
     plt.suptitle(title)
     plt.tight_layout(True)
 
     return Zns
 
 
-
-def multiplot_weighted_comparison(ph_list, diff=1., thresh=0.1, masked=True, title='', xlims=None, ylims=None):
-
-    if xlims is None and ylims is None:    
-        xlims, ylims = norm_limits(ph_list)
+def multiplot_weighted_comparison(
+    ph_list, diff=1.0, thresh=0.1, masked=True, title="", xlim=None, ylim=None
+):
+    """Compare multiple weighted plot."""
+    if xlim is None and ylim is None:
+        xlim, ylim = norm_limits(ph_list)
 
     # Generate normalized averages
     Zns = []
     for ph in ph_list:
-        Z = average_weighted_ph_from_list(ph, norm_factor=None, xlims=xlims, ylims=ylims)
+        Z = average_weighted_ph_from_list(ph, norm_factor=None, xlim=xlim, ylim=ylim)
         Zns.append(Z)
 
-    plot_imgs(Zns[0], new_fig=True, subplot=331, xlims=xlims, ylims=ylims, title='Control 4h')
-    plot_imgs(Zns[1], new_fig=False, subplot=332, xlims=xlims, ylims=ylims, title='Control 48h')
-    plot_imgs(Zns[2], new_fig=False, subplot=334, xlims=xlims, ylims=ylims, title='Drug 4h')
-    plot_imgs(Zns[3], new_fig=False, subplot=335, xlims=xlims, ylims=ylims, title='Drug 48h')
+    plot_imgs(Zns[0], new_fig=True, subplot=331, xlim=xlim, ylim=ylim, title="Control 4h")
+    plot_imgs(Zns[1], new_fig=False, subplot=332, xlim=xlim, ylim=ylim, title="Control 48h")
+    plot_imgs(Zns[2], new_fig=False, subplot=334, xlim=xlim, ylim=ylim, title="Drug 4h")
+    plot_imgs(Zns[3], new_fig=False, subplot=335, xlim=xlim, ylim=ylim, title="Drug 48h")
 
     D1 = img_diff(Zns[0], Zns[2], norm=False)
     D2 = img_diff(Zns[1], Zns[3], norm=False)
     D3 = img_diff(Zns[0], Zns[1], norm=False)
     D4 = img_diff(Zns[2], Zns[3], norm=False)
 
-    plot_imgs(D1, new_fig=False, subplot=337, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control - Drug 4h')
-    print 'Control - Drug 4h :', np.sum(np.abs(D1))
-    plot_imgs(D2, new_fig=False, subplot=338, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control - Drug 48h')
-    print 'Control - Drug 48h :', np.sum(np.abs(D2))
-    plot_imgs(D3, new_fig=False, subplot=333, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control 4h-48h')
-    print 'Control 4h-48h :', np.sum(np.abs(D3))
-    plot_imgs(D4, new_fig=False, subplot=336, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Drug 4h-48h')
-    print 'Drug 4h-48h :', np.sum(np.abs(D4))
+    plot_imgs(
+        D1,
+        new_fig=False,
+        subplot=337,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control - Drug 4h",
+    )
+    print("Control - Drug 4h :", np.sum(np.abs(D1)))
+    plot_imgs(
+        D2,
+        new_fig=False,
+        subplot=338,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control - Drug 48h",
+    )
+    print("Control - Drug 48h :", np.sum(np.abs(D2)))
+    plot_imgs(
+        D3,
+        new_fig=False,
+        subplot=333,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control 4h-48h",
+    )
+    print("Control 4h-48h :", np.sum(np.abs(D3)))
+    plot_imgs(
+        D4,
+        new_fig=False,
+        subplot=336,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Drug 4h-48h",
+    )
+    print("Drug 4h-48h :", np.sum(np.abs(D4)))
 
     plt.suptitle(title)
     plt.tight_layout(True)
 
     return Zns
 
 
-def multiplot_weighted_comparison_male_female(ph_list, diff=1., thresh=0.1, masked=True, title='', xlims=None, ylims=None):
-
-    if xlims is None and ylims is None:    
-        xlims, ylims = norm_limits(ph_list)
+def multiplot_weighted_comparison_male_female(
+    ph_list, diff=1.0, thresh=0.1, masked=True, title="", xlim=None, ylim=None
+):
+    """Compare multiple weighted plot."""
+    if xlim is None and ylim is None:
+        xlim, ylim = norm_limits(ph_list)
 
     # Generate normalized averages
     Zns = []
     for ph in ph_list:
-        Z = average_weighted_ph_from_list(ph, norm_factor=None, xlims=xlims, ylims=ylims)
+        Z = average_weighted_ph_from_list(ph, norm_factor=None, xlim=xlim, ylim=ylim)
         Zns.append(Z)
 
-    plot_imgs(Zns[0], new_fig=True, subplot=331, xlims=xlims, ylims=ylims, title='Control 4h')
-    plot_imgs(Zns[1], new_fig=False, subplot=332, xlims=xlims, ylims=ylims, title='Control 48h')
-    plot_imgs(Zns[2], new_fig=False, subplot=334, xlims=xlims, ylims=ylims, title='Drug 4h')
-    plot_imgs(Zns[3], new_fig=False, subplot=335, xlims=xlims, ylims=ylims, title='Drug 48h')
+    plot_imgs(Zns[0], new_fig=True, subplot=331, xlim=xlim, ylim=ylim, title="Control 4h")
+    plot_imgs(Zns[1], new_fig=False, subplot=332, xlim=xlim, ylim=ylim, title="Control 48h")
+    plot_imgs(Zns[2], new_fig=False, subplot=334, xlim=xlim, ylim=ylim, title="Drug 4h")
+    plot_imgs(Zns[3], new_fig=False, subplot=335, xlim=xlim, ylim=ylim, title="Drug 48h")
 
     D1 = img_diff(Zns[0], Zns[2], norm=False)
     D2 = img_diff(Zns[1], Zns[3], norm=False)
     D3 = img_diff(Zns[0], Zns[1], norm=False)
     D4 = img_diff(Zns[2], Zns[3], norm=False)
 
-    plot_imgs(D1, new_fig=False, subplot=337, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control - Drug 4h')
-    print 'Control - Drug 4h :', np.sum(np.abs(D1))
-    plot_imgs(D2, new_fig=False, subplot=338, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control - Drug 48h')
-    print 'Control - Drug 48h :', np.sum(np.abs(D2))
-    plot_imgs(D3, new_fig=False, subplot=333, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Control 4h-48h')
-    print 'Control 4h-48h :', np.sum(np.abs(D3))
-    plot_imgs(D4, new_fig=False, subplot=336, xlims=xlims, ylims=ylims, vmin=-diff, vmax=diff, masked=masked, threshold=thresh, title='Drug 4h-48h')
-    print 'Drug 4h-48h :', np.sum(np.abs(D4))
+    plot_imgs(
+        D1,
+        new_fig=False,
+        subplot=337,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control - Drug 4h",
+    )
+    print("Control - Drug 4h :", np.sum(np.abs(D1)))
+    plot_imgs(
+        D2,
+        new_fig=False,
+        subplot=338,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control - Drug 48h",
+    )
+    print("Control - Drug 48h :", np.sum(np.abs(D2)))
+    plot_imgs(
+        D3,
+        new_fig=False,
+        subplot=333,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Control 4h-48h",
+    )
+    print("Control 4h-48h :", np.sum(np.abs(D3)))
+    plot_imgs(
+        D4,
+        new_fig=False,
+        subplot=336,
+        xlim=xlim,
+        ylim=ylim,
+        vmin=-diff,
+        vmax=diff,
+        masked=masked,
+        threshold=thresh,
+        title="Drug 4h-48h",
+    )
+    print("Drug 4h-48h :", np.sum(np.abs(D4)))
 
     plt.suptitle(title)
     plt.tight_layout(True)
 
     return Zns
 
 
-def distance_number_of_cells(ph_list, step_size=10, samples=10, xlims=None, ylims=None, title=''):
-    #import seaborn
+def distance_number_of_cells(ph_list, step_size=10, samples=10, xlim=None, ylim=None, title=""):
+    """Plot distance number of cells."""
     min_max_size = np.min([len(p) for p in ph_list])
-    intervals = np.linspace(step_size, min_max_size, (min_max_size-step_size)/step_size)
+    intervals = np.linspace(step_size, min_max_size, (min_max_size - step_size) / step_size)
 
     distancesCD4 = []
     distancesCD4std = []
     distancesCD48 = []
     distancesCD48std = []
 
     for i in intervals:
-
         d4 = []
         d48 = []
 
         for s in np.arange(samples):
             Zns = []
             for ph in ph_list:
-                ph_random_indices = random.choice(np.arange(len(ph)), int(i), replace=False)
+                ph_random_indices = np.random.choice(np.arange(len(ph)), int(i), replace=False)
                 ph_random = np.array(ph)[ph_random_indices]
-                Z = average_weighted_ph_from_list(ph_random, norm_factor=None, xlims=xlims, ylims=ylims)
+                Z = average_weighted_ph_from_list(ph_random, norm_factor=None, xlim=xlim, ylim=ylim)
                 Zns.append(Z)
 
             DiffCD4 = np.sum(np.abs(img_diff(Zns[0], Zns[1], norm=False)))
             DiffCD48 = np.sum(np.abs(img_diff(Zns[0], Zns[2], norm=False)))
 
-            d4.append(DiffCD4/ (DiffCD4+DiffCD48))
-            d48.append(DiffCD48/ (DiffCD4+DiffCD48))
+            d4.append(DiffCD4 / (DiffCD4 + DiffCD48))
+            d48.append(DiffCD48 / (DiffCD4 + DiffCD48))
 
         distancesCD4.append(np.mean(d4))
         distancesCD48.append(np.mean(d48))
         distancesCD4std.append(np.std(d4))
         distancesCD48std.append(np.std(d48))
 
-    fig = plt.figure(figsize=(15,10))
-    plt.plot(intervals, distancesCD4, c='b', label='Dist: C-D4')
-    plt.plot(intervals, distancesCD48, c='r', label='Dist: C-D48')
+    plt.figure(figsize=(15, 10))
+    plt.plot(intervals, distancesCD4, c="b", label="Dist: C-D4")
+    plt.plot(intervals, distancesCD48, c="r", label="Dist: C-D48")
+
+    plt.fill_between(
+        intervals,
+        np.subtract(distancesCD4, distancesCD4std),
+        np.add(distancesCD4, distancesCD4std),
+        color="b",
+        alpha=0.2,
+    )
+    plt.fill_between(
+        intervals,
+        np.subtract(distancesCD48, distancesCD48std),
+        np.add(distancesCD48, distancesCD48std),
+        color="r",
+        alpha=0.2,
+    )
 
-    plt.fill_between(intervals, np.subtract(distancesCD4, distancesCD4std), np.add(distancesCD4, distancesCD4std), color='b', alpha=0.2)
-    plt.fill_between(intervals, np.subtract(distancesCD48, distancesCD48std), np.add(distancesCD48, distancesCD48std), color='r', alpha=0.2)
-
-    plt.xlabel('Number of cells', fontsize=18)
-    plt.ylabel('Normalized distance', fontsize=18)
+    plt.xlabel("Number of cells", fontsize=18)
+    plt.ylabel("Normalized distance", fontsize=18)
     plt.legend()
     plt.title(title)
 
     return intervals, distancesCD4, distancesCD48, distancesCD4std, distancesCD48std
 
 
 def check_input_data(filename):
-
+    """Check input data."""
     import os
+
     L = os.listdir(filename)
 
     counter_process = 0
     counter_load = 0
-    
+
     for c in L:
         try:
-            n = tmd.io.load_neuron(filename+c, tree_types={0:'basal'})
+            n = tmd.io.load_neuron(filename + c, tree_types={0: "basal_dendrite"})
             try:
-                p = tmd.methods.get_ph_neuron(n)
-            except:
+                tmd.methods.get_ph_neuron(n)
+            except Exception:
                 counter_process = counter_process + 1
-        except:
+        except Exception:
             counter_load = counter_load + 1
-            # print c
 
     return len(L), counter_load, counter_process
-
```

### Comparing `tmd-2.2.0/examples/classifier.py` & `TMD-2.3.0/examples/classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,93 @@
-import tmd
+"""Classifier examples."""
+import importlib
+
 import numpy as np
-# import view
 
-list_of_modules = ['discriminant_analysis', 'discriminant_analysis', 'tree']
+import tmd
+
+list_of_modules = ["discriminant_analysis", "discriminant_analysis", "tree"]
+
+list_of_classifiers = [
+    "LinearDiscriminantAnalysis",
+    "QuadraticDiscriminantAnalysis",
+    "DecisionTreeClassifier",
+]
 
-list_of_classifiers =['LinearDiscriminantAnalysis', 'QuadraticDiscriminantAnalysis', 'DecisionTreeClassifier']
 
 def train(mod, classifier, data, labels, **kwargs):
-    '''Trains the classifier from mod of sklearn
-       with data and targets.
-       Returns a fited classifier.
-    '''
-    import importlib
+    """Trains the classifier from mod of sklearn with data and targets.
 
-    clas_mod = importlib.import_module('sklearn.' + mod)
+    Returns a fited classifier.
+    """
+    clas_mod = importlib.import_module("sklearn." + mod)
     clf = getattr(clas_mod, classifier)()
     clf.set_params(**kwargs)
 
     clf.fit(data, labels)
 
     return clf
 
+
 def predict(clf, data):
-    '''Predict label for data for the trained classifier clf.
-       Returns the index of the predicted class
-       for each datapoint in data.
-    '''
+    """Predict label for data for the trained classifier clf.
+
+    Returns the index of the predicted class for each datapoint in data.
+    """
     predict_label = clf.predict([data])
 
     return predict_label[0]
 
-def classify_cell_in_groups(list_of_groups=['L5_UTPC', 'L5_STPC', 'L5_TTPC1', 'L5_TTPC2'],
-                            cell_to_classify='./L5_TTPC1/C030796A-P3.h5',
-                            neurite_type='apical',
-                            classifier_module=list_of_modules[0],
-                            classifier_method=list_of_classifiers[0],
-                            number_of_trials=20):
 
+def classify_cell_in_groups(
+    list_of_groups=["L5_UTPC", "L5_STPC", "L5_TTPC1", "L5_TTPC2"],
+    cell_to_classify="./L5_TTPC1/C030796A-P3.h5",
+    neurite_type="apical_dendrite",
+    classifier_module=list_of_modules[0],
+    classifier_method=list_of_classifiers[0],
+    number_of_trials=20,
+):
+    """Classify the cells in groups."""
     # ------------------------ Training dataset --------------------------------
     # Load all data from selected folders
-    groups = [tmd.io.load_population(l) for l in list_of_groups]
+    groups = [tmd.io.load_population(i) for i in list_of_groups]
     # Define labels depending on the number of neurons in each folder
-    labels = [i+1 for i,k in enumerate(groups) for j in k.neurons]
+    labels = [i + 1 for i, k in enumerate(groups) for j in k.neurons]
     # Generate a persistence diagram per neuron
-    pers_diagrams = [tmd.methods.get_ph_neuron(j, neurite_type=neurite_type)
-                     for i,k in enumerate(groups) for j in k.neurons]
+    pers_diagrams = [
+        tmd.methods.get_ph_neuron(j, neurite_type=neurite_type)
+        for i, k in enumerate(groups)
+        for j in k.neurons
+    ]
     # Define x-ylimits
-    xlims, ylims = tmd.analysis.define_limits(pers_diagrams)
+    xlim, ylim = tmd.analysis.define_limits(pers_diagrams)
     # Generate a persistence image for each diagram
-    pers_images = [tmd.analysis.persistence_image_data(p, xlims=xlims, ylims=ylims)
-                   for p in pers_diagrams]
+    pers_images = [
+        tmd.analysis.persistence_image_data(p, xlim=xlim, ylim=ylim) for p in pers_diagrams
+    ]
     # Create the train dataset from the flatten images
     train_dataset = [i.flatten() for i in pers_images]
 
     # ------------------------ Test cell dataset -------------------------------
     # Load cell to be classified
     neuron2test = tmd.io.load_neuron(cell_to_classify)
     # Get persistence diagram from test cell
     pers2test = tmd.methods.get_ph_neuron(neuron2test, neurite_type=neurite_type)
     # Get persistence image from test cell
-    pers_image2test = tmd.analysis.persistence_image_data(pers2test, xlims=xlims, ylims=ylims)
+    pers_image2test = tmd.analysis.persistence_image_data(pers2test, xlim=xlim, ylim=ylim)
     # Create the test dataset from the flatten image of the test cell
     test_dataset = pers_image2test.flatten()
 
     predict_labels = []
     # Train classifier with training images for selected number_of_trials
-    for i in xrange(number_of_trials):
-
+    for i in range(number_of_trials):
         clf = train(classifier_module, classifier_method, train_dataset, labels)
         # Test classifier with test image and return predictions
         predict_labels.append(predict(clf, test_dataset))
 
-    percentages = {groups[i-1].name: np.float(len(np.where(np.array(predict_labels) == i)[0])) / len(predict_labels)
-                   for i in np.unique(labels)}
+    percentages = {
+        groups[i - 1].name: np.float(len(np.where(np.array(predict_labels) == i)[0]))
+        / len(predict_labels)
+        for i in np.unique(labels)
+    }
 
     return percentages
```

### Comparing `tmd-2.2.0/examples/distances_example.py` & `TMD-2.3.0/examples/distances_example.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,49 @@
+"""Example for distance computation."""
+import numpy as np
+
 import tmd
-import tmd.view as view
 
-pop1 = tmd.io.load_population(directory1)
-pop2 = tmd.io.load_population(directory2)
+# from matplotlib import cm
+
+# import tmd.view as view
+
+
+def compute_distances(directory1, directory2):
+    """Compute distances."""
+    pop1 = tmd.io.load_population(directory1)
+    pop2 = tmd.io.load_population(directory2)
+
+    phs1 = [tmd.methods.get_ph_neuron(n, neurite_type="basal_dendrite") for n in pop1.neurons]
+    phs2 = [tmd.methods.get_ph_neuron(n, neurite_type="basal_dendrite") for n in pop2.neurons]
+
+    # Normalize the limits
+    xlim, ylim = tmd.analysis.get_limits(phs1 + phs2)
+
+    # Create average images for populations
+    # imgs1 = [tmd.analysis.get_persistence_image_data(p, xlim=xlim, ylim=ylim) for p in phs1]
+    IMG1 = tmd.analysis.get_average_persistence_image(phs1, xlim=xlim, ylim=ylim)
+    # imgs2 = [tmd.analysis.get_persistence_image_data(p, xlim=xlim, ylim=ylim) for p in phs2]
+    IMG2 = tmd.analysis.get_average_persistence_image(phs2, xlim=xlim, ylim=ylim)
+
+    # You can plot the images if you want to create pretty figures
+    # average_figure1 = view.common.plot_img_basic(
+    #     IMG1, title="", xlim=xlim, ylim=ylim, cmap=cm.jet
+    # )
+    # average_figure2 = view.common.plot_img_basic(
+    #     IMG2, title="", xlim=xlim, ylim=ylim, cmap=cm.jet
+    # )
+
+    # Create the difference between the two images
+    # Subtracts IMG2 from IMG1 so anything red IMG1 has more of it and anything blue IMG2 has more
+    # of it - or that's how it is supposed to be :)
+    DIMG = tmd.analysis.get_image_diff_data(IMG1, IMG2)
+
+    # Plot the difference between them
+    # diff_image = view.common.plot_img_basic(
+    #     DIMG, vmin=-1.0, vmax=1.0
+    # )  # vmin, vmax important to see changes
 
-phs1 = [tmd.methods.get_ph_neuron(n, neurite_type='basal') for n in pop1.neurons]
-phs2 = [tmd.methods.get_ph_neuron(n, neurite_type='basal') for n in pop2.neurons]
+    # Quantify the absolute distance between the two averages
+    dist = np.sum(np.abs(DIMG))
 
-# Normalize the limits
-xlims, ylims = tmd.analysis.get_limits(phs1 + phs2)
-
-# Create average images for populations
-imgs1 = [tmd.analysis.get_persistence_image_data(p, xlims=xlims, ylims=ylims) for p in phs1]
-IMG1 = tmd.analysis.get_average_persistence_image(phs1, xlims=xlims, ylims=ylims)
-imgs2 = [tmd.analysis.get_persistence_image_data(p, xlims=xlims, ylims=ylims) for p in phs2]
-IMG2 = tmd.analysis.get_average_persistence_image(phs2, xlims=xlims, ylims=ylims)
-
-# You can plot the images if you want to create pretty figures
-average_figure1 = view.common.plot_img_basic(IMG1, title='', xlims=xlims, ylims=ylims, cmap=cm.jet)
-average_figure2 = view.common.plot_img_basic(IMG2, title='', xlims=xlims, ylims=ylims, cmap=cm.jet)
-
-# Create the diffence between the two images
-DIMG = tmd.analysis.get_image_diff_data(IMG1, IMG2) # subtracts IMG2 from IMG1 so anything red IMG1 has more of it and anything blue IMG2 has more of it - or that's how it is supposed to be :)
-
-# Plot the difference between them
-diff_image = view.common.plot_img_basic(DIMG, vmin=-1.0, vmax=1.0) # vmin, vmax important to see changes
-# Quantify the absolute distance between the two averages
-dist = np.sum(np.abs(DIMG))
+    return dist
```

### Comparing `tmd-2.2.0/examples/extract_ph.py` & `TMD-2.3.0/examples/extract_ph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-# Example to extract the persistence diagram from a neuronal tree
+"""Example to extract the persistence diagram from a neuronal tree."""
 
 # Step 1: Import the tmd module
 import tmd
+from tmd.view import plot
+from tmd.view import view
 
 # Step 2: Load your morphology
-filename = '../tests/data/valid/C010398B-P2.CNG.swc'
+filename = "../tests/data/valid/C010398B-P2.CNG.swc"
 neu = tmd.io.load_neuron(filename)
 
 # Step 3: Extract the ph diagram of a tree
 tree = neu.neurites[0]
 ph = tmd.methods.get_persistence_diagram(tree)
 
 # Step 4: Extract the ph diagram of a neuron's trees
 ph_neu = tmd.methods.get_ph_neuron(neu)
 
 # Step 5: Extract the ph diagram of a neuron's trees,
 # depending on the neurite_type
-ph_apical = tmd.methods.get_ph_neuron(neu, neurite_type='apical')
-ph_axon = tmd.methods.get_ph_neuron(neu, neurite_type='axon')
-ph_basal = tmd.methods.get_ph_neuron(neu, neurite_type='basal')
+ph_apical = tmd.methods.get_ph_neuron(neu, neurite_type="apical_dendrite")
+ph_axon = tmd.methods.get_ph_neuron(neu, neurite_type="axon")
+ph_basal = tmd.methods.get_ph_neuron(neu, neurite_type="basal_dendrite")
 
 # Step 6: Plot the extracted topological data with three different ways
-from tmd.view import view, plot
 
 # Visualize the neuron
 view.neuron(neu)
 
 # Visualize a selected neurite type or multiple of them
-view.neuron(neu, neurite_type=['apical'])
+view.neuron(neu, neurite_type=["apical_dendrite"])
 
 # Visualize the persistence diagram
 plot.diagram(ph_apical)
 
 # Visualize the persistence barcode
 plot.barcode(ph_apical)
```

### Comparing `tmd-2.2.0/pylintrc` & `TMD-2.3.0/.pylintrc`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 [MESSAGES CONTROL]
-disable=fixme,invalid-name,len-as-condition,no-else-return,ungrouped-imports,useless-object-inheritance
+disable=
+	fixme,
+	invalid-name,
+	len-as-condition,
+	no-else-return
 
 [FORMAT]
+# Regexp for a line that is allowed to be longer than the limit.
+ignore-long-lines=\bhttps?://\S
 # Maximum number of characters on a single line.
 max-line-length=100
 
 [DESIGN]
 # Maximum number of arguments for function / method
 max-args=13
 # Argument names that match this expression will be ignored. Default to name
@@ -23,28 +29,26 @@
 max-parents=7
 # Maximum number of attributes for a class (see R0902).
 max-attributes=40
 # Minimum number of public methods for a class (see R0903).
 min-public-methods=0
 # Maximum number of public methods for a class (see R0904).
 max-public-methods=60
+
+[SIMILARITIES]
 # checks for similarities and duplicated code. This computation may be
 # memory / CPU intensive, so you should disable it if you experiments some
 # problems.
-#
 
-[SIMILARITIES]
 # Minimum lines number of a similarity.
 min-similarity-lines=25
 # Ignore comments when computing similarities.
 ignore-comments=yes
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 [TYPECHECK]
 # List of classes names for which member attributes should not be checked
 # (useful for classes with attributes dynamically set).
 
-#as of numpy 1.8.0, name resolution seems to be a problem.  Ignore lookups in numpy
-ignored-classes=numpy,list
-
-extension-pkg-whitelist=numpy,lxml,brain,pybinreports
+# as of numpy 1.8.0, name resolution seems to be a problem. Ignore lookups in numpy
+# ignored-classes=numpy,list
```

### Comparing `tmd-2.2.0/tests/data/sample.swc` & `TMD-2.3.0/tests/data/sample.swc`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/sample_disordered.swc` & `TMD-2.3.0/tests/data/sample_disordered.swc`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/sample_disordered_v1.h5` & `TMD-2.3.0/tests/data/sample_disordered_v1.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/sample_v0.h5` & `TMD-2.3.0/tests/data/sample_v0.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/sample_v1.h5` & `TMD-2.3.0/tests/data/sample_v1.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/sample_v2.h5` & `TMD-2.3.0/tests/data/sample_v2.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/test_morph.swc` & `TMD-2.3.0/tests/data/test_morph.swc`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/test_morph_v1.h5` & `TMD-2.3.0/tests/data/test_morph_v1.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/test_morph_v2.h5` & `TMD-2.3.0/tests/data/test_morph_v2.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/valid/C010398B-P2.CNG.swc` & `TMD-2.3.0/tests/data/valid/C010398B-P2.CNG.swc`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # SWC to SWC conversion from L-Measure. Sridevi Polavaram: spolavar@gmu.edu
 # Original fileName:Z:\Soumya\Test_Folders\Lm3.7.2Test\markram\CNG version\C010398B-P2.CNG.swc
 #
 # Original file C010398B-P2.asc.swc edited by Duncan Donohue using StdSwc version 1.21 on 8/4/05.
 # Irregularities and fixes documented in C010398B-P2.asc.swc.std.  See StdSwc1.21.doc for more information.
 #
 # Neurolucida to SWC conversion from L-Measure. R. Scorcioni: rscorcio@gmu.edu
-# Original fileName:C:\Documents and Settings\Duncan\Desktop\Cellular morphology\Archives\Markram\Combined(204)\Origional\All.stdors (type 2 included)\origional ASC files\C010398B-P2.asc
+# Original fileName:C:\Documents and Settings\Duncan\Desktop\Cellular morphology\Archives\Markram\Combined(204)\Original\All.stdors (type 2 included)\original ASC files\C010398B-P2.asc
 #
-# ORIGINAL_SOURCE 
-# CREATURE 
-# REGION 
-# FIELD/LAYER 
-# TYPE 
-# CONTRIBUTOR 
-# REFERENCE 
-# RAW 
-# EXTRAS 
-# SOMA_AREA 
-# SHRINKAGE_CORRECTION 
-# VERSION_NUMBER 
-# VERSION_DATE 
-# ********************************************* 
-# SCALE 1.0 1.0 1.0 
+# ORIGINAL_SOURCE
+# CREATURE
+# REGION
+# FIELD/LAYER
+# TYPE
+# CONTRIBUTOR
+# REFERENCE
+# RAW
+# EXTRAS
+# SOMA_AREA
+# SHRINKAGE_CORRECTION
+# VERSION_NUMBER
+# VERSION_DATE
+# *********************************************
+# SCALE 1.0 1.0 1.0
  1 1 27.48 22.09 2.37 6.474 -1
  2 1 27.48 28.56 2.37 6.474 1
  3 1 27.48 15.61 2.37 6.474 1
  4 4 29.9 27.76 1.2 0.665 1
  5 4 29.44 31.01 2.4 0.665 4
  6 4 28.56 32.43 3.5 0.665 5
  7 4 28.45 38.26 2 0.665 6
```

### Comparing `tmd-2.2.0/tests/data/valid/C010398B-P2.h5` & `TMD-2.3.0/tests/data/valid/C010398B-P2.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/valid/sample.swc` & `TMD-2.3.0/tests/data/valid/sample.swc`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/valid/sample_v1.h5` & `TMD-2.3.0/tests/data/valid/sample_v1.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/data/valid/sample_v2.h5` & `TMD-2.3.0/tests/data/valid/sample_v2.h5`

 * *Files identical despite different names*

### Comparing `tmd-2.2.0/tests/test_h5.py` & `TMD-2.3.0/tests/test_h5.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,191 @@
-'''Test tmd.io.h5'''
+"""Test tmd.io.h5."""
+# pylint: disable=protected-access
 import os
-from tmd.io import h5
+
+import h5py
 import numpy as np
 from numpy import testing as npt
-import h5py
+
+from tmd.io import h5
 
 _path = os.path.dirname(os.path.abspath(__file__))
-DATA_PATH = os.path.join(_path, 'data')
+DATA_PATH = os.path.join(_path, "data")
 
 # Filenames for testing
-basic_file = os.path.join(DATA_PATH, 'basic.swc')
-nosecids_file = os.path.join(DATA_PATH, 'basic_no_sec_ids.swc')
-sample_file = os.path.join(DATA_PATH, 'sample.swc')
-
-sample_h5_v1_file = os.path.join(DATA_PATH, 'sample_v1.h5')
-sample_h5_v2_file = os.path.join(DATA_PATH, 'sample_v2.h5')
-sample_h5_v0_file = os.path.join(DATA_PATH, 'sample_v0.h5')
-
-h5file_v0 = h5py.File(sample_h5_v0_file, mode='r')
-h5file_v1 = h5py.File(sample_h5_v1_file, mode='r')
-h5file_v2 = h5py.File(sample_h5_v2_file, mode='r')
-
-points_1 = np.array([[0.,   0.,   0.,   6.],
-                     [0.,   0.,   0.,   0.40000001],
-                     [0.,   1.,   0.,   0.40000001],
-                     [0.,   2.,   0.,   0.40000001],
-                     [0.,   3.,   0.,   0.40000001],
-                     [0.,   4.,   0.,   0.40000001],
-                     [0.,   5.,   0.,   0.40000001],
-                     [0.,   6.,   0.,   0.40000001],
-                     [0.,   7.,   0.,   0.40000001],
-                     [0.,   8.,   0.,   0.40000001]])
-groups_1 = np.array([[0,  1, -1],
-                     [1,  2,  0],
-                     [12,  2,  1],
-                     [18,  2,  1],
-                     [24,  2,  3],
-                     [30,  2,  3],
-                     [36,  3,  0],
-                     [47,  3,  6],
-                     [53,  3,  6]])
-
-data_1 = np.array([[0.,  1.,  0.,  0.,  0.,
-                    6., -1.],
-                   [1.,  2.,  0.,  0.,  0.,
-                    0.40000001,  0.],
-                   [2.,  2.,  0.,  1.,  0.,
-                    0.40000001,  1.],
-                   [3.,  2.,  0.,  2.,  0.,
-                    0.40000001,  2.],
-                   [4.,  2.,  0.,  3.,  0.,
-                    0.40000001,  3.],
-                   [5.,  2.,  0.,  4.,  0.,
-                    0.40000001,  4.],
-                   [6.,  2.,  0.,  5.,  0.,
-                    0.40000001,  5.],
-                   [7.,  2.,  0.,  6.,  0.,
-                    0.40000001,  6.],
-                   [8.,  2.,  0.,  7.,  0.,
-                    0.40000001,  7.],
-                   [9.,  2.,  0.,  8.,  0.,
-                    0.40000001,  8.]])
-
-bx1 = np.array([0.,  0.,  0.,  0.,  0.,  0.,  0.,  0.,  0.,  0.])
-by1 = np.array([0.,  0.,  1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.])
-bz1 = np.array([0.,  0.,  0.,  0.,  0.,  0.,  0.,  0.,  0.,  0.])
-bd1 = np.array([6.,  0.40000001,  0.40000001,  0.40000001,  0.40000001,
-                0.40000001,  0.40000001,  0.40000001,  0.40000001,  0.40000001])
-bt1 = np.array([1.,  2.,  2.,  2.,  2.,  2.,  2.,  2.,  2.,  2.])
-bp1 = np.array([-1.,  0.,  1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.])
+basic_file = os.path.join(DATA_PATH, "basic.swc")
+nosecids_file = os.path.join(DATA_PATH, "basic_no_sec_ids.swc")
+sample_file = os.path.join(DATA_PATH, "sample.swc")
+
+sample_h5_v1_file = os.path.join(DATA_PATH, "sample_v1.h5")
+sample_h5_v2_file = os.path.join(DATA_PATH, "sample_v2.h5")
+sample_h5_v0_file = os.path.join(DATA_PATH, "sample_v0.h5")
+
+h5file_v0 = h5py.File(sample_h5_v0_file, mode="r")
+h5file_v1 = h5py.File(sample_h5_v1_file, mode="r")
+h5file_v2 = h5py.File(sample_h5_v2_file, mode="r")
+
+points_1 = np.array(
+    [
+        [0.0, 0.0, 0.0, 6.0],
+        [0.0, 0.0, 0.0, 0.40000001],
+        [0.0, 1.0, 0.0, 0.40000001],
+        [0.0, 2.0, 0.0, 0.40000001],
+        [0.0, 3.0, 0.0, 0.40000001],
+        [0.0, 4.0, 0.0, 0.40000001],
+        [0.0, 5.0, 0.0, 0.40000001],
+        [0.0, 6.0, 0.0, 0.40000001],
+        [0.0, 7.0, 0.0, 0.40000001],
+        [0.0, 8.0, 0.0, 0.40000001],
+    ]
+)
+groups_1 = np.array(
+    [
+        [0, 1, -1],
+        [1, 2, 0],
+        [12, 2, 1],
+        [18, 2, 1],
+        [24, 2, 3],
+        [30, 2, 3],
+        [36, 3, 0],
+        [47, 3, 6],
+        [53, 3, 6],
+    ]
+)
+
+data_1 = np.array(
+    [
+        [0.0, 1.0, 0.0, 0.0, 0.0, 6.0, -1.0],
+        [1.0, 2.0, 0.0, 0.0, 0.0, 0.40000001, 0.0],
+        [2.0, 2.0, 0.0, 1.0, 0.0, 0.40000001, 1.0],
+        [3.0, 2.0, 0.0, 2.0, 0.0, 0.40000001, 2.0],
+        [4.0, 2.0, 0.0, 3.0, 0.0, 0.40000001, 3.0],
+        [5.0, 2.0, 0.0, 4.0, 0.0, 0.40000001, 4.0],
+        [6.0, 2.0, 0.0, 5.0, 0.0, 0.40000001, 5.0],
+        [7.0, 2.0, 0.0, 6.0, 0.0, 0.40000001, 6.0],
+        [8.0, 2.0, 0.0, 7.0, 0.0, 0.40000001, 7.0],
+        [9.0, 2.0, 0.0, 8.0, 0.0, 0.40000001, 8.0],
+    ]
+)
+
+bx1 = np.array([0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
+by1 = np.array([0.0, 0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0])
+bz1 = np.array([0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
+bd1 = np.array(
+    [
+        6.0,
+        0.40000001,
+        0.40000001,
+        0.40000001,
+        0.40000001,
+        0.40000001,
+        0.40000001,
+        0.40000001,
+        0.40000001,
+        0.40000001,
+    ]
+)
+bt1 = np.array([1.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0])
+bp1 = np.array([-1.0, 0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0])
 bch1 = {0: [1], 1: [2], 2: [3], 3: [4], 4: [5], 5: [6], 6: [7], 7: [8], 8: [9], 9: []}
 
 
 def test_h5_dict():
-    assert h5.h5_dct == {'PX': 0,
-                         'PY': 1,
-                         'PZ': 2,
-                         'PD': 3,
-                         'GPFIRST': 0,
-                         'GTYPE': 1,
-                         'GPID': 2}
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    assert h5.h5_dct == {"PX": 0, "PY": 1, "PZ": 2, "PD": 3, "GPFIRST": 0, "GTYPE": 1, "GPID": 2}
 
 
 def test_find_group():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     g0 = h5._find_group(0, groups_1)
-    npt.assert_allclose(g0, [0,  1, -1])
+    npt.assert_allclose(g0, [0, 1, -1])
 
     g12 = h5._find_group(12, groups_1)
     g13 = h5._find_group(13, groups_1)
-    npt.assert_allclose(g12, [12,  2,  1])
-    npt.assert_allclose(g13, [12,  2,  1])
+    npt.assert_allclose(g12, [12, 2, 1])
+    npt.assert_allclose(g13, [12, 2, 1])
 
 
 def test_find_parent_id():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     pid0 = h5._find_parent_id(0, groups_1)
     assert pid0 == -1
 
     pid0 = h5._find_parent_id(53, groups_1)
     assert pid0 == 46
 
     pid0 = h5._find_parent_id(59, groups_1)
     assert pid0 == 58
 
 
 def test_find_last_point():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     lp0 = h5._find_last_point(0, groups_1, points_1)
     assert lp0 == 0
 
     lp1 = h5._find_last_point(1, groups_1, points_1)
     assert lp1 == 11
 
     lp2 = h5._find_last_point(2, groups_1, points_1)
     assert lp2 == 17
 
     lp8 = h5._find_last_point(8, groups_1, points_1)
     assert lp8 == 9
 
 
 def test_remove_duplicate_points():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     points, groups = h5._unpack_v1(h5file_v1)
     p1, g1 = h5.remove_duplicate_points(points, groups)
     assert len(p1) == 53
     npt.assert_allclose(
-        np.transpose(g1)[0],
-        np.array([0.,   1.,  12.,  17.,
-                 22.,  27.,  32.,  43.,  48.])
+        np.transpose(g1)[0], np.array([0.0, 1.0, 12.0, 17.0, 22.0, 27.0, 32.0, 43.0, 48.0])
     )
     npt.assert_allclose(np.transpose(g1)[1], np.transpose(groups)[1])
     npt.assert_allclose(np.transpose(g1)[2], np.transpose(groups)[2])
 
 
 def test_get_h5_version():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     version_0 = h5._get_h5_version(h5file_v0)
     version_1 = h5._get_h5_version(h5file_v1)
     version_2 = h5._get_h5_version(h5file_v2)
     assert version_0 is None
     assert version_1 == 1
     assert version_2 == 2
 
 
 def test_unpack_v1():
-    points, groups = h5._unpack_v1(h5file_v1)
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    _, groups = h5._unpack_v1(h5file_v1)
     npt.assert_allclose(groups[:10], groups_1)
 
 
 def test_unpack_v2():
-    points, groups = h5._unpack_v2(h5file_v2, '2')
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    _, groups = h5._unpack_v2(h5file_v2, "2")
     npt.assert_allclose(groups[:10], groups_1)
 
 
 def test_unpack_data():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     data = h5._unpack_data(points_1, groups_1)
     npt.assert_allclose(data, data_1)
 
 
 def test_read_h5():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     data_v1 = h5.read_h5(sample_h5_v1_file)
     data_v2 = h5.read_h5(sample_h5_v2_file)
     npt.assert_allclose(data_v1[:10], data_1)
     npt.assert_allclose(data_v2[:10], data_1)
 
 
 def test_h5_data_to_lists():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     x1, y1, z1, d1, t1, p1, ch1 = h5.h5_data_to_lists(data_1)
     npt.assert_allclose(x1, bx1)
     npt.assert_allclose(y1, by1)
     npt.assert_allclose(z1, bz1)
     npt.assert_allclose(d1, bd1)
     npt.assert_allclose(t1, bt1)
     npt.assert_allclose(p1, bp1)
```

### Comparing `tmd-2.2.0/tests/test_neuron.py` & `TMD-2.3.0/tests/test_neuron.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,79 @@
-'''Test tmd.Neuron'''
+"""Test tmd.Neuron."""
+# pylint: disable=use-implicit-booleaness-not-comparison
 import numpy as np
+
 from tmd.Neuron import Neuron
 from tmd.Soma import Soma
 from tmd.Tree import Tree
 from tmd.utils import TREE_TYPE_DICT as td
 
-soma_test = Soma.Soma([0.],[0.],[0.],[12.])
-soma_test1 = Soma.Soma([0.],[0.],[0.],[6.])
-apical_test = Tree.Tree(x=np.array([5., 5.]), y=np.array([6., 6.]), z=np.array([ 7., 7.]),
-                       d=np.array([16., 16.]), t=np.array([4, 4]), p=np.array([-1,  0]))
-basal_test = Tree.Tree(x=np.array([4.]), y=np.array([5.]), z=np.array([6.]),
-                       d=np.array([14.]), t=np.array([3]), p=np.array([-1]))
-axon_test = Tree.Tree(x=np.array([ 3.]), y=np.array([4.]), z=np.array([5.]),
-                      d=np.array([12.]), t=np.array([2 ]), p=np.array([-1]))
+soma_test = Soma.Soma([0.0], [0.0], [0.0], [12.0])
+soma_test1 = Soma.Soma([0.0], [0.0], [0.0], [6.0])
+apical_test = Tree.Tree(
+    x=np.array([5.0, 5.0]),
+    y=np.array([6.0, 6.0]),
+    z=np.array([7.0, 7.0]),
+    d=np.array([16.0, 16.0]),
+    t=np.array([4, 4]),
+    p=np.array([-1, 0]),
+)
+basal_test = Tree.Tree(
+    x=np.array([4.0]),
+    y=np.array([5.0]),
+    z=np.array([6.0]),
+    d=np.array([14.0]),
+    t=np.array([3]),
+    p=np.array([-1]),
+)
+axon_test = Tree.Tree(
+    x=np.array([3.0]),
+    y=np.array([4.0]),
+    z=np.array([5.0]),
+    d=np.array([12.0]),
+    t=np.array([2]),
+    p=np.array([-1]),
+)
 
 neu_test = Neuron.Neuron()
 neu_test.set_soma(soma_test)
 neu_test.append_tree(apical_test, td)
 
+
 def test_neuron_init_():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     neu1 = Neuron.Neuron()
 
-    assert neu1.name == 'Neuron'
+    assert neu1.name == "Neuron"
     assert isinstance(neu1.soma, Soma.Soma)
     assert neu1.axon == []
-    assert neu1.basal == []
-    assert neu1.apical == []
+    assert neu1.basal_dendrite == []
+    assert neu1.apical_dendrite == []
     assert neu1.neurites == []
-    neu1 = Neuron.Neuron(name='test')
-    assert neu1.name == 'test'
+    neu1 = Neuron.Neuron(name="test")
+    assert neu1.name == "test"
+
 
 def test_neuron_rename():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     neu1 = Neuron.Neuron()
-    neu1.rename('test')
-    assert neu1.name == 'test'
+    neu1.rename("test")
+    assert neu1.name == "test"
+
 
 def test_copy_neuron():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     neu1 = Neuron.Neuron()
     neu2 = neu1.copy_neuron()
     assert neu1.is_equal(neu2)
     assert neu1 != neu2
 
+
 def test_neuron_is_equal():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     neu1 = Neuron.Neuron()
     neu1.set_soma(soma_test)
     neu1.append_tree(apical_test, td)
     assert neu1.is_equal(neu_test)
 
     neu1 = Neuron.Neuron()
     neu1.set_soma(soma_test1)
@@ -53,32 +81,38 @@
     assert not neu1.is_equal(neu_test)
 
     neu1 = Neuron.Neuron()
     neu1.set_soma(soma_test)
     neu1.append_tree(basal_test, td)
     assert not neu1.is_equal(neu_test)
 
+
 def test_neuron_is_same():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     neu1 = Neuron.Neuron()
     neu1.set_soma(soma_test)
     neu1.append_tree(apical_test, td)
     assert neu1.is_same(neu_test)
 
-    neu1.name = 'test_not_same'
+    neu1.name = "test_not_same"
     assert not neu1.is_same(neu_test)
 
+
 def test_neuron_set_soma():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     neu1 = Neuron.Neuron()
     neu1.set_soma(soma_test)
     assert neu1.soma.is_equal(soma_test)
 
+
 def test_append_tree():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     neu1 = Neuron.Neuron()
     neu1.append_tree(apical_test, td)
     assert len(neu1.neurites) == 1
 
     neu1.append_tree(basal_test, td)
     neu1.append_tree(axon_test, td)
     assert len(neu1.neurites) == 3
-    assert len(neu1.basal) == 1
+    assert len(neu1.basal_dendrite) == 1
     assert len(neu1.axon) == 1
-    assert len(neu1.apical) == 1
+    assert len(neu1.apical_dendrite) == 1
```

### Comparing `tmd-2.2.0/tests/test_neuron_conversion.py` & `TMD-2.3.0/tests/test_neuron_conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,117 @@
+"""Test Neuron conversions."""
+# pylint: disable=protected-access
 import os
+
 import mock
+import morphio
 import numpy as np
 from numpy import testing as npt
-import morphio
+
 from tmd.io import conversion as tested
 from tmd.io.io import load_neuron
 from tmd.io.io import load_neuron_from_morphio
 
 _path = os.path.dirname(os.path.abspath(__file__))
-DATA_PATH = os.path.join(_path, 'data')
+DATA_PATH = os.path.join(_path, "data")
 
 
 class MockSection:
+    """A Mock for the Section class."""
 
     def __init__(self, id, points, diameters, type, parent=None):
-
+        # pylint: disable=redefined-builtin
         self.id = id
         self.points = points
         self.diameters = diameters
         self.type = type
         self.parent = parent
         self.traversal = []
 
     def iter(self):
+        # noqa: D102 ; pylint: disable=missing-function-docstring
         return self.traversal
 
     @property
     def is_root(self):
+        # noqa: D102 ; pylint: disable=missing-function-docstring
         return self.parent is None
 
 
 class MockNeuron:
+    """A Mock for the Neuron class."""
 
     def __init__(self):
-
         root = MockSection(
-                id=0,
-                points = np.array([[0.1, 0.2, 0.3], [0.4, 0.5, 0.6], [0.7, 0.8, 0.9]]),
-                diameters = np.array([0.1, 0.2, 0.3]),
-                type=2,
-                parent=None
+            id=0,
+            points=np.array([[0.1, 0.2, 0.3], [0.4, 0.5, 0.6], [0.7, 0.8, 0.9]]),
+            diameters=np.array([0.1, 0.2, 0.3]),
+            type=2,
+            parent=None,
         )
 
         child1 = MockSection(
-                id=1,
-                points = np.array([[0.7, 0.8, 0.9], [0.4, 0.5, 0.6], [0.7, 0.8, 0.9]]),
-                diameters = np.array([0.3, 0.4, 0.5]),
-                type=2,
-                parent=root
+            id=1,
+            points=np.array([[0.7, 0.8, 0.9], [0.4, 0.5, 0.6], [0.7, 0.8, 0.9]]),
+            diameters=np.array([0.3, 0.4, 0.5]),
+            type=2,
+            parent=root,
         )
 
         child2 = MockSection(
-                id=2,
-                points = np.array([[0.7, 0.8, 0.9], [0.4, 0.5, 0.6], [0.7, 0.8, 0.9]]),
-                diameters = np.array([0.3, 0.6, 0.7]),
-                type=2,
-                parent=root
+            id=2,
+            points=np.array([[0.7, 0.8, 0.9], [0.4, 0.5, 0.6], [0.7, 0.8, 0.9]]),
+            diameters=np.array([0.3, 0.6, 0.7]),
+            type=2,
+            parent=root,
         )
 
         root.traversal = [root, child1, child2]
 
         self.root_sections = [root]
 
     @property
     def diameters(self):
+        # noqa: D102 ; pylint: disable=missing-function-docstring
         return np.hstack([s.diameters for root in self.root_sections for s in root.iter()])
 
     @property
     def points(self):
+        # noqa: D102 ; pylint: disable=missing-function-docstring
         return np.vstack([s.points for root in self.root_sections for s in root.iter()])
 
     @property
     def n_points(self):
+        # noqa: D102 ; pylint: disable=missing-function-docstring
         return len(self.points)
 
 
 def test_convert_morphio_soma():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     morphio_soma = mock.Mock(
-        points = np.array([
-            [0., 1., 2.],
-            [2., 3., 4.]
-        ]),
+        points=np.array([[0.0, 1.0, 2.0], [2.0, 3.0, 4.0]]),
         diameters=np.array([2.1, 3.4]),
     )
 
     soma = tested.convert_morphio_soma(morphio_soma)
 
-    npt.assert_allclose(soma.x, [0., 2.])
-    npt.assert_allclose(soma.y, [1., 3.])
-    npt.assert_allclose(soma.z, [2., 4.])
+    npt.assert_allclose(soma.x, [0.0, 2.0])
+    npt.assert_allclose(soma.y, [1.0, 3.0])
+    npt.assert_allclose(soma.z, [2.0, 4.0])
     npt.assert_allclose(soma.d, [2.1, 3.4])
 
 
 def test_section_to_data():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     section = MockSection(
         id=0,
-        points=np.array([
-            [0.1, 0.2, 0.3],
-            [0.4, 0.5, 0.6],
-            [0.7, 0.8, 0.9]
-        ]),
+        points=np.array([[0.1, 0.2, 0.3], [0.4, 0.5, 0.6], [0.7, 0.8, 0.9]]),
         diameters=np.array([1.2, 1.3, 1.4]),
         type=3,
-        parent=None
+        parent=None,
     )
 
     n, data = tested._section_to_data(section, tree_length=11, start=0, parent=-1)
 
     npt.assert_equal(n, 3)
     npt.assert_allclose(data.points, section.points)
     npt.assert_allclose(section.diameters, data.diameters)
@@ -121,15 +124,15 @@
     npt.assert_allclose(data.points, section.points[1:])
     npt.assert_allclose(data.diameters, section.diameters[1:])
     npt.assert_equal(data.section_type, 3)
     npt.assert_array_equal(data.parents, [5, 2 + 0])
 
 
 def test_convert_morphio_trees():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     morphio_neuron = MockNeuron()
 
     trees = list(tested.convert_morphio_trees(morphio_neuron))
 
     assert len(trees) == 1
 
     tree = trees[0]
@@ -139,51 +142,48 @@
     npt.assert_allclose(tree.z, [0.3, 0.6, 0.9, 0.6, 0.9, 0.6, 0.9])
     npt.assert_allclose(tree.d, [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7])
     npt.assert_array_equal(tree.t, [2, 2, 2, 2, 2, 2, 2])
     npt.assert_array_equal(tree.p, [-1, 0, 1, 2, 3, 2, 5])
 
 
 def _assert_neurons_equal(neuron1, neuron2):
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     npt.assert_allclose(neuron1.soma.x, neuron2.soma.x)
     npt.assert_allclose(neuron1.soma.y, neuron2.soma.y)
     npt.assert_allclose(neuron1.soma.z, neuron2.soma.z)
     npt.assert_allclose(neuron1.soma.d, neuron2.soma.d)
 
     for neurite1, neurite2 in zip(neuron1.neurites, neuron2.neurites):
-
         npt.assert_allclose(neurite1.x, neurite2.x)
         npt.assert_allclose(neurite1.y, neurite2.y)
         npt.assert_allclose(neurite1.z, neurite2.z)
         npt.assert_allclose(neurite1.d, neurite2.d)
         npt.assert_array_equal(neurite1.t, neurite2.t)
         npt.assert_array_equal(neurite1.p, neurite2.p)
 
 
 def test_neuron_building_consistency__h5():
-
-    path = f'{DATA_PATH}/valid/C010398B-P2.h5'
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    path = f"{DATA_PATH}/valid/C010398B-P2.h5"
 
     neuron1 = load_neuron(path)
     neuron2 = load_neuron_from_morphio(path)
 
     _assert_neurons_equal(neuron1, neuron2)
 
     neuron2 = load_neuron_from_morphio(morphio.Morphology(path))
 
     _assert_neurons_equal(neuron1, neuron2)
 
 
 def test_neuron_building_consistency__swc():
-
-    path = f'{DATA_PATH}/valid/C010398B-P2.CNG.swc'
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    path = f"{DATA_PATH}/valid/C010398B-P2.CNG.swc"
 
     neuron1 = load_neuron(path)
     neuron2 = load_neuron_from_morphio(path)
 
     _assert_neurons_equal(neuron1, neuron2)
 
     neuron2 = load_neuron_from_morphio(morphio.Morphology(path))
 
     _assert_neurons_equal(neuron1, neuron2)
-
-
```

### Comparing `tmd-2.2.0/tests/test_soma.py` & `TMD-2.3.0/tests/test_soma.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-'''Test tmd.soma'''
+"""Test tmd.soma."""
 import numpy as np
 from numpy import testing as npt
+
 from tmd.Soma import Soma
 
-x1 = np.array([0.,  3.,  4.,  5.,  5.])
-y1 = np.array([0.,  4.,  5.,  6.,  6.])
-z1 = np.array([ 0.,  5.,  6.,  7.,  7.])
-d1 = np.array([12.,  12.,  14.,  16.,  16.])
+x1 = np.array([0.0, 3.0, 4.0, 5.0, 5.0])
+y1 = np.array([0.0, 4.0, 5.0, 6.0, 6.0])
+z1 = np.array([0.0, 5.0, 6.0, 7.0, 7.0])
+d1 = np.array([12.0, 12.0, 14.0, 16.0, 16.0])
+
+x2 = np.array([0.0, 3.0, 4.0, 5.0, 4.0])
 
-x2 = np.array([0.,  3.,  4.,  5.,  4.])
 
 def test_soma_init_():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     soma1 = Soma.Soma(x=x1, y=y1, z=z1, d=d1)
     npt.assert_allclose(soma1.x, x1)
     npt.assert_allclose(soma1.y, y1)
     npt.assert_allclose(soma1.z, z1)
     npt.assert_allclose(soma1.d, d1)
 
+
 def test_soma_is_equal():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     soma1 = Soma.Soma(x=x1, y=y1, z=z1, d=d1)
     soma2 = Soma.Soma(x=x1, y=y1, z=z1, d=d1)
     assert soma1.is_equal(soma2)
 
     soma2 = Soma.Soma(x=x2, y=y1, z=z1, d=d1)
     assert not soma1.is_equal(soma2)
 
+
 def test_copy_soma():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     soma1 = Soma.Soma(x=x1, y=y1, z=z1, d=d1)
     soma2 = soma1.copy_soma()
     assert soma1.is_equal(soma2)
     assert soma1 != soma2
```

### Comparing `tmd-2.2.0/tests/test_topology_analysis.py` & `TMD-2.3.0/tests/test_topology_analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,190 +1,221 @@
-'''Test tmd.topology.analysis'''
+"""Test tmd.topology.analysis."""
+import os
+
 import numpy as np
 from numpy import testing as npt
+
 from tmd.Topology import analysis
-import os
 
 _path = os.path.dirname(os.path.abspath(__file__))
-DATA_PATH = os.path.join(_path, 'data')
+DATA_PATH = os.path.join(_path, "data")
 
 # Filenames for testing
-sample_ph_0_file = os.path.join(DATA_PATH, 'sample_ph_0.txt')
-sample_ph_1_file = os.path.join(DATA_PATH, 'sample_ph_1.txt')
-neuron_ph_1_file = os.path.join(DATA_PATH, 'neuron_ph_1.txt')
-neuron_ph_2_file = os.path.join(DATA_PATH, 'neuron_ph_2.txt')
+sample_ph_0_file = os.path.join(DATA_PATH, "sample_ph_0.txt")
+sample_ph_1_file = os.path.join(DATA_PATH, "sample_ph_1.txt")
+neuron_ph_1_file = os.path.join(DATA_PATH, "neuron_ph_1.txt")
+neuron_ph_2_file = os.path.join(DATA_PATH, "neuron_ph_2.txt")
 
 sample_data_0 = np.array([[10, 8], [9, 8], [9, 8]])
 sample_data_1 = np.array([[10, 7], [9, 8], [9, 8]])
 
+
 def test_load_file():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     f0 = analysis.load_file(sample_ph_0_file)
     f1 = analysis.load_file(sample_ph_1_file)
-    npt.assert_allclose(f0, np.array([[ 12.24744871,  11.18033989],
-                                     [ 11.18033989,  10.        ],
-                                     [ 12.24744871,  0.        ]]))
-    npt.assert_allclose(f1, np.array([[ 11.18033989,  10.        ],
-                                     [ 11.18033989,  0.        ]]))
+    npt.assert_allclose(
+        f0, np.array([[12.24744871, 11.18033989], [11.18033989, 10.0], [12.24744871, 0.0]])
+    )
+    npt.assert_allclose(f1, np.array([[11.18033989, 10.0], [11.18033989, 0.0]]))
+
 
 def test_histogram_horizontal():
-    bins, data = analysis.histogram_horizontal(sample_data_0, num_bins=11, min_bin=8.0, max_bin=10.0)
-    npt.assert_allclose(bins, np.array([ 8., 8.2, 8.4, 8.6, 8.8, 9., 9.2, 9.4, 9.6, 9.8, 10. ]))
-    npt.assert_allclose(data, np.array([ 3.,  3.,  3.,  3.,  1.,  3.,  1.,  1.,  1.,  1.]))
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    bins, data = analysis.histogram_horizontal(
+        sample_data_0, num_bins=11, min_bin=8.0, max_bin=10.0
+    )
+    npt.assert_allclose(bins, np.array([8.0, 8.2, 8.4, 8.6, 8.8, 9.0, 9.2, 9.4, 9.6, 9.8, 10.0]))
+    npt.assert_allclose(data, np.array([3.0, 3.0, 3.0, 3.0, 1.0, 3.0, 1.0, 1.0, 1.0, 1.0]))
     bins, data = analysis.histogram_horizontal(sample_data_0, num_bins=10)
-    npt.assert_allclose(bins, np.array([ 8.        , 8.22222222,   8.44444444,   8.66666667,
-                                        8.88888889, 9.11111111,   9.33333333,   9.55555556,
-                                        9.77777778, 10.]))
-    npt.assert_allclose(data, np.array([ 3.,  3.,  3.,  3.,  3.,  1.,  1.,  1.,  1.]))
-    bins, data = analysis.histogram_horizontal(sample_data_0, num_bins=4, min_bin=7., max_bin=10.)
-    npt.assert_allclose(bins, np.array([ 7.,   8.,   9.,  10.]))
-    npt.assert_allclose(data, np.array([ 0.,  3.,  1.]))
-    bins, data = analysis.histogram_horizontal(sample_data_1, num_bins=4, min_bin=7., max_bin=10.)
-    npt.assert_allclose(bins, np.array([ 7.,   8.,   9.,  10.]))
-    npt.assert_allclose(data, np.array([ 1.,  3.,  1.]))
+    npt.assert_allclose(
+        bins,
+        np.array(
+            [
+                8.0,
+                8.22222222,
+                8.44444444,
+                8.66666667,
+                8.88888889,
+                9.11111111,
+                9.33333333,
+                9.55555556,
+                9.77777778,
+                10.0,
+            ]
+        ),
+    )
+    npt.assert_allclose(data, np.array([3.0, 3.0, 3.0, 3.0, 3.0, 1.0, 1.0, 1.0, 1.0]))
+    bins, data = analysis.histogram_horizontal(sample_data_0, num_bins=4, min_bin=7.0, max_bin=10.0)
+    npt.assert_allclose(bins, np.array([7.0, 8.0, 9.0, 10.0]))
+    npt.assert_allclose(data, np.array([0.0, 3.0, 1.0]))
+    bins, data = analysis.histogram_horizontal(sample_data_1, num_bins=4, min_bin=7.0, max_bin=10.0)
+    npt.assert_allclose(bins, np.array([7.0, 8.0, 9.0, 10.0]))
+    npt.assert_allclose(data, np.array([1.0, 3.0, 1.0]))
+
 
 def test_histogram_stepped():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     bins, data = analysis.histogram_stepped(sample_data_0)
-    npt.assert_allclose(bins, np.array([ 8,  9, 10]))
-    npt.assert_allclose(data, np.array([ 3.,  1.]))
+    npt.assert_allclose(bins, np.array([8, 9, 10]))
+    npt.assert_allclose(data, np.array([3.0, 1.0]))
     bins, data = analysis.histogram_stepped(sample_data_1)
-    npt.assert_allclose(bins, np.array([ 7,  8,  9, 10]))
-    npt.assert_allclose(data, np.array([ 3.,  3.,  1.]))
+    npt.assert_allclose(bins, np.array([7, 8, 9, 10]))
+    npt.assert_allclose(data, np.array([3.0, 3.0, 1.0]))
+
 
 def test_distance_stepped():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     f0 = analysis.load_file(sample_ph_0_file)
     f1 = analysis.load_file(sample_ph_1_file)
     assert analysis.distance_stepped(f0, f0) == 0.0
     assert analysis.distance_stepped(f0, f0, order=1) == 0.0
     assert analysis.distance_stepped(f0, f0, order=2) == 0.0
     npt.assert_allclose(analysis.distance_stepped(f0, f1), 34.01795854515)
     npt.assert_allclose(analysis.distance_stepped(f0, f1, order=1), 34.01795854515)
     npt.assert_allclose(analysis.distance_stepped(f0, f1, order=2), 25.71017265966)
 
+
 def test_distance_horizontal():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     assert analysis.distance_horizontal(sample_data_0, sample_data_0) == 0.0
     assert analysis.distance_horizontal(sample_data_0, sample_data_1, bins=4) == 2.0
 
+
 def test_distance_horizontal_unnormed():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     assert analysis.distance_horizontal_unnormed(sample_data_0, sample_data_0) == 0.0
     assert analysis.distance_horizontal_unnormed(sample_data_0, sample_data_1, bins=4) == 1.0
 
 
 def _ph_list():
-
     return [
-                [
-                    [16.90, 6.68, 0.1, 0.1, 0.1, 0.1],
-                    [10.52, 5.98, 0.1, 0.1, 0.1, 0.1],
-                    [74.11, 0.00, 0.1, 0.1, 0.1, 0.1]
-                ],
-                [
-                    [3.010, 1.58, 0.1, 0.1, 0.1, 0.1],
-                    [15.22, 0.18, 0.1, 0.1, 0.1, 0.1],
-                    [60.48, 0.00, 0.1, 0.1, 0.1, 0.1]
-                ],
-                [
-                    [9.78, 5.30, 0.1, 0.1, 0.1, 0.1],
-                    [7.66, 1.60, 0.1, 0.1, 0.1, 0.1],
-                    [24.0, 0.00, 0.1, 0.1, 0.1, 0.1]
-                ],
-                [
-                    [6.05, 2.01, 0.1, 0.1, 0.1, 0.1],
-                    [3.91, 1.41, 0.1, 0.1, 0.1, 0.1],
-                    [8.05, 0.00, 0.1, 0.1, 0.1, 0.1]
-                ],
-                [
-                    [2.78, 0.87, 0.1, 0.1, 0.1, 0.1],
-                    [6.12, 0.21, 0.1, 0.1, 0.1, 0.1],
-                    [21.2, 0.00, 0.1, 0.1, 0.1, 0.1]
-                ],
-                [
-                    [4.99, 4.06, 0.1, 0.1, 0.1, 0.1],
-                    [4.38, 2.92, 0.1, 0.1, 0.1, 0.1],
-                    [6.79, 0.00, 0.1, 0.1, 0.1, 0.1]
-                ],
-                [
-                    [4.99, 4.06, 0.1, 0.1, 0.1, 0.1],
-                    [4.38, 2.92, 0.1, 0.1, 0.1, 0.1],
-                    [4.79, 0.00, 0.1, 0.1, 0.1, 0.1]
-                ]
+        [
+            [16.90, 6.68, 0.1, 0.1, 0.1, 0.1],
+            [10.52, 5.98, 0.1, 0.1, 0.1, 0.1],
+            [74.11, 0.00, 0.1, 0.1, 0.1, 0.1],
+        ],
+        [
+            [3.010, 1.58, 0.1, 0.1, 0.1, 0.1],
+            [15.22, 0.18, 0.1, 0.1, 0.1, 0.1],
+            [60.48, 0.00, 0.1, 0.1, 0.1, 0.1],
+        ],
+        [
+            [9.78, 5.30, 0.1, 0.1, 0.1, 0.1],
+            [7.66, 1.60, 0.1, 0.1, 0.1, 0.1],
+            [24.0, 0.00, 0.1, 0.1, 0.1, 0.1],
+        ],
+        [
+            [6.05, 2.01, 0.1, 0.1, 0.1, 0.1],
+            [3.91, 1.41, 0.1, 0.1, 0.1, 0.1],
+            [8.05, 0.00, 0.1, 0.1, 0.1, 0.1],
+        ],
+        [
+            [2.78, 0.87, 0.1, 0.1, 0.1, 0.1],
+            [6.12, 0.21, 0.1, 0.1, 0.1, 0.1],
+            [21.2, 0.00, 0.1, 0.1, 0.1, 0.1],
+        ],
+        [
+            [4.99, 4.06, 0.1, 0.1, 0.1, 0.1],
+            [4.38, 2.92, 0.1, 0.1, 0.1, 0.1],
+            [6.79, 0.00, 0.1, 0.1, 0.1, 0.1],
+        ],
+        [
+            [4.99, 4.06, 0.1, 0.1, 0.1, 0.1],
+            [4.38, 2.92, 0.1, 0.1, 0.1, 0.1],
+            [4.79, 0.00, 0.1, 0.1, 0.1, 0.1],
+        ],
     ]
 
-def test_closest_ph__reasonable_target_extent():
 
+def test_closest_ph__reasonable_target_extent():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     ph_list = _ph_list()
 
     target_extent = 6.0
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='from_above')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="from_above")
     npt.assert_equal(closest_index, 5)
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='from_below')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="from_below")
     npt.assert_equal(closest_index, 6)
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='nearest')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="nearest")
     npt.assert_equal(closest_index, 5)
 
 
 def test_closest_ph__very_big_target_extent():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     ph_list = _ph_list()
 
-    target_extent = 100.
+    target_extent = 100.0
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='from_above')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="from_above")
     npt.assert_equal(closest_index, 0)
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='from_below')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="from_below")
     npt.assert_equal(closest_index, 0)
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='nearest')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="nearest")
     npt.assert_equal(closest_index, 0)
 
 
 def test_closest_ph__very_small_target_extent():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     ph_list = _ph_list()
 
     target_extent = 2.0
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='from_above')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="from_above")
     npt.assert_equal(closest_index, 6)
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='from_below')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="from_below")
     npt.assert_equal(closest_index, 6)
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='nearest')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="nearest")
     npt.assert_equal(closest_index, 6)
 
 
 def test_closest_ph__exact_match_target_extent():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     ph_list = _ph_list()
 
     target_extent = 24.0
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='from_above')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="from_above")
     npt.assert_equal(closest_index, 2)
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='from_below')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="from_below")
     npt.assert_equal(closest_index, 2)
 
-    closest_index = analysis.closest_ph(ph_list, target_extent, method='nearest')
+    closest_index = analysis.closest_ph(ph_list, target_extent, method="nearest")
     npt.assert_equal(closest_index, 2)
 
 
 def test_apical_point():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     p1 = analysis.load_file(neuron_ph_1_file)
     p2 = analysis.load_file(neuron_ph_2_file)
     ap1 = analysis.find_apical_point_distance(p1)
     ap2 = analysis.find_apical_point_distance(p2)
     npt.assert_almost_equal(ap1, 413.2151457659, decimal=5)
     npt.assert_almost_equal(ap2, 335.8844214625, decimal=5)
 
 
 def test_apical_point_smoothed():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     p1 = analysis.load_file(neuron_ph_1_file)
     p2 = analysis.load_file(neuron_ph_2_file)
     ap1 = analysis.find_apical_point_distance_smoothed(p1, threshold=0.1)
     ap2 = analysis.find_apical_point_distance_smoothed(p2, threshold=0.1)
     npt.assert_almost_equal(ap1, 355.1980697442, decimal=5)
     npt.assert_almost_equal(ap2, 199.5273018308, decimal=5)
```

### Comparing `tmd-2.2.0/tests/test_topology_persistent_properties.py` & `TMD-2.3.0/tests/test_topology_persistent_properties.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,99 @@
-from mock import patch, Mock
+"""Test tmd.Topology.persistent_properties."""
+# pylint: disable=protected-access
 import numpy as np
 from numpy import testing as npt
+
 from tmd.Topology import persistent_properties as tested
 
 
 class MockTree:
+    """A Mock for the Tree class."""
 
     def __init__(self, points, parents=None, children=None, begs=None, ends=None):
-
         self._points = points
         self._parents = parents
         self._children = children
         self._begs = begs
         self._ends = ends
+        self.d = None
 
     def get_direction_between(self, start_id, end_id):
+        # noqa: D102 ; pylint: disable=missing-function-docstring
         vec = self._points[end_id] - self._points[start_id]
         vec /= np.linalg.norm(vec)
         return vec
 
     @property
     def sections(self):
+        # noqa: D102 ; pylint: disable=missing-function-docstring
         return self._begs, self._ends
 
     @property
     def parents_children(self):
+        # noqa: D102 ; pylint: disable=missing-function-docstring
         return self._parents, self._children
 
 
 def test_no_property():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     prop = tested.NoProperty(None)
 
     res_get = prop.get(None)
     res_inf = prop.infinite_component(None)
 
     assert isinstance(res_get, list)
     assert isinstance(res_inf, list)
 
     npt.assert_equal(len(res_get), 0)
     npt.assert_equal(len(res_inf), 0)
 
 
 def test_persistent_angles():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     tree = MockTree(
-        np.array([
-            [0., 0., 1.],
-            [0., 0., 0.],
-            [0., 0., -1.],
-            [0., 1., 0.]
-        ]),
+        np.array([[0.0, 0.0, 1.0], [0.0, 0.0, 0.0], [0.0, 0.0, -1.0], [0.0, 1.0, 0.0]]),
         parents={1: 0},
         children={1: [2, 3]},
-        begs=[-1, 1]
+        begs=[-1, 1],
     )
 
     prop = tested.PersistentAngles(tree)
 
     res_get = prop.get(1)
     res_inf = prop.infinite_component(0)
 
     assert isinstance(res_get, list)
     assert isinstance(res_inf, list)
 
-    npt.assert_allclose(res_get, [0., 0., 0.5 * np.pi, -0.5 * np.pi])
+    npt.assert_allclose(res_get, [0.0, 0.0, 0.5 * np.pi, -0.5 * np.pi])
     npt.assert_array_equal(res_inf, [np.nan, np.nan, np.nan, np.nan])
 
 
 def test_section_mean_radii():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     radii = np.array([0.1, 0.2, 0.3, 0.4, 0.5, 0.6])
 
     section_begs = np.array([0, 2, 5])
     section_ends = np.array([2, 5, 6])
 
     expected_mean_radii = [0.15, 0.4, 0.6]
 
     npt.assert_allclose(
         tested.PersistentMeanRadius._section_mean_radii(radii, section_begs, section_ends),
-        expected_mean_radii
+        expected_mean_radii,
     )
 
 
 def test_persistent_mean_radius():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     tree = MockTree(
-        np.array([
-            [0., 0., 1.],
-            [0., 0., 0.],
-            [0., 0., -1.],
-            [0., 1., 0.]
-        ]),
+        np.array([[0.0, 0.0, 1.0], [0.0, 0.0, 0.0], [0.0, 0.0, -1.0], [0.0, 1.0, 0.0]]),
         begs=np.array([0, 1, 2, 3]),
-        ends=np.array([1, 2, 3, 4])
+        ends=np.array([1, 2, 3, 4]),
     )
     tree.d = 2.0 * np.array([0.1, 0.2, 0.3, 0.4])
 
     prop = tested.PersistentMeanRadius(tree)
 
     res_get = prop.get(2)
     res_inf = prop.infinite_component(0)
@@ -106,99 +102,71 @@
     assert isinstance(res_inf, list)
 
     npt.assert_array_equal(res_get, [0.3])
     npt.assert_array_equal(res_inf, [0.1])
 
 
 def test_phi_theta():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    # pylint: disable=arguments-out-of-order
     func = tested.PersistentAngles._phi_theta
 
-    u = np.array([1., 0., 0.])
-    v = np.array([1., 0., 0.])
+    u = np.array([1.0, 0.0, 0.0])
+    v = np.array([1.0, 0.0, 0.0])
 
-    npt.assert_allclose(func(u, v), [0., 0.])
-    npt.assert_allclose(func(v, u), [0., 0.])
-    npt.assert_allclose(func(3. * u, 4. * v), [0., 0.])
+    npt.assert_allclose(func(u, v), [0.0, 0.0])
+    npt.assert_allclose(func(v, u), [0.0, 0.0])
+    npt.assert_allclose(func(3.0 * u, 4.0 * v), [0.0, 0.0])
 
-    u = np.array([1., 0., 0.])
-    v = np.array([0., 0., 1.])
+    u = np.array([1.0, 0.0, 0.0])
+    v = np.array([0.0, 0.0, 1.0])
 
-    npt.assert_allclose(func(u, v), [0., -np.pi * 0.5])
-    npt.assert_allclose(func(v, u), [0., +np.pi * 0.5])
-    npt.assert_allclose(func(2. * v, 3. * u), [0., np.pi * 0.5])
+    npt.assert_allclose(func(u, v), [0.0, -np.pi * 0.5])
+    npt.assert_allclose(func(v, u), [0.0, +np.pi * 0.5])
+    npt.assert_allclose(func(2.0 * v, 3.0 * u), [0.0, np.pi * 0.5])
 
-    u = np.array([1., 0., 0.])
-    v = np.array([-1., 0., 0.])
+    u = np.array([1.0, 0.0, 0.0])
+    v = np.array([-1.0, 0.0, 0.0])
 
-    npt.assert_allclose(func(u, v), [np.pi, 0.])
-    npt.assert_allclose(func(v, u), [-np.pi, 0.])
-    npt.assert_allclose(func(2. * v, 3. * u), [-np.pi, 0.])
+    npt.assert_allclose(func(u, v), [np.pi, 0.0])
+    npt.assert_allclose(func(v, u), [-np.pi, 0.0])
+    npt.assert_allclose(func(2.0 * v, 3.0 * u), [-np.pi, 0.0])
 
-    u = np.array([1., 1., 0.])
-    v = np.array([1., 0., 1.])
+    u = np.array([1.0, 1.0, 0.0])
+    v = np.array([1.0, 0.0, 1.0])
 
     npt.assert_allclose(func(u, v), [-0.25 * np.pi, -0.25 * np.pi])
     npt.assert_allclose(func(v, u), [0.25 * np.pi, 0.25 * np.pi])
-    npt.assert_allclose(func(2. * v, 3. * u), [0.25 * np.pi, 0.25 * np.pi])
+    npt.assert_allclose(func(2.0 * v, 3.0 * u), [0.25 * np.pi, 0.25 * np.pi])
 
 
 def test_angles_tree():
-
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     func = tested.PersistentAngles._angles_tree
 
-    tree = MockTree(
-        np.array([
-            [0., 0., 1.],
-            [0., 0., 0.],
-            [1., 0., 0.],
-            [0., 1., 0.]
-        ])
-    )
+    tree = MockTree(np.array([[0.0, 0.0, 1.0], [0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0]]))
 
     angles = func(tree, parID=0, parEND=1, ch1ID=2, ch2ID=3)
-    npt.assert_allclose(angles, [0., -0.5 * np.pi, 0.5 * np.pi, 0.])
+    npt.assert_allclose(angles, [0.0, -0.5 * np.pi, 0.5 * np.pi, 0.0])
 
-    tree = MockTree(
-        np.array([
-            [0., 0., 1.],
-            [0., 0., 0.],
-            [0., 0., -1.],
-            [0., 1., 0.]
-        ])
-    )
+    tree = MockTree(np.array([[0.0, 0.0, 1.0], [0.0, 0.0, 0.0], [0.0, 0.0, -1.0], [0.0, 1.0, 0.0]]))
 
     angles = func(tree, parID=0, parEND=1, ch1ID=2, ch2ID=3)
-    npt.assert_allclose(angles, [0., 0., 0.5 * np.pi, -0.5 * np.pi])
+    npt.assert_allclose(angles, [0.0, 0.0, 0.5 * np.pi, -0.5 * np.pi])
 
-    tree = MockTree(
-        np.array([
-            [0., 0., 1.],
-            [0., 0., 0.],
-            [0., 1., 0.],
-            [0., 0., -1.]
-        ])
-    )
+    tree = MockTree(np.array([[0.0, 0.0, 1.0], [0.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, -1.0]]))
 
     angles = func(tree, parID=0, parEND=1, ch1ID=2, ch2ID=3)
-    npt.assert_allclose(angles, [0., 0., 0.5 * np.pi, -0.5 * np.pi])
+    npt.assert_allclose(angles, [0.0, 0.0, 0.5 * np.pi, -0.5 * np.pi])
 
 
 def test_get_angles():
-
-    tree = MockTree(
-        np.array([
-            [0., 0., 1.],
-            [0., 0., 0.],
-            [0., 0., -1.],
-            [0., 1., 0.]
-        ])
-    )
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    tree = MockTree(np.array([[0.0, 0.0, 1.0], [0.0, 0.0, 0.0], [0.0, 0.0, -1.0], [0.0, 1.0, 0.0]]))
 
     begs = [-1, 1]
 
     children = {1: [2, 3]}
     parents = {1: 0}
 
     angles = tested.PersistentAngles._get_angles(tree, begs, parents, children)
-    npt.assert_allclose(angles, [[0., 0., 0., 0.], [0., 0., 0.5 * np.pi, -0.5 * np.pi]])
-
+    npt.assert_allclose(angles, [[0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.5 * np.pi, -0.5 * np.pi]])
```

### Comparing `tmd-2.2.0/tests/test_tree.py` & `TMD-2.3.0/tests/test_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,43 @@
-'''Test tmd.Tree'''
+"""Test tmd.Tree."""
 import numpy as np
 from numpy import testing as npt
+
 from tmd.Tree import Tree
 
-x1 = np.array([0.,  3.,  4.,  5.,  5.])
-y1 = np.array([0.,  4.,  5.,  6.,  6.])
-z1 = np.array([ 0.,  5.,  6.,  7.,  7.])
-d1 = np.array([12.,  12.,  14.,  16.,  16.])
+x1 = np.array([0.0, 3.0, 4.0, 5.0, 5.0])
+y1 = np.array([0.0, 4.0, 5.0, 6.0, 6.0])
+z1 = np.array([0.0, 5.0, 6.0, 7.0, 7.0])
+d1 = np.array([12.0, 12.0, 14.0, 16.0, 16.0])
 t1 = np.array([1, 1, 1, 1, 1])
-p1 = np.array([-1,  0,  1, 2, 3])
+p1 = np.array([-1, 0, 1, 2, 3])
+
+x2 = np.array([0.0, 3.0, 4.0, 5.0, 4.0])
 
-x2 = np.array([0.,  3.,  4.,  5.,  4.])
 
 def test_tree_init_():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     tree1 = Tree.Tree(x=x1, y=y1, z=z1, d=d1, t=t1, p=p1)
     npt.assert_allclose(tree1.x, x1)
     npt.assert_allclose(tree1.y, y1)
     npt.assert_allclose(tree1.z, z1)
     npt.assert_allclose(tree1.d, d1)
     npt.assert_allclose(tree1.t, t1)
     npt.assert_allclose(tree1.p, p1)
 
+
 def test_tree_is_equal():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     tree1 = Tree.Tree(x=x1, y=y1, z=z1, d=d1, t=t1, p=p1)
     tree2 = Tree.Tree(x=x1, y=y1, z=z1, d=d1, t=t1, p=p1)
     assert tree1.is_equal(tree2)
 
     tree3 = Tree.Tree(x=x2, y=y1, z=z1, d=d1, t=t1, p=p1)
     assert not tree1.is_equal(tree3)
 
+
 def test_copy_tree():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     tree1 = Tree.Tree(x=x1, y=y1, z=z1, d=d1, t=t1, p=p1)
     tree2 = tree1.copy_tree()
     assert tree1.is_equal(tree2)
     assert tree1 != tree2
```

### Comparing `tmd-2.2.0/tests/test_tree_methods.py` & `TMD-2.3.0/tests/test_tree_methods.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,194 +1,225 @@
-'''Test tmd.Tree'''
-import mock
+"""Test tmd.Tree methods."""
+# pylint: disable=protected-access
+import os
+
 import numpy as np
 from numpy import testing as npt
-from tmd.Tree import Tree
+
 from tmd.io import io
+from tmd.Tree import Tree
 from tmd.Tree import methods
-import os
 
 _path = os.path.dirname(os.path.abspath(__file__))
-DATA_PATH = os.path.join(_path, 'data')
-POP_PATH = os.path.join(DATA_PATH, 'valid')
+DATA_PATH = os.path.join(_path, "data")
+POP_PATH = os.path.join(DATA_PATH, "valid")
 
 # Filenames for testing
-sample_file = os.path.join(DATA_PATH, 'sample.swc')
-sample_file2 = os.path.join(POP_PATH, 'C010398B-P2.h5')
+sample_file = os.path.join(DATA_PATH, "sample.swc")
+sample_file2 = os.path.join(POP_PATH, "C010398B-P2.h5")
 
 neu1 = io.load_neuron(sample_file)
 neu3 = io.load_neuron(sample_file2)
 tree_h5 = neu3.axon[0]
 tree_h5_ap = neu3.apical[0]
 tree0 = neu1.neurites[0]
 tree1 = neu1.neurites[1]
 
-secs_h5_beg = np.array([0,  16,  17,  21,  30,  52,  78,  78,  52,  30, 196, 219, 219,
-                        196,  21,  17, 301, 301, 334, 334, 406, 409, 409, 406,  16, 508,
+# fmt: off
+secs_h5_beg = np.array([0, 16, 17, 21, 30, 52, 78, 78, 52, 30, 196, 219, 219,
+                        196, 21, 17, 301, 301, 334, 334, 406, 409, 409, 406, 16, 508,
                         519, 522, 612, 640, 645, 645, 640, 612, 710, 730, 738, 738, 730,
                         710, 522, 519, 508])
 
-secs_h5_end = np.array([16,  17,  21,  30,  52,  78,  86,  91, 190, 196, 219, 222, 230,
+secs_h5_end = np.array([16, 17, 21, 30, 52, 78, 86, 91, 190, 196, 219, 222, 230,
                         249, 256, 301, 330, 334, 385, 406, 409, 454, 482, 494, 508, 519,
                         522, 612, 640, 645, 678, 682, 684, 710, 730, 738, 772, 795, 804,
                         828, 829, 832, 838])
 
-secs_h5_beg_ap = np.array([0,   4,   5,   8,   9,  20,  33, 109, 109,  33,  20,   9,   8,
-                           213, 213,   5,   4])
+secs_h5_beg_ap = np.array([0, 4, 5, 8, 9, 20, 33, 109, 109, 33, 20, 9, 8,
+                           213, 213, 5, 4])
 
-secs_h5_end_ap = np.array([4,   5,   8,   9,  20,  33, 109, 121, 130, 143, 176, 205, 213,
+secs_h5_end_ap = np.array([4, 5, 8, 9, 20, 33, 109, 121, 130, 143, 176, 205, 213,
                            225, 251, 267, 292])
 
-secs_h5_beg_points_ap = np.array([0,   5,   6,   9,  10,  21,  34, 110, 122, 131, 144, 177, 206,
+secs_h5_beg_points_ap = np.array([0, 5, 6, 9, 10, 21, 34, 110, 122, 131, 144, 177, 206,
                                   214, 226, 252, 268])
 
-secs_h5_end_points_ap = np.array([4,   5,   8,   9,  20,  33, 109, 121, 130, 143, 176, 205, 213,
+secs_h5_end_points_ap = np.array([4, 5, 8, 9, 20, 33, 109, 121, 130, 143, 176, 205, 213,
                                   225, 251, 267, 292])
 
-secs_h5_beg_points = np.array([0,  17,  18,  22,  31,  53,  79,  87,  92, 191, 197, 220, 223,
+secs_h5_beg_points = np.array([0, 17, 18, 22, 31, 53, 79, 87, 92, 191, 197, 220, 223,
                                231, 250, 257, 302, 331, 335, 386, 407, 410, 455, 483, 495, 509,
                                520, 523, 613, 641, 646, 679, 683, 685, 711, 731, 739, 773, 796,
                                805, 829, 830, 833])
 
-secs_h5_end_points = np.array([16,  17,  21,  30,  52,  78,  86,  91, 190, 196, 219, 222, 230,
+secs_h5_end_points = np.array([16, 17, 21, 30, 52, 78, 86, 91, 190, 196, 219, 222, 230,
                                249, 256, 301, 330, 334, 385, 406, 409, 454, 482, 494, 508, 519,
                                522, 612, 640, 645, 678, 682, 684, 710, 730, 738, 772, 795, 804,
                                828, 829, 832, 838])
+# fmt: on
 
-x1 = np.array([0.,  1.,  2.,  3., 4.])
-y1 = np.array([0.,  2.,  3.,  4., 5.])
-z1 = np.array([0.,  3.,  4.,  5., 6.])
-d1 = np.array([2.,  4.,  6.,  8., 10.])
-t1 = np.array([2,   2,   2,   2,  2])
-p1 = np.array([-1,  0,   1,   2,  1])
+x1 = np.array([0.0, 1.0, 2.0, 3.0, 4.0])
+y1 = np.array([0.0, 2.0, 3.0, 4.0, 5.0])
+z1 = np.array([0.0, 3.0, 4.0, 5.0, 6.0])
+d1 = np.array([2.0, 4.0, 6.0, 8.0, 10.0])
+t1 = np.array([2, 2, 2, 2, 2])
+p1 = np.array([-1, 0, 1, 2, 1])
 
 tree = Tree.Tree(x=x1, y=y1, z=z1, d=d1, t=t1, p=p1)
 long_tree = Tree.Tree(
-    x=np.array([0.,  1.,  2.,  3., 4., 5., 6.]),
-    y=np.array([0.,  2.,  3.,  4., 5., 6., 7.]),
-    z=np.array([0.,  3.,  4.,  5., 6., 7., 8.]),
-    d=np.array([2.,  4.,  6.,  8., 10., 12., 14.]),
-    t=np.array([2,   2,   2,   2,  2, 2, 2]),
-    p=np.array([-1,  0,   1,   2,  2, 4, 5]),
+    x=np.array([0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0]),
+    y=np.array([0.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0]),
+    z=np.array([0.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0]),
+    d=np.array([2.0, 4.0, 6.0, 8.0, 10.0, 12.0, 14.0]),
+    t=np.array([2, 2, 2, 2, 2, 2, 2]),
+    p=np.array([-1, 0, 1, 2, 2, 4, 5]),
 )
 
+
 def test_rd():
-    assert methods._rd([0, 0], [0, 1]) == 1.
-    assert methods._rd([0, 0, 0], [0, 0, 1]) == 1.
-    assert methods._rd([1, 2, 0], [0, 2, 1]) == np.sqrt(2.)
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    assert methods._rd([0, 0], [0, 1]) == 1.0
+    assert methods._rd([0, 0, 0], [0, 0, 1]) == 1.0
+    assert methods._rd([1, 2, 0], [0, 2, 1]) == np.sqrt(2.0)
+
 
 # def test_rd_w():
 #    nt.ok_(methods._rd_w([0,0], [0,1], w=[0., 1.]) == 1.)
 #    nt.ok_(methods._rd_w([0,0], [1,1], w=[0., 2.], normed=False) == 2.)
 #    nt.ok_(methods._rd_w([0,0], [1,1], w=[0., 0.], normed=False) == 0.)
 #    nt.ok_(methods._rd_w([1,2,0], [0,2,1], normed=False) == methods._rd([1,2,0], [0,2,1]))
 
 
 def test_size():
-    assert methods.size(tree0) == 31.
-    assert methods.size(tree1) == 21.
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    assert methods.size(tree0) == 31.0
+    assert methods.size(tree1) == 21.0
 
 
 def test_get_type():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     assert tree0.get_type() == 2
     assert tree1.get_type() == 3
 
 
 def test_get_bounding_box():
-    np.allclose(tree0.get_bounding_box(),
-                       np.array([[-5.,  0., -5.],
-                                 [5., 10.,  5.]]))
-    np.allclose(tree1.get_bounding_box(),
-                       np.array([[-5.,  0., 0.],
-                                 [5., 10., 0.]]))
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    np.allclose(tree0.get_bounding_box(), np.array([[-5.0, 0.0, -5.0], [5.0, 10.0, 5.0]]))
+    np.allclose(tree1.get_bounding_box(), np.array([[-5.0, 0.0, 0.0], [5.0, 10.0, 0.0]]))
+
 
 def test_get_segments():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     seg0 = tree0.get_segments()
     seg1 = tree1.get_segments()
     seg = tree.get_segments()
     assert len(seg0) == 30
     assert len(seg1) == 20
-    npt.assert_allclose(seg, [np.array([[0.,  0.,  0.],
-                                       [1.,  2.,  3.]]),
-                             np.array([[1.,  2.,  3.],
-                                       [2.,  3.,  4.]]),
-                             np.array([[2.,  3.,  4.],
-                                       [3.,  4.,  5.]]),
-                             np.array([[1.,  2.,  3.],
-                                       [4.,  5.,  6.]])])
+    npt.assert_allclose(
+        seg,
+        [
+            np.array([[0.0, 0.0, 0.0], [1.0, 2.0, 3.0]]),
+            np.array([[1.0, 2.0, 3.0], [2.0, 3.0, 4.0]]),
+            np.array([[2.0, 3.0, 4.0], [3.0, 4.0, 5.0]]),
+            np.array([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]),
+        ],
+    )
+
 
 def test_get_point_radial_dist():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     prds = tree.get_point_radial_distances()
-    npt.assert_allclose(prds, np.array([0., 3.74165739, 5.38516481, 7.07106781, 8.77496439]))
+    npt.assert_allclose(prds, np.array([0.0, 3.74165739, 5.38516481, 7.07106781, 8.77496439]))
+
 
 def test_get_point_path_dist():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     pds = tree.get_point_path_distances()
-    npt.assert_allclose(pds, np.array([0., 3.74165739, 5.47370819, 7.205759  , 8.93780981]))
+    npt.assert_allclose(pds, np.array([0.0, 3.74165739, 5.47370819, 7.205759, 8.93780981]))
+
 
 def test_get_point_section_lengths():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     pds = tree.get_point_section_lengths()
-    npt.assert_array_almost_equal(pds, np.array([0., 3.7416575, 0., 3.46410161, 5.19615221]))
+    npt.assert_array_almost_equal(pds, np.array([0.0, 3.7416575, 0.0, 3.46410161, 5.19615221]))
 
     pds = long_tree.get_point_section_lengths()
-    npt.assert_array_almost_equal(pds, np.array([0., 0., 5.47370827, 1.73205078, 0., 0., 6.92820311]))
+    npt.assert_array_almost_equal(
+        pds, np.array([0.0, 0.0, 5.47370827, 1.73205078, 0.0, 0.0, 6.92820311])
+    )
+
 
 def test_get_trunk_length():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     pds = tree.get_trunk_length()
     npt.assert_almost_equal(pds, 3.7416575)
 
     pds = long_tree.get_trunk_length()
     npt.assert_almost_equal(pds, 5.4737083)
 
+
 def test_get_sections_2():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     secs = tree.get_sections_2()
     npt.assert_allclose(secs[0], np.array([0, 1, 1]))
     npt.assert_allclose(secs[1], np.array([1, 3, 4]))
     secs = tree_h5.get_sections_2()
     npt.assert_allclose(secs[0], secs_h5_beg)
     npt.assert_allclose(secs[1], secs_h5_end)
     secs = tree_h5_ap.get_sections_2()
     npt.assert_allclose(secs[0], secs_h5_beg_ap)
     npt.assert_allclose(secs[1], secs_h5_end_ap)
 
+
 def test_get_sections_only_points():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     secs = tree.get_sections_only_points()
     npt.assert_allclose(secs[0], np.array([0, 2, 4]))
     npt.assert_allclose(secs[1], np.array([1, 3, 4]))
     secs = tree_h5.get_sections_only_points()
     npt.assert_allclose(secs[0], secs_h5_beg_points)
     npt.assert_allclose(secs[1], secs_h5_end_points)
     secs = tree_h5_ap.get_sections_only_points()
     npt.assert_allclose(secs[0], secs_h5_beg_points_ap)
     npt.assert_allclose(secs[1], secs_h5_end_points_ap)
 
+
 def test_get_bif_term():
-    npt.assert_allclose(tree.get_bif_term(), np.array([1.,  2.,  1.,  0.,  0.]))
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    npt.assert_allclose(tree.get_bif_term(), np.array([1.0, 2.0, 1.0, 0.0, 0.0]))
+
 
 def test_get_bifurcations():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     npt.assert_allclose(tree.get_bifurcations(), np.array([1]))
 
+
 def test_get_terminations():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     npt.assert_allclose(tree.get_terminations(), np.array([3, 4]))
 
+
 def test_get_way_to_root():
+    # noqa: D103 ; pylint: disable=missing-function-docstring
     npt.assert_allclose(methods.get_way_to_root(tree), np.array([-1]))
 
 
 def test_parents_children():
-
-    tree = Tree.Tree(
+    # noqa: D103 ; pylint: disable=missing-function-docstring
+    tested_tree = Tree.Tree(
         x=np.zeros(5),
         y=np.zeros(5),
         z=np.zeros(5),
         d=np.zeros(5),
         t=np.zeros(5),
-        p=np.array([-1, 0, 1, 2, 2])
+        p=np.array([-1, 0, 1, 2, 2]),
     )
 
-    parents, children = tree.parents_children
+    parents, children = tested_tree.parents_children
 
     assert parents == {0: -1, 2: 0, 3: 2, 4: 2}
 
     expected_children = {2: [3, 4]}
 
     for key, values in expected_children.items():
         npt.assert_array_equal(children[key], values)
```

### Comparing `tmd-2.2.0/tmd/Neuron/Neuron.py` & `TMD-2.3.0/tmd/Neuron/Neuron.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,133 @@
-'''
-tmd class : Neuron
-'''
-import warnings
+"""TMD class : Neuron."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 import copy
+import warnings
+
 import numpy as np
+
 from tmd.Soma import Soma
 from tmd.Tree import Tree
 from tmd.utils import TREE_TYPE_DICT
 
 
-class Neuron(object):
-    """
-    A Neuron object is a container for Trees
-    (basal_dendrite, apical_dendrite and axon) and a Soma.
+class Neuron:
+    """A Neuron object is a container for Trees and a Soma.
+
+    The Trees can be basal_dendrite, apical_dendrite and axon.
+
+    Args:
+        name (str): The name of the Neuron.
     """
+
     # pylint: disable=import-outside-toplevel
-    from tmd.Neuron.methods import size
     from tmd.Neuron.methods import get_bounding_box
+    from tmd.Neuron.methods import size
 
-    def __init__(self, name='Neuron'):
-        '''Creates an empty Neuron object.
-        '''
+    def __init__(self, name="Neuron"):
+        """Creates an empty Neuron object."""
         self.soma = Soma.Soma()
         self.axon = []
         self.apical_dendrite = []
         self.basal_dendrite = []
         self.undefined = []
         self.name = name
 
     @property
     def neurites(self):
-        '''Get neurites'''
+        """Get neurites."""
         return self.apical_dendrite + self.axon + self.basal_dendrite + self.undefined
 
     @property
     def dendrites(self):
-        '''Get dendrites'''
+        """Get dendrites."""
         return self.apical_dendrite + self.basal_dendrite
 
     @property
     def apical(self):
-        '''Get apical dendrites'''
+        """Get apical dendrites."""
         warnings.warn(
             "The 'apical' property is deprecated, please use 'apical_dendrite' instead",
-            DeprecationWarning
+            DeprecationWarning,
         )
         return self.apical_dendrite
 
     @property
     def basal(self):
-        '''Get basal dendrites'''
+        """Get basal dendrites."""
         warnings.warn(
             "The 'basal' property is deprecated, please use 'basal_dendrite' instead",
-            DeprecationWarning
+            DeprecationWarning,
         )
         return self.basal_dendrite
 
     def rename(self, new_name):
-        """
-        Modifies the name of the Neuron to new_name.
-        """
+        """Modifies the name of the Neuron to new_name."""
         self.name = new_name
 
     def set_soma(self, new_soma):
-        """
-        If type of object is soma
-        sets the neuron soma to new_soma
-        """
+        """Set the given Soma object as the soma of the current Neuron."""
         if isinstance(new_soma, Soma.Soma):
             self.soma = new_soma
 
     def append_tree(self, new_tree, tree_types):
-        """
-        If type of object is tree
-        this function finds the type of tree
-        and adds the new_tree to the correct
-        list of trees in neuron.
+        """Append a Tree object to the Neuron.
+
+        If type of object is tree this function finds the type of tree and adds the new_tree to the
+        correct list of trees in neuron.
         """
         if isinstance(new_tree, Tree.Tree):
-
             if int(np.median(new_tree.t)) in tree_types.keys():
                 neurite_type = tree_types[int(np.median(new_tree.t))]
             else:
-                neurite_type = 'undefined'
+                neurite_type = "undefined"
             getattr(self, neurite_type).append(new_tree)
 
     def copy_neuron(self):
-        """
-        Returns a deep copy of the Neuron.
-        """
+        """Returns a deep copy of the Neuron."""
         return copy.deepcopy(self)
 
     def is_equal(self, neu):
-        '''Tests if all neuron structures are the same'''
-        eq = np.alltrue([self.soma.is_equal(neu.soma),
-                         np.alltrue([t1.is_equal(t2) for t1, t2 in
-                                     zip(self.neurites, neu.neurites)])])
+        """Tests if all neuron structures are the same."""
+        eq = np.alltrue(
+            [
+                self.soma.is_equal(neu.soma),
+                np.alltrue([t1.is_equal(t2) for t1, t2 in zip(self.neurites, neu.neurites)]),
+            ]
+        )
         return eq
 
     def is_same(self, neu):
-        '''Tests if all neuron data are the same'''
-        eq = np.alltrue([self.name == neu.name,
-                         self.soma.is_equal(neu.soma),
-                         np.alltrue([t1.is_equal(t2) for t1, t2 in
-                                     zip(self.neurites, neu.neurites)])])
+        """Tests if all neuron data are the same."""
+        eq = np.alltrue(
+            [
+                self.name == neu.name,
+                self.soma.is_equal(neu.soma),
+                np.alltrue([t1.is_equal(t2) for t1, t2 in zip(self.neurites, neu.neurites)]),
+            ]
+        )
         return eq
 
     def simplify(self):
-        '''Creates a copy of itself and simplifies all trees
-           to create a skeleton of the neuron
-        '''
+        """Creates a copy of itself and simplifies all trees to create a skeleton of the neuron."""
         neu = Neuron()
         neu.soma = self.soma.copy_soma()
 
         for tr in self.neurites:
             t = tr.extract_simplified()
             neu.append_tree(t, TREE_TYPE_DICT)
```

### Comparing `tmd-2.2.0/tmd/Topology/analysis.py` & `TMD-2.3.0/tmd/Topology/analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,222 +1,222 @@
-'''
-tmd Topology analysis algorithms implementation
-'''
+"""TMD Topology analysis algorithms implementation."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 # pylint: disable=invalid-slice-index
 import copy
 import math
 from itertools import chain
+
 import numpy as np
 from numpy.linalg import norm
-from scipy.spatial.distance import cdist
 from scipy import stats
+from scipy.spatial.distance import cdist
+
 from .statistics import get_lengths
 
 
 def collapse(ph_list):
-    '''Collapses a list of ph diagrams
-       into a single instance for plotting.
-    '''
+    """Collapses a list of ph diagrams into a single instance for plotting."""
     return [list(pi) for p in ph_list for pi in p]
 
 
 def sort_ph(ph):
-    """
-    Sorts barcode according to decreasing length of bars.
-    """
+    """Sorts barcode according to decreasing length of bars."""
     return np.array(ph)[np.argsort([p[0] - p[1] for p in ph])].tolist()
 
 
-def closest_ph(ph_list, target_extent, method='from_above'):
-    """
-    Returns the index of the persistent homology in the ph_list that has the maximum extent
-    which is closer to the target_extent according to the selected method.
+def closest_ph(ph_list, target_extent, method="from_above"):
+    """Get index of the persistent homology in the ph_list closest to a target extent.
+
+    For each ph the maximum extent is computed and compared to the target_extent according to the
+    selected method:
 
-    method:
-        from_above: smallest maximum extent that is greater or equal than target_extent
-        from_below: biggest maximum extent that is smaller or equal than target_extent
-        nearest: closest by absolute value
+    * `from_above`: smallest maximum extent that is greater or equal than target_extent.
+    * `from_below`: biggest maximum extent that is smaller or equal than target_extent.
+    * `nearest`: closest by absolute value.
     """
     n_bars = len(ph_list)
     max_extents = np.asarray([max(get_lengths(ph)) for ph in ph_list])
 
-    sorted_indices = np.argsort(max_extents, kind='mergesort')
+    sorted_indices = np.argsort(max_extents, kind="mergesort")
     sorted_extents = max_extents[sorted_indices]
 
-    if method == 'from_above':
-
-        above = np.searchsorted(sorted_extents, target_extent, side='right')
+    if method == "from_above":
+        above = np.searchsorted(sorted_extents, target_extent, side="right")
 
         # if target extent is close to current one, return this instead
         if above >= 1 and np.isclose(sorted_extents[above - 1], target_extent):
             closest_index = above - 1
         else:
             closest_index = above
 
         closest_index = np.clip(closest_index, 0, n_bars - 1)
 
-    elif method == 'from_below':
-
-        below = np.searchsorted(sorted_extents, target_extent, side='left')
+    elif method == "from_below":
+        below = np.searchsorted(sorted_extents, target_extent, side="left")
 
         # if target extent is close to current one, return this instead
         if below < n_bars and np.isclose(sorted_extents[below], target_extent):
             closest_index = below
         else:
             closest_index = below - 1
 
         closest_index = np.clip(closest_index, 0, n_bars - 1)
 
-    elif method == 'nearest':
-
+    elif method == "nearest":
         below = np.searchsorted(sorted_extents, target_extent, side="left")
         pos = np.clip(below, 0, n_bars - 2)
 
-        closest_index = \
-            min((pos, pos + 1), key=lambda i: abs(sorted_extents[i] - target_extent))
+        closest_index = min((pos, pos + 1), key=lambda i: abs(sorted_extents[i] - target_extent))
 
     else:
-        raise TypeError(f'Unknown method {method} for closest_ph')
+        raise TypeError(f"Unknown method {method} for closest_ph")
 
     return sorted_indices[closest_index]
 
 
-def load_file(filename, delimiter=' '):
-    """Load PH file in a np.array
-    """
-    with open(filename, 'r', encoding='utf-8') as f:
+def load_file(filename, delimiter=" "):
+    """Load PH file in a `np.array`."""
+    with open(filename, "r", encoding="utf-8") as f:
         ph = np.array([np.array(line.split(delimiter), dtype=float) for line in f])
     return ph
 
 
 def get_limits(phs_list, coll=True):
-    '''Returns the x-y coordinates limits (min, max)
-    for a list of persistence diagrams
-    '''
+    """Returns the x-y coordinates limits (min, max) for a list of persistence diagrams."""
     if coll:
         ph = collapse(phs_list)
     else:
         ph = copy.deepcopy(phs_list)
-    xlims = [min(np.transpose(ph)[0]), max(np.transpose(ph)[0])]
-    ylims = [min(np.transpose(ph)[1]), max(np.transpose(ph)[1])]
-    return xlims, ylims
-
-
-def get_persistence_image_data(ph, norm_factor=None, xlims=None, ylims=None, bw_method=None):
-    '''Create the data for the generation of the persistence image.
-    ph: persistence diagram
-    norm_factor: persistence image data are normalized according to this.
-        If norm_factor is provided the data will be normalized based on this,
-        otherwise they will be normalized to 1.
-    xlims, ylims: the image limits on x-y axes.
-        If xlims, ylims are provided the data will be scaled accordingly.
-    bw_method: The method used to calculate the estimator bandwidth for the gaussian_kde.
-    '''
-    if xlims is None or xlims is None:
-        xlims, ylims = get_limits(ph, coll=False)
+    xlim = [min(np.transpose(ph)[0]), max(np.transpose(ph)[0])]
+    ylim = [min(np.transpose(ph)[1]), max(np.transpose(ph)[1])]
+    return xlim, ylim
+
 
-    X, Y = np.mgrid[xlims[0]:xlims[1]:100j, ylims[0]:ylims[1]:100j]
+def get_persistence_image_data(ph, norm_factor=None, xlim=None, ylim=None, bw_method=None):
+    """Create the data for the generation of the persistence image.
+
+    Args:
+        ph: persistence diagram.
+        norm_factor: persistence image data are normalized according to this.
+            If norm_factor is provided the data will be normalized based on this,
+            otherwise they will be normalized to 1.
+        xlim: The image limits on x axis.
+        ylim: The image limits on y axis.
+        bw_method: The method used to calculate the estimator bandwidth for the gaussian_kde.
+
+    If xlim, ylim are provided the data will be scaled accordingly.
+    """
+    if xlim is None or xlim is None:
+        xlim, ylim = get_limits(ph, coll=False)
+
+    X, Y = np.mgrid[xlim[0] : xlim[1] : 100j, ylim[0] : ylim[1] : 100j]
 
     values = np.transpose(ph)
     kernel = stats.gaussian_kde(values, bw_method=bw_method)
     positions = np.vstack([X.ravel(), Y.ravel()])
     Z = np.reshape(kernel(positions).T, X.shape)
 
     if norm_factor is None:
         norm_factor = np.max(Z)
 
     return Z / norm_factor
 
 
 def get_image_diff_data(Z1, Z2, normalized=True):
-    """Takes as input two images
-       as exported from the gaussian kernel
-       plotting function, and returns
-       their difference: diff(Z1 - Z2)
-    """
+    """Get the difference of two images from the gaussian kernel plotting function."""
     if normalized:
         Z1 = Z1 / Z1.max()
         Z2 = Z2 / Z2.max()
     return Z1 - Z2
 
 
 def get_image_add_data(Z1, Z2, normalized=True):
-    """Takes as input two images
-       as exported from the gaussian kernel
-       plotting function, and returns
-       their sum: add(Z1 - Z2)
-    """
+    """Get the sum of two images from the gaussian kernel plotting function."""
     if normalized:
         Z1 = Z1 / Z1.max()
         Z2 = Z2 / Z2.max()
     return Z1 + Z2
 
 
 def histogram_horizontal(ph, num_bins=100, min_bin=None, max_bin=None):
-    """Calculate how many barcode lines are found in each bin.
-    """
+    """Calculate how many barcode lines are found in each bin."""
     ph1 = [p[:2] for p in ph]  # simplify to ensure ph corresponds to 2d barcode
 
     if min_bin is None:
         min_bin = np.min(ph1)
     if max_bin is None:
         max_bin = np.max(ph1)
 
     bins = np.linspace(min_bin, max_bin, num_bins, dtype=float)
-    binsize = (max_bin - min_bin) / (num_bins - 1.)
+    binsize = (max_bin - min_bin) / (num_bins - 1.0)
     results = np.zeros(num_bins - 1)
 
     for p in ph1:
-        ph_decompose = np.linspace(np.min(p), np.max(p),
-                                   math.ceil((np.max(p) - np.min(p)) / binsize),
-                                   dtype=float)
+        ph_decompose = np.linspace(
+            np.min(p), np.max(p), math.ceil((np.max(p) - np.min(p)) / binsize), dtype=float
+        )
 
         bin_ph = np.histogram(ph_decompose, bins=bins)[0]
         results = np.add(results, bin_ph)
 
     return bins, results
 
 
 def histogram_stepped(ph1):
-    '''Calculate step distance of ph data'''
+    """Calculate step distance of ph data."""
     bins = np.unique(list(chain(*ph1)))
     results = np.zeros(len(bins) - 1)
 
     for ph in ph1:
         for it, _ in enumerate(bins[:-1]):
             if min(ph) <= bins[it + 1] and max(ph) > bins[it]:
                 results[it] = results[it] + 1
 
     return bins, results
 
 
 def barcode_bin_centers(ph, num_bins=100, min_bin=None, max_bin=None):
     """Calculate how many barcode lines are found in each bin.
-       Returns the bin centers and the number of bars that fall within a bin.
+
+    Returns the bin centers and the number of bars that fall within a bin.
     """
     ph_2D = [p[:2] for p in ph]  # simplify to ensure ph corresponds to 2d barcode
     if min_bin is None:
         min_bin = np.min(ph_2D)
     if max_bin is None:
         max_bin = np.max(ph_2D)
     bins = np.linspace(min_bin, max_bin, num_bins, dtype=float)
     bin_centers = 0.5 * (bins[:-1] + bins[1:])
 
-    data = [bin_centers[i] for p in ph_2D for i in range(num_bins - 1)
-            if np.max(p) > bins[i + 1] and np.min(p) < bins[i]]
-    # data = []
-    # for i in range(num_bins - 1):
-    #    for p in ph_2D:
-    #        if np.max(p) > bins[i + 1] and np.min(p) < bins[i]:
-    #            data.append(bin_centers[i])
+    data = [
+        bin_centers[i]
+        for p in ph_2D
+        for i in range(num_bins - 1)
+        if np.max(p) > bins[i + 1] and np.min(p) < bins[i]
+    ]
     return bin_centers, data
 
 
 def distance_stepped(ph1, ph2, order=1):
-    '''Calculate step distance difference between two ph'''
+    """Calculate step distance difference between two ph."""
     bins1 = np.unique(list(chain(*ph1)))
     bins2 = np.unique(list(chain(*ph2)))
     bins = np.unique(np.append(bins1, bins2))
     results1 = np.zeros(len(bins) - 1)
     results2 = np.zeros(len(bins) - 1)
 
     for ph in ph1:
@@ -230,82 +230,73 @@
                 results2[it] = results2[it] + 1
 
     return norm(np.abs(np.subtract(results1, results2)) * (bins[1:] + bins[:-1]) / 2, order)
 
 
 def distance_horizontal(ph1, ph2, normalized=True, bins=100):
     """Calculate distance between two ph diagrams.
-       Distance definition:
+
+    Distance definition: TODO
     """
     _, data_1 = histogram_horizontal(ph1, num_bins=bins)
     _, data_2 = histogram_horizontal(ph2, num_bins=bins)
     return norm(np.abs(np.subtract(data_1, data_2)), normalized)
 
 
 def distance_horizontal_unnormed(ph1, ph2, normalized=True, bins=100):
-    """Calculate unnormed distance between two ph diagrams.
-    """
+    """Calculate unnormed distance between two ph diagrams."""
     maxb = np.max([np.max(ph1), np.max(ph2)])
     minb = np.min([np.min(ph1), np.min(ph2)])
     _, results1 = histogram_horizontal(ph1, num_bins=bins, min_bin=minb, max_bin=maxb)
     _, results2 = histogram_horizontal(ph2, num_bins=bins, min_bin=minb, max_bin=maxb)
     return norm(np.abs(np.subtract(results1, results2)), normalized)
 
 
-def distance_persistence_image(ph1, ph2, xlims=None, ylims=None):
-    """Computes the absolute difference of the respective persistence images
-    """
-    p1 = get_persistence_image_data(ph1, xlims=xlims, ylims=ylims)
-    p2 = get_persistence_image_data(ph2, xlims=xlims, ylims=ylims)
+def distance_persistence_image(ph1, ph2, xlim=None, ylim=None):
+    """Computes the absolute difference of the respective persistence images."""
+    p1 = get_persistence_image_data(ph1, xlim=xlim, ylim=ylim)
+    p2 = get_persistence_image_data(ph2, xlim=xlim, ylim=ylim)
     return np.sum(np.abs(get_image_diff_data(p1, p2)))
 
 
-def get_average_persistence_image(ph_list, xlims=None, ylims=None,
-                                  norm_factor=None, weighted=False):
-    '''Plots the gaussian kernel of a population of cells
-       as an average of the ph diagrams that are given.
-    '''
+def get_average_persistence_image(ph_list, xlim=None, ylim=None, norm_factor=None, weighted=False):
+    """Plot the gaussian kernel of a population as an average of the ph diagrams that are given."""
     im_av = False
     k = 1
     if weighted:
         weights = [len(p) for p in ph_list]
         weights = np.array(weights, dtype=float) / np.max(weights)
     else:
         weights = [1 for _ in ph_list]
 
     for weight, ph in zip(weights, ph_list):
         if not isinstance(im_av, np.ndarray):
             try:
-                im = get_persistence_image_data(ph, norm_factor=norm_factor,
-                                                xlims=xlims, ylims=ylims)
+                im = get_persistence_image_data(ph, norm_factor=norm_factor, xlim=xlim, ylim=ylim)
                 if not np.isnan(np.sum(im)):
                     im_av = weight * im
             except BaseException:  # pylint: disable=broad-except
                 pass
         else:
             try:
-                im = get_persistence_image_data(ph, norm_factor=norm_factor,
-                                                xlims=xlims, ylims=ylims)
+                im = get_persistence_image_data(ph, norm_factor=norm_factor, xlim=xlim, ylim=ylim)
                 if not np.isnan(np.sum(im)):
                     im_av = np.add(im_av, weight * im)
                     k = k + 1
             except BaseException:  # pylint: disable=broad-except
                 pass
     return im_av / k
 
 
 def find_apical_point_distance(ph):
-    '''
-    Finds the apical distance (measured in distance from soma)
-    based on the variation of the barcode.
-    '''
+    """Finds the apical distance (measured from the soma) based on the variation of the barcode."""
     # Computation of number of components within the barcode
     # as the number of bars with at least max length / 2
     lengths = get_lengths(ph)
-    num_components = len(np.where(np.array(lengths) >= max(lengths) / 2.)[0])
+    num_components = len(np.where(np.array(lengths) >= max(lengths) / 2.0)[0])
     # Separate the barcode into sufficiently many bins
     n_bins, counts = histogram_horizontal(ph, num_bins=3 * len(ph))
     # Compute derivatives
     der1 = counts[1:] - counts[:-1]  # first derivative
     der2 = der1[1:] - der1[:-1]  # second derivative
     # Find all points that take minimum value, defined as the number of components,
     # and have the first derivative zero == no variation
@@ -320,22 +311,20 @@
 
     if len(best_all) == 0 or n_bins[np.max(best_all)] == 0:
         return np.inf
     return n_bins[np.max(best_all)]
 
 
 def find_apical_point_distance_smoothed(ph, threshold=0.1):
-    '''
-    Finds the apical distance (measured in distance from soma)
-    based on the variation of the barcode.
-    This algorithm always computes a distance, even if
-    there is no obvious apical point.
-    Threshold corresponds to percent of minimum derivative variation
-    that is used to select the minima.
-    '''
+    """Finds the apical distance (measured from the soma) based on the variation of the barcode.
+
+    This algorithm always computes a distance, even if there is no obvious apical point.
+    The threshold corresponds to percent of minimum derivative variation that is used to select the
+    minima.
+    """
     bin_centers, data = barcode_bin_centers(ph, num_bins=100)
 
     # Gaussian kernel to smooth distribution of bars
     kde = stats.gaussian_kde(data)
     minimas = []
 
     # Compute first derivative
@@ -343,30 +332,27 @@
     # Compute second derivative
     der2 = np.gradient(der1)
 
     while len(minimas) == 0:
         # Compute minima of distribution
         minimas = np.where(abs(der1) < threshold * np.max(abs(der1)))[0]
         minimas = minimas[der2[minimas] > 0]
-        threshold *= 2.  # if threshold was too small, increase and retry
+        threshold *= 2.0  # if threshold was too small, increase and retry
     return bin_centers[minimas[0]]
 
 
 def _symmetric(p):
-    '''Returns the symmetric point of a PD point on the diagonal
-    '''
-    return [(p[0] + p[1]) / 2., (p[0] + p[1]) / 2]
+    """Returns the symmetric point of a PD point on the diagonal."""
+    return [(p[0] + p[1]) / 2.0, (p[0] + p[1]) / 2]
 
 
 def matching_munkress_modified(p1, p2, use_diag=True):
-    '''Returns a list of matching components
-       and the corresponding distance between
-       the two input diagrams
-    '''
+    """Find matching components and the corresponding distance between the two input diagrams."""
     import munkres  # pylint: disable=import-outside-toplevel
+
     if use_diag:
         p1_enh = p1 + [_symmetric(i) for i in p2]
         p2_enh = p2 + [_symmetric(i) for i in p1]
     else:
         p1_enh = p1
         p2_enh = p2
```

### Comparing `tmd-2.2.0/tmd/Topology/methods.py` & `TMD-2.3.0/tmd/Topology/methods.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,46 @@
-'''
-tmd Topology algorithms implementation
-'''
+"""TMD Topology algorithms implementation."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 import numpy as np
 import scipy.spatial as sp
+
+from tmd.Topology.analysis import sort_ph
 from tmd.Topology.persistent_properties import NoProperty
 from tmd.Topology.persistent_properties import PersistentAngles
 from tmd.Topology.persistent_properties import PersistentMeanRadius
-from tmd.Topology.analysis import sort_ph
 
 
-def write_ph(ph, output_file='test.txt'):
-    '''Writes a persistence diagram in
-       an output file.
-    '''
-    with open(output_file, 'w', encoding='utf-8') as wfile:
+def write_ph(ph, output_file="test.txt"):
+    """Writes a persistence diagram in an output file."""
+    with open(output_file, "w", encoding="utf-8") as wfile:
         for p in ph:
-            wfile.write(str(p[0]) + ' ' + str(p[1]) + '\n')
+            wfile.write(str(p[0]) + " " + str(p[1]) + "\n")
 
 
 def tree_to_property_barcode(tree, filtration_function, property_class=NoProperty):
-    """Decompose a tree data structure into a barcode, where each bar in the barcode
-    is optionally linked with a property determined by property_class.
+    """Decompose a tree data structure into a barcode.
 
-    Args:
+    Each bar in the barcode is optionally linked with a property determined by property_class.
 
+    Args:
         filtration_function (Callable[tree] -> np.ndarray):
             The filtration function to apply on the tree
 
         property_class (PersistentProperty, optional): A PersistentProperty class.By
             default the NoProperty is used which does not add entries in the barcode.
 
     Returns:
@@ -54,33 +67,29 @@
     alives = np.where(active)[0]
     point_ids_track = {al: [al] for al in alives}
     bars_to_points = []
 
     ph = []
     while len(alives) > 1:
         for alive in alives:
-
             p = parents[alive]
             c = children[p]
 
             if np.alltrue(active[c]):
-
                 active[p] = True
                 active[c] = False
 
                 mx = np.argmax(abs(point_values[c]))
                 mx_id = c[mx]
 
                 c = np.delete(c, mx)
 
                 for ci in c:
                     component_id = np.where(beg == p)[0][0]
-                    ph.append(
-                        [point_values[ci], point_values[p]] + prop.get(component_id)
-                    )
+                    ph.append([point_values[ci], point_values[p]] + prop.get(component_id))
                     bars_to_points.append(point_ids_track[ci])
 
                 point_values[p] = point_values[mx_id]
                 point_ids_track[p] = point_ids_track[mx_id] + [p]
         alives = np.where(active)[0]
 
     ph.append(
@@ -88,109 +97,106 @@
     )  # Add the last alive component
     bars_to_points.append(point_ids_track[alives[0]])
 
     return ph, bars_to_points
 
 
 def _filtration_function(feature, **kwargs):
-    """Returns filtration function lambda that will be applied point-wise
-    on the tree"""
-    return lambda tree: getattr(tree, 'get_point_' + feature)(**kwargs)
+    """Returns filtration function lambda that will be applied point-wise on the tree."""
+    return lambda tree: getattr(tree, "get_point_" + feature)(**kwargs)
 
 
-def get_persistence_diagram(tree, feature='radial_distances', **kwargs):
-    '''Method to extract ph from tree that contains mutlifurcations'''
+def get_persistence_diagram(tree, feature="radial_distances", **kwargs):
+    """Method to extract ph from tree that contains mutlifurcations."""
     ph, _ = tree_to_property_barcode(
-        tree,
-        filtration_function=_filtration_function(feature, **kwargs),
-        property_class=NoProperty
+        tree, filtration_function=_filtration_function(feature, **kwargs), property_class=NoProperty
     )
     return ph
 
 
-def get_ph_angles(tree, feature='radial_distances', **kwargs):
-    '''Method to extract ph from tree that contains mutlifurcations'''
+def get_ph_angles(tree, feature="radial_distances", **kwargs):
+    """Method to extract ph from tree that contains mutlifurcations."""
     ph, _ = tree_to_property_barcode(
         tree,
         filtration_function=_filtration_function(feature, **kwargs),
-        property_class=PersistentAngles
+        property_class=PersistentAngles,
     )
     return ph
 
 
-def get_ph_radii(tree, feature='radial_distances', **kwargs):
-    """Returns the ph diagram enhanced with the corresponding encoded radii"""
+def get_ph_radii(tree, feature="radial_distances", **kwargs):
+    """Returns the ph diagram enhanced with the corresponding encoded radii."""
     ph, _ = tree_to_property_barcode(
         tree,
         filtration_function=_filtration_function(feature, **kwargs),
-        property_class=PersistentMeanRadius
+        property_class=PersistentMeanRadius,
     )
     return ph
 
 
-def get_ph_neuron(neuron, feature='radial_distances', neurite_type='all', **kwargs):
-    '''Method to extract ph from a neuron that contains mutlifurcations'''
-
+def get_ph_neuron(neuron, feature="radial_distances", neurite_type="all", **kwargs):
+    """Method to extract ph from a neuron that contains mutlifurcations."""
     ph_all = []
 
-    if neurite_type == 'all':
-        neurite_list = ['neurites']
+    if neurite_type == "all":
+        neurite_list = ["neurites"]
     else:
         neurite_list = [neurite_type]
 
     for t in neurite_list:
         for tr in getattr(neuron, t):
             ph_all = ph_all + get_persistence_diagram(tr, feature=feature, **kwargs)
 
     return ph_all
 
 
-def extract_ph(tree, feature='radial_distances', output_file='test.txt',
-               sort=False, **kwargs):
-    '''Extracts persistent homology from tree'''
+def extract_ph(tree, feature="radial_distances", output_file="test.txt", sort=False, **kwargs):
+    """Extracts persistent homology from tree."""
     ph = get_persistence_diagram(tree, feature=feature, **kwargs)
 
     if sort:
         p = sort_ph(ph)
     else:
         p = ph
 
     write_ph(p, output_file)
 
 
-def extract_ph_neuron(neuron, feature='radial_distances', output_file=None,
-                      neurite_type='all', sort=False, **kwargs):
-    '''Extracts persistent homology from tree'''
-    ph = get_ph_neuron(neuron, feature=feature, neurite_type='all', **kwargs)
+def extract_ph_neuron(
+    neuron, feature="radial_distances", output_file=None, neurite_type="all", sort=False, **kwargs
+):
+    """Extracts persistent homology from tree."""
+    ph = get_ph_neuron(neuron, feature=feature, neurite_type="all", **kwargs)
 
     if sort:
         sort_ph(ph)
     else:
         p = ph
 
     if output_file is None:
-        output_file = 'PH_' + neuron.name + '_' + neurite_type + '.txt'
+        output_file = "PH_" + neuron.name + "_" + neurite_type + ".txt"
 
     write_ph(p, output_file)
 
 
-def get_lifetime(tree, feature='point_radial_distances'):
-    '''Returns the sequence of birth - death times for each section.
+def get_lifetime(tree, feature="point_radial_distances"):
+    """Returns the sequence of birth - death times for each section.
+
     This can be used as the first step for the approximation of P.H.
     of the radial distances of the neuronal branches.
-    '''
+    """
     begs, ends = tree.get_sections_2()
-    rd = getattr(tree, 'get_' + feature)()
+    rd = getattr(tree, "get_" + feature)()
     lifetime = np.array(len(begs) * [np.zeros(2)])
 
     for i, (beg, end) in enumerate(zip(begs, ends)):
         lifetime[i] = np.array([rd[beg], rd[end]])
 
     return lifetime
 
 
 def extract_connectivity_from_points(tree, threshold=1.0):
-    '''Extract connectivity from list of points'''
+    """Extract connectivity from list of points."""
     coords = np.transpose([tree.x, tree.y, tree.z])
     distances_matrix = sp.distance.cdist(coords, coords)
     mat = distances_matrix < threshold
     return mat
```

### Comparing `tmd-2.2.0/tmd/Tree/Tree.py` & `TMD-2.3.0/tmd/Tree/Tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,111 @@
-'''
-tmd class : Tree
-'''
+"""TMD class : Tree."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 import copy
-from cached_property import cached_property
+
 import numpy as np
 import scipy.sparse as sp
+from cached_property import cached_property
 
 
-class Tree(object):
-    '''Tree class'''
+class Tree:
+    """Tree class.
+
+    Args:
+        x (list[float]): The x-coordinates of the tree segments.
+        y (list[float]): The y-coordinates of the tree segments.
+        z (list[float]): The z-coordinate of the tree segments.
+        d (list[float]): The diameters of the tree segments.
+        t (list[int]): The types (basal_dendrite, apical_dendrite, axon) of the tree segments.
+        p (list[int]): The index of the parent of the tree segments.
+    """
+
     # pylint: disable=import-outside-toplevel
-    from tmd.Tree.methods import get_sections_2
-    from tmd.Tree.methods import get_sections_only_points
-    from tmd.Tree.methods import get_segments
+    from tmd.Tree.methods import get_bif_term
+    from tmd.Tree.methods import get_bifurcations
     from tmd.Tree.methods import get_bounding_box
-    from tmd.Tree.methods import get_pca
-    from tmd.Tree.methods import get_type
     from tmd.Tree.methods import get_direction_between
-    from tmd.Tree.methods import get_point_radial_distances
-    from tmd.Tree.methods import get_point_radial_distances_time
-    from tmd.Tree.methods import get_point_weighted_radial_distances
+    from tmd.Tree.methods import get_multifurcations
+    from tmd.Tree.methods import get_pca
     from tmd.Tree.methods import get_point_path_distances
     from tmd.Tree.methods import get_point_projection
-    from tmd.Tree.methods import get_point_section_lengths
+    from tmd.Tree.methods import get_point_radial_distances
+    from tmd.Tree.methods import get_point_radial_distances_time
     from tmd.Tree.methods import get_point_section_branch_orders
-    from tmd.Tree.methods import get_bif_term
-    from tmd.Tree.methods import get_bifurcations
-    from tmd.Tree.methods import get_multifurcations
+    from tmd.Tree.methods import get_point_section_lengths
+    from tmd.Tree.methods import get_point_weighted_radial_distances
+    from tmd.Tree.methods import get_sections_2
+    from tmd.Tree.methods import get_sections_only_points
+    from tmd.Tree.methods import get_segments
     from tmd.Tree.methods import get_terminations
     from tmd.Tree.methods import get_trunk_length
+    from tmd.Tree.methods import get_type
 
     def __init__(self, x, y, z, d, t, p):
-        '''Constructor of tmd Tree Object
-
-        Parameters
-        ----------
-        x : numpy array
-            The x-coordinates of neuron's tree segments.
-        y : numpy array
-            The y-coordinates of neuron's tree segments.
-        z : numpy array
-            The z-coordinate of neuron's tree segments.
-        d : numpy array
-            The diameters of neuron's tree segments.
-        t : numpy array
-            The types (basal, apical, axon) of neuron's tree segments.
-        p : numpy array
-            The index of the parent of neuron's tree segments.
-
-        Returns
-        -------
-        tree : Tree
-            tmd Tree object
-        '''
+        """Constructor of tmd Tree Object."""
         self.x = np.array(x, dtype=np.float32)
         self.y = np.array(y, dtype=np.float32)
         self.z = np.array(z, dtype=np.float32)
         self.d = np.array(d, dtype=np.float32)
         self.t = np.array(t, dtype=np.int32)
         self.p = np.array(p, dtype=np.int64)
-        self.dA = sp.csr_matrix((np.ones(len(self.x) - 1),
-                                 (range(1, len(self.x)), self.p[1:])),
-                                shape=(len(self.x), len(self.x)))
+        self.dA = sp.csr_matrix(
+            (np.ones(len(self.x) - 1), (range(1, len(self.x)), self.p[1:])),
+            shape=(len(self.x), len(self.x)),
+        )
 
     def copy_tree(self):
-        """
-        Returns a deep copy of the Tree.
-        """
+        """Returns a deep copy of the Tree."""
         return copy.deepcopy(self)
 
     def is_equal(self, tree):
-        '''Tests if all tree lists are the same'''
-        eq = np.alltrue([np.allclose(self.x, tree.x, atol=1e-4),
-                         np.allclose(self.y, tree.y, atol=1e-4),
-                         np.allclose(self.z, tree.z, atol=1e-4),
-                         np.allclose(self.d, tree.d, atol=1e-4),
-                         np.allclose(self.t, tree.t, atol=1e-4),
-                         np.allclose(self.p, tree.p, atol=1e-4)])
+        """Tests if all tree lists are the same."""
+        eq = np.alltrue(
+            [
+                np.allclose(self.x, tree.x, atol=1e-4),
+                np.allclose(self.y, tree.y, atol=1e-4),
+                np.allclose(self.z, tree.z, atol=1e-4),
+                np.allclose(self.d, tree.d, atol=1e-4),
+                np.allclose(self.t, tree.t, atol=1e-4),
+                np.allclose(self.p, tree.p, atol=1e-4),
+            ]
+        )
         return eq
 
     def rotate_xy(self, angle):
-        """Rotates the tree in the x-y plane
-        by the defined angle.
-        """
+        """Rotates the tree in the x-y plane by the defined angle."""
         new_x = self.x * np.cos(angle) - self.y * np.sin(angle)
         new_y = self.x * np.sin(angle) + self.y * np.cos(angle)
 
         self.x = new_x
         self.y = new_y
 
     def move_to_point(self, point=(0, 0, 0)):
-        """Moves the tree in the x-y-z plane
-        so that it starts from the selected point.
-        """
+        """Moves the tree in the x-y-z plane so that it starts from the selected point."""
         self.x = self.x - (self.x[0]) + point[0]
         self.y = self.y - (self.y[0]) + point[1]
         self.z = self.z - (self.z[0]) + point[2]
 
     def extract_simplified(self):
-        """Returns a simplified tree that corresponds
-           to the start - end of the sections points
-        """
+        """Returns a simplified tree that corresponds to the start - end of the sections points."""
         beg0, end0 = self.get_sections_2()
         sections = np.transpose([beg0, end0])
 
         x = np.zeros([len(sections) + 1])
         y = np.zeros([len(sections) + 1])
         z = np.zeros([len(sections) + 1])
         d = np.zeros([len(sections) + 1])
@@ -112,41 +113,42 @@
         p = np.zeros([len(sections) + 1])
 
         x[0] = self.x[sections[0][0]]
         y[0] = self.y[sections[0][0]]
         z[0] = self.z[sections[0][0]]
         d[0] = self.d[sections[0][0]]
         t[0] = self.t[sections[0][0]]
-        p[0] = - 1
+        p[0] = -1
 
         for i, s in enumerate(sections):
             x[i + 1] = self.x[s[1]]
             y[i + 1] = self.y[s[1]]
             z[i + 1] = self.z[s[1]]
             d[i + 1] = self.d[s[1]]
             t[i + 1] = self.t[s[1]]
             p[i + 1] = np.where(beg0 == s[0])[0][0]
 
         return Tree(x, y, z, d, t, p)
 
     @cached_property
     def sections(self):
-        """
+        """Get the sections of the current tree.
+
         Returns:
             tuple:
                 section_beg_point_ids (np.ndarray):
                     The starting point ids of sections
                 section_end_point_ids (np.ndarray)
                     The ending point ids of actions
         """
         return self.get_sections_2()
 
     @cached_property
     def parents_children(self):
-        """Returns the parents and children nodes of each section
+        """Returns the parents and children nodes of each section.
 
         Returns:
             parents (dict): Each key corresponds to a section id
                 and the respective values to the parent section ids
             children (dict): Each key corresponds to a section id
                 and the respective values to the children section ids
```

### Comparing `tmd-2.2.0/tmd/Tree/methods.py` & `TMD-2.3.0/tmd/Tree/methods.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,125 +1,131 @@
-'''
-tmd Tree's methods
-'''
+"""TMD Tree's methods."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 import copy
 from collections import OrderedDict
 from itertools import starmap
 
 import numpy as np
 import scipy.sparse as sp
 from sklearn.decomposition import PCA
 
 
 def _rd(point1, point2):
-    '''Returns euclidean distance between point1 and point2
-    '''
+    """Return euclidean distance between point1 and point2."""
     return np.linalg.norm(np.subtract(point1, point2), 2)
 
 
-def _rd_w(p1, p2, w=(1., 1., 1.), normed=True):
-    '''Returns weighted euclidean distance between p1 and p2
-    '''
+def _rd_w(p1, p2, w=(1.0, 1.0, 1.0), normed=True):
+    """Return weighted euclidean distance between p1 and p2."""
     if normed:
-        w = (np.array(w) / np.linalg.norm(w))
+        w = np.array(w) / np.linalg.norm(w)
     return np.dot(w, (np.subtract(p1, p2)))
 
 
 def size(tree):
-    '''
-    Tree method to get the size of the tree lists.
+    """Tree method to get the size of the tree lists.
+
+    .. note::
 
-    Note: All the lists of the Tree should be
-    of the same size, but this should be
-    checked in the initialization of the Tree!
-    '''
+        All the lists of the Tree should be of the same size, but this should be checked in the
+        initialization of the Tree!
+    """
     return int(len(tree.x))
 
 
 def get_type(self):
-    '''Returns type of tree
-    '''
+    """Return type of tree."""
     return int(np.median(self.t))
 
 
 def get_bounding_box(self):
-    """
-    Input
-    ------
-    tree: tmd tree
-
-    Returns
-    ---------
-    bounding_box: np.array
-        ([xmin,ymin,zmin], [xmax,ymax,zmax])
+    """Get the bounding box of the neurites.
+
+    Args:
+        self: A TMD tree.
+
+    Return:
+        bounding_box: np.array
+            ([xmin,ymin,zmin], [xmax,ymax,zmax])
     """
     xmin = np.min(self.x)
     xmax = np.max(self.x)
     ymin = np.min(self.y)
     ymax = np.max(self.y)
     zmin = np.min(self.z)
     zmax = np.max(self.z)
 
     return np.array([[xmin, ymin, zmin], [xmax, ymax, zmax]])
 
 
 # Segment features
 def get_segments(self, seg_ids=None):
-    """Return segment coordinates
-    Input
-    ------
-    tree: tmd tree
-    seg_ids: segment numbers to consider
-
-    Returns
-    ---------
-    seg_list: np.array
-        (child[x,y,z], parent[x,y,z])
+    """Return segment coordinates.
+
+    Args:
+        self: A TMD tree.
+        seg_ids: segment numbers to consider
+
+    Return:
+        seg_list: np.array
+            (child[x,y,z], parent[x,y,z])
     """
     seg_list = []
     if not seg_ids:
         seg_ids = range(0, size(self) - 1)
 
     for seg_id in seg_ids:
         par_id = self.p[seg_id + 1]
-        child_coords = np.array([self.x[seg_id + 1],
-                                 self.y[seg_id + 1],
-                                 self.z[seg_id + 1]])
-        parent_coords = np.array([self.x[par_id],
-                                  self.y[par_id],
-                                  self.z[par_id]])
+        child_coords = np.array([self.x[seg_id + 1], self.y[seg_id + 1], self.z[seg_id + 1]])
+        parent_coords = np.array([self.x[par_id], self.y[par_id], self.z[par_id]])
         seg_list.append(np.array([parent_coords, child_coords]))
 
     return seg_list
 
 
 def get_segment_lengths(tree, seg_ids=None):
-    '''Returns segment lengths
-    Input
-    ------
-    tree: tmd tree
-    seg_ids: segment numbers to consider
-    '''
+    """Return segment lengths.
+
+    Args:
+        tree: tmd tree
+        seg_ids: segment numbers to consider
+    """
     if not seg_ids:
         seg_ids = range(0, size(tree) - 1)
 
     segs = tree.get_segments(seg_ids)
 
     seg_len = np.fromiter(starmap(_rd, segs), dtype=float)
 
     return seg_len
 
 
 # Points features to be used for topological extraction
-def get_point_radial_distances(self, point=None, dim='xyz'):
-    '''Tree method to get radial distances from a point.
+def get_point_radial_distances(self, point=None, dim="xyz"):
+    """Tree method to get radial distances from a point.
+
     If point is None, the soma surface -defined by
     the initial point of the tree- will be used
     as a reference point.
-    '''
+    """
     if point is None:
         point = []
         for d in dim:
             point.append(getattr(self, d)[0])
 
     radial_distances = np.zeros(size(self), dtype=float)
 
@@ -129,20 +135,21 @@
             point_dest.append(getattr(self, d)[i])
 
         radial_distances[i] = _rd(point, point_dest)
 
     return radial_distances
 
 
-def get_point_radial_distances_time(self, point=None, dim='xyz', zero_time=0, time=1):
-    '''Tree method to get radial distances from a point.
+def get_point_radial_distances_time(self, point=None, dim="xyz", zero_time=0, time=1):
+    """Tree method to get radial distances from a point.
+
     If point is None, the soma surface -defined by
     the initial point of the tree- will be used
     as a reference point.
-    '''
+    """
     if point is None:
         point = []
         for d in dim:
             point.append(getattr(self, d)[0])
     point.append(zero_time)
 
     radial_distances = np.zeros(size(self), dtype=float)
@@ -154,20 +161,21 @@
         point_dest.append(time)
 
         radial_distances[i] = _rd(point, point_dest)
 
     return radial_distances
 
 
-def get_point_weighted_radial_distances(self, point=None, dim='xyz', w=(1, 1, 1), normed=False):
-    '''Tree method to get radial distances from a point.
+def get_point_weighted_radial_distances(self, point=None, dim="xyz", w=(1, 1, 1), normed=False):
+    """Tree method to get radial distances from a point.
+
     If point is None, the soma surface -defined by
     the initial point of the tree- will be used
     as a reference point.
-    '''
+    """
     if point is None:
         point = []
         for d in dim:
             point.append(getattr(self, d)[0])
 
     radial_distances = np.zeros(size(self), dtype=float)
 
@@ -178,197 +186,181 @@
 
         radial_distances[i] = _rd_w(point, point_dest, w, normed)
 
     return radial_distances
 
 
 def get_point_path_distances(self):
-    '''Tree method to get path distances from the root.
-    '''
+    """Tree method to get path distances from the root."""
     seg_len = get_segment_lengths(self)
     path_lengths = np.append(0, copy.deepcopy(seg_len))
     children = get_children(self)
 
     for k, v in children.items():
         path_lengths[v] = path_lengths[v] + path_lengths[k]
 
     return path_lengths
 
 
 def get_trunk_length(self):
-    '''Tree method to get the trunk (first section length).
-    '''
+    """Tree method to get the trunk (first section length)."""
     ways, end = self.get_sections_only_points()
     first_section_id = np.where(ways == 0)
     first_section_start = ways[first_section_id]
     first_section_end = end[first_section_id]
     seg_ids = range(first_section_start[0], first_section_end[0])
 
     seg_lengths = get_segment_lengths(self, seg_ids)
     return seg_lengths.sum()
 
 
 def get_point_section_lengths(self):
-    '''Tree method to get section lengths.
-    '''
+    """Tree method to get section lengths."""
     lengths = np.zeros(size(self), dtype=float)
     ways, end = self.get_sections_only_points()
     seg_len = get_segment_lengths(self)
 
     for start_id, end_id in zip(ways, end):
-        lengths[end_id] = np.sum(seg_len[max(0, start_id - 1):end_id])
+        lengths[end_id] = np.sum(seg_len[max(0, start_id - 1) : end_id])
 
     return lengths
 
 
 def get_branch_order(tree, seg_id):
-    '''Returns branch order of segment'''
+    """Return branch order of segment."""
     B = tree.get_multifurcations()
     return sum(1 if i in B else 0 for i in get_way_to_root(tree, seg_id))
 
 
 def get_point_section_branch_orders(self):
-    '''Tree method to get section lengths.
-    '''
+    """Tree method to get section lengths."""
     return np.array([get_branch_order(self, i) for i in range(size(self))])
 
 
 def get_point_projection(self, vect=(0, 1, 0), point=None):
-    """Projects each point in the tree (x,y,z) - input_point
-       to a selected vector. This gives the orientation of
-       each section according to a vector in space, if normalized,
-       otherwise it returns the relative length of the section.
+    """Projects each point in the tree (x,y,z) - input_point to a selected vector.
+
+    This gives the orientation of
+    each section according to a vector in space, if normalized,
+    otherwise it return the relative length of the section.
     """
     if point is None:
         point = [self.x[0], self.y[0], self.z[0]]
 
     xyz = np.transpose([self.x, self.y, self.z]) - point
 
     return np.dot(xyz, vect)
 
 
 # Section features
 def get_sections_2(self):
-    '''Tree method to get the indices of the parents of the first sections' points
-    and the indices of the last points of the sections.
-    '''
+    """Get indices of the parents of the first sections' points and of their last points."""
     end = np.array(sp.csr_matrix.sum(self.dA, 0) != 1)[0].nonzero()[0]
 
     if 0 in end:  # If first segment is a bifurcation
         end = end[1:]
 
     beg = np.append([0], self.p[np.delete(np.hstack([0, 1 + end]), len(end))][1:])
 
     return beg, end
 
 
 def get_sections_only_points(self):
-    '''Tree method to get the sections' begining and ending indices.
-    '''
+    """Tree method to get the sections' beginning and ending indices."""
     end = np.array(sp.csr_matrix.sum(self.dA, 0) != 1)[0].nonzero()[0]
 
     if 0 in end:  # If first segment is a bifurcation
         end = end[1:]
 
     beg = np.delete(np.hstack([0, 1 + end]), len(end))
 
     return beg, end
 
 
 def get_bif_term(self):
-    '''Returns number of children per point
-    '''
+    """Return number of children per point."""
     return np.array(sp.csr_matrix.sum(self.dA, axis=0))[0]
 
 
 def get_bifurcations(self):
-    '''Returns bifurcations
-    '''
+    """Return bifurcations."""
     bif_term = get_bif_term(self)
-    bif = np.where(bif_term == 2.)[0]
+    bif = np.where(bif_term == 2.0)[0]
     return bif
 
 
 def get_multifurcations(self):
-    '''Returns bifurcations
-    '''
+    """Return bifurcations."""
     bif_term = get_bif_term(self)
-    bif = np.where(bif_term >= 2.)[0]
+    bif = np.where(bif_term >= 2.0)[0]
     return bif
 
 
 def get_terminations(self):
-    '''Returns terminations
-    '''
+    """Return terminations."""
     bif_term = get_bif_term(self)
-    term = np.where(bif_term == 0.)[0]
+    term = np.where(bif_term == 0.0)[0]
     return term
 
 
 def get_direction_between(self, start_id=0, end_id=1):
-    '''Returns direction of a branch
-    defined as end point - start point
-    normalized as a unit vector.
-    '''
+    """Return direction of a branch.
+
+    The direction is defined as end point - start point normalized as a unit vector.
+    """
     # pylint: disable=assignment-from-no-return
-    vect = np.subtract([self.x[end_id], self.y[end_id], self.z[end_id]],
-                       [self.x[start_id], self.y[start_id], self.z[start_id]])
+    vect = np.subtract(
+        [self.x[end_id], self.y[end_id], self.z[end_id]],
+        [self.x[start_id], self.y[start_id], self.z[start_id]],
+    )
 
     if np.linalg.norm(vect) != 0.0:
         return vect / np.linalg.norm(vect)
     return vect
 
 
 def _vec_angle(u, v):
-    '''Returns the angle between v and u in 3D.
-    '''
+    """Return the angle between v and u in 3D."""
     c = np.dot(u, v) / np.linalg.norm(u) / np.linalg.norm(v)
     return np.arccos(c)
 
 
-def get_angle_between(tree, sec_id1, sec_id2):
-    '''Returns local bifurcations angle
-    between two sections, defined by their ids.
-    sec_id1: the start point of the section #1
-    sec_id2: the start point of the section #2
-    '''
+def get_angle_between(tree, sec_id1, sec_id2):  # noqa: D417
+    """Return local bifurcations angle between two sections, defined by their ids.
+
+    Args:
+        sec_id1: the start point of the section #1
+        sec_id2: the start point of the section #2
+    """
     beg, end = tree.get_sections_only_points()
     b1 = np.where(beg == sec_id1)[0][0]
     b2 = np.where(beg == sec_id2)[0][0]
 
-    u = tree.get_direction_between(beg[b1],
-                                   end[b1])
-    v = tree.get_direction_between(beg[b2],
-                                   end[b2])
+    u = tree.get_direction_between(beg[b1], end[b1])
+    v = tree.get_direction_between(beg[b2], end[b2])
 
     return _vec_angle(u, v)
 
 
 def get_way_to_root(tree, sec_id=0):
-    '''Returns way to root
-    '''
+    """Return way to root."""
     way = []
     tmp_id = sec_id
 
     while tmp_id != -1:
         way.append(tree.p[tmp_id])
         tmp_id = tree.p[tmp_id]
 
     return way
 
 
 def get_children(tree):
-    '''Returns a dictionary of children
-       for each node of the tree
-    '''
+    """Return a dictionary of children for each node of the tree."""
     return OrderedDict({i: np.where(tree.p == i)[0] for i in range(len(tree.p))})
 
 
-def get_pca(self, plane='xy', component=0):
-    '''Returns the i-th principal
-    component of PCA on the points
-    of the tree in the selected plane
-    '''
+def get_pca(self, plane="xy", component=0):
+    """Return the i-th principal component of PCA of the tree points in the selected plane."""
     pca = PCA(n_components=2)
     pca.fit(np.transpose([getattr(self, plane[0]), getattr(self, plane[1])]))
 
     return pca.components_[component]
```

### Comparing `tmd-2.2.0/tmd/io/io.py` & `TMD-2.3.0/tmd/io/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,184 +1,218 @@
-'''
-Python module that contains the functions
-about reading and writing files.
-'''
-from __future__ import print_function
+"""Python module that contains the functions about reading and writing files."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import os
+import warnings
 from pathlib import Path
+
 import numpy as _np
 from scipy import sparse as sp
 from scipy.sparse import csgraph as cs
+
+from tmd.io.conversion import convert_morphio_soma
+from tmd.io.conversion import convert_morphio_trees
+from tmd.io.h5 import read_h5
 from tmd.io.swc import SWC_DCT
 from tmd.io.swc import read_swc
 from tmd.io.swc import swc_to_data
-from tmd.io.h5 import read_h5
-from tmd.io.conversion import convert_morphio_soma
-from tmd.io.conversion import convert_morphio_trees
 from tmd.Neuron import Neuron
-from tmd.Tree import Tree
-from tmd.Soma import Soma
 from tmd.Population import Population
-from tmd.utils import TREE_TYPE_DICT
+from tmd.Soma import Soma
+from tmd.Tree import Tree
 from tmd.utils import SOMA_TYPE
+from tmd.utils import TREE_TYPE_DICT
+from tmd.utils import TmdError
 
 
-class LoadNeuronError(Exception):
-    '''Captures the exception of failing to load a single neuron
-    '''
+class LoadNeuronError(TmdError):
+    """Captures the exception of failing to load a single neuron."""
 
 
 def make_tree(data):
-    '''Make tree structure from loaded data.
-       Returns a tree of tmd.Tree
-       type.
-    '''
+    """Make tree structure from loaded data."""
     tr_data = _np.transpose(data)
 
-    parents = [_np.where(tr_data[0] == i)[0][0]
-               if len(_np.where(tr_data[0] == i)[0]) > 0
-               else - 1 for i in tr_data[6]]
-
-    return Tree.Tree(x=tr_data[SWC_DCT['x']], y=tr_data[SWC_DCT['y']], z=tr_data[SWC_DCT['z']],
-                     d=tr_data[SWC_DCT['radius']], t=tr_data[SWC_DCT['type']], p=parents)
+    parents = [
+        _np.where(tr_data[0] == i)[0][0] if len(_np.where(tr_data[0] == i)[0]) > 0 else -1
+        for i in tr_data[6]
+    ]
+
+    return Tree.Tree(
+        x=tr_data[SWC_DCT["x"]],
+        y=tr_data[SWC_DCT["y"]],
+        z=tr_data[SWC_DCT["z"]],
+        d=tr_data[SWC_DCT["radius"]],
+        t=tr_data[SWC_DCT["type"]],
+        p=parents,
+    )
 
 
 def redefine_types(user_types=None):
-    """
-    Returns tree types depending on the customized types
-        selected by the user.
+    """Return tree types depending on the customized types selected by the user.
 
-        Args:
-            user_types (dictionary or None):
+    Args:
+        user_types (dictionary or None):
 
-        Returns:
-            final_types (dict): tree types for the construction of Neuron.
+    Returns:
+        final_types (dict): tree types for the construction of Neuron.
     """
     final_tree_types = TREE_TYPE_DICT.copy()
     if user_types is not None:
         final_tree_types.update(user_types)
     return final_tree_types
 
 
-def load_neuron(input_file, line_delimiter='\n', soma_type=None,
-                user_tree_types=None, remove_duplicates=True):
-    """
-    Io method to load an swc or h5 file into a Neuron object.
-    """
+def load_neuron(
+    input_file, line_delimiter="\n", soma_type=None, user_tree_types=None, remove_duplicates=True
+):
+    """I/O method to load an swc or h5 file into a Neuron object."""
     tree_types = redefine_types(user_tree_types)
 
     # Definition of swc types from type_dict function
     if soma_type is None:
         soma_index = SOMA_TYPE
     else:
         soma_index = soma_type
 
     # Make neuron with correct filename and load data
-    if os.path.splitext(input_file)[-1] == '.swc':
-        data = swc_to_data(read_swc(input_file=input_file,
-                                    line_delimiter=line_delimiter))
-        neuron = Neuron.Neuron(name=input_file.replace('.swc', ''))
+    if os.path.splitext(input_file)[-1] == ".swc":
+        data = swc_to_data(read_swc(input_file=input_file, line_delimiter=line_delimiter))
+        neuron = Neuron.Neuron(name=str(input_file).replace(".swc", ""))
 
-    elif os.path.splitext(input_file)[-1] == '.h5':
+    elif os.path.splitext(input_file)[-1] == ".h5":
         data = read_h5(input_file=input_file, remove_duplicates=remove_duplicates)
-        neuron = Neuron.Neuron(name=input_file.replace('.h5', ''))
+        neuron = Neuron.Neuron(name=str(input_file).replace(".h5", ""))
+
+    # Check for duplicated IDs
+    IDs, counts = _np.unique(data[:, 0], return_counts=True)
+    if (counts != 1).any():
+        warnings.warn(f"The following IDs are duplicated: {IDs[counts > 1]}")
+
+    data_T = _np.transpose(data)
 
     try:
-        soma_ids = _np.where(_np.transpose(data)[1] == soma_index)[0]
+        soma_ids = _np.where(data_T[1] == soma_index)[0]
     except IndexError as exc:
-        raise LoadNeuronError('Soma points not in the expected format') from exc
+        raise LoadNeuronError("Soma points not in the expected format") from exc
 
     # Extract soma information from swc
-    soma = Soma.Soma(x=_np.transpose(data)[SWC_DCT['x']][soma_ids],
-                     y=_np.transpose(data)[SWC_DCT['y']][soma_ids],
-                     z=_np.transpose(data)[SWC_DCT['z']][soma_ids],
-                     d=_np.transpose(data)[SWC_DCT['radius']][soma_ids])
+    soma = Soma.Soma(
+        x=data_T[SWC_DCT["x"]][soma_ids],
+        y=data_T[SWC_DCT["y"]][soma_ids],
+        z=data_T[SWC_DCT["z"]][soma_ids],
+        d=data_T[SWC_DCT["radius"]][soma_ids],
+    )
 
     # Save soma in Neuron
     neuron.set_soma(soma)
-    p = _np.array(_np.transpose(data)[6], dtype=int) - _np.transpose(data)[0][0]
+    p = _np.array(data_T[6], dtype=int) - _np.transpose(data)[0][0]
     # return p, soma_ids
     try:
-        dA = sp.csr_matrix((_np.ones(len(p) - len(soma_ids)),
-                           (range(len(soma_ids), len(p)),
-                            p[len(soma_ids):])), shape=(len(p), len(p)))
+        dA = sp.csr_matrix(
+            (_np.ones(len(p) - len(soma_ids)), (range(len(soma_ids), len(p)), p[len(soma_ids) :])),
+            shape=(len(p), len(p)),
+        )
     except Exception as exc:
-        raise LoadNeuronError('Cannot create connectivity, nodes not connected correctly.') from exc
+        raise LoadNeuronError("Cannot create connectivity, nodes not connected correctly.") from exc
 
     # assuming soma points are in the beginning of the file.
-    comp = cs.connected_components(dA[len(soma_ids):, len(soma_ids):])
+    comp = cs.connected_components(dA[len(soma_ids) :, len(soma_ids) :])
 
     # Extract trees
     for i in range(comp[0]):
         tree_ids = _np.where(comp[1] == i)[0] + len(soma_ids)
         tree = make_tree(data[tree_ids])
         neuron.append_tree(tree, tree_types)
 
     return neuron
 
 
 def load_neuron_from_morphio(path_or_obj, user_tree_types=None):
-    """
-    Create Neuron object from morphio object or from path
-        loaded via morphio.
-        Supported file formats: h5, swc, asc.
-
-        Args:
-            path_or_obj (Union[str, morphio.Morphology]):
-                Filepath or morphio object
+    """Create Neuron object from morphio object or from path loaded via morphio.
+
+    Supported file formats: h5, swc, asc.
 
-        Returns:
-            neuron (Neuron): tmd Neuron object
+    Args:
+        path_or_obj (Union[str, morphio.Morphology]):
+            Filepath or morphio object
+
+    Returns:
+        neuron (Neuron): tmd Neuron object
     """
     from morphio import Morphology  # pylint: disable=import-outside-toplevel
 
     tree_types = redefine_types(user_tree_types)
 
     if isinstance(path_or_obj, (str, Path)):
         obj = Morphology(path_or_obj)
         filename = path_or_obj
     else:
         obj = path_or_obj
         # MorphIO does not support naming of objects yet.
-        filename = ''
+        filename = ""
 
     neuron = Neuron.Neuron()
     neuron.name = filename
     neuron.set_soma(convert_morphio_soma(obj.soma))
     for tree in convert_morphio_trees(obj):
         neuron.append_tree(tree, tree_types)
 
     return neuron
 
 
 def load_population(neurons, user_tree_types=None, name=None, use_morphio=False):
-    '''Loads all data of recognised format (swc, h5)
-       into a Population object.
-       Takes as input a directory or a list of files to load.
-    '''
+    """Load all data of recognised format (swc, h5) into a Population object.
+
+    Takes as input a directory or a list of files to load.
+    """
     if isinstance(neurons, (list, tuple)):
         files = neurons
-        name = name if name is not None else 'Population'
+        name = name if name is not None else "Population"
     elif os.path.isdir(neurons):  # Assumes given input is a directory
         files = [os.path.join(neurons, neuron_dir) for neuron_dir in os.listdir(neurons)]
         name = name if name is not None else os.path.basename(neurons)
+    elif os.path.isfile(neurons):  # Assumes given input is a file
+        files = [neurons]
+        name = name if name is not None else os.path.basename(neurons)
+    else:
+        raise TypeError(
+            "The format of the given neurons is not supported. "
+            "Expected an iterable of files, or a directory, or a single morphology file. "
+            f"Got: {neurons}"
+        )
 
     pop = Population.Population(name=name)
 
     for filename in files:
         try:
+            ext = os.path.splitext(filename)[-1][1:]
             if not use_morphio:
-                assert filename.endswith(('.h5', '.swc'))
+                assert ext in ("h5", "swc")
                 pop.append_neuron(load_neuron(filename, user_tree_types=user_tree_types))
             else:
-                assert filename.endswith(('.h5', '.swc', '.asc'))
-                pop.append_neuron(load_neuron_from_morphio(filename,
-                                                           user_tree_types=user_tree_types))
+                assert ext in ("h5", "swc", "asc")
+                pop.append_neuron(
+                    load_neuron_from_morphio(filename, user_tree_types=user_tree_types)
+                )
 
         except AssertionError as exc:
             error_msg = "{} is not a valid h5, swc or asc file. If asc set use_morphio to True."
             raise Warning(error_msg.format(filename)) from exc
         except LoadNeuronError:
-            print(f'File failed to load: {filename}')
+            print(f"File failed to load: {filename}")
 
     return pop
```

### Comparing `tmd-2.2.0/tmd/io/swc.py` & `TMD-2.3.0/tmd/io/swc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-'''
-Python module that contains the functions
-about reading swc files.
-'''
+"""Python module that contains the functions about reading swc files."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 import re
+
 import numpy as np
 
+from tmd.utils import TmdError
 
 # Definition of swc data container
-SWC_DCT = {'index': 0,
-           'type': 1,
-           'x': 2,
-           'y': 3,
-           'z': 4,
-           'radius': 5,
-           'parent': 6}
+SWC_DCT = {"index": 0, "type": 1, "x": 2, "y": 3, "z": 4, "radius": 5, "parent": 6}
 
 
-def read_swc(input_file, line_delimiter='\n'):
-    '''Function to properly load a swc file
-       that contains a list of sections,
-       into a 'Data' format that contains all
-       info extracting comments.
-    '''
+def read_swc(input_file, line_delimiter="\n"):
+    """Load a swc file containing a list of sections, into a 'Data' format."""
     # Read all data from file.
-    with open(input_file, 'r', encoding='utf-8') as f:
-
+    with open(input_file, "r", encoding="utf-8") as f:
         read_data = f.read()
 
     # Split data per lines
     split_data = read_data.split(line_delimiter)
 
     # Clean data from comments and empty lines
-    split_data = [a for a in split_data if '#' not in a]
-    split_data = [a for a in split_data if a != '']
+    split_data = [a for a in split_data if "#" not in a]
+    split_data = [a for a in split_data if a != ""]
 
     return np.array(split_data)
 
 
 def swc_to_data(data_swc):
-    '''Transform swc to data to be used in make_tree.
-    '''
-    expected_data = re.compile(r'^\s*([-+]?\d*\.\d+|[-+]?\d+)'
-                               r'\s*([-+]?\d*\.\d+|[-+]?\d+)\s'
-                               r'*([-+]?\d*\.\d+|[-+]?\d+)\s*'
-                               r'([-+]?\d*\.\d+|[-+]?\d+)\s*'
-                               r'([-+]?\d*\.\d+|[-+]?\d+)\s*'
-                               r'([-+]?\d*\.\d+|[-+]?\d+)\s*'
-                               r'([-+]?\d*\.\d+|[-+]?\d+)\s*$')
+    """Transform swc to data to be used in make_tree."""
+    expected_data = re.compile(
+        r"^\s*([-+]?\d*\.\d+|[-+]?\d+)"
+        r"\s*([-+]?\d*\.\d+|[-+]?\d+)\s"
+        r"*([-+]?\d*\.\d+|[-+]?\d+)\s*"
+        r"([-+]?\d*\.\d+|[-+]?\d+)\s*"
+        r"([-+]?\d*\.\d+|[-+]?\d+)\s*"
+        r"([-+]?\d*\.\d+|[-+]?\d+)\s*"
+        r"([-+]?\d*\.\d+|[-+]?\d+)\s*$"
+    )
 
     data = []
 
     for dpoint in data_swc:
-
-        if expected_data.match(dpoint.replace('\r', '')):
-
-            segment_point = np.array(expected_data.match(dpoint.replace('\r', '')).groups(),
-                                     dtype=float)
+        if expected_data.match(dpoint.replace("\r", "")):
+            segment_point = np.array(
+                expected_data.match(dpoint.replace("\r", "")).groups(), dtype=float
+            )
 
             # make the radius diameter
-            segment_point[SWC_DCT['radius']] = 2. * segment_point[SWC_DCT['radius']]
+            segment_point[SWC_DCT["radius"]] = 2.0 * segment_point[SWC_DCT["radius"]]
 
             data.append(segment_point)
 
     return np.array(data)
 
 
 def swc_data_to_lists(data):
-    """
-    Transforms data as loaded from read_swc
-    into a set of 'meaningful' lists:
+    """Transforms data as loaded from read_swc into a set of 'meaningful' lists.
 
-    x: list of floats
-        x-coordinates
+    The lists are the following:
 
-    y: list of floats
+    * x: list of floats
+        x-coordinates
+    * y: list of floats
         y-coordinates
-
-    z: list of floats
+    * z: list of floats
         z-coordinates
-
-    d: list of floats
+    * d: list of floats
         diameters
-
-    t: list of ints
+    * t: list of ints
         tree type
-
-    p: list of ints
+    * p: list of ints
         parent id
-
-    ch: dictionary
+    * ch: dictionary
         children id(s)
     """
     length = len(data)
 
     # Here we define the expected structure of the data.
     # If this structure is not followed, the data will fail
     # to load and the method will be terminated, with an error message.
 
-    expected_data = re.compile(r'^\s*([-+]?\d*\.\d+|[-+]?\d+)'
-                               r'\s*([-+]?\d*\.\d+|[-+]?\d+)\s'
-                               r'*([-+]?\d*\.\d+|[-+]?\d+)\s*'
-                               r'([-+]?\d*\.\d+|[-+]?\d+)\s*'
-                               r'([-+]?\d*\.\d+|[-+]?\d+)\s*'
-                               r'([-+]?\d*\.\d+|[-+]?\d+)\s*'
-                               r'([-+]?\d*\.\d+|[-+]?\d+)\s*$')
+    expected_data = re.compile(
+        r"^\s*([-+]?\d*\.\d+|[-+]?\d+)"
+        r"\s*([-+]?\d*\.\d+|[-+]?\d+)\s"
+        r"*([-+]?\d*\.\d+|[-+]?\d+)\s*"
+        r"([-+]?\d*\.\d+|[-+]?\d+)\s*"
+        r"([-+]?\d*\.\d+|[-+]?\d+)\s*"
+        r"([-+]?\d*\.\d+|[-+]?\d+)\s*"
+        r"([-+]?\d*\.\d+|[-+]?\d+)\s*$"
+    )
 
     # Definition of swc data from SWC_DCT function
 
     x = np.zeros(length, dtype=float)
     y = np.zeros(length, dtype=float)
     z = np.zeros(length, dtype=float)
     d = np.zeros(length, dtype=float)
     t = np.zeros(length, dtype=int)
     p = np.zeros(length, dtype=int)
     ch = {}
 
-    first_line_data = expected_data.match(data[0].replace('\r', ''))
+    first_line_data = expected_data.match(data[0].replace("\r", ""))
 
     total_offset = int(first_line_data.groups()[0])
 
     for enline in range(length):
+        segment_point = expected_data.match(data[enline].replace("\r", "")).groups()
 
-        segment_point = expected_data.match(data[enline].replace('\r', '')).groups()
-
-        x[enline] = float(segment_point[SWC_DCT['x']])
-        y[enline] = float(segment_point[SWC_DCT['y']])
-        z[enline] = float(segment_point[SWC_DCT['z']])
+        x[enline] = float(segment_point[SWC_DCT["x"]])
+        y[enline] = float(segment_point[SWC_DCT["y"]])
+        z[enline] = float(segment_point[SWC_DCT["z"]])
         # swc contains radii, and here it is transformed into diameter.
-        d[enline] = 2 * float(segment_point[SWC_DCT['radius']])
-        t[enline] = int(segment_point[SWC_DCT['type']])
+        d[enline] = 2 * float(segment_point[SWC_DCT["radius"]])
+        t[enline] = int(segment_point[SWC_DCT["type"]])
         if enline != 0:
-            p[enline] = int(segment_point[SWC_DCT['parent']]) - total_offset
+            p[enline] = int(segment_point[SWC_DCT["parent"]]) - total_offset
         else:
-            p[enline] = int(segment_point[SWC_DCT['parent']])
+            p[enline] = int(segment_point[SWC_DCT["parent"]])
 
-        if int(segment_point[SWC_DCT['index']]) - enline != total_offset:
-            raise Exception("Aborting process, with non-sequential ids error.\
-                             Fix to proceed.")
+        if int(segment_point[SWC_DCT["index"]]) - enline != total_offset:
+            raise TmdError(
+                "Aborting process, with non-sequential ids error.\
+                             Fix to proceed."
+            )
 
     for enline in range(length):
-
         ch[enline] = list(np.where(p == enline)[0])
 
     return x, y, z, d, t, p, ch
```

### Comparing `tmd-2.2.0/tmd/view/common.py` & `TMD-2.3.0/tmd/view/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,59 @@
-"""
-Module containing the common functionality
-to be used by view-plot modules.
-"""
+"""Module containing the common functionality to be used by view-plot modules."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 import os
-import numpy as np
+
 import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D  # pylint: disable=unused-import
+import numpy as np
 
 jet_map = plt.cm.get_cmap("jet")
 blues_map = plt.cm.get_cmap("Blues")
 reds_map = plt.cm.get_cmap("Reds")
 
 
 def figure_naming(pretitle=None, posttitle=None, prefile=None, postfile=None):
-    """
-    Helping function to define the strings that handle pre-post conventions
-    for viewing - plotting title and saving options.
+    """Helping function to define the strings that handle pre-post conventions.
 
-    Options
-    ----------
-    pretitle : str
-        String to include before the general title of the figure.
-        Default is None.
-
-    posttitle : str
-        String to include after the general title of the figure.
-        Default is None.
-
-    prefile : str
-        String to include before the general filename of the figure.
-        Default is None.
-
-    postfile : str
-        String to include after the general filename of the figure.
-        Default is None.
-
-    Returns
-    -------
-    string_output : string
-        String to include in the figure name and title, in a suitable form.
+    These strings can be used for viewing - plotting title and saving options.
 
+    Args:
+        pretitle : str
+            String to include before the general title of the figure.
+            Default is None.
+
+        posttitle : str
+            String to include after the general title of the figure.
+            Default is None.
+
+        prefile : str
+            String to include before the general filename of the figure.
+            Default is None.
+
+        postfile : str
+            String to include after the general filename of the figure.
+            Default is None.
+
+    Returns:
+        string_output : string
+            String to include in the figure name and title, in a suitable form.
     """
     if not pretitle:
         pretitle = ""
     else:
         pretitle = f"{pretitle} -- "
 
     if not posttitle:
@@ -61,73 +71,69 @@
     else:
         postfile = f"_{postfile}"
 
     return pretitle, posttitle, prefile, postfile
 
 
 def get_color(treecolor, tree_type):
-    """
-    If treecolor is none returns the color depending on the type:
-    Basal dendrite: "red"
-    Axon : "blue"
-    Apical dendrite: "purple"
-    Soma tree: "black"
-    Undefined-Any other unrecognised type: "green"
-    Otherwise returns the treecolor.
+    """If treecolor is none returns the color depending on the type.
+
+    The mapping is the following:
+    * Basal dendrite: "red"
+    * Axon : "blue"
+    * Apical dendrite: "purple"
+    * Soma tree: "black"
+    * Undefined-Any other unrecognised type: "green"
+
+    Otherwise return the treecolor.
     """
     if treecolor is None:
-        if tree_type == 'basal':
+        if tree_type == "basal_dendrite":
             treecolor = "red"
-        elif tree_type == 'apical':
+        elif tree_type == "apical_dendrite":
             treecolor = "purple"
-        elif tree_type == 'axon':
+        elif tree_type == "axon":
             treecolor = "blue"
-        elif tree_type == 'soma':
+        elif tree_type == "soma":
             treecolor = "black"
         else:
             treecolor = "green"
 
     return treecolor
 
 
-def get_figure(new_fig=True, new_axes=False, subplot=False, params=None,
-               no_axes=False):
-    """
-    Function to be used for viewing - plotting,
-    to initialize the matplotlib figure - axes.
-
-    Options
-    ----------
-    new_fig : boolean
-        Defines if a new figure will be created.
-        If False the current figure is returned.
-        Default is True.
-
-    subplot : subplot or False
-        Defines if a subplot will be generated.
-        If False the subplot is the standard 111.
-        Default is False.
-
-    params: dict
-        If dict not empty the parameters will
-        be passed to the initialization of the axes.
-        Default value is {}
-
-    no_axes: boolean
-        Defines the output of the function:
-        If False the axes is returned.
-        If True the figure is returned.
-        Default value is False.
-
-    Returns
-    -------
-    figure or axes
-        Returns a figure if no_axes is True,
-        or axes if no_axes is False.
+def get_figure(new_fig=True, new_axes=False, subplot=False, params=None, no_axes=False):
+    """Function to be used for viewing - plotting, to initialize the matplotlib figure - axes.
 
+    Args:
+        new_fig : boolean
+            Defines if a new figure will be created.
+            If False the current figure is returned.
+            Default is True.
+
+        subplot : subplot or False
+            Defines if a subplot will be generated.
+            If False the subplot is the standard 111.
+            Default is False.
+
+        params: dict
+            If dict not empty the parameters will
+            be passed to the initialization of the axes.
+            Default value is {}
+
+        no_axes: boolean
+            Defines the output of the function:
+            If False the axes is returned.
+            If True the figure is returned.
+            Default value is False.
+
+    Returns:
+        figure or axes
+            Returns a figure if no_axes is True,
+            or axes if no_axes is False.
     """
     if new_fig:
         fig = plt.figure()
     else:
         fig = plt.gcf()
 
     if no_axes:
@@ -147,284 +153,265 @@
     else:
         ax = plt.gca()
 
     return fig, ax
 
 
 def save_plot(fig, **kwargs):
+    """Function to be used for viewing - plotting to save a matplotlib figure.
 
-    """
-    Function to be used for viewing - plotting
-    to save a matplotlib figure.
-
-    Input
-    -------
-    fig: matplotlib figure
-
-    Options
-    ----------
-    prefile : str
-        String to include before the general filename of the figure.
-        Default is None.
-
-    postfile : str
-        String to include after the general filename of the figure.
-        Default is None.
-
-    output_path : str
-        String to define the path to the output directory.
-        Default value is './'
-
-    output_name : str
-        String to define the name of the output figure.
-        Default value is 'Figure'
-
-    output_format : str
-        String to define the format of the output figure.
-        Default value is 'png'
-
-    dpi: int
-        Define the DPI (Dots per Inch) of the figure.
-        Default value is 300.
-
-    transparent: boolean
-        If True the saved figure will have a transparent background.
-        Default value is False.
-
-    Returns
-    -------
-    Generates a figure file in the selected directory.
-
-    """
+    Args:
+        fig: matplotlib figure
 
-    prefile = kwargs.get('prefile', '')
-    postfile = kwargs.get('postfile', '')
-    output_path = kwargs.get('output_path', './')
-    output_name = kwargs.get('output_name', 'Figure')
-    output_format = kwargs.get('output_format', 'png')
-    dpi = kwargs.get('dpi', 300)
-    transparent = kwargs.get('transparent', False)
+    Keyword args:
+        prefile : str
+            String to include before the general filename of the figure.
+            Default is None.
+
+        postfile : str
+            String to include after the general filename of the figure.
+            Default is None.
+
+        output_path : str
+            String to define the path to the output directory.
+            Default value is './'
+
+        output_name : str
+            String to define the name of the output figure.
+            Default value is 'Figure'
+
+        output_format : str
+            String to define the format of the output figure.
+            Default value is 'png'
+
+        dpi: int
+            Define the DPI (Dots per Inch) of the figure.
+            Default value is 300.
+
+        transparent: boolean
+            If True the saved figure will have a transparent background.
+            Default value is False.
+
+    Returns:
+        Generates a figure file in the selected directory.
+    """
+    prefile = kwargs.get("prefile", "")
+    postfile = kwargs.get("postfile", "")
+    output_path = kwargs.get("output_path", "./")
+    output_name = kwargs.get("output_name", "Figure")
+    output_format = kwargs.get("output_format", "png")
+    dpi = kwargs.get("dpi", 300)
+    transparent = kwargs.get("transparent", False)
 
     if not os.path.exists(output_path):
         os.makedirs(output_path)  # Make output directory if non-exsiting
 
-    output = os.path.join(output_path, prefile +
-                          output_name + postfile + "." + output_format)
+    output = os.path.join(output_path, prefile + output_name + postfile + "." + output_format)
 
     plt.savefig(output, dpi=dpi, transparent=transparent)
 
     return fig
 
 
 def plot_style(fig, ax, **kwargs):
+    """Function to set the basic options of a matplotlib figure.
 
-    """
-    Function to set the basic options of a matplotlib figure,
-    to be used by viewing - plotting functions.
+    Args:
+        ax: matplotlib axes
 
-    Parameters
-    ----------
-    ax: matplotlib axes
-
-    Options
-    -------
-    pretitle : str
-        String to include before the general title of the figure.
-        Default value is None.
-
-    posttitle : str
-        String to include after the general title of the figure.
-        Default value is None.
-
-    title : str
-        The title for the figure
-        Default value is "Figure".
-
-    no_title : boolean
-        Defines the presence of a title in the figure.
-        If True the title will be set to an empty string "".
-        Default value is False.
-
-    title_fontsize : int
-        Defines the size of the title's font.
-        Default value is 14.
-
-    title_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as title arguments.
-        Default value is None.
-
-    xlabel : str
-        The xlabel for the figure
-        Default value is "X".
-
-    ylabel : str
-        The xlabel for the figure
-        Default value is "Y".
-
-    no_labels : boolean
-        Defines the presence of the labels in the figure.
-        If True the labels will be set to an empty string "".
-        Default value is False.
-
-    no_xlabel : boolean
-        Defines the presence of the xlabel in the figure.
-        If True the xlabel will be set to an empty string "".
-        Default value is False.
-
-    no_ylabel : boolean
-        Defines the presence of the ylabel in the figure.
-        If True the ylabel will be set to an empty string "".
-        Default value is False.
-
-    label_fontsize : int
-        Defines the size of the labels' font.
-        Default value is 14.
-
-    xlabel_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as xlabel arguments.
-        Default value is None.
-
-    ylabel_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as ylabel arguments.
-        Default value is None.
-
-    no_ticks : boolean
-        Defines the presence of x-y ticks in the figure.
-        If True the ticks will be empty.
-        Default value is False.
-
-    no_xticks : boolean
-        Defines the presence of x ticks in the figure.
-        If True the ticks will be empty.
-        Default value is False.
-
-    no_yticks : boolean
-        Defines the presence of y ticks in the figure.
-        If True the ticks will be empty.
-        Default value is False.
-
-    xticks : list of ticks
-        Defines the values of x ticks in the figure.
-        Default value is None.
-
-    yticks : list of ticks
-        Defines the values of y ticks in the figure.
-        Default value is None.
-
-    tick_fontsize : int
-        Defines the size of the ticks' font.
-        Default value is 12.
-
-    xticks_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as xticks arguments.
-        Default value is None.
-
-    yticks_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as yticks arguments.
-        Default value is None.
-
-    no_limits : boolean
-        Defines the presence of plot limits in the figure.
-        Default value is False.
-
-    no_xlim : boolean
-        Defines the presence of plot x-limits in the figure.
-        Default value is False.
-
-    no_ylim : boolean
-        Defines the presence of plot y-limits in the figure.
-        Default value is False.
-
-    xlim: list of two floats
-        Defines the min and the max values in x-axis.
-        Default in None
-
-    ylim: list of two floats
-        Defines the min and the max values in y-axis.
-        Default in None
-
-    no_legend : boolean
-        Defines the presence of a legend in the figure.
-        If True the legend will not be included in the Figure.
-        Default value is True.
-
-    legend_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as legend arguments.
-        Default value is None.
-
-    prefile : str
-        String to include before the general filename of the figure.
-        Default is None.
-
-    postfile : str
-        String to include after the general filename of the figure.
-        Default is None.
-
-    output_path : str
-        String to define the path to the output directory.
-        Default value is './'
-
-    output_name : str
-        String to define the name of the output figure.
-        Default value is 'Figure'
-
-    output_format : str
-        String to define the format of the output figure.
-        Default value is 'png'
-
-    dpi: int
-        Define the DPI (Dots per Inch) of the figure.
-        Default value is 300.
-
-    transparent: boolean
-        If True the saved figure will have a transparent background.
-        Default value is False.
-
-    show_plot : boolean
-        If True the figure is displayed.
-        Default value is True.
-
-    no_axes: boolean
-        If True the labels and the frame will be set off.
-        Default value is False.
-
-    tight: boolean
-        If True the set layout of matplotlib will be activated.
-        Default value is False.
-
-    Returns
-    -------
-    figure_output : figure, axes
+    Keyword args:
+        pretitle : str
+            String to include before the general title of the figure.
+            Default value is None.
+
+        posttitle : str
+            String to include after the general title of the figure.
+            Default value is None.
+
+        title : str
+            The title for the figure
+            Default value is "Figure".
+
+        no_title : boolean
+            Defines the presence of a title in the figure.
+            If True the title will be set to an empty string "".
+            Default value is False.
+
+        title_fontsize : int
+            Defines the size of the title's font.
+            Default value is 14.
+
+        title_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as title arguments.
+            Default value is None.
+
+        xlabel : str
+            The xlabel for the figure
+            Default value is "X".
+
+        ylabel : str
+            The xlabel for the figure
+            Default value is "Y".
+
+        no_labels : boolean
+            Defines the presence of the labels in the figure.
+            If True the labels will be set to an empty string "".
+            Default value is False.
+
+        no_xlabel : boolean
+            Defines the presence of the xlabel in the figure.
+            If True the xlabel will be set to an empty string "".
+            Default value is False.
+
+        no_ylabel : boolean
+            Defines the presence of the ylabel in the figure.
+            If True the ylabel will be set to an empty string "".
+            Default value is False.
+
+        label_fontsize : int
+            Defines the size of the labels' font.
+            Default value is 14.
+
+        xlabel_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as xlabel arguments.
+            Default value is None.
+
+        ylabel_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as ylabel arguments.
+            Default value is None.
+
+        no_ticks : boolean
+            Defines the presence of x-y ticks in the figure.
+            If True the ticks will be empty.
+            Default value is False.
+
+        no_xticks : boolean
+            Defines the presence of x ticks in the figure.
+            If True the ticks will be empty.
+            Default value is False.
+
+        no_yticks : boolean
+            Defines the presence of y ticks in the figure.
+            If True the ticks will be empty.
+            Default value is False.
+
+        xticks : list of ticks
+            Defines the values of x ticks in the figure.
+            Default value is None.
+
+        yticks : list of ticks
+            Defines the values of y ticks in the figure.
+            Default value is None.
+
+        tick_fontsize : int
+            Defines the size of the ticks' font.
+            Default value is 12.
+
+        xticks_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as xticks arguments.
+            Default value is None.
+
+        yticks_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as yticks arguments.
+            Default value is None.
+
+        no_limits : boolean
+            Defines the presence of plot limits in the figure.
+            Default value is False.
+
+        no_xlim : boolean
+            Defines the presence of plot x-limits in the figure.
+            Default value is False.
+
+        no_ylim : boolean
+            Defines the presence of plot y-limits in the figure.
+            Default value is False.
+
+        xlim: list of two floats
+            Defines the min and the max values in x-axis.
+            Default in None
+
+        ylim: list of two floats
+            Defines the min and the max values in y-axis.
+            Default in None
+
+        no_legend : boolean
+            Defines the presence of a legend in the figure.
+            If True the legend will not be included in the Figure.
+            Default value is True.
+
+        legend_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as legend arguments.
+            Default value is None.
+
+        prefile : str
+            String to include before the general filename of the figure.
+            Default is None.
+
+        postfile : str
+            String to include after the general filename of the figure.
+            Default is None.
+
+        output_path : str
+            String to define the path to the output directory.
+            Default value is './'
+
+        output_name : str
+            String to define the name of the output figure.
+            Default value is 'Figure'
+
+        output_format : str
+            String to define the format of the output figure.
+            Default value is 'png'
+
+        dpi: int
+            Define the DPI (Dots per Inch) of the figure.
+            Default value is 300.
+
+        transparent: boolean
+            If True the saved figure will have a transparent background.
+            Default value is False.
+
+        show_plot : boolean
+            If True the figure is displayed.
+            Default value is True.
+
+        no_axes: boolean
+            If True the labels and the frame will be set off.
+            Default value is False.
+
+        tight: boolean
+            If True the set layout of matplotlib will be activated.
+            Default value is False.
 
+    Returns:
+        figure_output : figure, axes
     """
     # Definition of title/file naming variables
-    prefile = kwargs.get('prefile', '')
-    postfile = kwargs.get('postfile', '')
-    pretitle = kwargs.get('pretitle', '')
-    posttitle = kwargs.get('posttitle', '')
+    prefile = kwargs.get("prefile", "")
+    postfile = kwargs.get("postfile", "")
+    pretitle = kwargs.get("pretitle", "")
+    posttitle = kwargs.get("posttitle", "")
 
     # Definition of global options
-    no_axes = kwargs.get('no_axes', False)
-    show_plot = kwargs.get('show_plot', True)
-    tight = kwargs.get('tight', False)
-    aspect = kwargs.get('aspect', 'auto')
+    no_axes = kwargs.get("no_axes", False)
+    show_plot = kwargs.get("show_plot", True)
+    tight = kwargs.get("tight", False)
+    aspect = kwargs.get("aspect", "auto")
 
     # Definition of save options
-    output_path = kwargs.get('output_path', None)
+    output_path = kwargs.get("output_path", None)
 
-    pretitle, posttitle, prefile, postfile = figure_naming(pretitle,
-                                                           posttitle,
-                                                           prefile,
-                                                           postfile)
+    pretitle, posttitle, prefile, postfile = figure_naming(pretitle, posttitle, prefile, postfile)
 
     fig, ax = plot_title(fig, ax, **kwargs)
 
     fig, ax = plot_labels(fig, ax, **kwargs)
 
     fig, ax = plot_ticks(fig, ax, **kwargs)
 
@@ -449,217 +436,192 @@
         plt.close()
         return (None, None)
 
     return fig, ax
 
 
 def plot_title(fig, ax, **kwargs):
+    """Function that defines the title options of a matplotlib plot.
 
-    """
-    Function that defines the title options
-    of a matplotlib plot.
+    Args:
+        fig: matplotlib figure
 
-    Parameters
-    ----------
-    fig: matplotlib figure
-
-    ax: matplotlib axes
-
-    Options
-    -------
-    pretitle : str
-        String to include before the general title of the figure.
-        Default value is None.
-
-    posttitle : str
-        String to include after the general title of the figure.
-        Default value is None.
-
-    title : str
-        Set the title for the figure.
-        If "" no title will be added.
-        Default value is "Figure".
-
-    title_fontsize : int
-        Defines the size of the title's font.
-        Default value is 14.
-
-    title_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as title arguments.
-        Default value is None.
-
-    Returns
-    -------
-    figure_output : figure, axes
+        ax: matplotlib axes
 
-    """
+    Keyword args:
+        pretitle : str
+            String to include before the general title of the figure.
+            Default value is None.
+
+        posttitle : str
+            String to include after the general title of the figure.
+            Default value is None.
+
+        title : str
+            Set the title for the figure.
+            If "" no title will be added.
+            Default value is "Figure".
+
+        title_fontsize : int
+            Defines the size of the title's font.
+            Default value is 14.
+
+        title_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as title arguments.
+            Default value is None.
 
+    Returns:
+        figure_output : figure, axes
+    """
     # Definition of title options
-    pretitle = kwargs.get('pretitle', '')
-    posttitle = kwargs.get('posttitle', '')
-    title = kwargs.get('title', 'Figure')
-    title_fontsize = kwargs.get('titlefontsize', 14)
-    title_arg = kwargs.get('titlearg', None)
+    pretitle = kwargs.get("pretitle", "")
+    posttitle = kwargs.get("posttitle", "")
+    title = kwargs.get("title", "Figure")
+    title_fontsize = kwargs.get("titlefontsize", 14)
+    title_arg = kwargs.get("titlearg", None)
 
     if title_arg is None:
         title_arg = {}
 
-    ax.set_title(pretitle + title + posttitle,
-                 fontsize=title_fontsize, **title_arg)
+    ax.set_title(pretitle + title + posttitle, fontsize=title_fontsize, **title_arg)
 
     return fig, ax
 
 
 def plot_labels(fig, ax, **kwargs):
+    """Function that defines the labels options of a matplotlib plot.
 
-    """
-    Function that defines the labels options
-    of a matplotlib plot.
+    Args
+        fig: matplotlib figure
 
-    Parameters
-    ----------
-    fig: matplotlib figure
-
-    ax: matplotlib axes
-
-    Options
-    -------
-    xlabel : str
-        The xlabel for the figure.
-        For no_xlabel set to ''.
-        Default value is "X".
-
-    ylabel : str
-        The xlabel for the figure.
-        For no_ylabel set to ''.
-        Default value is "Y".
-
-    zlabel : str
-        The zlabel for the figure.
-        For no_zlabel set to ''.
-        Default value is "Z".
-
-    label_fontsize : int
-        Defines the size of the labels' font.
-        Default value is 14.
-
-    xlabel_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as xlabel arguments.
-        Default value is None.
-
-    ylabel_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as ylabel arguments.
-        Default value is None.
-
-    zlabel_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as zlabel arguments.
-        Default value is None.
-
-    Returns
-    -------
-    figure_output : figure, axes
+        ax: matplotlib axes
 
-    """
+    Keyword args:
+        xlabel : str
+            The xlabel for the figure.
+            For no_xlabel set to ''.
+            Default value is "X".
+
+        ylabel : str
+            The xlabel for the figure.
+            For no_ylabel set to ''.
+            Default value is "Y".
+
+        zlabel : str
+            The zlabel for the figure.
+            For no_zlabel set to ''.
+            Default value is "Z".
+
+        label_fontsize : int
+            Defines the size of the labels' font.
+            Default value is 14.
+
+        xlabel_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as xlabel arguments.
+            Default value is None.
+
+        ylabel_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as ylabel arguments.
+            Default value is None.
+
+        zlabel_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as zlabel arguments.
+            Default value is None.
 
+    Returns:
+        figure_output : figure, axes
+    """
     # Definition of label options
-    xlabel = kwargs.get('xlabel', 'X')
-    ylabel = kwargs.get('ylabel', 'Y')
-    zlabel = kwargs.get('zlabel', 'Z')
-    label_fontsize = kwargs.get('labelfontsize', 14)
-    xlabel_arg = kwargs.get('xlabel_arg', None)
-    ylabel_arg = kwargs.get('ylabel_arg', None)
-    zlabel_arg = kwargs.get('zlabel_arg', None)
+    xlabel = kwargs.get("xlabel", "X")
+    ylabel = kwargs.get("ylabel", "Y")
+    zlabel = kwargs.get("zlabel", "Z")
+    label_fontsize = kwargs.get("labelfontsize", 14)
+    xlabel_arg = kwargs.get("xlabel_arg", None)
+    ylabel_arg = kwargs.get("ylabel_arg", None)
+    zlabel_arg = kwargs.get("zlabel_arg", None)
 
     if xlabel_arg is None:
         xlabel_arg = {}
 
     if ylabel_arg is None:
         ylabel_arg = {}
 
     if zlabel_arg is None:
         zlabel_arg = {}
 
     ax.set_xlabel(xlabel, fontsize=label_fontsize, **xlabel_arg)
     ax.set_ylabel(ylabel, fontsize=label_fontsize, **ylabel_arg)
 
-    if hasattr(ax, 'zaxis'):
+    if hasattr(ax, "zaxis"):
         ax.set_zlabel(zlabel, fontsize=label_fontsize, **zlabel_arg)
 
     return fig, ax
 
 
 def plot_ticks(fig, ax, **kwargs):
+    """Function that defines the labels options of a matplotlib plot.
 
-    """
-    Function that defines the labels options
-    of a matplotlib plot.
+    Args
+        fig: matplotlib figure
 
-    Parameters
-    ----------
-    fig: matplotlib figure
-
-    ax: matplotlib axes
-
-    Options
-    -------
-    xticks : list of ticks
-        Defines the values of x ticks in the figure.
-        If None the xticks will not be modified.
-        For no_xticks set to [].
-        Default value is None.
-
-    yticks : list of ticks
-        Defines the values of y ticks in the figure.
-        If None the yticks will not be modified.
-        For no_yticks set to [].
-        Default value is None.
-
-    zticks : list of ticks
-        Defines the values of z ticks in the figure.
-        If None the zticks will not be modified.
-        For no_zticks set to [].
-        Default value is None.
-
-    tick_fontsize : int
-        Defines the size of the ticks' font.
-        Default value is 12.
-
-    xticks_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as xticks arguments.
-        Default value is None.
-
-    yticks_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as yticks arguments.
-        Default value is None.
-
-    zticks_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as zticks arguments.
-        Default value is None.
-
-    Returns
-    -------
-    figure_output : figure, axes
+        ax: matplotlib axes
 
-    """
+    Keyword args:
+        xticks : list of ticks
+            Defines the values of x ticks in the figure.
+            If None the xticks will not be modified.
+            For no_xticks set to [].
+            Default value is None.
+
+        yticks : list of ticks
+            Defines the values of y ticks in the figure.
+            If None the yticks will not be modified.
+            For no_yticks set to [].
+            Default value is None.
+
+        zticks : list of ticks
+            Defines the values of z ticks in the figure.
+            If None the zticks will not be modified.
+            For no_zticks set to [].
+            Default value is None.
+
+        tick_fontsize : int
+            Defines the size of the ticks' font.
+            Default value is 12.
+
+        xticks_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as xticks arguments.
+            Default value is None.
+
+        yticks_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as yticks arguments.
+            Default value is None.
+
+        zticks_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as zticks arguments.
+            Default value is None.
 
+    Returns:
+        figure_output : figure, axes
+    """
     # Definition of tick options
-    xticks = kwargs.get('xticks', None)
-    yticks = kwargs.get('yticks', None)
-    zticks = kwargs.get('zticks', None)
-    tick_fontsize = kwargs.get('tickfontsize', 12)
-    xticks_arg = kwargs.get('xticksarg', None)
-    yticks_arg = kwargs.get('yticksarg', None)
-    zticks_arg = kwargs.get('zticksarg', None)
+    xticks = kwargs.get("xticks", None)
+    yticks = kwargs.get("yticks", None)
+    zticks = kwargs.get("zticks", None)
+    tick_fontsize = kwargs.get("tickfontsize", 12)
+    xticks_arg = kwargs.get("xticksarg", None)
+    yticks_arg = kwargs.get("yticksarg", None)
+    zticks_arg = kwargs.get("zticksarg", None)
 
     if xticks_arg is None:
         xticks_arg = {}
 
     if yticks_arg is None:
         yticks_arg = {}
 
@@ -678,153 +640,154 @@
         ax.set_zticks(zticks)
         ax.zaxis.set_tick_params(labelsize=tick_fontsize, **zticks_arg)
 
     return fig, ax
 
 
 def plot_limits(fig, ax, **kwargs):
+    """Function that defines the limit options of a matplotlib plot.
 
-    """
-    Function that defines the limit options
-    of a matplotlib plot.
+    Args:
+        fig: matplotlib figure
+
+        ax: matplotlib axes
+
+    Keyword args:
+        no_limits : boolean
+            Defines the presence of plot limits in the figure.
+            Default value is False.
 
-    Parameters
-    ----------
-    fig: matplotlib figure
-
-    ax: matplotlib axes
-
-    Options
-    -------
-    no_limits : boolean
-        Defines the presence of plot limits in the figure.
-        Default value is False.
-
-    no_xlim : boolean
-        Defines the presence of plot x-limits in the figure.
-        Default value is False.
-
-    no_ylim : boolean
-        Defines the presence of plot y-limits in the figure.
-        Default value is False.
-
-    xlim: list of two floats
-        Defines the min and the max values in x-axis.
-        Default in None
-
-    ylim: list of two floats
-        Defines the min and the max values in y-axis.
-        Default in None
-
-    Returns
-    -------
-    figure_output : figure, axes
+        no_xlim : boolean
+            Defines the presence of plot x-limits in the figure.
+            Default value is False.
 
+        no_ylim : boolean
+            Defines the presence of plot y-limits in the figure.
+            Default value is False.
+
+        xlim: list of two floats
+            Defines the min and the max values in x-axis.
+            Default in None
+
+        ylim: list of two floats
+            Defines the min and the max values in y-axis.
+            Default in None
+
+    Returns:
+        figure_output : figure, axes
     """
     # Definition of limit options
-    no_xlim = kwargs.get('no_xlim', False)
-    no_ylim = kwargs.get('no_ylim', False)
-    no_zlim = kwargs.get('no_zlim', False)
-    xlim = kwargs.get('xlim', None)
-    ylim = kwargs.get('ylim', None)
-    zlim = kwargs.get('zlim', None)
+    no_xlim = kwargs.get("no_xlim", False)
+    no_ylim = kwargs.get("no_ylim", False)
+    no_zlim = kwargs.get("no_zlim", False)
+    xlim = kwargs.get("xlim", None)
+    ylim = kwargs.get("ylim", None)
+    zlim = kwargs.get("zlim", None)
 
     if not no_xlim:
         ax.set_xlim(xlim)
     if not no_ylim:
         ax.set_ylim(ylim)
-    if hasattr(ax, 'zaxis') and not no_zlim:
+    if hasattr(ax, "zaxis") and not no_zlim:
         ax.set_zlim(zlim)
 
     return fig, ax
 
 
 def plot_legend(fig, ax, **kwargs):
+    """Function that defines the legend options of a matplotlib plot.
 
-    """
-    Function that defines the legend options
-    of a matplotlib plot.
+    Args:
+        fig: matplotlib figure
+
+        ax: matplotlib axes
 
-    Parameters
-    ----------
-    fig: matplotlib figure
-
-    ax: matplotlib axes
-
-    Options
-    -------
-    no_legend : boolean
-        Defines the presence of a legend in the figure.
-        If True the legend will not be included in the Figure.
-        Default value is True.
-
-    legend_arg : dict
-        Defines the arguments that will be passsed
-        into matplotlib as legend arguments.
-        Default value is None.
-
-    Returns
-    -------
-    figure_output : figure, axes
+    Keyword args:
+        no_legend : boolean
+            Defines the presence of a legend in the figure.
+            If True the legend will not be included in the Figure.
+            Default value is True.
+
+        legend_arg : dict
+            Defines the arguments that will be passed
+            into matplotlib as legend arguments.
+            Default value is None.
 
+    Returns:
+        figure_output : figure, axes
     """
     # Definition of legend options
-    no_legend = kwargs.get('no_legend', True)
-    legend_arg = kwargs.get('legendarg', None)
+    no_legend = kwargs.get("no_legend", True)
+    legend_arg = kwargs.get("legendarg", None)
 
     if legend_arg is None:
         legend_arg = {}
 
     if not no_legend:
         ax.legend(**legend_arg)
 
     return fig, ax
 
 
-def plot_sphere(fig, ax, center, radius, color='black', alpha=1.):
-    """
-    Plots a 3d sphere, given the center and the radius.
-    """
-
+def plot_sphere(fig, ax, center, radius, color="black", alpha=1.0):
+    """Plots a 3d sphere, given the center and the radius."""
     u = np.linspace(0, 2 * np.pi, 300)
     v = np.linspace(0, np.pi, 300)
 
     x = center[0] + radius * np.outer(np.cos(u), np.sin(v))
     y = center[1] + radius * np.outer(np.sin(u), np.sin(v))
     z = center[2] + radius * np.outer(np.ones_like(u), np.cos(v))
 
     ax.plot_surface(x, y, z, linewidth=0.0, color=color, alpha=alpha)
 
     return fig, ax
 
 
-def plot_img_basic(img, new_fig=True, subplot=111, title='', xlims=None, ylims=None, colorbar=False,
-                   cmap=jet_map, vmin=None, vmax=None, masked=False, threshold=0.01, **kwargs):
-    '''Plots the gaussian kernel of the input image.
-    '''
-    if xlims is None:
-        xlims = (0, 100)
-    if ylims is None:
-        ylims = (0, 100)
+def plot_img_basic(
+    img,
+    new_fig=True,
+    subplot=111,
+    title="",
+    xlim=None,
+    ylim=None,
+    colorbar=False,
+    cmap=jet_map,
+    vmin=None,
+    vmax=None,
+    masked=False,
+    threshold=0.01,
+    **kwargs,
+):
+    """Plots the gaussian kernel of the input image."""
+    if xlim is None:
+        xlim = (0, 100)
+    if ylim is None:
+        ylim = (0, 100)
 
     if vmin is None:
         vmin = np.min(img)
     if vmax is None:
         vmax = np.max(img)
 
     fig, ax = get_figure(new_fig=new_fig, subplot=subplot)
 
     if masked:
         img = np.ma.masked_where((threshold > np.abs(img)), img)
 
-    cax = ax.imshow(np.rot90(img), vmin=vmin, vmax=vmax, cmap=cmap,
-                    interpolation='bilinear', extent=xlims + ylims)
-
-    kwargs['xlim'] = xlims
-    kwargs['ylim'] = ylims
-    kwargs['title'] = title
+    cax = ax.imshow(
+        np.rot90(img),
+        vmin=vmin,
+        vmax=vmax,
+        cmap=cmap,
+        interpolation="bilinear",
+        extent=xlim + ylim,
+    )
+
+    kwargs["xlim"] = xlim
+    kwargs["ylim"] = ylim
+    kwargs["title"] = title
 
     if colorbar:
         plt.colorbar(cax)
-    ax.set_aspect('equal')
+    ax.set_aspect("equal")
 
-    return plot_style(fig=fig, ax=ax, aspect='equal', **kwargs)
+    return plot_style(fig=fig, ax=ax, aspect="equal", **kwargs)
```

### Comparing `tmd-2.2.0/tmd/view/plot.py` & `TMD-2.3.0/tmd/view/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,275 +1,390 @@
-"""Plotting functions of tmd"""
+"""Plotting functions of TMD."""
+
+# Copyright (C) 2022  Blue Brain Project, EPFL
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import numpy as np
 from matplotlib import pylab as plt
-from tmd.view import common as cm
+
 from tmd.Topology import analysis
-from tmd.view.common import jet_map
 from tmd.Topology.statistics import transform_ph_to_length
+from tmd.view import common as cm
+from tmd.view.common import jet_map
 
 
-def barcode(ph, new_fig=True, subplot=False, color='b', linewidth=1.2, **kwargs):
-    """
-    Generates a 2d figure (barcode) of the persistent homology
-    of a tree as it has been computed by
-    Topology.get_persistent_homology method.
+def barcode(ph, new_fig=True, subplot=False, color="b", linewidth=1.2, **kwargs):
+    """Generate a 2d figure (barcode) of the persistent homology of a tree.
+
+    The persistent homology should have been computed by Topology.get_persistent_homology method.
     """
     # Initialization of matplotlib figure and axes.
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
     ph_sort = analysis.sort_ph(ph)
 
-    for ip, p in enumerate(ph_sort):
-        ax.plot(p[:2], [ip, ip], c=color, linewidth=linewidth)
-
-    kwargs['title'] = kwargs.get('title', 'Persistence barcode')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'Lifetime: radial distance from soma')
+    for ibar, pbar in enumerate(ph_sort):
+        bar_color = color[ibar] if isinstance(color, list) else color
+        ax.plot(pbar[:2], [ibar, ibar], c=bar_color, linewidth=linewidth)
+
+    all_kwargs = {
+        "title": "Persistence barcode",
+        "xlabel": "Lifetime: radial distance",
+    }
+    all_kwargs.update(kwargs)
 
     plt.ylim([-1, len(ph_sort)])
-    return cm.plot_style(fig=fig, ax=ax, **kwargs)
+    return cm.plot_style(fig=fig, ax=ax, **all_kwargs)
 
 
-def barcode_enhanced(ph, new_fig=True, subplot=False, linewidth=1.2,
-                     valID=2, cmap=jet_map, **kwargs):
-    """
-    Generates a 2d figure (barcode) of the persistent homology
-    of a tree enhanced by a parameter encodes in ph[valID]
+def barcode_enhanced(
+    ph, new_fig=True, subplot=False, linewidth=1.2, valID=2, cmap=jet_map, **kwargs
+):
+    """Generate a 2d figure (barcode) of the persistent homology of an enhanced tree.
+
+    The tree is enhanced by a parameter encoded in ph[valID].
     """
     # Initialization of matplotlib figure and axes.
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
     val_max = np.max(ph, axis=0)[valID]
 
     # Hack for colorbar creation
-    Z = [[0, 0], [0, 0]]
+    Z = [[-100, -100], [-100, -100]]
     levels = np.linspace(0.0, val_max, 200)
     CS3 = plt.contourf(Z, levels, cmap=cmap)
 
     def sort_ph_enhanced(ph, valID):
-        """
-        Sorts barcode according to length.
-        """
-        ph_sort = [p[:valID + 1] + [np.abs(p[0] - p[1])] for p in ph]
+        """Sorts barcode according to length."""
+        ph_sort = [p[: valID + 1] + [np.abs(p[0] - p[1])] for p in ph]
         ph_sort.sort(key=lambda x: x[valID + 1])
         return ph_sort
 
     ph_sort = sort_ph_enhanced(ph, valID)
 
-    for ip, p in enumerate(ph_sort):
-        ax.plot(p[:2], [ip, ip], c=cmap(p[valID] / val_max), linewidth=linewidth)
+    for ibar, pbar in enumerate(ph_sort):
+        ax.plot(pbar[:2], [ibar, ibar], c=cmap(pbar[valID] / val_max), linewidth=linewidth)
+
+    all_kwargs = {
+        "title": "Persistence barcode",
+        "xlabel": "Lifetime",
+    }
+    all_kwargs.update(kwargs)
 
-    kwargs['title'] = kwargs.get('title', 'Barcode of p.h.')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'Lifetime')
     plt.ylim([-1, len(ph_sort)])
     plt.colorbar(CS3)
 
-    return cm.plot_style(fig=fig, ax=ax, **kwargs)
+    return cm.plot_style(fig=fig, ax=ax, **all_kwargs)
 
 
-def diagram(ph, new_fig=True, subplot=False, color='b', alpha=1.0,
-            edgecolors='black', s=30, **kwargs):
-    """
-    Generates a 2d figure (ph diagram) of the persistent homology of a tree.
-    """
+def diagram(
+    ph, new_fig=True, subplot=False, color="b", alpha=1.0, edgecolors="black", s=30, **kwargs
+):
+    """Generate a 2d figure (ph diagram) of the persistent homology of a tree."""
     # Initialization of matplotlib figure and axes.
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
 
     bounds_max = np.max(np.max(ph))
     bounds_min = np.min(np.min(ph))
-    plt.plot([bounds_min, bounds_max], [bounds_min, bounds_max], c='black')
-
-    ax.scatter(np.array(ph)[:, 0], np.array(ph)[:, 1], c=color, alpha=alpha,
-               edgecolors=edgecolors, s=s)
-
-    kwargs['title'] = kwargs.get('title', 'Persistence diagram')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'End radial distance from soma')
-    kwargs['ylabel'] = kwargs.get('ylabel', 'Start radial distance from soma')
-
-    return cm.plot_style(fig=fig, ax=ax, **kwargs)
+    plt.plot([bounds_min, bounds_max], [bounds_min, bounds_max], c="black")
 
+    ax.scatter(
+        np.array(ph)[:, 0], np.array(ph)[:, 1], c=color, alpha=alpha, edgecolors=edgecolors, s=s
+    )
+
+    all_kwargs = {
+        "title": "Persistence diagram",
+        "xlabel": "End radial distance",
+        "ylabel": "Start radial distance",
+    }
+    all_kwargs.update(kwargs)
+
+    return cm.plot_style(fig=fig, ax=ax, **all_kwargs)
+
+
+def diagram_enhanced(
+    ph,
+    new_fig=True,
+    subplot=False,
+    alpha=1.0,
+    valID=2,
+    cmap=jet_map,
+    edgecolors="black",
+    s=30,
+    **kwargs,
+):
+    """Generate a 2d figure (diagram) of the persistent homology of a enhanced tree.
 
-def diagram_enhanced(ph, new_fig=True, subplot=False, alpha=1.0, valID=2,
-                     cmap=jet_map, edgecolors='black', s=30, **kwargs):
-    """
-    Generates a 2d figure (diagram) of the persistent homology
-    of a tree enhanced by a parameter encodes in ph[valID]
+    The tree is enhanced by a parameter encodes in ph[valID].
     """
     # Initialization of matplotlib figure and axes.
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
     val_max = np.max(ph, axis=0)[valID]
 
     # Hack for colorbar creation
     Z = [[0, 0], [0, 0]]
     levels = np.linspace(0.0, val_max, 200)
     CS3 = plt.contourf(Z, levels, cmap=cmap)
 
     def sort_ph_enhanced(ph, valID):
-        """
-        Sorts barcode according to length.
-        """
-        ph_sort = [p[:valID + 1] + [np.abs(p[0] - p[1])] for p in ph]
+        """Sorts barcode according to length."""
+        ph_sort = [p[: valID + 1] + [np.abs(p[0] - p[1])] for p in ph]
         ph_sort.sort(key=lambda x: x[valID + 1])
         return ph_sort
 
     ph_sort = sort_ph_enhanced(ph, valID)
 
     bounds_max = np.max(np.max(ph_sort))
     bounds_min = np.min(np.min(ph_sort))
-    plt.plot([bounds_min, bounds_max], [bounds_min, bounds_max], c='black')
+    plt.plot([bounds_min, bounds_max], [bounds_min, bounds_max], c="black")
 
     colors = [cmap(p[valID] / val_max) for p in ph_sort]
 
-    ax.scatter(np.array(ph_sort)[:, 0], np.array(ph_sort)[:, 1],
-               c=colors, alpha=alpha, edgecolors=edgecolors, s=s)
-
-    kwargs['title'] = kwargs.get('title', 'Persistence diagram')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'End radial distance from soma')
-    kwargs['ylabel'] = kwargs.get('ylabel', 'Start radial distance from soma')
+    ax.scatter(
+        np.array(ph_sort)[:, 0],
+        np.array(ph_sort)[:, 1],
+        c=colors,
+        alpha=alpha,
+        edgecolors=edgecolors,
+        s=s,
+    )
+
+    all_kwargs = {
+        "title": "Persistence diagram",
+        "xlabel": "End radial distance",
+        "ylabel": "Start radial distance",
+    }
+    all_kwargs.update(kwargs)
 
     plt.ylim([-1, len(ph_sort)])
     plt.colorbar(CS3)
 
-    return cm.plot_style(fig=fig, ax=ax, **kwargs)
+    return cm.plot_style(fig=fig, ax=ax, **all_kwargs)
 
 
-def persistence_image(ph, new_fig=True, subplot=111, xlims=None, ylims=None,
-                      masked=False, colorbar=False, norm_factor=None, threshold=0.01,
-                      vmin=None, vmax=None, cmap=jet_map, bw_method=None, **kwargs):
-    '''Plots the gaussian kernel
-       of the ph diagram that is given.
-    '''
-    if xlims is None or xlims is None:
-        xlims, ylims = analysis.get_limits(ph, coll=False)
+def persistence_image(
+    ph,
+    new_fig=True,
+    subplot=111,
+    xlim=None,
+    ylim=None,
+    masked=False,
+    colorbar=False,
+    norm_factor=None,
+    threshold=0.01,
+    vmin=None,
+    vmax=None,
+    cmap=jet_map,
+    bw_method=None,
+    **kwargs,
+):
+    """Plot the gaussian kernel of the ph diagram that is given."""
+    if xlim is None or xlim is None:
+        xlim, ylim = analysis.get_limits(ph, coll=False)
 
     # pylint: disable=unexpected-keyword-arg
-    Zn = analysis.get_persistence_image_data(ph, norm_factor=norm_factor, bw_method=bw_method,
-                                             xlims=xlims, ylims=ylims)
+    Zn = analysis.get_persistence_image_data(
+        ph, norm_factor=norm_factor, bw_method=bw_method, xlim=xlim, ylim=ylim
+    )
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
 
     if masked:
         Zn = np.ma.masked_where((threshold > Zn), Zn)
 
-    cax = ax.imshow(np.rot90(Zn), vmin=vmin, vmax=vmax, cmap=cmap,
-                    interpolation='bilinear', extent=xlims + ylims)
+    cax = ax.imshow(
+        np.rot90(Zn),
+        vmin=vmin,
+        vmax=vmax,
+        cmap=cmap,
+        interpolation="bilinear",
+        extent=xlim + ylim,
+    )
 
     if colorbar:
         plt.colorbar(cax)
 
-    kwargs['xlim'] = xlims
-    kwargs['ylim'] = ylims
-    kwargs['title'] = kwargs.get('title', 'Persistence image')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'End radial distance from soma')
-    kwargs['ylabel'] = kwargs.get('ylabel', 'Start radial distance from soma')
-
-    return Zn, cm.plot_style(fig=fig, ax=ax, **kwargs)
+    kwargs["xlim"] = xlim
+    kwargs["ylim"] = ylim
 
+    all_kwargs = {
+        "title": "Persistence image",
+        "xlabel": "End radial distance",
+        "ylabel": "Start radial distance",
+    }
+    all_kwargs.update(kwargs)
+
+    return Zn, cm.plot_style(fig=fig, ax=ax, **all_kwargs)
+
+
+def persistence_image_diff(
+    Z1,
+    Z2,
+    new_fig=True,
+    subplot=111,
+    xlim=None,
+    ylim=None,
+    norm=True,
+    vmin=-1.0,
+    vmax=1.0,
+    cmap=jet_map,
+    **kwargs,
+):
+    """Plot the difference of 2 images from the gaussian kernel plotting function.
 
-def persistence_image_diff(Z1, Z2, new_fig=True, subplot=111, xlims=None, ylims=None,
-                           norm=True, vmin=-1., vmax=1., cmap=jet_map, **kwargs):
-    """Takes as input two images as exported from the gaussian kernel
-       plotting function, and plots their difference.
+    The difference is computed as: diff(Z1 - Z2))
     """
-    if xlims is None or xlims is None:
-        xlims, ylims = ((0, 100), (0, 100))
+    if xlim is None or xlim is None:
+        xlim, ylim = ((0, 100), (0, 100))
 
     difference = analysis.get_image_diff_data(Z1, Z2, normalized=norm)
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
-    ax.imshow(np.rot90(difference), vmin=vmin, vmax=vmax, cmap=cmap,
-              interpolation='bilinear', extent=xlims + ylims)
+    ax.imshow(
+        np.rot90(difference),
+        vmin=vmin,
+        vmax=vmax,
+        cmap=cmap,
+        interpolation="bilinear",
+        extent=xlim + ylim,
+    )
 
-    kwargs['xlim'] = xlims
-    kwargs['ylim'] = ylims
+    kwargs["xlim"] = xlim
+    kwargs["ylim"] = ylim
     return cm.plot_style(fig=fig, ax=ax, **kwargs)
 
 
-def persistence_image_add(Z2, Z1, new_fig=True, subplot=111, xlims=None, ylims=None,
-                          norm=True, vmin=0, vmax=2., cmap=jet_map, **kwargs):
-    """Takes as input two images as exported from the gaussian kernel
-       plotting function, and plots their addition.
-    """
-    if xlims is None or xlims is None:
-        xlims, ylims = ((0, 100), (0, 100))
+def persistence_image_add(
+    Z2,
+    Z1,
+    new_fig=True,
+    subplot=111,
+    xlim=None,
+    ylim=None,
+    norm=True,
+    vmin=0,
+    vmax=2.0,
+    cmap=jet_map,
+    **kwargs,
+):
+    """Plot the sum of 2 images from the gaussian kernel plotting function."""
+    if xlim is None or xlim is None:
+        xlim, ylim = ((0, 100), (0, 100))
 
     addition = analysis.get_image_add_data(Z1, Z2, normalized=norm)
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
-    ax.imshow(np.rot90(addition), vmin=vmin, vmax=vmax, cmap=cmap,
-              interpolation='bilinear', extent=xlims + ylims)
+    ax.imshow(
+        np.rot90(addition),
+        vmin=vmin,
+        vmax=vmax,
+        cmap=cmap,
+        interpolation="bilinear",
+        extent=xlim + ylim,
+    )
 
-    kwargs['xlim'] = xlims
-    kwargs['ylim'] = ylims
+    kwargs["xlim"] = xlim
+    kwargs["ylim"] = ylim
     return cm.plot_style(fig=fig, ax=ax, **kwargs)
 
 
-def persistence_image_average(ph_list, new_fig=True, subplot=111, xlims=None,
-                              ylims=None, norm_factor=1.0, vmin=None, vmax=None,
-                              cmap=jet_map, weighted=False, **kwargs):
-    """Merges a list of ph diagrams and plots their respective average image.
-    """
+def persistence_image_average(
+    ph_list,
+    new_fig=True,
+    subplot=111,
+    xlim=None,
+    ylim=None,
+    norm_factor=1.0,
+    vmin=None,
+    vmax=None,
+    cmap=jet_map,
+    weighted=False,
+    **kwargs,
+):
+    """Merge a list of ph diagrams and plot their respective average image."""
     # pylint: disable=unexpected-keyword-arg
-    av_imgs = analysis.get_average_persistence_image(ph_list, xlims=xlims, ylims=ylims,
-                                                     norm_factor=norm_factor, weighted=weighted)
-    if xlims is None or xlims is None:
-        xlims, ylims = analysis.get_limits(ph_list)
+    av_imgs = analysis.get_average_persistence_image(
+        ph_list, xlim=xlim, ylim=ylim, norm_factor=norm_factor, weighted=weighted
+    )
+    if xlim is None or xlim is None:
+        xlim, ylim = analysis.get_limits(ph_list)
 
     if vmin is None:
         vmin = np.min(av_imgs)
     if vmax is None:
         vmax = np.max(av_imgs)
 
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
-    ax.imshow(np.rot90(av_imgs), vmin=vmin, vmax=vmax, cmap=cmap,
-              interpolation='bilinear', extent=xlims + ylims)
+    ax.imshow(
+        np.rot90(av_imgs),
+        vmin=vmin,
+        vmax=vmax,
+        cmap=cmap,
+        interpolation="bilinear",
+        extent=xlim + ylim,
+    )
+
+    kwargs["xlim"] = xlim
+    kwargs["ylim"] = ylim
+
+    all_kwargs = {
+        "title": "Average persistence image",
+        "xlabel": "End radial distance",
+        "ylabel": "Start radial distance",
+    }
+    all_kwargs.update(kwargs)
+
+    return av_imgs, cm.plot_style(fig=fig, ax=ax, **all_kwargs)
+
 
-    kwargs['xlim'] = xlims
-    kwargs['ylim'] = ylims
-    kwargs['title'] = kwargs.get('title', 'Average persistence image')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'End radial distance from soma')
-    kwargs['ylabel'] = kwargs.get('ylabel', 'Start radial distance from soma')
-
-    return av_imgs, cm.plot_style(fig=fig, ax=ax, **kwargs)
-
-
-def start_length_diagram(ph, new_fig=True, subplot=False, color='b', alpha=1.0, **kwargs):
-    '''Plots the transformed ph diagram that represents lengths and starting points
-       of a component.
-    '''
+def start_length_diagram(ph, new_fig=True, subplot=False, color="b", alpha=1.0, **kwargs):
+    """Plot a transformed ph diagram that represents lengths and starting points of a component."""
     ph_transformed = transform_ph_to_length(ph)
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
 
     for p in ph_transformed:
-        ax.scatter(p[0], p[1], c=color, edgecolors='black', alpha=alpha)
+        ax.scatter(p[0], p[1], c=color, edgecolors="black", alpha=alpha)
 
-    kwargs['title'] = kwargs.get('title', 'Transformed Persistence diagram')
-    kwargs['xlabel'] = kwargs.get('xlabel', 'Start of the component')
-    kwargs['ylabel'] = kwargs.get('ylabel', 'Length of the component')
-    return cm.plot_style(fig=fig, ax=ax, **kwargs)
+    all_kwargs = {
+        "title": "Transformed persistence diagram",
+        "xlabel": "Start of the component",
+        "ylabel": "Length of the component",
+    }
+    all_kwargs.update(kwargs)
+    return cm.plot_style(fig=fig, ax=ax, **all_kwargs)
 
 
-def histogram_stepped(ph, new_fig=True, subplot=False, color='b', alpha=0.7, **kwargs):
-    '''Extracts and plots the stepped histogram of a persistent
-       homology array.
-    '''
+def histogram_stepped(ph, new_fig=True, subplot=False, color="b", alpha=0.7, **kwargs):
+    """Extract and plot the stepped histogram of a persistent homology array."""
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
     hist_data = analysis.histogram_stepped(ph)
     ax.fill_between(hist_data[0][:-1], 0, hist_data[1], color=color, alpha=alpha)
     return cm.plot_style(fig=fig, ax=ax, **kwargs)
 
 
-def histogram_stepped_population(ph_list, new_fig=True, subplot=False,
-                                 color='b', alpha=0.7, **kwargs):
-    '''Extracts and plots the stepped histogram of a list of persistence diagrams.
-       The histogram is normalized acording to the number of persistence diagrams.
-    '''
+def histogram_stepped_population(
+    ph_list, new_fig=True, subplot=False, color="b", alpha=0.7, **kwargs
+):
+    """Extract and plot the stepped histogram of a list of persistence diagrams.
+
+    The histogram is normalized according to the number of persistence diagrams.
+    """
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
     hist_data = analysis.histogram_stepped(analysis.collapse(ph_list))
     ax.fill_between(hist_data[0][:-1], 0, hist_data[1] / len(ph_list), color=color, alpha=alpha)
     return cm.plot_style(fig=fig, ax=ax, **kwargs)
 
 
-def histogram_horizontal(ph, new_fig=True, subplot=False, bins=100, color='b', alpha=0.7, **kwargs):
-    '''Extracts and plots the binned histogram of a persistent
-       homology array.
-    '''
+def histogram_horizontal(ph, new_fig=True, subplot=False, bins=100, color="b", alpha=0.7, **kwargs):
+    """Extract and plot the binned histogram of a persistent homology array."""
     fig, ax = cm.get_figure(new_fig=new_fig, subplot=subplot)
     hist_data = analysis.histogram_horizontal(ph, num_bins=bins)
     ax.fill_between(hist_data[0][:-1], 0, hist_data[1], color=color, alpha=alpha)
 
     return cm.plot_style(fig=fig, ax=ax, **kwargs)
```

