# Comparing `tmp/gym_collision_avoidance-0.0.2.post2.tar.gz` & `tmp/gym_collision_avoidance-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/mfe/code/gym-collision-avoidance/dist/tmp06ipju27/gym_collision_avoidance-0.0.2.post2.tar", last modified: Sat Feb  6 21:56:01 2021, max compression
+gzip compressed data, was "gym_collision_avoidance-0.0.3.tar", last modified: Fri Apr 28 18:12:29 2023, max compression
```

## Comparing `gym_collision_avoidance-0.0.2.post2.tar` & `gym_collision_avoidance-0.0.3.tar`

### file list

```diff
@@ -1,116 +1,132 @@
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/
--rw-r--r--   0 mfe        (501) staff       (20)     3117 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/PKG-INFO
--rw-r--r--   0 mfe        (501) staff       (20)       94 2021-01-11 21:58:45.000000 gym_collision_avoidance-0.0.2.post2/MANIFEST.in
--rw-r--r--   0 mfe        (501) staff       (20)     2329 2021-02-01 00:06:06.000000 gym_collision_avoidance-0.0.2.post2/README.md
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/__init__.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/
--rw-r--r--   0 mfe        (501) staff       (20)     3880 2021-02-06 21:51:40.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/run_full_test_suite.py
--rw-r--r--   0 mfe        (501) staff       (20)     4437 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/process_full_test_suite_pickles.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)    21778 2021-02-06 21:50:33.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/env_utils.py
--rw-r--r--   0 mfe        (501) staff       (20)     2057 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/run_cadrl_formations.py
--rw-r--r--   0 mfe        (501) staff       (20)     1912 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/example.py
--rw-r--r--   0 mfe        (501) staff       (20)     5770 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/run_trajectory_dataset_creator.py
--rw-r--r--   0 mfe        (501) staff       (20)     2190 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/collect_regression_dataset.py
--rw-r--r--   0 mfe        (501) staff       (20)      234 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/__init__.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/
--rw-r--r--   0 mfe        (501) staff       (20)      831 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/Sensor.py
--rw-r--r--   0 mfe        (501) staff       (20)     5733 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/LaserScanSensor.py
--rw-r--r--   0 mfe        (501) staff       (20)     7677 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/OtherAgentsStatesSensor.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)     4900 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/OccupancyGridSensor.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/
--rw-r--r--   0 mfe        (501) staff       (20)     2088 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/UnicycleDynamics.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)     1858 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/UnicycleDynamicsMaxTurnRate.py
--rw-r--r--   0 mfe        (501) staff       (20)      466 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/ExternalDynamics.py
--rw-r--r--   0 mfe        (501) staff       (20)     1711 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/Dynamics.py
--rw-r--r--   0 mfe        (501) staff       (20)     6772 2021-02-06 21:37:41.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/vec_env.py
--rw-r--r--   0 mfe        (501) staff       (20)    13585 2021-02-06 20:06:26.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/config.py
--rw-r--r--   0 mfe        (501) staff       (20)     6976 2021-02-01 00:06:06.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/util.py
--rw-r--r--   0 mfe        (501) staff       (20)      763 2021-02-01 00:06:06.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)    13118 2021-02-01 00:06:06.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/visualize.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/
--rw-r--r--   0 mfe        (501) staff       (20)     9217 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/circle_world.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)     9318 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/stage_world1.py
--rw-r--r--   0 mfe        (501) staff       (20)     6994 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/ppo_stage1.py
--rw-r--r--   0 mfe        (501) staff       (20)     9765 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/stage_world2.py
--rw-r--r--   0 mfe        (501) staff       (20)     7440 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/ppo_stage2.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/model/
--rwxr-xr-x   0 mfe        (501) staff       (20)     4656 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/model/net.py
--rwxr-xr-x   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/model/__init__.py
--rwxr-xr-x   0 mfe        (501) staff       (20)     7229 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/model/utils.py
--rwxr-xr-x   0 mfe        (501) staff       (20)    10411 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/model/ppo.py
--rw-r--r--   0 mfe        (501) staff       (20)     3154 2020-04-22 18:23:21.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/circle_test.py
--rw-r--r--   0 mfe        (501) staff       (20)      479 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/ExternalPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)     5487 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/RVOPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)      920 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/InternalPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)      833 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/NonCooperativePolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)     2835 2021-02-06 21:33:14.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/PPOCADRLPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)     8335 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRLPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)     8422 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3CCADRLPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)     1092 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/LearningPolicyGA3C.py
--rw-r--r--   0 mfe        (501) staff       (20)     1498 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/Policy.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)     1357 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CARRLPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)      831 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/StaticPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)     4486 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRLLongPolicy.py
--rw-r--r--   0 mfe        (501) staff       (20)     1482 2020-08-09 15:20:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/LearningPolicy.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/__init__.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/pickle_files/
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/pickle_files/__init__.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/
--rw-r--r--   0 mfe        (501) staff       (20)    10912 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_results_multi.py
--rw-r--r--   0 mfe        (501) staff       (20)    34756 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/pedData_processing_multi.py
--rw-r--r--   0 mfe        (501) staff       (20)    16381 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_debug_multi.py
--rw-r--r--   0 mfe        (501) staff       (20)    69270 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_rl_multi.py
--rw-r--r--   0 mfe        (501) staff       (20)    14950 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_rand_testcases.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)     2577 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/global_var.py
--rw-r--r--   0 mfe        (501) staff       (20)   100397 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_navigation_value_multi.py
--rw-r--r--   0 mfe        (501) staff       (20)    27072 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/ros_nn.py
--rw-r--r--   0 mfe        (501) staff       (20)    26055 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_plots_multi.py
--rw-r--r--   0 mfe        (501) staff       (20)    31561 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/pedData_processing_multi_old.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/__init__.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/
--rw-r--r--   0 mfe        (501) staff       (20)     8815 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/multiagent_network_param.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/
--rw-r--r--   0 mfe        (501) staff       (20)     2868 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_spirals.py
--rw-r--r--   0 mfe        (501) staff       (20)     5007 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_symmetric_sinusoids.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)     3435 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_sinusoids.py
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)    12868 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network.py
--rw-r--r--   0 mfe        (501) staff       (20)    34792 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network_regr_multi.py
--rw-r--r--   0 mfe        (501) staff       (20)     1507 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/nn_training_param.py
--rw-r--r--   0 mfe        (501) staff       (20)    18432 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network_regr.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/
--rw-r--r--   0 mfe        (501) staff       (20)     1420 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.index
--rw-r--r--   0 mfe        (501) staff       (20)   403965 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.meta
--rw-r--r--   0 mfe        (501) staff       (20)  2049180 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.data-00000-of-00001
--rw-r--r--   0 mfe        (501) staff       (20)        0 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/__init__.py
--rw-r--r--   0 mfe        (501) staff       (20)     4036 2021-02-01 00:06:06.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/network.py
--rw-r--r--   0 mfe        (501) staff       (20)    24844 2021-02-01 00:06:06.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/collision_avoidance_env.py
--rw-r--r--   0 mfe        (501) staff       (20)     3055 2020-04-22 18:23:17.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/Map.py
--rw-r--r--   0 mfe        (501) staff       (20)     6322 2021-02-06 21:38:18.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/wrappers.py
--rw-r--r--   0 mfe        (501) staff       (20)    18615 2021-02-06 20:06:26.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/agent.py
--rw-r--r--   0 mfe        (501) staff       (20)    28500 2020-12-21 20:42:49.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/test_cases.py
--rw-r--r--   0 mfe        (501) staff       (20)     1430 2021-02-06 21:55:52.000000 gym_collision_avoidance-0.0.2.post2/setup.py
-drwxr-xr-x   0 mfe        (501) staff       (20)        0 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance.egg-info/
--rw-r--r--   0 mfe        (501) staff       (20)     3117 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance.egg-info/PKG-INFO
--rw-r--r--   0 mfe        (501) staff       (20)     5736 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance.egg-info/SOURCES.txt
--rw-r--r--   0 mfe        (501) staff       (20)       95 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance.egg-info/requires.txt
--rw-r--r--   0 mfe        (501) staff       (20)       24 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance.egg-info/top_level.txt
--rw-r--r--   0 mfe        (501) staff       (20)        1 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance.egg-info/dependency_links.txt
--rw-r--r--   0 mfe        (501) staff       (20)       38 2021-02-06 21:56:01.000000 gym_collision_avoidance-0.0.2.post2/setup.cfg
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.823963 gym_collision_avoidance-0.0.3/
+-rw-r--r--   0 mfe        (501) staff       (20)     1125 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/LICENSE
+-rw-r--r--   0 mfe        (501) staff       (20)     2904 2023-04-28 18:12:29.823635 gym_collision_avoidance-0.0.3/PKG-INFO
+-rw-r--r--   0 mfe        (501) staff       (20)     2562 2023-04-28 18:10:40.000000 gym_collision_avoidance-0.0.3/README.md
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.664724 gym_collision_avoidance-0.0.3/gym_collision_avoidance/
+-rw-r--r--   0 mfe        (501) staff       (20)      234 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/__init__.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.678908 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/
+-rw-r--r--   0 mfe        (501) staff       (20)     3055 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/Map.py
+-rw-r--r--   0 mfe        (501) staff       (20)      763 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/__init__.py
+-rw-r--r--   0 mfe        (501) staff       (20)    18659 2023-04-27 17:30:19.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/agent.py
+-rw-r--r--   0 mfe        (501) staff       (20)    26541 2023-04-28 17:37:11.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/collision_avoidance_env.py
+-rw-r--r--   0 mfe        (501) staff       (20)    13585 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/config.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.682624 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/
+-rw-r--r--   0 mfe        (501) staff       (20)     1711 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/Dynamics.py
+-rw-r--r--   0 mfe        (501) staff       (20)      466 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/ExternalDynamics.py
+-rw-r--r--   0 mfe        (501) staff       (20)     2088 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/UnicycleDynamics.py
+-rw-r--r--   0 mfe        (501) staff       (20)     1858 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/UnicycleDynamicsMaxTurnRate.py
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/__init__.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.691731 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.691985 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/__init__.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.692233 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/__init__.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.694014 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/__init__.py
+-rw-r--r--   0 mfe        (501) staff       (20)      196 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/nn_rl_training_param.p
+-rw-r--r--   0 mfe        (501) staff       (20)      313 2023-04-28 17:46:45.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/nn_training_param.p
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.659037 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/no_constr_none/
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.694919 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/no_constr_none/RL_selfplay/
+-rw-r--r--   0 mfe        (501) staff       (20)  1350287 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/no_constr_none/RL_selfplay/4_agents_policy_iter_1000.p
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.659520 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/rotate_constr_right/
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.716399 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/rotate_constr_right/RL_selfplay/
+-rw-r--r--   0 mfe        (501) staff       (20)  1303373 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/rotate_constr_right/RL_selfplay/4_agents_policy_iter_1300.p
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.726417 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/__init__.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.742210 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/__init__.py
+-rw-r--r--   0 mfe        (501) staff       (20)    30051 2023-04-28 16:49:40.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_plots_multi.py
+-rw-r--r--   0 mfe        (501) staff       (20)    14948 2023-04-28 16:50:52.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_rand_testcases.py
+-rw-r--r--   0 mfe        (501) staff       (20)    10892 2023-04-28 16:49:55.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_results_multi.py
+-rw-r--r--   0 mfe        (501) staff       (20)     2577 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/global_var.py
+-rw-r--r--   0 mfe        (501) staff       (20)    16361 2023-04-28 16:50:57.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_debug_multi.py
+-rw-r--r--   0 mfe        (501) staff       (20)   108798 2023-04-28 16:47:52.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_navigation_value_multi.py
+-rw-r--r--   0 mfe        (501) staff       (20)    69251 2023-04-28 16:50:12.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_rl_multi.py
+-rw-r--r--   0 mfe        (501) staff       (20)    34732 2023-04-28 16:51:25.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/pedData_processing_multi.py
+-rw-r--r--   0 mfe        (501) staff       (20)    31534 2023-04-28 16:50:31.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/pedData_processing_multi_old.py
+-rw-r--r--   0 mfe        (501) staff       (20)    27052 2023-04-28 16:51:33.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/ros_nn.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.749862 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/__init__.py
+-rw-r--r--   0 mfe        (501) staff       (20)     8815 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/multiagent_network_param.py
+-rw-r--r--   0 mfe        (501) staff       (20)    16274 2023-04-28 16:57:42.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network.py
+-rw-r--r--   0 mfe        (501) staff       (20)    18313 2023-04-28 16:55:54.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network_regr.py
+-rw-r--r--   0 mfe        (501) staff       (20)    34709 2023-04-28 16:53:49.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network_regr_multi.py
+-rw-r--r--   0 mfe        (501) staff       (20)     1507 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/nn_training_param.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.751899 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/__init__.py
+-rw-r--r--   0 mfe        (501) staff       (20)     3435 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_sinusoids.py
+-rw-r--r--   0 mfe        (501) staff       (20)     2868 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_spirals.py
+-rw-r--r--   0 mfe        (501) staff       (20)     5007 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_symmetric_sinusoids.py
+-rw-r--r--   0 mfe        (501) staff       (20)     8335 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRLPolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)     1357 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CARRLPolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)     4486 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRLLongPolicy.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.757108 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/__init__.py
+-rw-r--r--   0 mfe        (501) staff       (20)     3154 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/circle_test.py
+-rw-r--r--   0 mfe        (501) staff       (20)     9217 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/circle_world.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.759552 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/model/
+-rwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/model/__init__.py
+-rwxr-xr-x   0 mfe        (501) staff       (20)     4656 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/model/net.py
+-rwxr-xr-x   0 mfe        (501) staff       (20)    10411 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/model/ppo.py
+-rwxr-xr-x   0 mfe        (501) staff       (20)     7229 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/model/utils.py
+-rw-r--r--   0 mfe        (501) staff       (20)     6994 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/ppo_stage1.py
+-rw-r--r--   0 mfe        (501) staff       (20)     7440 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/ppo_stage2.py
+-rw-r--r--   0 mfe        (501) staff       (20)     9318 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/stage_world1.py
+-rw-r--r--   0 mfe        (501) staff       (20)     9765 2023-04-27 17:22:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/stage_world2.py
+-rw-r--r--   0 mfe        (501) staff       (20)      678 2023-04-27 17:30:19.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/ExternalPolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)     8422 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3CCADRLPolicy.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.760879 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/__init__.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.661713 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.773910 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/
+-rw-r--r--   0 mfe        (501) staff       (20)  2049180 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.data-00000-of-00001
+-rw-r--r--   0 mfe        (501) staff       (20)     1420 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.index
+-rw-r--r--   0 mfe        (501) staff       (20)   403965 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.meta
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.790237 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_015942-jzuhlntn/
+-rw-r--r--   0 mfe        (501) staff       (20)  2049180 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_015942-jzuhlntn/network_01490000.data-00000-of-00001
+-rw-r--r--   0 mfe        (501) staff       (20)     1420 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_015942-jzuhlntn/network_01490000.index
+-rw-r--r--   0 mfe        (501) staff       (20)   369619 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_015942-jzuhlntn/network_01490000.meta
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.808960 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_192048-qedrf08y/
+-rw-r--r--   0 mfe        (501) staff       (20)  2049180 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_192048-qedrf08y/network_01900000.data-00000-of-00001
+-rw-r--r--   0 mfe        (501) staff       (20)     1420 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_192048-qedrf08y/network_01900000.index
+-rw-r--r--   0 mfe        (501) staff       (20)   369619 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_192048-qedrf08y/network_01900000.meta
+-rw-r--r--   0 mfe        (501) staff       (20)     4046 2023-04-27 17:30:19.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/network.py
+-rw-r--r--   0 mfe        (501) staff       (20)      920 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/InternalPolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)     1482 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/LearningPolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)     1092 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/LearningPolicyGA3C.py
+-rw-r--r--   0 mfe        (501) staff       (20)      833 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/NonCooperativePolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)     3240 2023-04-28 17:35:04.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/PPOCADRLPolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)     1498 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/Policy.py
+-rw-r--r--   0 mfe        (501) staff       (20)     5487 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/RVOPolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)      831 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/StaticPolicy.py
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/__init__.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.815786 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/
+-rw-r--r--   0 mfe        (501) staff       (20)     5733 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/LaserScanSensor.py
+-rw-r--r--   0 mfe        (501) staff       (20)     4900 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/OccupancyGridSensor.py
+-rw-r--r--   0 mfe        (501) staff       (20)     7677 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/OtherAgentsStatesSensor.py
+-rw-r--r--   0 mfe        (501) staff       (20)      831 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/Sensor.py
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/__init__.py
+-rw-r--r--   0 mfe        (501) staff       (20)    34876 2023-04-28 17:23:35.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/test_cases.py
+-rw-r--r--   0 mfe        (501) staff       (20)     6976 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/util.py
+-rw-r--r--   0 mfe        (501) staff       (20)     6772 2023-04-28 17:35:04.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/vec_env.py
+-rw-r--r--   0 mfe        (501) staff       (20)    13118 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/visualize.py
+-rw-r--r--   0 mfe        (501) staff       (20)     6604 2023-04-28 17:36:34.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/wrappers.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.816077 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/__init__.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.822626 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/
+-rw-r--r--   0 mfe        (501) staff       (20)        0 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/__init__.py
+-rw-r--r--   0 mfe        (501) staff       (20)     2190 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/collect_regression_dataset.py
+-rw-r--r--   0 mfe        (501) staff       (20)    20904 2023-04-28 17:44:50.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/env_utils.py
+-rw-r--r--   0 mfe        (501) staff       (20)     1996 2023-04-28 16:34:15.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/example.py
+-rw-r--r--   0 mfe        (501) staff       (20)     4437 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/process_full_test_suite_pickles.py
+-rw-r--r--   0 mfe        (501) staff       (20)     2342 2023-04-28 17:15:04.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/run_cadrl_formations.py
+-rw-r--r--   0 mfe        (501) staff       (20)     4443 2023-04-28 17:16:38.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/run_full_test_suite.py
+-rw-r--r--   0 mfe        (501) staff       (20)     5770 2023-04-27 17:22:13.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/run_trajectory_dataset_creator.py
+drwxr-xr-x   0 mfe        (501) staff       (20)        0 2023-04-28 18:12:29.667779 gym_collision_avoidance-0.0.3/gym_collision_avoidance.egg-info/
+-rw-r--r--   0 mfe        (501) staff       (20)     2904 2023-04-28 18:12:29.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance.egg-info/PKG-INFO
+-rw-r--r--   0 mfe        (501) staff       (20)     6846 2023-04-28 18:12:29.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance.egg-info/SOURCES.txt
+-rw-r--r--   0 mfe        (501) staff       (20)        1 2023-04-28 18:12:29.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance.egg-info/dependency_links.txt
+-rw-r--r--   0 mfe        (501) staff       (20)       84 2023-04-28 18:12:29.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance.egg-info/requires.txt
+-rw-r--r--   0 mfe        (501) staff       (20)       24 2023-04-28 18:12:29.000000 gym_collision_avoidance-0.0.3/gym_collision_avoidance.egg-info/top_level.txt
+-rw-r--r--   0 mfe        (501) staff       (20)       38 2023-04-28 18:12:29.824532 gym_collision_avoidance-0.0.3/setup.cfg
+-rw-r--r--   0 mfe        (501) staff       (20)     1008 2023-04-28 18:11:02.000000 gym_collision_avoidance-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gym_collision_avoidance-0.0.2.post2/PKG-INFO` & `gym_collision_avoidance-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,52 @@
-Metadata-Version: 2.1
-Name: gym_collision_avoidance
-Version: 0.0.2.post2
-Summary: Simulation environment for collision avoidance
-Home-page: https://github.com/mit-acl/gym-collision-avoidance
-Author: Michael Everett, Yu Fan Chen, Jonathan P. How, MIT
-License: UNKNOWN
-Description: # gym-collision-avoidance
-        
-        <img src="docs/_static/combo.gif" alt="Agents spelling ``CADRL''">
-        
-        This is the code associated with the following publications:
-        
-        **Journal Version:** M. Everett, Y. Chen, and J. P. How, "Collision Avoidance in Pedestrian-Rich Environments with Deep Reinforcement Learning", IEEE Access Vol. 9, 2021, pp. 10357-10377. [10.1109/ACCESS.2021.3050338](http://doi.org/10.1109/ACCESS.2021.3050338), [Arxiv PDF](https://arxiv.org/abs/1910.11689)
-        
-        **Conference Version:** M. Everett, Y. Chen, and J. P. How, "Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning", IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2018. [Arxiv PDF](https://arxiv.org/abs/1805.01956), [Link to Video](https://www.youtube.com/watch?v=XHoXkWLhwYQ)
-        
-        This repo also contains the trained policy for the SA-CADRL paper (referred to as CADRL here) from the proceeding paper: Y. Chen, M. Everett, M. Liu, and J. P. How. “Socially Aware Motion Planning with Deep Reinforcement Learning.” IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). Vancouver, BC, Canada, Sept. 2017. [Arxiv PDF](https://arxiv.org/abs/1703.08862)
-        
-        If you're looking to train our GA3C-CADRL policy, please see [this repo](https://github.com/mit-acl/rl_collision_avoidance) instead.
-        
-        ---
-        
-        ### About the Code
-        
-        Please see [the documentation](https://gym-collision-avoidance.readthedocs.io/en/latest/)!
-        
-        ### If you find this code useful, please consider citing:
-        
-        ```
-        @inproceedings{Everett18_IROS,
-          address = {Madrid, Spain},
-          author = {Everett, Michael and Chen, Yu Fan and How, Jonathan P.},
-          booktitle = {IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
-          date-modified = {2018-10-03 06:18:08 -0400},
-          month = sep,
-          title = {Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning},
-          year = {2018},
-          url = {https://arxiv.org/pdf/1805.01956.pdf},
-          bdsk-url-1 = {https://arxiv.org/pdf/1805.01956.pdf}
-        }
-        ```
-        
-        or
-        
-        ```
-        @article{everett2021collision,
-          title={Collision avoidance in pedestrian-rich environments with deep reinforcement learning},
-          author={Everett, Michael and Chen, Yu Fan and How, Jonathan P},
-          journal={IEEE Access},
-          volume={9},
-          pages={10357--10377},
-          year={2021},
-          publisher={IEEE}
-        }
-        ```
-        
-Keywords: robotics planning gym rl
-Platform: UNKNOWN
-Requires-Python: <3.8
-Description-Content-Type: text/markdown
+# gym-collision-avoidance
+
+Updates:
+- **2023-04-28:** Updated to be compatible with Python 3.10 and tensorflow 2. Corresponding v0.0.3 available on pypi as well, if you do not intend to modify the source code (`python -m pip install gym-collision-avoidance`)
+
+<img src="docs/_static/combo.gif" alt="Agents spelling ``CADRL''">
+
+This is the code associated with the following publications:
+
+**Journal Version:** M. Everett, Y. Chen, and J. P. How, "Collision Avoidance in Pedestrian-Rich Environments with Deep Reinforcement Learning", IEEE Access Vol. 9, 2021, pp. 10357-10377. [10.1109/ACCESS.2021.3050338](http://doi.org/10.1109/ACCESS.2021.3050338), [Arxiv PDF](https://arxiv.org/abs/1910.11689)
+
+**Conference Version:** M. Everett, Y. Chen, and J. P. How, "Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning", IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2018. [Arxiv PDF](https://arxiv.org/abs/1805.01956), [Link to Video](https://www.youtube.com/watch?v=XHoXkWLhwYQ)
+
+This repo also contains the trained policy for the SA-CADRL paper (referred to as CADRL here) from the proceeding paper: Y. Chen, M. Everett, M. Liu, and J. P. How. “Socially Aware Motion Planning with Deep Reinforcement Learning.” IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). Vancouver, BC, Canada, Sept. 2017. [Arxiv PDF](https://arxiv.org/abs/1703.08862)
+
+If you're looking to train our GA3C-CADRL policy, please see [this repo](https://github.com/mit-acl/rl_collision_avoidance) instead.
+
+---
+
+### About the Code
+
+Please see [the documentation](https://gym-collision-avoidance.readthedocs.io/en/latest/)!
+
+### If you find this code useful, please consider citing:
+
+```
+@inproceedings{Everett18_IROS,
+  address = {Madrid, Spain},
+  author = {Everett, Michael and Chen, Yu Fan and How, Jonathan P.},
+  booktitle = {IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
+  date-modified = {2018-10-03 06:18:08 -0400},
+  month = sep,
+  title = {Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning},
+  year = {2018},
+  url = {https://arxiv.org/pdf/1805.01956.pdf},
+  bdsk-url-1 = {https://arxiv.org/pdf/1805.01956.pdf}
+}
+```
+
+or
+
+```
+@article{everett2021collision,
+  title={Collision avoidance in pedestrian-rich environments with deep reinforcement learning},
+  author={Everett, Michael and Chen, Yu Fan and How, Jonathan P},
+  journal={IEEE Access},
+  volume={9},
+  pages={10357--10377},
+  year={2021},
+  publisher={IEEE}
+}
+```
```

### Comparing `gym_collision_avoidance-0.0.2.post2/README.md` & `gym_collision_avoidance-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+Metadata-Version: 2.1
+Name: gym_collision_avoidance
+Version: 0.0.3
+Summary: Simulation environment for collision avoidance
+Home-page: https://github.com/mit-acl/gym-collision-avoidance
+Author: Michael Everett, Yu Fan Chen, Jonathan P. How, MIT
+Keywords: robotics planning gym rl
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # gym-collision-avoidance
 
+Updates:
+- **2023-04-28:** Updated to be compatible with Python 3.10 and tensorflow 2. Corresponding v0.0.3 available on pypi as well, if you do not intend to modify the source code (`python -m pip install gym-collision-avoidance`)
+
 <img src="docs/_static/combo.gif" alt="Agents spelling ``CADRL''">
 
 This is the code associated with the following publications:
 
 **Journal Version:** M. Everett, Y. Chen, and J. P. How, "Collision Avoidance in Pedestrian-Rich Environments with Deep Reinforcement Learning", IEEE Access Vol. 9, 2021, pp. 10357-10377. [10.1109/ACCESS.2021.3050338](http://doi.org/10.1109/ACCESS.2021.3050338), [Arxiv PDF](https://arxiv.org/abs/1910.11689)
 
 **Conference Version:** M. Everett, Y. Chen, and J. P. How, "Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning", IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2018. [Arxiv PDF](https://arxiv.org/abs/1805.01956), [Link to Video](https://www.youtube.com/watch?v=XHoXkWLhwYQ)
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/process_full_test_suite_pickles.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/process_full_test_suite_pickles.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/env_utils.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/env_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,506 +1,492 @@
 import gym
+
 gym.logger.set_level(40)
 import numpy as np
+import pandas as pd
+
 from gym_collision_avoidance.envs import Config
-from gym_collision_avoidance.envs.wrappers import FlattenDictWrapper, MultiagentFlattenDictWrapper, MultiagentDummyVecEnv, MultiagentDictToMultiagentArrayWrapper
-from gym_collision_avoidance.envs.vec_env import DummyVecEnv
+from gym_collision_avoidance.envs.wrappers import (
+    FlattenDictWrapper,
+    MultiagentDictToMultiagentArrayWrapper,
+    MultiagentFlattenDictWrapper,
+)
+
 
 def create_env():
-    import tensorflow as tf
-    tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
+    import tensorflow.compat.v1 as tf
+
+    tf.logging.set_verbosity(tf.compat.v1.logging.ERROR)
     tf.Session().__enter__()
-    num_envs = 1
-    ncpu = 1
-    
+
     def make_env():
         env = gym.make("CollisionAvoidance-v0")
 
         # The env provides a dict observation by default. Most RL code
         # doesn't handle dict observations, so these wrappers convert to arrays
         if Config.TRAIN_SINGLE_AGENT:
             # only return observations of a single agent
             env = FlattenDictWrapper(env, dict_keys=Config.STATES_IN_OBS)
         else:
             # Convert the dict into an np array, shape=(max_num_agents, num_states_per_agent)
-            env = MultiagentDictToMultiagentArrayWrapper(env, dict_keys=Config.STATES_IN_OBS, max_num_agents=Config.MAX_NUM_AGENTS_IN_ENVIRONMENT)
+            env = MultiagentDictToMultiagentArrayWrapper(
+                env,
+                dict_keys=Config.STATES_IN_OBS,
+                max_num_agents=Config.MAX_NUM_AGENTS_IN_ENVIRONMENT,
+            )
             # Convert the dict into a flat np array, shape=(max_num_agents*num_states_per_agent)
             # env = MultiagentFlattenDictWrapper(env, dict_keys=Config.STATES_IN_OBS, max_num_agents=Config.MAX_NUM_AGENTS_IN_ENVIRONMENT)
-        
+
         return env
-    
-    # To be prepared for training on multiple instances of the env at once
-    if Config.TRAIN_SINGLE_AGENT:
-        env = DummyVecEnv([make_env for _ in range(num_envs)])
-    else:
-        env = MultiagentDummyVecEnv([make_env for _ in range(num_envs)])
-    unwrapped_envs = [e.unwrapped for e in env.envs]
-    
-    # Set env id for each env
-    for i, e in enumerate(unwrapped_envs):
-        e.id = i
-    
-    one_env = unwrapped_envs[0]
-    return env, one_env
 
-def run_episode(env, one_env):
+    env = make_env()
+    return env
+
+
+def run_episode(env):
     total_reward = 0
     step = 0
-    done = False
-    while not done:
-        obs, rew, done, info = env.step([None])
-        total_reward += rew[0]
+    terminated = False
+    while not terminated:
+        obs, rew, terminated, truncated, info = env.step(None)
+        total_reward += rew
         step += 1
 
     # After end of episode, store some statistics about the environment
     # Some stats apply to every gym env...
     generic_episode_stats = {
-        'total_reward': total_reward,
-        'steps': step,
+        "total_reward": total_reward,
+        "steps": step,
     }
 
-    agents = one_env.agents
-    # agents = one_env.prev_episode_agents
+    agents = env.agents
     time_to_goal = np.array([a.t for a in agents])
-    extra_time_to_goal = np.array([a.t - a.straight_line_time_to_reach_goal for a in agents])
-    collision = np.array(
-        np.any([a.in_collision for a in agents])).tolist()
-    all_at_goal = np.array(
-        np.all([a.is_at_goal for a in agents])).tolist()
+    extra_time_to_goal = np.array(
+        [a.t - a.straight_line_time_to_reach_goal for a in agents]
+    )
+    collision = np.array(np.any([a.in_collision for a in agents])).tolist()
+    all_at_goal = np.array(np.all([a.is_at_goal for a in agents])).tolist()
     any_stuck = np.array(
-        np.any([not a.in_collision and not a.is_at_goal for a in agents])).tolist()
-    outcome = "collision" if collision else "all_at_goal" if all_at_goal else "stuck"
+        np.any([not a.in_collision and not a.is_at_goal for a in agents])
+    ).tolist()
+    outcome = (
+        "collision" if collision else "all_at_goal" if all_at_goal else "stuck"
+    )
     specific_episode_stats = {
-        'num_agents': len(agents),
-        'time_to_goal': time_to_goal,
-        'total_time_to_goal': np.sum(time_to_goal),
-        'extra_time_to_goal': extra_time_to_goal,
-        'collision': collision,
-        'all_at_goal': all_at_goal,
-        'any_stuck': any_stuck,
-        'outcome': outcome,
-        'policies': [agent.policy.str for agent in agents],
+        "num_agents": len(agents),
+        "time_to_goal": time_to_goal,
+        "total_time_to_goal": np.sum(time_to_goal),
+        "extra_time_to_goal": extra_time_to_goal,
+        "collision": collision,
+        "all_at_goal": all_at_goal,
+        "any_stuck": any_stuck,
+        "outcome": outcome,
+        "policies": [agent.policy.str for agent in agents],
     }
 
     # Merge all stats into a single dict
     episode_stats = {**generic_episode_stats, **specific_episode_stats}
 
     env.reset()
 
     return episode_stats, agents
 
+
 def store_stats(df, hyperparameters, episode_stats):
     # Add a new row to the pandas DataFrame (a table of results, where each row is an episode)
     # that contains the hyperparams and stats from that episode, for logging purposes
     df_columns = {**hyperparameters, **episode_stats}
-    df = df.append(df_columns, ignore_index=True)
+    df = pd.concat([df, pd.DataFrame([df_columns])], ignore_index=True)
     return df
 
 
 policies = {
-
-    'GA3C-CADRL-10-WS-4-1': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-184-72-212-132.compute-1.amazonaws.com/wandb/run-20200403_144424-3eoowzko/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-10-WS-4-2': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-34-228-142-219.compute-1.amazonaws.com/wandb/run-20200403_144424-eozu6syw/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-10-WS-4-3': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-146-99-195.compute-1.amazonaws.com/wandb/run-20200403_144424-22s6pbwt/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-10-WS-4-4': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-227-24-219.compute-1.amazonaws.com/wandb/run-20200403_144424-2f8r4ydk/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-10-WS-4-5': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-242-32-57.compute-1.amazonaws.com/wandb/run-20200403_144424-i41jmnda/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-
-
-    'GA3C-CADRL-4-WS-4-1': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-184-72-212-132.compute-1.amazonaws.com/wandb/run-20200402_210747-dt4uwai3/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-4-WS-4-2': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-34-228-142-219.compute-1.amazonaws.com/wandb/run-20200402_210747-cvcfrsqt/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-4-WS-4-3': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-146-99-195.compute-1.amazonaws.com/wandb/run-20200402_210747-1rmgsf1f/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-4-WS-4-4': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-227-24-219.compute-1.amazonaws.com/wandb/run-20200402_210747-2unxv49c/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-4-WS-4-5': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-242-32-57.compute-1.amazonaws.com/wandb/run-20200402_210747-2hjygfa8/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-
-
-    'GA3C-CADRL-10-LSTM-1': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-107-21-169-18.compute-1.amazonaws.com/wandb/run-20200403_144352-24y2fdt1/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 19,
-            },
-        },
-    'GA3C-CADRL-10-LSTM-2': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-107-22-158-27.compute-1.amazonaws.com/wandb/run-20200403_144352-degz8bdo/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 19,
-            },
-        },
-    'GA3C-CADRL-10-LSTM-3': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-34-228-80-228.compute-1.amazonaws.com/wandb/run-20200403_144352-38r4hkya/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 19,
-            },
-        },
-    'GA3C-CADRL-10-LSTM-4': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-54-226-118-56.compute-1.amazonaws.com/wandb/run-20200403_144352-2wxsxlws/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 19,
-            },
-        },
-    'GA3C-CADRL-10-LSTM-5': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-54-226-192-14.compute-1.amazonaws.com/wandb/run-20200403_144352-13bui0x5/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 19,
-            },
-        },
-
-    'GA3C-CADRL-4-LSTM-1': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-107-21-169-18.compute-1.amazonaws.com/wandb/run-20200402_205112-3dz5k5pp/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-4-LSTM-2': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-107-22-158-27.compute-1.amazonaws.com/wandb/run-20200402_205111-1kglu4km/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-4-LSTM-3': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-34-228-80-228.compute-1.amazonaws.com/wandb/run-20200402_205112-16352wzy/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-4-LSTM-4': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-54-226-118-56.compute-1.amazonaws.com/wandb/run-20200402_205112-25eq7fer/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-    'GA3C-CADRL-4-LSTM-5': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-54-226-192-14.compute-1.amazonaws.com/wandb/run-20200402_205111-2pka2zpr/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 3,
-            },
-        },
-
-
-
-    'GA3C-CADRL-4-WS-6-1': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-35-174-113-253.compute-1.amazonaws.com/wandb/run-20200412_151445-icfzrvij/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 5,
-            },
-        },
-    'GA3C-CADRL-4-WS-6-2': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-3-88-36-89.compute-1.amazonaws.com/wandb/run-20200412_151445-2iv4i4nj/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 5,
-            },
-        },
-    'GA3C-CADRL-4-WS-6-3': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-54-161-193-150.compute-1.amazonaws.com/wandb/run-20200412_151445-91kuvs98/checkpoints/',
-        'checkpt_name': 'network_01490001',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 5,
-            },
-        },
-    'GA3C-CADRL-4-WS-6-4': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-54-243-3-91.compute-1.amazonaws.com/wandb/run-20200412_051045-crf4k6on/checkpoints/',
-        'checkpt_name': 'network_01490001',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 5,
-            },
-        },
-    'GA3C-CADRL-10-WS-6-1': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-35-174-113-253.compute-1.amazonaws.com/wandb/run-20200413_023855-3mbmr1nc/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 5,
-            },
-        },
-    'GA3C-CADRL-10-WS-6-2': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-3-88-36-89.compute-1.amazonaws.com/wandb/run-20200413_023855-3pxw2ixl/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 5,
-            },
-        },
-    'GA3C-CADRL-10-WS-6-3': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-54-161-193-150.compute-1.amazonaws.com/wandb/run-20200413_023939-sgw8r5gx/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 5,
-            },
-        },
-    'GA3C-CADRL-10-WS-6-4': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-54-243-3-91.compute-1.amazonaws.com/wandb/run-20200412_163307-1yz34rae/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 5,
-            },
-        },
-
-    'GA3C-CADRL-4-WS-8-1': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-18-212-168-204.compute-1.amazonaws.com/wandb/run-20200412_151345-1luyhexf/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 7,
-            },
-        },
-    'GA3C-CADRL-4-WS-8-2': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-34-203-243-164.compute-1.amazonaws.com/wandb/run-20200412_151345-2j2jvgjv/checkpoints/',
-        'checkpt_name': 'network_01490001',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 7,
-            },
-        },
-    'GA3C-CADRL-4-WS-8-3': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-3-92-177-119.compute-1.amazonaws.com/wandb/run-20200412_051045-3oza4dxf/checkpoints/',
-        'checkpt_name': 'network_01490002',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 7,
-            },
-        },
-    'GA3C-CADRL-4-WS-8-4': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-54-211-142-133.compute-1.amazonaws.com/wandb/run-20200412_151345-3ql9fhpf/checkpoints/',
-        'checkpt_name': 'network_01490000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 7,
-            },
-        },
-    'GA3C-CADRL-10-WS-8-1': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-18-212-168-204.compute-1.amazonaws.com/wandb/run-20200413_024321-3m0g6fei/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 7,
-            },
-        },
-    'GA3C-CADRL-10-WS-8-2': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-34-203-243-164.compute-1.amazonaws.com/wandb/run-20200413_024321-1qog6ten/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 7,
-            },
-        },
-    'GA3C-CADRL-10-WS-8-3': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-3-92-177-119.compute-1.amazonaws.com/wandb/run-20200412_163307-1yslbfru/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 7,
-            },
-        },
-    'GA3C-CADRL-10-WS-8-4': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': '/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-54-211-142-133.compute-1.amazonaws.com/wandb/run-20200413_024321-1i8errn0/checkpoints/',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 7,
-            },
-        },
-
-    'GA3C-CADRL-10': {
-        'policy': 'GA3C_CADRL',
-        'checkpt_dir': 'IROS18',
-        'checkpt_name': 'network_01900000',
-        'sensors': ['other_agents_states'],
-        'sensor_args': {
-            'agent_sorting_method': 'closest_last',
-            'max_num_other_agents_observed': 19,
-            },
+    "GA3C-CADRL-10-WS-4-1": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-184-72-212-132.compute-1.amazonaws.com/wandb/run-20200403_144424-3eoowzko/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-10-WS-4-2": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-34-228-142-219.compute-1.amazonaws.com/wandb/run-20200403_144424-eozu6syw/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-10-WS-4-3": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-146-99-195.compute-1.amazonaws.com/wandb/run-20200403_144424-22s6pbwt/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-10-WS-4-4": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-227-24-219.compute-1.amazonaws.com/wandb/run-20200403_144424-2f8r4ydk/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-10-WS-4-5": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-242-32-57.compute-1.amazonaws.com/wandb/run-20200403_144424-i41jmnda/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-WS-4-1": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-184-72-212-132.compute-1.amazonaws.com/wandb/run-20200402_210747-dt4uwai3/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-WS-4-2": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-34-228-142-219.compute-1.amazonaws.com/wandb/run-20200402_210747-cvcfrsqt/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-WS-4-3": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-146-99-195.compute-1.amazonaws.com/wandb/run-20200402_210747-1rmgsf1f/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-WS-4-4": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-227-24-219.compute-1.amazonaws.com/wandb/run-20200402_210747-2unxv49c/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-WS-4-5": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_ec2-54-242-32-57.compute-1.amazonaws.com/wandb/run-20200402_210747-2hjygfa8/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-10-LSTM-1": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-107-21-169-18.compute-1.amazonaws.com/wandb/run-20200403_144352-24y2fdt1/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 19,
+        },
+    },
+    "GA3C-CADRL-10-LSTM-2": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-107-22-158-27.compute-1.amazonaws.com/wandb/run-20200403_144352-degz8bdo/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 19,
+        },
+    },
+    "GA3C-CADRL-10-LSTM-3": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-34-228-80-228.compute-1.amazonaws.com/wandb/run-20200403_144352-38r4hkya/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 19,
+        },
+    },
+    "GA3C-CADRL-10-LSTM-4": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-54-226-118-56.compute-1.amazonaws.com/wandb/run-20200403_144352-2wxsxlws/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 19,
+        },
+    },
+    "GA3C-CADRL-10-LSTM-5": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-54-226-192-14.compute-1.amazonaws.com/wandb/run-20200403_144352-13bui0x5/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 19,
+        },
+    },
+    "GA3C-CADRL-4-LSTM-1": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-107-21-169-18.compute-1.amazonaws.com/wandb/run-20200402_205112-3dz5k5pp/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-LSTM-2": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-107-22-158-27.compute-1.amazonaws.com/wandb/run-20200402_205111-1kglu4km/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-LSTM-3": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-34-228-80-228.compute-1.amazonaws.com/wandb/run-20200402_205112-16352wzy/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-LSTM-4": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-54-226-118-56.compute-1.amazonaws.com/wandb/run-20200402_205112-25eq7fer/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-LSTM-5": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/rnn_order_ec2-54-226-192-14.compute-1.amazonaws.com/wandb/run-20200402_205111-2pka2zpr/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 3,
+        },
+    },
+    "GA3C-CADRL-4-WS-6-1": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-35-174-113-253.compute-1.amazonaws.com/wandb/run-20200412_151445-icfzrvij/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 5,
+        },
+    },
+    "GA3C-CADRL-4-WS-6-2": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-3-88-36-89.compute-1.amazonaws.com/wandb/run-20200412_151445-2iv4i4nj/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 5,
+        },
+    },
+    "GA3C-CADRL-4-WS-6-3": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-54-161-193-150.compute-1.amazonaws.com/wandb/run-20200412_151445-91kuvs98/checkpoints/",
+        "checkpt_name": "network_01490001",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 5,
+        },
+    },
+    "GA3C-CADRL-4-WS-6-4": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-54-243-3-91.compute-1.amazonaws.com/wandb/run-20200412_051045-crf4k6on/checkpoints/",
+        "checkpt_name": "network_01490001",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 5,
+        },
+    },
+    "GA3C-CADRL-10-WS-6-1": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-35-174-113-253.compute-1.amazonaws.com/wandb/run-20200413_023855-3mbmr1nc/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 5,
+        },
+    },
+    "GA3C-CADRL-10-WS-6-2": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-3-88-36-89.compute-1.amazonaws.com/wandb/run-20200413_023855-3pxw2ixl/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 5,
+        },
+    },
+    "GA3C-CADRL-10-WS-6-3": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-54-161-193-150.compute-1.amazonaws.com/wandb/run-20200413_023939-sgw8r5gx/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 5,
+        },
+    },
+    "GA3C-CADRL-10-WS-6-4": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_6_ec2-54-243-3-91.compute-1.amazonaws.com/wandb/run-20200412_163307-1yz34rae/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 5,
+        },
+    },
+    "GA3C-CADRL-4-WS-8-1": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-18-212-168-204.compute-1.amazonaws.com/wandb/run-20200412_151345-1luyhexf/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 7,
+        },
+    },
+    "GA3C-CADRL-4-WS-8-2": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-34-203-243-164.compute-1.amazonaws.com/wandb/run-20200412_151345-2j2jvgjv/checkpoints/",
+        "checkpt_name": "network_01490001",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 7,
+        },
+    },
+    "GA3C-CADRL-4-WS-8-3": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-3-92-177-119.compute-1.amazonaws.com/wandb/run-20200412_051045-3oza4dxf/checkpoints/",
+        "checkpt_name": "network_01490002",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 7,
+        },
+    },
+    "GA3C-CADRL-4-WS-8-4": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-54-211-142-133.compute-1.amazonaws.com/wandb/run-20200412_151345-3ql9fhpf/checkpoints/",
+        "checkpt_name": "network_01490000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 7,
+        },
+    },
+    "GA3C-CADRL-10-WS-8-1": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-18-212-168-204.compute-1.amazonaws.com/wandb/run-20200413_024321-3m0g6fei/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 7,
+        },
+    },
+    "GA3C-CADRL-10-WS-8-2": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-34-203-243-164.compute-1.amazonaws.com/wandb/run-20200413_024321-1qog6ten/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 7,
+        },
+    },
+    "GA3C-CADRL-10-WS-8-3": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-3-92-177-119.compute-1.amazonaws.com/wandb/run-20200412_163307-1yslbfru/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 7,
+        },
+    },
+    "GA3C-CADRL-10-WS-8-4": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "/home/mfe/ijrr_cadrl_results/multiple_seeds/ws_order_8_ec2-54-211-142-133.compute-1.amazonaws.com/wandb/run-20200413_024321-1i8errn0/checkpoints/",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 7,
+        },
+    },
+    "GA3C-CADRL-10": {
+        "policy": "GA3C_CADRL",
+        "checkpt_dir": "IROS18",
+        "checkpt_name": "network_01900000",
+        "sensors": ["other_agents_states"],
+        "sensor_args": {
+            "agent_sorting_method": "closest_last",
+            "max_num_other_agents_observed": 19,
         },
-
+    },
     # 'GA3C-CADRL-4-LSTM': {
     #     'policy': 'GA3C_CADRL',
     #     'checkpt_dir': "run-20190727_015942-jzuhlntn",
     #     'checkpt_name': 'network_01490000',
     #     'sensors': ['other_agents_states'],
     #     },
