# Comparing `tmp/mentpy-0.1.0a3.tar.gz` & `tmp/mentpy-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentpy-0.1.0a3.tar", last modified: Tue Apr 25 08:51:38 2023, max compression
+gzip compressed data, was "mentpy-0.1.0a4.tar", last modified: Fri Apr 28 10:01:58 2023, max compression
```

## Comparing `mentpy-0.1.0a3.tar` & `mentpy-0.1.0a4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.460457 mentpy-0.1.0a3/
--rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a3/LICENSE
--rw-r--r--   0 luismantilla   (501) staff       (20)     3373 2023-04-25 08:51:38.460282 mentpy-0.1.0a3/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     3093 2023-04-08 10:02:59.000000 mentpy-0.1.0a3/README.md
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.444218 mentpy-0.1.0a3/mentpy/
--rw-r--r--   0 luismantilla   (501) staff       (20)      283 2023-04-16 02:10:35.000000 mentpy-0.1.0a3/mentpy/__init__.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.446183 mentpy-0.1.0a3/mentpy/gradients/
--rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/gradients/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2016 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/gradients/finite_difference.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.448140 mentpy-0.1.0a3/mentpy/mbqc/
--rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a3/mentpy/mbqc/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    16348 2023-04-16 05:41:03.000000 mentpy-0.1.0a3/mentpy/mbqc/flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    25108 2023-04-21 10:07:34.000000 mentpy-0.1.0a3/mentpy/mbqc/mbqcircuit.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.449951 mentpy-0.1.0a3/mentpy/mbqc/states/
--rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-04-16 02:07:17.000000 mentpy-0.1.0a3/mentpy/mbqc/states/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      163 2023-04-15 11:17:22.000000 mentpy-0.1.0a3/mentpy/mbqc/states/aklt.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      195 2023-04-15 11:17:22.000000 mentpy-0.1.0a3/mentpy/mbqc/states/cluster.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a3/mentpy/mbqc/states/graphstate.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     7359 2023-04-18 08:22:14.000000 mentpy-0.1.0a3/mentpy/mbqc/templates.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.450531 mentpy-0.1.0a3/mentpy/noise/
--rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/noise/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/noise/base_noise.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.452204 mentpy-0.1.0a3/mentpy/operators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      236 2023-04-21 07:24:47.000000 mentpy-0.1.0a3/mentpy/operators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2822 2023-04-21 09:50:33.000000 mentpy-0.1.0a3/mentpy/operators/controlled_ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1567 2023-04-16 01:27:43.000000 mentpy-0.1.0a3/mentpy/operators/gates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     7820 2023-04-21 10:14:40.000000 mentpy-0.1.0a3/mentpy/operators/ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5354 2023-04-15 10:49:22.000000 mentpy-0.1.0a3/mentpy/operators/pauliop.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.453816 mentpy-0.1.0a3/mentpy/optimizers/
--rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a3/mentpy/optimizers/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3054 2023-03-22 20:56:41.000000 mentpy-0.1.0a3/mentpy/optimizers/adam.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/optimizers/base_optimizer.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/optimizers/bp_tools.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3121 2023-04-25 08:49:44.000000 mentpy-0.1.0a3/mentpy/optimizers/rcd.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-04-15 23:00:30.000000 mentpy-0.1.0a3/mentpy/optimizers/sgd.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.456594 mentpy-0.1.0a3/mentpy/simulators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a3/mentpy/simulators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2143 2023-04-18 08:22:14.000000 mentpy-0.1.0a3/mentpy/simulators/base_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a3/mentpy/simulators/cirq_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    13040 2023-04-21 10:14:40.000000 mentpy-0.1.0a3/mentpy/simulators/np_simulator_dm.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    14376 2023-04-19 21:51:28.000000 mentpy-0.1.0a3/mentpy/simulators/np_simulator_sv.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2668 2023-04-18 19:39:18.000000 mentpy-0.1.0a3/mentpy/simulators/pattern_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5854 2023-04-21 09:50:33.000000 mentpy-0.1.0a3/mentpy/simulators/pennylane_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1255 2023-04-21 09:50:33.000000 mentpy-0.1.0a3/mentpy/simulators/qiskit_simulators.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.458685 mentpy-0.1.0a3/mentpy/utils/
--rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-04-16 02:10:19.000000 mentpy-0.1.0a3/mentpy/utils/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     6674 2023-04-16 02:23:18.000000 mentpy-0.1.0a3/mentpy/utils/expressivity.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a3/mentpy/utils/flow_space.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a3/mentpy/utils/generate_data.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/utils/lc_equivalence.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3313 2023-04-16 01:44:39.000000 mentpy-0.1.0a3/mentpy/utils/lie_algebra.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.445427 mentpy-0.1.0a3/mentpy.egg-info/
--rw-r--r--   0 luismantilla   (501) staff       (20)     3373 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     1409 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/SOURCES.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/dependency_links.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/requires.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/top_level.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-04-25 08:51:38.460516 mentpy-0.1.0a3/setup.cfg
--rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-04-21 10:24:58.000000 mentpy-0.1.0a3/setup.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.459863 mentpy-0.1.0a3/tests/
--rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a3/tests/test_flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a3/tests/test_graph_state.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a3/tests/test_mbqc_templates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      999 2023-04-19 21:51:31.000000 mentpy-0.1.0a3/tests/test_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.053017 mentpy-0.1.0a4/
+-rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a4/LICENSE
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3373 2023-04-28 10:01:58.052776 mentpy-0.1.0a4/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3093 2023-04-08 10:02:59.000000 mentpy-0.1.0a4/README.md
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.035236 mentpy-0.1.0a4/mentpy/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      283 2023-04-16 02:10:35.000000 mentpy-0.1.0a4/mentpy/__init__.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.037449 mentpy-0.1.0a4/mentpy/gradients/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/gradients/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2014 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/gradients/finite_difference.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.038659 mentpy-0.1.0a4/mentpy/mbqc/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a4/mentpy/mbqc/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    16348 2023-04-16 05:41:03.000000 mentpy-0.1.0a4/mentpy/mbqc/flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    25586 2023-04-28 04:28:02.000000 mentpy-0.1.0a4/mentpy/mbqc/mbqcircuit.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.039278 mentpy-0.1.0a4/mentpy/mbqc/states/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-04-16 02:07:17.000000 mentpy-0.1.0a4/mentpy/mbqc/states/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      163 2023-04-15 11:17:22.000000 mentpy-0.1.0a4/mentpy/mbqc/states/aklt.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      195 2023-04-15 11:17:22.000000 mentpy-0.1.0a4/mentpy/mbqc/states/cluster.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a4/mentpy/mbqc/states/graphstate.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     7358 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/mbqc/templates.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.039866 mentpy-0.1.0a4/mentpy/noise/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/noise/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/noise/base_noise.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.041726 mentpy-0.1.0a4/mentpy/operators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      236 2023-04-21 07:24:47.000000 mentpy-0.1.0a4/mentpy/operators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2822 2023-04-21 09:50:33.000000 mentpy-0.1.0a4/mentpy/operators/controlled_ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1567 2023-04-16 01:27:43.000000 mentpy-0.1.0a4/mentpy/operators/gates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     7820 2023-04-21 10:14:40.000000 mentpy-0.1.0a4/mentpy/operators/ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5392 2023-04-28 08:07:49.000000 mentpy-0.1.0a4/mentpy/operators/pauliop.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.045479 mentpy-0.1.0a4/mentpy/optimizers/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a4/mentpy/optimizers/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3054 2023-03-22 20:56:41.000000 mentpy-0.1.0a4/mentpy/optimizers/adam.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/optimizers/base_optimizer.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/optimizers/bp_tools.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3101 2023-04-25 09:08:43.000000 mentpy-0.1.0a4/mentpy/optimizers/rcd.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-04-15 23:00:30.000000 mentpy-0.1.0a4/mentpy/optimizers/sgd.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.047979 mentpy-0.1.0a4/mentpy/simulators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a4/mentpy/simulators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2143 2023-04-18 08:22:14.000000 mentpy-0.1.0a4/mentpy/simulators/base_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a4/mentpy/simulators/cirq_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    13039 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/simulators/np_simulator_dm.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    14384 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/simulators/np_simulator_sv.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2688 2023-04-28 03:47:29.000000 mentpy-0.1.0a4/mentpy/simulators/pattern_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5853 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/simulators/pennylane_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1254 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/simulators/qiskit_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.048967 mentpy-0.1.0a4/mentpy/utils/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-04-16 02:10:19.000000 mentpy-0.1.0a4/mentpy/utils/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     6673 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/utils/expressivity.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a4/mentpy/utils/flow_space.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a4/mentpy/utils/generate_data.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/utils/lc_equivalence.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5172 2023-04-28 08:24:36.000000 mentpy-0.1.0a4/mentpy/utils/lie_algebra.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.036184 mentpy-0.1.0a4/mentpy.egg-info/
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3373 2023-04-28 10:01:57.000000 mentpy-0.1.0a4/mentpy.egg-info/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1409 2023-04-28 10:01:58.000000 mentpy-0.1.0a4/mentpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-04-28 10:01:57.000000 mentpy-0.1.0a4/mentpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-04-28 10:01:57.000000 mentpy-0.1.0a4/mentpy.egg-info/requires.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-04-28 10:01:57.000000 mentpy-0.1.0a4/mentpy.egg-info/top_level.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-04-28 10:01:58.053091 mentpy-0.1.0a4/setup.cfg
+-rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-04-28 10:00:53.000000 mentpy-0.1.0a4/setup.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.051991 mentpy-0.1.0a4/tests/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a4/tests/test_flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a4/tests/test_graph_state.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a4/tests/test_mbqc_templates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      997 2023-04-28 03:46:02.000000 mentpy-0.1.0a4/tests/test_simulators.py
```

### Comparing `mentpy-0.1.0a3/LICENSE` & `mentpy-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/PKG-INFO` & `mentpy-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a3 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a4 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
 Content-Type: text/markdown License-File: LICENSE :warning: **This library is
 under development.**
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
```

### Comparing `mentpy-0.1.0a3/README.md` & `mentpy-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/gradients/finite_difference.py` & `mentpy-0.1.0a4/mentpy/gradients/finite_difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 
 
 def estimate_gradient(f, x, h=1e-5, type="central"):
