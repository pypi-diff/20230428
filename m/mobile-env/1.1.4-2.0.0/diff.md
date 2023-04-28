# Comparing `tmp/mobile-env-1.1.4.tar.gz` & `tmp/mobile-env-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobile-env-1.1.4.tar", last modified: Tue Feb  8 11:26:07 2022, max compression
+gzip compressed data, was "mobile-env-2.0.0.tar", last modified: Fri Apr 28 17:28:46 2023, max compression
```

## Comparing `mobile-env-1.1.4.tar` & `mobile-env-2.0.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 11:26:07.559457 mobile-env-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-02-08 11:25:55.000000 mobile-env-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6937 2022-02-08 11:26:07.559457 mobile-env-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6421 2022-02-08 11:25:55.000000 mobile-env-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 11:26:07.551457 mobile-env-1.1.4/mobile_env/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 11:26:07.555457 mobile-env-1.1.4/mobile_env/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/arrival.py
--rw-r--r--   0 runner    (1001) docker     (121)    27168 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4659 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/channels.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3957 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/movement.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/schedules.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 11:26:07.555457 mobile-env-1.1.4/mobile_env/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/handlers/central.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/handlers/multi_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 11:26:07.555457 mobile-env-1.1.4/mobile_env/scenarios/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/scenarios/large.py
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/scenarios/medium.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/scenarios/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/scenarios/small.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 11:26:07.559457 mobile-env-1.1.4/mobile_env/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-02-08 11:25:55.000000 mobile-env-1.1.4/mobile_env/wrappers/multi_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 11:26:07.551457 mobile-env-1.1.4/mobile_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6937 2022-02-08 11:26:07.000000 mobile-env-1.1.4/mobile_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-02-08 11:26:07.000000 mobile-env-1.1.4/mobile_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 11:26:07.000000 mobile-env-1.1.4/mobile_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 11:26:07.000000 mobile-env-1.1.4/mobile_env.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-08 11:26:07.000000 mobile-env-1.1.4/mobile_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-08 11:26:07.000000 mobile-env-1.1.4/mobile_env.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-08 11:26:07.559457 mobile-env-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-08 11:25:55.000000 mobile-env-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 11:26:07.559457 mobile-env-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 11:25:55.000000 mobile-env-1.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-02-08 11:25:55.000000 mobile-env-1.1.4/tests/test_central_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 17:28:36.000000 mobile-env-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-28 17:28:46.061926 mobile-env-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-28 17:28:36.000000 mobile-env-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.057926 mobile-env-2.0.0/mobile_env/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/mobile_env/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/arrival.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28237 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/mobile_env/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/handlers/central.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/handlers/multi_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/mobile_env/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/small.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/mobile_env/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/wrappers/multi_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.057926 mobile-env-2.0.0/mobile_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 17:28:46.061926 mobile-env-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 17:28:36.000000 mobile-env-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:36.000000 mobile-env-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-28 17:28:36.000000 mobile-env-2.0.0/tests/test_central_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-28 17:28:36.000000 mobile-env-2.0.0/tests/test_env_stepping.py
```

### Comparing `mobile-env-1.1.4/LICENSE` & `mobile-env-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mobile-env-1.1.4/PKG-INFO` & `mobile-env-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,73 @@
 Metadata-Version: 2.1
 Name: mobile-env
