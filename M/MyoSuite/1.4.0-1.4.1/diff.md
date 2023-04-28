# Comparing `tmp/MyoSuite-1.4.0.tar.gz` & `tmp/MyoSuite-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyoSuite-1.4.0.tar", last modified: Thu Apr 27 17:49:48 2023, max compression
+gzip compressed data, was "MyoSuite-1.4.1.tar", last modified: Fri Apr 28 17:17:32 2023, max compression
```

## Comparing `MyoSuite-1.4.0.tar` & `MyoSuite-1.4.1.tar`

### file list

```diff
@@ -1,50 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:48.928453 MyoSuite-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:48.924453 MyoSuite-1.4.0/MyoSuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-27 17:49:48.000000 MyoSuite-1.4.0/MyoSuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-27 17:49:48.000000 MyoSuite-1.4.0/MyoSuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:49:48.000000 MyoSuite-1.4.0/MyoSuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 17:49:48.000000 MyoSuite-1.4.0/MyoSuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 17:49:48.000000 MyoSuite-1.4.0/MyoSuite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-27 17:49:48.924453 MyoSuite-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:48.924453 MyoSuite-1.4.0/myosuite/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:48.924453 MyoSuite-1.4.0/myosuite/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26895 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/env_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/env_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:48.924453 MyoSuite-1.4.0/myosuite/envs/myo/
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/base_v0.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/key_turn_v0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:48.924453 MyoSuite-1.4.0/myosuite/envs/myo/myochallenge/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/myochallenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/myochallenge/baoding_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/myochallenge/reorient_v0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/obj_hold_v0.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/pen_v0.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/pose_v0.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/envs/myo/reach_v0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:48.924453 MyoSuite-1.4.0/myosuite/robot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/robot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38019 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/robot/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:48.924453 MyoSuite-1.4.0/myosuite/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/examine_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/examine_rollout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/examine_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/inverse_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/min_jerk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/obj_vec_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/paths_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/quat_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/render_cams.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/vector_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/viz_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/myosuite/utils/xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:49:48.928453 MyoSuite-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-27 17:49:42.000000 MyoSuite-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.533197 MyoSuite-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.529198 MyoSuite-1.4.1/MyoSuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-28 17:17:32.000000 MyoSuite-1.4.1/MyoSuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-28 17:17:32.000000 MyoSuite-1.4.1/MyoSuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:17:32.000000 MyoSuite-1.4.1/MyoSuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 17:17:32.000000 MyoSuite-1.4.1/MyoSuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 17:17:32.000000 MyoSuite-1.4.1/MyoSuite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-28 17:17:32.533197 MyoSuite-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.529198 MyoSuite-1.4.1/myosuite/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.529198 MyoSuite-1.4.1/myosuite/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26895 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/env_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/env_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.529198 MyoSuite-1.4.1/myosuite/envs/myo/
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.525197 MyoSuite-1.4.1/myosuite/envs/myo/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.529198 MyoSuite-1.4.1/myosuite/envs/myo/assets/arm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/assets/arm/myo_elbow_1dof6muscles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/assets/arm/myo_elbow_1dof6muscles_1dofexo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.529198 MyoSuite-1.4.1/myosuite/envs/myo/assets/hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/assets/hand/myo_hand_baoding.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/assets/hand/myo_hand_die.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/assets/hand/myo_hand_hold.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/assets/hand/myo_hand_keyturn.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/assets/hand/myo_hand_pen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/assets/hand/myo_hand_pose.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/base_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/key_turn_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.533197 MyoSuite-1.4.1/myosuite/envs/myo/myochallenge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/myochallenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/myochallenge/baoding_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/myochallenge/reorient_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/obj_hold_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/pen_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/pose_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/envs/myo/reach_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.533197 MyoSuite-1.4.1/myosuite/robot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/robot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38019 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/robot/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.533197 MyoSuite-1.4.1/myosuite/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/tests/test_myo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:32.533197 MyoSuite-1.4.1/myosuite/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/examine_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/examine_rollout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/examine_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/inverse_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/min_jerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/obj_vec_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/paths_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/quat_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/render_cams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/vector_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/viz_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/myosuite/utils/xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 17:17:32.533197 MyoSuite-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-28 17:17:29.000000 MyoSuite-1.4.1/setup.py
```

### Comparing `MyoSuite-1.4.0/LICENSE` & `MyoSuite-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/MyoSuite.egg-info/PKG-INFO` & `MyoSuite-1.4.1/MyoSuite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyoSuite
-Version: 1.4.0
+Version: 1.4.1
 Summary: Musculoskeletal environments simulated in MuJoCo
 Home-page: UNKNOWN
 Author: MyoSuite Authors - Vikash Kumar (Meta AI), Vittorio Caggiano (Meta AI), Huawei Wang (University of Twente), Guillaume Durandau (University of Twente), Massimo Sartori (University of Twente)
 Author-email: vikashplus@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `MyoSuite-1.4.0/PKG-INFO` & `MyoSuite-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyoSuite
-Version: 1.4.0
+Version: 1.4.1
 Summary: Musculoskeletal environments simulated in MuJoCo
 Home-page: UNKNOWN
 Author: MyoSuite Authors - Vikash Kumar (Meta AI), Vittorio Caggiano (Meta AI), Huawei Wang (University of Twente), Guillaume Durandau (University of Twente), Massimo Sartori (University of Twente)
 Author-email: vikashplus@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `MyoSuite-1.4.0/README.md` & `MyoSuite-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/env_base.py` & `MyoSuite-1.4.1/myosuite/envs/env_base.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/env_variants.py` & `MyoSuite-1.4.1/myosuite/envs/env_variants.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/__init__.py` & `MyoSuite-1.4.1/myosuite/envs/myo/__init__.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/base_v0.py` & `MyoSuite-1.4.1/myosuite/envs/myo/base_v0.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/key_turn_v0.py` & `MyoSuite-1.4.1/myosuite/envs/myo/key_turn_v0.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/myochallenge/__init__.py` & `MyoSuite-1.4.1/myosuite/envs/myo/myochallenge/__init__.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/myochallenge/baoding_v1.py` & `MyoSuite-1.4.1/myosuite/envs/myo/myochallenge/baoding_v1.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/myochallenge/reorient_v0.py` & `MyoSuite-1.4.1/myosuite/envs/myo/myochallenge/reorient_v0.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/obj_hold_v0.py` & `MyoSuite-1.4.1/myosuite/envs/myo/obj_hold_v0.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/pen_v0.py` & `MyoSuite-1.4.1/myosuite/envs/myo/pen_v0.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/pose_v0.py` & `MyoSuite-1.4.1/myosuite/envs/myo/pose_v0.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/envs/myo/reach_v0.py` & `MyoSuite-1.4.1/myosuite/envs/myo/reach_v0.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/robot/robot.py` & `MyoSuite-1.4.1/myosuite/robot/robot.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/dict_utils.py` & `MyoSuite-1.4.1/myosuite/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/examine_env.py` & `MyoSuite-1.4.1/myosuite/utils/examine_env.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/examine_rollout.py` & `MyoSuite-1.4.1/myosuite/utils/examine_rollout.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/examine_sim.py` & `MyoSuite-1.4.1/myosuite/utils/examine_sim.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/inverse_kinematics.py` & `MyoSuite-1.4.1/myosuite/utils/inverse_kinematics.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/min_jerk.py` & `MyoSuite-1.4.1/myosuite/utils/min_jerk.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/obj_vec_dict.py` & `MyoSuite-1.4.1/myosuite/utils/obj_vec_dict.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/paths_utils.py` & `MyoSuite-1.4.1/myosuite/utils/paths_utils.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/quat_math.py` & `MyoSuite-1.4.1/myosuite/utils/quat_math.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/render_cams.py` & `MyoSuite-1.4.1/myosuite/utils/render_cams.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/tensor_utils.py` & `MyoSuite-1.4.1/myosuite/utils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/vector_math.py` & `MyoSuite-1.4.1/myosuite/utils/vector_math.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/viz_paths.py` & `MyoSuite-1.4.1/myosuite/utils/viz_paths.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/myosuite/utils/xml_utils.py` & `MyoSuite-1.4.1/myosuite/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `MyoSuite-1.4.0/setup.py` & `MyoSuite-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             if filename.endswith(ends_with):
                 paths.append(os.path.join('..', path, filename))
     return paths
 
-mjc_models_files = package_files('myosuite/envs/myo/assets/','.mjb')
+mjc_models_files = package_files('myosuite/envs/myo/assets/','.xml')
 
 
 if __name__ == "__main__":
     setup(
         name="MyoSuite",
         version=get_version("myosuite/__init__.py"),
         author='MyoSuite Authors - Vikash Kumar (Meta AI), Vittorio Caggiano (Meta AI), Huawei Wang (University of Twente), Guillaume Durandau (University of Twente), Massimo Sartori (University of Twente)',
@@ -56,11 +56,11 @@
         classifiers=[
             "Programming Language :: Python :: 3.7",
             "License :: OSI Approved :: Apache Software License",
             "Topic :: Scientific/Engineering :: Artificial Intelligence ",
             "Operating System :: OS Independent",
         ],
         package_data={'': mjc_models_files},
-        packages=find_packages(exclude=("myosuite.tests", "myosuite.agents")),
+        packages=find_packages(exclude=("myosuite.agents")),
         python_requires=">=3.7.1",
         install_requires=fetch_requirements(),
     )
```