-
     if type not in ["central", "forward", "backward"]:
         raise UserWarning(
             f"Expected type to be 'central', 'forward', or 'backward' but {type} was given"
         )
 
     grad = np.zeros(len(x))
     for i in range(len(x)):
@@ -18,15 +17,14 @@
             grad[i] = (f(x + h * np.eye(len(x))[i]) - f(x)) / h
         elif type == "backward":
             grad[i] = (f(x) - f(x - h * np.eye(len(x))[i])) / h
     return grad
 
 
 def estimate_hessian(f, x, h=1e-5, type="central"):
-
     if type not in ["central", "forward", "backward"]:
         raise UserWarning(
             f"Expected type to be 'central', 'forward', or 'backward' but {type} was given"
         )
 
     hess = np.zeros((len(x), len(x)))
     for i in range(len(x)):
```

### Comparing `mentpy-0.1.0a3/mentpy/mbqc/flow.py` & `mentpy-0.1.0a4/mentpy/mbqc/flow.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/mbqc/mbqcircuit.py` & `mentpy-0.1.0a4/mentpy/mbqc/mbqcircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional, List, Tuple, Callable, Union, Any, Dict
 
 import numpy as np
 import scipy as scp
 import networkx as nx
 import matplotlib.pyplot as plt
 
