# Comparing `tmp/openrl-0.0.5.tar.gz` & `tmp/openrl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrl-0.0.5.tar", last modified: Wed Apr 26 15:36:17 2023, max compression
+gzip compressed data, was "openrl-0.0.6.tar", last modified: Fri Apr 28 10:05:16 2023, max compression
```

## Comparing `openrl-0.0.5.tar` & `openrl-0.0.6.tar`

### file list

```diff
@@ -1,172 +1,173 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.149727 openrl-0.0.5/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-12 14:31:37.000000 openrl-0.0.5/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.5/LICENSE.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)    11299 2023-04-26 15:36:17.149418 openrl-0.0.5/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)    10214 2023-04-26 08:59:55.000000 openrl-0.0.5/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.115630 openrl-0.0.5/openrl/
--rw-r--r--   0 4paradigm   (501) staff       (20)      194 2023-04-26 13:13:37.000000 openrl-0.0.5/openrl/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.117819 openrl-0.0.5/openrl/algorithms/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/algorithms/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/algorithms/base_algorithm.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/algorithms/ppo.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.118964 openrl-0.0.5/openrl/buffers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/buffers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-18 09:40:26.000000 openrl-0.0.5/openrl/buffers/normal_buffer.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/buffers/replay_data.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.120182 openrl-0.0.5/openrl/buffers/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/buffers/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/buffers/utils/obs_data.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/buffers/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.120705 openrl-0.0.5/openrl/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/cli/cli.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-26 12:06:55.000000 openrl-0.0.5/openrl/cli/train.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.121193 openrl-0.0.5/openrl/configs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/configs/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-26 12:06:55.000000 openrl-0.0.5/openrl/configs/config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.122275 openrl-0.0.5/openrl/drivers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/drivers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/drivers/base_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9926 2023-04-26 12:08:00.000000 openrl-0.0.5/openrl/drivers/onpolicy_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/drivers/rl_driver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.122480 openrl-0.0.5/openrl/envs/
--rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.123191 openrl-0.0.5/openrl/envs/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/common/build_envs.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3299 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/common/registration.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.123446 openrl-0.0.5/openrl/envs/gymnasium/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/gymnasium/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.126217 openrl-0.0.5/openrl/envs/mpe/
--rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-18 09:57:30.000000 openrl-0.0.5/openrl/envs/mpe/core.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/mpe_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/multi_discrete.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/multiagent_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/rendering.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/scenario.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.126558 openrl-0.0.5/openrl/envs/mpe/scenarios/
--rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/scenarios/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/mpe/scenarios/simple_spread.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.127627 openrl-0.0.5/openrl/envs/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7259 2023-04-26 12:38:02.000000 openrl-0.0.5/openrl/envs/nlp/daily_dialog_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/nlp/nlp_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11061 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/nlp/nlp_rewards.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.129228 openrl-0.0.5/openrl/envs/nlp/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-26 13:39:44.000000 openrl-0.0.5/openrl/envs/nlp/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/envs/nlp/utils/custom_text_generation_pools.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-26 12:50:40.000000 openrl-0.0.5/openrl/envs/nlp/utils/distribution.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/envs/nlp/utils/evaluation_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.129875 openrl-0.0.5/openrl/envs/nlp/utils/metrics/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-26 08:59:55.000000 openrl-0.0.5/openrl/envs/nlp/utils/metrics/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/envs/nlp/utils/metrics/meteor.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-26 12:51:48.000000 openrl-0.0.5/openrl/envs/nlp/utils/observation.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/nlp/utils/sampler.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/nlp/utils/text_generation_pool.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.131039 openrl-0.0.5/openrl/envs/vec_env/
--rw-r--r--   0 4paradigm   (501) staff       (20)      326 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/vec_env/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/async_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7845 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/vec_env/base_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/sync_venv.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.132089 openrl-0.0.5/openrl/envs/vec_env/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/envs/vec_env/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/utils/numpy_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/utils/share_memory.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/envs/vec_env/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.133414 openrl-0.0.5/openrl/envs/vec_env/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2174 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/reward_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3343 2023-04-26 12:42:13.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2078 2023-04-26 12:38:40.000000 openrl-0.0.5/openrl/envs/vec_env/wrappers/vec_monitor.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.134682 openrl-0.0.5/openrl/envs/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2199 2023-04-26 08:59:48.000000 openrl-0.0.5/openrl/envs/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/wrappers/extra_wrappers.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-13 02:35:11.000000 openrl-0.0.5/openrl/envs/wrappers/multiagent_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/envs/wrappers/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.135757 openrl-0.0.5/openrl/modules/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/modules/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-14 07:55:18.000000 openrl-0.0.5/openrl/modules/base_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.136502 openrl-0.0.5/openrl/modules/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/modules/common/base_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3407 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/common/ppo_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/model_config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.138190 openrl-0.0.5/openrl/modules/networks/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/modules/networks/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-14 07:55:00.000000 openrl-0.0.5/openrl/modules/networks/base_policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/base_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/policy_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3967 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/modules/networks/policy_value_network_gpt.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.140445 openrl-0.0.5/openrl/modules/networks/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2022-09-12 08:05:59.000000 openrl-0.0.5/openrl/modules/networks/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-26 12:18:00.000000 openrl-0.0.5/openrl/modules/networks/utils/act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/attention.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/cnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/distributed_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/distributions.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/mix.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/mlp.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.141256 openrl-0.0.5/openrl/modules/networks/utils/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2022-09-12 08:05:59.000000 openrl-0.0.5/openrl/modules/networks/utils/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/modules/networks/utils/nlp/base_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/modules/networks/utils/nlp/causal_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-26 13:14:53.000000 openrl-0.0.5/openrl/modules/networks/utils/nlp/hf_generation_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/popart.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/rnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/transformer_act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/networks/value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/ppo_module.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/rl_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.142672 openrl-0.0.5/openrl/modules/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/modules/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/modules/utils/valuenorm.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.143559 openrl-0.0.5/openrl/rewards/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-26 08:59:55.000000 openrl-0.0.5/openrl/rewards/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      366 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/rewards/base_reward.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2808 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/rewards/nlp_reward.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      572 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/rewards/register.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.143787 openrl-0.0.5/openrl/runners/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/runners/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.145211 openrl-0.0.5/openrl/runners/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      156 2023-04-26 13:14:42.000000 openrl-0.0.5/openrl/runners/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/runners/common/base_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3186 2023-04-26 13:56:42.000000 openrl-0.0.5/openrl/runners/common/chat_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6112 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/runners/common/ppo_agent.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.145417 openrl-0.0.5/openrl/supports/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/supports/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.145681 openrl-0.0.5/openrl/supports/opendata/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-26 13:08:19.000000 openrl-0.0.5/openrl/supports/opendata/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.146289 openrl-0.0.5/openrl/supports/opendata/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-26 13:08:19.000000 openrl-0.0.5/openrl/supports/opendata/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-26 12:30:15.000000 openrl-0.0.5/openrl/supports/opendata/utils/opendata_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.146921 openrl-0.0.5/openrl/supports/opengpu/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-26 13:08:19.000000 openrl-0.0.5/openrl/supports/opengpu/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3897 2023-04-26 13:11:15.000000 openrl-0.0.5/openrl/supports/opengpu/gpu_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7051 2023-04-26 13:14:52.000000 openrl-0.0.5/openrl/supports/opengpu/manager.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.147913 openrl-0.0.5/openrl/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/openrl/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-26 13:12:54.000000 openrl-0.0.5/openrl/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-25 09:16:38.000000 openrl-0.0.5/openrl/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.116857 openrl-0.0.5/openrl.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11299 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     4465 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      284 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-04-26 15:36:17.000000 openrl-0.0.5/openrl.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-04-26 15:36:17.149782 openrl-0.0.5/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     3066 2023-04-26 14:24:44.000000 openrl-0.0.5/setup.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.148153 openrl-0.0.5/tests/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/tests/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.148713 openrl-0.0.5/tests/project/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/tests/project/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-25 09:16:38.000000 openrl-0.0.5/tests/project/test_version.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-26 15:36:17.149152 openrl-0.0.5/tests/test_buffer/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.5/tests/test_buffer/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-25 09:16:38.000000 openrl-0.0.5/tests/test_buffer/test_buffer.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.776518 openrl-0.0.6/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.0.6/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11261 2023-04-28 10:05:16.776305 openrl-0.0.6/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10202 2023-04-28 07:15:42.000000 openrl-0.0.6/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.752503 openrl-0.0.6/openrl/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      194 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.753887 openrl-0.0.6/openrl/algorithms/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/algorithms/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/algorithms/base_algorithm.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/algorithms/ppo.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.754560 openrl-0.0.6/openrl/buffers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/normal_buffer.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/buffers/replay_data.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.755583 openrl-0.0.6/openrl/buffers/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/utils/obs_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.756098 openrl-0.0.6/openrl/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/cli/cli.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/cli/train.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.756418 openrl-0.0.6/openrl/configs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/configs/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/configs/config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.757152 openrl-0.0.6/openrl/drivers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/drivers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/drivers/base_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9929 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/drivers/onpolicy_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/drivers/rl_driver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.757300 openrl-0.0.6/openrl/envs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.757794 openrl-0.0.6/openrl/envs/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/common/build_envs.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3305 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/common/registration.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.758126 openrl-0.0.6/openrl/envs/gymnasium/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-28 09:05:04.000000 openrl-0.0.6/openrl/envs/gymnasium/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.759657 openrl-0.0.6/openrl/envs/mpe/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/core.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/mpe_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/multi_discrete.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/multiagent_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/rendering.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/scenario.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.760034 openrl-0.0.6/openrl/envs/mpe/scenarios/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/scenarios/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/scenarios/simple_spread.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.760570 openrl-0.0.6/openrl/envs/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/nlp/daily_dialog_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/nlp_env.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.761850 openrl-0.0.6/openrl/envs/nlp/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/custom_text_generation_pools.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/distribution.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/evaluation_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.762196 openrl-0.0.6/openrl/envs/nlp/utils/metrics/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/metrics/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/metrics/meteor.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/observation.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/sampler.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/text_generation_pool.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.762935 openrl-0.0.6/openrl/envs/vec_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      348 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/async_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7845 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/vec_env/base_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/sync_venv.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.763829 openrl-0.0.6/openrl/envs/vec_env/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/vec_env/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/utils/numpy_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/utils/share_memory.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/vec_env/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.764491 openrl-0.0.6/openrl/envs/vec_env/vec_info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1058 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/vec_info/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/vec_info/base_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/vec_info/nlp_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1222 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/vec_info/simple_vec_info.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.765234 openrl-0.0.6/openrl/envs/vec_env/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/vec_env/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2046 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/wrappers/reward_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.766127 openrl-0.0.6/openrl/envs/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1612 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/wrappers/extra_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/wrappers/multiagent_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/wrappers/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.766960 openrl-0.0.6/openrl/modules/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/base_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.767532 openrl-0.0.6/openrl/modules/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/common/base_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3441 2023-04-28 09:15:51.000000 openrl-0.0.6/openrl/modules/common/ppo_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/model_config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.768638 openrl-0.0.6/openrl/modules/networks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/base_policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/base_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/policy_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3991 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/modules/networks/policy_value_network_gpt.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.770506 openrl-0.0.6/openrl/modules/networks/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/attention.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/cnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/distributed_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/distributions.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/mix.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/mlp.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.771122 openrl-0.0.6/openrl/modules/networks/utils/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/nlp/base_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/modules/networks/utils/nlp/causal_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/modules/networks/utils/nlp/hf_generation_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/popart.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/rnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/transformer_act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/ppo_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/rl_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.772313 openrl-0.0.6/openrl/modules/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/utils/valuenorm.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.772893 openrl-0.0.6/openrl/rewards/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      919 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/rewards/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1102 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/rewards/base_reward.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/rewards/nlp_reward.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.773041 openrl-0.0.6/openrl/runners/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/runners/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.773713 openrl-0.0.6/openrl/runners/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      156 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/runners/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/runners/common/base_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3185 2023-04-28 09:15:51.000000 openrl-0.0.6/openrl/runners/common/chat_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6083 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/runners/common/ppo_agent.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.773856 openrl-0.0.6/openrl/supports/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.773989 openrl-0.0.6/openrl/supports/opendata/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opendata/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.774266 openrl-0.0.6/openrl/supports/opendata/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opendata/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opendata/utils/opendata_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.774787 openrl-0.0.6/openrl/supports/opengpu/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opengpu/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3897 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opengpu/gpu_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7051 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/supports/opengpu/manager.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.775355 openrl-0.0.6/openrl/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.753259 openrl-0.0.6/openrl.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11261 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4542 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      284 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-04-28 10:05:16.776564 openrl-0.0.6/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3066 2023-04-28 09:15:51.000000 openrl-0.0.6/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.775497 openrl-0.0.6/tests/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.775786 openrl-0.0.6/tests/project/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/project/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/project/test_version.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.776072 openrl-0.0.6/tests/test_buffer/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/test_buffer/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/test_buffer/test_buffer.py
```

### Comparing `openrl-0.0.5/LICENSE` & `openrl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/PKG-INFO` & `openrl-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.5
+Version: 0.0.6
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
@@ -18,15 +18,14 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mpe
 Provides-Extra: nlp
 License-File: LICENSE