-    'CADRL': {
-        'policy': 'CADRL',
-        'sensors': ['other_agents_states'],
-        },
-    'RVO': {
-        'policy': 'RVO',
-        'sensors': ['other_agents_states'],
-        },
-    'DRL-Long': {
-        'policy': 'drllong',
-        'checkpt_name': 'stage2.pth',
-        'sensors': ['other_agents_states', 'laserscan']
-        },
-    }
-
-if __name__ == '__main__':
-    env, one_env = create_env()
-    env.reset()
-    run_episode(env, one_env)
+    "CADRL": {
+        "policy": "CADRL",
+        "sensors": ["other_agents_states"],
+    },
+    "RVO": {
+        "policy": "RVO",
+        "sensors": ["other_agents_states"],
+    },
+    "DRL-Long": {
+        "policy": "drllong",
+        "checkpt_name": "stage2.pth",
+        "sensors": ["other_agents_states", "laserscan"],
+    },
+}
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/example.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 import os
-import numpy as np
+
 import gym
+import numpy as np
+
 gym.logger.set_level(40)
-os.environ['GYM_CONFIG_CLASS'] = 'Example'
-from gym_collision_avoidance.envs import test_cases as tc
+os.environ["GYM_CONFIG_CLASS"] = "Example"
 from gym_collision_avoidance.envs import Config
+from gym_collision_avoidance.envs import test_cases as tc
+
 
 def main():