-from mentpy.operators import Ment, ControlMent
+from mentpy.operators import Ment, ControlMent, PauliOp
 from mentpy.mbqc.states.graphstate import GraphState
 from mentpy.mbqc.flow import find_gflow, find_cflow, find_flow, check_if_flow
 
 __all__ = ["MBQCircuit", "draw", "merge", "hstack", "vstack"]
 
 
 class MBQCircuit:
@@ -298,15 +298,14 @@
 
     def _update_attributes(self) -> None:
         trainable_nodes = []
         controlled_nodes = []
         planes = {}
         for nodei, menti in self._measurements.items():
             if menti is not None:
-
                 if isinstance(menti, ControlMent):
                     controlled_nodes.append(nodei)
 
                 if menti.angle is None:
                     trainable_nodes.append(nodei)
 
                 planes[nodei] = menti.plane
@@ -315,15 +314,14 @@
             else:
                 planes[nodei] = ""
         self._trainable_nodes = trainable_nodes
         self._controlled_nodes = controlled_nodes
         self._planes = planes
 
     def _update_attributes_key(self, key) -> None:
-
         menti = self._measurements[key]
         if menti is not None:
             if menti.angle is None and key not in self._trainable_nodes:
                 self._trainable_nodes.append(key)
             elif menti.angle is not None and key in self._trainable_nodes:
                 self._trainable_nodes.remove(key)
             self._planes[key] = menti.plane