-Version: 1.1.4
+Version: 2.0.0
 Summary: mobile-env: An Open Environment for Autonomous Coordination in Wireless Mobile Networks
 Home-page: https://github.com/stefanbschneider/mobile-env
 Author: Stefan Schneider, Stefan Werner
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-package.yml/badge.svg)](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-package.yml)
 [![PyPI](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-publish.yml/badge.svg)](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-publish.yml)
 [![Documentation](https://readthedocs.org/projects/mobile-env/badge/?version=latest)](https://mobile-env.readthedocs.io/en/latest/?badge=latest)
+[![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)
 
 
 # mobile-env: An Open Environment for Autonomous Coordination in Mobile Networks
 
-mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks. 
+mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks.
 The environment allows modeling users moving around an area and can connect to one or multiple base stations.
 Using the Gym interface, the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
 The environment is highly configurable and can be easily extended (e.g., regarding users, movement patterns, channel models, etc.).
 
 mobile-env supports multi-agent and centralized reinforcement learning policies. It provides various choices for rewards and observations. mobile-env is also easily extendable, so that anyone may add another channel models (e.g. path loss), movement patterns, utility functions, etc.
 
 As an example, mobile-env can be used to study multi-cell selection in coordinated multipoint.
-Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally. 
-To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates. 
-However, BSs multiplex resources among connected UEs (e.g. schedule physical resource blocks) and, therefore, UEs compete for limited resources (conflicting goals). 
+Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally.
+To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates.
+However, BSs multiplex resources among connected UEs (e.g. schedule physical resource blocks) and, therefore, UEs compete for limited resources (conflicting goals).
 To maximize QoE globally, the policy must recognize that (1) the data rate of any connection is governed by the channel (e.g. SNR) between UE and BS and (2) QoE of single UEs not necessarily grows linearly with increasing data rate.
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/36734964/139288123-7732eff2-24d4-4c25-87fd-ac906f261c93.gif" width="65%"/>
     <br>
     <sup><a href="https://thenounproject.com/search/?q=base+station&i=1286474" target="_blank">Base station icon</a> by Clea Doltz from the Noun Project</sup>
 </p>
 
 **[Try mobile-env: ![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)**
 
 Documentation and API: [ReadTheDocs](https://mobile-env.readthedocs.io/en/latest/)
 
 
+## Citation
+
+
+If you use `mobile-env` in your work, please cite our paper ([author PDF](https://ris.uni-paderborn.de/download/30236/30237/author_version.pdf)):
+
+```
+@inproceedings{schneider2022mobileenv,
+  author = {Schneider, Stefan and Werner, Stefan and Khalili, Ramin and Hecker, Artur and Karl, Holger},
+  title = {mobile-env: An Open Platform for Reinforcement Learning in Wireless Mobile Networks},
+  booktitle={Network Operations and Management Symposium (NOMS)},
+  year = {2022},
+  publisher = {IEEE/IFIP},
+}
+```
+
+mobile-env is based on the underlying environment using in [DeepCoMP](https://github.com/CN-UPB/DeepCoMP), which is a combination of reinforcement learning approaches for dynamic multi-cell selection.
+mobile-env provides this underlying environment as open, stand-alone environment.
+
+
 ## Installation
 
 ### From PyPI (Recommended)
 
 The simplest option is to install the latest release of `mobile-env` from [PyPI](https://pypi.org/project/mobile-env/) using pip:
 
 ```bash
@@ -69,34 +88,35 @@
 
 If you want to run tests or examples, also install the requirements in `tests`.
 For dependencies for building docs, install the requirements in `docs`.
 
 ## Example Usage
 
 ```python
-import gym
+import gymnasium as gym
 import mobile_env
 
 env = gym.make("mobile-medium-central-v0")
-obs = env.reset()
+obs, info = env.reset()
 done = False
 
 while not done:
     action = ... # Your agent code here
-    obs, reward, done, info = env.step(action)
+    obs, reward, terminated, truncated, info = env.step(action)
+    done = terminated or truncated
     env.render()
 ```
 
 ## Customization
 
-mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions. 
+mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions.
 For example, replacing the default [Okumura–Hata](https://en.wikipedia.org/wiki/Hata_model) channel model by a (simplified) path loss model can be as easy as this:
 
 ```python
-import gym
+import gymnasium as gym
 import numpy as np
 from mobile_env.core.base import MComCore
 from mobile_env.core.channel import Channel
 
 
 class PathLoss(Channel):
     def __init__(self, gamma, **kwargs):
@@ -107,57 +127,35 @@
     def power_loss(self, bs, ue):
         """Computes power loss between BS and UE."""
         dist = bs.point.distance(ue.point)
         loss = 10 * self.gamma * np.log10(4 * np.pi * dist * bs.frequency)
         return loss
 
 
-# replace default channel model in configuration 
+# replace default channel model in configuration
 config = MComCore.default_config()
 config['channel'] = PathLoss
 
 # pass init parameters to custom channel class!
 config['channel_params'].update({'gamma': 2.0})
 
 # create environment with custom channel model
 env = gym.make('mobile-small-central-v0', config=config)
 # ...
 ```
 
+## Projects Using mobile-env
 
-## About `mobile-env`
-
-
-If you use mobile-env in your work, please cite with:
-
-```
-@misc{mobile-env,
-  author = {Schneider, Stefan and Werner, Stefan and Karl, Holger},
-  title = {An Open Environment for Autonomous Coordination in Mobile Networks},
-  year = {2021},
-  publisher = {GitHub},
-  journal = {GitHub Repository},
-  howpublished = {\url{https://github.com/stefanbschneider/mobile-env}},
-}
-```
-
-mobile-env is based on [DeepCoMP](https://github.com/CN-UPB/DeepCoMP), providing the underlying environment as open, stand-alone platform to be used by others.
-
-
-List of repositories, publications, or preprints using `mobile-env` (please open a pull request to add missing entries):
-
-* [DeepCoMP](https://github.com/CN-UPB/DeepCoMP)
+If you are using `movile-env`, please let us know and we are happy to link to your project from the readme. You can also open a pull request yourself.
 
+* [Mohammadreza Kouchaki and Vuk Marojevic, "Actor-Critic Network for O-RAN Resource Allocation: xApp Design, Deployment, and Analysis", 2022](https://arxiv.org/abs/2210.04604)
+* [Stefan Schneider, Ramin Khalili, Artur Hecker, Holger Karl, "DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)", 2021](https://github.com/CN-UPB/DeepCoMP)
 
 
 ## Contributing
 
 Development: [@stefanbschneider](https://github.com/stefanbschneider) and [@stwerner97](https://github.com/stwerner97/)
 
 
-We happy if you find `mobile-env` useful. If you have feedback or want to report bugs, feel free to [open an issue](https://github.com/stefanbschneider/mobile-env/issues/new).
+We happy if you find `mobile-env` useful. If you have feedback or want to report bugs, feel free to [open an issue](https://github.com/stefanbschneider/mobile-env/issues/new). Also, we are happy to link to your projects if you use `mobile-env`.
 
 We also welcome contributions: Whether you implement a new channel model, fix a bug, or just make a minor addition elsewhere, feel free to open a pull request!
-
-
-
-
```

### Comparing `mobile-env-1.1.4/README.md` & `mobile-env-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,59 @@
 [![CI](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-package.yml/badge.svg)](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-package.yml)
 [![PyPI](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-publish.yml/badge.svg)](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-publish.yml)
 [![Documentation](https://readthedocs.org/projects/mobile-env/badge/?version=latest)](https://mobile-env.readthedocs.io/en/latest/?badge=latest)
+[![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)
 
 
 # mobile-env: An Open Environment for Autonomous Coordination in Mobile Networks
 
-mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks. 
+mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks.
 The environment allows modeling users moving around an area and can connect to one or multiple base stations.
 Using the Gym interface, the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
 The environment is highly configurable and can be easily extended (e.g., regarding users, movement patterns, channel models, etc.).
 
 mobile-env supports multi-agent and centralized reinforcement learning policies. It provides various choices for rewards and observations. mobile-env is also easily extendable, so that anyone may add another channel models (e.g. path loss), movement patterns, utility functions, etc.
 
 As an example, mobile-env can be used to study multi-cell selection in coordinated multipoint.
-Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally. 
-To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates. 
-However, BSs multiplex resources among connected UEs (e.g. schedule physical resource blocks) and, therefore, UEs compete for limited resources (conflicting goals). 
+Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally.
+To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates.
+However, BSs multiplex resources among connected UEs (e.g. schedule physical resource blocks) and, therefore, UEs compete for limited resources (conflicting goals).
 To maximize QoE globally, the policy must recognize that (1) the data rate of any connection is governed by the channel (e.g. SNR) between UE and BS and (2) QoE of single UEs not necessarily grows linearly with increasing data rate.
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/36734964/139288123-7732eff2-24d4-4c25-87fd-ac906f261c93.gif" width="65%"/>
     <br>
     <sup><a href="https://thenounproject.com/search/?q=base+station&i=1286474" target="_blank">Base station icon</a> by Clea Doltz from the Noun Project</sup>
 </p>
 
 **[Try mobile-env: ![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)**
 
 Documentation and API: [ReadTheDocs](https://mobile-env.readthedocs.io/en/latest/)
 
 
+## Citation
+
+
+If you use `mobile-env` in your work, please cite our paper ([author PDF](https://ris.uni-paderborn.de/download/30236/30237/author_version.pdf)):
+
+```
+@inproceedings{schneider2022mobileenv,
+  author = {Schneider, Stefan and Werner, Stefan and Khalili, Ramin and Hecker, Artur and Karl, Holger},
+  title = {mobile-env: An Open Platform for Reinforcement Learning in Wireless Mobile Networks},
+  booktitle={Network Operations and Management Symposium (NOMS)},
+  year = {2022},
+  publisher = {IEEE/IFIP},
+}
+```
+
+mobile-env is based on the underlying environment using in [DeepCoMP](https://github.com/CN-UPB/DeepCoMP), which is a combination of reinforcement learning approaches for dynamic multi-cell selection.
+mobile-env provides this underlying environment as open, stand-alone environment.
+
+
 ## Installation
 
 ### From PyPI (Recommended)
 
 The simplest option is to install the latest release of `mobile-env` from [PyPI](https://pypi.org/project/mobile-env/) using pip:
 
 ```bash
@@ -54,34 +74,35 @@
 
 If you want to run tests or examples, also install the requirements in `tests`.
 For dependencies for building docs, install the requirements in `docs`.
 
 ## Example Usage
 
 ```python
-import gym
+import gymnasium as gym
 import mobile_env
 
 env = gym.make("mobile-medium-central-v0")
-obs = env.reset()
+obs, info = env.reset()
 done = False
 
 while not done:
     action = ... # Your agent code here
-    obs, reward, done, info = env.step(action)
+    obs, reward, terminated, truncated, info = env.step(action)
+    done = terminated or truncated
     env.render()
 ```
 
 ## Customization
 
-mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions. 
+mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions.
 For example, replacing the default [Okumura–Hata](https://en.wikipedia.org/wiki/Hata_model) channel model by a (simplified) path loss model can be as easy as this:
 
 ```python
-import gym
+import gymnasium as gym
 import numpy as np
 from mobile_env.core.base import MComCore
 from mobile_env.core.channel import Channel
 
 
 class PathLoss(Channel):
     def __init__(self, gamma, **kwargs):
@@ -92,55 +113,35 @@
     def power_loss(self, bs, ue):
         """Computes power loss between BS and UE."""
         dist = bs.point.distance(ue.point)
         loss = 10 * self.gamma * np.log10(4 * np.pi * dist * bs.frequency)
         return loss
 
 
-# replace default channel model in configuration 
+# replace default channel model in configuration
 config = MComCore.default_config()
 config['channel'] = PathLoss
 
 # pass init parameters to custom channel class!
 config['channel_params'].update({'gamma': 2.0})
 
 # create environment with custom channel model
 env = gym.make('mobile-small-central-v0', config=config)
 # ...
 ```
 
+## Projects Using mobile-env
 
-## About `mobile-env`
-
-
-If you use mobile-env in your work, please cite with:
-
-```
-@misc{mobile-env,
-  author = {Schneider, Stefan and Werner, Stefan and Karl, Holger},
-  title = {An Open Environment for Autonomous Coordination in Mobile Networks},
-  year = {2021},
-  publisher = {GitHub},
-  journal = {GitHub Repository},
-  howpublished = {\url{https://github.com/stefanbschneider/mobile-env}},
-}
-```
-
-mobile-env is based on [DeepCoMP](https://github.com/CN-UPB/DeepCoMP), providing the underlying environment as open, stand-alone platform to be used by others.
-
-
-List of repositories, publications, or preprints using `mobile-env` (please open a pull request to add missing entries):
-
-* [DeepCoMP](https://github.com/CN-UPB/DeepCoMP)
+If you are using `movile-env`, please let us know and we are happy to link to your project from the readme. You can also open a pull request yourself.
 
+* [Mohammadreza Kouchaki and Vuk Marojevic, "Actor-Critic Network for O-RAN Resource Allocation: xApp Design, Deployment, and Analysis", 2022](https://arxiv.org/abs/2210.04604)
+* [Stefan Schneider, Ramin Khalili, Artur Hecker, Holger Karl, "DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)", 2021](https://github.com/CN-UPB/DeepCoMP)
 
 
 ## Contributing
 
 Development: [@stefanbschneider](https://github.com/stefanbschneider) and [@stwerner97](https://github.com/stwerner97/)
 
 
-We happy if you find `mobile-env` useful. If you have feedback or want to report bugs, feel free to [open an issue](https://github.com/stefanbschneider/mobile-env/issues/new).
+We happy if you find `mobile-env` useful. If you have feedback or want to report bugs, feel free to [open an issue](https://github.com/stefanbschneider/mobile-env/issues/new). Also, we are happy to link to your projects if you use `mobile-env`.
 
 We also welcome contributions: Whether you implement a new channel model, fix a bug, or just make a minor addition elsewhere, feel free to open a pull request!
-
-
```

### Comparing `mobile-env-1.1.4/mobile_env/core/arrival.py` & `mobile-env-2.0.0/mobile_env/core/arrival.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 import numpy as np
 
 from mobile_env.core.entities import UserEquipment
 
 
 class Arrival:
-    def __init__(
-        self, ep_time: int, seed: int, reset_rng_episode: bool, **kwargs
-    ):
+    def __init__(self, ep_time: int, seed: int, reset_rng_episode: bool, **kwargs):
         self.ep_time = ep_time
         self.seed = seed
         self.reset_rng_episode = reset_rng_episode
         # RNG for arrival and departure times of UEs
         self.rng = None
 
     def reset(self) -> None:
```

### Comparing `mobile-env-1.1.4/mobile_env/core/base.py` & `mobile-env-2.0.0/mobile_env/core/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import string
-from typing import List, Tuple, Dict, Set
 from collections import Counter, defaultdict
+from typing import Dict, List, Set, Tuple
 
-import gym
-import pygame
-import numpy as np
-import matplotlib.pyplot as plt
+import gymnasium as gym
 import matplotlib.patheffects as pe
-from pygame import Surface
+import matplotlib.pyplot as plt
+import numpy as np
+import pygame
 from matplotlib import cm
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
+from pygame import Surface
 
 from mobile_env.core import metrics
-from mobile_env.handlers.central import MComCentralHandler
-from mobile_env.core.util import BS_SYMBOL
-from mobile_env.core.logging import Monitor
 from mobile_env.core.arrival import NoDeparture
 from mobile_env.core.channels import OkumuraHata
-from mobile_env.core.schedules import ResourceFair
-from mobile_env.core.utilities import BoundedLogUtility
 from mobile_env.core.entities import BaseStation, UserEquipment
+from mobile_env.core.logging import Monitor
 from mobile_env.core.movement import RandomWaypointMovement
-from mobile_env.core.util import deep_dict_merge
+from mobile_env.core.schedules import ResourceFair
+from mobile_env.core.util import BS_SYMBOL, deep_dict_merge
+from mobile_env.core.utilities import BoundedLogUtility
+from mobile_env.handlers.central import MComCentralHandler
 
 
 class MComCore(gym.Env):
     NOOP_ACTION = 0
+    metadata = {"render_modes": ["rgb_array", "human"]}
 
-    def __init__(self, stations, users, config={}):
+    def __init__(self, stations, users, config={}, render_mode=None):
         super().__init__()
+
+        self.render_mode = render_mode
+        assert render_mode in self.metadata["render_modes"] + [None]
+
         # set unspecified parameters to default configuration
         config = deep_dict_merge(self.default_config(), config)
         config = self.seeding(config)
 
         self.width, self.height = config["width"], config["height"]
         self.seed = config["seed"]
         self.reset_rng_episode = config["reset_rng_episode"]
@@ -154,36 +158,52 @@
             }
         )
 
         return config
 
     @classmethod
     def seeding(cls, config):
+        """Return config with updated and rotated seeds."""
+
         seed = config["seed"]
         keys = [
             "arrival_params",
             "channel_params",
             "scheduler_params",
             "movement_params",
             "utility_params",
         ]
         for num, key in enumerate(keys):
+            if key not in config:
+                config[key] = {}
             config[key]["seed"] = seed + num + 1
 
         return config
 
-    def reset(self):
-        """Reset environment to starting state."""
+    def reset(self, *, seed=None, options=None):
+        """Reset env to starting state. Return the initial obs and info."""
+        super().reset(seed=seed)
+
         # reset time
         self.time = 0.0
 
+        # set seed
+        if seed is not None:
+            self.seeding({"seed": seed})
+
         # initialize RNG or reset (if necessary on episode end)
         if self.reset_rng_episode or self.rng is None:
             self.rng = np.random.default_rng(self.seed)
 
+        # extra options currently not supported
+        if options is not None:
+            raise NotImplementedError(
+                "Passing extra options on env.reset() is not supported."
+            )
+
         # reset state kept by arrival pattern, channel, scheduler, etc.
         self.arrival.reset()
         self.channel.reset()
         self.scheduler.reset()
         self.movement.reset()
         self.utility.reset()
 
@@ -214,15 +234,20 @@
         self.monitor.reset()
 
         # check if handler is applicable to mobile scenario
         # NOTE: e.g. fails if the central handler is used,
         # although the number of UEs changes
         self.handler.check(self)
 
-        return self.handler.observation(self)
+        # info
+        info = self.handler.info(self)
+        # store latest monitored results in `info` dictionary
+        info = {**info, **self.monitor.info()}
+
+        return self.handler.observation(self), info
 
     def apply_action(self, action: int, ue: UserEquipment) -> None:
         """Connect or disconnect `ue` to/from basestation `action`."""
         # do not apply update to connections if NOOP_ACTION is selected
         if action == self.NOOP_ACTION or ue not in self.active:
             return
 
@@ -251,15 +276,15 @@
             bs: set(ue for ue in ues if self.check_connectivity(bs, ue))
             for bs, ues in self.connections.items()
         }
         self.connections.clear()
         self.connections.update(connections)
 
     def step(self, actions: Dict[int, int]):
-        assert not self.done, "step() called on already terminated episode"
+        assert not self.time_is_up, "step() called on terminated episode"
 
         # apply handler to transform actions to expected shape
         actions = self.handler.action(self, actions)
 
         # release established connections that moved e.g. out-of-range
         self.update_connections()
 
@@ -317,35 +342,40 @@
             drates = self.station_allocation(bs)
             self.datarates.update(drates)
 
         # update internal time of environment
         self.time += 1
 
         # check whether episode is done & close the environment
-        if self.done and self.window:
+        if self.time_is_up and self.window:
             self.close()
 
         # do not invoke next step on policies before at least one UE is active
-        if not self.active and not self.done:
+        if not self.active and not self.time_is_up:
             return self.step({})
 
         # compute observations for next step and information
         # methods are defined by handler according to strategy pattern
         # NOTE: compute observations after proceeding in time (may skip ahead)
         observation = self.handler.observation(self)
         info = self.handler.info(self)
 
         # store latest monitored results in `info` dictionary
         info = {**info, **self.monitor.info()}
 
-        return observation, rewards, self.done, info
+        # there is not natural episode termination, just limited time
+        # terminated is always False and truncated is True once time is up
+        terminated = False
+        truncated = self.time_is_up
+
+        return observation, rewards, terminated, truncated, info
 
     @property
-    def done(self):
-        """Episode is done after max. time steps or once last UE departed."""
+    def time_is_up(self):
+        """Return true after max. time steps or once last UE departed."""
         return self.time >= min(self.EP_MAX_TIME, self.max_departure)
 
     def macro_datarates(self, datarates):
         """Compute aggregated UE data rates given all its connections."""
         ue_datarates = Counter()
         for (bs, ue), datarate in self.datarates.items():
             ue_datarates.update({ue: datarate})
@@ -482,15 +512,17 @@
         # define dummy observations for non-active UEs
         idle_ues = set(self.users.values()) - set(self.active)
         obs = {ue.ue_id: dummy_features(ue) for ue in idle_ues}
         obs.update({ue.ue_id: ue_features(ue) for ue in self.active})
 
         return obs
 
-    def render(self, mode="human") -> None:
+    def render(self) -> None:
+        mode = self.render_mode
+
         # do not continue rendering once environment has been closed
         if self.closed:
             return
 
         # calculate isoline contours for BSs' connectivity range
         if self.conn_isolines is None:
             self.conn_isolines = self.bs_isolines(0.0)
@@ -600,17 +632,15 @@
                 ue.point.x,
                 ue.point.y,
                 s=200,
                 zorder=2,
                 color=color,
                 marker="o",
             )
-            ax.annotate(
-                ue.ue_id, xy=(ue.point.x, ue.point.y), ha="center", va="center"
-            )
+            ax.annotate(ue.ue_id, xy=(ue.point.x, ue.point.y), ha="center", va="center")
 
         for bs in self.stations.values():
             # plot BS symbol and annonate by its BS ID
             ax.plot(
                 bs.point.x,
                 bs.point.y,
                 marker=BS_SYMBOL,
```

### Comparing `mobile-env-1.1.4/mobile_env/core/channels.py` & `mobile-env-2.0.0/mobile_env/core/channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Dict, Tuple
 from abc import abstractmethod
+from typing import Dict, Tuple
 
 import numpy as np
 
 from mobile_env.core.entities import BaseStation, UserEquipment
 
-
 EPSILON = 1e-16
 
 
 class Channel:
     def __init__(self, **kwargs):
         pass
 
@@ -131,16 +130,13 @@
 
         ch = (
             0.8
             + (1.1 * np.log10(bs.frequency) - 0.7) * ue.height
             - 1.56 * np.log10(bs.frequency)
         )
         tmp_1 = (
-            69.55
-            - ch
-            + 26.16 * np.log10(bs.frequency)
-            - 13.82 * np.log10(bs.height)
+            69.55 - ch + 26.16 * np.log10(bs.frequency) - 13.82 * np.log10(bs.height)
         )
         tmp_2 = 44.9 - 6.55 * np.log10(bs.height)
 
         # add small epsilon to avoid log(0) if distance = 0
         return tmp_1 + tmp_2 * np.log10(distance + EPSILON)
```

### Comparing `mobile-env-1.1.4/mobile_env/core/entities.py` & `mobile-env-2.0.0/mobile_env/core/entities.py`

 * *Files identical despite different names*

### Comparing `mobile-env-1.1.4/mobile_env/core/logging.py` & `mobile-env-2.0.0/mobile_env/core/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from typing import Dict
 
 import pandas as pd
 
 
 class Monitor:
     def __init__(
-        self,
-        scalar_metrics: Dict,
-        ue_metrics: Dict,
-        bs_metrics: Dict,
-        **kwargs
+        self, scalar_metrics: Dict, ue_metrics: Dict, bs_metrics: Dict, **kwargs
     ):
 
         self.scalar_metrics: Dict = scalar_metrics
         self.ue_metrics: Dict = ue_metrics
         self.bs_metrics: Dict = bs_metrics
 
         self.scalar_results: Dict = None
@@ -28,38 +24,33 @@
         self.bs_results = {name: [] for name in self.bs_metrics}
 
     def update(self, simulation):
         """Evaluate and update metrics given the simulation state."""
 
         # evaluate scalar, ue, bs metrics by passing the simulation state
         scalar_updates = {
-            name: metric(simulation)
-            for name, metric in self.scalar_metrics.items()
+            name: metric(simulation) for name, metric in self.scalar_metrics.items()
         }
         ue_updates = {
-            name: metric(simulation)
-            for name, metric in self.ue_metrics.items()
+            name: metric(simulation) for name, metric in self.ue_metrics.items()
         }
         bs_updates = {
-            name: metric(simulation)
-            for name, metric in self.bs_metrics.items()
+            name: metric(simulation) for name, metric in self.bs_metrics.items()
         }
 
         # update results by appending the metrics' return values
         self.scalar_results = {
             name: self.scalar_results[name] + [scalar_updates[name]]
             for name in self.scalar_metrics
         }
         self.ue_results = {
-            name: self.ue_results[name] + [ue_updates[name]]
-            for name in self.ue_metrics
+            name: self.ue_results[name] + [ue_updates[name]] for name in self.ue_metrics
         }
         self.bs_results = {
-            name: self.bs_results[name] + [bs_updates[name]]
-            for name in self.bs_metrics
+            name: self.bs_results[name] + [bs_updates[name]] for name in self.bs_metrics
         }
 
     def load_results(self):
         """Outputs results of tracked metrics as data frames."""
         # load scalar results with index (metric; time)
         scalar_results = pd.DataFrame(self.scalar_results)
         scalar_results.index.names = ["Time Step"]
@@ -71,43 +62,38 @@
             for ue_id in set().union(*entries)
         }
         ue_results = pd.DataFrame(ue_results).transpose()
         ue_results.index.names = ["Metric", "UE ID"]
         # change data frame format to align time axis along rows
         ue_results = ue_results.stack()
         ue_results.index.names = ["Metric", "UE ID", "Time Step"]
-        ue_results = ue_results.reorder_levels(
-            ["Time Step", "UE ID", "Metric"]
-        )
+        ue_results = ue_results.reorder_levels(["Time Step", "UE ID", "Metric"])
         ue_results = ue_results.unstack()
 
         # load BS results with index (metric, BS ID; time)
         bs_results = {
             (metric, bs_id): [values.get(bs_id) for values in entries]
             for metric, entries in self.bs_results.items()
             for bs_id in set().union(*entries)
         }
         bs_results = pd.DataFrame(bs_results).transpose()
         bs_results.index.names = ["Metric", "BS ID"]
         # change data frame format to align time axis along rows
         bs_results = bs_results.stack()
         bs_results.index.names = ["Metric", "BS ID", "Time Step"]
-        bs_results = bs_results.reorder_levels(
-            ["Time Step", "BS ID", "Metric"]
-        )
+        bs_results = bs_results.reorder_levels(["Time Step", "BS ID", "Metric"])
         bs_results = bs_results.unstack()
 
         return scalar_results, ue_results, bs_results
 
     def info(self):
         """Outputs the latest results as a dictionary."""
-        scalar_info = {
-            name: values[-1] for name, values in self.scalar_results.items()
-        }
-        ue_info = {
-            name: values[-1] for name, values in self.ue_results.items()
-        }
-        bs_info = {
-            name: values[-1] for name, values in self.bs_results.items()
-        }
+
+        # Return empty infos if there are no scalar results.
+        if any(len(results) == 0 for results in self.scalar_results.values()):
+            return {}
+
+        scalar_info = {name: values[-1] for name, values in self.scalar_results.items()}
+        ue_info = {name: values[-1] for name, values in self.ue_results.items()}
+        bs_info = {name: values[-1] for name, values in self.bs_results.items()}
 
         return {**scalar_info, **ue_info, **bs_info}
```

### Comparing `mobile-env-1.1.4/mobile_env/core/metrics.py` & `mobile-env-2.0.0/mobile_env/core/metrics.py`

 * *Files identical despite different names*

### Comparing `mobile-env-1.1.4/mobile_env/core/movement.py` & `mobile-env-2.0.0/mobile_env/core/movement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-from typing import Dict, Tuple
 from abc import abstractmethod
+from typing import Dict, Tuple
 
 import numpy as np
 
 from mobile_env.core.entities import UserEquipment
 
 
 class Movement:
     def __init__(
-        self,
-        width: float,
-        height: float,
-        seed: int,
-        reset_rng_episode: str,
-        **kwargs
+        self, width: float, height: float, seed: int, reset_rng_episode: str, **kwargs
     ):
 
         self.width, self.height = width, height
         self.reset_rng_episode = reset_rng_episode
 
         # RNG for movement and initial positions of UEs
         self.seed = seed
```

### Comparing `mobile-env-1.1.4/mobile_env/core/schedules.py` & `mobile-env-2.0.0/mobile_env/core/schedules.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import List
 from abc import abstractmethod
+from typing import List
 
 from mobile_env.core.entities import BaseStation
 
 
 class Scheduler:
     def __init__(self, **kwargs):
         pass
```

### Comparing `mobile-env-1.1.4/mobile_env/core/util.py` & `mobile-env-2.0.0/mobile_env/core/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 
-import svgpath2mpl
 import matplotlib
+import svgpath2mpl
 
 BS_SYMBOL = (
     "M31.5,19c0-4.1-3.4-7.5-7.5-7.5s-7.5,3.4-7.5,7.5c0,2.9,1.6,5.4,4,"
     "6.7l0.9-1.8c-1.7-0.9-2.9-2.8-2.9-4.9c0-3,2.5-5.5,5.5-5.5s5.5,2.5,"
     "5.5,5.5c0,2.1-1.2,3.9-2.9,4.9l0.9,1.8C29.9,24.4,31.5,21.9,31.5,19"
     "zM37,19c0-7.2-5.8-13-13-13s-13,5.8-13,13c0,5.1,2.9,9.4,7.1,11.6l0"
     ".9-1.8c-3.6-1.8-6-5.5-6-9.8c0-6.1,4.9-11,11-11s11,4.9,11,11c0,4.3"
@@ -30,12 +30,12 @@
 
 def deep_dict_merge(dest: Dict, source: Dict):
     """Merge dictionaries recursively (i.e. deep merge)."""
     for key, value in source.items():
         if isinstance(value, dict):
             # get node or create one
             node = dest.setdefault(key, {})
-            deep_dict_merge(value, node)
+            deep_dict_merge(node, value)
         else:
             dest[key] = value
 
     return dest
```

### Comparing `mobile-env-1.1.4/mobile_env/core/utilities.py` & `mobile-env-2.0.0/mobile_env/core/utilities.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Dict, Tuple
 from abc import abstractmethod
+from typing import Dict, Tuple
 
 import numpy as np
 
 
 class Utility:
     def __init__(self, **kwargs):
         pass
```

### Comparing `mobile-env-1.1.4/mobile_env/handlers/central.py` & `mobile-env-2.0.0/mobile_env/handlers/central.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Tuple
 
 import numpy as np
-from gym import spaces
+from gymnasium import spaces
 
 from mobile_env.handlers.handler import Handler
 
 
 class MComCentralHandler(Handler):
     features = ["connections", "snrs", "utility"]
```

### Comparing `mobile-env-1.1.4/mobile_env/handlers/handler.py` & `mobile-env-2.0.0/mobile_env/handlers/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 from typing import Dict
 
-from gym.spaces.space import Space
+from gymnasium.spaces.space import Space
 
 
 class Handler:
     """Defines Gym interface methods called by core simulation."""
 
     @classmethod
     @abc.abstractmethod
```

### Comparing `mobile-env-1.1.4/mobile_env/handlers/multi_agent.py` & `mobile-env-2.0.0/mobile_env/handlers/multi_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict
 
-import gym
+import gymnasium as gym
 import numpy as np
-from gym import spaces
 
 from mobile_env.handlers.handler import Handler
 
 
 class MComMAHandler(Handler):
     features = [
         "connections",
@@ -17,31 +16,31 @@
     ]
 
     @classmethod
     def ue_obs_size(cls, env) -> int:
         return sum(env.feature_sizes[ftr] for ftr in cls.features)
 
     @classmethod
-    def action_space(cls, env) -> spaces.Dict:
-        return spaces.Dict(
+    def action_space(cls, env) -> gym.spaces.Dict:
+        return gym.spaces.Dict(
             {
                 ue.ue_id: gym.spaces.Discrete(env.NUM_STATIONS + 1)
                 for ue in env.users.values()
             }
         )
 
     @classmethod
-    def observation_space(cls, env) -> spaces.Dict:
+    def observation_space(cls, env) -> gym.spaces.Dict:
         size = cls.ue_obs_size(env)
         space = {
-            ue_id: spaces.Box(low=-1, high=1, shape=(size,), dtype=np.float32)
+            ue_id: gym.spaces.Box(low=-1, high=1, shape=(size,), dtype=np.float32)
             for ue_id in env.users
         }
 
-        return spaces.Dict(space)
+        return gym.spaces.Dict(space)
 
     @classmethod
     def reward(cls, env):
         """UE's reward is their utility and the avg. utility of nearby BSs."""
         # compute average utility of UEs for each BS
         # set to lower bound if no UEs are connected
         bs_utilities = env.station_utilities()
@@ -67,28 +66,25 @@
     @classmethod
     def observation(cls, env) -> Dict[int, np.ndarray]:
         """Select features for MA setting & flatten each UE's features."""
 
         # get features for currently active UEs
         active = set([ue.ue_id for ue in env.active if not env.done])
         features = env.features()
-        features = {
-            ue_id: obs for ue_id, obs in features.items() if ue_id in active
-        }
+        features = {ue_id: obs for ue_id, obs in features.items() if ue_id in active}
 
         # select observations for multi-agent setting from base feature set
         obs = {
             ue_id: [obs_dict[key] for key in cls.features]
             for ue_id, obs_dict in features.items()
         }
 
         # flatten each UE's Dict observation to vector representation
         obs = {
-            ue_id: np.concatenate([o for o in ue_obs])
-            for ue_id, ue_obs in obs.items()
+            ue_id: np.concatenate([o for o in ue_obs]) for ue_id, ue_obs in obs.items()
         }
         return obs
 
     @classmethod
     def action(cls, env, action: Dict[int, int]):
         """Base environment by default expects action dictionary."""
         return action
```

### Comparing `mobile-env-1.1.4/mobile_env/scenarios/large.py` & `mobile-env-2.0.0/mobile_env/scenarios/large.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from mobile_env.core.base import MComCore
 from mobile_env.core.entities import BaseStation, UserEquipment
 from mobile_env.core.util import deep_dict_merge
 
 
 class MComLarge(MComCore):
-    def __init__(self, config={}):
+    def __init__(self, config={}, render_mode=None):
         # set unspecified parameters to default configuration
         config = deep_dict_merge(self.default_config(), config)
 
         config.update({"width": 300, "height": 300})
         stations = [
             (50, 100),
             (60, 210),
@@ -27,12 +27,10 @@
         stations = [(x, y) for x, y in stations]
         stations = [
             BaseStation(bs_id, pos, **config["bs"])
             for bs_id, pos in enumerate(stations)
         ]
 
         num_ues = 30
-        ues = [
-            UserEquipment(ue_id, **config["ue"]) for ue_id in range(num_ues)
-        ]
+        ues = [UserEquipment(ue_id, **config["ue"]) for ue_id in range(num_ues)]
 
-        super().__init__(stations, ues, config)
+        super().__init__(stations, ues, config, render_mode)
```

### Comparing `mobile-env-1.1.4/mobile_env/scenarios/medium.py` & `mobile-env-2.0.0/mobile_env/scenarios/small.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 from mobile_env.core.base import MComCore
 from mobile_env.core.entities import BaseStation, UserEquipment
 from mobile_env.core.util import deep_dict_merge
 
 
-class MComMedium(MComCore):
-    def __init__(self, config={}):
+class MComSmall(MComCore):
+    def __init__(self, config={}, render_mode=None):
         # set unspecified parameters to default configuration
         config = deep_dict_merge(self.default_config(), config)
-        config["width"], config["height"] = 200, 300
 
-        stations = [
-            (95, 240),
-            (100, 140),
-            (105, 60),
-            (35, 200),
-            (40, 95),
-            (165, 220),
-            (160, 110),
-        ]
-        stations = [(x, y) for x, y in stations]
+        station_pos = [(110, 130), (65, 80), (120, 30)]
         stations = [
             BaseStation(bs_id, pos, **config["bs"])
-            for bs_id, pos in enumerate(stations)
-        ]
-
-        num_ues = 15
-        ues = [
-            UserEquipment(ue_id, **config["ue"]) for ue_id in range(num_ues)
+            for bs_id, pos in enumerate(station_pos)
         ]
+        num_ues = 5
+        ues = [UserEquipment(ue_id, **config["ue"]) for ue_id in range(num_ues)]
 
-        super().__init__(stations, ues, config)
+        super().__init__(stations, ues, config, render_mode)
```

### Comparing `mobile-env-1.1.4/mobile_env/scenarios/registry.py` & `mobile-env-2.0.0/mobile_env/scenarios/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import itertools
 
-import gym
+import gymnasium as gym
 
-from mobile_env.scenarios.small import MComSmall
-from mobile_env.scenarios.medium import MComMedium
-from mobile_env.scenarios.large import MComLarge
-from mobile_env.handlers.multi_agent import MComMAHandler
 from mobile_env.handlers.central import MComCentralHandler
-
+from mobile_env.handlers.multi_agent import MComMAHandler
+from mobile_env.scenarios.large import MComLarge
+from mobile_env.scenarios.medium import MComMedium
+from mobile_env.scenarios.small import MComSmall
 
 scenarios = {"small": MComSmall, "medium": MComMedium, "large": MComLarge}
 handlers = {"ma": MComMAHandler, "central": MComCentralHandler}
 
 for scenario, handler in itertools.product(scenarios, handlers):
     env_name = scenarios[scenario].__name__
     config = {"handler": handlers[handler]}
```

### Comparing `mobile-env-1.1.4/mobile_env.egg-info/PKG-INFO` & `mobile-env-2.0.0/mobile_env.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,73 @@
 Metadata-Version: 2.1
 Name: mobile-env
-Version: 1.1.4
+Version: 2.0.0
 Summary: mobile-env: An Open Environment for Autonomous Coordination in Wireless Mobile Networks
 Home-page: https://github.com/stefanbschneider/mobile-env
 Author: Stefan Schneider, Stefan Werner
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-package.yml/badge.svg)](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-package.yml)
 [![PyPI](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-publish.yml/badge.svg)](https://github.com/stefanbschneider/mobile-env/actions/workflows/python-publish.yml)
 [![Documentation](https://readthedocs.org/projects/mobile-env/badge/?version=latest)](https://mobile-env.readthedocs.io/en/latest/?badge=latest)
+[![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)
 
 
 # mobile-env: An Open Environment for Autonomous Coordination in Mobile Networks
 
-mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks. 
+mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks.
 The environment allows modeling users moving around an area and can connect to one or multiple base stations.
 Using the Gym interface, the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
 The environment is highly configurable and can be easily extended (e.g., regarding users, movement patterns, channel models, etc.).
 
 mobile-env supports multi-agent and centralized reinforcement learning policies. It provides various choices for rewards and observations. mobile-env is also easily extendable, so that anyone may add another channel models (e.g. path loss), movement patterns, utility functions, etc.
 
 As an example, mobile-env can be used to study multi-cell selection in coordinated multipoint.
-Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally. 
-To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates. 
-However, BSs multiplex resources among connected UEs (e.g. schedule physical resource blocks) and, therefore, UEs compete for limited resources (conflicting goals). 
+Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally.
+To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates.
+However, BSs multiplex resources among connected UEs (e.g. schedule physical resource blocks) and, therefore, UEs compete for limited resources (conflicting goals).
 To maximize QoE globally, the policy must recognize that (1) the data rate of any connection is governed by the channel (e.g. SNR) between UE and BS and (2) QoE of single UEs not necessarily grows linearly with increasing data rate.
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/36734964/139288123-7732eff2-24d4-4c25-87fd-ac906f261c93.gif" width="65%"/>
     <br>
     <sup><a href="https://thenounproject.com/search/?q=base+station&i=1286474" target="_blank">Base station icon</a> by Clea Doltz from the Noun Project</sup>
 </p>
 
 **[Try mobile-env: ![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)**
 
 Documentation and API: [ReadTheDocs](https://mobile-env.readthedocs.io/en/latest/)
 
 
+## Citation
+
+
+If you use `mobile-env` in your work, please cite our paper ([author PDF](https://ris.uni-paderborn.de/download/30236/30237/author_version.pdf)):
+
+```
+@inproceedings{schneider2022mobileenv,
+  author = {Schneider, Stefan and Werner, Stefan and Khalili, Ramin and Hecker, Artur and Karl, Holger},
+  title = {mobile-env: An Open Platform for Reinforcement Learning in Wireless Mobile Networks},
+  booktitle={Network Operations and Management Symposium (NOMS)},
+  year = {2022},
+  publisher = {IEEE/IFIP},
+}
+```
+
+mobile-env is based on the underlying environment using in [DeepCoMP](https://github.com/CN-UPB/DeepCoMP), which is a combination of reinforcement learning approaches for dynamic multi-cell selection.
+mobile-env provides this underlying environment as open, stand-alone environment.
+
+
 ## Installation
 
 ### From PyPI (Recommended)
 
 The simplest option is to install the latest release of `mobile-env` from [PyPI](https://pypi.org/project/mobile-env/) using pip:
 
 ```bash
@@ -69,34 +88,35 @@
 
 If you want to run tests or examples, also install the requirements in `tests`.
 For dependencies for building docs, install the requirements in `docs`.
 
 ## Example Usage
 
 ```python
-import gym
+import gymnasium as gym
 import mobile_env
 
 env = gym.make("mobile-medium-central-v0")
-obs = env.reset()
+obs, info = env.reset()
 done = False
 
 while not done:
     action = ... # Your agent code here
-    obs, reward, done, info = env.step(action)
+    obs, reward, terminated, truncated, info = env.step(action)
+    done = terminated or truncated
     env.render()
 ```
 
 ## Customization
 
-mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions. 
+mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions.
 For example, replacing the default [Okumura–Hata](https://en.wikipedia.org/wiki/Hata_model) channel model by a (simplified) path loss model can be as easy as this:
 
 ```python
-import gym
+import gymnasium as gym
 import numpy as np
 from mobile_env.core.base import MComCore
 from mobile_env.core.channel import Channel
 
 
 class PathLoss(Channel):
     def __init__(self, gamma, **kwargs):
@@ -107,57 +127,35 @@
     def power_loss(self, bs, ue):
         """Computes power loss between BS and UE."""
         dist = bs.point.distance(ue.point)
         loss = 10 * self.gamma * np.log10(4 * np.pi * dist * bs.frequency)
         return loss
 
 
-# replace default channel model in configuration 
+# replace default channel model in configuration
 config = MComCore.default_config()
 config['channel'] = PathLoss
 
 # pass init parameters to custom channel class!
 config['channel_params'].update({'gamma': 2.0})
 
 # create environment with custom channel model
 env = gym.make('mobile-small-central-v0', config=config)
 # ...
 ```
 
+## Projects Using mobile-env
 
-## About `mobile-env`
-
-
-If you use mobile-env in your work, please cite with:
-
-```
-@misc{mobile-env,
-  author = {Schneider, Stefan and Werner, Stefan and Karl, Holger},
-  title = {An Open Environment for Autonomous Coordination in Mobile Networks},
-  year = {2021},
-  publisher = {GitHub},
-  journal = {GitHub Repository},
-  howpublished = {\url{https://github.com/stefanbschneider/mobile-env}},
-}
-```
-
-mobile-env is based on [DeepCoMP](https://github.com/CN-UPB/DeepCoMP), providing the underlying environment as open, stand-alone platform to be used by others.
-
-
-List of repositories, publications, or preprints using `mobile-env` (please open a pull request to add missing entries):
-
-* [DeepCoMP](https://github.com/CN-UPB/DeepCoMP)
+If you are using `movile-env`, please let us know and we are happy to link to your project from the readme. You can also open a pull request yourself.
 
+* [Mohammadreza Kouchaki and Vuk Marojevic, "Actor-Critic Network for O-RAN Resource Allocation: xApp Design, Deployment, and Analysis", 2022](https://arxiv.org/abs/2210.04604)
+* [Stefan Schneider, Ramin Khalili, Artur Hecker, Holger Karl, "DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)", 2021](https://github.com/CN-UPB/DeepCoMP)
 
 
 ## Contributing
 
 Development: [@stefanbschneider](https://github.com/stefanbschneider) and [@stwerner97](https://github.com/stwerner97/)
 
 
-We happy if you find `mobile-env` useful. If you have feedback or want to report bugs, feel free to [open an issue](https://github.com/stefanbschneider/mobile-env/issues/new).
+We happy if you find `mobile-env` useful. If you have feedback or want to report bugs, feel free to [open an issue](https://github.com/stefanbschneider/mobile-env/issues/new). Also, we are happy to link to your projects if you use `mobile-env`.
 
 We also welcome contributions: Whether you implement a new channel model, fix a bug, or just make a minor addition elsewhere, feel free to open a pull request!
-
-
-
-
```

### Comparing `mobile-env-1.1.4/mobile_env.egg-info/SOURCES.txt` & `mobile-env-2.0.0/mobile_env.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 mobile_env/__init__.py
 mobile_env.egg-info/PKG-INFO
 mobile_env.egg-info/SOURCES.txt
 mobile_env.egg-info/dependency_links.txt
 mobile_env.egg-info/not-zip-safe
 mobile_env.egg-info/requires.txt
@@ -27,8 +28,9 @@
 mobile_env/scenarios/large.py
 mobile_env/scenarios/medium.py
 mobile_env/scenarios/registry.py
 mobile_env/scenarios/small.py
 mobile_env/wrappers/__init__.py
 mobile_env/wrappers/multi_agent.py
 tests/__init__.py
-tests/test_central_envs.py
+tests/test_central_envs.py
+tests/test_env_stepping.py
```

### Comparing `mobile-env-1.1.4/setup.py` & `mobile-env-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import os
-from setuptools import setup, find_packages
 
+from setuptools import find_packages, setup
 
 # read the contents of the README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 requirements = [
-    "gym>=0.19.0",
-    "matplotlib==3.5.0",
-    "numpy==1.21.4",
-    "pygame==2.1.0",
-    "shapely==1.8.0",
-    "svgpath2mpl==1.0.0",
+    "gymnasium",
+    "matplotlib",
+    "numpy",
+    "pandas",
+    "pygame",
+    "shapely",
+    "svgpath2mpl",
 ]
 
 setup(
     name="mobile-env",
-    version="1.1.4",
+    version="2.0.0",
     author="Stefan Schneider, Stefan Werner",
-    description="mobile-env: An Open Environment for Autonomous Coordination in Wireless Mobile Networks",
+    description="mobile-env: An Open Environment for Autonomous Coordination in "
+    "Wireless Mobile Networks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/stefanbschneider/mobile-env",
     packages=find_packages(),
-    python_requires=">=3.7.*",
+    python_requires=">=3.7.0",
     install_requires=requirements,
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