-    '''
+    """
     Minimum working example:
     2 agents: 1 running external policy, 1 running GA3C-CADRL
-    '''
+    """
 
     # Create single tf session for all experiments
-    import tensorflow as tf
-    tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
+    import tensorflow.compat.v1 as tf
+
+    tf.logging.set_verbosity(tf.compat.v1.logging.ERROR)
     tf.Session().__enter__()
 
     # Instantiate the environment
     env = gym.make("CollisionAvoidance-v0")
 
     # In case you want to save plots, choose the directory
     env.set_plot_save_dir(
-        os.path.dirname(os.path.realpath(__file__)) + '/../../experiments/results/example/')
+        os.path.dirname(os.path.realpath(__file__))
+        + "/../../experiments/results/example/"
+    )
 
     # Set agent configuration (start/goal pos, radius, size, policy)
     agents = tc.get_testcase_two_agents()
-    [agent.policy.initialize_network() for agent in agents if hasattr(agent.policy, 'initialize_network')]
+    [
+        agent.policy.initialize_network()
+        for agent in agents
+        if hasattr(agent.policy, "initialize_network")
+    ]
     env.set_agents(agents)
 
-    obs = env.reset() # Get agents' initial observations
+    obs = env.reset()  # Get agents' initial observations
 
     # Repeatedly send actions to the environment based on agents' observations
     num_steps = 100
     for i in range(num_steps):
-
         # Query the external agents' policies
         # e.g., actions[0] = external_policy(dict_obs[0])
         actions = {}
-        actions[0] = np.array([1., 0.5])
+        actions[0] = np.array([1.0, 0.5])
 
         # Internal agents (running a pre-learned policy defined in envs/policies)
         # will automatically query their policy during env.step
         # ==> no need to supply actions for internal agents here
 
         # Run a simulation step (check for collisions, move sim agents)
-        obs, rewards, game_over, which_agents_done = env.step(actions)
+        obs, rewards, terminated, truncated, which_agents_done = env.step(
+            actions
+        )
 
-        if game_over:
+        if terminated:
             print("All agents finished!")
             break
     env.reset()
 
     return True
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
     print("Experiment over.")
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/run_trajectory_dataset_creator.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/run_trajectory_dataset_creator.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/experiments/src/collect_regression_dataset.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/experiments/src/collect_regression_dataset.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/Sensor.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/Sensor.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/LaserScanSensor.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/LaserScanSensor.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/OtherAgentsStatesSensor.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/OtherAgentsStatesSensor.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/sensors/OccupancyGridSensor.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/sensors/OccupancyGridSensor.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/UnicycleDynamics.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/UnicycleDynamics.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/UnicycleDynamicsMaxTurnRate.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/UnicycleDynamicsMaxTurnRate.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/dynamics/Dynamics.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/dynamics/Dynamics.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/vec_env.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/vec_env.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/config.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/config.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/util.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/util.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/__init__.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/visualize.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/visualize.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/circle_world.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/circle_world.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/stage_world1.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/stage_world1.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/ppo_stage1.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/ppo_stage1.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/stage_world2.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/stage_world2.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/ppo_stage2.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/ppo_stage2.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/model/net.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/model/net.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/model/utils.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/model/utils.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/model/ppo.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/model/ppo.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRL_Long/circle_test.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRL_Long/circle_test.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/RVOPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/RVOPolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/InternalPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/InternalPolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/NonCooperativePolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/NonCooperativePolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/PPOCADRLPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/PPOCADRLPolicy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,92 @@
-import numpy as np
 import os
-from gym_collision_avoidance.envs.policies.InternalPolicy import InternalPolicy
+
+import numpy as np
+
 # from stable_baselines.common.policies import build_policy
 from gym_collision_avoidance.envs import Config
+from gym_collision_avoidance.envs.policies.InternalPolicy import InternalPolicy
+
+# from stable_baselines.ppo2.mfe_network import mfe_network
+# import tensorflow as tf
 # from stable_baselines.ppo2.mfe_network import mfe_network
-import tensorflow as tf
+# import tensorflow.compat.v1 as tf
+
 
 class PPOCADRLPolicy(InternalPolicy):
     def __init__(self):
         InternalPolicy.__init__(self, str="PPO_CADRL")
         self.ppo_or_learning_policy = True
 
     def initialize_network(self, **kwargs):
-        if 'checkpt_name' in kwargs:
-            checkpoint_name = kwargs['checkpt_name']
+        if "checkpt_name" in kwargs:
+            checkpoint_name = kwargs["checkpt_name"]
         else:
-            checkpoint_name = '2019-07-09-02-21-39-039832-00610'
+            checkpoint_name = "2019-07-09-02-21-39-039832-00610"
         network = Config.NETWORK
-        file_dir = os.path.dirname(os.path.realpath(__file__)) + '/PPO_CADRL/checkpoints/'
+        file_dir = (
+            os.path.dirname(os.path.realpath(__file__))
+            + "/PPO_CADRL/checkpoints/"
+        )
         load_path = file_dir + checkpoint_name
-        load_path = "/tmp/wandb/run-20190712_184254-9ko7u0w0/checkpoints/00575.ckpt"
-        load_path = "/tmp/wandb/run-20190712_210835-xos1fxrm/checkpoints/00410.ckpt"
-        load_path = "/tmp/wandb/run-20190712_213449-3nteijf4/checkpoints/00545.ckpt"
-        load_path = "/tmp/wandb/run-20190712_222413-ha8ghayz/checkpoints/00500.ckpt"
-        load_path = "/tmp/wandb/run-20190714_183509-x6mb5po7/checkpoints/00545.ckpt"
-        load_path = "/tmp/wandb/run-20190714_190552-nmamlb75/checkpoints/00610.ckpt"
-        load_path = "/tmp/wandb/run-20190714_195544-ozrm02gt/checkpoints/00610.ckpt"
-        load_path = "/tmp/wandb/run-20190714_203538-7peo10xo/checkpoints/00610.ckpt"
-        load_path = "/tmp/wandb/run-20190715_200243-ngfnyie7/checkpoints/00610.ckpt"
-        load_path = "/tmp/wandb/run-20190716_001241-4bw8vz63/checkpoints/02100.ckpt"
-
+        load_path = (
+            "/tmp/wandb/run-20190712_184254-9ko7u0w0/checkpoints/00575.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190712_210835-xos1fxrm/checkpoints/00410.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190712_213449-3nteijf4/checkpoints/00545.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190712_222413-ha8ghayz/checkpoints/00500.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190714_183509-x6mb5po7/checkpoints/00545.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190714_190552-nmamlb75/checkpoints/00610.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190714_195544-ozrm02gt/checkpoints/00610.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190714_203538-7peo10xo/checkpoints/00610.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190715_200243-ngfnyie7/checkpoints/00610.ckpt"
+        )
+        load_path = (
+            "/tmp/wandb/run-20190716_001241-4bw8vz63/checkpoints/02100.ckpt"
+        )
 
         network_kwargs = {
-            'states_in_obs': Config.STATES_IN_OBS,
-            'states_not_used_in_network': Config.STATES_NOT_USED_IN_POLICY,
-            'mean_obs': Config.MEAN_OBS,
-            'std_obs': Config.STD_OBS,
-            'normalize_input': Config.NORMALIZE_INPUT,
-            'num_hidden': Config.NUM_HIDDEN_UNITS,
-            'num_layers': Config.NUM_LAYERS,
-            'lstm_hidden_size': Config.LSTM_HIDDEN_SIZE
+            "states_in_obs": Config.STATES_IN_OBS,
+            "states_not_used_in_network": Config.STATES_NOT_USED_IN_POLICY,
+            "mean_obs": Config.MEAN_OBS,
+            "std_obs": Config.STD_OBS,
+            "normalize_input": Config.NORMALIZE_INPUT,
+            "num_hidden": Config.NUM_HIDDEN_UNITS,
+            "num_layers": Config.NUM_LAYERS,
+            "lstm_hidden_size": Config.LSTM_HIDDEN_SIZE,
         }
 
         policy = build_policy(self.env, network, **network_kwargs)
 
-        with tf.variable_scope('ppo2_model', reuse=tf.AUTO_REUSE):
+        with tf.variable_scope("ppo2_model", reuse=tf.AUTO_REUSE):
             self.trained_policy = policy(1, 1)
         self.trained_policy.load(load_path)
 
         self.one_env = self.env.envs[0]
 
     def find_next_action(self, dict_obs, agents, agent_index):
-
-        network_output, _, _, _ = self.trained_policy.step([dict_obs], evaluate=True)
+        network_output, _, _, _ = self.trained_policy.step(
+            [dict_obs], evaluate=True
+        )
 
         print(network_output)
 
         agent = agents[agent_index]
-        heading = agent.max_heading_change*(2.*network_output[0, 1] - 1.)
+        heading = agent.max_heading_change * (2.0 * network_output[0, 1] - 1.0)
         speed = agent.pref_speed * network_output[0, 0]
         actions = np.array([speed, heading])
         return actions
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRLPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRLPolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3CCADRLPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3CCADRLPolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/LearningPolicyGA3C.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/LearningPolicyGA3C.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/Policy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/Policy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CARRLPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CARRLPolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/StaticPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/StaticPolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/DRLLongPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/DRLLongPolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/LearningPolicy.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/LearningPolicy.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_results_multi.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_results_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 import sys
 import os
 file_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(file_dir+'/../neural_networks')
 
 import numpy as np
-import numpy.matlib
 import pickle
 from mpl_toolkits.mplot3d import Axes3D
 from matplotlib import cm
 import matplotlib.pyplot as plt
 import matplotlib
 import copy
 import time
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/pedData_processing_multi.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/pedData_processing_multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python
-import sys
 import os
+import sys
+
 file_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(file_dir+'/../neural_networks')
 
-import numpy as np
-import numpy.matlib
+import copy
 import pickle
-import matplotlib.pyplot as plt
 import time
+
+import matplotlib.pyplot as plt
+import numpy as np
+
 from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import global_var as gb
-import copy
 
 # setting up global variables
 COLLISION_COST = gb.COLLISION_COST
 DIST_2_GOAL_THRES = gb.DIST_2_GOAL_THRES
 GETTING_CLOSE_PENALTY = gb.GETTING_CLOSE_PENALTY
 GETTING_CLOSE_RANGE = gb.GETTING_CLOSE_RANGE
 EPS = gb.EPS
@@ -379,16 +381,16 @@
 	num_agents = len(others_states) + 1
 	assert(num_agents <= num_agents_in_network)
 	num_rawStates = agent_states.shape[0]
 	states_nn = np.zeros((num_rawStates, 7+8*(num_agents_in_network-1)))
 	for i in range(num_agents-1, num_agents_in_network-1):
 		# states_nn[:,7+8*i:7+8*i+7] = np.matlib.repmat(\
 			# np.array([0.0, 0.0, -8.0, 0.0, 0.35, 0.70, 8.0]), num_rawStates, 1)
-		states_nn[:,7+8*i:7+8*i+7] = np.matlib.repmat(\
-			np.array([-2.0, -2.0, -10, -10.0, -0.2, -0.2, -2.0]), num_rawStates, 1)
+		states_nn[:,7+8*i:7+8*i+7] = np.tile(\
+			np.array([-2.0, -2.0, -10, -10.0, -0.2, -0.2, -2.0]), (num_rawStates, 1))
 
 	# agent
 	# distance to goal
 	goal_direction = agent_states[:,6:8]-agent_states[:,0:2]
 	dist_to_goal = np.clip(np.linalg.norm(goal_direction, axis=1), 0, 30)
 	# desired speed
 	pref_speed = agent_states[:,5]
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_debug_multi.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_debug_multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 import sys
 sys.path.append('../neural_networks')
 
 import numpy as np
-import numpy.matlib
 import pickle
 from mpl_toolkits.mplot3d import Axes3D
 from matplotlib import cm
 import matplotlib.pyplot as plt
 import copy
 import os
 import time
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_rl_multi.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_rl_multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
-import sys
 import os
+import sys
+
 file_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(file_dir+'/../neural_networks')
 
-import numpy as np
-import numpy.matlib
-import pickle
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
-import matplotlib.pyplot as plt
 import copy
+import pickle
 import time
 
+import gen_rand_testcases as gen_tc
+import global_var as gb
+import matplotlib.pyplot as plt
 import neural_network_regr_multi as nn
 import nn_navigation_value_multi as nn_nav
+import numpy as np
 import pedData_processing_multi as pedData
-import global_var as gb
-import gen_rand_testcases as gen_tc
+from matplotlib import cm
+from mpl_toolkits.mplot3d import Axes3D
 
 # setting up global variables
 COLLISION_COST = gb.COLLISION_COST
 DIST_2_GOAL_THRES = gb.DIST_2_GOAL_THRES
 GETTING_CLOSE_PENALTY = gb.GETTING_CLOSE_PENALTY
 GETTING_CLOSE_RANGE = gb.GETTING_CLOSE_RANGE
 EPS = gb.EPS
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_rand_testcases.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_rand_testcases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 #!/usr/bin/env python
 import sys
+
 sys.path.append('../neural_networks')
 
-import numpy as np
-import numpy.matlib
-import pickle
 import copy
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
-import matplotlib.pyplot as plt
 import os
+import pickle
 import time
-import copy
 
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks import neural_network_regr_multi as nn
-from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import pedData_processing_multi as pedData
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.nn_training_param import NN_training_param
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.multiagent_network_param import Multiagent_network_param
-from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import global_var as gb
+import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib import cm
+from mpl_toolkits.mplot3d import Axes3D
 
+from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import global_var as gb
+from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import (
+    pedData_processing_multi as pedData,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks import (
+    neural_network_regr_multi as nn,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.multiagent_network_param import (
+    Multiagent_network_param,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.nn_training_param import (
+    NN_training_param,
+)
 
 # setting up global variables
 COLLISION_COST = gb.COLLISION_COST
 DIST_2_GOAL_THRES = gb.DIST_2_GOAL_THRES
 GETTING_CLOSE_PENALTY = gb.GETTING_CLOSE_PENALTY
 GETTING_CLOSE_RANGE = gb.GETTING_CLOSE_RANGE
 EPS = gb.EPS
@@ -61,15 +68,15 @@
 	critical_dist = end_dist.copy() 
 	# start_dist * np.ones((num_pts,))   # initialize
 	# critical points (where d/dt = 0)
 	z_bar = (x2 - x1) - (y2 - y1)             # shape = (num_actions, 2)
 	inds = np.where((np.linalg.norm(z_bar,axis=1)>0))[0]
 	t_bar = - np.sum((x1-y1) * z_bar[inds,:], axis=1) \
 			/ np.sum(z_bar[inds,:] * z_bar[inds,:], axis=1)
-	t_bar_rep = np.matlib.repmat(t_bar, 2, 1).transpose()
+	t_bar_rep = np.tile(t_bar, (2, 1)).transpose()
 	dist_bar = np.linalg.norm(x1 + (x2[inds,:]-x1) * t_bar_rep \
 			  - y1 - (y2[inds,:]-y1) * t_bar_rep, axis=1)
 	inds_2 = np.where((t_bar > 0) & (t_bar < 1.0))
 	critical_dist[inds[inds_2]] = dist_bar[inds_2] 
 
 	# end_dist = end_dist.clip(min=0, max=start_dist)
 	min_dist = np.amin(np.vstack((end_dist, critical_dist)), axis=0)
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/global_var.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/global_var.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_navigation_value_multi.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_navigation_value_multi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 #!/usr/bin/env python
 import sys
-sys.path.append('../neural_networks')
 
-import numpy as np
-import numpy.matlib
-import pickle
+sys.path.append("../neural_networks")
+
 import copy
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
-import matplotlib.pyplot as plt
 import os
+import pickle
 import time
-import copy
 
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks import neural_network_regr_multi as nn
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.multiagent_network_param import Multiagent_network_param
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.nn_training_param import NN_training_param
-from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import pedData_processing_multi as pedData
-from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import global_var as gb
-from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import gen_rand_testcases as gen_tc
+import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib import cm
+from mpl_toolkits.mplot3d import Axes3D
+
+from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import (
+    gen_rand_testcases as gen_tc,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import (
+    global_var as gb,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.multi import (
+    pedData_processing_multi as pedData,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks import (
+    neural_network_regr_multi as nn,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.multiagent_network_param import (
+    Multiagent_network_param,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.nn_training_param import (
+    NN_training_param,
+)
 
 # setting up global variables
 COLLISION_COST = gb.COLLISION_COST
 DIST_2_GOAL_THRES = gb.DIST_2_GOAL_THRES
 GETTING_CLOSE_PENALTY = gb.GETTING_CLOSE_PENALTY
 GETTING_CLOSE_RANGE = gb.GETTING_CLOSE_RANGE
 EPS = gb.EPS
@@ -33,691 +45,869 @@
 # plotting colors
 plt_colors = gb.plt_colors
 GAMMA = gb.RL_gamma
 DT_NORMAL = gb.RL_dt_normal
 SMOOTH_COST = gb.SMOOTH_COST
 
 # for 'rotate_constr'
-TURNING_LIMIT = np.pi/6.0
+TURNING_LIMIT = np.pi / 6.0
 
-# neural network 
+# neural network
 NN_ranges = gb.NN_ranges
 
+
 # assume no kinematic constraints
 def find_action_grids():
     nom_speed = 1.0
     num_angles = 18
     num_speeds = 5
     angles = np.linspace(0, 2 * np.pi, num_angles, endpoint=False)
     speeds = np.linspace(nom_speed, 0.0, num_speeds, endpoint=False)
-    
+
     angles, speeds = np.meshgrid(angles, speeds)
     angles = np.append([0.0], angles.flatten())
     speeds = np.append([0.0], speeds.flatten())
 
     actions = np.vstack((speeds, angles)).transpose()
-    assert(actions.shape[0] == num_angles*num_speeds + 1)
-    assert(actions.shape[1] == 2)
+    assert actions.shape[0] == num_angles * num_speeds + 1
+    assert actions.shape[1] == 2
 
     # plot (for debugging)
     # fig = plt.figure(frameon=False)
-    x = actions[:,0] * np.cos(actions[:,1])
-    y = actions[:,0] * np.sin(actions[:,1])
+    x = actions[:, 0] * np.cos(actions[:, 1])
+    y = actions[:, 0] * np.sin(actions[:, 1])
     # plt.scatter(x, y, 50, cmap="rainbow")
     # plt.title('discrete actions')
     # plt.draw()
     # plt.show()
 
     return actions
 
+
 # assume min/max acceleration over 1 seconds
 def find_close_actions():
     num_angles = 6
     num_speeds = 4
     nom_speed = 1.0
-    angles = np.linspace(-TURNING_LIMIT, TURNING_LIMIT, num_angles, endpoint=True)
+    angles = np.linspace(
+        -TURNING_LIMIT, TURNING_LIMIT, num_angles, endpoint=True
+    )
     speeds = np.linspace(nom_speed, 0.0, num_speeds, endpoint=False)
-    
+
     angles, speeds = np.meshgrid(angles, speeds)
     angles = np.append([0.0], angles.flatten())
     speeds = np.append([0.0], speeds.flatten())
-    
+
     actions = np.vstack((speeds, angles)).transpose()
     # plot (for debugging)
     # fig = plt.figure(frameon=False)
     # x = actions[:,0] * np.cos(actions[:,1])
     # y = actions[:,0] * np.sin(actions[:,1])
     # plt.scatter(x, y, 50, cmap="rainbow")
     # plt.title('discrete actions')
     # plt.draw()
     # plt.show()
     return actions
 
+
 # angle_1 - angle_2
 # contains direction in range [-3.14, 3.14]
 def find_angle_diff(angle_1, angle_2):
     angle_diff_raw = angle_1 - angle_2
     angle_diff = (angle_diff_raw + np.pi) % (2 * np.pi) - np.pi
     return angle_diff
 
+
 def compute_multi_net_param(num_agents):
     num_others = num_agents - 1
 
     # no max layer
     # layers_type = []
     # layers_info = []
     # layers_info.append(np.array([[1, 7], [num_others, 8] ])); layers_type.append('conn')
     # layers_info.append(np.array([[1, 50], [num_others, 50]])); layers_type.append('conn')
     # layers_info.append(np.array([[1, 50], [num_others, 50]]));  layers_type.append('conn')
-    # layers_info.append(np.array([[1, 50]])); layers_type.append('conn') 
-    # layers_info.append(np.array([[1, 25]])); layers_type.append('conn') 
+    # layers_info.append(np.array([[1, 50]])); layers_type.append('conn')
+    # layers_info.append(np.array([[1, 25]])); layers_type.append('conn')
     # layers_info.append(np.array([[1, 1]]));
 
     # with max layer
     layers_type = []
     layers_info = []
-    layers_info.append(np.array([[1, 7], [num_others, 8] ])); layers_type.append('conn')
-    layers_info.append(np.array([[1, 50], [num_others, 50]])); layers_type.append('conn')
-    layers_info.append(np.array([[1, 50], [num_others, 50]]));  layers_type.append('max')
-    layers_info.append(np.array([[1, 50], [1, 50]]));  layers_type.append('conn')
-    layers_info.append(np.array([[1, 50]]));  layers_type.append('conn')
-    # layers_info.append(np.array([[1, 100]])); layers_type.append('conn') 
-    # layers_info.append(np.array([[1, 25]])); layers_type.append('conn') 
-    layers_info.append(np.array([[1, 1]]));
+    layers_info.append(np.array([[1, 7], [num_others, 8]]))
+    layers_type.append("conn")
+    layers_info.append(np.array([[1, 50], [num_others, 50]]))
+    layers_type.append("conn")
+    layers_info.append(np.array([[1, 50], [num_others, 50]]))
+    layers_type.append("max")
+    layers_info.append(np.array([[1, 50], [1, 50]]))
+    layers_type.append("conn")
+    layers_info.append(np.array([[1, 50]]))
+    layers_type.append("conn")
+    # layers_info.append(np.array([[1, 100]])); layers_type.append('conn')
+    # layers_info.append(np.array([[1, 25]])); layers_type.append('conn')
+    layers_info.append(np.array([[1, 1]]))
 
     # with max and self layer
     # layers_type = []
     # layers_info = []
     # layers_info.append(np.array([[1, 7], [num_others, 8] ])); layers_type.append('self')
     # layers_info.append(np.array([[1, 50], [num_others, 50] ])); layers_type.append('conn')
     # layers_info.append(np.array([[1, 50], [num_others, 50]])); layers_type.append('conn')
     # layers_info.append(np.array([[1, 50], [num_others, 50]]));  layers_type.append('max')
     # layers_info.append(np.array([[1, 50], [1, 50]]));  layers_type.append('conn')
     # layers_info.append(np.array([[1, 50]]));  layers_type.append('conn')
-    # # layers_info.append(np.array([[1, 100]])); layers_type.append('conn') 
-    # # layers_info.append(np.array([[1, 25]])); layers_type.append('conn') 
+    # # layers_info.append(np.array([[1, 100]])); layers_type.append('conn')
+    # # layers_info.append(np.array([[1, 25]])); layers_type.append('conn')
     # layers_info.append(np.array([[1, 1]]));
 
     multi_net_param = Multiagent_network_param(layers_info, layers_type)
     # for layer in range(len(layers_info)-1):
     #   print 'layer', layer
     #   print multi_net_param.symmetric_indices[layer]
     # raw_input()
     # print multi_net_param.symmetric_indices_b
     # raw_input()
     return layers_info, layers_type, multi_net_param
 
+
 def find_nn_ranges(num_agents, NN_ranges):
-    num_states = 7 + 8 * (num_agents-1)
-    input_avg_vec = np.zeros((num_states,)); input_avg_vec[0:7] = NN_ranges[0][0].copy()
-    input_std_vec = np.zeros((num_states,)); input_std_vec[0:7] = NN_ranges[1][0].copy()
-    for i in range(num_agents-1):
+    num_states = 7 + 8 * (num_agents - 1)
+    input_avg_vec = np.zeros((num_states,))
+    input_avg_vec[0:7] = NN_ranges[0][0].copy()
+    input_std_vec = np.zeros((num_states,))
+    input_std_vec[0:7] = NN_ranges[1][0].copy()
+    for i in range(num_agents - 1):
         a = 7 + 8 * i
-        b = 7 + 8 * (i+1)
+        b = 7 + 8 * (i + 1)
         input_avg_vec[a:b] = NN_ranges[0][1].copy()
         input_std_vec[a:b] = NN_ranges[1][1].copy()
     output_avg_vec = NN_ranges[2]
     output_std_vec = NN_ranges[3]
 
     NN_ranges_processed = []
-    NN_ranges_processed.append(input_avg_vec); NN_ranges_processed.append(input_std_vec)
-    NN_ranges_processed.append(output_avg_vec); NN_ranges_processed.append(output_std_vec)
+    NN_ranges_processed.append(input_avg_vec)
+    NN_ranges_processed.append(input_std_vec)
+    NN_ranges_processed.append(output_avg_vec)
+    NN_ranges_processed.append(output_std_vec)
     return NN_ranges_processed
 
 
 class NN_navigation_value:
-    def __init__(self, num_agents, nn_training_param, mode='no_constr', passing_side='none'):
+    def __init__(
+        self,
+        num_agents,
+        nn_training_param,
+        mode="no_constr",
+        passing_side="none",
+    ):
         self.num_agents = num_agents
         self.nn_training_param = nn_training_param
         self.nn = nn.Neural_network_regr_multi(self.nn_training_param)
         self.current_value = 0
         self.plot_actions = find_action_grids()
         self.close_actions = find_close_actions()
         self.test_vel_data = None
         self.dt_forward = 1.0
-        self.radius_buffer = 0.0 # buffer around collision radius
+        self.radius_buffer = 0.0  # buffer around collision radius
         self.mode = mode
         self.passing_side = passing_side
-        self.training_passing_side_weight = 0.5 #0.7 #0.2
+        self.training_passing_side_weight = 0.5  # 0.7 #0.2
         self.old_value_net = None
 
     # setup neural network
     def initialize_nn(self, num_agents):
-        layers_info, layers_type, multi_net_param = compute_multi_net_param(num_agents)
-        self.nn.initialize_network_param(layers_info, layers_type, multiagent_net_param=multi_net_param)
-
-
-    def train_neural_network(self, training_data, test_data, test_vel_data=None):
-        if not hasattr(self.nn, 'W'):
+        layers_info, layers_type, multi_net_param = compute_multi_net_param(
+            num_agents
+        )
+        self.nn.initialize_network_param(
+            layers_info, layers_type, multiagent_net_param=multi_net_param
+        )
+
+    def train_neural_network(
+        self, training_data, test_data, test_vel_data=None
+    ):
+        if not hasattr(self.nn, "W"):
             self.initialize_nn(self.num_agents)
 
         # for plotting
         self.test_vel_data = test_vel_data
         self.nn.set_plotting_func(self.plot_ped_testCase_rand, test_data[0])
         # initialize neural network
         ERM = 0
         # self.nn.set_training_stepsize('sqrt_decay', 1.0, 0.1)
         # self.nn.set_training_stepsize('sum_of_grad', 0.1, 0.1)
-        self.nn.set_training_stepsize('rmsprop', 0.1, 0.1)
+        self.nn.set_training_stepsize("rmsprop", 0.1, 0.1)
         NN_ranges_processed = find_nn_ranges(self.num_agents, NN_ranges)
-        self.nn.train_nn(training_data, ERM, test_data, input_output_ranges=NN_ranges_processed)
+        self.nn.train_nn(
+            training_data,
+            ERM,
+            test_data,
+            input_output_ranges=NN_ranges_processed,
+        )
         self.test_vel_data = None
 
     def plot_ped_testCase_rand(self, X, Y_hat, title_string, figure_name=None):
         # Y_hat = [value]
         ind = np.random.randint(0, X.shape[0])
         # ind = 5
-        x = X[ind,:]
-        y_hat = Y_hat[ind,:]
+        x = X[ind, :]
+        y_hat = Y_hat[ind, :]
         if (self.test_vel_data is None) or (ind > self.test_vel_data.shape[0]):
             y = None
         else:
-            y = self.test_vel_data[ind,:]
+            y = self.test_vel_data[ind, :]
         self.plot_ped_testCase(x, y_hat, title_string, figure_name, y)
 
-    def plot_ped_testCase(self, x, y_hat, title_string, figure_name, y=None, plt_colors_custom=None):
+    def plot_ped_testCase(
+        self,
+        x,
+        y_hat,
+        title_string,
+        figure_name,
+        y=None,
+        plt_colors_custom=None,
+    ):
         # print x.shape
         # print y_hat.shape
         # print y
         # raw_input()
         # new figure
         if figure_name is None:
             fig = plt.figure(figsize=(15, 6), frameon=False)
         else:
-            fig = plt.figure(figure_name,figsize=(15, 6), frameon=False)
+            fig = plt.figure(figure_name, figsize=(15, 6), frameon=False)
             plt.clf()
 
         if plt_colors_custom is None:
             plt_colors_local = plt_colors
         else:
             plt_colors_local = plt_colors_custom
 
         # convert to representation that's easier to plot
-        a_s, other_agent_states = pedData.agentCentricState_2_rawState_noRotate(x)
+        a_s, other_agent_states = (
+            pedData.agentCentricState_2_rawState_noRotate(x)
+        )
         # print 'x', x
         # print 'a_s', a_s
         # print 'len(other_agent_states)', len(other_agent_states)
         # print a_s
         # print len(other_agent_states)
         # print other_agent_states
         # raw_input()
 
         # subfigure 1
         ax = fig.add_subplot(1, 2, 1)
         # agent at (0,0)
-        circ1 = plt.Circle((0.0, 0.0), radius=a_s[8], fc='w', ec=plt_colors_local[0])
+        circ1 = plt.Circle(
+            (0.0, 0.0), radius=a_s[8], fc="w", ec=plt_colors_local[0]
+        )
         ax.add_patch(circ1)
         # goal
-        plt.plot(a_s[6], a_s[7], c=plt_colors_local[0], marker='*', markersize=20)
+        plt.plot(
+            a_s[6], a_s[7], c=plt_colors_local[0], marker="*", markersize=20
+        )
         # pref speed
-        plt.arrow(0.0, 0.0, a_s[5], 0.0, fc='m', ec='m', head_width=0.05, head_length=0.1)
-        vel_pref, = plt.plot([0.0, a_s[5]], [0.0, 0.0], 'm', linewidth=2)
+        plt.arrow(
+            0.0,
+            0.0,
+            a_s[5],
+            0.0,
+            fc="m",
+            ec="m",
+            head_width=0.05,
+            head_length=0.1,
+        )
+        (vel_pref,) = plt.plot([0.0, a_s[5]], [0.0, 0.0], "m", linewidth=2)
         # current speed
-        plt.arrow(0.0, 0.0, a_s[2], a_s[3], fc='k', ec='k', head_width=0.05, head_length=0.1)
-        vel_cur, = plt.plot([0.0, a_s[2]], [0.0,  a_s[3]], 'k', linewidth=2)
-
+        plt.arrow(
+            0.0,
+            0.0,
+            a_s[2],
+            a_s[3],
+            fc="k",
+            ec="k",
+            head_width=0.05,
+            head_length=0.1,
+        )
+        (vel_cur,) = plt.plot([0.0, a_s[2]], [0.0, a_s[3]], "k", linewidth=2)
 
         # actual speed
         if y != None:
-            x_vel = y[0] 
-            y_vel = y[1] 
-            plt.arrow(0.0, 0.0, x_vel, y_vel,  fc=plt_colors_local[0], \
-                ec=plt_colors_local[0], head_width=0.05, head_length=0.1)
-            vel_select, = plt.plot([0.0, x_vel], [0.0, y_vel], \
-                c=plt_colors_local[0], linewidth=2)
+            x_vel = y[0]
+            y_vel = y[1]
+            plt.arrow(
+                0.0,
+                0.0,
+                x_vel,
+                y_vel,
+                fc=plt_colors_local[0],
+                ec=plt_colors_local[0],
+                head_width=0.05,
+                head_length=0.1,
+            )
+            (vel_select,) = plt.plot(
+                [0.0, x_vel], [0.0, y_vel], c=plt_colors_local[0], linewidth=2
+            )
 
         # other agents
         for i, o_s in enumerate(other_agent_states):
-            circ = plt.Circle((o_s[0], o_s[1]), radius=o_s[8], fc='w', ec=plt_colors_local[i+1])
+            circ = plt.Circle(
+                (o_s[0], o_s[1]),
+                radius=o_s[8],
+                fc="w",
+                ec=plt_colors_local[i + 1],
+            )
             ax.add_patch(circ)
             # other agent's speed
-            plt.arrow(o_s[0], o_s[1], o_s[2], o_s[3], fc=plt_colors_local[i+1], \
-                ec=plt_colors_local[i+1], head_width=0.05, head_length=0.1)
+            plt.arrow(
+                o_s[0],
+                o_s[1],
+                o_s[2],
+                o_s[3],
+                fc=plt_colors_local[i + 1],
+                ec=plt_colors_local[i + 1],
+                head_width=0.05,
+                head_length=0.1,
+            )
             # vel_other, = plt.plot([o_s[0], o_s[0]+o_s[2]], [o_s[1], o_s[1]+o_s[3]], \
             #   c=plt_colors_local[i+1], linewidth=2)
-        
+
         # meta data
         agent_state = a_s
         action = self.find_next_action(agent_state, other_agent_states)
-        x_tmp = action[0] * np.cos(action[1]) 
+        x_tmp = action[0] * np.cos(action[1])
         y_tmp = action[0] * np.sin(action[1])
-        plt.arrow(0.0, 0.0, x_tmp, y_tmp, fc='g',\
-            ec='g', head_width=0.05, head_length=0.1)
-        vel_nn, = plt.plot([0.0, x_tmp], [0.0, y_tmp], 'g-', linewidth=2)
-        value = self.find_next_states_values(agent_state, action.reshape([1,2]), other_agent_states)
+        plt.arrow(
+            0.0,
+            0.0,
+            x_tmp,
+            y_tmp,
+            fc="g",
+            ec="g",
+            head_width=0.05,
+            head_length=0.1,
+        )
+        (vel_nn,) = plt.plot([0.0, x_tmp], [0.0, y_tmp], "g-", linewidth=2)
+        value = self.find_next_states_values(
+            agent_state, action.reshape([1, 2]), other_agent_states
+        )
         # plt.title(title_string + '; pred_value: %f, true_value: %f' % \
         #   (y_hat[0], y[0]))
-        plt.xlabel('x (m)')
-        plt.ylabel('y (m)')
-        dist_2_other_agents = np.zeros((len(other_agent_states), ))
+        plt.xlabel("x (m)")
+        plt.ylabel("y (m)")
+        dist_2_other_agents = np.zeros((len(other_agent_states),))
         for i, other_agent_state in enumerate(other_agent_states):
-            dist_2_other_agents[i] = np.linalg.norm(agent_state[0:2]-other_agent_state[0:2]) - \
-                            agent_state[8] - other_agent_state[8]
+            dist_2_other_agents[i] = (
+                np.linalg.norm(agent_state[0:2] - other_agent_state[0:2])
+                - agent_state[8]
+                - other_agent_state[8]
+            )
         dist_2_other_agent = np.min(dist_2_other_agents)
         # print 'dist_2_other_agents', dist_2_other_agents
         # print 'dist_2_other_agent', dist_2_other_agent
         # raw_input()
-        plt.title(title_string + '\n pref_speed: %.3f, min_dist_2_others: %.3f' % \
-                                (a_s[5],dist_2_other_agent))
+        plt.title(
+            title_string
+            + "\n pref_speed: %.3f, min_dist_2_others: %.3f"
+            % (a_s[5], dist_2_other_agent)
+        )
         # if y != None:
         #   plt.legend([vel_pref, vel_cur,vel_other, vel_select, vel_nn], \
         #       ['vel_pref', 'vel_cur', 'vel_other', 'vel_select', 'vel_nn'])
         # else:
         #   plt.legend([vel_pref, vel_cur, vel_other, vel_nn], \
         #       ['vel_pref', 'vel_cur', 'vel_other', 'vel_nn'])
-        plt.legend([vel_cur, vel_pref, vel_nn], \
-                ['${heading}$', '$v_{pref}$','$v_{select}$'], \
-                loc='lower left', fontsize=30, frameon=False)
-    
-        ax.axis('equal')
+        plt.legend(
+            [vel_cur, vel_pref, vel_nn],
+            ["${heading}$", "$v_{pref}$", "$v_{select}$"],
+            loc="lower left",
+            fontsize=30,
+            frameon=False,
+        )
+
+        ax.axis("equal")
         xlim = ax.get_xlim()
-        new_xlim = np.array((xlim[0], xlim[1]+0.5))
+        new_xlim = np.array((xlim[0], xlim[1] + 0.5))
         ax.set_xlim(new_xlim)
         # plotting style (only show axis on bottom and left)
-        ax.spines['top'].set_visible(False)
-        ax.spines['right'].set_visible(False)
-        ax.yaxis.set_ticks_position('left')
-        ax.xaxis.set_ticks_position('bottom')
+        ax.spines["top"].set_visible(False)
+        ax.spines["right"].set_visible(False)
+        ax.yaxis.set_ticks_position("left")
+        ax.xaxis.set_ticks_position("bottom")
 
         # second subfigure
         # ax = fig.add_subplot(1, 2, 2, projection='3d')
         ax = fig.add_subplot(1, 2, 2)
         # print 'before', agent_state
         # agent_state, other_agent_states = \
         #       pedData.agentCentricState_2_rawState_noRotate(x)
         # print 'after', agent_state
-        if self.mode == 'no_constr':
-            ''' all possible actions '''
-            ''' actions choice 1 '''
+        if self.mode == "no_constr":
+            """all possible actions"""
+            """ actions choice 1 """
             default_action_xy = agent_state[2:4]
             speed = np.linalg.norm(default_action_xy)
-            angle_select = np.arctan2(default_action_xy[1], default_action_xy[0])
+            angle_select = np.arctan2(
+                default_action_xy[1], default_action_xy[0]
+            )
 
             # default_action_theta = np.array([speed, angle_select])
             # actions = self.find_actions_theta(agent_state, default_action_theta)
-            
+
             # circular for plotting
             actions = self.plot_actions.copy()
-            actions[:,1] = (actions[:,1] + np.pi) % (2 * np.pi) - np.pi
-            actions[:,0] *= a_s[5]
+            actions[:, 1] = (actions[:, 1] + np.pi) % (2 * np.pi) - np.pi
+            actions[:, 0] *= a_s[5]
             # turning needs to be slower
             # angle_diff_abs = abs(find_angle_diff(actions[:,1],agent_state[4]))
             # actions[:,0] *= (1 - angle_diff_abs / (2*np.pi))
-        elif self.mode == 'rotate_constr':
-            ''' dynamically feasible actions '''
+        elif self.mode == "rotate_constr":
+            """dynamically feasible actions"""
             # print 'x', x
             # print 'agent_state', agent_state
             # print 'other_agent_state', other_agent_state
-            cur_heading = agent_state[4]; desired_speed = agent_state[5]
+            cur_heading = agent_state[4]
+            desired_speed = agent_state[5]
             actions = self.close_actions.copy()
-            actions[:,0] *= desired_speed
-            print('rotate_constr')
-            actions[:,1] = actions[:,1] + cur_heading
-            actions[:,1] = (actions[:,1] + np.pi) % (2 * np.pi) - np.pi
+            actions[:, 0] *= desired_speed
+            print("rotate_constr")
+            actions[:, 1] = actions[:, 1] + cur_heading
+            actions[:, 1] = (actions[:, 1] + np.pi) % (2 * np.pi) - np.pi
             # actions = self.find_actions_theta_dynConstr(agent_state, 1.0)
             # print cur_heading
         else:
-            assert(0)
+            assert 0
 
-        
         # agent_state, other_agent_state = \
-            # pedData.agentCentricState_2_rawState_noRotate(x)
+        # pedData.agentCentricState_2_rawState_noRotate(x)
         # actions, accels_theta = self.find_actions_theta_dynConstr(agent_state, 1.0)
-        
-        plot_x = actions[:,0] * np.cos(actions[:,1])
-        plot_y = actions[:,0] * np.sin(actions[:,1])
+
+        plot_x = actions[:, 0] * np.cos(actions[:, 1])
+        plot_y = actions[:, 0] * np.sin(actions[:, 1])
         # assert(0)
         # print 'before, agent state', agent_state
         # print 'before, other_agent state',other_agent_state
 
         # print 'after, agent state', agent_state
         # print 'after, other_agent state', other_agent_state
-        plot_z = self.find_next_states_values(agent_state, actions, other_agent_states)
+        plot_z = self.find_next_states_values(
+            agent_state, actions, other_agent_states
+        )
         # print actions.shape, plot_x.shape
         # print np.hstack((actions, plot_z.reshape(plot_z.shape[0], 1)))
         value = np.amax(plot_z)
         ind = np.argmax(plot_z)
         x_tmp = actions[ind, 0] * np.cos(actions[ind, 1])
         y_tmp = actions[ind, 0] * np.sin(actions[ind, 1])
-        ''' plot using plot_trisurf (2D view of a 3D plot)'''
+        """ plot using plot_trisurf (2D view of a 3D plot)"""
         # print plot_x.shape, plot_y.shape, plot_z.shape
         # ax = fig.gca(projection='3d')
         # im = ax.plot_trisurf(plot_x, plot_y, plot_z, cmap=cm.jet, linewidth=0.2)
         # ax.view_init(90.0, 270.0)
         # plt.title('value of best action: %.3f' % value)
         # fig.colorbar(im, shrink=0.5)
-        
-        ''' plot using tripcolor (2D plot) '''
+
+        """ plot using tripcolor (2D plot) """
         # triang = tri.Triangulation(plot_x, plot_y)
-        color_min_inds = np.where(plot_z>0)[0]
+        color_min_inds = np.where(plot_z > 0)[0]
         if len(color_min_inds) > 0:
             color_min = np.amin(plot_z[color_min_inds]) - 0.05
         else:
             color_min = 0.0
-        color_max = max(np.amax(plot_z),0.0)
+        color_max = max(np.amax(plot_z), 0.0)
         # plt.tripcolor(plot_x, plot_y, plot_z, shading='flat', \
         #       cmap=plt.cm.rainbow, edgecolors='k',vmin=color_min, vmax=color_max)
-        plt.tripcolor(plot_x, plot_y, plot_z, shading='flat', \
-                cmap=plt.cm.rainbow, vmin=color_min, vmax=color_max)
+        plt.tripcolor(
+            plot_x,
+            plot_y,
+            plot_z,
+            shading="flat",
+            cmap=plt.cm.rainbow,
+            vmin=color_min,
+            vmax=color_max,
+        )
         if actions[ind, 0] > EPS:
-            plt.title('value of best action: %.3f \n action_x %.3f, action_y %.3f' \
-                % (value, x_tmp, y_tmp))
+            plt.title(
+                "value of best action: %.3f \n action_x %.3f, action_y %.3f"
+                % (value, x_tmp, y_tmp)
+            )
         else:
-            plt.title('value of best action: %.3f \n action_speed %.3f, action_angle %.3f' \
-                % (value, actions[ind, 0], actions[ind, 1]))
-        plt.xlabel('v_x (m/s)')
-        plt.ylabel('v_y (m/s)')
+            plt.title(
+                "value of best action: %.3f \n action_speed %.3f, action_angle"
+                " %.3f" % (value, actions[ind, 0], actions[ind, 1])
+            )
+        plt.xlabel("v_x (m/s)")
+        plt.ylabel("v_y (m/s)")
         cbar = plt.colorbar()
-        cbar.set_ticks([color_min,(color_min+color_max)/2.0,color_max])
-        cbar.ax.set_yticklabels(['%.3f'%color_min, \
-                            '%.3f'%((color_min+color_max)/2.0), \
-                            '%.3f'%color_max])
+        cbar.set_ticks([color_min, (color_min + color_max) / 2.0, color_max])
+        cbar.ax.set_yticklabels(
+            [
+                "%.3f" % color_min,
+                "%.3f" % ((color_min + color_max) / 2.0),
+                "%.3f" % color_max,
+            ]
+        )
 
         # plotting style (only show axis on bottom and left)
-        ax.spines['top'].set_visible(False)
-        ax.spines['right'].set_visible(False)
-        ax.yaxis.set_ticks_position('left')
-        ax.xaxis.set_ticks_position('bottom')
+        ax.spines["top"].set_visible(False)
+        ax.spines["right"].set_visible(False)
+        ax.yaxis.set_ticks_position("left")
+        ax.xaxis.set_ticks_position("bottom")
 
         plt.draw()
         plt.pause(0.0001)
         # raw_input()
 
     def find_actions_theta(self, agent_state, default_action_theta):
         # action = [speed theta]
         num_near_actions = 10
         num_rand_actions = 5
 
         # zero action
-        zero_action = np.zeros((1,2))
+        zero_action = np.zeros((1, 2))
 
         # desired action
         # cur_state = agent_state[0:2]
         # goal = agent_state[6:8]
         # nom_speed = agent_state[5]
         # desired_act = self.computePrefVel(cur_state, goal, nom_speed)
-        desired_act = np.array([agent_state[5], \
-                        np.arctan2(agent_state[7]-agent_state[1], \
-                                agent_state[6]-agent_state[0])])
-        desired_actions = np.matlib.repmat(desired_act, 5, 1)
-        desired_actions[1,0] *= 0.80 
-        desired_actions[2,0] *= 0.60
-        desired_actions[3,0] *= 0.40 
-        desired_actions[4,0] *= 0.20
+        desired_act = np.array(
+            [
+                agent_state[5],
+                np.arctan2(
+                    agent_state[7] - agent_state[1],
+                    agent_state[6] - agent_state[0],
+                ),
+            ]
+        )
+        desired_actions = np.tile(desired_act, (5, 1))
+        desired_actions[1, 0] *= 0.80
+        desired_actions[2, 0] *= 0.60
+        desired_actions[3, 0] *= 0.40
+        desired_actions[4, 0] *= 0.20
 
         # near by actions: default action with perturbed action & reduced speed
         tmp_action_theta = default_action_theta.copy()
         # tmp_action_theta[0] = np.amax((0.75 * desired_act[0], default_action_theta[0]))
         tmp_action_theta[0] = agent_state[5]
         # tmp_action_theta[1] = desired_act[1]
-        near_actions = np.matlib.repmat(tmp_action_theta, num_near_actions, 1)
-        near_actions[:,1] += np.linspace(-np.pi/3.0, np.pi/3.0, num=num_near_actions)
-
+        near_actions = np.tile(tmp_action_theta, (num_near_actions, 1))
+        near_actions[:, 1] += np.linspace(
+            -np.pi / 3.0, np.pi / 3.0, num=num_near_actions
+        )
 
         near_actions_reduced = near_actions.copy()
         near_actions_reduced_1 = near_actions.copy()
         near_actions_reduced_2 = near_actions.copy()
-        near_actions_reduced[:,0] *= 0.75 #0.75
-        near_actions_reduced_1[:,0] *= 0.50 #0.75
-        near_actions_reduced_2[:,0] *= 0.25 #0.75
+        near_actions_reduced[:, 0] *= 0.75  # 0.75
+        near_actions_reduced_1[:, 0] *= 0.50  # 0.75
+        near_actions_reduced_2[:, 0] *= 0.25  # 0.75
 
         # near_actions = np.vstack((near_actions, near_actions_reduced))
-        near_actions = np.vstack((near_actions, near_actions_reduced, \
-            near_actions_reduced_1, near_actions_reduced_2))
+        near_actions = np.vstack(
+            (
+                near_actions,
+                near_actions_reduced,
+                near_actions_reduced_1,
+                near_actions_reduced_2,
+            )
+        )
 
         # random actions: random actions with max speed at desired speed
         # pref_speed = agent_state[5]
         # rand_actions = np.zeros((num_rand_actions, 2))
         # rand_actions[:,0] = pref_speed * np.random.rand(num_rand_actions,)
         # rand_actions[:,1] = 2 * np.pi * np.random.rand(num_rand_actions,) - np.pi
 
-
-
         # put all actions together
-        actions = np.vstack((default_action_theta, desired_actions, \
-                            zero_action, near_actions)) #, rand_actions))
+        actions = np.vstack(
+            (default_action_theta, desired_actions, zero_action, near_actions)
+        )  # , rand_actions))
 
         # avoid oscillation
         # angles_diff = find_angle_diff(actions[:,1], agent_state[4])
         # if agent_state[9] > EPS:
         #   valid_inds = np.where(angles_diff > -EPS)[0]
         #   actions = actions[valid_inds,:]
         # elif agent_state[9] < -EPS:
         #   valid_inds = np.where(angles_diff < EPS)[0]
         #   actions = actions[valid_inds,:]
 
-
         # plot_actions = self.plot_actions.copy()
         # plot_actions[:,1] += default_action_theta[1]
         # plot_actions[:,0] *= agent_state[5]
         # actions = np.vstack((default_action_theta, desired_actions, \
-                            # plot_actions))
+        # plot_actions))
         # actions = np.vstack((default_action_theta, zero_action, near_actions, rand_actions))
-        actions[:,1] = (actions[:,1] + np.pi) % (np.pi * 2) - np.pi
+        actions[:, 1] = (actions[:, 1] + np.pi) % (np.pi * 2) - np.pi
 
         # turning needs to be slower
         # angle_diff_abs = abs(find_angle_diff(actions[:,1],agent_state[4]))
         # actions[:,0] *= (1 - angle_diff_abs / (2*np.pi))
         return actions
 
     def find_actions_theta_dynConstr(self, agent_state, dt):
-        assert(dt > 0.9)
-        angle_lim = TURNING_LIMIT*min(dt,1.0)
+        assert dt > 0.9
+        angle_lim = TURNING_LIMIT * min(dt, 1.0)
         # action = [speed theta]
         cur_heading = agent_state[4]
         desired_speed = agent_state[5]
 
         # near by actions: default action
         num_near_actions = 10
         cur_speed = np.linalg.norm(agent_state[2:4])
         actions = self.close_actions.copy()
         # actions[:,0] *= max(0.75 * desired_speed, cur_speed)
-        actions[:,0] *= desired_speed
-        actions[:,1] = actions[:,1] + cur_heading
+        actions[:, 0] *= desired_speed
+        actions[:, 1] = actions[:, 1] + cur_heading
 
         # desired action: add if desired_heading is within reachable range
         # of cur_heading
-        desired_heading = np.arctan2(agent_state[7]-agent_state[1], \
-                                agent_state[6]-agent_state[0])
+        desired_heading = np.arctan2(
+            agent_state[7] - agent_state[1], agent_state[6] - agent_state[0]
+        )
         angle_diff_abs = abs(find_angle_diff(desired_heading, cur_heading))
-        if  angle_diff_abs < angle_lim:
+        if angle_diff_abs < angle_lim:
             desired_act = np.array([desired_speed, desired_heading])
-            desired_actions = np.matlib.repmat(desired_act, 5, 1)
-            desired_actions[1,0] *= 0.80 
-            desired_actions[2,0] *= 0.60
-            desired_actions[3,0] *= 0.40 
-            desired_actions[4,0] *= 0.20
+            desired_actions = np.tile(desired_act, (5, 1))
+            desired_actions[1, 0] *= 0.80
+            desired_actions[2, 0] *= 0.60
+            desired_actions[3, 0] *= 0.40
+            desired_actions[4, 0] *= 0.20
             # put all actions together
             actions = np.vstack((desired_actions, actions))
             # print '---- desired actions added'
-        
+
         # default action: add if default_heading is within reachable range
         # of cur_heading
         default_heading = np.arctan2(agent_state[3], agent_state[2])
         angle_diff_abs = abs(find_angle_diff(default_heading, cur_heading))
-        if  angle_diff_abs < angle_lim and cur_speed > 0.05:
+        if angle_diff_abs < angle_lim and cur_speed > 0.05:
             default_act = np.array([cur_speed, default_heading])
-            default_actions = np.matlib.repmat(default_act, 2, 1)
-            default_actions[1,0] *= 0.75 
+            default_actions = np.tile(default_act, (2, 1))
+            default_actions[1, 0] *= 0.75
             # put all actions together
             actions = np.vstack((default_actions, actions))
             # print '---- default actions added'
 
         # turning on spot
         # min_turning_radius = 0.5
         limit = TURNING_LIMIT
         # print 'desired_speed, dt, limit', desired_speed, dt, limit
         # print 'dt', dt
-        added_actions = np.array([[0.0, limit + cur_heading], \
-                [0.0, 0.66 * limit + cur_heading], \
-                [0.0, 0.33 * limit + cur_heading], \
-                [0.0, -0.33 * limit + cur_heading], \
-                [0.0, -0.66 * limit + cur_heading], \
-                [0.0, -limit + cur_heading]])
+        added_actions = np.array(
+            [
+                [0.0, limit + cur_heading],
+                [0.0, 0.66 * limit + cur_heading],
+                [0.0, 0.33 * limit + cur_heading],
+                [0.0, -0.33 * limit + cur_heading],
+                [0.0, -0.66 * limit + cur_heading],
+                [0.0, -limit + cur_heading],
+            ]
+        )
         actions = np.vstack((actions, added_actions))
-        
 
         # getting unique rows
         # print 'before', actions
         actions = np.asarray(np.vstack([tuple(row) for row in actions]))
         # raw_input()
         # print 'after', actions
         # raw_input()
-        actions[:,1] = (actions[:,1] + np.pi) % (np.pi * 2) - np.pi
+        actions[:, 1] = (actions[:, 1] + np.pi) % (np.pi * 2) - np.pi
 
         # turning needs to be slower
         # angle_diff_abs = abs(find_angle_diff(actions[:,1],agent_state[4]))
         # actions[:,0] *= (1 - angle_diff_abs / (2*np.pi))
 
         return actions
 
     # cost of action (smoothness)
     def find_state_action_cost(self, agent_state, actions_theta, dt_forward):
         cur_heading = agent_state[4]
-        angle_diff = find_angle_diff(actions_theta[:,1], cur_heading)
-        speed_diff = (actions_theta[:,0] - np.linalg.norm(agent_state[2:4]))
-        
+        angle_diff = find_angle_diff(actions_theta[:, 1], cur_heading)
+        speed_diff = actions_theta[:, 0] - np.linalg.norm(agent_state[2:4])
+
         # bias turning right early on
         # left_inds = np.where((angle_diff>0))[0]
         # angle_diff_abs = angle_diff
         # if np.linalg.norm(agent_state[0:2]-agent_state[6:8]) > 3.0:
         #   angle_diff_abs[left_inds] = 1.0 * abs(angle_diff[left_inds])
         # else:
         #   angle_diff_abs[left_inds] = abs(angle_diff[left_inds])
 
         # right_inds = np.where((angle_diff<0))[0]
         # angle_diff_abs[right_inds] = abs(angle_diff[right_inds])
         angle_diff_abs = abs(angle_diff) / np.pi
-        zero_inds = np.where((actions_theta[:,1] < EPS) | (angle_diff_abs < np.pi/12.0) )[0]
+        zero_inds = np.where(
+            (actions_theta[:, 1] < EPS) | (angle_diff_abs < np.pi / 12.0)
+        )[0]
         angle_diff_abs[zero_inds] = 0
 
         speed_diff_abs = abs(speed_diff) / agent_state[5]
-        zero_inds = np.where( (speed_diff_abs < 0.5) )[0]
+        zero_inds = np.where((speed_diff_abs < 0.5))[0]
         speed_diff_abs[zero_inds] = 0
 
-
         # print 'angle_diff', angle_diff
         # print 'angle_diff_abs', angle_diff_abs
         # print 'speed_diff', speed_diff
         # print 'speed_diff_abs', speed_diff_abs
-        assert(SMOOTH_COST < 0)
+        assert SMOOTH_COST < 0
 
-        cost = np.clip(angle_diff_abs * SMOOTH_COST, -0.25, 0) + \
-            np.clip(speed_diff_abs * SMOOTH_COST, -0.25, 0)
+        cost = np.clip(angle_diff_abs * SMOOTH_COST, -0.25, 0) + np.clip(
+            speed_diff_abs * SMOOTH_COST, -0.25, 0
+        )
         # cost = np.clip(cost, -0.5, 0.0)
         # print cost
 
         d = np.linalg.norm(agent_state[0:2] - agent_state[6:8])
         v = agent_state[5]
-        getting_close_penalty = abs(GAMMA ** (d/DT_NORMAL) * (1.0 - GAMMA ** (-v/DT_NORMAL)))
-        assert(np.all(cost <= 0))
+        getting_close_penalty = abs(
+            GAMMA ** (d / DT_NORMAL) * (1.0 - GAMMA ** (-v / DT_NORMAL))
+        )
+        assert np.all(cost <= 0)
         # return cost
         smoothness_cost = cost * getting_close_penalty
         # print smoothness_cost
         # raw_input()
         return smoothness_cost
 
-
     # limited to this application
-    # future implementation should generalize 
-    def find_action_rewards(self, agent_state, cur_dist, min_dists, dt_forward):
+    # future implementation should generalize
+    def find_action_rewards(
+        self, agent_state, cur_dist, min_dists, dt_forward
+    ):
         # print 'cur_dist', cur_dist
         # print 'min_dists', min_dists
         rewards = np.zeros((len(min_dists),))
         # collision
         if cur_dist < 0:
             rewards[:] = COLLISION_COST
             return rewards
 
         d = np.linalg.norm(agent_state[0:2] - agent_state[6:8])
         v = agent_state[5]
-        getting_close_penalty = GAMMA ** (d/DT_NORMAL) * (1.0 - GAMMA ** (-v/DT_NORMAL))
-        
+        getting_close_penalty = GAMMA ** (d / DT_NORMAL) * (
+            1.0 - GAMMA ** (-v / DT_NORMAL)
+        )
+
         # getting to close
-        close_inds = np.where((min_dists > 0) & \
-            (min_dists < GETTING_CLOSE_RANGE))[0]
+        close_inds = np.where(
+            (min_dists > 0) & (min_dists < GETTING_CLOSE_RANGE)
+        )[0]
 
         # current pos
         if cur_dist < GETTING_CLOSE_RANGE:
-            assert(GETTING_CLOSE_RANGE - cur_dist > 0)
+            assert GETTING_CLOSE_RANGE - cur_dist > 0
             rewards[:] = getting_close_penalty
-        
-        # future pos 
+
+        # future pos
         rewards[close_inds] += getting_close_penalty
 
         collision_inds = np.where(min_dists < 0)[0]
         rewards[collision_inds] = COLLISION_COST
-        
 
         # rewards[close_inds] = rewards[close_inds] + GETTING_CLOSE_PENALTY \
         #   - 0.3 * (GETTING_CLOSE_RANGE - min_dists[close_inds])
 
         scaling_cur = 2
         scaling_future = 5
         # scaling_future = 20
-        rewards[close_inds] = scaling_cur * rewards[close_inds] \
-            + scaling_future * getting_close_penalty * (GETTING_CLOSE_RANGE - min_dists[close_inds])
+        rewards[close_inds] = scaling_cur * rewards[
+            close_inds
+        ] + scaling_future * getting_close_penalty * (
+            GETTING_CLOSE_RANGE - min_dists[close_inds]
+        )
+
+        rewards[close_inds] = np.clip(
+            rewards[close_inds], COLLISION_COST + 0.01, 0.0
+        )
+        assert np.all(GETTING_CLOSE_RANGE - min_dists[close_inds] > 0)
 
-        rewards[close_inds] = np.clip(rewards[close_inds], COLLISION_COST+0.01, 0.0)
-        assert(np.all(GETTING_CLOSE_RANGE - min_dists[close_inds]>0))
-
-        # other states are 
+        # other states are
         return rewards
 
-    
-    def find_passing_side_cost(self, agent_state, actions_theta, other_agents_state, \
-        other_agents_action_theta, dt_forward):
+    def find_passing_side_cost(
+        self,
+        agent_state,
+        actions_theta,
+        other_agents_state,
+        other_agents_action_theta,
+        dt_forward,
+    ):
         weight = self.training_passing_side_weight
         # print weight
         num_pts = len(actions_theta)
 
-
-        num_states = 7 + 8 * (self.num_agents-1)
+        num_states = 7 + 8 * (self.num_agents - 1)
         agent_centric_states = np.zeros((num_pts, num_states))
-        agent_next_states = self.update_states(agent_state, \
-                            actions_theta, dt_forward)
-        
+        agent_next_states = self.update_states(
+            agent_state, actions_theta, dt_forward
+        )
+
         # only use the closest other agent
-        dist_2_others = [(np.linalg.norm(other_agent_state[0:2]-agent_state[0:2]) - \
-                other_agent_state[8] - agent_state[8]) for other_agent_state in other_agents_state]
+        dist_2_others = [
+            (
+                np.linalg.norm(other_agent_state[0:2] - agent_state[0:2])
+                - other_agent_state[8]
+                - agent_state[8]
+            )
+            for other_agent_state in other_agents_state
+        ]
         agent_num = np.argmin(np.array(dist_2_others))
-        other_agent_next_state = self.update_state(other_agents_state[agent_num], \
-                            other_agents_action_theta[agent_num], dt_forward)
+        other_agent_next_state = self.update_state(
+            other_agents_state[agent_num],
+            other_agents_action_theta[agent_num],
+            dt_forward,
+        )
         other_agents_next_state = [other_agent_next_state]
-        
 
-        ref_prll_vec, ref_orth_vec, agent_centric_states = \
-            pedData.rawStates_2_agentCentricStates(\
-                agent_next_states, other_agents_next_state, self.num_agents)
+        ref_prll_vec, ref_orth_vec, agent_centric_states = (
+            pedData.rawStates_2_agentCentricStates(
+                agent_next_states, other_agents_next_state, self.num_agents
+            )
+        )
 
         # for i in range(num_pts):
         #   ref_prll, ref_orth, agent_centric_states[i,:] = \
         #       pedData.rawState_2_agentCentricState( \
         #       agent_next_states[i,:], other_agent_next_state)
 
-        bad_inds_oppo, bad_inds_same, bad_inds_tangent = \
-            self.find_bad_inds(agent_centric_states)
-        #scaling factor
+        bad_inds_oppo, bad_inds_same, bad_inds_tangent = self.find_bad_inds(
+            agent_centric_states
+        )
+        # scaling factor
         d = np.linalg.norm(agent_state[0:2] - agent_state[6:8])
         v = agent_state[5]
-        getting_close_penalty =np.ones((num_pts,)) \
-            * GAMMA ** (d/DT_NORMAL) * (1.0 - GAMMA ** (-v/DT_NORMAL))
+        getting_close_penalty = (
+            np.ones((num_pts,))
+            * GAMMA ** (d / DT_NORMAL)
+            * (1.0 - GAMMA ** (-v / DT_NORMAL))
+        )
         penalty = np.zeros((num_pts,))
         penalty[bad_inds_oppo] = weight * getting_close_penalty[bad_inds_oppo]
-        penalty[bad_inds_same] = 1.0 * weight * getting_close_penalty[bad_inds_same]
-        penalty[bad_inds_tangent] = weight * getting_close_penalty[bad_inds_tangent]
+        penalty[bad_inds_same] = (
+            1.0 * weight * getting_close_penalty[bad_inds_same]
+        )
+        penalty[bad_inds_tangent] = (
+            weight * getting_close_penalty[bad_inds_tangent]
+        )
 
         return penalty
-        
-        
 
-    # for RL 
+    # for RL
     # back out information required by find_next_states_values
-    def find_next_state_pair_value_and_action_reward(self, agent_state, agent_next_state, \
-        other_agents_state, other_agents_next_state, dt_forward):
+    def find_next_state_pair_value_and_action_reward(
+        self,
+        agent_state,
+        agent_next_state,
+        other_agents_state,
+        other_agents_next_state,
+        dt_forward,
+    ):
         # agents
         # action_xy = agent_next_state[2:4]
         action_xy = (agent_next_state[0:2] - agent_state[0:2]) / dt_forward
         action_speed = np.linalg.norm(action_xy)
         if action_speed > EPS:
             action_angle = np.arctan2(action_xy[1], action_xy[0])
         else:
@@ -725,178 +915,263 @@
         action_theta = np.array([[action_speed, action_angle]])
 
         # other agents (TODO: vectorize)
         num_other_agents = len(other_agents_state)
         other_actions_theta = []
         for i, other_agent_next_state in enumerate(other_agents_next_state):
             # other_action_xy = other_agent_next_state[2:4]
-            other_action_xy = (other_agent_next_state[0:2] - other_agents_state[i][0:2]) / dt_forward
+            other_action_xy = (
+                other_agent_next_state[0:2] - other_agents_state[i][0:2]
+            ) / dt_forward
             other_action_speed = np.linalg.norm(other_action_xy)
             if other_action_speed > EPS:
-                other_action_angle = np.arctan2(other_action_xy[1], other_action_xy[0])
+                other_action_angle = np.arctan2(
+                    other_action_xy[1], other_action_xy[0]
+                )
             else:
                 other_action_angle = other_agent_next_state[4]
-            other_actions_theta.append(np.array([other_action_speed, other_action_angle]))
-
-        state_value, action_reward = \
-            self.find_values_and_action_rewards(agent_state, action_theta, \
-                            other_agents_state, other_actions_theta, dt_forward)
+            other_actions_theta.append(
+                np.array([other_action_speed, other_action_angle])
+            )
+
+        state_value, action_reward = self.find_values_and_action_rewards(
+            agent_state,
+            action_theta,
+            other_agents_state,
+            other_actions_theta,
+            dt_forward,
+        )
 
         return state_value, action_reward
 
-    def check_collisions_and_get_action_rewards(self, agent_state, actions_theta, \
-                            other_agents_state_in, other_agents_action=None, dt_forward=None):
+    def check_collisions_and_get_action_rewards(
+        self,
+        agent_state,
+        actions_theta,
+        other_agents_state_in,
+        other_agents_action=None,
+        dt_forward=None,
+    ):
         actions_theta_copy = actions_theta.copy()
         other_agents_state = copy.deepcopy(other_agents_state_in)
 
         # ref_prll, ref_orth, state_nn = \
         #   pedData.rawState_2_agentCentricState( \
         #   agent_state, other_agents_state, self.num_agents)
         num_actions = actions_theta.shape[0]
         # update other agent state
         num_other_agents = len(other_agents_state)
         if other_agents_action is None:
             other_agents_action = []
             for tt in range(num_other_agents):
-                other_agent_speed = np.linalg.norm(other_agents_state_in[tt][2:4])
-                other_agent_angle = np.arctan2(other_agents_state_in[tt][3], other_agents_state_in[tt][2])
-                other_agents_action.append(np.array([other_agent_speed, other_agent_angle]))
+                other_agent_speed = np.linalg.norm(
+                    other_agents_state_in[tt][2:4]
+                )
+                other_agent_angle = np.arctan2(
+                    other_agents_state_in[tt][3], other_agents_state_in[tt][2]
+                )
+                other_agents_action.append(
+                    np.array([other_agent_speed, other_agent_angle])
+                )
         # update other agents' velocity
         for tt in range(num_other_agents):
-            other_agents_state[tt][2] = other_agents_action[tt][0] * np.cos(other_agents_action[tt][1])
-            other_agents_state[tt][3] = other_agents_action[tt][0] * np.sin(other_agents_action[tt][1])
+            other_agents_state[tt][2] = other_agents_action[tt][0] * np.cos(
+                other_agents_action[tt][1]
+            )
+            other_agents_state[tt][3] = other_agents_action[tt][0] * np.sin(
+                other_agents_action[tt][1]
+            )
 
         # assume other agent is heading toward the vehicle
         # rel_pos = agent_state[0:2] - other_agent_state[0:2]
         # rel_angle = np.arctan2(rel_pos[1], rel_pos[0])
         # angle_diff = find_angle_diff(rel_angle, other_agent_action[1])
         # other_agent_action[1] += max(-np.pi/9.0, min(np.pi/9.0, angle_diff))
 
         # print 'other_agent_state, other_agent_action', other_agent_state, other_agent_action
         other_agents_next_state = []
         for tt in range(num_other_agents):
             # dt_forward_other = min(1,0, dt_forward)
-            other_agents_next_state.append(self.update_state(other_agents_state[tt], \
-                            other_agents_action[tt], dt_forward))
+            other_agents_next_state.append(
+                self.update_state(
+                    other_agents_state[tt], other_agents_action[tt], dt_forward
+                )
+            )
         # other_agent_next_state = (other_agent_state + other_agent_next_state) / 2.0
         agent_desired_speed = agent_state[5]
         # print 'other_agent_action', other_agent_action
         # compute values for each state
 
-
         # collide (not just getting close)
         min_dists_mat = np.zeros((num_actions, num_other_agents))
         if_collide_mat = np.zeros((num_actions, num_other_agents))
         cur_dist_vec = np.zeros((num_other_agents,))
         for tt in range(num_other_agents):
-            min_dists_mat[:,tt], if_collide_mat[:,tt] = self.if_actions_collide(agent_state, 
-                        actions_theta, other_agents_state[tt], other_agents_action[tt], dt_forward)
-        
-            radius = agent_state[8] + other_agents_state[tt][8] + self.radius_buffer
-            cur_dist_vec[tt] = np.linalg.norm(agent_state[0:2]-other_agents_state[tt][0:2]) - radius
+            min_dists_mat[:, tt], if_collide_mat[:, tt] = (
+                self.if_actions_collide(
+                    agent_state,
+                    actions_theta,
+                    other_agents_state[tt],
+                    other_agents_action[tt],
+                    dt_forward,
+                )
+            )
+
+            radius = (
+                agent_state[8] + other_agents_state[tt][8] + self.radius_buffer
+            )
+            cur_dist_vec[tt] = (
+                np.linalg.norm(agent_state[0:2] - other_agents_state[tt][0:2])
+                - radius
+            )
 
         min_dists = np.min(min_dists_mat, axis=1)
         if_collide = np.max(if_collide_mat, axis=1)
         cur_dist = np.min(cur_dist_vec)
 
         # print 'min_dists_mat', min_dists_mat
         # print 'if_collide_mat', if_collide_mat
         # print 'cur_dist_vec', cur_dist_vec
 
         # print 'min_dists', min_dists
         # print 'if_collide', if_collide
         # print 'cur_dist', cur_dist
         # raw_input()
 
-        action_rewards = self.find_action_rewards(agent_state, cur_dist, min_dists, dt_forward)
+        action_rewards = self.find_action_rewards(
+            agent_state, cur_dist, min_dists, dt_forward
+        )
         # print 'action_rewards', action_rewards
 
         # print 'action_rewards', action_rewards
-        return if_collide, action_rewards, min_dists, other_agents_next_state, num_actions, other_agents_state
-
-    def find_values_and_action_rewards(self, agent_state, actions_theta, \
-                            other_agents_state_in, other_agents_action=None, dt_forward=None):
-        if_collide, action_rewards, min_dists, other_agents_next_state, num_actions, other_agents_state = self.check_collisions_and_get_action_rewards(agent_state, actions_theta, \
-                            other_agents_state_in, other_agents_action, dt_forward)
+        return (
+            if_collide,
+            action_rewards,
+            min_dists,
+            other_agents_next_state,
+            num_actions,
+            other_agents_state,
+        )
+
+    def find_values_and_action_rewards(
+        self,
+        agent_state,
+        actions_theta,
+        other_agents_state_in,
+        other_agents_action=None,
+        dt_forward=None,
+    ):
+        (
+            if_collide,
+            action_rewards,
+            min_dists,
+            other_agents_next_state,
+            num_actions,
+            other_agents_state,
+        ) = self.check_collisions_and_get_action_rewards(
+            agent_state,
+            actions_theta,
+            other_agents_state_in,
+            other_agents_action,
+            dt_forward,
+        )
         state_values = np.zeros((num_actions,))
-        non_collision_inds = np.where(if_collide==False)[0]
+        non_collision_inds = np.where(if_collide == False)[0]
 
         # find states_values in batch
         gamma = GAMMA
         dt_normal = DT_NORMAL
         if len(non_collision_inds) > 0:
-            agent_next_states = self.update_states(agent_state, \
-                    actions_theta[non_collision_inds,:], dt_forward)
+            agent_next_states = self.update_states(
+                agent_state, actions_theta[non_collision_inds, :], dt_forward
+            )
 
             # find next_states that have reached the goal
-            dists_to_goal = np.linalg.norm(agent_next_states[:,0:2]-agent_next_states[:,6:8],axis=1)
-
-            reached_goals_inds = np.where((dists_to_goal < DIST_2_GOAL_THRES) & \
-                                (min_dists[non_collision_inds]>GETTING_CLOSE_RANGE))[0]
+            dists_to_goal = np.linalg.norm(
+                agent_next_states[:, 0:2] - agent_next_states[:, 6:8], axis=1
+            )
+
+            reached_goals_inds = np.where(
+                (dists_to_goal < DIST_2_GOAL_THRES)
+                & (min_dists[non_collision_inds] > GETTING_CLOSE_RANGE)
+            )[0]
             # not_reached_goals_inds = np.where(dists_to_goal >= DIST_2_GOAL_THRES)[0]
-            not_reached_goals_inds = np.setdiff1d(np.arange(len(non_collision_inds)), reached_goals_inds)
-            
-            non_collision_reached_goals_inds = non_collision_inds[reached_goals_inds]
-            non_collision_not_reached_goals_inds = non_collision_inds[not_reached_goals_inds]
-            
-            state_values[non_collision_not_reached_goals_inds] = \
-                self.find_states_values(agent_next_states[not_reached_goals_inds], other_agents_next_state)
-
+            not_reached_goals_inds = np.setdiff1d(
+                np.arange(len(non_collision_inds)), reached_goals_inds
+            )
+
+            non_collision_reached_goals_inds = non_collision_inds[
+                reached_goals_inds
+            ]
+            non_collision_not_reached_goals_inds = non_collision_inds[
+                not_reached_goals_inds
+            ]
+
+            state_values[non_collision_not_reached_goals_inds] = (
+                self.find_states_values(
+                    agent_next_states[not_reached_goals_inds],
+                    other_agents_next_state,
+                )
+            )
 
             # state_values[non_collision_reached_goals_inds] = gamma ** (dists_to_goal / dt_normal)
             # print 'dists_to_goal', dists_to_goal
             # print 'reached_goals_inds', reached_goals_inds
             # print 'non_collision_reached_goals_inds', non_collision_reached_goals_inds
             # print 'non_collision_not_reached_goals_inds', non_collision_not_reached_goals_inds
-            state_values[non_collision_reached_goals_inds] = \
-                gamma ** (dists_to_goal[reached_goals_inds] / dt_normal)
+            state_values[non_collision_reached_goals_inds] = gamma ** (
+                dists_to_goal[reached_goals_inds] / dt_normal
+            )
 
         try:
-            assert(np.all(action_rewards + state_values < 1.0001))
+            assert np.all(action_rewards + state_values < 1.0001)
         except:
-            print('agent_state', agent_state)
-            print('actions_theta', actions_theta)
-            print('other_agent_state', other_agent_state)
-            print('other_agent_action', other_agent_action)
-            print('dt_forward', dt_forward)
-            print('dists_to_goal', dists_to_goal)
-            print('actions_rewerds', action_rewards)
-            print('state_values', state_values)
-            print('values', action_rewards + gamma ** (dt_forward * \
-                agent_desired_speed / dt_normal) * state_values)
-            assert(0)       
-        
+            print("agent_state", agent_state)
+            print("actions_theta", actions_theta)
+            print("other_agent_state", other_agent_state)
+            print("other_agent_action", other_agent_action)
+            print("dt_forward", dt_forward)
+            print("dists_to_goal", dists_to_goal)
+            print("actions_rewerds", action_rewards)
+            print("state_values", state_values)
+            print(
+                "values",
+                action_rewards
+                + gamma ** (dt_forward * agent_desired_speed / dt_normal)
+                * state_values,
+            )
+            assert 0
+
         # np.set_printoptions(precision=4,formatter={'float': '{: 0.3f}'.format})
         # if True:#np.max(actions_theta[:,1]) - np.min(actions_theta[:,1]) < 1.5 * np.pi:
         #   actions_theta[:,1] -= agent_state[4]
         #   print '---------------------------'
         #   dist_between_agents = (np.linalg.norm(agent_state[0:2]-other_agents_state[0][0:2]) - \
         #                       agent_state[8] - other_agents_state[0][8])
         #   print 'dist between agents %.3f' % dist_between_agents
-            
+
         #   values = action_rewards + gamma ** (dt_forward * \
         #           agent_desired_speed/ dt_normal) *state_values
         #   print np.hstack((actions_theta, np.vstack((min_dists, action_rewards,\
         #       values, state_values)).transpose()))
         #   best_action_ind = np.argmax(values)
         #   print 'current heading', agent_state[4]
         #   print 'best_action', actions_theta[best_action_ind,:]
         #   print 'next_best_state', agent_next_states[best_action_ind,:]
         #   print 'other_agents_state[0]', other_agents_state[0]
         #   print 'other_agents_next_state[0]', other_agents_next_state[0]
         #   print 'other_agents_action[0]', other_agents_action[0]
         #   print other_agents_state_in[0]
         #   actions_theta[:,1] += agent_state[4]
 
-        
         # # print gamma ** (dt_forward * \
         # #         agent_desired_speed/ dt_normal)
         # # print 'state_values', state_values
         # # print 'dt_forward', dt_forward
-        # # print 'agent_state', agent_state 
+        # # print 'agent_state', agent_state
         # # print 'other_agent_state', other_agent_state
         # # print 'other_agent_action', other_agent_action
         # # print 'other_agent_next_state', other_agent_next_state
         # # print agent_next_states.shape
         # # print actions_theta.shape
         # # print state_values[:,np.newaxis].shape
         # # print 'agent_next_states', np.hstack((agent_next_states, actions_theta[non_collision_inds], \
@@ -906,16 +1181,21 @@
         # actions_theta[:,1] += agent_state[4]
         # # raw_input()
         # # if dist_between_agents < GETTING_CLOSE_RANGE:
         # #     raw_input()
 
         # assert(np.sum(actions_theta_copy - actions_theta) < 0.0001)
         # smoothness_cost = self.find_state_action_cost(agent_state, actions_theta, dt_forward)
-        passing_side_cost = self.find_passing_side_cost(agent_state, actions_theta,\
-            other_agents_state, other_agents_action, dt_forward)
+        passing_side_cost = self.find_passing_side_cost(
+            agent_state,
+            actions_theta,
+            other_agents_state,
+            other_agents_action,
+            dt_forward,
+        )
         # print passing_side_cost
         # raw_input()
         # return state_values, action_rewards + smoothness_cost + passing_side_cost
         # if len(state_values)>5:
         #   print 'state_values', state_values
         #   print 'action_rewards', action_rewards
         #   print 'min_dists', min_dists
@@ -934,99 +1214,135 @@
         #   print 'best_ind %d, best_value %.3f, min_dist[min_ind] %.3f, action_rewards[min_ind] %.3f, state_values[min_ind] %.3f\n' % \
         #       (best_ind, total[best_ind], min_dists[best_ind], \
         #       action_rewards[best_ind], state_values[best_ind])
         #   print 'dt_forward', dt_forward
         #   print 'current_dist', np.linalg.norm(agent_state[0:2] - agent_state[6:8])
         #   print 'next_dist_2_goal', np.linalg.norm(agent_next_states[:,0:2]-agent_next_states[:,6:8], axis=1)
         #   print 'speed', actions_theta[:,0]
-        return state_values, action_rewards + passing_side_cost #+ smoothness_cost
+        return (
+            state_values,
+            action_rewards + passing_side_cost,
+        )  # + smoothness_cost
 
     # assuming the other agent follows its current speed
     # agent_state: agent's current state
     # actions_theta: multiple actions considered
     # other_agent_state: other agent's current state
-    def find_next_states_values(self, agent_state, actions_theta, \
-                            other_agents_state, other_agents_action=None, dt_forward=None):
-        values, state_values, action_rewards, dt_forward = self.find_next_states_values_and_components(agent_state, actions_theta, other_agents_state, other_agents_action, dt_forward)
+    def find_next_states_values(
+        self,
+        agent_state,
+        actions_theta,
+        other_agents_state,
+        other_agents_action=None,
+        dt_forward=None,
+    ):
+        values, state_values, action_rewards, dt_forward = (
+            self.find_next_states_values_and_components(
+                agent_state,
+                actions_theta,
+                other_agents_state,
+                other_agents_action,
+                dt_forward,
+            )
+        )
         return values
 
-    def find_next_states_values_and_components(self, agent_state, actions_theta, \
-                            other_agents_state, other_agents_action=None, dt_forward=None):
+    def find_next_states_values_and_components(
+        self,
+        agent_state,
+        actions_theta,
+        other_agents_state,
+        other_agents_action=None,
+        dt_forward=None,
+    ):
         # making sure look ahead time is not too long (reaching goal)
         # or too short (if agent's desired speed is too slow)
         if dt_forward is None:
             agent_speed = agent_state[5]
-            dt_forward_max = max(self.dt_forward, 0.5/agent_speed)
+            dt_forward_max = max(self.dt_forward, 0.5 / agent_speed)
             # dt_forward_max = self.dt_forward
-            dist_to_goal = np.linalg.norm(agent_state[6:8]- agent_state[0:2])
+            dist_to_goal = np.linalg.norm(agent_state[6:8] - agent_state[0:2])
             time_to_goal = dist_to_goal / agent_speed
-            dt_forward = min(dt_forward_max, time_to_goal) #1.0
+            dt_forward = min(dt_forward_max, time_to_goal)  # 1.0
 
-        state_values, action_rewards = \
-            self.find_values_and_action_rewards(agent_state, actions_theta, \
-                            other_agents_state, other_agents_action, dt_forward)
+        state_values, action_rewards = self.find_values_and_action_rewards(
+            agent_state,
+            actions_theta,
+            other_agents_state,
+            other_agents_action,
+            dt_forward,
+        )
 
         gamma = GAMMA
         dt_normal = DT_NORMAL
         agent_desired_speed = agent_state[5]
 
         num_states = len(actions_theta)
         # method 1
         # dt_forward_vec = np.ones((num_states,))
         # dt_forward_vec *= dt_forward
         # method 2
         dt_forward_vec = 0.2 * np.ones((num_states,)) * dt_forward
-        dt_forward_vec += 0.8 * actions_theta[:,0] / agent_desired_speed * dt_forward
+        dt_forward_vec += (
+            0.8 * actions_theta[:, 0] / agent_desired_speed * dt_forward
+        )
         # print 'dt_forwards', dt_forward
         # print 'dt_forwards_vec', dt_forward_vec
         # raw_input()
-        values =  action_rewards + gamma ** (dt_forward_vec * \
-            agent_desired_speed / dt_normal) * state_values
+        values = (
+            action_rewards
+            + gamma ** (dt_forward_vec * agent_desired_speed / dt_normal)
+            * state_values
+        )
 
         return values, state_values, action_rewards, dt_forward
 
     def find_feasible_actions(self, agent_state, static_constraints=None):
         # print 'agent_state', agent_state
-        if self.mode == 'no_constr':
-            ''' actions choice 1 '''
+        if self.mode == "no_constr":
+            """actions choice 1"""
             default_action_xy = agent_state[2:4]
             speed = np.linalg.norm(default_action_xy)
             # angle_select = np.arctan2(default_action_xy[1], default_action_xy[0])
             angle_select = agent_state[4]
 
             default_action_theta = np.array([speed, angle_select])
-            actions_theta = self.find_actions_theta(agent_state, default_action_theta)
+            actions_theta = self.find_actions_theta(
+                agent_state, default_action_theta
+            )
 
             # possibly stuck
             # if speed < agent_state[5] * 0.1:
-            #   actions_theta_tmp = self.plot_actions.copy()    
+            #   actions_theta_tmp = self.plot_actions.copy()
             #   actions_theta_tmp[:,0] *= agent_state[5]
             #   actions_theta_tmp[:,1] = (actions_theta_tmp[:,1] - np.pi)  / 2.0
             #   actions_theta_tmp[:,1] += np.arctan2(agent_state[7]-agent_state[1], \
             #                   agent_state[6]-agent_state[0])
             #   actions_theta = np.vstack((actions_theta, actions_theta_tmp))
             #   actions_theta[:,1] = (actions_theta[:,1] + np.pi) % (np.pi * 2) - np.pi
 
             # print 'agent_state', agent_state
             # print 'actions_theta', actions_theta
-        elif self.mode == 'rotate_constr':
-            ''' actions choice 2 '''
+        elif self.mode == "rotate_constr":
+            """actions choice 2"""
             # need to handle acceleration better (limits on changing velocity as a function of time)
             actions_theta = self.find_actions_theta_dynConstr(agent_state, 1.0)
         else:
-            assert(0)
+            assert 0
 
         # print actions_theta
         # print '---'
         # print 'before, max_speed', np.max(actions_theta[:,0])
         # prune actions if there are static constraints (from static obstacles in map)
         # static_constraints: max_speeds, angles
         if static_constraints is not None:
             # print static_constraints
-            angle_incr = abs(static_constraints[2,1] - static_constraints[1,1])
+            angle_incr = abs(
+                static_constraints[2, 1] - static_constraints[1, 1]
+            )
             # check
             # angle_incr_vec = abs(static_constraints[1:,1] - static_constraints[0:-1,1])
             # try:
             #   assert(np.all(angle_incr_vec - angle_incr<EPS))
             # except AssertionError:
             #   print 'static_constraints error (angle spacing)',
             #   print static_constraints
@@ -1035,58 +1351,78 @@
             # min_angle = static_constraints[0,1]
             # lower_inds = ((actions_theta[:,1]-min_angle) / angle_incr).astype(int)
             # upper_inds = lower_inds + 1
             # print 'theta_col:',actions_theta[:,1]
             # print 'stat col:',static_constraints[:,1]
             # print 'len theta', len(actions_theta[:,1])
             # print 'len stat', len(static_constraints[:,1])
-            upper_inds = np.digitize(actions_theta[:,1], static_constraints[:,1])
+            upper_inds = np.digitize(
+                actions_theta[:, 1], static_constraints[:, 1]
+            )
             # print 'lower_inds', lower_inds
             lower_inds = upper_inds - 1
             # print 'upper_inds', upper_inds
             try:
-                assert(np.all(lower_inds<len(static_constraints)))
+                assert np.all(lower_inds < len(static_constraints))
             except AssertionError:
-                print('lower_inds:',lower_inds)
-                print('len(actions_theta):', len(actions_theta))
-                bad_ind = np.where(lower_inds>=len(actions_theta))[0]
-                print('actions theta:',actions_theta)
-                print('bad_ind', actions_theta[bad_ind,1])
-                print('static_constraints', static_constraints)
-                assert(0)
-
-            alpha = (actions_theta[:,1] - static_constraints[lower_inds,1]) / angle_incr
+                print("lower_inds:", lower_inds)
+                print("len(actions_theta):", len(actions_theta))
+                bad_ind = np.where(lower_inds >= len(actions_theta))[0]
+                print("actions theta:", actions_theta)
+                print("bad_ind", actions_theta[bad_ind, 1])
+                print("static_constraints", static_constraints)
+                assert 0
+
+            alpha = (
+                actions_theta[:, 1] - static_constraints[lower_inds, 1]
+            ) / angle_incr
             # print 'static_constraints', static_constraints
             # print 'before---', actions_theta
             # print static_constraints
             # print 'alpha', alpha
-            max_speeds_int = alpha * static_constraints[upper_inds,0] + (1-alpha) * static_constraints[lower_inds,0]
+            max_speeds_int = (
+                alpha * static_constraints[upper_inds, 0]
+                + (1 - alpha) * static_constraints[lower_inds, 0]
+            )
             pref_speed = agent_state[5]
             # assert(np.all(max_speeds_int <=pref_speed))
-            actions_theta[:,0] = actions_theta[:,0] * max_speeds_int / pref_speed
+            actions_theta[:, 0] = (
+                actions_theta[:, 0] * max_speeds_int / pref_speed
+            )
             #   unique rows
-            actions_theta = np.asarray(np.vstack({tuple(row) for row in actions_theta}))
+            actions_theta = np.asarray(
+                np.vstack({tuple(row) for row in actions_theta})
+            )
             # print 'after---', actions_theta
             # print 'cur_pos, goal', agent_state[0:2], agent_state[6:8]
         # print 'after, max_speed', np.max(actions_theta[:,0])
 
         return actions_theta
 
     # state raw is in global frame
     # velocity output should also be in global frame
-    def find_next_action(self, agent_state, other_agents_state, other_agents_action=None, static_constraints=None):
+    def find_next_action(
+        self,
+        agent_state,
+        other_agents_state,
+        other_agents_action=None,
+        static_constraints=None,
+    ):
         # state_raw =  2x [pos.x, pos.y, vel.x, vel.y,prefVelocity.x, \
         # prefVelocity.y, goals[0].x, goals[0].y]
         # state_nn = [dist_to_goal, pref_speed, vx, vy, \
         # other_vx, other_vx, rel_pos_x, rel_pos_y]
 
-        actions_theta = self.find_feasible_actions(agent_state, static_constraints=static_constraints)
-
-        state_values = self.find_next_states_values(agent_state, \
-            actions_theta, other_agents_state, other_agents_action)
+        actions_theta = self.find_feasible_actions(
+            agent_state, static_constraints=static_constraints
+        )
+
+        state_values = self.find_next_states_values(
+            agent_state, actions_theta, other_agents_state, other_agents_action
+        )
 
         # print("actions_theta:", actions_theta)
         # print("state_values:", state_values)
 
         best_action_ind = np.argmax(state_values)
         best_action = actions_theta[best_action_ind]
         # print '------'
@@ -1115,57 +1451,84 @@
 
         # print 'best_action', best_action
         # raw_input()
         # print 'action_chosen', best_action[0] * np.cos(best_action[1]), \
         #   best_action[0] * np.sin(best_action[1])
         return best_action
 
-    def find_subgoal(self, agent_state,\
-     other_agents_state, min_dist, other_agents_action=None, static_constraints=None):
-
+    def find_subgoal(
+        self,
+        agent_state,
+        other_agents_state,
+        min_dist,
+        other_agents_action=None,
+        static_constraints=None,
+    ):
         # Find subgoals that are far away and have good diffusion costs
         diff_map_goal = agent_state[6:8]
-        angle_to_diff_map_goal = np.arctan2(diff_map_goal[1]-agent_state[1],diff_map_goal[0]-agent_state[0])
-        lower_cost_to_go_inds = np.where((static_constraints[:,2] > 6.5) & \
-                    (abs(static_constraints[:,1]-angle_to_diff_map_goal) < np.pi/8))[0]
-        print('MIN_DIST:', min_dist)
+        angle_to_diff_map_goal = np.arctan2(
+            diff_map_goal[1] - agent_state[1],
+            diff_map_goal[0] - agent_state[0],
+        )
+        lower_cost_to_go_inds = np.where(
+            (static_constraints[:, 2] > 6.5)
+            & (
+                abs(static_constraints[:, 1] - angle_to_diff_map_goal)
+                < np.pi / 8
+            )
+        )[0]
+        print("MIN_DIST:", min_dist)
         # if len(lower_cost_to_go_inds)>0:# and min_dist < 7.0:
         if False:
-            lower_cost_to_go_actions = static_constraints[lower_cost_to_go_inds,:]
-            x = lower_cost_to_go_actions[:,2] * np.cos(lower_cost_to_go_actions[:,1]) + agent_state[0]
-            y = lower_cost_to_go_actions[:,2] * np.sin(lower_cost_to_go_actions[:,1]) + agent_state[1]
-            lower_cost_to_go_subgoals = np.column_stack((x,y))
+            lower_cost_to_go_actions = static_constraints[
+                lower_cost_to_go_inds, :
+            ]
+            x = (
+                lower_cost_to_go_actions[:, 2]
+                * np.cos(lower_cost_to_go_actions[:, 1])
+                + agent_state[0]
+            )
+            y = (
+                lower_cost_to_go_actions[:, 2]
+                * np.sin(lower_cost_to_go_actions[:, 1])
+                + agent_state[1]
+            )
+            lower_cost_to_go_subgoals = np.column_stack((x, y))
             # print 'static_constraints:', static_constraints
             # print 'lower cost2go inds:', lower_cost_to_go_inds
-            print('lower cost2go actions:', lower_cost_to_go_actions)
+            print("lower cost2go actions:", lower_cost_to_go_actions)
             # print 'lower cost2go subgoals:', lower_cost_to_go_subgoals
 
-            agent_states = np.zeros((len(lower_cost_to_go_inds),len(agent_state)))
+            agent_states = np.zeros(
+                (len(lower_cost_to_go_inds), len(agent_state))
+            )
             for i in range(len(lower_cost_to_go_inds)):
                 state = copy.deepcopy(agent_state)
-                state[6:8] = lower_cost_to_go_subgoals[i,0:2]
+                state[6:8] = lower_cost_to_go_subgoals[i, 0:2]
                 # state[2] = agent_state[5] * np.cos(agent_state[4])
                 # state[3] = agent_state[5] * np.sin(agent_state[4])
                 agent_states[i] = state
             # print 'states:', agent_states
             # Query the NN about every potential subgoal and pick the best one
-            state_values = self.find_states_values(agent_states, other_agents_state)
+            state_values = self.find_states_values(
+                agent_states, other_agents_state
+            )
             best_subgoal_ind = np.argmax(state_values)
             # print 'best_subgoal ind', best_subgoal_ind
             best_subgoal = lower_cost_to_go_subgoals[best_subgoal_ind]
 
             # print 'states_values:', state_values
             agent_state[6:8] = best_subgoal
-            print('Good Subgoal Found')
+            print("Good Subgoal Found")
             # print 'Best subgoal:', best_subgoal
         else:
             # use subgoal directly from diffusion map
             lower_cost_to_go_subgoals = None
             best_subgoal = agent_state[6:8]
-            print('No good subgoal found.')
+            print("No good subgoal found.")
 
         return best_subgoal, lower_cost_to_go_subgoals
 
     # def find_next_action_using_cost_to_go(self, agent_state,\
     #        other_agents_state, min_dist, other_agents_action=None, static_constraints=None):
 
     #   # Use that best subgoal to query every feasible action
@@ -1185,67 +1548,93 @@
     #   if self.if_collide_with_other_agents(agent_state, other_agents_state):
     #       self.current_value = COLLISION_COST
     #   else:
     #       self.current_value = state_values[best_action_ind]
 
     #   return best_action
 
-    
-
     def if_collide_with_other_agents(self, agent_state, other_agents_state):
         num_other_agents = len(other_agents_state)
         for other_agent_state in other_agents_state:
-            if self.if_pos_collide(agent_state[0:2], other_agent_state[0:2], \
-                agent_state[8] + other_agent_state[8]):
+            if self.if_pos_collide(
+                agent_state[0:2],
+                other_agent_state[0:2],
+                agent_state[8] + other_agent_state[8],
+            ):
                 return True
         return False
 
     def if_terminal_state(self, agent_state, other_agents_state):
         # check collision
         if self.if_collide_with_other_agents(agent_state, other_agents_state):
             return COLLIDED
         # check if reached goal
         for other_agent_state in other_agents_state:
-            if not ((( np.linalg.norm(agent_state[0:2] - agent_state[6:8])<DIST_2_GOAL_THRES) \
-                and (np.linalg.norm(agent_state[0:2] - other_agent_state[0:2]) >  \
-                agent_state[8] + other_agent_state[8] + GETTING_CLOSE_RANGE or \
-                 np.linalg.norm(other_agent_state[0:2] - other_agent_state[6:8])<DIST_2_GOAL_THRES))):
+            if not (
+                (
+                    (
+                        np.linalg.norm(agent_state[0:2] - agent_state[6:8])
+                        < DIST_2_GOAL_THRES
+                    )
+                    and (
+                        np.linalg.norm(
+                            agent_state[0:2] - other_agent_state[0:2]
+                        )
+                        > agent_state[8]
+                        + other_agent_state[8]
+                        + GETTING_CLOSE_RANGE
+                        or np.linalg.norm(
+                            other_agent_state[0:2] - other_agent_state[6:8]
+                        )
+                        < DIST_2_GOAL_THRES
+                    )
+                )
+            ):
                 break
             return REACHED_GOAL
         return NON_TERMINAL
 
     # find a random action
-    def find_rand_action(self, agent_state, other_agents_state, \
-            other_agents_action=None, isBestAction=False, static_constraints=None):
+    def find_rand_action(
+        self,
+        agent_state,
+        other_agents_state,
+        other_agents_action=None,
+        isBestAction=False,
+        static_constraints=None,
+    ):
         rand_float = np.random.rand()
         cur_state = agent_state[0:2]
         goal = agent_state[6:8]
         nom_speed = agent_state[5]
         # if rand_float < 0.3: # prefered speed toward goal
         #   action = self.computePrefVel(cur_state, goal, nom_speed)
         # elif rand_float < 0.6: # zero action
         #   action = np.zeros((2,))
         # else: # random action
         #   action = np.zeros((2,))
         #   action[0] = np.random.uniform(0, nom_speed)
         #   action[1] = np.random.uniform(0, 2 * np.pi) - np.pi
-        actions_theta = self.find_feasible_actions(agent_state, static_constraints=static_constraints)
-
-        state_values = self.find_next_states_values(agent_state, \
-            actions_theta, other_agents_state, other_agents_action)
+        actions_theta = self.find_feasible_actions(
+            agent_state, static_constraints=static_constraints
+        )
+
+        state_values = self.find_next_states_values(
+            agent_state, actions_theta, other_agents_state, other_agents_action
+        )
 
-        if isBestAction: 
+        if isBestAction:
             max_inds = np.argpartition(state_values, -4)[-1:]
-        else: 
+        else:
             max_inds = np.argpartition(state_values, -4)[-5:-2]
 
         # ind = np.random.randint(len(actions_theta))
         ind = np.random.randint(len(max_inds))
         ind = max_inds[ind]
-        action = actions_theta[ind,:]
+        action = actions_theta[ind, :]
         return action
 
     def update_state(self, state, action_theta, dt):
         speed = action_theta[0]
         angle_select = action_theta[1]
         next_state = copy.deepcopy(state)
         pref_speed = state[5]
@@ -1267,119 +1656,132 @@
         # next_state[9] = min(3.0, next_state[9] + dt)
         # turning direction and previous osscilation magnitude
         angle_diff = find_angle_diff(action_theta[1], state[4])
         # next_state[9] = angle_diff
         if abs(next_state[9]) < EPS:
             next_state[9] = 0.11 * np.sign(angle_diff)
         elif next_state[9] * angle_diff < 0:
-            next_state[9] = max(-np.pi, min(np.pi, -next_state[9] + angle_diff))
+            next_state[9] = max(
+                -np.pi, min(np.pi, -next_state[9] + angle_diff)
+            )
         else:
-            next_state[9] = np.sign(next_state[9]) * max(0.0, abs(next_state[9])-0.1)
+            next_state[9] = np.sign(next_state[9]) * max(
+                0.0, abs(next_state[9]) - 0.1
+            )
         # print 'state[9]', state[9]
         # print 'angle_diff', angle_diff
         # print 'next_state[9]', next_state[9]
-        # raw_input() 
+        # raw_input()
 
-        if self.mode == 'no_constr':
+        if self.mode == "no_constr":
             next_state[4] = angle_select
-        elif self.mode == 'rotate_constr':
+        elif self.mode == "rotate_constr":
             min_turning_radius = 0.5
-            limit = pref_speed / min_turning_radius * dt  
+            limit = pref_speed / min_turning_radius * dt
             angle_diff = find_angle_diff(action_theta[1], state[4])
-            delta_heading_lb = - limit
+            delta_heading_lb = -limit
             delta_heading_ub = limit
-            next_state[4] = state[4] + np.clip(angle_diff, \
-                delta_heading_lb, delta_heading_ub)
+            next_state[4] = state[4] + np.clip(
+                angle_diff, delta_heading_lb, delta_heading_ub
+            )
             next_state[4] = (next_state[4] + np.pi) % (2 * np.pi) - np.pi
         else:
-            assert(0)
+            assert 0
 
         # if np.linalg.norm(next_state[0:2] - next_state[6:8]) == 0:
-            # next_state[5] /= (np.linalg.norm(next_state[4:6]+EPS) * 100.0)
+        # next_state[5] /= (np.linalg.norm(next_state[4:6]+EPS) * 100.0)
         # try:
         #   assert(next_state[4] > -np.pi-EPS and next_state[4] < np.pi+EPS)
         # except AssertionError:
         #   print action_theta
         #   assert(0)
 
         return next_state
 
     def update_states(self, state, actions_theta, dt):
-        speeds = actions_theta[:,0]
-        angles_select = actions_theta[:,1]
+        speeds = actions_theta[:, 0]
+        angles_select = actions_theta[:, 1]
         num_actions = actions_theta.shape[0]
-        next_states = np.matlib.repmat(state, num_actions, 1)
+        next_states = np.tile(state, (num_actions, 1))
         pref_speed = state[5]
         # try:
         #   assert(np.all(actions_theta[:,0] < pref_speed + 0.0001))
         # except:
         #   print 'pref_speed', pref_speed
         #   print 'actions_theta[:,0]', actions_theta[:,0]
         #   assert(0)
-        
+
         # print angle_select
-        next_states[:,0] += speeds * np.cos(angles_select) * dt
-        next_states[:,1] += speeds * np.sin(angles_select) * dt
+        next_states[:, 0] += speeds * np.cos(angles_select) * dt
+        next_states[:, 1] += speeds * np.sin(angles_select) * dt
         # next_states[:,2] = 0.5 * next_states[:,2] + 0.5 * speeds * np.cos(angles_select)
         # next_states[:,3] = 0.5 * next_states[:,3] + 0.5 * speeds * np.sin(angles_select)
-        next_states[:,2] = speeds * np.cos(angles_select)
-        next_states[:,3] = speeds * np.sin(angles_select)
-        next_states[:,5] = pref_speed
+        next_states[:, 2] = speeds * np.cos(angles_select)
+        next_states[:, 3] = speeds * np.sin(angles_select)
+        next_states[:, 5] = pref_speed
         # next_states[:,9] = np.clip(next_states[:,9] + dt, 0.0, 3.0)
         # angles_diff = find_angle_diff(actions_theta[:,1], state[4])
         # next_states[:,9] = angles_diff
 
-        angles_diff = find_angle_diff(actions_theta[:,1], state[4])
+        angles_diff = find_angle_diff(actions_theta[:, 1], state[4])
         # next_states[:,9] = angles_diff
-        zero_inds = np.where(abs(next_states[:,9]) < EPS)[0]
-        oscillation_inds = np.where(next_states[:,9] * angles_diff < 0)[0]
+        zero_inds = np.where(abs(next_states[:, 9]) < EPS)[0]
+        oscillation_inds = np.where(next_states[:, 9] * angles_diff < 0)[0]
         oscillation_inds = np.setdiff1d(oscillation_inds, zero_inds)
 
-        same_dir_inds = np.where(next_states[:,9] * angles_diff > -EPS)[0]
-        same_dir_inds = np.setdiff1d(same_dir_inds, np.union1d(zero_inds, oscillation_inds))
-
-        
-        next_states[zero_inds,9] = 0.11 * np.sign(angles_diff[zero_inds])
-        next_states[oscillation_inds,9] = np.clip(-next_states[oscillation_inds,9] \
-            + angles_diff[oscillation_inds], -np.pi, np.pi)
-        next_states[same_dir_inds,9] = np.sign(next_states[same_dir_inds,9]) * \
-            np.clip(abs(next_states[same_dir_inds,9]) - 0.1, 0.0, np.pi)
+        same_dir_inds = np.where(next_states[:, 9] * angles_diff > -EPS)[0]
+        same_dir_inds = np.setdiff1d(
+            same_dir_inds, np.union1d(zero_inds, oscillation_inds)
+        )
+
+        next_states[zero_inds, 9] = 0.11 * np.sign(angles_diff[zero_inds])
+        next_states[oscillation_inds, 9] = np.clip(
+            -next_states[oscillation_inds, 9] + angles_diff[oscillation_inds],
+            -np.pi,
+            np.pi,
+        )
+        next_states[same_dir_inds, 9] = np.sign(
+            next_states[same_dir_inds, 9]
+        ) * np.clip(abs(next_states[same_dir_inds, 9]) - 0.1, 0.0, np.pi)
 
-        # print 'states[:,9], angles_diff, next_state[:,9]', 
+        # print 'states[:,9], angles_diff, next_state[:,9]',
         # print np.vstack((np.matlib.repmat(state[9], 1, len(actions_theta)),\
         #       angles_diff, next_states[:,9])).transpose()
-        # raw_input() 
+        # raw_input()
 
-        if self.mode == 'no_constr':
-            next_states[:,4] = angles_select
-        elif self.mode == 'rotate_constr':
+        if self.mode == "no_constr":
+            next_states[:, 4] = angles_select
+        elif self.mode == "rotate_constr":
             min_turning_radius = 0.5
-            limit = pref_speed / min_turning_radius * dt  
-            angles_diff = find_angle_diff(actions_theta[:,1], state[4])
+            limit = pref_speed / min_turning_radius * dt
+            angles_diff = find_angle_diff(actions_theta[:, 1], state[4])
             # assert(len(angles_diff) == actions_theta.shape[0])
             max_angle_diff = np.amax(abs(angles_diff))
             # try:
             #   assert(max_angle_diff < limit/dt + 0.01)
             # except:
             #   print '---\n state[4]', state[4]
             #   print 'actions_theta', actions_theta
             #   print 'angles_diff', angles_diff
             #   print 'max_angle_diff', max_angle_diff
             #   print 'pref_speed, dt, limit', pref_speed, dt, limit/dt
             #   assert(0)
             delta_heading_lb = -limit
             delta_heading_ub = limit
-            next_states[:,4] = state[4] + np.clip(angles_diff, \
-                delta_heading_lb, delta_heading_ub)
-            next_states[:,4] = (next_states[:,4] + np.pi) % (2 * np.pi) - np.pi
+            next_states[:, 4] = state[4] + np.clip(
+                angles_diff, delta_heading_lb, delta_heading_ub
+            )
+            next_states[:, 4] = (next_states[:, 4] + np.pi) % (
+                2 * np.pi
+            ) - np.pi
         else:
-            assert(0)
+            assert 0
 
         # compute pref_vecs
-        # avoid divide by zero problem 
+        # avoid divide by zero problem
         # next_states[:,4:6] /= (np.linalg.norm(next_states[:,4:6], axis=1)[:,np.newaxis] * 100.0)
         # tmp_vec = next_states[:,6:8] - next_states[:,0:2]
         # pref_speeds = np.linalg.norm(tmp_vec, axis=1)[:,np.newaxis]
         # valid_inds = np.where(pref_speeds > 0)[0]
         # pref_vecs = tmp_vec[valid_inds] / pref_speeds[valid_inds] * pref_speed
         # next_states[valid_inds,4] = pref_vecs[:,0]
         # next_states[valid_inds,5] = pref_vecs[:,1]
@@ -1387,17 +1789,23 @@
         #   assert(np.all(next_states[:,4] > -np.pi-EPS) and np.all(next_states[:,4] < np.pi+EPS))
         # except AssertionError:
         #   print actions_theta
         #   assert(0)
 
         return next_states
 
-    # check collision 
-    def if_action_collide(self, agent_state, agent_action, other_agent_state, \
-                            other_agent_action, delta_t):
+    # check collision
+    def if_action_collide(
+        self,
+        agent_state,
+        agent_action,
+        other_agent_state,
+        other_agent_action,
+        delta_t,
+    ):
         # sampling version
         # t = 0.0
         # incr = np.min((delta_t, 0.25))
         # radius = agent_state[8] + other_agent_state[8] + self.radius_buffer
         # agent_v = np.zeros((2,))
         # agent_v[0] = agent_action[0] * np.cos(agent_action[1])
         # agent_v[1] = agent_action[0] * np.sin(agent_action[1])
@@ -1411,147 +1819,187 @@
         # return False
 
         # analytical version
         agent_v = np.zeros((2,))
         agent_v[0] = agent_action[0] * np.cos(agent_action[1])
         agent_v[1] = agent_action[0] * np.sin(agent_action[1])
         other_agent_v = np.zeros((2,))
-        other_agent_v[0] = other_agent_action[0] * np.cos(other_agent_action[1])
-        other_agent_v[1] = other_agent_action[0] * np.sin(other_agent_action[1])
+        other_agent_v[0] = other_agent_action[0] * np.cos(
+            other_agent_action[1]
+        )
+        other_agent_v[1] = other_agent_action[0] * np.sin(
+            other_agent_action[1]
+        )
         # other_agent_v[0] = other_agent_action[0] * np.cos(other_agent_action[1] + np.random.randn()*np.pi/36)
         # other_agent_v[1] = other_agent_action[0] * np.sin(other_agent_action[1] + np.random.randn()*np.pi/36)
 
         # modifying distance calculation
-        rel_pos_angle = np.arctan2(other_agent_state[1] - agent_state[1], \
-                        other_agent_state[0] - agent_state[0])
+        rel_pos_angle = np.arctan2(
+            other_agent_state[1] - agent_state[1],
+            other_agent_state[0] - agent_state[0],
+        )
         agent_speed_angle = np.arctan2(agent_v[1], agent_v[0])
         angle_diff = find_angle_diff(rel_pos_angle, agent_speed_angle)
         # other agent in front, zero out other agent's speed in the same direction
         if abs(angle_diff) < np.pi:
             dot_product = np.sum(agent_v * other_agent_v)
             if dot_product > EPS:
-                other_agent_v = other_agent_v - dot_prouct / np.linalg.norm(agent_v) * agent_v 
+                other_agent_v = (
+                    other_agent_v
+                    - dot_prouct / np.linalg.norm(agent_v) * agent_v
+                )
 
         # blind spot
         # elif abs(angle_diff) > 3.0 * np.pi/4.0:
 
-
         radius = agent_state[8] + other_agent_state[8] + self.radius_buffer
         x1 = agent_state[0:2]
         x2 = agent_state[0:2] + delta_t * agent_v
         y1 = other_agent_state[0:2]
         y2 = other_agent_state[0:2] + delta_t * other_agent_v
         # return if_segs_collide(x1, x2, y1, y2, radius)
         min_dist = ind_dist_between_segs(x1, x2, y1, y2)
         # min_dist = min_dist - 0.03 * np.random.random()
-        cur_dist = np.linalg.norm(x1-y1)
+        cur_dist = np.linalg.norm(x1 - y1)
         if cur_dist < radius:
             if_collide = True
         else:
             if_collide = min_dists < radius
         # dist_future = x2 - (0.75*y1 + 0.25*y2)
         # dist_future = np.linalg.norm(dist_future)
         # min_dist = min(dist_future, min_dist)
         min_dist = min_dist - radius
         return min_dist, min_dist < 0
 
-    # check collision 
-    def if_actions_collide(self, agent_state, agent_actions, other_agent_state, \
-                            other_agent_action, delta_t):
+    # check collision
+    def if_actions_collide(
+        self,
+        agent_state,
+        agent_actions,
+        other_agent_state,
+        other_agent_action,
+        delta_t,
+    ):
         # bnd
         agent_pref_speed = agent_state[5]
         other_agent_speed = other_agent_action[0]
         radius = agent_state[8] + other_agent_state[8] + self.radius_buffer
         num_actions = agent_actions.shape[0]
         if_collide = np.zeros((num_actions), dtype=bool)
-        min_dists = (radius + GETTING_CLOSE_RANGE + EPS) * np.ones((num_actions), dtype=bool)
+        min_dists = (radius + GETTING_CLOSE_RANGE + EPS) * np.ones(
+            (num_actions), dtype=bool
+        )
         # two agents are too far away for collision
-        if np.linalg.norm(agent_state[0:2] - other_agent_state[0:2]) > \
-            (agent_pref_speed+other_agent_speed) * delta_t + radius:
-            return min_dists, if_collide # default to no collision
-
-        # check for each action individually 
-        agent_vels = np.zeros((num_actions,2))
-        agent_vels[:,0] = agent_actions[:,0] * np.cos(agent_actions[:,1])
-        agent_vels[:,1] = agent_actions[:,0] * np.sin(agent_actions[:,1])
+        if (
+            np.linalg.norm(agent_state[0:2] - other_agent_state[0:2])
+            > (agent_pref_speed + other_agent_speed) * delta_t + radius
+        ):
+            return min_dists, if_collide  # default to no collision
+
+        # check for each action individually
+        agent_vels = np.zeros((num_actions, 2))
+        agent_vels[:, 0] = agent_actions[:, 0] * np.cos(agent_actions[:, 1])
+        agent_vels[:, 1] = agent_actions[:, 0] * np.sin(agent_actions[:, 1])
         other_agent_v = np.zeros((2,))
-        other_agent_v[0] = other_agent_action[0] * np.cos(other_agent_action[1])
-        other_agent_v[1] = other_agent_action[0] * np.sin(other_agent_action[1])
+        other_agent_v[0] = other_agent_action[0] * np.cos(
+            other_agent_action[1]
+        )
+        other_agent_v[1] = other_agent_action[0] * np.sin(
+            other_agent_action[1]
+        )
         # other_agent_v[0] = other_agent_action[0] * np.cos(other_agent_action[1] + np.random.randn()*np.pi/36)
         # other_agent_v[1] = other_agent_action[0] * np.sin(other_agent_action[1] + np.random.randn()*np.pi/36)
-        other_agent_vels = np.matlib.repmat(other_agent_v, num_actions, 1)
+        other_agent_vels = np.tile(other_agent_v, (num_actions, 1))
 
         # modifying distance calculation
-        p_oa_angle = np.arctan2(other_agent_state[1] - agent_state[1], \
-                        other_agent_state[0] - agent_state[0])
-        agent_speed_angles = np.arctan2(agent_vels[:,1], agent_vels[:,0])
+        p_oa_angle = np.arctan2(
+            other_agent_state[1] - agent_state[1],
+            other_agent_state[0] - agent_state[0],
+        )
+        agent_speed_angles = np.arctan2(agent_vels[:, 1], agent_vels[:, 0])
         other_speed_angle = np.arctan2(other_agent_v[1], other_agent_v[0])
         heading_diff = find_angle_diff(agent_speed_angles, other_speed_angle)
         agent_heading_2_other = find_angle_diff(agent_speed_angles, p_oa_angle)
         r = agent_state[8] + other_agent_state[8] + GETTING_CLOSE_RANGE
-        coll_angle = abs(np.arcsin(min(0.95, r / np.linalg.norm(\
-                        agent_state[0:2]-other_agent_state[0:2]))))
-        
+        coll_angle = abs(
+            np.arcsin(
+                min(
+                    0.95,
+                    r
+                    / np.linalg.norm(
+                        agent_state[0:2] - other_agent_state[0:2]
+                    ),
+                )
+            )
+        )
+
         # other agent in front, zero out other agent's speed in the same direction
-        front_inds = np.where( (abs(agent_heading_2_other)<coll_angle) & \
-            (abs(heading_diff) < np.pi/2.0))[0]
-        if len(front_inds)>0:
+        front_inds = np.where(
+            (abs(agent_heading_2_other) < coll_angle)
+            & (abs(heading_diff) < np.pi / 2.0)
+        )[0]
+        if len(front_inds) > 0:
             # print other_agent_vels[front_inds,:].shape
             # print other_agent_vels[front_inds,:].shape
             # print np.matlib.repmat(np.linalg.norm(agent_vels[front_inds,:], axis=1),2,1).transpose().shape
             # print agent_vels[front_inds,:].shape
             dot_product = np.sum(agent_vels * other_agent_vels, axis=1)
-            valid_inds = np.where(agent_vels[:,0]>EPS)[0]
-            dot_product[valid_inds] /= np.linalg.norm(agent_vels[valid_inds,:], axis=1)
-            other_agent_vels[front_inds,:] = other_agent_vels[front_inds,:] -  \
-                np.matlib.repmat(dot_product[front_inds], 2, 1).transpose()\
-                * agent_vels[front_inds,:] / 2.0
+            valid_inds = np.where(agent_vels[:, 0] > EPS)[0]
+            dot_product[valid_inds] /= np.linalg.norm(
+                agent_vels[valid_inds, :], axis=1
+            )
+            other_agent_vels[front_inds, :] = (
+                other_agent_vels[front_inds, :]
+                - np.tile(dot_product[front_inds], (2, 1)).transpose()
+                * agent_vels[front_inds, :]
+                / 2.0
+            )
 
         # analytical version
-        x1 = agent_state[0:2]                      # shape = (2,)
-        x2 = x1 + min(1.0, delta_t) * agent_vels             # shape = (num_actions, 2)
-        y1 = other_agent_state[0:2]                # shape = (2,)
-        y2 = y1 + min(1.0, delta_t) * other_agent_vels     # shape = (num_actions, 2)
+        x1 = agent_state[0:2]  # shape = (2,)
+        x2 = x1 + min(1.0, delta_t) * agent_vels  # shape = (num_actions, 2)
+        y1 = other_agent_state[0:2]  # shape = (2,)
+        y2 = (
+            y1 + min(1.0, delta_t) * other_agent_vels
+        )  # shape = (num_actions, 2)
         # end points
         # if np.linalg.norm(x1-y1) < radius:
         #   return np.ones((num_actions,), dtype=bool)
         # if_collide = np.linalg.norm(x2-y2, axis=1) < radius
 
         # # critical points (where d/dt = 0)
         # z_bar = (x2 - x1) - (y2 - y1)             # shape = (num_actions, 2)
         # inds = np.where((np.linalg.norm(z_bar,axis=1)>0) & (if_collide == False))[0]
         # t_bar = - np.sum((x1-y1) * z_bar[inds,:], axis=1) \
         #       / np.sum(z_bar[inds,:] * z_bar[inds,:], axis=1)
         # t_bar_rep = np.matlib.repmat(t_bar, 2, 1).transpose()
         # dist_bar = np.linalg.norm(x1 + (x2[inds,:]-x1) * t_bar_rep \
         #         - y1 - (y2-y1) * t_bar_rep, axis=1)
-        # if_collide[inds] = np.logical_and(np.logical_and(dist_bar < radius,  t_bar > 0), t_bar < 1.0) 
+        # if_collide[inds] = np.logical_and(np.logical_and(dist_bar < radius,  t_bar > 0), t_bar < 1.0)
 
         min_dists = gen_tc.find_dist_between_segs(x1, x2, y1, y2)
 
         # min_dists = min_dists - 0.03 * np.random.random(min_dists.shape)
 
         # if other agent in back, and will run into the agent
         # p_ao_angle = np.arctan2(agent_state[1] - other_agent_state[1], \
         #   agent_state[0] - other_agent_state[0])
         # other_heading_2_agent = find_angle_diff(other_speed_angle, p_ao_angle)
         # back_inds = np.where( (abs(other_heading_2_agent)<coll_angle) & \
         #   (abs(heading_diff) < np.pi/2.0))[0]
         # back_inds = np.setdiff1d(back_inds, front_inds)
         # min_dists[back_inds] += GETTING_CLOSE_RANGE
 
-
-
         # print find_dist_between_segs(x1, x2, y1, y2)
         # print if_collide_2
         # print radius
         # print if_collide
         # print if_collide - if_collide_2
         # assert(np.all(if_collide == if_collide_2))
-        cur_dist = np.linalg.norm(x1-y1)
+        cur_dist = np.linalg.norm(x1 - y1)
         if cur_dist < radius:
             if_collide[:] = True
         else:
             if_collide = min_dists < radius
         # dist_future = x2 - (0.75 * y1 + 0.25 * y2)
         # dist_future = np.linalg.norm(dist_future, axis=1)
         # min_dists = np.minimum(dist_future, min_dists)
@@ -1560,17 +2008,17 @@
 
         # sampling vector version
         # incr = 0.25 #np.min((0.25, delta_t))
         # T = np.linspace(0, delta_t, num=np.ceil((delta_t+0.0001) / incr))
         # for t in T:
         #   dist_vec = agent_vels * t + np.matlib.repmat(agent_state[0:2] - \
         #               (other_agent_state[0:2] + other_agent_v * t), num_actions, 1)
-        #   if_collide_pt = np.linalg.norm(dist_vec, axis=1) < radius 
+        #   if_collide_pt = np.linalg.norm(dist_vec, axis=1) < radius
         #   if_collide = np.logical_or(if_collide, if_collide_pt)
-        
+
         # sampling loop version
         # for i in range(num_actions):
         #   t = 0.0
         #   while t <= delta_t:
         #       agent_pos = agent_state[0:2] + agent_vels[i,:] * t
         #       other_agent_pos = other_agent_state[0:2] + other_agent_v * t
         #       if self.if_pos_collide(agent_pos, other_agent_pos, radius):
@@ -1595,120 +2043,144 @@
 
     def if_pos_collide(self, agent1_pos, agent2_pos, radius):
         if np.linalg.norm(agent1_pos - agent2_pos) < radius:
             return True
         return False
 
     # query state values from the neural network
-    # don't consider terminal state 
+    # don't consider terminal state
     # (expect the neural network to have learned values of the terminal states)
     def find_states_values(self, agent_states, other_agents_state):
         # print 'agent_states in find_states_values', agent_states
         # print 'other_agent_state', other_agent_state
         if agent_states.ndim == 1:
-            ref_prll, ref_orth, state_nn = \
-                pedData.rawState_2_agentCentricState( \
-                agent_states, other_agents_state, self.num_agents)
+            ref_prll, ref_orth, state_nn = (
+                pedData.rawState_2_agentCentricState(
+                    agent_states, other_agents_state, self.num_agents
+                )
+            )
 
             # print("state_nn:", state_nn)
             # try upper bounding with max
-            value = np.squeeze(self.nn.make_prediction_raw(state_nn).clip(min=-0.25, max=1.0))
+            value = np.squeeze(
+                self.nn.make_prediction_raw(state_nn).clip(min=-0.25, max=1.0)
+            )
             # print 'state_nn', state_nn
             # print('before, value', value)
             upper_bnd = GAMMA ** (state_nn[0] / DT_NORMAL)
             value = min(upper_bnd, value)
             # print('after, value', value)
 
             return value
         else:
             num_states = agent_states.shape[0]
             # states_nn = np.zeros((num_states, 14))
             # for i in range(num_states):
             #   ref_prll, ref_orth, states_nn[i,:] = \
             #       pedData.rawState_2_agentCentricState( \
             #       agent_states[i,:], other_agent_state)
-            ref_prll_vec, ref_orth_vec, states_nn = \
-            pedData.rawStates_2_agentCentricStates(\
-                agent_states, other_agents_state, self.num_agents)
+            ref_prll_vec, ref_orth_vec, states_nn = (
+                pedData.rawStates_2_agentCentricStates(
+                    agent_states, other_agents_state, self.num_agents
+                )
+            )
 
             # print 'states_nn[0,:]', states_nn[0,:]
-            values = np.squeeze(self.nn.make_prediction_raw(states_nn).clip(min=-0.25, max=1.0))
+            values = np.squeeze(
+                self.nn.make_prediction_raw(states_nn).clip(min=-0.25, max=1.0)
+            )
             # print 'states_nn', states_nn
             # print 'before, values', values
-            upper_bnd = GAMMA ** (states_nn[:,0] / DT_NORMAL)
+            upper_bnd = GAMMA ** (states_nn[:, 0] / DT_NORMAL)
             # print 'upper_bnd', upper_bnd
             # print 'values', values
             values = np.minimum(upper_bnd, values)
             # print 'values[-1]', values
             # raw_input()
 
             return values
 
-
-    def find_agent_next_state(self, agent_state, other_agents_state, \
-            other_agents_action, dt):
-        action_theta = self.find_next_action(agent_state, \
-            other_agents_state, other_agents_action)
+    def find_agent_next_state(
+        self, agent_state, other_agents_state, other_agents_action, dt
+    ):
+        action_theta = self.find_next_action(
+            agent_state, other_agents_state, other_agents_action
+        )
         next_state = self.update_state(agent_state, action_theta, dt)
         return next_state
 
-    def find_agent_next_rand_state(self, agent_state, other_agents_state, random_action_theta, dt):
+    def find_agent_next_rand_state(
+        self, agent_state, other_agents_state, random_action_theta, dt
+    ):
         # action_theta = self.find_rand_action(agent_state, other_agent_state)
         next_state = self.update_state(agent_state, random_action_theta, dt)
         return next_state
 
-
-
-    def testcase_2_agentStates(self, test_case, ifRandSpeed=False, ifRandHeading=False):
-        assert(test_case[0, 5] > 0.1 or ifRandSpeed==True)
+    def testcase_2_agentStates(
+        self, test_case, ifRandSpeed=False, ifRandHeading=False
+    ):
+        assert test_case[0, 5] > 0.1 or ifRandSpeed == True
 
         num_agents = len(test_case)
         agents_states = []
 
         for i in range(num_agents):
-            agent_state = np.zeros((10,)); 
-            agent_state[0:2] = test_case[i,0:2]; agent_state[6:8] = test_case[i,2:4];
+            agent_state = np.zeros((10,))
+            agent_state[0:2] = test_case[i, 0:2]
+            agent_state[6:8] = test_case[i, 2:4]
             agent_state[9] = 0.0
             if ifRandSpeed == True:
-                agent_state[5] = np.random.rand() * (1.5-0.1) + 0.1
-                agent_state[8] = 0.3 + np.random.uniform(0,0.2)
+                agent_state[5] = np.random.rand() * (1.5 - 0.1) + 0.1
+                agent_state[8] = 0.3 + np.random.uniform(0, 0.2)
             else:
-                agent_state[5] = test_case[i,4]
-                agent_state[8] = test_case[i,5]
+                agent_state[5] = test_case[i, 4]
+                agent_state[8] = test_case[i, 5]
 
             # assume originally facing the goal direction
             if ifRandHeading == True:
                 agent_state[4] = np.random.rand() * 2 * np.pi - np.pi
             else:
-                agent_state[4] = np.arctan2(test_case[i,3]-test_case[i,1], \
-                        test_case[i,2]-test_case[i,0])
+                agent_state[4] = np.arctan2(
+                    test_case[i, 3] - test_case[i, 1],
+                    test_case[i, 2] - test_case[i, 0],
+                )
 
             # if agent is not stationary, assume it's travelling along its initially heading
             if np.linalg.norm(agent_state[0:2] - agent_state[6:8]) > EPS:
-                heading_dir = np.array([np.cos(agent_state[4]), np.sin(agent_state[4])])
+                heading_dir = np.array(
+                    [np.cos(agent_state[4]), np.sin(agent_state[4])]
+                )
                 # agent_state[2:4] = agent_state[5] * heading_dir
 
             try:
-                assert(agent_state[5] > 0.05)
+                assert agent_state[5] > 0.05
             except:
                 print(agent_state)
                 print(test_case)
-                assert(0)
+                assert 0
             agents_states.append(agent_state)
 
         return agents_states
 
     # generate a trajectory using the current value neural network
     # test_case: [ [start_x, start_y, end_x, end_y, desired_speed, radius],
     #              [start_x, start_y, end_x, end_y, desired_speed, radius] ]
     # rl_epsilon: explore a new action with rl_epsilon probability
     # ifRandSpeed: whether generate  random [desired_speed and radius] for test case
     # figure_name: name of figure, "no_plot" for no figure
-    def generate_traj(self, test_case, rl_epsilon=0.0, \
-            ifRandSpeed=False, figure_name=None, stopOnCollision=True, ifRandHeading=False, ifNonCoop=False):
+    def generate_traj(
+        self,
+        test_case,
+        rl_epsilon=0.0,
+        ifRandSpeed=False,
+        figure_name=None,
+        stopOnCollision=True,
+        ifRandHeading=False,
+        ifNonCoop=False,
+    ):
         time_start = time.time()
         num_agents = test_case.shape[0]
         time_vec = []
         dt_vec = []
         traj_raw_multi = []
         agent_num_thres = self.num_agents / 4.0
         if_non_coop_vec = np.zeros((num_agents,), dtype=bool)
@@ -1716,74 +2188,85 @@
             if_non_coop_vec = np.random.randint(2, size=(num_agents,))
 
         for i in range(num_agents):
             traj_raw_multi.append([])
         time_to_complete = np.zeros((num_agents,))
         agents_dt = np.ones((num_agents,))
         if_completed_vec = np.zeros((num_agents,), dtype=bool)
-        time_past_one_ind = 0 # ind of time one second ago in time_vec
+        time_past_one_ind = 0  # ind of time one second ago in time_vec
         filtered_actions_theta = [None] * num_agents
         filtered_actions_theta_close = [None] * num_agents
         filtered_actions_theta_far = [None] * num_agents
         dist_mat = np.zeros((num_agents, num_agents))
 
         # initialize
-        agents_states = self.testcase_2_agentStates(test_case, ifRandSpeed, ifRandHeading)
+        agents_states = self.testcase_2_agentStates(
+            test_case, ifRandSpeed, ifRandHeading
+        )
         next_agents_states = copy.deepcopy(agents_states)
         agents_speeds = np.zeros((num_agents,))
         max_t_vec = np.zeros((num_agents,))
         for i in range(num_agents):
             agents_speeds[i] = agents_states[i][5]
-            max_t_vec[i] = 3.0 * (np.linalg.norm(test_case[i, 2:4] - test_case[i, 0:2]) / agents_speeds[i])
+            max_t_vec[i] = 3.0 * (
+                np.linalg.norm(test_case[i, 2:4] - test_case[i, 0:2])
+                / agents_speeds[i]
+            )
         max_t = np.amax(max_t_vec)
 
-        max_t = 0.2 ###################### delete later
-
+        max_t = 0.2  ###################### delete later
 
         dt_nominal = 0.1
         t = 0
 
         # for epsilon random action
         rand_action_time_thres = 0.5
         if_agents_rand_action = np.zeros((num_agents,), dtype=bool)
-        agents_rand_action_duration = np.zeros((num_agents, ))
-        agents_rand_action_theta = np.zeros((num_agents,2))
+        agents_rand_action_duration = np.zeros((num_agents,))
+        agents_rand_action_theta = np.zeros((num_agents, 2))
 
         while True:
             # append to stats
             time_vec.append(t)
             for i in range(num_agents):
                 traj_raw_multi[i].append(agents_states[i].copy())
 
             # compute if completed and dt
             # dt_nominal = 0.1
             for i in range(num_agents):
-                dist_2_goal = np.linalg.norm(agents_states[i][0:2] - agents_states[i][6:8])
+                dist_2_goal = np.linalg.norm(
+                    agents_states[i][0:2] - agents_states[i][6:8]
+                )
                 if_completed_vec[i] = dist_2_goal < DIST_2_GOAL_THRES
-                agents_dt[i] = dist_2_goal/agents_speeds[i]
+                agents_dt[i] = dist_2_goal / agents_speeds[i]
                 if if_completed_vec[i]:
                     agents_states[i][2:4] = 0
                     agents_dt[i] = 1
-            dt = min(dt_nominal,np.amin(agents_dt))
+            dt = min(dt_nominal, np.amin(agents_dt))
             t += dt
             dt_vec.append(dt)
-            
+
             # collision (TODO)
             for i in range(num_agents):
                 for j in range(i):
-                    dist_mat[i,j] = np.linalg.norm(agents_states[i][0:2] - agents_states[j][0:2]) - \
-                                    agents_states[i][8] - agents_states[j][8]
-                    dist_mat[j,i] = dist_mat[i,j]
+                    dist_mat[i, j] = (
+                        np.linalg.norm(
+                            agents_states[i][0:2] - agents_states[j][0:2]
+                        )
+                        - agents_states[i][8]
+                        - agents_states[j][8]
+                    )
+                    dist_mat[j, i] = dist_mat[i, j]
             min_sepDist = np.min(dist_mat)
             if stopOnCollision and min_sepDist < 0:
                 break
 
             # time too long, probably diverged
             if t > max_t:
-                break 
+                break
 
             # completed
             if np.all(if_completed_vec):
                 break
 
             # idling, not reaching goal (TODO)
 
@@ -1792,222 +2275,310 @@
             while t - time_vec[time_past_one_ind] > 0.45:
                 time_past_one_ind += 1
             dt_past_vec = np.asarray(dt_vec[time_past_one_ind:])
 
             for i in range(num_agents):
                 if len(time_vec) != 0:
                     # if np.random.rand()>0.5 or filtered_actions_theta_close[i] is None:
-                    past_vel = np.asarray(traj_raw_multi[i][time_past_one_ind:])[:,2:5]
+                    past_vel = np.asarray(
+                        traj_raw_multi[i][time_past_one_ind:]
+                    )[:, 2:5]
                     # filtered_actions_theta[i] = nn_nav.filter_vel(dt_past_vec, past_vel)
-                    filtered_actions_theta_close[i] = filter_vel(dt_past_vec, past_vel,ifClose=True)
-                    filtered_actions_theta_far[i] = filter_vel(dt_past_vec, past_vel,ifClose=False)
+                    filtered_actions_theta_close[i] = filter_vel(
+                        dt_past_vec, past_vel, ifClose=True
+                    )
+                    filtered_actions_theta_far[i] = filter_vel(
+                        dt_past_vec, past_vel, ifClose=False
+                    )
 
             # propagate forward in time
             rl_random = np.random.rand()
             for i in range(num_agents):
                 agent_state = agents_states[i]
                 if not if_completed_vec[i]:
-                    other_agents_states = [x for j, x in enumerate(agents_states) if j!=i]
+                    other_agents_states = [
+                        x for j, x in enumerate(agents_states) if j != i
+                    ]
                     # other_agents_actions = [x for j, x in enumerate(filtered_actions_theta) if i!=j]
                     other_agents_actions = []
                     for j in range(num_agents):
                         if j != i:
-                            if dist_mat[i,j] < 0.5:
-                                other_agents_actions.append(filtered_actions_theta_close[j])
+                            if dist_mat[i, j] < 0.5:
+                                other_agents_actions.append(
+                                    filtered_actions_theta_close[j]
+                                )
                             else:
-                                other_agents_actions.append(filtered_actions_theta_far[j])
+                                other_agents_actions.append(
+                                    filtered_actions_theta_far[j]
+                                )
 
                     # non-cooperative (for plotting)
                     if i > 0 and if_non_coop_vec[i] == True:
-                        desired_velocity = self.computePrefVel(agent_state[0:2], \
-                                    agent_state[6:8], agent_state[5])
+                        desired_velocity = self.computePrefVel(
+                            agent_state[0:2], agent_state[6:8], agent_state[5]
+                        )
                         next_agents_states[i] = agent_state.copy()
                         next_agents_states[i][2:4] = desired_velocity
                         next_agents_states[i][0:2] += dt * agent_state[2:4]
-                        next_agents_states[i][4] = np.arctan2(desired_velocity[1], desired_velocity[0])
+                        next_agents_states[i][4] = np.arctan2(
+                            desired_velocity[1], desired_velocity[0]
+                        )
 
                     else:
                         # cooperative
-                        if if_agents_rand_action[i] == False and rl_random < rl_epsilon \
-                            and np.linalg.norm(agent_state[0:2] - agent_state[6:8]) > 1.0 and i < agent_num_thres: # only first agent freeze
+                        if (
+                            if_agents_rand_action[i] == False
+                            and rl_random < rl_epsilon
+                            and np.linalg.norm(
+                                agent_state[0:2] - agent_state[6:8]
+                            )
+                            > 1.0
+                            and i < agent_num_thres
+                        ):  # only first agent freeze
                             if_agents_rand_action[i] = True
                             agents_rand_action_duration[i] = 0.0
                             if i < agent_num_thres:
-                                agents_rand_action_theta[i] = self.find_rand_action(agent_state, other_agents_states, \
-                                other_agents_action = other_agents_actions, isBestAction=False)
-                            else: 
-                                agents_rand_action_theta[i] = self.find_rand_action(agent_state, other_agents_states, \
-                                other_agents_action = other_agents_actions, isBestAction=True)
-                        elif agents_rand_action_duration[i] > rand_action_time_thres:
+                                agents_rand_action_theta[i] = (
+                                    self.find_rand_action(
+                                        agent_state,
+                                        other_agents_states,
+                                        other_agents_action=other_agents_actions,
+                                        isBestAction=False,
+                                    )
+                                )
+                            else:
+                                agents_rand_action_theta[i] = (
+                                    self.find_rand_action(
+                                        agent_state,
+                                        other_agents_states,
+                                        other_agents_action=other_agents_actions,
+                                        isBestAction=True,
+                                    )
+                                )
+                        elif (
+                            agents_rand_action_duration[i]
+                            > rand_action_time_thres
+                        ):
                             if_agents_rand_action[i] = False
 
                         if if_agents_rand_action[i] == True:
-                            next_agents_states[i] = self.find_agent_next_rand_state(\
-                                agent_state, other_agents_states, agents_rand_action_theta[i], dt)
+                            next_agents_states[i] = (
+                                self.find_agent_next_rand_state(
+                                    agent_state,
+                                    other_agents_states,
+                                    agents_rand_action_theta[i],
+                                    dt,
+                                )
+                            )
                             agents_rand_action_duration[i] += dt
                         else:
-                            next_agents_states[i] = self.find_agent_next_state(\
-                                agent_state, other_agents_states, other_agents_actions, dt)
+                            next_agents_states[i] = self.find_agent_next_state(
+                                agent_state,
+                                other_agents_states,
+                                other_agents_actions,
+                                dt,
+                            )
 
                     time_to_complete[i] = t
                 else:
                     next_agents_states[i] = agent_state.copy()
 
             agents_states = copy.deepcopy(next_agents_states)
 
         # add time to trajectory list
         traj_raw_multi = [time_vec] + traj_raw_multi
         for i, vec in enumerate(traj_raw_multi):
             traj_raw_multi[i] = np.asarray(vec)
 
-
         # print 'traj_raw', traj_raw
         if figure_name != "no_plot":
-            title_string = 'total time: %f' % (np.sum(time_to_complete))
-            print('time_to_complete', time_to_complete)
-            pedData.plot_traj_raw_multi(traj_raw_multi, title_string, figure_name)
-            print('finished generating trajectory with %d points in %fs' % \
-                (len(traj_raw_multi[0]), time.time()-time_start))
+            title_string = "total time: %f" % (np.sum(time_to_complete))
+            print("time_to_complete", time_to_complete)
+            pedData.plot_traj_raw_multi(
+                traj_raw_multi, title_string, figure_name
+            )
+            print(
+                "finished generating trajectory with %d points in %fs"
+                % (len(traj_raw_multi[0]), time.time() - time_start)
+            )
         return traj_raw_multi, time_to_complete
 
     # find preferred velocity vector (toward goal at desired(nominal) speed)
     def computePrefVel(self, cur_state, goal, nom_speed):
         pref_vec = goal - cur_state
         # print 'goal, cur_state', goal, cur_state
         # print 'nom_speed', nom_speed
         # print 'pref_vec before normalizing', pref_vec
         pref_speed = np.linalg.norm(pref_vec)
-        if pref_speed > 0: 
+        if pref_speed > 0:
             pref_vec = pref_vec / pref_speed * nom_speed
         else:
             pref_vec = np.array([EPS, 0])
         # print 'pref_vec', pref_vec
         return pref_vec
 
     # compute agent_centric_states
     def find_bad_inds(self, agent_centric_states):
         # closest other agent is the first agent
         # dist_2_others (see README.txt)
-        agent_vel = agent_centric_states[:,4:6]
+        agent_vel = agent_centric_states[:, 4:6]
         agent_speed = np.linalg.norm(agent_vel, axis=1)
-        agent_vx = agent_vel[:,0]
-        agent_vy = agent_vel[:,1]
-        agent_heading = agent_centric_states[:,3]
-
-        dist_2_goal = agent_centric_states[:,0]
-        other_pos = agent_centric_states[:,9:11]
-        other_px = other_pos[:,0]
-        other_py = other_pos[:,1]
-
-        other_vel = agent_centric_states[:,7:9]
-        other_vx = other_vel[:,0]
-        other_vy = other_vel[:,1]
+        agent_vx = agent_vel[:, 0]
+        agent_vy = agent_vel[:, 1]
+        agent_heading = agent_centric_states[:, 3]
+
+        dist_2_goal = agent_centric_states[:, 0]
+        other_pos = agent_centric_states[:, 9:11]
+        other_px = other_pos[:, 0]
+        other_py = other_pos[:, 1]
+
+        other_vel = agent_centric_states[:, 7:9]
+        other_vx = other_vel[:, 0]
+        other_vy = other_vel[:, 1]
         other_speed = np.linalg.norm(other_vel, axis=1)
         other_heading = np.arctan2(other_vy, other_vx)
 
         rel_vel = agent_vel - other_vel
-        rel_vel_angle = np.arctan2(rel_vel[:,1], rel_vel[:,0])
-        rel_pos_angle = np.arctan2(0-other_py, 0-other_px)
+        rel_vel_angle = np.arctan2(rel_vel[:, 1], rel_vel[:, 0])
+        rel_pos_angle = np.arctan2(0 - other_py, 0 - other_px)
         rot_angle = find_angle_diff(rel_vel_angle, rel_pos_angle)
 
         bad_inds_oppo = []
         bad_inds_same = []
         bad_inds_tangent = []
-        if self.passing_side == 'right':
+        if self.passing_side == "right":
             # opposite  direction
             # same direction
             # faster
-            bad_inds_same_fast = np.where( (dist_2_goal > 1) & (other_speed > EPS) & \
-                (agent_speed > EPS) & \
-                (agent_speed > other_speed + 0.1) & \
-                (other_py > -0.5) & (other_py < 2) & \
-                (other_px > 0) & (other_px < 3) & \
-                (agent_heading < 0) & \
-                (abs(other_heading) < np.pi/6.0))[0]
+            bad_inds_same_fast = np.where(
+                (dist_2_goal > 1)
+                & (other_speed > EPS)
+                & (agent_speed > EPS)
+                & (agent_speed > other_speed + 0.1)
+                & (other_py > -0.5)
+                & (other_py < 2)
+                & (other_px > 0)
+                & (other_px < 3)
+                & (agent_heading < 0)
+                & (abs(other_heading) < np.pi / 6.0)
+            )[0]
             # slower
-            bad_inds_same_slow = np.where( (dist_2_goal > 1) & (other_speed > EPS) & \
-                (agent_speed > EPS) & \
-                (agent_speed < other_speed - 0.1) & \
-                (other_py < 0) & (other_py > -2) & \
-                (other_px < 0) & (other_px > -3) & \
-                (agent_heading > 0) & \
-                (abs(other_heading) < np.pi/6.0))[0]
+            bad_inds_same_slow = np.where(
+                (dist_2_goal > 1)
+                & (other_speed > EPS)
+                & (agent_speed > EPS)
+                & (agent_speed < other_speed - 0.1)
+                & (other_py < 0)
+                & (other_py > -2)
+                & (other_px < 0)
+                & (other_px > -3)
+                & (agent_heading > 0)
+                & (abs(other_heading) < np.pi / 6.0)
+            )[0]
 
             bad_inds_same = np.union1d(bad_inds_same_fast, bad_inds_same_slow)
 
             # opposite direction
-            bad_inds_oppo = np.where( (dist_2_goal > 1) & (other_speed > EPS) & \
-                (agent_speed > EPS) & \
-                (other_py < 0) & (other_py > -2) & \
-                (other_px > 0) & (other_px < 5) & \
-                (agent_heading > EPS) & \
-                (other_heading < -5.0*np.pi/6.0))[0]
+            bad_inds_oppo = np.where(
+                (dist_2_goal > 1)
+                & (other_speed > EPS)
+                & (agent_speed > EPS)
+                & (other_py < 0)
+                & (other_py > -2)
+                & (other_px > 0)
+                & (other_px < 5)
+                & (agent_heading > EPS)
+                & (other_heading < -5.0 * np.pi / 6.0)
+            )[0]
 
             # tangent direction
-            agent_speed = agent_centric_states[0,1]
+            agent_speed = agent_centric_states[0, 1]
             other_rel_dist = np.linalg.norm(other_pos, axis=1)
-            bad_inds_tangent = np.where( (dist_2_goal > 1) & (other_speed > EPS) & \
-                (agent_speed > EPS) & \
-                # (other_py < 3 * agent_speed) & (other_py > -3 * agent_speed) & \
+            bad_inds_tangent = np.where(
+                (dist_2_goal > 1)
+                & (other_speed > EPS)
+                & (agent_speed > EPS)
+                &  # (other_py < 3 * agent_speed) & (other_py > -3 * agent_speed) & \
                 # (other_px > 0 * agent_speed) & (other_px < 3 * agent_speed) & \
-                (other_px > 0) & (other_rel_dist < 3) & \
-                (rot_angle < 0) & \
-                (abs(other_heading) > np.pi/4.0) & \
-                (agent_speed > other_speed - 0.2)) [0]
-                # & (abs(other_heading) < 5.0* np.pi/6.0) )[0]
-
+                (other_px > 0)
+                & (other_rel_dist < 3)
+                & (rot_angle < 0)
+                & (abs(other_heading) > np.pi / 4.0)
+                & (agent_speed > other_speed - 0.2)
+            )[0]
+            # & (abs(other_heading) < 5.0* np.pi/6.0) )[0]
 
-        elif self.passing_side == 'left':
+        elif self.passing_side == "left":
             # opposite  direction
             # same direction
             # faster
-            bad_inds_same_fast = np.where( (dist_2_goal > 1) & (other_speed > EPS) & \
-                (agent_speed > EPS) & \
-                (agent_speed > other_speed + 0.1) & \
-                (other_py > -2) & (other_py < 0.5) & \
-                (other_px > 0) & (other_px < 3) & \
-                (agent_heading > 0) & \
-                (abs(other_heading) < np.pi/6.0))[0]
+            bad_inds_same_fast = np.where(
+                (dist_2_goal > 1)
+                & (other_speed > EPS)
+                & (agent_speed > EPS)
+                & (agent_speed > other_speed + 0.1)
+                & (other_py > -2)
+                & (other_py < 0.5)
+                & (other_px > 0)
+                & (other_px < 3)
+                & (agent_heading > 0)
+                & (abs(other_heading) < np.pi / 6.0)
+            )[0]
             # slower
-            bad_inds_same_slow = np.where( (dist_2_goal > 1) & (other_speed > EPS) & \
-                (agent_speed > EPS) & \
-                (agent_speed < other_speed - 0.1) & \
-                (other_py < 2) & (other_py > 0) & \
-                (other_px < 0) & (other_px > -3) & \
-                (agent_heading > 0) & \
-                (abs(other_heading) < np.pi/6.0))[0]
+            bad_inds_same_slow = np.where(
+                (dist_2_goal > 1)
+                & (other_speed > EPS)
+                & (agent_speed > EPS)
+                & (agent_speed < other_speed - 0.1)
+                & (other_py < 2)
+                & (other_py > 0)
+                & (other_px < 0)
+                & (other_px > -3)
+                & (agent_heading > 0)
+                & (abs(other_heading) < np.pi / 6.0)
+            )[0]
 
             bad_inds_same = np.union1d(bad_inds_same_fast, bad_inds_same_slow)
 
             # opposite direction
-            bad_inds_oppo = np.where( (dist_2_goal > 1) & (other_speed > EPS) & \
-                (agent_speed > EPS) & \
-                (other_py < 2) & (other_py > 0) & \
-                (other_px > 0) & (other_px < 5) & \
-                (agent_heading < EPS) & \
-                (other_heading > 5.0*np.pi/6.0))[0]
+            bad_inds_oppo = np.where(
+                (dist_2_goal > 1)
+                & (other_speed > EPS)
+                & (agent_speed > EPS)
+                & (other_py < 2)
+                & (other_py > 0)
+                & (other_px > 0)
+                & (other_px < 5)
+                & (agent_heading < EPS)
+                & (other_heading > 5.0 * np.pi / 6.0)
+            )[0]
 
             # tangent direction
-            agent_speed = agent_centric_states[0,1]
+            agent_speed = agent_centric_states[0, 1]
             other_rel_dist = np.linalg.norm(other_pos, axis=1)
-            bad_inds_tangent = np.where( (dist_2_goal > 1) & (other_speed > EPS) & \
-                (agent_speed > EPS) & \
-                # (other_py < 3* agent_speed) & (other_py > -3* agent_speed) & \
+            bad_inds_tangent = np.where(
+                (dist_2_goal > 1)
+                & (other_speed > EPS)
+                & (agent_speed > EPS)
+                &  # (other_py < 3* agent_speed) & (other_py > -3* agent_speed) & \
                 # (other_px > 0* agent_speed) & (other_px < 3* agent_speed) & \
-                (other_px > 0) & (other_rel_dist < 3) & \
-                (rot_angle > 0) & \
-                (abs(other_heading) > np.pi/4.0) & \
-                (agent_speed > other_speed - 0.2))[0]
-                # (abs(other_heading) < 5.0* np.pi/6.0) )[0]
+                (other_px > 0)
+                & (other_rel_dist < 3)
+                & (rot_angle > 0)
+                & (abs(other_heading) > np.pi / 4.0)
+                & (agent_speed > other_speed - 0.2)
+            )[0]
+            # (abs(other_heading) < 5.0* np.pi/6.0) )[0]
 
         # return    [], bad_inds_same, []
-        return  bad_inds_oppo, bad_inds_same, bad_inds_tangent
+        return bad_inds_oppo, bad_inds_same, bad_inds_tangent
+
 
 # speed filter
-# input: past velocity in (x,y) at time_past 
+# input: past velocity in (x,y) at time_past
 # output: filtered velocity in (speed, theta)
 def filter_vel(dt_vec, agent_past_vel, ifClose=False):
     # if np.sum(dt_vec) == 0:
     #   print 'dt_vec', dt_vec
     #   print 'agent_past_vel_xy', agent_past_vel_xy
     #   assert(0)
 
@@ -2018,135 +2589,204 @@
     #   angle_diff_vec = find_angle_diff( agent_past_vel[1:,2], \
     #       agent_past_vel[0:-1,2] )
     #   if np.all(angle_diff_vec>-EPS) or np.all(angle_diff_vec<EPS):
     #       speed = np.linalg.norm(agent_past_vel[-1,0:2])
     #       angle = agent_past_vel[-1,2]
     #       return np.array([speed, angle])
 
-    if True: #ifClose == False:
-        agent_past_vel_xy = agent_past_vel[-2:,0:2]
-        agent_heading = agent_past_vel[-2:,2]
+    if True:  # ifClose == False:
+        agent_past_vel_xy = agent_past_vel[-2:, 0:2]
+        agent_heading = agent_past_vel[-2:, 2]
         dt_vec = dt_vec[-2:]
     else:
-        length = min(2, len(dt_vec)-1)
+        length = min(2, len(dt_vec) - 1)
         # length = len(dt_vec)-1
-        agent_past_vel_xy = agent_past_vel[-length:,0:2]
-        agent_heading = agent_past_vel[-length:,2]
+        agent_past_vel_xy = agent_past_vel[-length:, 0:2]
+        agent_heading = agent_past_vel[-length:, 2]
         dt_vec = dt_vec[-length:]
     # print 'len(dt_vec)', len(dt_vec)
 
-    average_x = np.sum(dt_vec * agent_past_vel_xy[:,0]) / np.sum(dt_vec)
-    average_y = np.sum(dt_vec * agent_past_vel_xy[:,1]) / np.sum(dt_vec)
+    average_x = np.sum(dt_vec * agent_past_vel_xy[:, 0]) / np.sum(dt_vec)
+    average_y = np.sum(dt_vec * agent_past_vel_xy[:, 1]) / np.sum(dt_vec)
     speeds = np.linalg.norm(agent_past_vel_xy, axis=1)
     # speed = np.mean(speeds)
     # speed = speeds[-1]
     # speed = np.linalg.norm(agent_past_vel_xy[-1,:])
     # assert(speed == speed1)
     speed = np.linalg.norm(np.array([average_x, average_y]))
     angle = np.arctan2(average_y, average_x)
 
     return np.array([speed, angle])
 
 
 # load NN_navigation
-def load_NN_navigation_value(file_dir, num_agents, mode, passing_side, filename=None, ifPrint=True):
-    ''' initializing neural network ''' 
+def load_NN_navigation_value(
+    file_dir, num_agents, mode, passing_side, filename=None, ifPrint=True
+):
+    """initializing neural network"""
     try:
         # Messed up from transfer into this directory structure. I don't plan to ever change these settings.
         # nn_training_param_ = pickle.load(open(file_dir+"/../../pickle_files/multi/nn_training_param.p", "rb"))
-        d = {'sgd_step_size': 0.5, 'sgd_step_c': 0.1, 'reg_lambda': 0.001, 'w_scale': 0.1, 'sgd_step_epsilon': 0.1, 'nb_iter': 1000, 'sgd_stepsize_mode': 'fixed_decay', 'sgd_batch_size': 500}
-        nn_training_param = NN_training_param(d['sgd_step_size'],d['reg_lambda'], d['nb_iter'], d['sgd_batch_size'], d['w_scale'])
-        assert(0)
+        d = {
+            "sgd_step_size": 0.5,
+            "sgd_step_c": 0.1,
+            "reg_lambda": 0.001,
+            "w_scale": 0.1,
+            "sgd_step_epsilon": 0.1,
+            "nb_iter": 1000,
+            "sgd_stepsize_mode": "fixed_decay",
+            "sgd_batch_size": 500,
+        }
+        nn_training_param = NN_training_param(
+            d["sgd_step_size"],
+            d["reg_lambda"],
+            d["nb_iter"],
+            d["sgd_batch_size"],
+            d["w_scale"],
+        )
+        assert 0
     except AssertionError:
-        sgd_step_size = 10.0/20.0
-        reg_lambda = 1.0/1000.0
+        sgd_step_size = 10.0 / 20.0
+        reg_lambda = 1.0 / 1000.0
         nb_iter = 1000
         sgd_batch_size = 500
         w_scale = 0.1
-        sgd_stepsize_mode = 'training data' 
+        sgd_stepsize_mode = "training data"
         sgd_step_c = 0.1
         sgd_step_epsilon = 0.1
 
-        nn_training_param = nn.NN_training_param(sgd_step_size, reg_lambda, nb_iter, sgd_batch_size, w_scale)
-        with open(file_dir+"/../../pickle_files/multi/nn_training_param.p", "wb") as f:
+        nn_training_param = nn.NN_training_param(
+            sgd_step_size, reg_lambda, nb_iter, sgd_batch_size, w_scale
+        )
+        with open(
+            file_dir + "/../../pickle_files/multi/nn_training_param.p", "wb"
+        ) as f:
             pickle.dump(nn_training_param, f)
 
-    nn_navigation = NN_navigation_value(num_agents, nn_training_param, mode=mode, passing_side=passing_side)
-    
+    nn_navigation = NN_navigation_value(
+        num_agents, nn_training_param, mode=mode, passing_side=passing_side
+    )
 
-    ''' load nn_navigation '''
+    """ load nn_navigation """
     if filename is None:
-        nn_filename = file_dir + "/../../pickle_files/multi/%d_agents_nn_regr_value_data.p" % num_agents
-        print('loading NN trained on cadrl at ' + nn_filename)
+        nn_filename = (
+            file_dir
+            + "/../../pickle_files/multi/%d_agents_nn_regr_value_data.p"
+            % num_agents
+        )
+        print("loading NN trained on cadrl at " + nn_filename)
     else:
-        nn_filename = file_dir + "/../../pickle_files/multi/" + mode + "_" + passing_side + \
-            "/RL_selfplay/" + filename
+        nn_filename = (
+            file_dir
+            + "/../../pickle_files/multi/"
+            + mode
+            + "_"
+            + passing_side
+            + "/RL_selfplay/"
+            + filename
+        )
         if ifPrint:
-            print('loading NN trained on RL self-play ' + nn_filename)
+            print("loading NN trained on RL self-play " + nn_filename)
 
     # loading neural network
     try:
         # assert (0)
         nn_navigation.nn.load_neural_network(nn_filename)
     # train neural network for nn_navigation
     except AssertionError:
-        print('failed to load navigation value network',  nn_filename)
-        assert(0)
-        # load data 
-        dataset_ped_train, dataset_ped_test, dataset_ped_test_vel = load_ped_data(file_dir, num_agents)
+        print("failed to load navigation value network", nn_filename)
+        assert 0
+        # load data
+        dataset_ped_train, dataset_ped_test, dataset_ped_test_vel = (
+            load_ped_data(file_dir, num_agents)
+        )
         # train neural network
-        nn_navigation.train_neural_network(dataset_ped_train, dataset_ped_test, dataset_ped_test_vel)
+        nn_navigation.train_neural_network(
+            dataset_ped_train, dataset_ped_test, dataset_ped_test_vel
+        )
         nn_navigation.nn.save_neural_network(nn_filename)
-        print('saved nn_navigation')
+        print("saved nn_navigation")
 
     return nn_navigation
 
+
 def load_ped_data(file_dir, num_agents):
     try:
         # print 'num_agents', num_agents
-        dataset_ped_train = pickle.load(open(file_dir+\
-            "/../../pickle_files/multi/%d_agents_dataset_value_train.p"%num_agents, "rb"))
+        dataset_ped_train = pickle.load(
+            open(
+                file_dir
+                + "/../../pickle_files/multi/%d_agents_dataset_value_train.p"
+                % num_agents,
+                "rb",
+            )
+        )
         # print 'radius', dataset_ped_train[0][:,8:10]
-        dataset_ped_test = pickle.load(open(file_dir+\
-            "/../../pickle_files/multi/%d_agents_dataset_value_test.p"%num_agents, "rb"))
+        dataset_ped_test = pickle.load(
+            open(
+                file_dir
+                + "/../../pickle_files/multi/%d_agents_dataset_value_test.p"
+                % num_agents,
+                "rb",
+            )
+        )
         # print 'loaded dataset'
         num_train_pts = dataset_ped_train[0].shape[0]
         num_test_pts = dataset_ped_test[0].shape[0]
         # print 'here'
-        dataset_ped_test_vel = pickle.load(open(file_dir+\
-            "/../../pickle_files/multi/%d_agents_dataset_regr_test.p"%num_agents, "rb"))
+        dataset_ped_test_vel = pickle.load(
+            open(
+                file_dir
+                + "/../../pickle_files/multi/%d_agents_dataset_regr_test.p"
+                % num_agents,
+                "rb",
+            )
+        )
         dataset_ped_test_vel = dataset_ped_test_vel[1]
-        print('dataset contains %d pts, training set has %d pts, test set has %d pts' % \
-                (num_train_pts+num_test_pts, num_train_pts, num_test_pts))
+        print(
+            "dataset contains %d pts, training set has %d pts, test set has"
+            " %d pts"
+            % (num_train_pts + num_test_pts, num_train_pts, num_test_pts)
+        )
     except AssertionError:
-        print('pickle file does not exist, exiting')
-        assert(0)
+        print("pickle file does not exist, exiting")
+        assert 0
 
     return dataset_ped_train, dataset_ped_test, dataset_ped_test_vel
 
 
-if __name__ == '__main__':
-    print('hello world from nn_navigation_value_multi.py')
+if __name__ == "__main__":
+    print("hello world from nn_navigation_value_multi.py")
     file_dir = os.path.dirname(os.path.realpath(__file__))
-    plt.rcParams.update({'font.size': 18})
-    
-    ''' load nn_navigation_value and train if pickle file doesnot exist '''
+    plt.rcParams.update({"font.size": 18})
+
+    """ load nn_navigation_value and train if pickle file doesnot exist """
     num_agents = 4
-    mode = 'no_constr'
+    mode = "no_constr"
     # mode = 'rotate_constr'
-    nn_navigation = load_NN_navigation_value(file_dir, num_agents, mode, 'none')
-
-    ''' make prediction '''
-    dataset_ped_train, dataset_ped_test, dataset_ped_test_vel = load_ped_data(file_dir, num_agents)
+    nn_navigation = load_NN_navigation_value(
+        file_dir, num_agents, mode, "none"
+    )
+
+    """ make prediction """
+    dataset_ped_train, dataset_ped_test, dataset_ped_test_vel = load_ped_data(
+        file_dir, num_agents
+    )
     scores = nn_navigation.nn.make_prediction_raw(dataset_ped_test[0])
     # nn_navigation.plot_ped_testCase_rand(dataset_ped_test[0], scores, 'testing')
     # nn_navigation.plot_ped_testCase_rand(dataset_ped_test[0], scores, 'testing')
     # nn_navigation.plot_ped_testCase_rand(dataset_ped_test[0], scores, 'testing')
-    test_case = np.array([[-3.0, 0.0, 3.0, 0.0, 1.0, 0.4],\
-                                        [0.0, 3.0, 0.0, -3.0, 1.0, 0.4], \
-                                        [0.0, -3.0, 0.0, 3.0, 1.0, 0.4], \
-                                        [3.0, 0.0, -3.0, 0.0, 1.0, 0.4]])
+    test_case = np.array(
+        [
+            [-3.0, 0.0, 3.0, 0.0, 1.0, 0.4],
+            [0.0, 3.0, 0.0, -3.0, 1.0, 0.4],
+            [0.0, -3.0, 0.0, 3.0, 1.0, 0.4],
+            [3.0, 0.0, -3.0, 0.0, 1.0, 0.4],
+        ]
+    )
     nn_navigation.generate_traj(test_case[0:num_agents], ifRandSpeed=False)
-    test_case = gen_tc.generate_rand_test_case_multi(num_agents, 4.0, np.array([0.5,1.2]), np.array([0.3, 0.5]))
+    test_case = gen_tc.generate_rand_test_case_multi(
+        num_agents, 4.0, np.array([0.5, 1.2]), np.array([0.3, 0.5])
+    )
     nn_navigation.generate_traj(test_case)
 
     plt.show()
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/ros_nn.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/ros_nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # sys.path.append('multi/neural_networks')
 import nn_navigation_value_multi as nn_nav
 # minimax of 2 agent work
 # sys.path.append('pairwise/neural_networks')
 # import nn_navigation_value_pairwise_multi as nn_nav
 
 import numpy as np
-import numpy.matlib
 import pickle
 # from mpl_toolkits.mplot3d import Axes3D
 from matplotlib import cm
 import matplotlib.pyplot as plt
 from test_data import generate_spirals
 import copy
 import os
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/pedData_processing_multi_old.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/multi/pedData_processing_multi_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 import sys
 import os
 file_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(file_dir+'/../neural_networks')
 
 import numpy as np
-import numpy.matlib
 import pickle
 import matplotlib.pyplot as plt
 import time
 import global_var as gb
 import copy
 
 # setting up global variables
@@ -325,16 +324,16 @@
 
 def rawStates_2_agentCentricStates(agent_states, others_states, num_agents_in_network):
 	num_agents = len(others_states) + 1
 	assert(num_agents <= num_agents_in_network)
 	num_rawStates = agent_states.shape[0]
 	states_nn = np.zeros((num_rawStates, 7+8*(num_agents_in_network-1)))
 	for i in xrange(num_agents-1, num_agents_in_network-1):
-		states_nn[:,7+8*i:7+8*i+7] = np.matlib.repmat(\
-			np.array([0.0, 0.0, -8.0, 0.0, 0.35, 0.70, 8.0]), num_rawStates, 1)
+		states_nn[:,7+8*i:7+8*i+7] = np.tile(\
+			np.array([0.0, 0.0, -8.0, 0.0, 0.35, 0.70, 8.0]), (num_rawStates, 1))
 
 	# agent
 	# distance to goal
 	goal_direction = agent_states[:,6:8]-agent_states[:,0:2]
 	dist_to_goal = np.linalg.norm(goal_direction, axis=1)
 	# desired speed
 	pref_speed = agent_states[:,5]
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/multiagent_network_param.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/multiagent_network_param.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_spirals.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_spirals.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_symmetric_sinusoids.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_symmetric_sinusoids.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_sinusoids.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/test_data/generate_sinusoids.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network_regr_multi.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network_regr_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 #!/usr/bin/env python
 
-import numpy as np
-import numpy.matlib
-import pickle
-import matplotlib.pyplot as plt
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.test_data import generate_symmetric_sinusoids
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.nn_training_param import NN_training_param
-from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.multiagent_network_param import Multiagent_network_param
+import copy
 import os
+import pickle
 import time
-import copy
 
+import matplotlib.pyplot as plt
+import numpy as np
+
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.multiagent_network_param import (
+    Multiagent_network_param,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.nn_training_param import (
+    NN_training_param,
+)
+from gym_collision_avoidance.envs.policies.CADRL.scripts.neural_networks.test_data import (
+    generate_symmetric_sinusoids,
+)
 
 # fully connected nerual network with weight sharing for 
 # capturing symmetry in multiagent systems
 
 class Neural_network_regr_multi:
 	def __init__(self, nn_training_param, plotting_func=None, X_vis=None):
 		self.set_training_param(nn_training_param)
@@ -432,36 +438,36 @@
 
 	# scale X (xRaw_2_x)
 	def xRaw_2_x(self, X_raw):
 		if len(X_raw.shape) > 1:
 			nb_examples = X_raw.shape[0]
 		else:
 			nb_examples = 1
-		X = (X_raw - np.matlib.repmat(self.avg_vec, nb_examples, 1)) \
-			/ np.matlib.repmat(self.std_vec, nb_examples, 1)
+		X = (X_raw - np.tile(self.avg_vec, (nb_examples, 1))) \
+			/ np.tile(self.std_vec, (nb_examples, 1))
 		return X
 
 	# scale Y (yRaw_2_y)
 	def yRaw_2_y(self, Y_raw):
 		if len(Y_raw.shape) > 1:
 			nb_examples = Y_raw.shape[0]
 		else:
 			nb_examples = 1
-		Y = (Y_raw - np.matlib.repmat(self.output_avg_vec, nb_examples, 1)) \
-			/ np.matlib.repmat(self.output_std_vec, nb_examples, 1)
+		Y = (Y_raw - np.tile(self.output_avg_vec, (nb_examples, 1))) \
+			/ np.tile(self.output_std_vec, (nb_examples, 1))
 		return Y
 
 	# scale Y (y_2_yraw)
 	def y_2_yRaw(self, Y):
 		if len(Y.shape) > 1:
 			nb_examples = Y.shape[0]
 		else:
 			nb_examples = 1
-		Y_raw = Y * np.matlib.repmat(self.output_std_vec, nb_examples, 1) \
-			+ np.matlib.repmat(self.output_avg_vec, nb_examples, 1)
+		Y_raw = Y * np.tile(self.output_std_vec, (nb_examples, 1)) \
+			+ np.tile(self.output_avg_vec, (nb_examples, 1))
 		return Y_raw
 
 	# back propagation
 	def backprop(self, X, Y, step_size, iteration):
 		if_nn_nav = False
 		# if X.shape[1] >= 7 + 8 and (X.shape[1] - 7 ) % 8 == 0:
 		# 	if_nn_nav = True
@@ -492,15 +498,15 @@
 		for layer in range(nb_layers-1):
 			# RelU
 			# print 'layer', layer
 			# print 'self.W[layer].shape', self.W[layer].shape
 			# print 'out', out.shape
 			if self.multiagent_net_param.layers_type[layer] == 'conn':
 				tmp = np.dot(out, self.W[layer]) \
-					+ np.matlib.repmat(self.b[layer], batch_size, 1)
+					+ np.tile(self.b[layer], (batch_size, 1))
 				forward_prop_o[layer] = tmp * (tmp>0)
 			elif self.multiagent_net_param.layers_type[layer] == 'max':
 				num_pts = out.shape[0]
 				next_layer_size = np.sum(self.multiagent_net_param.layers_info[layer][:,1])
 				forward_prop_o[layer] = np.zeros((num_pts, next_layer_size))
 				cur_s_ind = 0
 				next_s_ind = 0
@@ -546,16 +552,16 @@
 			out = forward_prop_o[layer].copy()
 
 		# last layer, softmax
 		# print 'y_out.shape', y_out.shape
 		# print 'self.output_dim_weights', self.output_dim_weights
 		scores = y_out - \
 				 (np.dot(forward_prop_o[-2], self.W[nb_layers-1]) + \
-				 np.matlib.repmat(self.b[nb_layers-1], batch_size, 1))
-		scores = - np.matlib.repmat(self.output_dim_weights, batch_size, 1) * scores
+				 np.tile(self.b[nb_layers-1], (batch_size, 1)))
+		scores = - np.tile(self.output_dim_weights, (batch_size, 1)) * scores
 		# print scores.shape
 		# print expscores.shape
 		# print expscores.sum(axis=1).shape
 		# print np.matlib.repmat(expscores.sum(axis=1), k,1).transpose().shape
 
 			
 		#### backward pass starting from the output, i.e. the class probabilities
@@ -707,15 +713,15 @@
 	# evaluating network loss
 	def evaluate_network_loss(self, X, Y):
 		Y_hat = self.make_prediction(X)
 		sqloss = self.compute_sqloss(Y_hat, Y)
 
 		scores = Y - Y_hat
 		batch_size = Y.shape[0]
-		scores = np.matlib.repmat(self.output_dim_weights, batch_size, 1) * np.square(scores)
+		scores = np.tile(self.output_dim_weights, (batch_size, 1)) * np.square(scores)
 		Y_hat = np.sum(scores, axis = 1)
 		threshold = 0.25
 		discrete_loss = (Y.squeeze() > 0.25).sum() / float(Y.shape[0])
 		return discrete_loss, sqloss
 
 	def make_prediction(self, X):
 		if len(X.shape) > 1:
@@ -740,15 +746,15 @@
 		# 			assert(0)
 
 		nb_layers = self.num_hidden_layers + 1
 		out = X
 		for layer in range(nb_layers-1):
 			if self.multiagent_net_param.layers_type[layer] == 'conn':
 				tmp = np.dot(out, self.W[layer]) \
-					+ np.matlib.repmat(self.b[layer], nb_examples, 1)
+					+ np.tile(self.b[layer], (nb_examples, 1))
 				out = tmp * (tmp>0)
 			elif self.multiagent_net_param.layers_type[layer] == 'max':
 				num_pts = out.shape[0]
 				next_layer_size = np.sum(self.multiagent_net_param.layers_info[layer][:,1])
 				out_next = np.zeros((num_pts, np.sum(next_layer_size)))
 				if num_pts == 0:
 					out = out_next
@@ -788,24 +794,24 @@
 			# 	for tt in range(num_other_agents):
 			# 		out[agent_off_indices[tt],start_ind:start_ind+stride] = 0
 			# 		start_ind += stride
 
 
 
 		y_hat = np.dot(out, self.W[nb_layers-1]) + \
-					 np.matlib.repmat(self.b[nb_layers-1], nb_examples, 1)
+					 np.tile(self.b[nb_layers-1], (nb_examples, 1))
 		return y_hat
 
 	def compute_sqloss(self, Y_hat, Y):	
 		# print Y_hat
 		# print 'Y', Y	
 		# assert(0)
 		batch_size = Y.shape[0]
 		scores = Y - Y_hat
-		scores = np.matlib.repmat(self.output_dim_weights, batch_size, 1) * scores
+		scores = np.tile(self.output_dim_weights, (batch_size, 1)) * scores
 		sq_loss = 0.5 * np.sum(np.square(scores)) / batch_size
 		return sq_loss
 
 	# requires scaling the input dimension
 	def make_prediction_raw(self, X_raw):
 		X = self.xRaw_2_x(X_raw)
 		Y_scale = self.make_prediction(X)
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/nn_training_param.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/nn_training_param.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network_regr.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/CADRL/scripts/neural_networks/neural_network_regr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 
 import numpy as np
-import numpy.matlib
 import pickle
 import matplotlib.pyplot as plt
 from test_data import generate_sinusoids
 from nn_training_param import NN_training_param
 import os
 import time
 
@@ -175,36 +174,36 @@
 
 	# scale X (xRaw_2_x)
 	def xRaw_2_x(self, X_raw):
 		if len(X_raw.shape) > 1:
 			nb_examples = X_raw.shape[0]
 		else:
 			nb_examples = 1
-		X = (X_raw - np.matlib.repmat(self.avg_vec, nb_examples, 1)) \
-			/ np.matlib.repmat(self.std_vec, nb_examples, 1)
+		X = (X_raw - np.(self.avg_vec, (nb_examples, 1))) \
+			/ np.(self.std_vec, (nb_examples, 1))
 		return X
 
 	# scale Y (yRaw_2_y)
 	def yRaw_2_y(self, Y_raw):
 		if len(Y_raw.shape) > 1:
 			nb_examples = Y_raw.shape[0]
 		else:
 			nb_examples = 1
-		Y = (Y_raw - np.matlib.repmat(self.output_avg_vec, nb_examples, 1)) \
-			/ np.matlib.repmat(self.output_std_vec, nb_examples, 1)
+		Y = (Y_raw - np.tile(self.output_avg_vec, (nb_examples, 1))) \
+			/ np.tile(self.output_std_vec, (nb_examples, 1))
 		return Y
 
 	# scale Y (y_2_yraw)
 	def y_2_yRaw(self, Y):
 		if len(Y.shape) > 1:
 			nb_examples = Y.shape[0]
 		else:
 			nb_examples = 1
-		Y_raw = Y * np.matlib.repmat(self.output_std_vec, nb_examples, 1) \
-			+ np.matlib.repmat(self.output_avg_vec, nb_examples, 1)
+		Y_raw = Y * np.tile(self.output_std_vec, (nb_examples, 1)) \
+			+ np.tile(self.output_avg_vec, (nb_examples, 1))
 		return Y_raw
 
 	# back propagation
 	def backprop(self, X, Y, step_size, iter):
 		# training param
 		param = self.nn_training_param
 		# for forward/backward propogation
@@ -222,28 +221,28 @@
 		# one step back prop
 		for layer in xrange(nb_layers-1):
 			# RelU
 			# print 'layer', layer
 			# print 'self.W[layer].shape', self.W[layer].shape
 			# print 'out', out.shape
 			tmp = np.dot(out, self.W[layer]) \
-				+ np.matlib.repmat(self.b[layer], batch_size, 1)
+				+ np.tile(self.b[layer], (batch_size, 1))
 			forward_prop_o[layer] = tmp * (tmp>0)
 			# dropout
 			# p = 0.80
 			# dropout_mask = (np.random.rand(*tmp.shape) < p) / p
 			# forward_prop_o[layer] *= dropout_mask
 
 			out = forward_prop_o[layer].copy()
 
 		# last layer, derivative of quadratic cost
 		scores = y_out - \
 				 (np.dot(forward_prop_o[-2], self.W[nb_layers-1]) + \
-				 np.matlib.repmat(self.b[nb_layers-1], batch_size, 1))
-		scores = - np.matlib.repmat(self.output_dim_weights, batch_size, 1) * scores
+				 np.tile(self.b[nb_layers-1], (batch_size, 1)))
+		scores = - np.tile(self.output_dim_weights, (batch_size, 1)) * scores
 		# print scores.shape
 		# print expscores.shape
 		# print expscores.sum(axis=1).shape
 		# print np.matlib.repmat(expscores.sum(axis=1), k,1).transpose().shape
 
 			
 		#### backward pass starting from the output, i.e. the class probabilities
@@ -410,42 +409,42 @@
 	# evaluating network loss
 	def evaluate_network_loss(self, X, Y):
 		Y_hat = self.make_prediction(X)
 		sqloss = self.compute_sqloss(Y_hat, Y)
 
 		scores = Y - Y_hat
 		batch_size = Y.shape[0]
-		scores = np.matlib.repmat(self.output_dim_weights, batch_size, 1) * np.square(scores)
+		scores = np.tile(self.output_dim_weights, (batch_size, 1)) * np.square(scores)
 		Y_hat = np.sum(scores, axis = 1)
 		threshold = 0.25
 		discrete_loss = (Y.squeeze() > 0.25).sum() / float(Y.shape[0])
 		return discrete_loss, sqloss
 
 	def make_prediction(self, X):
 		if len(X.shape) > 1:
 			nb_examples = X.shape[0]
 		else:
 			nb_examples = 1
 		nb_layers = self.num_hidden_layers + 1
 		out = X
 		for layer in xrange(nb_layers-1):
 			tmp = np.dot(out, self.W[layer]) \
-					+ np.matlib.repmat(self.b[layer], nb_examples, 1)
+					+ np.tile(self.b[layer], (nb_examples, 1))
 			out = tmp * (tmp>0)
 		y_hat = np.dot(out, self.W[nb_layers-1]) + \
-					 np.matlib.repmat(self.b[nb_layers-1], nb_examples, 1)
+					 np.tile(self.b[nb_layers-1], (nb_examples, 1))
 		return y_hat
 
 	def compute_sqloss(self, Y_hat, Y):	
 		# print Y_hat
 		# print 'Y', Y	
 		# assert(0)
 		batch_size = Y.shape[0]
 		scores = Y - Y_hat
-		scores = np.matlib.repmat(self.output_dim_weights, batch_size, 1) * scores
+		scores = np.tile(self.output_dim_weights, (batch_size, 1)) * scores
 		sq_loss = 0.5 * np.sum(np.square(scores)) / batch_size
 		return sq_loss
 
 	# requires scaling the input dimension
 	def make_prediction_raw(self, X_raw):
 		X = self.xRaw_2_x(X_raw)
 		Y_scale = self.make_prediction(X)
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.index` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.index`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.meta` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.meta`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.data-00000-of-00001` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/policies/GA3C_CADRL/network.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/policies/GA3C_CADRL/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-import tensorflow as tf
+import tensorflow.compat.v1 as tf
 import time
 
 np.set_printoptions(precision=3, suppress=True)
 
 class Actions():
     # Define 11 choices of actions to be:
     # [v_pref,      [-pi/6, -pi/12, 0, pi/12, pi/6]]
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/collision_avoidance_env.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/collision_avoidance_env.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,59 @@
-'''
+"""
 Collision Avoidance Environment
 Author: Michael Everett
 MIT Aerospace Controls Lab