@@ -387,15 +385,15 @@
     return True
 
 
 def merge(state1: MBQCircuit, state2: MBQCircuit, along=[]) -> MBQCircuit:
     """Merge two MBQC circuits into a larger MBQC circuit. This is, the input and
     output of the new MBQC circuit will depend on the concat_indices."""
 
-    for (i, j) in along:
+    for i, j in along:
         if i not in state1.output_nodes or j not in state2.input_nodes:
             raise ValueError(f"Cannot merge states at indices {i} and {j}")
 
     graph = nx.disjoint_union(state1.graph, state2.graph)
     along1, along2 = zip(*along)
 
     input_nodes = state1.input_nodes + [
@@ -419,15 +417,15 @@
     ]
 
     measurements = dict(state1.measurements)
     measurements.update(
         {i + len(state1.graph): ment for i, ment in state2.measurements.items()}
     )
 
-    for (i, j) in along:
+    for i, j in along:
         graph.add_edge(i, j + len(state1.graph))
         graph = nx.contracted_edge(graph, (j + len(state1.graph), i), self_loops=False)
         del measurements[i]
 
     return MBQCircuit(graph, input_nodes, output_nodes, measurements=measurements)
 
 
@@ -529,15 +527,15 @@
     output_nodes = [nodes2.index(j) + len(nodes1) for j in state2.output_nodes]
 
     measurements = {nodes1.index(i): ment for i, ment in state1.measurements.items()}
     measurements.update(
         {nodes2.index(i) + len(nodes1): ment for i, ment in state2.measurements.items()}
     )
 
-    for (i, j) in zip(state1.output_nodes, state2.input_nodes):
+    for i, j in zip(state1.output_nodes, state2.input_nodes):
         graph.add_edge(i, j + len(state1.graph))
         graph = nx.contracted_edge(graph, (j + len(state1.graph), i), self_loops=False)
         del measurements[i]
 
     # TODO: Compute flow and partial order
     return MBQCircuit(graph, input_nodes, output_nodes, measurements=measurements)
 
@@ -573,20 +571,26 @@
         "node_size": 500,
         "edge_color": "grey",
         "with_labels": True,
         "label": "indices",
         "transparent": True,
         "figsize": (8, 3),
         "show_controls": True,
+        "pauliop": None
     }
 
     options.update(kwargs)
 
     show_controls = options.pop("show_controls")
 
+    pauliop = options.pop("pauliop")
+
+    if pauliop is not None:
+        options["label"] = "pauliop"
+
     transp = options.pop("transparent")
     fig, ax = plt.subplots(figsize=options.pop("figsize"))
 
     if transp:
         fig.patch.set_alpha(0)
         ax.patch.set_alpha(0)
 
@@ -671,15 +675,23 @@
                         labels[node] = round(state.measurements[node].angle, 3)
                     else:
                         labels[node] = r"$\theta$"
                 else:
                     labels[node] = ""
 
             options["labels"] = labels
-
+        
+        elif options["label"] == "pauliop":
+            if len(pauliop) != 1:
+                raise ValueError("pauliop must be a single Pauli operator")
+            labels = {}
+            for ind, node in enumerate(state.graph.nodes()):
+                labels[node] = pauliop.txt[ind]
+            options["labels"] = labels
+            
         else:
             raise ValueError(
                 "label must be either 'index' or 'plane', not {}".format(
                     options["label"]
                 )
             )
 
@@ -707,7 +719,9 @@
     """Return digraph with flow (but does not have all CZ edges!)"""
     g = state.graph
     gflow = nx.DiGraph()
     gflow.add_nodes_from(g.nodes())
     for node in state.outputc:
         gflow.add_edge(node, state.flow(node))
     return gflow
+
+
```

### Comparing `mentpy-0.1.0a3/mentpy/mbqc/states/graphstate.py` & `mentpy-0.1.0a4/mentpy/mbqc/states/graphstate.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/mbqc/templates.py` & `mentpy-0.1.0a4/mentpy/mbqc/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,14 @@
         "restrict-trainable": True,
     }
 
     SIZE_TRIANGLE = 5
 
     big_graph = None
     for wire in range(n_wires):
-
         g = many_wires([SIZE_TRIANGLE] * n_wires)
         if options["restrict-trainable"]:
             g.trainable_nodes = list(
                 set(g.trainable_nodes) - set([i - 1 for i in g.output_nodes])
             )
             # TODO! Make soemthing with this...