-License-File: LICENSE.txt
 
 <div align="center">
     <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
@@ -34,29 +33,29 @@
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://codecov.io/gh/OpenRL-Lab/openrl)
 
-[![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 [![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
+[![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
-![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL)
+![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL-Lab)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.5 is updated on April 19, 2023 
+OpenRL-v0.0.6 is updated on April 28, 2023 
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
```

#### html2text {}

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.5 Summary: unified
+Metadata-Version: 2.1 Name: openrl Version: 0.0.6 Summary: unified
 reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
 openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
 URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
 https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
 multi-agent reinforcement-learning-algorithms pytorch machine-learning
 baselines toolbox python data-science gym gymnasium Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Provides-Extra: test Provides-Extra: dev Provides-Extra: mpe Provides-Extra:
-nlp License-File: LICENSE License-File: LICENSE.txt
+nlp License-File: LICENSE
                         [./docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
 openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl) [!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg)](https://github.com/psf/black) [![Hits-of-Code](https://
 hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/
 github/OpenRL-Lab/openrl/view?branch=main) [![codecov](https://codecov.io/gh/
-OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https:
-//codecov.io/gh/OpenRL-Lab/openrl_release) [![Read the Docs](https://
+OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://
+codecov.io/gh/OpenRL-Lab/openrl) [![Documentation Status](https://
+readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
+docs.readthedocs.io/zh/latest/?badge=latest) [![Read the Docs](https://
 img.shields.io/readthedocs/openrl-docs-
 zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-
-docs.readthedocs.io/zh/latest/) [![Documentation Status](https://
-readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
-docs.readthedocs.io/zh/latest/?badge=latest) ![GitHub Org's stars](https://
-img.shields.io/github/stars/OpenRL) [![GitHub stars](https://img.shields.io/
-github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/
-stargazers) [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/
-openrl)](https://github.com/OpenRL-Lab/openrl/network) ![GitHub commit
-activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [!
-[GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https:
-//github.com/OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/
-github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
-pulls) [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/
-openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub
-license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://
-github.com/OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.5 is updated on
-April 19, 2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
-(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
-openrl-docs.readthedocs.io/en/latest/
+docs.readthedocs.io/zh/latest/) ![GitHub Org's stars](https://img.shields.io/
+github/stars/OpenRL-Lab) [![GitHub stars](https://img.shields.io/github/stars/
+OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers) [![GitHub
+forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://
+github.com/OpenRL-Lab/openrl/network) ![GitHub commit activity](https://
+img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
+(https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
+OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
+issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
+[Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
+(https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.6 is updated on April 28,
+2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
+openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
+docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
 ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
 æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
 [Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
```

### Comparing `openrl-0.0.5/README.md` & `openrl-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://codecov.io/gh/OpenRL-Lab/openrl)
 
-[![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 [![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
+[![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
-![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL)
+![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL-Lab)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.5 is updated on April 19, 2023 
+OpenRL-v0.0.6 is updated on April 28, 2023 
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
```

#### html2text {}

```diff
@@ -6,36 +6,36 @@
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
 openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl) [!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg)](https://github.com/psf/black) [![Hits-of-Code](https://
 hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/
 github/OpenRL-Lab/openrl/view?branch=main) [![codecov](https://codecov.io/gh/
-OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https:
-//codecov.io/gh/OpenRL-Lab/openrl_release) [![Read the Docs](https://
+OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://
+codecov.io/gh/OpenRL-Lab/openrl) [![Documentation Status](https://
+readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
+docs.readthedocs.io/zh/latest/?badge=latest) [![Read the Docs](https://
 img.shields.io/readthedocs/openrl-docs-
 zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-
-docs.readthedocs.io/zh/latest/) [![Documentation Status](https://
-readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
-docs.readthedocs.io/zh/latest/?badge=latest) ![GitHub Org's stars](https://
-img.shields.io/github/stars/OpenRL) [![GitHub stars](https://img.shields.io/
-github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/
-stargazers) [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/
-openrl)](https://github.com/OpenRL-Lab/openrl/network) ![GitHub commit
-activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [!
-[GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https:
-//github.com/OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/
-github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
-pulls) [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/
-openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub
-license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://
-github.com/OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.5 is updated on
-April 19, 2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
-(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
-openrl-docs.readthedocs.io/en/latest/
+docs.readthedocs.io/zh/latest/) ![GitHub Org's stars](https://img.shields.io/
+github/stars/OpenRL-Lab) [![GitHub stars](https://img.shields.io/github/stars/
+OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers) [![GitHub
+forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://
+github.com/OpenRL-Lab/openrl/network) ![GitHub commit activity](https://
+img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
+(https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
+OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
+issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
+[Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
+(https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.6 is updated on April 28,
+2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
+openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
+docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
 ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
 æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
 [Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
```

### Comparing `openrl-0.0.5/openrl/algorithms/__init__.py` & `openrl-0.0.6/openrl/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/algorithms/base_algorithm.py` & `openrl-0.0.6/openrl/algorithms/base_algorithm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/algorithms/ppo.py` & `openrl-0.0.6/openrl/algorithms/ppo.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/buffers/__init__.py` & `openrl-0.0.6/openrl/buffers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/buffers/normal_buffer.py` & `openrl-0.0.6/openrl/buffers/normal_buffer.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/buffers/replay_data.py` & `openrl-0.0.6/openrl/buffers/replay_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/buffers/utils/__init__.py` & `openrl-0.0.6/openrl/buffers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/buffers/utils/obs_data.py` & `openrl-0.0.6/openrl/buffers/utils/obs_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/buffers/utils/util.py` & `openrl-0.0.6/openrl/buffers/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/cli/__init__.py` & `openrl-0.0.6/openrl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/cli/cli.py` & `openrl-0.0.6/openrl/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/cli/train.py` & `openrl-0.0.6/openrl/cli/train.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/configs/__init__.py` & `openrl-0.0.6/openrl/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/configs/config.py` & `openrl-0.0.6/openrl/configs/config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/drivers/__init__.py` & `openrl-0.0.6/openrl/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/drivers/onpolicy_driver.py` & `openrl-0.0.6/openrl/drivers/onpolicy_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,28 +171,23 @@
         )
 
     def actor_rollout(self):
         self.trainer.prep_rollout()
         import time
 
         for step in range(self.episode_length):
-            act_data = self.act(step)
-
-            (
-                values,
-                actions,
-                action_log_probs,
-                rnn_states,
-                rnn_states_critic,
-            ) = act_data
+            values, actions, action_log_probs, rnn_states, rnn_states_critic = self.act(
+                step
+            )
 
             extra_data = {
-                "act_data": act_data,
-                "buffer": self.buffer,
+                "values": values,
+                "action_log_probs": action_log_probs,
                 "step": step,
+                "buffer": self.buffer,
             }
 
             obs, rewards, dones, infos = self.envs.step(actions, extra_data)
 
             data = (
                 obs,
                 rewards,
@@ -202,21 +197,23 @@
                 actions,
                 action_log_probs,
                 rnn_states,
                 rnn_states_critic,
             )
 
             self.add2buffer(data)
-        infos = self.envs.batch_rewards(self.buffer)
+
+        batch_rew_infos = self.envs.batch_rewards(self.buffer)
+
         if self.envs.use_monitor:
-            statistics_info = self.envs.statistics()
-            infos.update(statistics_info)
-            return infos
+            statistics_info = self.envs.statistics(self.buffer)
+            statistics_info.update(batch_rew_infos)
+            return statistics_info
         else:
-            return infos
+            return batch_rew_infos
 
     def run(self) -> None:
         episodes = (
             int(self.num_env_steps)
             // self.episode_length
             // self.learner_n_rollout_threads
         )
```

### Comparing `openrl-0.0.5/openrl/drivers/rl_driver.py` & `openrl-0.0.6/openrl/drivers/rl_driver.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/common/__init__.py` & `openrl-0.0.6/openrl/envs/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/common/build_envs.py` & `openrl-0.0.6/openrl/envs/common/build_envs.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/common/registration.py` & `openrl-0.0.6/openrl/envs/common/registration.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,22 @@
 """"""
 from typing import Optional
 
 import gymnasium as gym
 from gymnasium import Env
 
 import openrl
-from openrl.envs.vec_env import AsyncVectorEnv, RewardWrapper, SyncVectorEnv, VecMonitor
-from openrl.envs.vec_env.wrappers.vec_monitor import VecInfoFactory
+from openrl.envs.vec_env import (
+    AsyncVectorEnv,
+    RewardWrapper,
+    SyncVectorEnv,
+    VecMonitorWrapper,
+)
+from openrl.envs.vec_env.vec_info import VecInfoFactory
+from openrl.rewards import RewardFactory
 
 
 def make(
     id: str,
     cfg=None,
     env_num: int = 1,
     asynchronous: bool = False,
@@ -74,23 +80,18 @@
         raise NotImplementedError(f"env {id} is not supported.")
 
     if asynchronous:
         env = AsyncVectorEnv(env_fns, render_mode=render_mode)
     else:
         env = SyncVectorEnv(env_fns, render_mode=render_mode)
 
-    if cfg is not None:
-        from openrl.rewards.register import RewardFactory
-
-        reward_class = RewardFactory.get_reward_class(cfg.reward_class, env)
-    else:
-        reward_class = None
+    reward_class = cfg.reward_class if cfg else None
+    reward_class = RewardFactory.get_reward_class(reward_class, env)
 
     env = RewardWrapper(env, reward_class)
 
     if add_monitor:
-        vec_info_class = VecInfoFactory.get_vec_info_class(
-            cfg.vec_info_class if cfg else None, env
-        )
-        env = VecMonitor(vec_info_class, env)
+        vec_info_class = cfg.vec_info_class if cfg else None
+        vec_info_class = VecInfoFactory.get_vec_info_class(vec_info_class, env)
+        env = VecMonitorWrapper(vec_info_class, env)
 
     return env
```

### Comparing `openrl-0.0.5/openrl/envs/gymnasium/__init__.py` & `openrl-0.0.6/openrl/envs/gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/mpe/__init__.py` & `openrl-0.0.6/openrl/envs/mpe/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/mpe/core.py` & `openrl-0.0.6/openrl/envs/mpe/core.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/mpe/mpe_env.py` & `openrl-0.0.6/openrl/envs/mpe/mpe_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/mpe/multi_discrete.py` & `openrl-0.0.6/openrl/envs/mpe/multi_discrete.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/mpe/multiagent_env.py` & `openrl-0.0.6/openrl/envs/mpe/multiagent_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/mpe/rendering.py` & `openrl-0.0.6/openrl/envs/mpe/rendering.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/mpe/scenarios/simple_spread.py` & `openrl-0.0.6/openrl/envs/mpe/scenarios/simple_spread.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/__init__.py` & `openrl-0.0.6/openrl/envs/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/daily_dialog_env.py` & `openrl-0.0.6/openrl/envs/nlp/daily_dialog_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from openrl.envs.nlp.utils.text_generation_pool import Sample
 
 
 class DailyDialogEnv(Env):
     def __init__(
         self,
         cfg,
-        max_episode_length: int = 20,  # 512,
+        max_episode_length: int = 20,
         priority_scale: float = 0.0,
-        max_prompt_length: Optional[int] = 128,  # None,
+        max_prompt_length: Optional[int] = 128,
         terminate_on_eos: bool = True,  # False,
         context_start_token: Optional[int] = None,
         prompt_truncation_side: str = "left",
     ):
         """
         A generic RL environment to generate textual sequences.
         For eg: text generation, summarization, machine translation, text simplification
@@ -32,15 +32,15 @@
             priority_scale (float, optional): weight for the priority sampler Defaults to 0.0.
             max_prompt_length (Optional[int], optional): maximum prompt length. Defaults to None.
             terminate_on_eos (bool, optional): whether to terminate on EOS. Defaults to False.
             context_start_token (bool, optional): start token for the context (For Encoder-Decoder models! )
             prompt_truncation_side (str): truncation side for prompt text (Defaults to "left")
         """
 
-        self.debug = cfg.data_path is None
+        self.debug = cfg.env.args["data_path"] is None
 
         self.env_name = "daily_dialog"
         tokenizer_name = cfg.env.args["tokenizer_path"]
         self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name, use_fast=True)
         if self.tokenizer.pad_token is None:
             self.tokenizer.pad_token = self.tokenizer.eos_token
         self.tokenizer.padding_side = "left"
@@ -81,15 +81,15 @@
             n = 32128
             self.action_space = Discrete(n=n)
 
         if not self.debug:
             self.sampler_for_replaying = PrioritySampler(priority_scale=priority_scale)
 
             samples_config = {}
-            samples_config["data_path"] = cfg.data_path
+            samples_config["data_path"] = cfg.env.args["data_path"]
             samples_config["context_size"] = 5
             samples_config["split"] = "train"
             samples_config["small_debug"] = False
             samples = DailyDialog.prepare(**samples_config)
 
             for sample, weight in samples:
                 self.sampler_for_replaying.add(sample, weight)
@@ -118,29 +118,34 @@
         done = (action == self.tokenizer.eos_token_id and self._terminate_on_eos) or (
             self.__time_step == self.max_steps
         )
 
         done = done or self.__current_obs.context_text.endswith(DailyDialog.EOU_TOKEN)
 
         reward = 0.0
-        reward_info = {}
+        reward_info = dict()
 
-        if self.reward_function is None:
-            pass
-        else:
-            for reward_function in self.reward_function:
-                reward_new, reward_info_new = reward_function(
-                    [self.__current_obs.prompt_or_input_text],
-                    [self.__current_obs.context_text],
-                    [self.__current_obs.target_or_reference_texts],
-                    [done],
-                    [self.__current_obs.meta_info],
-                )
+        if done and self.reward_function:
+            for reward_function in self.reward_function.values():
+                inner_reward_data = {
+                    "generated_texts": self.__current_obs.context_text,
+                    "reference_texts": self.__current_obs.target_or_reference_texts,
+                }
+                reward_new, reward_info_new = reward_function(inner_reward_data)
                 reward += reward_new
                 reward_info.update(reward_info_new)
+
+        if done:
+            batch_reward_data = {
+                "generated_texts": self.__current_obs.context_text,
+                "prompt_texts": self.__current_obs.prompt_or_input_text,
+                "meta_infos": self.__current_obs.meta_info,
+            }
+            reward_info.update(batch_reward_data)
+
         # populate additional info
         info = dict()
         info.update(reward_info)
 
         obs = self.__current_obs.to_dict()
 
         return obs, reward, done, done, info
```

### Comparing `openrl-0.0.5/openrl/envs/nlp/utils/custom_text_generation_pools.py` & `openrl-0.0.6/openrl/envs/nlp/utils/custom_text_generation_pools.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/utils/distribution.py` & `openrl-0.0.6/openrl/envs/nlp/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/utils/evaluation_utils.py` & `openrl-0.0.6/openrl/envs/nlp/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/utils/metrics/__init__.py` & `openrl-0.0.6/openrl/envs/nlp/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/utils/metrics/meteor.py` & `openrl-0.0.6/openrl/envs/nlp/utils/metrics/meteor.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/utils/observation.py` & `openrl-0.0.6/openrl/envs/nlp/utils/observation.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/utils/sampler.py` & `openrl-0.0.6/openrl/envs/nlp/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/nlp/utils/text_generation_pool.py` & `openrl-0.0.6/openrl/envs/nlp/utils/text_generation_pool.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/async_venv.py` & `openrl-0.0.6/openrl/envs/vec_env/async_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/base_venv.py` & `openrl-0.0.6/openrl/envs/vec_env/base_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/sync_venv.py` & `openrl-0.0.6/openrl/envs/vec_env/sync_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/utils/__init__.py` & `openrl-0.0.6/openrl/envs/vec_env/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/utils/numpy_utils.py` & `openrl-0.0.6/openrl/envs/vec_env/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/utils/share_memory.py` & `openrl-0.0.6/openrl/envs/vec_env/utils/share_memory.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/utils/util.py` & `openrl-0.0.6/openrl/envs/vec_env/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/wrappers/__init__.py` & `openrl-0.0.6/openrl/envs/vec_env/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/wrappers/base_wrapper.py` & `openrl-0.0.6/openrl/envs/vec_env/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/vec_env/wrappers/reward_wrapper.py` & `openrl-0.0.6/openrl/envs/vec_env/wrappers/reward_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,46 +11,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional, Union
 
+import numpy as np
 from gymnasium.core import ActType
 
 from openrl.envs.vec_env.base_venv import BaseVecEnv
 from openrl.envs.vec_env.wrappers.base_wrapper import VecEnvWrapper
 from openrl.rewards.base_reward import BaseReward
 
 
 class RewardWrapper(VecEnvWrapper):
-    def __init__(self, env: BaseVecEnv, reward_class: Optional[BaseReward] = None):
+    def __init__(self, env: BaseVecEnv, reward_class: BaseReward):
         super().__init__(env)
         self.reward_class = reward_class
-        if self.reward_class and len(self.reward_class.inner_reward_fn) > 0:
+        if len(self.reward_class.inner_reward_fn) > 0:
             env.call("set_reward", **{"reward_fn": self.reward_class.inner_reward_fn})
 
-    def step(self, action: ActType, extra_data: Optional[Dict[str, Any]] = None):
+    def step(
+        self, action: ActType, extra_data: Optional[Dict[str, Any]]
+    ) -> Union[Any, np.ndarray, np.ndarray, List[Dict[str, Any]]]:
         obs, rewards, dones, infos = self.env.step(action)
 
-        if self.reward_class is not None and extra_data is not None:
-            extra_data.update({"action": action})
+        if extra_data:
+            extra_data.update({"actions": action})
             extra_data.update({"obs": obs})
-            extra_data.update({"reward": rewards})
-            extra_data.update({"done": dones})
-            extra_data.update({"info": infos})
-            rewards, new_infos = self.reward_class.get_reward(data=extra_data)
-
-            if new_infos is not None:
-                num_envs = len(infos)
-                for i in range(num_envs):
-                    infos[i] = {**infos[i], **new_infos[i]}
+            extra_data.update({"rewards": rewards})
+            extra_data.update({"dones": dones})
+            extra_data.update({"infos": infos})
+            rewards, new_infos = self.reward_class.step_reward(data=extra_data)
+
+            num_envs = len(infos)
+            for i in range(num_envs):
+                infos[i].update(new_infos[i])
 
         return obs, rewards, dones, infos
 
     def batch_rewards(self, buffer):
-        infos = {}
-        if self.reward_class is not None:
-            infos = self.reward_class.batch_rewards(buffer)
-        return infos
+        return self.reward_class.batch_rewards(buffer)
```

### Comparing `openrl-0.0.5/openrl/envs/vec_env/wrappers/vec_info.py` & `openrl-0.0.6/openrl/envs/vec_env/vec_info/nlp_vec_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,69 @@
 import time
 from typing import Any, Dict
 
 import numpy as np
 
+from openrl.envs.vec_env.vec_info.base_vec_info import BaseVecInfo
 
-class NLPVecInfo:
-    def __init__(self, parallel_env_num, agent_num):
-        self.parallel_env_num = parallel_env_num
-        self.agent_num = agent_num
+
+class NLPVecInfo(BaseVecInfo):
+    def __init__(self, parallel_env_num: int, agent_num: int):
+        super().__init__(parallel_env_num, agent_num)
 
         self.episode_infos = []
-        self.rewards = []
 
         self.start_time = time.time()
         self.total_step = 0
 
         self.log_items = [
             "alpha",
             "kl_div",
-        ]
-        self.log_final_items = [
-            "intent_rewards",
-            "meteor_rewards",
+            "intent",
+            "meteor",
         ]
 
-    def statistics(self) -> Dict[str, Any]:
-        # this function should be called each episode
-        rewards = np.array(self.rewards)
+    def statistics(self, buffer: Any) -> Dict[str, Any]:
+        # get agent's episode reward
+        rewards = buffer.data.rewards.copy()
         self.total_step += np.prod(rewards.shape[:2])
         rewards = rewards.transpose(2, 1, 0, 3)
         info_dict = {}
         ep_rewards = []
         for i in range(self.agent_num):
             agent_reward = rewards[i].mean(0).sum()
             ep_rewards.append(agent_reward)
             info_dict["agent_{}/episode_reward".format(i)] = agent_reward
 
+        # get episode reward
+        info_dict["FPS"] = int(self.total_step / (time.time() - self.start_time))
+        info_dict["episode_reward"] = np.mean(ep_rewards)
+
+        # get env info
         new_infos = dict()
         for step_infos in self.episode_infos:
-            for env_infos in step_infos:
-                for key in env_infos:
-                    if key in new_infos:
-                        new_infos[key].append(env_infos[key])
-                    else:
-                        new_infos[key] = [env_infos[key]]
+            for env_info in step_infos:
+                for key in env_info:
+                    if key in self.log_items:
+                        if key in new_infos:
+                            new_infos[key].append(env_info[key])
+                        else:
+                            new_infos[key] = [env_info[key]]
+                if "final_info" in env_info:
+                    for key in env_info["final_info"]:
+                        if key in self.log_items:
+                            if key in new_infos:
+                                new_infos[key].append(env_info["final_info"][key])
+                            else:
+                                new_infos[key] = [env_info["final_info"][key]]
         for key in new_infos:
-            if key in self.log_items:
-                info_dict[key] = np.array(new_infos[key]).mean()
-        for key in self.log_final_items:
-            if "final_info" in new_infos:
-                info_dict[key] = np.array(
-                    [item[key] for item in new_infos["final_info"]]
-                ).mean()
-
-        info_dict["FPS"] = int(self.total_step / (time.time() - self.start_time))
-        info_dict["episode_reward"] = np.mean(ep_rewards)
+            new_infos[key] = np.array(new_infos[key]).mean()
+        info_dict.update(new_infos)
 
         return info_dict
 
-    def append(self, reward, info):
-        assert reward.shape[:2] == (self.parallel_env_num, self.agent_num)
+    def append(self, info: Dict[str, Any]) -> None:
         self.episode_infos.append(info)
-        self.rewards.append(reward)
 
-    def reset(self):
+    def reset(self) -> None:
         self.episode_infos = []
         self.rewards = []
-
-
-class VecInfo:
-    def __init__(self, parallel_env_num, agent_num):
-        self.parallel_env_num = parallel_env_num
-        self.agent_num = agent_num
-
-        self.infos = []
-        self.rewards = []
-
-        self.start_time = time.time()
-        self.total_step = 0
-
-    def statistics(self) -> Dict[str, Any]:
-        # this function should be called each episode
-        rewards = np.array(self.rewards)
-        self.total_step += np.prod(rewards.shape[:2])
-        rewards = rewards.transpose(2, 1, 0, 3)
-        info_dict = {}
-        ep_rewards = []
-        for i in range(self.agent_num):
-            agent_reward = rewards[i].mean(0).sum()
-            ep_rewards.append(agent_reward)
-            info_dict["agent_{}/episode_reward".format(i)] = agent_reward
-
-        info_dict["FPS"] = int(self.total_step / (time.time() - self.start_time))
-        info_dict["episode_reward"] = np.mean(ep_rewards)
-        return info_dict
-
-    def append(self, reward, info):
-        assert reward.shape[:2] == (self.parallel_env_num, self.agent_num)
-        self.infos.append(info)
-        self.rewards.append(reward)
-
-    def reset(self):
-        self.infos = []
-        self.rewards = []
```

### Comparing `openrl-0.0.5/openrl/envs/vec_env/wrappers/vec_monitor.py` & `openrl-0.0.6/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,50 +16,31 @@
 
 """"""
 from typing import Any, Dict, Optional
 
 from gymnasium.core import ActType
 
 from openrl.envs.vec_env.base_venv import BaseVecEnv
+from openrl.envs.vec_env.vec_info.base_vec_info import BaseVecInfo
 from openrl.envs.vec_env.wrappers.base_wrapper import VecEnvWrapper
-from openrl.envs.vec_env.wrappers.vec_info import NLPVecInfo, VecInfo
 
-registed_vec_info = {
-    "default": VecInfo,
-    "NLPVecInfo": NLPVecInfo,
-}
-
-
-class VecInfoFactory:
-    @staticmethod
-    def get_vec_info_class(vec_info_class, env):
-        if vec_info_class is None or vec_info_class.id is None:
-            return registed_vec_info["default"](env.parallel_env_num, env.agent_num)
-        return registed_vec_info[vec_info_class.id](
-            env.parallel_env_num, env.agent_num, **vec_info_class.args
-        )
-
-    @staticmethod
-    def register(name, vec_info):
-        registed_vec_info[name] = vec_info
 
-
-class VecMonitor(VecEnvWrapper):
-    def __init__(self, vec_info: Any, env: BaseVecEnv):
+class VecMonitorWrapper(VecEnvWrapper):
+    def __init__(self, vec_info: BaseVecInfo, env: BaseVecEnv):
         super().__init__(env)
         self.vec_info = vec_info
 
     @property
     def use_monitor(self):
         return True
 
     def step(self, action: ActType, extra_data: Optional[Dict[str, Any]] = None):
         returns = self.env.step(action, extra_data)
-        self.vec_info.append(reward=returns[1], info=returns[-1])
+        self.vec_info.append(info=returns[-1])
 
         return returns
 
-    def statistics(self):
+    def statistics(self, buffer):  # TODO
         # this function should be called each episode
-        info_dict = self.vec_info.statistics()
+        info_dict = self.vec_info.statistics(buffer)
         self.vec_info.reset()
         return info_dict
```

### Comparing `openrl-0.0.5/openrl/envs/wrappers/base_wrapper.py` & `openrl-0.0.6/openrl/envs/wrappers/base_wrapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,38 +11,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from typing import Any, Dict, Optional
-
 import gymnasium as gym
 
 
 class BaseWrapper(gym.Wrapper):
     def __init__(self, env, reward_class=None) -> None:
         super().__init__(env)
         self.reward_class = reward_class
 
-    def step(self, action, extra_data: Optional[Dict[str, Any]] = None):
-        returns = super().step(action)
-        rewards = returns[1]
-        if self.reward_class is not None and extra_data is not None:
-            extra_data.update({"action": action})
-            extra_data.update({"reward": returns[1]})
-            extra_data.update({"returns": returns})
-            rewards = self.reward_class.get_reward(extra_data)
-
-        return returns[0], rewards, *returns[2:]
-
-    def batch_rewards(self, buffer):
-        if self.reward_class is not None:
-            self.reward_class.batch_rewards(buffer)
+    def step(self, action):
+        return super().step(action)
 
     @property
     def env_name(self):
         if hasattr(self.env, "env_name"):
             return self.env.env_name
         return self.env.unwrapped.spec.id
```

### Comparing `openrl-0.0.5/openrl/envs/wrappers/extra_wrappers.py` & `openrl-0.0.6/openrl/envs/wrappers/extra_wrappers.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/wrappers/multiagent_wrapper.py` & `openrl-0.0.6/openrl/envs/wrappers/multiagent_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/envs/wrappers/util.py` & `openrl-0.0.6/openrl/envs/wrappers/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/__init__.py` & `openrl-0.0.6/openrl/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/base_module.py` & `openrl-0.0.6/openrl/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/common/base_net.py` & `openrl-0.0.6/openrl/modules/common/base_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/common/ppo_net.py` & `openrl-0.0.6/openrl/modules/common/ppo_net.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,31 +81,30 @@
         self.masks = None
 
     def act(
         self,
         observation: Union[np.ndarray, Dict[str, np.ndarray]],
         deterministic: bool = False,
     ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
-        if not self.first_reset:
-            self.reset()
-
         actions, self.rnn_states_actor = self.module.act(
             obs=observation,
             rnn_states_actor=self.rnn_states_actor,
             masks=self.masks,
             available_actions=None,
             deterministic=deterministic,
         )
 
         return actions, self.rnn_states_actor
 
-    def reset(self):
+    def reset(self, env: Optional[gym.Env] = None) -> None:
+        if env is not None:
+            self.env = env
         self.first_reset = False
         self.rnn_states_actor, self.masks = self.module.init_rnn_states(
-            rollout_num=self.cfg.n_rollout_threads,
+            rollout_num=self.env.parallel_env_num,
             agent_num=self.env.agent_num,
             rnn_layers=self.cfg.recurrent_N,
             hidden_size=self.cfg.rnn_hidden_size,
         )
 
     def load_policy(self, path: str) -> None:
         self.module.load_policy(path)
```

### Comparing `openrl-0.0.5/openrl/modules/model_config.py` & `openrl-0.0.6/openrl/modules/model_config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/__init__.py` & `openrl-0.0.6/openrl/modules/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/base_policy_network.py` & `openrl-0.0.6/openrl/modules/networks/base_policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/base_value_network.py` & `openrl-0.0.6/openrl/modules/networks/base_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/policy_network.py` & `openrl-0.0.6/openrl/modules/networks/policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/policy_value_network.py` & `openrl-0.0.6/openrl/modules/networks/policy_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/policy_value_network_gpt.py` & `openrl-0.0.6/openrl/modules/networks/policy_value_network_gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         policy_output, past_model_kwargs = super().get_distribution(
             obs, past_model_kwargs
         )
         actions = policy_output.mode() if deterministic else policy_output.sample()
         action_log_probs = policy_output.log_prob(actions)
 
         return actions.unsqueeze(-1), action_log_probs.unsqueeze(-1), rnn_states
-        # , past_model_kwargs # TODO
+        # TODO: add past_model_kwargs, i.e., past key value.
 
     def eval_actions(
         self, obs, rnn_states, action, masks, available_actions, active_masks=None
     ):
         for key in obs.keys():
             obs[key] = check(obs[key], self.use_half, self.tpdv)
         action = check(action, self.use_half, self.tpdv).squeeze()
```

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/act.py` & `openrl-0.0.6/openrl/modules/networks/utils/act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/attention.py` & `openrl-0.0.6/openrl/modules/networks/utils/attention.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/cnn.py` & `openrl-0.0.6/openrl/modules/networks/utils/cnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/distributed_utils.py` & `openrl-0.0.6/openrl/modules/networks/utils/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/distributions.py` & `openrl-0.0.6/openrl/modules/networks/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/mix.py` & `openrl-0.0.6/openrl/modules/networks/utils/mix.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/mlp.py` & `openrl-0.0.6/openrl/modules/networks/utils/mlp.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/nlp/base_policy.py` & `openrl-0.0.6/openrl/modules/networks/utils/nlp/base_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/nlp/causal_policy.py` & `openrl-0.0.6/openrl/modules/networks/utils/nlp/causal_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/nlp/hf_generation_utils.py` & `openrl-0.0.6/openrl/modules/networks/utils/nlp/hf_generation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/popart.py` & `openrl-0.0.6/openrl/modules/networks/utils/popart.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/rnn.py` & `openrl-0.0.6/openrl/modules/networks/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/utils/transformer_act.py` & `openrl-0.0.6/openrl/modules/networks/utils/transformer_act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/networks/value_network.py` & `openrl-0.0.6/openrl/modules/networks/value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/ppo_module.py` & `openrl-0.0.6/openrl/modules/ppo_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/rl_module.py` & `openrl-0.0.6/openrl/modules/rl_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/utils/__init__.py` & `openrl-0.0.6/openrl/modules/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/utils/util.py` & `openrl-0.0.6/openrl/modules/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/modules/utils/valuenorm.py` & `openrl-0.0.6/openrl/modules/utils/valuenorm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/rewards/nlp_reward.py` & `openrl-0.0.6/openrl/rewards/nlp_reward.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,113 @@
-from typing import Any, Dict
+from typing import Any, Dict, List, Union
 
 import numpy as np
 from gymnasium import Env
 
-from openrl.buffers.normal_buffer import NormalReplayBuffer
-from openrl.envs.nlp.nlp_rewards import IntentAccuracy
+from openrl.envs.nlp.rewards.intent import Intent
+from openrl.envs.nlp.rewards.kl_penalty import KLPenalty
+from openrl.envs.nlp.rewards.meteor import Meteor
 from openrl.rewards.base_reward import BaseReward
 
 
 class NLPReward(BaseReward):
     def __init__(self, env: Env, ref_model: str, intent_model: str):
-        from openrl.envs.nlp.nlp_rewards import KLPenalty
-
         self.rew_infos = []
+        self.env_infos = []
+
+        meteor_config = {
+            "meteor_coeff": 0.5,
+        }
+        self.inner_reward_fn = {
+            "meteor": Meteor(**meteor_config),
+        }
 
-        reward_config = {
-            "model_path": intent_model,
+        kl_config = {
+            "action_space": env.action_space,
+            "ref_model": ref_model,
+        }
+        self.step_rew_funcs = {
+            "kl_pen": KLPenalty(**kl_config),
+        }
+
+        intent_config = {
+            "intent_model": intent_model,
             "intent_coeff": 0.5,
-            "auto_coeff": 0.5,
-            "debug": False,
         }
-        self.inner_reward_fn = [IntentAccuracy(**reward_config)]
-        self.step_rew_funcs = []
         self.batch_rew_funcs = {
-            "kl": KLPenalty(env.action_space, ref_model),
+            "intent_acc": Intent(**intent_config),
         }
 
-    def get_reward(self, data: Dict[str, Any]):
-        rewards = data["reward"].copy()
-        infos = None
+    def step_reward(
+        self, data: Dict[str, Any]
+    ) -> Union[np.ndarray, List[Dict[str, Any]]]:
+        # step reward
+        infos = []
+        rewards = data["rewards"].copy()
 
-        for rew_func in self.step_rew_funcs:
+        for rew_func in self.step_rew_funcs.values():
             new_rew, new_info = rew_func(data)
-            if infos is None:
+            if len(infos) == 0:
                 infos = new_info
             else:
                 for i in range(len(infos)):
                     infos[i].update(new_info[i])
-
             rewards += new_rew
 
+        # collect data for alpha adjustment
         self.rew_infos.append(infos)
 
+        # collect data for batch reward
+        self.env_infos.append(data["infos"])
+
         return rewards, infos
 
-    def batch_rewards(self, buffer: NormalReplayBuffer):
-        """update KL_penalty's alpha coef per episode
+    def batch_rewards(self, buffer) -> Dict[str, Any]:
+        """
+        calculate batch rewards and update KL_penalty's alpha coeff here.
 
         Args:
-            buffer (NormalReplayBuffer): Not used
+            buffer (): buffer.data.rewards is updated here
         """
 
-        infos = dict()
-        if len(self.batch_rew_funcs) > 0:
-            for step in range(buffer.data.actions.shape[0]):
-                obs = buffer.data.all_batch_data("policy_obs", min=step, max=step + 1)
-                actions = buffer.data.all_batch_data("actions", min=step, max=step + 1)
-                action_log_probs = buffer.data.all_batch_data(
-                    "action_log_probs", min=step, max=step + 1
-                )
-
-                data = {
-                    "obs": obs,
-                    "actions": actions,
-                    "action_log_probs": action_log_probs,
-                }
-                for rew_func in self.batch_rew_funcs.values():
-                    new_rew, new_info = rew_func(data)
-                    for key in new_info:
-                        if key not in infos:
-                            infos[key] = [new_info[key]]
-                        else:
-                            infos[key].append(new_info[key])
-                    buffer.data.rewards[step] += new_rew.reshape(
-                        buffer.data.rewards[step].shape
+        # collect batch data
+        done_idx = []
+        data = {"prompt_texts": [], "generated_texts": [], "meta_infos": []}
+
+        for step_infos in self.env_infos:
+            for env_info in step_infos:
+                done = "final_info" in env_info
+                done_idx.append(done)
+                if done:
+                    data["prompt_texts"].append(env_info["final_info"]["prompt_texts"])
+                    data["generated_texts"].append(
+                        env_info["final_info"]["generated_texts"]
                     )
+                    data["meta_infos"].append(env_info["final_info"]["meta_infos"])
+        done_idx = np.array(done_idx)
 
-            for key in infos:
-                infos[key] = np.array(infos[key]).mean()
+        # get batch reward
+        infos = dict()
+        rewards = np.zeros_like(buffer.data.rewards).flatten()
+        for rew_func in self.batch_rew_funcs.values():
+            new_rew, new_info = rew_func(data)
+            if len(infos) == 0:
+                infos = new_info
+            else:
+                infos.update(new_info)
+            rewards[done_idx] += new_rew
+        rewards = rewards.reshape(buffer.data.rewards.shape)
+        buffer.data.rewards += rewards
+
+        # update alpha
+        kl = []
+        for step_infos in self.rew_infos:
+            for env_info in step_infos:
+                kl.append(env_info["kl_div"])
+        kl_div = np.array(kl).mean()
+        self.step_rew_funcs["kl_pen"].update_alpha(kl_div)
 
-            if "kl" in self.batch_rew_funcs:
-                self.batch_rew_funcs["kl"].update_alpha(infos["kl_div"])
+        # reset vec infos
+        self.rew_infos = []
+        self.env_infos = []
 
         return infos
```

### Comparing `openrl-0.0.5/openrl/runners/__init__.py` & `openrl-0.0.6/openrl/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/runners/common/base_agent.py` & `openrl-0.0.6/openrl/runners/common/base_agent.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/runners/common/chat_agent.py` & `openrl-0.0.6/openrl/runners/common/chat_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import io
 import pathlib
 from typing import List, Optional, Type, Union
 
 import torch
 
-
 from openrl.runners.common.base_agent import BaseAgent, SelfAgent
 
 
 class ChatAgent(BaseAgent):
     def __init__(self, model, tokenizer, device=None):
         self.model = model
         self.tokenizer = tokenizer
```

### Comparing `openrl-0.0.5/openrl/runners/common/ppo_agent.py` & `openrl-0.0.6/openrl/runners/common/ppo_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         env: Union[gym.Env, str] = None,
     ):
         self.net.reset()
         if env is not None:
             self._env = env
             self.env_num = env.parallel_env_num
         env.reset(seed=self._cfg.seed)
+        self.net.reset(env)
 
     def save(self, path: Union[str, pathlib.Path, io.BufferedIOBase]) -> None:
         if isinstance(path, str):
             path = pathlib.Path(path)
         path.mkdir(parents=True, exist_ok=True)
         torch.save(self.net.module, path / "module.pt")
 
@@ -172,15 +173,14 @@
             path = path / "module.pt"
 
         assert path.exists(), f"{path} does not exist"
 
         if not torch.cuda.is_available():
             self.net.module = torch.load(path, map_location=torch.device("cpu"))
             self.net.module.device = torch.device("cpu")
-            self.net.module.device = torch.device("cpu")
             for key in self.net.module.models:
                 self.net.module.models[key].tpdv = dict(
                     dtype=torch.float32, device=torch.device("cpu")
                 )
         else:
             self.net.module = torch.load(path)
```

### Comparing `openrl-0.0.5/openrl/supports/__init__.py` & `openrl-0.0.6/openrl/supports/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/supports/opendata/__init__.py` & `openrl-0.0.6/openrl/supports/opendata/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/supports/opendata/utils/__init__.py` & `openrl-0.0.6/openrl/supports/opendata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/supports/opendata/utils/opendata_utils.py` & `openrl-0.0.6/openrl/supports/opendata/utils/opendata_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/supports/opengpu/__init__.py` & `openrl-0.0.6/openrl/supports/opengpu/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/supports/opengpu/gpu_info.py` & `openrl-0.0.6/openrl/supports/opengpu/gpu_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/supports/opengpu/manager.py` & `openrl-0.0.6/openrl/supports/opengpu/manager.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/utils/__init__.py` & `openrl-0.0.6/openrl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/utils/logger.py` & `openrl-0.0.6/openrl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl/utils/util.py` & `openrl-0.0.6/openrl/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/openrl.egg-info/PKG-INFO` & `openrl-0.0.6/openrl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.5
+Version: 0.0.6
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
@@ -18,15 +18,14 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mpe
 Provides-Extra: nlp
 License-File: LICENSE
-License-File: LICENSE.txt
 
 <div align="center">
     <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
@@ -34,29 +33,29 @@
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://codecov.io/gh/OpenRL-Lab/openrl)
 
-[![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 [![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
+[![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
-![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL)
+![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL-Lab)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.5 is updated on April 19, 2023 
+OpenRL-v0.0.6 is updated on April 28, 2023 
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
```

#### html2text {}

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.5 Summary: unified
+Metadata-Version: 2.1 Name: openrl Version: 0.0.6 Summary: unified
 reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
 openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
 URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
 https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
 multi-agent reinforcement-learning-algorithms pytorch machine-learning
 baselines toolbox python data-science gym gymnasium Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Provides-Extra: test Provides-Extra: dev Provides-Extra: mpe Provides-Extra:
-nlp License-File: LICENSE License-File: LICENSE.txt
+nlp License-File: LICENSE
                         [./docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
 openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl) [!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg)](https://github.com/psf/black) [![Hits-of-Code](https://
 hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/
 github/OpenRL-Lab/openrl/view?branch=main) [![codecov](https://codecov.io/gh/
-OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https:
-//codecov.io/gh/OpenRL-Lab/openrl_release) [![Read the Docs](https://
+OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://
+codecov.io/gh/OpenRL-Lab/openrl) [![Documentation Status](https://
+readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
+docs.readthedocs.io/zh/latest/?badge=latest) [![Read the Docs](https://
 img.shields.io/readthedocs/openrl-docs-
 zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-
-docs.readthedocs.io/zh/latest/) [![Documentation Status](https://
-readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
-docs.readthedocs.io/zh/latest/?badge=latest) ![GitHub Org's stars](https://
-img.shields.io/github/stars/OpenRL) [![GitHub stars](https://img.shields.io/
-github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/
-stargazers) [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/
-openrl)](https://github.com/OpenRL-Lab/openrl/network) ![GitHub commit
-activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [!
-[GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https:
-//github.com/OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/
-github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
-pulls) [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/
-openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub
-license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://
-github.com/OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.5 is updated on
-April 19, 2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
-(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
-openrl-docs.readthedocs.io/en/latest/
+docs.readthedocs.io/zh/latest/) ![GitHub Org's stars](https://img.shields.io/
+github/stars/OpenRL-Lab) [![GitHub stars](https://img.shields.io/github/stars/
+OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers) [![GitHub
+forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://
+github.com/OpenRL-Lab/openrl/network) ![GitHub commit activity](https://
+img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
+(https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
+OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
+issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
+[Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
+(https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.6 is updated on April 28,
+2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
+openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
+docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
 ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
 æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
 [Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
```

### Comparing `openrl-0.0.5/openrl.egg-info/SOURCES.txt` & `openrl-0.0.6/openrl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-LICENSE.txt
 README.md
 setup.py
 openrl/__init__.py
 openrl.egg-info/PKG-INFO
 openrl.egg-info/SOURCES.txt
 openrl.egg-info/dependency_links.txt
 openrl.egg-info/entry_points.txt
@@ -40,15 +39,14 @@
 openrl/envs/mpe/rendering.py
 openrl/envs/mpe/scenario.py
 openrl/envs/mpe/scenarios/__init__.py
 openrl/envs/mpe/scenarios/simple_spread.py
 openrl/envs/nlp/__init__.py
 openrl/envs/nlp/daily_dialog_env.py
 openrl/envs/nlp/nlp_env.py
-openrl/envs/nlp/nlp_rewards.py
 openrl/envs/nlp/utils/__init__.py
 openrl/envs/nlp/utils/custom_text_generation_pools.py
 openrl/envs/nlp/utils/distribution.py
 openrl/envs/nlp/utils/evaluation_utils.py
 openrl/envs/nlp/utils/observation.py
 openrl/envs/nlp/utils/sampler.py
 openrl/envs/nlp/utils/text_generation_pool.py
@@ -58,19 +56,22 @@
 openrl/envs/vec_env/async_venv.py
 openrl/envs/vec_env/base_venv.py
 openrl/envs/vec_env/sync_venv.py
 openrl/envs/vec_env/utils/__init__.py
 openrl/envs/vec_env/utils/numpy_utils.py
 openrl/envs/vec_env/utils/share_memory.py
 openrl/envs/vec_env/utils/util.py
+openrl/envs/vec_env/vec_info/__init__.py
+openrl/envs/vec_env/vec_info/base_vec_info.py
+openrl/envs/vec_env/vec_info/nlp_vec_info.py
+openrl/envs/vec_env/vec_info/simple_vec_info.py
 openrl/envs/vec_env/wrappers/__init__.py
 openrl/envs/vec_env/wrappers/base_wrapper.py
 openrl/envs/vec_env/wrappers/reward_wrapper.py
-openrl/envs/vec_env/wrappers/vec_info.py
-openrl/envs/vec_env/wrappers/vec_monitor.py
+openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
 openrl/envs/wrappers/__init__.py
 openrl/envs/wrappers/base_wrapper.py
 openrl/envs/wrappers/extra_wrappers.py
 openrl/envs/wrappers/multiagent_wrapper.py
 openrl/envs/wrappers/util.py
 openrl/modules/__init__.py
 openrl/modules/base_module.py
@@ -105,15 +106,14 @@
 openrl/modules/networks/utils/nlp/hf_generation_utils.py
 openrl/modules/utils/__init__.py
 openrl/modules/utils/util.py
 openrl/modules/utils/valuenorm.py
 openrl/rewards/__init__.py
 openrl/rewards/base_reward.py
 openrl/rewards/nlp_reward.py
-openrl/rewards/register.py
 openrl/runners/__init__.py
 openrl/runners/common/__init__.py
 openrl/runners/common/base_agent.py
 openrl/runners/common/chat_agent.py
 openrl/runners/common/ppo_agent.py
 openrl/supports/__init__.py
 openrl/supports/opendata/__init__.py
```

### Comparing `openrl-0.0.5/setup.py` & `openrl-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "torch",
         "treevalue",
         "rich",
         "wandb",
         "seaborn",
         "jsonargparse",
         "imageio",
-        "python-opencv",
+        "opencv-python",
     ]
 
 
 def get_extra_requires() -> dict:
     req = {
         "test": [
             "pytest",
```

### Comparing `openrl-0.0.5/tests/__init__.py` & `openrl-0.0.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/tests/project/__init__.py` & `openrl-0.0.6/tests/project/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/tests/project/test_version.py` & `openrl-0.0.6/tests/project/test_version.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/tests/test_buffer/__init__.py` & `openrl-0.0.6/tests/test_buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.5/tests/test_buffer/test_buffer.py` & `openrl-0.0.6/tests/test_buffer/test_buffer.py`

 * *Files identical despite different names*