-'''
+"""
 
-import gym
-import gym.spaces
-import numpy as np
-import itertools
 import copy
-import os
 import inspect
+import itertools
+import os
 import sys
 
+import gym
+import gym.spaces
+import numpy as np
+
 from gym_collision_avoidance.envs import Config
-from gym_collision_avoidance.envs.util import find_nearest, rgba2rgb, l2norm, makedirs
-from gym_collision_avoidance.envs.visualize import plot_episode, animate_episode
+from gym_collision_avoidance.envs import test_cases as tc
 from gym_collision_avoidance.envs.agent import Agent
 from gym_collision_avoidance.envs.Map import Map
-from gym_collision_avoidance.envs import test_cases as tc
+from gym_collision_avoidance.envs.util import (
+    find_nearest,
+    l2norm,
+    makedirs,
+    rgba2rgb,
+)
+from gym_collision_avoidance.envs.visualize import (
+    animate_episode,
+    plot_episode,
+)
+
 
 class CollisionAvoidanceEnv(gym.Env):
-    """ Gym Environment for multiagent collision avoidance
+    """Gym Environment for multiagent collision avoidance
 
     The environment contains a list of agents.
 
     :param agents: (list) A list of :class:`~gym_collision_avoidance.envs.agent.Agent` objects that represent the dynamic objects in the scene.
     :param num_agents: (int) The maximum number of agents in the environment.
     """
 
     # Attributes:
     #     agents: A list of :class:`~gym_collision_avoidance.envs.agent.Agent` objects that represent the dynamic objects in the scene.
     #     num_agents: The maximum number of agents in the environment.
 
     metadata = {
         # UNUSED !!
-        'render.modes': ['human', 'rgb_array'],
-        'video.frames_per_second': 30
+        "render.modes": ["human", "rgb_array"],
+        "video.frames_per_second": 30,
     }
 
     def __init__(self):
-
         self.id = 0
 
         # Initialize Rewards
         self._initialize_rewards()
 
         # Simulation Parameters
         self.num_agents = Config.MAX_NUM_AGENTS_IN_ENVIRONMENT
@@ -53,15 +62,17 @@
         # Collision Parameters
         self.collision_dist = Config.COLLISION_DIST
         self.getting_close_range = Config.GETTING_CLOSE_RANGE
 
         # Plotting Parameters
         self.evaluate = Config.EVALUATE_MODE
 
-        self.plot_episodes = Config.SHOW_EPISODE_PLOTS or Config.SAVE_EPISODE_PLOTS
+        self.plot_episodes = (
+            Config.SHOW_EPISODE_PLOTS or Config.SAVE_EPISODE_PLOTS
+        )
         self.plt_limits = Config.PLT_LIMITS
         self.plt_fig_size = Config.PLT_FIG_SIZE
         self.test_case_index = 0
 
         self.set_testcase(Config.TEST_CASE_FN, Config.TEST_CASE_ARGS)
 
         self.animation_period_steps = Config.ANIMATION_PERIOD_STEPS
@@ -70,53 +81,66 @@
         #     self.low_state = np.zeros((Config.FULL_LABELED_STATE_LENGTH))
         #     self.high_state = np.zeros((Config.FULL_LABELED_STATE_LENGTH))
         # else:
         #     self.low_state = np.zeros((Config.FULL_STATE_LENGTH))
         #     self.high_state = np.zeros((Config.FULL_STATE_LENGTH))
 
         # Upper/Lower bounds on Actions
-        self.max_heading_change = np.pi/3
+        self.max_heading_change = np.pi / 3
         self.min_heading_change = -self.max_heading_change
         self.min_speed = 0.0
         self.max_speed = 1.0
 
         ### The gym.spaces library doesn't support Python2.7 (syntax of Super().__init__())
         self.action_space_type = Config.ACTION_SPACE_TYPE
-        
+
         if self.action_space_type == Config.discrete:
-            self.action_space = gym.spaces.Discrete(self.actions.num_actions, dtype=np.float32)
+            self.action_space = gym.spaces.Discrete(
+                self.actions.num_actions, dtype=np.float32
+            )
         elif self.action_space_type == Config.continuous:
-            self.low_action = np.array([self.min_speed,
-                                        self.min_heading_change])
-            self.high_action = np.array([self.max_speed,
-                                         self.max_heading_change])
-            self.action_space = gym.spaces.Box(self.low_action, self.high_action, dtype=np.float32)
-        
+            self.low_action = np.array(
+                [self.min_speed, self.min_heading_change]
+            )
+            self.high_action = np.array(
+                [self.max_speed, self.max_heading_change]
+            )
+            self.action_space = gym.spaces.Box(
+                self.low_action, self.high_action, dtype=np.float32
+            )
 
         # original observation space
         # self.observation_space = gym.spaces.Box(self.low_state, self.high_state, dtype=np.float32)
-        
+
         # not used...
         # self.observation_space = np.array([gym.spaces.Box(self.low_state, self.high_state, dtype=np.float32)
-                                           # for _ in range(self.num_agents)])
+        # for _ in range(self.num_agents)])
         # observation_space = gym.spaces.Box(self.low_state, self.high_state, dtype=np.float32)
-        
+
         # single agent dict obs
         self.observation = {}
+        self.observation_space = gym.spaces.Dict({})
         for agent in range(Config.MAX_NUM_AGENTS_IN_ENVIRONMENT):
             self.observation[agent] = {}
+            self.observation_space.spaces[agent] = gym.spaces.Dict({})
 
         # The observation returned by the environment is a Dict of Boxes, keyed by agent index.
-        self.observation_space = gym.spaces.Dict({})
         for state in Config.STATES_IN_OBS:
-            self.observation_space.spaces[state] = gym.spaces.Box(Config.STATE_INFO_DICT[state]['bounds'][0]*np.ones((Config.STATE_INFO_DICT[state]['size'])),
-                Config.STATE_INFO_DICT[state]['bounds'][1]*np.ones((Config.STATE_INFO_DICT[state]['size'])),
-                dtype=Config.STATE_INFO_DICT[state]['dtype'])
             for agent in range(Config.MAX_NUM_AGENTS_IN_ENVIRONMENT):
-                self.observation[agent][state] = np.zeros((Config.STATE_INFO_DICT[state]['size']), dtype=Config.STATE_INFO_DICT[state]['dtype'])
+                self.observation[agent][state] = np.zeros(
+                    (Config.STATE_INFO_DICT[state]["size"]),
+                    dtype=Config.STATE_INFO_DICT[state]["dtype"],
+                )
+                self.observation_space.spaces[agent][state] = gym.spaces.Box(
+                    Config.STATE_INFO_DICT[state]["bounds"][0]
+                    * np.ones((Config.STATE_INFO_DICT[state]["size"])),
+                    Config.STATE_INFO_DICT[state]["bounds"][1]
+                    * np.ones((Config.STATE_INFO_DICT[state]["size"])),
+                    dtype=Config.STATE_INFO_DICT[state]["dtype"],
+                )
 
         self.agents = None
         self.default_agents = None
         self.prev_episode_agents = None
 
         self.static_map_filename = None
         self.map = None
@@ -126,15 +150,15 @@
 
         self.plot_save_dir = None
         self.plot_policy_name = None
 
         self.perturbed_obs = None
 
     def step(self, actions, dt=None):
-        """ Run one timestep of environment dynamics.
+        """Run one timestep of environment dynamics.
 
         This is the main function. An external process will compute an action for every agent
         then call env.step(actions). The agents take those actions,
         then we check if any agents have earned a reward (collision/goal/...).
         Then agents take an observation of the new world state. We compute whether each agent is done
         (collided/reached goal/ran out of time) and if everyone's done, the episode ends.
         We return the relevant info back to the process that called env.step(actions).
@@ -163,120 +187,170 @@
 
         # Collect rewards
         rewards = self._compute_rewards()
 
         # Take observation
         next_observations = self._get_obs()
 
-        if Config.ANIMATE_EPISODES and self.episode_step_number % self.animation_period_steps == 0:
-            plot_episode(self.agents, False, self.map, self.test_case_index,
+        if (
+            Config.ANIMATE_EPISODES
+            and self.episode_step_number % self.animation_period_steps == 0
+        ):
+            plot_episode(
+                self.agents,
+                False,
+                self.map,
+                self.test_case_index,
                 circles_along_traj=Config.PLOT_CIRCLES_ALONG_TRAJ,
                 plot_save_dir=self.plot_save_dir,
                 plot_policy_name=self.plot_policy_name,
                 save_for_animation=True,
                 limits=self.plt_limits,
                 fig_size=self.plt_fig_size,
                 perturbed_obs=self.perturbed_obs,
                 show=False,
-                save=True)
+                save=True,
+            )
 
         # Check which agents' games are finished (at goal/collided/out of time)
         which_agents_done, game_over = self._check_which_agents_done()
 
         which_agents_done_dict = {}
         which_agents_learning_dict = {}
         for i, agent in enumerate(self.agents):
             which_agents_done_dict[agent.id] = which_agents_done[i]
-            which_agents_learning_dict[agent.id] = agent.policy.is_still_learning
-
-        return next_observations, rewards, game_over, \
+            which_agents_learning_dict[agent.id] = (
+                agent.policy.is_still_learning
+            )
+
+        return (
+            next_observations,
+            rewards,
+            game_over,
+            False,
             {
-                'which_agents_done': which_agents_done_dict,
-                'which_agents_learning': which_agents_learning_dict,
-            }
+                "which_agents_done": which_agents_done_dict,
+                "which_agents_learning": which_agents_learning_dict,
+            },
+        )
 
     def reset(self):
-        """ Resets the environment, re-initializes agents, plots episode (if applicable) and returns an initial observation.
+        """Resets the environment, re-initializes agents, plots episode (if applicable) and returns an initial observation.
 
         Returns:
             initial observation (np array): each agent's observation given the initial configuration
         """
-        if self.episode_step_number is not None and self.episode_step_number > 0 and self.plot_episodes and self.test_case_index >= 0:
-            plot_episode(self.agents, self.evaluate, self.map, self.test_case_index, self.id, circles_along_traj=Config.PLOT_CIRCLES_ALONG_TRAJ, plot_save_dir=self.plot_save_dir, plot_policy_name=self.plot_policy_name, limits=self.plt_limits, fig_size=self.plt_fig_size, show=Config.SHOW_EPISODE_PLOTS, save=Config.SAVE_EPISODE_PLOTS)
+        if (
+            self.episode_step_number is not None
+            and self.episode_step_number > 0
+            and self.plot_episodes
+            and self.test_case_index >= 0
+        ):
+            plot_episode(
+                self.agents,
+                self.evaluate,
+                self.map,
+                self.test_case_index,
+                self.id,
+                circles_along_traj=Config.PLOT_CIRCLES_ALONG_TRAJ,
+                plot_save_dir=self.plot_save_dir,
+                plot_policy_name=self.plot_policy_name,
+                limits=self.plt_limits,
+                fig_size=self.plt_fig_size,
+                show=Config.SHOW_EPISODE_PLOTS,
+                save=Config.SAVE_EPISODE_PLOTS,
+            )
             if Config.ANIMATE_EPISODES:
-                animate_episode(num_agents=len(self.agents), plot_save_dir=self.plot_save_dir, plot_policy_name=self.plot_policy_name, test_case_index=self.test_case_index, agents=self.agents)
+                animate_episode(
+                    num_agents=len(self.agents),
+                    plot_save_dir=self.plot_save_dir,
+                    plot_policy_name=self.plot_policy_name,
+                    test_case_index=self.test_case_index,
+                    agents=self.agents,
+                )
             self.episode_number += 1
         self.begin_episode = True
         self.episode_step_number = 0
         self._init_agents()
         if Config.USE_STATIC_MAP:
             self._init_static_map()
         for state in Config.STATES_IN_OBS:
             for agent in range(Config.MAX_NUM_AGENTS_IN_ENVIRONMENT):
-                self.observation[agent][state] = np.zeros((Config.STATE_INFO_DICT[state]['size']), dtype=Config.STATE_INFO_DICT[state]['dtype'])
-        return self._get_obs()
+                self.observation[agent][state] = np.zeros(
+                    (Config.STATE_INFO_DICT[state]["size"]),
+                    dtype=Config.STATE_INFO_DICT[state]["dtype"],
+                )
+        return self._get_obs(), {}
 
     def _take_action(self, actions, dt):
-        """ Some agents' actions come externally through the actions arg, agents with internal policies query their policy here, 
+        """Some agents' actions come externally through the actions arg, agents with internal policies query their policy here,
         then each agent takes a step simultaneously.
 
         This makes it so an external script that steps through the environment doesn't need to
         be aware of internals of the environment, like ensuring RVO agents compute their RVO actions.
         Instead, all policies that are already trained/frozen are computed internally, and if an
         agent's policy is still being trained, it's convenient to isolate the training code from the environment this way.
-        Or, if there's a real robot with its own planner on-board (thus, the agent should have an ExternalPolicy), 
+        Or, if there's a real robot with its own planner on-board (thus, the agent should have an ExternalPolicy),
         we don't bother computing its next action here and just take what the actions dict said.
 
         Args:
             actions (dict): keyed by agent indices, each value has a [delta heading angle, speed] command.
                 Agents with an ExternalPolicy sub-class receive their actions through this dict.
-                Other agents' indices shouldn't appear in this dict, but will be ignored if so, because they have 
+                Other agents' indices shouldn't appear in this dict, but will be ignored if so, because they have
                 an InternalPolicy sub-class, meaning they can
                 compute their actions internally given their observation (e.g., already trained CADRL, RVO, Non-Cooperative, etc.)
             dt (float): time in seconds to run the simulation (defaults to :code:`self.dt_nominal`)
 
         """
         num_actions_per_agent = 2  # speed, delta heading angle
-        all_actions = np.zeros((len(self.agents), num_actions_per_agent), dtype=np.float32)
+        all_actions = np.zeros(
+            (len(self.agents), num_actions_per_agent), dtype=np.float32
+        )
 
         # Agents set their action (either from external or w/ find_next_action)
         for agent_index, agent in enumerate(self.agents):
             if agent.is_done:
                 continue
             elif agent.policy.is_external:
-                all_actions[agent_index, :] = agent.policy.external_action_to_action(agent, actions[agent_index])
+                all_actions[agent_index, :] = (
+                    agent.policy.external_action_to_action(
+                        agent, actions[agent_index]
+                    )
+                )
             else:
                 dict_obs = self.observation[agent_index]
-                all_actions[agent_index, :] = agent.policy.find_next_action(dict_obs, self.agents, agent_index)
+                all_actions[agent_index, :] = agent.policy.find_next_action(
+                    dict_obs, self.agents, agent_index
+                )
 
         # After all agents have selected actions, run one dynamics update
         for i, agent in enumerate(self.agents):
-            agent.take_action(all_actions[i,:], dt)
+            agent.take_action(all_actions[i, :], dt)
 
     def _update_top_down_map(self):
-        """ After agents have moved, call this to update the map with their new occupancies. """
+        """After agents have moved, call this to update the map with their new occupancies."""
         self.map.add_agents_to_map(self.agents)
         # plt.imshow(self.map.map)
         # plt.pause(0.1)
 
     def set_agents(self, agents):
-        """ Set the default agent configuration, which will get used at the start of each episode (and bypass calling self.test_case_fn)
+        """Set the default agent configuration, which will get used at the start of each episode (and bypass calling self.test_case_fn)
 
         Args:
             agents (list): of :class:`~gym_collision_avoidance.envs.agent.Agent` objects that should become the self.default_agents
                 and thus be loaded in that configuration every time the env resets.
 
         """
         self.default_agents = agents
 
     def _init_agents(self):
-        """ Set self.agents (presumably at the start of a new episode) and set each agent's max heading change and speed based on env limits.
+        """Set self.agents (presumably at the start of a new episode) and set each agent's max heading change and speed based on env limits.
 
         self.agents gets set to self.default_agents if it exists.
-        Otherwise, self.agents gets set to the result of self.test_case_fn(self.test_case_args).        
+        Otherwise, self.agents gets set to the result of self.test_case_fn(self.test_case_args).
         """
 
         # The evaluation scripts need info about the previous episode's agents
         # (in case env.reset was called and thus self.agents was wiped)
         if self.evaluate and self.agents is not None:
             self.prev_episode_agents = copy.deepcopy(self.agents)
 
@@ -289,92 +363,105 @@
 
         # Make every agent respect the same env-wide limits on actions (this probably should live elsewhere...)
         for agent in self.agents:
             agent.max_heading_change = self.max_heading_change
             agent.max_speed = self.max_speed
 
     def set_static_map(self, map_filename):
-        """ If you want to have static obstacles, provide the path to the map image file that should be loaded.
-        
+        """If you want to have static obstacles, provide the path to the map image file that should be loaded.
+
         Args:
-            map_filename (str or list): full path of a binary png file corresponding to the environment prior map 
+            map_filename (str or list): full path of a binary png file corresponding to the environment prior map
                 (or list of candidate map paths to randomly choose btwn each episode)
         """
         self.static_map_filename = map_filename
 
     def _init_static_map(self):
-        """ Load the map based on its pre-provided filename, and initialize a :class:`~gym_collision_avoidance.envs.Map.Map` object
+        """Load the map based on its pre-provided filename, and initialize a :class:`~gym_collision_avoidance.envs.Map.Map` object
 
         Currently the dimensions of the world map are hard-coded.
 
         """
         if isinstance(self.static_map_filename, list):
             static_map_filename = np.random.choice(self.static_map_filename)
         else:
             static_map_filename = self.static_map_filename
 
-        x_width = 16 # meters
-        y_width = 16 # meters
-        grid_cell_size = 0.1 # meters/grid cell
+        x_width = 16  # meters
+        y_width = 16  # meters
+        grid_cell_size = 0.1  # meters/grid cell
         self.map = Map(x_width, y_width, grid_cell_size, static_map_filename)
 
     def _compute_rewards(self):
-        """ Check for collisions and reaching of the goal here, and also assign the corresponding rewards based on those calculations.
-        
+        """Check for collisions and reaching of the goal here, and also assign the corresponding rewards based on those calculations.
+
         Returns:
             rewards (scalar or list): is a scalar if we are only training on a single agent, or
                       is a list of scalars if we are training on mult agents
         """
 
         # if nothing noteworthy happened in that timestep, reward = -0.01
-        rewards = self.reward_time_step*np.ones(len(self.agents))
-        collision_with_agent, collision_with_wall, entered_norm_zone, dist_btwn_nearest_agent = \
-            self._check_for_collisions()
+        rewards = self.reward_time_step * np.ones(len(self.agents))
+        (
+            collision_with_agent,
+            collision_with_wall,
+            entered_norm_zone,
+            dist_btwn_nearest_agent,
+        ) = self._check_for_collisions()
 
         for i, agent in enumerate(self.agents):
             if agent.is_at_goal:
                 if agent.was_at_goal_already is False:
                     # agents should only receive the goal reward once
                     rewards[i] = self.reward_at_goal
                     # print("Agent %i: Arrived at goal!"
-                          # % agent.id)
+                    # % agent.id)
             else:
                 # agents at their goal shouldn't be penalized if someone else
                 # bumps into them
                 if agent.was_in_collision_already is False:
                     if collision_with_agent[i]:
                         rewards[i] = self.reward_collision_with_agent
                         agent.in_collision = True
                         # print("Agent %i: Collision with another agent!"
                         #       % agent.id)
                     elif collision_with_wall[i]:
                         rewards[i] = self.reward_collision_with_wall
                         agent.in_collision = True
                         # print("Agent %i: Collision with wall!"
-                              # % agent.id)
+                        # % agent.id)
                     else:
                         # There was no collision
-                        if dist_btwn_nearest_agent[i] <= Config.GETTING_CLOSE_RANGE:
-                            rewards[i] = -0.1 - dist_btwn_nearest_agent[i]/2.
+                        if (
+                            dist_btwn_nearest_agent[i]
+                            <= Config.GETTING_CLOSE_RANGE
+                        ):
+                            rewards[i] = (
+                                -0.1 - dist_btwn_nearest_agent[i] / 2.0
+                            )
                             # print("Agent %i: Got close to another agent!"
                             #       % agent.id)
-                        if abs(agent.past_actions[0, 1]) > self.wiggly_behavior_threshold:
+                        if (
+                            abs(agent.past_actions[0, 1])
+                            > self.wiggly_behavior_threshold
+                        ):
                             # Slightly penalize wiggly behavior
                             rewards[i] += self.reward_wiggly_behavior
                         # elif entered_norm_zone[i]:
                         #     rewards[i] = self.reward_entered_norm_zone
-        rewards = np.clip(rewards, self.min_possible_reward,
-                          self.max_possible_reward)
+        rewards = np.clip(
+            rewards, self.min_possible_reward, self.max_possible_reward
+        )
         if Config.TRAIN_SINGLE_AGENT:
             rewards = rewards[0]
         return rewards
 
     def _check_for_collisions(self):
-        """ Check whether each agent has collided with another agent or a static obstacle in the map 
-        
+        """Check whether each agent has collided with another agent or a static obstacle in the map
+
         This method doesn't compute social zones currently!!!!!
 
         Returns:
             - collision_with_agent (list): for each agent, bool True if that agent is in collision with another agent
             - collision_with_wall (list): for each agent, bool True if that agent is in collision with object in map
             - entered_norm_zone (list): for each agent, bool True if that agent entered another agent's social zone
             - dist_btwn_nearest_agent (list): for each agent, float closest distance to another agent
@@ -385,66 +472,92 @@
         entered_norm_zone = [False for _ in self.agents]
         dist_btwn_nearest_agent = [np.inf for _ in self.agents]
         agent_shapes = []
         agent_front_zones = []
         agent_inds = list(range(len(self.agents)))
         agent_pairs = list(itertools.combinations(agent_inds, 2))
         for i, j in agent_pairs:
-            dist_btwn = l2norm(self.agents[i].pos_global_frame, self.agents[j].pos_global_frame)
+            dist_btwn = l2norm(
+                self.agents[i].pos_global_frame,
+                self.agents[j].pos_global_frame,
+            )
             combined_radius = self.agents[i].radius + self.agents[j].radius
-            dist_btwn_nearest_agent[i] = min(dist_btwn_nearest_agent[i], dist_btwn - combined_radius)
+            dist_btwn_nearest_agent[i] = min(
+                dist_btwn_nearest_agent[i], dist_btwn - combined_radius
+            )
+            dist_btwn_nearest_agent[j] = min(
+                dist_btwn_nearest_agent[j], dist_btwn - combined_radius
+            )
             if dist_btwn <= combined_radius:
                 # Collision with another agent!
                 collision_with_agent[i] = True
                 collision_with_agent[j] = True
         if Config.USE_STATIC_MAP:
             for i in agent_inds:
                 agent = self.agents[i]
-                [pi, pj], in_map = self.map.world_coordinates_to_map_indices(agent.pos_global_frame)
+                [pi, pj], in_map = self.map.world_coordinates_to_map_indices(
+                    agent.pos_global_frame
+                )
                 mask = self.map.get_agent_map_indices([pi, pj], agent.radius)
                 # plt.figure('static map')
                 # plt.imshow(self.map.static_map + mask)
                 # plt.pause(0.1)
                 if in_map and np.any(self.map.static_map[mask]):
                     # Collision with wall!
                     collision_with_wall[i] = True
-        return collision_with_agent, collision_with_wall, entered_norm_zone, dist_btwn_nearest_agent
+        return (
+            collision_with_agent,
+            collision_with_wall,
+            entered_norm_zone,
+            dist_btwn_nearest_agent,
+        )
 
     def _check_which_agents_done(self):
-        """ Check if any agents have reached goal, run out of time, or collided.
+        """Check if any agents have reached goal, run out of time, or collided.
 
         Returns:
             - which_agents_done (list): for each agent, True if agent is done, o.w. False
             - game_over (bool): depending on mode, True if all agents done, True if 1st agent done, True if all learning agents done
         """
-        at_goal_condition = np.array(
-                [a.is_at_goal for a in self.agents])
+        at_goal_condition = np.array([a.is_at_goal for a in self.agents])
         ran_out_of_time_condition = np.array(
-                [a.ran_out_of_time for a in self.agents])
+            [a.ran_out_of_time for a in self.agents]
+        )
         in_collision_condition = np.array(
-                [a.in_collision for a in self.agents])
-        which_agents_done = np.logical_or.reduce((at_goal_condition, ran_out_of_time_condition, in_collision_condition))
+            [a.in_collision for a in self.agents]
+        )
+        which_agents_done = np.logical_or.reduce(
+            (
+                at_goal_condition,
+                ran_out_of_time_condition,
+                in_collision_condition,
+            )
+        )
         for agent_index, agent in enumerate(self.agents):
             agent.is_done = which_agents_done[agent_index]
-        
+
         if Config.EVALUATE_MODE:
             # Episode ends when every agent is done
             game_over = np.all(which_agents_done)
         elif Config.TRAIN_SINGLE_AGENT:
             # Episode ends when ego agent is done
             game_over = which_agents_done[0]
         else:
             # Episode is done when all *learning* agents are done
-            learning_agent_inds = [i for i in range(len(self.agents)) if self.agents[i].policy.is_still_learning]
+            learning_agent_inds = [
+                i
+                for i in range(len(self.agents))
+                if self.agents[i].policy.is_still_learning
+            ]
             game_over = np.all(which_agents_done[learning_agent_inds])
-        
+
         return which_agents_done, game_over
 
     def _get_obs(self):
-        """ Update the map now that agents have moved, have each agent sense the world, and fill in their observations 
+        """Update the map now that agents have moved, have each agent sense the world, and fill in their observations
 
         Returns:
             observation (list): for each agent, a dictionary observation.
 
         """
 
         if Config.USE_STATIC_MAP:
@@ -458,73 +571,76 @@
         # Agents fill in their element of the multiagent observation vector
         for i, agent in enumerate(self.agents):
             self.observation[i] = agent.get_observation_dict(self.agents)
 
         return self.observation
 
     def _initialize_rewards(self):
-        """ Set some class attributes regarding reward values based on Config """
+        """Set some class attributes regarding reward values based on Config"""
         self.reward_at_goal = Config.REWARD_AT_GOAL
         self.reward_collision_with_agent = Config.REWARD_COLLISION_WITH_AGENT
         self.reward_collision_with_wall = Config.REWARD_COLLISION_WITH_WALL
         self.reward_getting_close = Config.REWARD_GETTING_CLOSE
         self.reward_entered_norm_zone = Config.REWARD_ENTERED_NORM_ZONE
         self.reward_time_step = Config.REWARD_TIME_STEP
 
         self.reward_wiggly_behavior = Config.REWARD_WIGGLY_BEHAVIOR
         self.wiggly_behavior_threshold = Config.WIGGLY_BEHAVIOR_THRESHOLD
 
-        self.possible_reward_values = \
-            np.array([self.reward_at_goal,
-                      self.reward_collision_with_agent,
-                      self.reward_time_step,
-                      self.reward_collision_with_wall,
-                      self.reward_wiggly_behavior
-                      ])
+        self.possible_reward_values = np.array(
+            [
+                self.reward_at_goal,
+                self.reward_collision_with_agent,
+                self.reward_time_step,
+                self.reward_collision_with_wall,
+                self.reward_wiggly_behavior,
+            ]
+        )
         self.min_possible_reward = np.min(self.possible_reward_values)
         self.max_possible_reward = np.max(self.possible_reward_values)
 
     def set_plot_save_dir(self, plot_save_dir):
-        """ Set where to save plots of trajectories (will get created if non-existent)
-        
+        """Set where to save plots of trajectories (will get created if non-existent)
+
         Args:
             plot_save_dir (str): path to directory you'd like to save plots in
 
         """
         makedirs(plot_save_dir, exist_ok=True)
         self.plot_save_dir = plot_save_dir
 
     def set_perturbed_info(self, perturbed_obs):
-        """ Used for robustness paper to pass info that could be visualized. Too hacky.
-        """
+        """Used for robustness paper to pass info that could be visualized. Too hacky."""
         self.perturbed_obs = perturbed_obs
 
     def set_testcase(self, test_case_fn_str, test_case_args):
-        """ 
+        """
 
         Args:
             test_case_fn_str (str): name of function in test_cases.py
         """
 
         # Provide a fn (which returns list of agents) and the fn's args,
         # to be called on each env.reset()
         test_case_fn = getattr(tc, test_case_fn_str, None)
-        assert(callable(test_case_fn))
+        assert callable(test_case_fn)
 
         # Before running test_case_fn, make sure we didn't provide any args it doesn't accept
-        if sys.version[0] == '3':
+        if sys.version[0] == "3":
             signature = inspect.signature(test_case_fn)
-        elif sys.version[0] == '2':
+        elif sys.version[0] == "2":
             import funcsigs
+
             signature = funcsigs.signature(test_case_fn)
         test_case_fn_args = signature.parameters
         test_case_args_keys = list(test_case_args.keys())
         for key in test_case_args_keys:
             # print("checking if {} accepts {}".format(test_case_fn, key))
             if key not in test_case_fn_args:
                 # print("{} doesn't accept {} -- removing".format(test_case_fn, key))
                 del test_case_args[key]
         self.test_case_fn = test_case_fn
         self.test_case_args = test_case_args
 
-if __name__ == '__main__':
-    print("See example.py for a minimum working example.")
+
+if __name__ == "__main__":
+    print("See example.py for a minimum working example.")
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/Map.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/Map.py`

 * *Files identical despite different names*

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/wrappers.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import gym
 import numpy as np
-from gym_collision_avoidance.envs.vec_env import DummyVecEnv
 
-__all__ = ['FlattenDictWrapper', 'MultiagentFlattenDictWrapper', 'MultiagentDummyVecEnv', 'MultiagentDictToMultiagentArrayWrapper']
+__all__ = [
+    "FlattenDictWrapper",
+    "MultiagentFlattenDictWrapper",
+    "MultiagentDictToMultiagentArrayWrapper",
+]
+
 
 class MultiagentFlattenDictWrapper(gym.ObservationWrapper):
     """Flattens selected keys of a Dict observation space into
     an array.
     """
+
     def __init__(self, env, dict_keys, max_num_agents):
         super(MultiagentFlattenDictWrapper, self).__init__(env)
         self.dict_keys = dict_keys
         self.max_num_agents = max_num_agents
 
         self.setup_obs(max_num_agents, dict_keys)
-        self.observation_space = gym.spaces.Box(-np.inf, np.inf, shape=self.obs_shape, dtype='float32')
-
-        single_agent_size = self.observation_indices[0]['BOUNDS'][1] - self.observation_indices[0]['BOUNDS'][0]
-        self.single_agent_observation_space = gym.spaces.Box(-np.inf, np.inf, shape=(single_agent_size,), dtype='float32')
+        self.observation_space = gym.spaces.Box(
+            -np.inf, np.inf, shape=self.obs_shape, dtype="float32"
+        )
+
+        single_agent_size = (
+            self.observation_indices[0]["BOUNDS"][1]
+            - self.observation_indices[0]["BOUNDS"][0]
+        )
+        self.single_agent_observation_space = gym.spaces.Box(
+            -np.inf, np.inf, shape=(single_agent_size,), dtype="float32"
+        )
 
         self.dict_observation_space = self.env.observation_space
 
     def setup_obs(self, max_num_agents, dict_keys):
         self.observation_indices = {}
         size = 0
         for agent in range(max_num_agents):
@@ -29,15 +41,18 @@
             agent_lower_ind = size
             for key in dict_keys:
                 shape = self.env.observation_space.spaces[key].shape
                 prev_size = size
                 size += np.prod(shape)
                 self.observation_indices[agent][key] = [prev_size, size]
             agent_upper_ind = size
-            self.observation_indices[agent]['BOUNDS'] = [agent_lower_ind, agent_upper_ind]
+            self.observation_indices[agent]["BOUNDS"] = [
+                agent_lower_ind,
+                agent_upper_ind,
+            ]
 
         self.obs_shape = (size,)
 
     def observation(self, observation):
         # Turn multiagent dict obs into a really long 1d array
         # with all agents & states concatenated
         assert isinstance(observation, dict)
@@ -50,89 +65,109 @@
     def observationArrayToDict(self, observation_array):
         assert isinstance(observation_array, np.ndarray)
         assert observation_array.shape == self.observation_space.shape
         obs = {}
         for agent in range(self.max_num_agents):
             obs[agent] = {}
             for key in self.dict_keys:
-                obs[agent][key] = observation_array[self.observation_indices[agent][key][0]: self.observation_indices[agent][key][1]]
+                obs[agent][key] = observation_array[
+                    self.observation_indices[agent][key][
+                        0
+                    ] : self.observation_indices[agent][key][1]
+                ]
         return obs
 
     def multiEnvObservationArrayToDict(self, observation_array):
         assert isinstance(observation_array, np.ndarray)
         # assert observation_array.shape == self.observation_space.shape
         num_envs = observation_array.shape[0]
         dict_obs = np.empty((num_envs, self.max_num_agents), dtype=dict)
         for env in range(num_envs):
             for agent in range(self.max_num_agents):
-                key = 'use_ppo'
-                ppo = observation_array[env][self.observation_indices[agent][key][0]: self.observation_indices[agent][key][1]]
+                key = "use_ppo"
+                ppo = observation_array[env][
+                    self.observation_indices[agent][key][
+                        0
+                    ] : self.observation_indices[agent][key][1]
+                ]
                 if ppo == False:
                     continue
                 dict_obs[env][agent] = {}
                 for key in self.dict_keys:
-                    dict_obs[env][agent][key] = observation_array[env][self.observation_indices[agent][key][0]: self.observation_indices[agent][key][1]].reshape(self.env.observation_space.spaces[key].shape)
+                    dict_obs[env][agent][key] = observation_array[env][
+                        self.observation_indices[agent][key][
+                            0
+                        ] : self.observation_indices[agent][key][1]
+                    ].reshape(self.env.observation_space.spaces[key].shape)
         return dict_obs
 
     def singleAgentObservationArrayToDict(self, observation_array, agent):
         assert isinstance(observation_array, np.ndarray)
         # assert observation_array.shape == self.single_agent_observation_space.shape
 
         obs = []
         for env in range(observation_array.shape[0]):
             obs.append({})
             for key in self.dict_keys:
-                obs[env][key] = observation_array[env, self.observation_indices[agent][key][0]: self.observation_indices[agent][key][1]].reshape(self.env.observation_space.spaces[key].shape)
+                obs[env][key] = observation_array[
+                    env,
+                    self.observation_indices[agent][key][
+                        0
+                    ] : self.observation_indices[agent][key][1],
+                ].reshape(self.env.observation_space.spaces[key].shape)
         return obs
 
     def keyToArrayInds(self, key):
         inds = []
         for agent in range(self.max_num_agents):
             inds.append(self.observation_indices[agent][key])
         return inds
 
     def singleAgentObservationArray(self, observation_array, agent):
-        return observation_array[self.observation_indices[agent]['BOUNDS'][0]:self.observation_indices[agent]['BOUNDS'][1]]
+        return observation_array[
+            self.observation_indices[agent]["BOUNDS"][
+                0
+            ] : self.observation_indices[agent]["BOUNDS"][1]
+        ]
 
     def singleAgentObservationInds(self, agent):
-        return self.observation_indices[agent]['BOUNDS']
+        return self.observation_indices[agent]["BOUNDS"]
+
 
 class FlattenDictWrapper(MultiagentFlattenDictWrapper):
     def __init__(self, env, dict_keys):
-        super(FlattenDictWrapper, self).__init__(env, dict_keys, max_num_agents=1)
+        super(FlattenDictWrapper, self).__init__(
+            env, dict_keys, max_num_agents=1
+        )
 
-class MultiagentDummyVecEnv(DummyVecEnv):
-    def __init__(self, env_fns):
-        DummyVecEnv.__init__(self, env_fns)
-
-        self.buf_dones = np.zeros((self.num_envs,), dtype=np.ndarray)
-        self.buf_rews  = np.zeros((self.num_envs,), dtype=np.ndarray)
 
 class MultiagentDictToMultiagentArrayWrapper(MultiagentFlattenDictWrapper):
     def __init__(self, env, dict_keys, max_num_agents):
-        super(MultiagentDictToMultiagentArrayWrapper, self).__init__(env, dict_keys, max_num_agents=max_num_agents)
+        super(MultiagentDictToMultiagentArrayWrapper, self).__init__(
+            env, dict_keys, max_num_agents=max_num_agents
+        )
 
     def setup_obs(self, max_num_agents, dict_keys):
         self.observation_indices = {}
         for agent in range(max_num_agents):
             self.observation_indices[agent] = {}
             size = 0
             for key in dict_keys:
-                shape = self.env.observation_space.spaces[key].shape
+                shape = self.env.observation_space.spaces[agent][key].shape
                 prev_size = size
                 size += np.prod(shape)
                 self.observation_indices[agent][key] = [prev_size, size]
             agent_upper_ind = size
-            self.observation_indices[agent]['BOUNDS'] = [0, agent_upper_ind]
+            self.observation_indices[agent]["BOUNDS"] = [0, agent_upper_ind]
 
         self.obs_shape = (max_num_agents, size)
 
     def observation(self, observation):
         # Turn multiagent dict obs into a 2d array
         # with shape (max_num_agents, num_states_per_agent)
         assert isinstance(observation, dict)
         obs = np.zeros(shape=self.obs_shape)
         for agent in range(self.max_num_agents):
             for key in self.dict_keys:
                 low, high = self.observation_indices[agent][key]
                 obs[agent][low:high] = observation[agent][key].ravel()
-        return obs
+        return obs
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance/envs/agent.py` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance/envs/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         self.action_dim = 2
         
         self.id = id
         self.dist_to_goal = 0.0
         self.near_goal_threshold = Config.NEAR_GOAL_THRESHOLD
         self.dt_nominal = Config.DT
 
+        self.num_other_agents_observed = 0
+
         self.min_x = -20.0
         self.max_x = 20.0
         self.min_y = -20.0
         self.max_y = 20.0
 
         self.t_offset = None
         self.global_state_dim = 11
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance.egg-info/PKG-INFO` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 Metadata-Version: 2.1
 Name: gym-collision-avoidance
-Version: 0.0.2.post2
+Version: 0.0.3
 Summary: Simulation environment for collision avoidance
 Home-page: https://github.com/mit-acl/gym-collision-avoidance
 Author: Michael Everett, Yu Fan Chen, Jonathan P. How, MIT
-License: UNKNOWN
-Description: # gym-collision-avoidance
-        
-        <img src="docs/_static/combo.gif" alt="Agents spelling ``CADRL''">
-        
-        This is the code associated with the following publications:
-        
-        **Journal Version:** M. Everett, Y. Chen, and J. P. How, "Collision Avoidance in Pedestrian-Rich Environments with Deep Reinforcement Learning", IEEE Access Vol. 9, 2021, pp. 10357-10377. [10.1109/ACCESS.2021.3050338](http://doi.org/10.1109/ACCESS.2021.3050338), [Arxiv PDF](https://arxiv.org/abs/1910.11689)
-        
-        **Conference Version:** M. Everett, Y. Chen, and J. P. How, "Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning", IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2018. [Arxiv PDF](https://arxiv.org/abs/1805.01956), [Link to Video](https://www.youtube.com/watch?v=XHoXkWLhwYQ)
-        
-        This repo also contains the trained policy for the SA-CADRL paper (referred to as CADRL here) from the proceeding paper: Y. Chen, M. Everett, M. Liu, and J. P. How. “Socially Aware Motion Planning with Deep Reinforcement Learning.” IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). Vancouver, BC, Canada, Sept. 2017. [Arxiv PDF](https://arxiv.org/abs/1703.08862)
-        
-        If you're looking to train our GA3C-CADRL policy, please see [this repo](https://github.com/mit-acl/rl_collision_avoidance) instead.
-        
-        ---
-        
-        ### About the Code
-        
-        Please see [the documentation](https://gym-collision-avoidance.readthedocs.io/en/latest/)!
-        
-        ### If you find this code useful, please consider citing:
-        
-        ```
-        @inproceedings{Everett18_IROS,
-          address = {Madrid, Spain},
-          author = {Everett, Michael and Chen, Yu Fan and How, Jonathan P.},
-          booktitle = {IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
-          date-modified = {2018-10-03 06:18:08 -0400},
-          month = sep,
-          title = {Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning},
-          year = {2018},
-          url = {https://arxiv.org/pdf/1805.01956.pdf},
-          bdsk-url-1 = {https://arxiv.org/pdf/1805.01956.pdf}
-        }
-        ```
-        
-        or
-        
-        ```
-        @article{everett2021collision,
-          title={Collision avoidance in pedestrian-rich environments with deep reinforcement learning},
-          author={Everett, Michael and Chen, Yu Fan and How, Jonathan P},
-          journal={IEEE Access},
-          volume={9},
-          pages={10357--10377},
-          year={2021},
-          publisher={IEEE}
-        }
-        ```
-        
 Keywords: robotics planning gym rl
-Platform: UNKNOWN
-Requires-Python: <3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# gym-collision-avoidance
+
+Updates:
+- **2023-04-28:** Updated to be compatible with Python 3.10 and tensorflow 2. Corresponding v0.0.3 available on pypi as well, if you do not intend to modify the source code (`python -m pip install gym-collision-avoidance`)
+
+<img src="docs/_static/combo.gif" alt="Agents spelling ``CADRL''">
+
+This is the code associated with the following publications:
+
+**Journal Version:** M. Everett, Y. Chen, and J. P. How, "Collision Avoidance in Pedestrian-Rich Environments with Deep Reinforcement Learning", IEEE Access Vol. 9, 2021, pp. 10357-10377. [10.1109/ACCESS.2021.3050338](http://doi.org/10.1109/ACCESS.2021.3050338), [Arxiv PDF](https://arxiv.org/abs/1910.11689)
+
+**Conference Version:** M. Everett, Y. Chen, and J. P. How, "Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning", IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2018. [Arxiv PDF](https://arxiv.org/abs/1805.01956), [Link to Video](https://www.youtube.com/watch?v=XHoXkWLhwYQ)
+
+This repo also contains the trained policy for the SA-CADRL paper (referred to as CADRL here) from the proceeding paper: Y. Chen, M. Everett, M. Liu, and J. P. How. “Socially Aware Motion Planning with Deep Reinforcement Learning.” IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). Vancouver, BC, Canada, Sept. 2017. [Arxiv PDF](https://arxiv.org/abs/1703.08862)
+
+If you're looking to train our GA3C-CADRL policy, please see [this repo](https://github.com/mit-acl/rl_collision_avoidance) instead.
+
+---
+
+### About the Code
+
+Please see [the documentation](https://gym-collision-avoidance.readthedocs.io/en/latest/)!
+
+### If you find this code useful, please consider citing:
+
+```
+@inproceedings{Everett18_IROS,
+  address = {Madrid, Spain},
+  author = {Everett, Michael and Chen, Yu Fan and How, Jonathan P.},
+  booktitle = {IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
+  date-modified = {2018-10-03 06:18:08 -0400},
+  month = sep,
+  title = {Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning},
+  year = {2018},
+  url = {https://arxiv.org/pdf/1805.01956.pdf},
+  bdsk-url-1 = {https://arxiv.org/pdf/1805.01956.pdf}
+}
+```
+
+or
+
+```
+@article{everett2021collision,
+  title={Collision avoidance in pedestrian-rich environments with deep reinforcement learning},
+  author={Everett, Michael and Chen, Yu Fan and How, Jonathan P},
+  journal={IEEE Access},
+  volume={9},
+  pages={10357--10377},
+  year={2021},
+  publisher={IEEE}
+}
+```
```

### Comparing `gym_collision_avoidance-0.0.2.post2/gym_collision_avoidance.egg-info/SOURCES.txt` & `gym_collision_avoidance-0.0.3/gym_collision_avoidance.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MANIFEST.in
+LICENSE
 README.md
 setup.py
 gym_collision_avoidance/__init__.py
 gym_collision_avoidance.egg-info/PKG-INFO
 gym_collision_avoidance.egg-info/SOURCES.txt
 gym_collision_avoidance.egg-info/dependency_links.txt
 gym_collision_avoidance.egg-info/requires.txt
@@ -35,14 +35,18 @@
 gym_collision_avoidance/envs/policies/Policy.py
 gym_collision_avoidance/envs/policies/RVOPolicy.py
 gym_collision_avoidance/envs/policies/StaticPolicy.py
 gym_collision_avoidance/envs/policies/__init__.py
 gym_collision_avoidance/envs/policies/CADRL/__init__.py
 gym_collision_avoidance/envs/policies/CADRL/pickle_files/__init__.py
 gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/__init__.py
+gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/nn_rl_training_param.p
+gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/nn_training_param.p
+gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/no_constr_none/RL_selfplay/4_agents_policy_iter_1000.p
+gym_collision_avoidance/envs/policies/CADRL/pickle_files/multi/rotate_constr_right/RL_selfplay/4_agents_policy_iter_1300.p
 gym_collision_avoidance/envs/policies/CADRL/scripts/__init__.py
 gym_collision_avoidance/envs/policies/CADRL/scripts/multi/__init__.py
 gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_plots_multi.py
 gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_rand_testcases.py
 gym_collision_avoidance/envs/policies/CADRL/scripts/multi/gen_results_multi.py
 gym_collision_avoidance/envs/policies/CADRL/scripts/multi/global_var.py
 gym_collision_avoidance/envs/policies/CADRL/scripts/multi/nn_debug_multi.py
@@ -73,14 +77,20 @@
 gym_collision_avoidance/envs/policies/DRL_Long/model/ppo.py
 gym_collision_avoidance/envs/policies/DRL_Long/model/utils.py
 gym_collision_avoidance/envs/policies/GA3C_CADRL/__init__.py
 gym_collision_avoidance/envs/policies/GA3C_CADRL/network.py
 gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.data-00000-of-00001
 gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.index
 gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/IROS18/network_01900000.meta
+gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_015942-jzuhlntn/network_01490000.data-00000-of-00001
+gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_015942-jzuhlntn/network_01490000.index
+gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_015942-jzuhlntn/network_01490000.meta
+gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_192048-qedrf08y/network_01900000.data-00000-of-00001
+gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_192048-qedrf08y/network_01900000.index
+gym_collision_avoidance/envs/policies/GA3C_CADRL/checkpoints/run-20190727_192048-qedrf08y/network_01900000.meta
 gym_collision_avoidance/envs/sensors/LaserScanSensor.py
 gym_collision_avoidance/envs/sensors/OccupancyGridSensor.py
 gym_collision_avoidance/envs/sensors/OtherAgentsStatesSensor.py
 gym_collision_avoidance/envs/sensors/Sensor.py
 gym_collision_avoidance/envs/sensors/__init__.py
 gym_collision_avoidance/experiments/__init__.py
 gym_collision_avoidance/experiments/src/__init__.py
```