```

### Comparing `mentpy-0.1.0a3/mentpy/operators/controlled_ment.py` & `mentpy-0.1.0a4/mentpy/operators/controlled_ment.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/operators/gates.py` & `mentpy-0.1.0a4/mentpy/operators/gates.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/operators/ment.py` & `mentpy-0.1.0a4/mentpy/operators/ment.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/operators/pauliop.py` & `mentpy-0.1.0a4/mentpy/operators/pauliop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from typing import Union, List
 import galois
+import copy
 
 __all__ = ["PauliOp"]
 
 GF = galois.GF(2)
 
 
 class PauliOp:
@@ -78,31 +79,34 @@
             raise ValueError(
                 "PauliOp must be initialized with a string or a numpy array"
             )
 
         if self.mat.shape[0] == 1:
             self._array = [self]
         else:
-            self._array = [PauliOp(op) for op in self.txt.split("\n")]
+            self._array = [PauliOp(op) for op in self.txt.split("\n") if op != ""]
 
     def __repr__(self):
         return self.txt
 
     def __len__(self):
         return self.mat.shape[0]
 
     def __getitem__(self, key):
         paulis = self._array[key]
         if isinstance(key, slice):
             return PauliOp(";".join([pauli.txt for pauli in paulis]))
         return paulis
 
     def __contains__(self, item: "PauliOp"):
-        # check item.mat rows are in self.mat rows
-        return np.prod((self.mat[:, None] == item.mat).all(axis=2).any(axis=0))
+        
+        for row in item.mat:
+            if not np.any((self.mat == row).all(axis=1)):
+                return False
+        return True
 
     def _mat_to_txt(self, op):
         n_qubits = op.shape[1] // 2
         txt = ""
         for i in range(op.shape[0]):
             for j in range(op.shape[1] // 2):
                 if op[i, j] == 1 and op[i, j + n_qubits] == 0:
```

### Comparing `mentpy-0.1.0a3/mentpy/optimizers/adam.py` & `mentpy-0.1.0a4/mentpy/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/optimizers/base_optimizer.py` & `mentpy-0.1.0a4/mentpy/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/optimizers/rcd.py` & `mentpy-0.1.0a4/mentpy/optimizers/rcd.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Examples
     --------
     Create a random coordinate descent optimizer
 
     .. ipython:: python
 
-        opt = mp.optimizers.RandomCoordinateDescentOptimizer()
+        opt = mp.optimizers.RCDOptimizer()
         print(opt)
 
     Group
     -----
     optimizers
     """
```

### Comparing `mentpy-0.1.0a3/mentpy/optimizers/sgd.py` & `mentpy-0.1.0a4/mentpy/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/simulators/base_simulator.py` & `mentpy-0.1.0a4/mentpy/simulators/base_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/simulators/cirq_simulator.py` & `mentpy-0.1.0a4/mentpy/simulators/cirq_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/simulators/np_simulator_dm.py` & `mentpy-0.1.0a4/mentpy/simulators/np_simulator_dm.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 
     def current_number_simulated_nodes(self) -> int:
         """Returns the number of nodes that are currently simulated."""
         n = self.window_size
         return min(n, len(self.mbqcircuit) - self.current_measurement)
 
     def measure(self, angle: float) -> Tuple:
-
         if self.current_measurement >= len(self.schedule_measure):
             raise ValueError("No more measurements to be done.")
 
         current_ment = self.mbqcircuit[
             self.schedule_measure[self.current_measurement]
         ].copy()
         self.qstate, outcome = self.measure_ment(
```

### Comparing `mentpy-0.1.0a3/mentpy/simulators/np_simulator_sv.py` & `mentpy-0.1.0a4/mentpy/simulators/np_simulator_sv.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 
     def current_number_simulated_nodes(self) -> int:
         """Returns the number of nodes that are currently simulated."""
         n = self.window_size
         return min(n, len(self.mbqcircuit) - self.current_measurement)
 
     def measure(self, angle: float) -> Tuple:
-
         if self.current_measurement >= len(self.schedule_measure):
             raise ValueError("No more measurements to be done.")
 
         current_ment = self.mbqcircuit[
             self.schedule_measure[self.current_measurement]
         ].copy()
         self.qstate, outcome = self.measure_ment(
@@ -255,15 +254,16 @@
             else:
                 op2 = np.kron(op2, np.eye(2))
                 op3 = np.kron(op3, np.eye(2))
         return op1 + op2 + op3 + op4
 
     def partial_trace_pure_state(self, psi, indices):
         """Partial trace of a pure state over some indices. It is asumed that the indices
-        over which the trace is taken are unentangled with the rest of the rest of the system."""
+        over which the trace is taken are unentangled with the rest of the rest of the system.
+        """
         n = int(np.log2(len(psi)))
         indices_to_keep = [x for x in range(n) if x not in indices]
         preserved_dim = 2 ** len(indices_to_keep)
 
         # Reshape the state vector into a tensor with shape (2, 2, ..., 2)
         reshaped_psi = psi.reshape([2] * n)
```

### Comparing `mentpy-0.1.0a3/mentpy/simulators/pennylane_simulator.py` & `mentpy-0.1.0a4/mentpy/simulators/pennylane_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
     def measure(self, angle: float, plane: str = "XY"):
         raise NotImplementedError
 
     def run(
         self, angles: List[float], planes: Union[List[str], str] = "XY", **kwargs
     ) -> Tuple[List[int], np.ndarray]:
-
         if len(angles) != len(self.mbqcircuit.trainable_nodes):
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
         # TODO: Implement this
         if planes != "XY":
```

### Comparing `mentpy-0.1.0a3/mentpy/simulators/qiskit_simulators.py` & `mentpy-0.1.0a4/mentpy/simulators/qiskit_simulators.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
     Group
     -----
     simulators
     """
 
     def __init__(self, mbqcircuit: MBQCircuit, input_state: np.ndarray = None) -> None:
-
         super().__init__(mbqcircuit, input_state)
 
         raise NotImplementedError
 
     def measure(self, angle: float, plane: str = "XY", **kwargs):
         raise NotImplementedError
```

### Comparing `mentpy-0.1.0a3/mentpy/utils/expressivity.py` & `mentpy-0.1.0a4/mentpy/utils/expressivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,14 @@
         curr_g = deg_graph.nodes[node]["mbqc_circuit"].graph
         if not independent_groups:
             independent_groups[0] = [curr_g]
             independent_groups_ind[0] = [node]
         else:
             added = False
             for k, g in independent_groups.items():
-
                 if are_lc_equivalent(g[0], curr_g)[0]:
                     added = True
                     independent_groups[k].append(curr_g)
                     independent_groups_ind[k].append(node)
                     if sanity_check:
                         for n in g:
                             if not are_lc_equivalent(n, curr_g)[0]:
```

### Comparing `mentpy-0.1.0a3/mentpy/utils/flow_space.py` & `mentpy-0.1.0a4/mentpy/utils/flow_space.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/utils/generate_data.py` & `mentpy-0.1.0a4/mentpy/utils/generate_data.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy/utils/lc_equivalence.py` & `mentpy-0.1.0a4/mentpy/utils/lc_equivalence.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/mentpy.egg-info/PKG-INFO` & `mentpy-0.1.0a4/mentpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a3 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a4 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
 Content-Type: text/markdown License-File: LICENSE :warning: **This library is
 under development.**
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
```

### Comparing `mentpy-0.1.0a3/mentpy.egg-info/SOURCES.txt` & `mentpy-0.1.0a4/mentpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/setup.py` & `mentpy-0.1.0a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.1.0a3"
+version = "0.1.0a4"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="mentpy",
     version=version,
```

### Comparing `mentpy-0.1.0a3/tests/test_mbqc_templates.py` & `mentpy-0.1.0a4/tests/test_mbqc_templates.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a3/tests/test_simulators.py` & `mentpy-0.1.0a4/tests/test_simulators.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @pytest.mark.parametrize("simulator", ["numpy-dm", "numpy-sv", "pennylane"])
 class TestSimulators(object):
     def test_teleportation(cls, simulator):
         """Test teleportation in one wire."""
         for i in range(1, 5):
             gs = mp.templates.linear_cluster(2 * i + 1)
             sts = mp.utils.generate_haar_random_states(1, 5)
-            ps = mp.simulators.PatternSimulator(gs, simulator=simulator)
+            ps = mp.simulators.PatternSimulator(gs, backend=simulator)
             for st in sts:
                 ps.reset(input_state=st)
                 assert (
                     len(ps.mbqcircuit.trainable_nodes) == 2 * i
                 ), f"{ps.mbqcircuit.trainable_nodes} != {2*i}, {simulator} failed"
                 output_dm = ps([0] * (2 * i))
                 expected_dm = np.outer(st, st.conj().T)
```

