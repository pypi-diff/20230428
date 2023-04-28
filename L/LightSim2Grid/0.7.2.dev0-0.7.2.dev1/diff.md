# Comparing `tmp/LightSim2Grid-0.7.2.dev0.tar.gz` & `tmp/LightSim2Grid-0.7.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LightSim2Grid-0.7.2.dev0.tar", last modified: Wed Feb 22 15:33:38 2023, max compression
+gzip compressed data, was "LightSim2Grid-0.7.2.dev1.tar", last modified: Fri Apr 28 14:27:30 2023, max compression
```

## Comparing `LightSim2Grid-0.7.2.dev0.tar` & `LightSim2Grid-0.7.2.dev1.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-22 15:33:38.576439 LightSim2Grid-0.7.2.dev0/
--rw-r--r--   0 runner     (501) staff       (20)      449 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/AUTHORS.txt
--rw-r--r--   0 runner     (501) staff       (20)    16725 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    16725 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/LICENSE.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-22 15:33:38.498767 LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    18311 2023-02-22 15:33:38.000000 LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1464 2023-02-22 15:33:38.000000 LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-02-22 15:33:38.000000 LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-02-22 15:33:37.000000 LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      297 2023-02-22 15:33:38.000000 LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       32 2023-02-22 15:33:38.000000 LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)    18311 2023-02-22 15:33:38.544863 LightSim2Grid-0.7.2.dev0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    17147 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-22 15:33:38.501740 LightSim2Grid-0.7.2.dev0/lightsim2grid/
--rw-r--r--   0 runner     (501) staff       (20)     1596 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-22 15:33:38.502182 LightSim2Grid-0.7.2.dev0/lightsim2grid/elements/
--rw-r--r--   0 runner     (501) staff       (20)     1216 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/elements/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-22 15:33:38.508499 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/
--rw-r--r--   0 runner     (501) staff       (20)      553 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1430 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_gen.py
--rw-r--r--   0 runner     (501) staff       (20)     1989 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_line.py
--rw-r--r--   0 runner     (501) staff       (20)     1318 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_load.py
--rw-r--r--   0 runner     (501) staff       (20)     3132 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_sgen.py
--rw-r--r--   0 runner     (501) staff       (20)     1325 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_shunt.py
--rw-r--r--   0 runner     (501) staff       (20)     6040 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_slack.py
--rw-r--r--   0 runner     (501) staff       (20)     1394 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_storage.py
--rw-r--r--   0 runner     (501) staff       (20)     4373 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_trafo.py
--rw-r--r--   0 runner     (501) staff       (20)     2951 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_check_legit.py
--rw-r--r--   0 runner     (501) staff       (20)     4365 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/initGridModel.py
--rw-r--r--   0 runner     (501) staff       (20)    48512 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/lightSimBackend.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-22 15:33:38.509395 LightSim2Grid-0.7.2.dev0/lightsim2grid/newtonpf/
--rw-r--r--   0 runner     (501) staff       (20)      591 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/newtonpf/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12570 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/newtonpf/newtonpf.py
--rw-r--r--   0 runner     (501) staff       (20)     5582 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/physical_law_checker.py
--rw-r--r--   0 runner     (501) staff       (20)    13788 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/securityAnalysis.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-22 15:33:38.509845 LightSim2Grid-0.7.2.dev0/lightsim2grid/solver/
--rw-r--r--   0 runner     (501) staff       (20)     2061 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/solver/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11440 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/lightsim2grid/timeSerie.py
--rw-r--r--   0 runner     (501) staff       (20)      138 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-02-22 15:33:38.576713 LightSim2Grid-0.7.2.dev0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)    15438 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-22 15:33:38.544103 LightSim2Grid-0.7.2.dev0/src/
--rw-r--r--   0 runner     (501) staff       (20)      767 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/BaseConstants.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2980 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/BaseMultiplePowerflow.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5849 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/BaseSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)      487 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/ChooseSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4867 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/Computers.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7403 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/DataConverter.cpp
--rw-r--r--   0 runner     (501) staff       (20)    16238 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/DataGen.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6449 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/DataGeneric.cpp
--rw-r--r--   0 runner     (501) staff       (20)    11757 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/DataLine.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4353 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/DataLoad.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6389 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/DataSGen.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7133 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/DataShunt.cpp
--rw-r--r--   0 runner     (501) staff       (20)    15457 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/DataTrafo.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4864 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/GaussSeidelSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2239 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/GaussSeidelSynchSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)    32577 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/GridModel.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2589 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/KLUSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9499 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/SecurityAnalysis.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1920 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/SparseLUSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)   102754 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/help_fun_msg.cpp
--rw-r--r--   0 runner     (501) staff       (20)    64672 2023-02-22 15:28:48.000000 LightSim2Grid-0.7.2.dev0/src/main.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.918510 LightSim2Grid-0.7.2.dev1/
+-rw-r--r--   0 runner     (501) staff       (20)      449 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/AUTHORS.txt
+-rw-r--r--   0 runner     (501) staff       (20)    16725 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    16725 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/LICENSE.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.888748 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    18311 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1527 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-28 14:27:29.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      304 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       32 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)    18311 2023-04-28 14:27:30.917921 LightSim2Grid-0.7.2.dev1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    17147 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.897498 LightSim2Grid-0.7.2.dev1/lightsim2grid/
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.898013 LightSim2Grid-0.7.2.dev1/lightsim2grid/elements/
+-rw-r--r--   0 runner     (501) staff       (20)     1216 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/elements/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.904134 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/
+-rw-r--r--   0 runner     (501) staff       (20)      553 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2950 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_dc_line.py
+-rw-r--r--   0 runner     (501) staff       (20)     1430 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_gen.py
+-rw-r--r--   0 runner     (501) staff       (20)     1989 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_line.py
+-rw-r--r--   0 runner     (501) staff       (20)     1318 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_load.py
+-rw-r--r--   0 runner     (501) staff       (20)     3132 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_sgen.py
+-rw-r--r--   0 runner     (501) staff       (20)     1325 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_shunt.py
+-rw-r--r--   0 runner     (501) staff       (20)     6047 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_slack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1394 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)     4373 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_trafo.py
+-rw-r--r--   0 runner     (501) staff       (20)     2977 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_check_legit.py
+-rw-r--r--   0 runner     (501) staff       (20)     4493 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/initGridModel.py
+-rw-r--r--   0 runner     (501) staff       (20)    49089 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/lightSimBackend.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.905182 LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/
+-rw-r--r--   0 runner     (501) staff       (20)      591 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12570 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/newtonpf.py
+-rw-r--r--   0 runner     (501) staff       (20)     5582 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/physical_law_checker.py
+-rw-r--r--   0 runner     (501) staff       (20)    13788 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/securityAnalysis.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.905647 LightSim2Grid-0.7.2.dev1/lightsim2grid/solver/
+-rw-r--r--   0 runner     (501) staff       (20)     2423 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/solver/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11432 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/timeSerie.py
+-rw-r--r--   0 runner     (501) staff       (20)      138 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-28 14:27:30.918630 LightSim2Grid-0.7.2.dev1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)    15878 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.917118 LightSim2Grid-0.7.2.dev1/src/
+-rw-r--r--   0 runner     (501) staff       (20)      767 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/BaseConstants.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2980 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/BaseMultiplePowerflow.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5849 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/BaseSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      487 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/ChooseSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     4867 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/Computers.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     7403 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataConverter.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2520 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataDCLine.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    16458 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataGen.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     6449 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataGeneric.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    11757 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataLine.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     4353 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataLoad.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     6389 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataSGen.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     7133 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataShunt.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    15457 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataTrafo.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     4864 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/GaussSeidelSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2239 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/GaussSeidelSynchSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    34888 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/GridModel.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2589 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/KLUSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     9499 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/SecurityAnalysis.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1920 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/SparseLUSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)   110165 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/help_fun_msg.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    68726 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/main.cpp
```

### Comparing `LightSim2Grid-0.7.2.dev0/LICENSE` & `LightSim2Grid-0.7.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/LICENSE.md` & `LightSim2Grid-0.7.2.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/PKG-INFO` & `LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LightSim2Grid
-Version: 0.7.2.dev0
+Version: 0.7.2.dev1
 Summary: LightSim2Grid implements a c++ backend targeting the Grid2Op platform.
 Home-page: https://github.com/BDonnot/lightsim2grid/
 Author: Benjamin Donnot
 Author-email: benjamin.donnot@rte-france.com
 License: MPL 2.0
 Keywords: pandapower powergrid simulator KLU Eigen c++
 Platform: Windows
```

### Comparing `LightSim2Grid-0.7.2.dev0/LightSim2Grid.egg-info/SOURCES.txt` & `LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 lightsim2grid/__init__.py
 lightsim2grid/lightSimBackend.py
 lightsim2grid/physical_law_checker.py
 lightsim2grid/securityAnalysis.py
 lightsim2grid/timeSerie.py
 lightsim2grid/elements/__init__.py
 lightsim2grid/gridmodel/__init__.py
+lightsim2grid/gridmodel/_aux_add_dc_line.py
 lightsim2grid/gridmodel/_aux_add_gen.py
 lightsim2grid/gridmodel/_aux_add_line.py
 lightsim2grid/gridmodel/_aux_add_load.py
 lightsim2grid/gridmodel/_aux_add_sgen.py
 lightsim2grid/gridmodel/_aux_add_shunt.py
 lightsim2grid/gridmodel/_aux_add_slack.py
 lightsim2grid/gridmodel/_aux_add_storage.py
@@ -32,14 +33,15 @@
 lightsim2grid/solver/__init__.py
 src/BaseConstants.cpp
 src/BaseMultiplePowerflow.cpp
 src/BaseSolver.cpp
 src/ChooseSolver.cpp
 src/Computers.cpp
 src/DataConverter.cpp
+src/DataDCLine.cpp
 src/DataGen.cpp
 src/DataGeneric.cpp
 src/DataLine.cpp
 src/DataLoad.cpp
 src/DataSGen.cpp
 src/DataShunt.cpp
 src/DataTrafo.cpp
```

### Comparing `LightSim2Grid-0.7.2.dev0/PKG-INFO` & `LightSim2Grid-0.7.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LightSim2Grid
-Version: 0.7.2.dev0
+Version: 0.7.2.dev1
 Summary: LightSim2Grid implements a c++ backend targeting the Grid2Op platform.
 Home-page: https://github.com/BDonnot/lightsim2grid/
 Author: Benjamin Donnot
 Author-email: benjamin.donnot@rte-france.com
 License: MPL 2.0
 Keywords: pandapower powergrid simulator KLU Eigen c++
 Platform: Windows
```

### Comparing `LightSim2Grid-0.7.2.dev0/README.md` & `LightSim2Grid-0.7.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/__init__.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # See AUTHORS.txt
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of LightSim2grid, LightSim2grid implements a c++ backend targeting the Grid2Op platform.
 
-__version__ = "0.7.2.dev0"
+import faulthandler
+faulthandler.enable()
+
+__version__ = "0.7.2.dev1"
 
 __all__ = ["newtonpf", "SolverType", "ErrorType", "solver"]
 
 # import directly from c++ module
 from lightsim2grid.solver import SolverType
 from lightsim2grid.solver import ErrorType
```

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/elements/__init__.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/__init__.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_gen.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_gen.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_line.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_line.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_load.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_load.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_sgen.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_sgen.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_shunt.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_shunt.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_slack.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 warnings.warn("We found some Nans in the slack coefficients \"slack_coeff_norm\", "
                               " (probably because the slack weights sum to 0.0 initially)"
                               "We set them all to the same value !")
                 slack_coeff_norm[:] = 1.0 / slack_coeff_norm.shape[0]
                 slack_coeff[:] = 1.0
                 
             slack_gen_ids = np.arange(nb_slack) + pp_net.gen.shape[0]
-            slack_contrib = (np.sum(pp_net.gen["p_mw"]) - np.sum(pp_net.load["p_mw"]) ) * slack_coeff_norm
+            slack_contrib = -1.0 * (np.sum(pp_net.gen["p_mw"]) - np.sum(pp_net.load["p_mw"]) ) * slack_coeff_norm
             vm_pu = 1.0 * pp_net.ext_grid["vm_pu"].values
             gen_p = np.concatenate((pp_net.gen["p_mw"].values, slack_contrib))
             gen_v = np.concatenate((pp_net.gen["vm_pu"].values, vm_pu))
             gen_bus = np.concatenate((pp_net.gen["bus"].values, slack_bus_ids))
             gen_min_q = np.concatenate((pp_net.gen["min_q_mvar"].values, [-999999.]))
             gen_max_q = np.concatenate((pp_net.gen["max_q_mvar"].values, [+99999.]))
             model.init_generators(gen_p, gen_v, gen_min_q, gen_max_q, gen_bus)
```

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_storage.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_storage.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_add_trafo.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_trafo.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/_aux_check_legit.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_check_legit.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,18 @@
                            "in pandapower network")
     if "ward" in pp_net and pp_net.ward.shape[0]:
         raise RuntimeError("Unsupported element found (Ward - \"pp_net.ward\") "
                            "in pandapower network")
     if "xward" in pp_net and pp_net.xward.shape[0]:
         raise RuntimeError("Unsupported element found (Extended Ward - \"pp_net.xward\") "
                            "in pandapower network")
-    if "dcline" in pp_net and pp_net.dcline.shape[0]:
-        raise RuntimeError("Unsupported element found (DC Line - \"pp_net.dcline\") "
-                           "in pandapower network")
+    # supported now
+    # if "dcline" in pp_net and pp_net.dcline.shape[0]:
+    #     raise RuntimeError("Unsupported element found (DC Line - \"pp_net.dcline\") "
+    #                        "in pandapower network")
 
     # bus indexes should start at 0 and be contiguous
     if np.any(np.sort(pp_net.bus.index) != np.arange(pp_net.bus.shape[0])):
         raise RuntimeError("In order to work, pandapower bus indexes should start at 0 and be contiguous. "
                            "Make sure that `pp_net.bus.index` have this property. You can write a github "
                            "issue if you want improvment on this regard.")
```

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/gridmodel/initGridModel.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/initGridModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from lightsim2grid.gridmodel._aux_add_trafo import _aux_add_trafo
 from lightsim2grid.gridmodel._aux_add_line import _aux_add_line
 from lightsim2grid.gridmodel._aux_add_gen import _aux_add_gen
 from lightsim2grid.gridmodel._aux_add_shunt import _aux_add_shunt
 from lightsim2grid.gridmodel._aux_check_legit import _aux_check_legit
 from lightsim2grid.gridmodel._aux_add_slack import _aux_add_slack
 from lightsim2grid.gridmodel._aux_add_storage import _aux_add_storage
+from lightsim2grid.gridmodel._aux_add_dc_line import _aux_add_dc_line
 
 
 def init(pp_net):
     """
     Convert a pandapower network as input into a GridModel.
 
     This can fail to convert the grid and still not throw any error, use with care (for example, you can run a powerflow
@@ -105,11 +106,14 @@
 
     # handle generators
     _aux_add_gen(model, pp_net)
 
     # handle storage units
     _aux_add_storage(model, pp_net)
 
+    # handle dc line
+    _aux_add_dc_line(model, pp_net)
+
     # deal with slack bus
     _aux_add_slack(model, pp_net)
 
     return model
```

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/lightSimBackend.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/lightSimBackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,28 @@
     def __init__(self,
                  detailed_infos_for_cascading_failures: bool=False,
                  can_be_copied: bool=True,
                  max_iter: int=10,
                  tol: float=1e-8,
                  solver_type: Optional[SolverType]=None,
                  turned_off_pv : bool=True,  # are gen turned off (or with p=0) contributing to voltage or not
-                 dist_slack_non_renew: bool=False  # distribute the slack on non renewable turned on (and with P>0) generators
+                 dist_slack_non_renew: bool=False,  # distribute the slack on non renewable turned on (and with P>0) generators
+                 use_static_gen: bool=False, # add the static generators as generator gri2dop side
                  ):
         try:
             # for grid2Op >= 1.7.1
             Backend.__init__(self,
                              detailed_infos_for_cascading_failures=detailed_infos_for_cascading_failures,
                              can_be_copied=can_be_copied,
                              solver_type=solver_type,
                              max_iter=max_iter,
                              tol=tol,
                              turned_off_pv=turned_off_pv,
-                             dist_slack_non_renew=dist_slack_non_renew)
+                             dist_slack_non_renew=dist_slack_non_renew,
+                             use_static_gen=use_static_gen)
         except TypeError as exc_:
             warnings.warn("Please use grid2op >= 1.7.1: with older grid2op versions, "
                           "you cannot set max_iter, tol nor solver_type arguments.")
             Backend.__init__(self,
                              detailed_infos_for_cascading_failures=detailed_infos_for_cascading_failures)
 
         # lazy loading because it crashes...
@@ -157,14 +159,17 @@
         # does the "turned off" generators (including when p=0)
         # are pv buses
         self._turned_off_pv = turned_off_pv
         
         # distributed slack, on non renewable gen with P > 0
         self._dist_slack_non_renew = dist_slack_non_renew
         
+        # add the static gen to the list of controlable gen in grid2Op
+        self._use_static_gen = use_static_gen  # TODO implement it
+        
     def turnedoff_no_pv(self):
         self._turned_off_pv = False
         self._grid.turnedoff_no_pv()
         
     def turnedoff_pv(self):
         self._turned_off_pv = True
         self._grid.turnedoff_pv()
@@ -405,15 +410,15 @@
         self.lines_or_pu_to_kv = self.init_pp_backend.lines_or_pu_to_kv
         self.lines_ex_pu_to_kv = self.init_pp_backend.lines_ex_pu_to_kv
 
         self.name_gen = self.init_pp_backend.name_gen
         self.name_load = self.init_pp_backend.name_load
         self.name_line = self.init_pp_backend.name_line
         self.name_sub = self.init_pp_backend.name_sub
-
+            
         # TODO storage check grid2op version and see if storage is available !
         if self.__has_storage:
             self.n_storage = self.init_pp_backend.n_storage
             self.storage_to_subid = self.init_pp_backend.storage_to_subid
             self.storage_pu_to_kv = self.init_pp_backend.storage_pu_to_kv
             self.name_storage = self.init_pp_backend.name_storage
             self.storage_to_sub_pos = self.init_pp_backend.storage_to_sub_pos
@@ -669,16 +674,18 @@
             # shunt topology
             # (need to be done before to avoid error like "impossible to set reactive value of a disconnected shunt")
             for sh_id, new_bus in shunt_bus:
                 if new_bus == -1:
                     self._grid.deactivate_shunt(sh_id)
                 else:
                     self._grid.reactivate_shunt(sh_id)
-                    self._grid.change_bus_shunt(sh_id, self.shunt_to_subid[sh_id] * new_bus)
-
+                    if hasattr(type(self), "local_bus_to_global_int"):
+                        self._grid.change_bus_shunt(sh_id, type(self).local_bus_to_global_int(new_bus, self.shunt_to_subid[sh_id]))
+                    else:
+                        self._grid.change_bus_shunt(sh_id, self.shunt_to_subid[sh_id] + (new_bus == 2) * type(self).n_sub)
             for sh_id, new_p in shunt_p:
                 self._grid.change_p_shunt(sh_id, new_p)
             for sh_id, new_q in shunt_q:
                 self._grid.change_q_shunt(sh_id, new_q)
 
         # and now change the overall topology
         # TODO hack for storage units: if 0. production i pretend they are disconnected on the
```

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/newtonpf/__init__.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 # See AUTHORS.txt
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of LightSim2grid, LightSim2grid implements a c++ backend targeting the Grid2Op platform.
 
-from lightsim2grid.newtonpf.newtonpf import newtonpf, newtonpf_new, newtonpf_old
-
 __all__ = ["newtonpf", "newtonpf_new", "newtonpf_old"]
+
+from lightsim2grid.newtonpf.newtonpf import newtonpf, newtonpf_new, newtonpf_old
```

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/newtonpf/newtonpf.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/newtonpf.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/physical_law_checker.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/physical_law_checker.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/securityAnalysis.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/securityAnalysis.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/solver/__init__.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/solver/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,46 +14,46 @@
            "SparseLUSolver",
            "SparseLUSolverSingleSlack",
            "DCSolver"]
 
 from lightsim2grid_cpp import SolverType
 from lightsim2grid_cpp import ErrorType
 from lightsim2grid_cpp import AnySolver
-
-from lightsim2grid_cpp import GaussSeidelSolver
-from lightsim2grid_cpp import GaussSeidelSynchSolver
-from lightsim2grid_cpp import SparseLUSolver
-from lightsim2grid_cpp import SparseLUSolverSingleSlack
-from lightsim2grid_cpp import DCSolver
+               
+from lightsim2grid_cpp import GaussSeidelSolver  # SolverType.GaussSeidel
+from lightsim2grid_cpp import GaussSeidelSynchSolver  # SolverType.GaussSeidelSynch
+from lightsim2grid_cpp import SparseLUSolver  # SolverType.SparseLU
+from lightsim2grid_cpp import SparseLUSolverSingleSlack  # SolverType.SparseLUSingleSlack
+from lightsim2grid_cpp import DCSolver  # SolverType.DC
 
 try:
-    from lightsim2grid_cpp import KLUSolver
-    from lightsim2grid_cpp import KLUSolverSingleSlack
-    from lightsim2grid_cpp import KLUDCSolver
+    from lightsim2grid_cpp import KLUSolver  # SolverType.KLU
+    from lightsim2grid_cpp import KLUSolverSingleSlack  # SolverType.KLUSingleSlack
+    from lightsim2grid_cpp import KLUDCSolver  # SolverType.KLUDC
     __all__.append("KLUSolver")
     __all__.append("KLUSolverSingleSlack")
     __all__.append("KLUDCSolver")
 except Exception as exc_:
     # KLU is not available
     pass
 
 try:
-    from lightsim2grid_cpp import NICSLUSolver
-    from lightsim2grid_cpp import NICSLUSolverSingleSlack
-    from lightsim2grid_cpp import NICSLUDCSolver
+    from lightsim2grid_cpp import NICSLUSolver  # SolverType.NICSLU
+    from lightsim2grid_cpp import NICSLUSolverSingleSlack  # SolverType.NICSLUSingleSlack
+    from lightsim2grid_cpp import NICSLUDCSolver  # SolverType.NICSLUDC
     __all__.append("NICSLUSolver")
     __all__.append("NICSLUSolverSingleSlack")
     __all__.append("NICSLUDCSolver")
 except Exception as exc_:
     # NICSLU is not available
     pass
 
 try:
-    from lightsim2grid_cpp import CKTSOSolver
-    from lightsim2grid_cpp import CKTSOSolverSingleSlack
-    from lightsim2grid_cpp import CKTSODCSolver
+    from lightsim2grid_cpp import CKTSOSolver  # SolverType.CKTSO
+    from lightsim2grid_cpp import CKTSOSolverSingleSlack  # SolverType.CKTSOSingleSlack
+    from lightsim2grid_cpp import CKTSODCSolver  # SolverType.CKTSODC
     __all__.append("CKTSOSolver")
     __all__.append("CKTSOSolverSingleSlack")
     __all__.append("CKTSODCSolver")
 except Exception as exc_:
     # NICSLU is not available
     pass
```

### Comparing `LightSim2Grid-0.7.2.dev0/lightsim2grid/timeSerie.py` & `LightSim2Grid-0.7.2.dev1/lightsim2grid/timeSerie.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of LightSim2grid, LightSim2grid implements a c++ backend targeting the Grid2Op platform.
 
 __all__ = ["Computers", "TimeSerie"]
-import os
+
 import numpy as np
 import warnings
 
 from grid2op.Chronics import Multifolder, GridStateFromFile
 
 from lightsim2grid.lightSimBackend import LightSimBackend
 from lightsim2grid.solver import SolverType
 from lightsim2grid_cpp import Computers
 
+
 class TimeSerie:
     """
     This helper class, that only works with grid2op when using a LightSimBackend allows to compute
     the flows (at the origin side of the powerline / transformers). It is roughly equivalent to the
     grid2op code:
 
     .. code-block:: python
```

### Comparing `LightSim2Grid-0.7.2.dev0/setup.py` & `LightSim2Grid-0.7.2.dev1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup
 import sys
 import os
 import warnings
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
 
-__version__ = "0.7.2.dev0"
+__version__ = "0.7.2.dev1"
 KLU_SOLVER_AVAILABLE = False
 
 # Try to link against SuiteSparse (if available)
 # check that they exist (if SuiteSparse has been built with "make")
 suitesparse_path_make = os.path.abspath("./SuiteSparse")
 LIBS_MAKE = ["{}/KLU/Lib/libklu.a",
              "{}/BTF/Lib/libbtf.a",
@@ -145,14 +145,15 @@
              "src/DataLine.cpp",
              "src/DataGeneric.cpp",
              "src/DataShunt.cpp",
              "src/DataTrafo.cpp",
              "src/DataLoad.cpp",
              "src/DataGen.cpp",
              "src/DataSGen.cpp",
+             "src/DataDCLine.cpp",
              "src/ChooseSolver.cpp",
              "src/GaussSeidelSolver.cpp",
              "src/GaussSeidelSynchSolver.cpp",
              "src/BaseSolver.cpp",
              "src/BaseMultiplePowerflow.cpp",
              "src/Computers.cpp",
              "src/SecurityAnalysis.cpp"]
@@ -205,15 +206,15 @@
     if include_nicslu and libnicslu_path is not None:
         LIBS.append(os.path.join(path_nicslu, libnicslu_path))
         include_dirs.append(os.path.join(path_nicslu, "include"))
         src_files.append("src/NICSLUSolver.cpp")
         extra_compile_args.append("-DNICSLU_SOLVER_AVAILABLE")
         print("INFO: Using NICSLU package")
 
-# Try to locate the CKTSO sparse linaer solver
+# Try to locate the CKTSO sparse linear solver
 if "PATH_CKTSO" in os.environ:
     # user indicate the path for the CKTSO library (see https://github.com/chenxm1986/cktso)
     # eg "/home/user/Documents/cktso/"
     
     path_cktso = os.path.abspath(os.environ["PATH_CKTSO"])
     include_cktso = True
     # check for appropriate license
@@ -307,16 +308,24 @@
     )
 ]
 
 # before pandapower 2.8 scipy was forced to be <= 1.6 which does not work with
 # python 3.10+
 req_pkgs = [
         "pandapower" if sys.version_info < (3, 10) else "pandapower>=2.8",
+        "pytest",  # for pandapower see https://github.com/e2nIEE/pandapower/issues/1988
     ]
 
+if sys.version_info.major == 3 and sys.version_info.minor <= 7:
+    # typing "Literal" not available on python 3.7
+    req_pkgs.append("typing_extensions")
+    # do not use pandapower 2.12 (broken on python 3.7 
+    # see https://github.com/e2nIEE/pandapower/issues/1985
+    req_pkgs[0] = "pandapower>=2.2.2,<2.12"
+
 pkgs = {
     "required": req_pkgs,
     "extras": {
         "docs": [
             "numpydoc>=0.9.2",
             "sphinx>=2.4.4",
             "sphinx-rtd-theme>=0.4.3",
```

### Comparing `LightSim2Grid-0.7.2.dev0/src/BaseConstants.cpp` & `LightSim2Grid-0.7.2.dev1/src/BaseConstants.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/BaseMultiplePowerflow.cpp` & `LightSim2Grid-0.7.2.dev1/src/BaseMultiplePowerflow.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/BaseSolver.cpp` & `LightSim2Grid-0.7.2.dev1/src/BaseSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/Computers.cpp` & `LightSim2Grid-0.7.2.dev1/src/Computers.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/DataConverter.cpp` & `LightSim2Grid-0.7.2.dev1/src/DataConverter.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/DataGen.cpp` & `LightSim2Grid-0.7.2.dev1/src/DataGen.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -315,34 +315,39 @@
         const auto my_contrib_slack = gen_slack_weight_[gen_id];
         // now take "my part"
         // std::cout << "gen_id " << gen_id << " my_contrib_slack " << my_contrib_slack << ", " << total_contrib_slack << " node_mismatch " << node_mismatch(bus_id_solver) << std::endl;
         res_p_(gen_id) += node_mismatch(bus_id_solver) * my_contrib_slack / total_contrib_slack;
     }
 }
 
-void DataGen::init_q_vector(int nb_bus_total)  // total number of bus on the grid
+void DataGen::init_q_vector(int nb_bus,
+                            Eigen::VectorXi & total_gen_per_bus,
+                            RealVect & total_q_min_per_bus,
+                            RealVect & total_q_max_per_bus) const // delta_q_per_gen_)  // total number of bus on the grid
 {
     const int nb_gen = nb();
-    total_q_min_per_bus_ = RealVect::Constant(nb_bus_total, 0.);
-    total_q_max_per_bus_ = RealVect::Constant(nb_bus_total, 0.);
-    total_gen_per_bus_ = Eigen::VectorXi::Constant(nb_bus_total, 0);
     for(int gen_id = 0; gen_id < nb_gen; ++gen_id)
     {
         if(!status_[gen_id]) continue;
 
         if ((!turnedoff_gen_pv_) && p_mw_(gen_id) == 0.) continue;  // in this case turned off generators are not pv
         
         int bus_id = bus_id_(gen_id);
-        total_q_min_per_bus_(bus_id) += min_q_(gen_id);
-        total_q_max_per_bus_(bus_id) += max_q_(gen_id);
-        total_gen_per_bus_(bus_id) += 1;
+        total_q_min_per_bus(bus_id) += min_q_(gen_id);
+        total_q_max_per_bus(bus_id) += max_q_(gen_id);
+        total_gen_per_bus(bus_id) += 1;
     }
 }
 
-void DataGen::set_q(const RealVect & reactive_mismatch, const std::vector<int> & id_grid_to_solver, bool ac)
+void DataGen::set_q(const RealVect & reactive_mismatch,
+                    const std::vector<int> & id_grid_to_solver,
+                    bool ac,
+                    const Eigen::VectorXi & total_gen_per_bus,
+                    const RealVect & total_q_min_per_bus,
+                    const RealVect & total_q_max_per_bus)
 {
     const int nb_gen = nb();
     res_q_ = RealVect::Constant(nb_gen, 0.);
     if(!ac) return;  // do not consider Q values in dc mode
     real_type eps_q = 1e-8;
     for(int gen_id = 0; gen_id < nb_gen; ++gen_id)
     {
@@ -353,17 +358,17 @@
 
         int bus_id = bus_id_(gen_id);
         const auto bus_solver = id_grid_to_solver[bus_id];
         // TODO DEBUG MODE: check that the bus is correct!
         real_type q_to_absorb = reactive_mismatch[bus_solver];
         real_type max_q_me = max_q_(gen_id);
         real_type min_q_me = min_q_(gen_id);
-        real_type max_q_bus = total_q_max_per_bus_(bus_id);
-        real_type min_q_bus = total_q_min_per_bus_(bus_id);
-        int nb_gen_with_me = total_gen_per_bus_(bus_id);
+        real_type max_q_bus = total_q_max_per_bus(bus_id);
+        real_type min_q_bus = total_q_min_per_bus(bus_id);
+        int nb_gen_with_me = total_gen_per_bus(bus_id);
         if(nb_gen_with_me == 1){
             real_q = q_to_absorb;
         }else{
             real_type ratio = (max_q_me - min_q_me + eps_q) / (max_q_bus - min_q_bus + nb_gen_with_me * eps_q) ;
             real_q = q_to_absorb * ratio ;
         }
         res_q_(gen_id) = real_q;
```

### Comparing `LightSim2Grid-0.7.2.dev0/src/DataGeneric.cpp` & `LightSim2Grid-0.7.2.dev1/src/DataGeneric.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/DataLine.cpp` & `LightSim2Grid-0.7.2.dev1/src/DataLine.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/DataLoad.cpp` & `LightSim2Grid-0.7.2.dev1/src/DataLoad.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/DataSGen.cpp` & `LightSim2Grid-0.7.2.dev1/src/DataSGen.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/DataShunt.cpp` & `LightSim2Grid-0.7.2.dev1/src/DataShunt.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/DataTrafo.cpp` & `LightSim2Grid-0.7.2.dev1/src/DataTrafo.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/GaussSeidelSolver.cpp` & `LightSim2Grid-0.7.2.dev1/src/GaussSeidelSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/GaussSeidelSynchSolver.cpp` & `LightSim2Grid-0.7.2.dev1/src/GaussSeidelSynchSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/GridModel.cpp` & `LightSim2Grid-0.7.2.dev1/src/GridModel.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
     // 7. static generators
     sgens_ = other.sgens_;
 
     // 8. storage units
     storages_ = other.storages_;
 
+    // dc lines
+    dc_lines_ = other.dc_lines_;
+
     // copy the attributes specific grid2op (speed optimization)
     n_sub_ = other.n_sub_;
     load_pos_topo_vect_ = other.load_pos_topo_vect_;
     gen_pos_topo_vect_ = other.gen_pos_topo_vect_;
     line_or_pos_topo_vect_ = other.line_or_pos_topo_vect_;
     line_ex_pos_topo_vect_ = other.line_ex_pos_topo_vect_;
     trafo_hv_pos_topo_vect_ = other.trafo_hv_pos_topo_vect_;
@@ -77,29 +80,31 @@
     auto res_line = powerlines_.get_state();
     auto res_shunt = shunts_.get_state();
     auto res_trafo = trafos_.get_state();
     auto res_gen = generators_.get_state();
     auto res_load = loads_.get_state();
     auto res_sgen = sgens_.get_state();
     auto res_storage = storages_.get_state();
+    auto res_dc_line = dc_lines_.get_state();
 
     GridModel::StateRes res(version_major,
                             version_medium,
                             version_minor,
                             init_vm_pu_,
                             sn_mva_,
                             bus_vn_kv,
                             bus_status_,
                             res_line,
                             res_shunt,
                             res_trafo,
                             res_gen,
                             res_load,
                             res_sgen,
-                            res_storage
+                            res_storage,
+                            res_dc_line
                             );
     return res;
 };
 
 void GridModel::set_state(GridModel::StateRes & my_state)
 {
     // after loading back, the instance need to be reset anyway
@@ -138,14 +143,16 @@
     DataGen::StateRes & state_gens = std::get<10>(my_state);
     // loads
     DataLoad::StateRes & state_loads = std::get<11>(my_state);
     // static gen
     DataSGen::StateRes & state_sgens= std::get<12>(my_state);
     // storage units
     DataLoad::StateRes & state_storages = std::get<13>(my_state);
+    // dc lines
+    DataDCLine::StateRes & state_dc_lines = std::get<14>(my_state);
 
     // assign it to this instance
 
     // buses
     // 1. bus_vn_kv_
     bus_vn_kv_ = RealVect::Map(&bus_vn_kv[0], bus_vn_kv.size());
     // 2. bus status
@@ -162,14 +169,16 @@
     generators_.set_state(state_gens);
     // 5. loads
     loads_.set_state(state_loads);
     // 6. static generators
     sgens_.set_state(state_sgens);
     // 7. storage units
     storages_.set_state(state_storages);
+    // dc lines
+    dc_lines_.set_state(state_dc_lines);
 };
 
 //init
 void GridModel::init_bus(const RealVect & bus_vn_kv, int nb_line, int nb_trafo){
     /**
     initialize the bus_vn_kv_ member
     and
@@ -243,14 +252,73 @@
     // store results (in ac mode)
     process_results(conv, res, Vinit, true, id_me_to_ac_solver_);
 
     // return the vector of complex voltage at each bus
     return res;
 };
 
+void GridModel::check_solution_q_values_onegen(CplxVect & res,
+                                               const DataGen::GenInfo& gen,
+                                               bool check_q_limits) const{
+    if(check_q_limits)
+    {
+        // i need to check the reactive can be absorbed / produced by the generator
+        real_type new_q = my_zero_;
+        real_type react_this_bus = std::imag(res.coeff(gen.bus_id));
+        if((react_this_bus >= gen.min_q_mvar) && (react_this_bus <= gen.max_q_mvar))
+        {
+            // this generator is able to handle all reactive
+            new_q = my_zero_;
+        }else if(react_this_bus < gen.min_q_mvar){
+            // generator cannot absorb enough reactive power
+            new_q = react_this_bus - gen.min_q_mvar; //ex. need -50, qmin is -30, remains: (-50) - (-30) = -20 MVAr
+        }else{
+            // generator cannot produce enough reactive power
+            new_q = react_this_bus - gen.max_q_mvar;  // ex. need 50, qmax is 30, remains: 50 - 30 = 20 MVAr
+        }
+        res.coeffRef(gen.bus_id) = {std::real(res.coeff(gen.bus_id)), new_q};
+    }else{
+        // the q value for the bus at which the generator is connected will be 0
+        res.coeffRef(gen.bus_id) = {std::real(res.coeff(gen.bus_id)), my_zero_};
+    }
+}
+
+void GridModel::check_solution_q_values(CplxVect & res, bool check_q_limits) const{
+    // test for iterator though generators
+    for(const auto & gen: generators_)
+    {
+        if(!gen.connected)
+        {
+            // the generator is disconnected, I do nothing
+            continue;
+        }
+        check_solution_q_values_onegen(res, gen, check_q_limits);
+
+        // if(gen.id == gen_slackbus_)
+        if(gen.is_slack)
+        {
+            // slack bus, by definition, can handle all active value
+            // This is probably not the case with distributed slack !
+            res.coeffRef(gen.bus_id) = {my_zero_, std::imag(res.coeff(gen.bus_id))};
+        }
+    }
+
+    // then do the same for dc powerlines
+    for(const auto & dcline: dc_lines_)
+    {
+        if(!dcline.connected)
+        {
+            // the generator is disconnected, I do nothing
+            continue;
+        }
+        check_solution_q_values_onegen(res, dcline.gen_or, check_q_limits);
+        check_solution_q_values_onegen(res, dcline.gen_ex, check_q_limits);
+    }
+}
+
 CplxVect GridModel::check_solution(const CplxVect & V_proposed, bool check_q_limits)
 {
     // pre process the data to define a proper jacobian matrix, the proper voltage vector etc.
     const int nb_bus = static_cast<int>(V_proposed.size());
     bool is_ac = true;
     bool reset_solver = false;
     CplxVect V = pre_process_solver(V_proposed, Ybus_ac_, 
@@ -266,52 +334,15 @@
     CplxVect res = _get_results_back_to_orig_nodes(mis,
                                                    id_me_to_ac_solver_,
                                                    static_cast<int>(V_proposed.size())
                                                    );
     if(sn_mva_ != 1.) res *= sn_mva_;
 
     // now check reactive values for buses where there are generators and active values of slack bus
-    // test for iterator though generator
-    for(const auto & gen: generators_)
-    {
-        if(!gen.connected)
-        {
-            // the generator is disconnected, I do nothing
-            continue;
-        }
-        if(check_q_limits)
-        {
-            // i need to check the reactive can be absorbed / produced by the generator
-            real_type new_q = my_zero_;
-            real_type react_this_bus = std::imag(res.coeff(gen.bus_id));
-            if((react_this_bus >= gen.min_q_mvar) && (react_this_bus <= gen.max_q_mvar))
-            {
-                // this generator is able to handle all reactive
-                new_q = my_zero_;
-            }else if(react_this_bus < gen.min_q_mvar){
-                // generator cannot absorb enough reactive power
-                new_q = react_this_bus - gen.min_q_mvar; //ex. need -50, qmin is -30, remains: (-50) - (-30) = -20 MVAr
-            }else{
-                // generator cannot produce enough reactive power
-                new_q = react_this_bus - gen.max_q_mvar;  // ex. need 50, qmax is 30, remains: 50 - 30 = 20 MVAr
-            }
-            res.coeffRef(gen.bus_id) = {std::real(res.coeff(gen.bus_id)), new_q};
-        }else{
-            // the q value for the bus at which the generator is connected will be 0
-            res.coeffRef(gen.bus_id) = {std::real(res.coeff(gen.bus_id)), my_zero_};
-        }
-
-        // if(gen.id == gen_slackbus_)
-        if(gen.is_slack)
-        {
-            // slack bus, by definition, can handle all active value
-            // This is probably not the case with distributed slack !
-            res.coeffRef(gen.bus_id) = {my_zero_, std::imag(res.coeff(gen.bus_id))};
-        }
-    }
+    check_solution_q_values(res, check_q_limits);
 
     // set to 0 the error on the disconnected bus (it is not initialized at 0.0 in _get_results_back_to_orig_nodes)
     for(int bus_id = 0; bus_id < nb_bus; ++bus_id)
     {
         if(bus_status_[bus_id]) continue;
         res.coeffRef(bus_id) = my_zero_;
     }
@@ -347,25 +378,31 @@
         // TODO do not reinit Ybus if the topology does not change
         init_Ybus(Ybus, id_me_to_solver, id_solver_to_me);
         fillYbus(Ybus, is_ac, id_me_to_solver);
     }
     init_Sbus(Sbus_, id_me_to_solver, id_solver_to_me, slack_bus_id_solver);
     fillpv_pq(id_me_to_solver, id_solver_to_me, slack_bus_id_solver); // TODO what if pv and pq changed ? :O
     
-    generators_.init_q_vector(static_cast<int>(bus_vn_kv_.size()));
+    int nb_bus_total = static_cast<int>(bus_vn_kv_.size());
+    total_q_min_per_bus_ = RealVect::Constant(nb_bus_total, 0.);
+    total_q_max_per_bus_ = RealVect::Constant(nb_bus_total, 0.);
+    total_gen_per_bus_ = Eigen::VectorXi::Constant(nb_bus_total, 0);
+    generators_.init_q_vector(nb_bus_total, total_gen_per_bus_, total_q_min_per_bus_, total_q_max_per_bus_);
+    dc_lines_.init_q_vector(nb_bus_total, total_gen_per_bus_, total_q_min_per_bus_, total_q_max_per_bus_);
     fillSbus_me(Sbus_, is_ac, id_me_to_solver);
 
     const int nb_bus_solver = static_cast<int>(id_solver_to_me.size());
     CplxVect V = CplxVect::Constant(nb_bus_solver, init_vm_pu_);
     for(int bus_solver_id = 0; bus_solver_id < nb_bus_solver; ++bus_solver_id){
         int bus_me_id = id_solver_to_me[bus_solver_id];  //TODO DEBUG MODE : POSSIBLE SEGFAULT
         cplx_type tmp = Vinit(bus_me_id);
         V(bus_solver_id) = tmp;
     }
     generators_.set_vm(V, id_me_to_solver);
+    dc_lines_.set_vm(V, id_me_to_solver);
     return V;
 }
 
 CplxVect GridModel::_get_results_back_to_orig_nodes(const CplxVect & res_tmp, 
                                                     std::vector<int> & id_me_to_solver,
                                                     int size)
 {
@@ -468,29 +505,30 @@
     powerlines_.fillYbus(tripletList, ac, id_me_to_solver, sn_mva_);
     shunts_.fillYbus(tripletList, ac, id_me_to_solver, sn_mva_);
     trafos_.fillYbus(tripletList, ac, id_me_to_solver, sn_mva_);
     loads_.fillYbus(tripletList, ac, id_me_to_solver, sn_mva_);
     sgens_.fillYbus(tripletList, ac, id_me_to_solver, sn_mva_);
     storages_.fillYbus(tripletList, ac, id_me_to_solver, sn_mva_);
     generators_.fillYbus(tripletList, ac, id_me_to_solver, sn_mva_);
+    dc_lines_.fillYbus(tripletList, ac, id_me_to_solver, sn_mva_);
     res.setFromTriplets(tripletList.begin(), tripletList.end());
     res.makeCompressed();
 }
 
 void GridModel::fillSbus_me(CplxVect & Sbus, bool ac, const std::vector<int>& id_me_to_solver)
 {
     // init the Sbus vector
     powerlines_.fillSbus(Sbus, id_me_to_solver);
     trafos_.fillSbus(Sbus, id_me_to_solver);
     shunts_.fillSbus(Sbus, id_me_to_solver);
     loads_.fillSbus(Sbus, id_me_to_solver);
     sgens_.fillSbus(Sbus, id_me_to_solver);
     storages_.fillSbus(Sbus, id_me_to_solver);
     generators_.fillSbus(Sbus, id_me_to_solver);
-
+    dc_lines_.fillSbus(Sbus, id_me_to_solver);
     if (sn_mva_ != 1.0) Sbus /= sn_mva_;
     // in dc mode, this is used for the phase shifter, this should not be divided by sn_mva_ !
     trafos_.hack_Sbus_for_dc_phase_shifter(Sbus, ac, id_me_to_solver);
 }
 
 void GridModel::fillpv_pq(const std::vector<int>& id_me_to_solver,
                           std::vector<int>& id_solver_to_me,
@@ -510,14 +548,15 @@
     powerlines_.fillpv(bus_pv, has_bus_been_added, slack_bus_id_solver, id_me_to_solver);
     shunts_.fillpv(bus_pv, has_bus_been_added, slack_bus_id_solver, id_me_to_solver);
     trafos_.fillpv(bus_pv, has_bus_been_added, slack_bus_id_solver, id_me_to_solver);
     loads_.fillpv(bus_pv, has_bus_been_added, slack_bus_id_solver, id_me_to_solver);
     storages_.fillpv(bus_pv, has_bus_been_added, slack_bus_id_solver, id_me_to_solver);
     sgens_.fillpv(bus_pv, has_bus_been_added, slack_bus_id_solver, id_me_to_solver);
     generators_.fillpv(bus_pv, has_bus_been_added, slack_bus_id_solver, id_me_to_solver);
+    dc_lines_.fillpv(bus_pv, has_bus_been_added, slack_bus_id_solver, id_me_to_solver);
 
     for(int bus_id = 0; bus_id< nb_bus; ++bus_id){
         if(is_in_vect(bus_id, slack_bus_id_solver)) continue;  // slack bus is not PQ either
         if(has_bus_been_added[bus_id]) continue; // a pv bus cannot be PQ
         bus_pq.push_back(bus_id);
         has_bus_been_added[bus_id] = true;  // don't add it a second time
     }
@@ -541,14 +580,16 @@
     sgens_.compute_results(Va, Vm, V, id_me_to_solver, bus_vn_kv_, sn_mva_, ac);
     // for storage units
     storages_.compute_results(Va, Vm, V, id_me_to_solver, bus_vn_kv_, sn_mva_, ac);
     // for shunts
     shunts_.compute_results(Va, Vm, V, id_me_to_solver, bus_vn_kv_, sn_mva_, ac);
     // for prods
     generators_.compute_results(Va, Vm, V, id_me_to_solver, bus_vn_kv_, sn_mva_, ac);
+    // for dclines
+    dc_lines_.compute_results(Va, Vm, V, id_me_to_solver, bus_vn_kv_, sn_mva_, ac);
 
     //handle_slack_bus active power
     CplxVect mismatch;  // power mismatch at each bus (SOLVER BUS !!!)
     RealVect ractive_mismatch;  // not used in dc mode (DO NOT ATTEMPT TO USE IT THERE)
     RealVect active_mismatch;
     if(ac){
         // In AC mode i am not forced to run through all the grid
@@ -564,25 +605,29 @@
         const auto id_slack = slack_bus_id_dc_solver_(0);
         active_mismatch(id_slack) = -Sbus_.real().sum() * sn_mva_;
     }
     generators_.set_p_slack(active_mismatch, id_me_to_solver);
 
     if(ac) ractive_mismatch = mismatch.imag() * sn_mva_;
     // mainly to initialize the Q value of the generators in dc (just fill it with 0.)
-    generators_.set_q(ractive_mismatch, id_me_to_solver, ac);
+    generators_.set_q(ractive_mismatch, id_me_to_solver, ac,
+                      total_gen_per_bus_, total_q_min_per_bus_, total_q_max_per_bus_);
+    dc_lines_.set_q(ractive_mismatch, id_me_to_solver, ac,
+                    total_gen_per_bus_, total_q_min_per_bus_, total_q_max_per_bus_);
 }
 
 void GridModel::reset_results(){
     powerlines_.reset_results();
     shunts_.reset_results();
     trafos_.reset_results();
     loads_.reset_results();
     sgens_.reset_results();
     storages_.reset_results();
     generators_.reset_results();
+    dc_lines_.reset_results();
 }
 
 CplxVect GridModel::dc_pf(const CplxVect & Vinit,
                           int max_iter,  // not used for DC
                           real_type tol  // not used for DC
                           )
 {
@@ -695,14 +740,20 @@
 
 void GridModel::update_gens_p(Eigen::Ref<Eigen::Array<bool, Eigen::Dynamic, Eigen::RowMajor> > has_changed,
                               Eigen::Ref<Eigen::Array<float, Eigen::Dynamic, Eigen::RowMajor> > new_values)
 {
     update_continuous_values(has_changed, new_values, &GridModel::change_p_gen);
 }
 
+void GridModel::update_sgens_p(Eigen::Ref<Eigen::Array<bool, Eigen::Dynamic, Eigen::RowMajor> > has_changed,
+                              Eigen::Ref<Eigen::Array<float, Eigen::Dynamic, Eigen::RowMajor> > new_values)
+{
+    update_continuous_values(has_changed, new_values, &GridModel::change_p_sgen);
+}
+
 void GridModel::update_gens_v(Eigen::Ref<Eigen::Array<bool, Eigen::Dynamic, Eigen::RowMajor> > has_changed,
                               Eigen::Ref<Eigen::Array<float, Eigen::Dynamic, Eigen::RowMajor> > new_values)
 {
     update_continuous_values(has_changed, new_values, &GridModel::change_v_gen);
 }
 
 void GridModel::update_loads_p(Eigen::Ref<Eigen::Array<bool, Eigen::Dynamic, Eigen::RowMajor> > has_changed,
```

### Comparing `LightSim2Grid-0.7.2.dev0/src/KLUSolver.cpp` & `LightSim2Grid-0.7.2.dev1/src/KLUSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/SecurityAnalysis.cpp` & `LightSim2Grid-0.7.2.dev1/src/SecurityAnalysis.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/SparseLUSolver.cpp` & `LightSim2Grid-0.7.2.dev1/src/SparseLUSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev0/src/help_fun_msg.cpp` & `LightSim2Grid-0.7.2.dev1/src/help_fun_msg.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020, RTE (https://www.rte-france.com)
+// Copyright (c) 2020-2023, RTE (https://www.rte-france.com)
 // See AUTHORS.txt
 // This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 // If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 // you can obtain one at http://mozilla.org/MPL/2.0/.
 // SPDX-License-Identifier: MPL-2.0
 // This file is part of LightSim2grid, LightSim2grid implements a c++ backend targeting the Grid2Op platform.
 
@@ -540,59 +540,55 @@
     Retrieve the capacitance (real part) and dielectric conductance (imaginary part)
     (given in pair unit system) of the powerlines or the transformers. 
     
     This is a complex number and is represented by the number `h` in the line model.
 
 )mydelimiter" + DocIterator::line_model;
 
+
+const std::string DocIterator::only_avail_res = R"mydelimiter(
+    
+    .. warning::
+        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
+
+)mydelimiter";
+
 const std::string DocIterator::res_p_mw = R"mydelimiter(
     Get the active production (or consumption) in MW for element of the grid supporting this feature.
 
     For generators (and static generators) it is given following the "generator convention" (positive = power is injected to the grid)
     
     For loads (and storage units) it is given following the "load convention" (positive = power is absorbed from the grid)
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_q_mvar = R"mydelimiter(
     Get the reactive production (or consumption) in MVAr for element of the grid supporting this feature.
 
     For generators (and static generators) it is given following the "generator convention" (positive = power is injected to the grid)
     
     For loads (and storage units) it is given following the "load convention" (positive = power is absorbed from the grid)
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_theta_deg = R"mydelimiter(
     Get the angle of the complex voltage (in degree, not in radian) of the bus at which this object is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_theta_deg"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_v_kv = R"mydelimiter(
     Get the magnitude of the complex voltage (in kV) of the bus at which this object is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_v_kv"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::target_vm_pu = R"mydelimiter(
     Get the voltage magnitude setpoint (in pair unit and NOT in kV) for each element of the grid supporting this feature.
 
     .. warning::
         This is given in "pair unit" (pu) system and not in kilo Volt (kV) !
 
@@ -1054,102 +1050,72 @@
     that the transformer is disconnected.
 
 )mydelimiter";
 
 const std::string DocIterator::res_p_hv_mw = R"mydelimiter(
     Get the active power in MW for at the "hv" side of the transformer. If it is positive it means power is absorbed by the transformer.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_p_lv_mw = R"mydelimiter(
     Get the active power in MW for at the "lv" side of the transformer. If it is positive it means power is absorbed by the transformer.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_q_hv_mvar = R"mydelimiter(
     Get the reactive power in MVAr for at the "hv" side of the transformer. If it is positive it means power is absorbed by the transformer.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_q_lv_mvar = R"mydelimiter(
     Get the reactive power in MVAr for at the "lv" side of the transformer. If it is positive it means power is absorbed by the transformer.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_theta_hv_deg = R"mydelimiter(
     Get the angle of the complex voltage (in degree, not in radian) of the bus at which this "hv" side of the transformer is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_theta_deg"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_theta_lv_deg = R"mydelimiter(
     Get the angle of the complex voltage (in degree, not in radian) of the bus at which this "lv" side of the transformer is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_theta_deg"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_v_hv_kv = R"mydelimiter(
     Get the magnitude of the complex voltage (in kV) of the bus at which this "hv" side of the transformer is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_v_kv"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_v_lv_kv = R"mydelimiter(
     Get the magnitude of the complex voltage (in kV) of the bus at which this "lv" side of the transformer is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_v_kv"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_a_lv_ka = R"mydelimiter(
     Get the current flows (in kA) at the "lv" side of the transformer.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_a_hv_ka = R"mydelimiter(
     Get the current flows (in kA) at the "hv" side of the transformer.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::DataLine = R"mydelimiter(
     This class allows to iterate through the powerlines of the :class:`lightsim2grid.gridmodel.GridModel` easily, as if they were
     in a python list.
 
     Powerlines are modeled as in pandapower and can be represented a the 
     `pandapower lines <https://pandapower.readthedocs.io/en/latest/elements/line.html#electric-model>`_ .
@@ -1237,103 +1203,285 @@
     that the line is disconnected.
 
 )mydelimiter";
 
 const std::string DocIterator::res_p_or_mw = R"mydelimiter(
     Get the active power in MW for at the "or" side of the line. If it is positive it means power is absorbed by the line.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_p_ex_mw = R"mydelimiter(
     Get the active power in MW for at the "ex" side of the line. If it is positive it means power is absorbed by the line.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_q_or_mvar = R"mydelimiter(
     Get the reactive power in MVAr for at the "or" side of the line. If it is positive it means power is absorbed by the line.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_q_ex_mvar = R"mydelimiter(
     Get the reactive power in MVAr for at the "ex" side of the line. If it is positive it means power is absorbed by the line.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_theta_or_deg = R"mydelimiter(
     Get the angle of the complex voltage (in degree, not in radian) of the bus at which this "or" side of the line is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_theta_deg"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_theta_ex_deg = R"mydelimiter(
     Get the angle of the complex voltage (in degree, not in radian) of the bus at which this "ex" side of the line is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_theta_deg"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_v_or_kv = R"mydelimiter(
     Get the magnitude of the complex voltage (in kV) of the bus at which this "or" side of the line is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_v_kv"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_v_ex_kv = R"mydelimiter(
     Get the magnitude of the complex voltage (in kV) of the bus at which this "ex" side of the line is connected.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
     .. note::
         All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_v_kv"
 
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_a_or_ka = R"mydelimiter(
     Get the current flows (in kA) at the "or" side of the line.
 
-    .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
-
-)mydelimiter";
+)mydelimiter" + DocIterator::only_avail_res;
 
 const std::string DocIterator::res_a_ex_ka = R"mydelimiter(
     Get the current flows (in kA) at the "ex" side of the line.
 
+)mydelimiter" + DocIterator::only_avail_res;
+
+
+const std::string DocIterator::DataDCLine = R"mydelimiter(
+    This class allows to iterate through the dc lines of the :class:`lightsim2grid.gridmodel.GridModel` easily, as if they were
+    in a python list.
+
+    DC lines are modeled as in pandapower and can be represented a the 
+    `pandapower dclines <https://pandapower.readthedocs.io/en/latest/elements/dcline.html#electric-model>`_ . Basically
+    a dc line is made of 2 generators (one at each side `or` or `ex`). These
+    two generators are linked together: if one produces xx MW the other one consume yy MW (and there 
+    exists a relation between xx and yy).
+
+    To dive a bit into the modelling, the two underlying generators can be controlled independantly for the voltage
+    setpoint. But they are linked together for their active value. A dc powerline has some losses (both in MW and in 
+    percent) and the formula for computing the power injected / produced by each generator is:
+
+    - if `xx` is positive, then `yy = -1.0 * (xx - loss_mw) * (1.0 - 0.01 * loss_percent)`
+    - if `xx` is negative, then `yy = -1.0 * xx / (1.0 - 0.01 * loss_percent) + loss_mw
+
+    The first formula directly comes from pandapower. The second one ensures that if the direction of the flow is 
+    inverted, then flows should also be inverted (`xx` becomes `yy` and reciprocally).
+
+    Examples
+    --------
+
+    .. code-block:: python
+
+        import grid2op
+        from lightsim2grid import LightSimBackend
+
+        # create a lightsim2grid "gridmodel"
+        env_name = ... # eg. "l2rpn_case14_test"
+        env = grid2op.make(env_name, backend=LightSimBackend())
+        grid_model = env.backend._grid
+
+        # manipulate the dc powerlines (usually there are none...)
+        for dcline in grid_model.get_dclines():
+            # do something with line !
+            dcline.bus_or_id
+
+        print(f"There are {len(grid_model.get_dclines())} lines on the grid.")
+
+        // first_dcline = grid_model.get_dclines()[0]
+
+    You can have a look at :class:`lightsim2grid.elements.DCLineInfo` for properties of these elements.
+
+)mydelimiter";
+
+
+const std::string DocIterator::DCLineInfo = R"mydelimiter(
+    This class represents what you get from retrieving the dc powerlines from :class:`lightsim2grid.elements.DataDCLine`.
+
+    It allows to read information from each dc powerline of the powergrid.
+
+    DC Powerlines have two sides, one is "or" for "origin" and one is "ex" for "extremity" that are connected and linked to each other
+    by some equations.
+
+    For accessing the results, it's basically the same as having two "elements" (so you get two "voltage_magnitude" `res_v_kv`,
+    two "injected power" `res_p_mw` etc.)
+
     .. warning::
-        This feature is only relevant if the results have been computed (for example if a powerflow has successfully run)
+        Data ca only be accessed from this element. You cannot modify (yet) the grid using this class.
+
+    Examples
+    --------
+
+    .. code-block:: python
+
+        import grid2op
+        from lightsim2grid import LightSimBackend
+
+        # create a lightsim2grid "gridmodel"
+        env_name = ... # eg. "l2rpn_case14_test"
+        env = grid2op.make(env_name, backend=LightSimBackend())
+        grid_model = env.backend._grid
+
+        # for powerlines
+        first_line = grid_model.get_dclines()[0]  # first dcline, this is a `DCLineInfo`
+        for dcline in grid_model.get_dclines():
+            # dcline is a `LineInfo`
+            dcline.bus_or_id
+
+    Notes
+    -----
+    DC lines are modeled by two underlying generators.
+    
+    Each of them can be controlled independantly for the voltage setpoint. 
+    
+    But they are linked together for their active value. A dc powerline has some losses (both in MW `loss_mw` and in 
+    percent `loss_percent`) and the formula for computing the power injected / produced by each generator is:
+
+    - if `xx` is positive, then `yy = -1.0 * (xx - loss_mw) * (1.0 - 0.01 * loss_percent)`
+    - if `xx` is negative, then `yy = -1.0 * xx / (1.0 - 0.01 * loss_percent) + loss_mw
+
+    The first formula directly comes from pandapower. The second one ensures that if the direction of the flow is 
+    inverted, then flows should also be inverted (`xx` becomes `yy` and reciprocally).
+
+    For the sake of simplicity, you can only control the active value at the `or` side of the dc powerline. The
+    active value at the `ex` side 
+)mydelimiter";
+
+const std::string DocIterator::target_p_or_mw = R"mydelimiter(
+    The target active production setpoint at the `or` side of the dc powerline (in MW).
+
+    .. note:: 
+        If it's positive it means that power is actually injected at the `or` side, so the
+        power flows from `ex` to `or`.
+        
+)mydelimiter";
+
+const std::string DocIterator::target_vm_or_pu = R"mydelimiter(
+    The target active voltage setpoint at the `or` side of the powerline (in pu NOT in kV).
+)mydelimiter";
+
+const std::string DocIterator::target_vm_ex_pu = R"mydelimiter(
+    The target active voltage setpoint at the `ex` side of the powerline (in pu NOT in kV).
+)mydelimiter";
+
+const std::string DocIterator::dc_line_formula = R"mydelimiter(
+    .. note::
+        A DC line is modeled by two connected generators and some losses to convert the power from one to the other.
+
+        Two types of losses are considered:
+        
+        - `flat` losses: `loss_mw` (in MW) 
+        - `relative` losses: `loss_percent` (no unit) 
+        
+        The formula for computing the power injected / produced by each generator is:
+
+        - if `or_mw` is positive, then `ex_mw = -1.0 * (or_mw - loss_mw) * (1.0 - 0.01 * loss_percent)`
+        - if `or_mw` is negative, then `ex_mw = -1.0 * or_mw / (1.0 - 0.01 * loss_percent) + loss_mw
+
+        Where `or_mw` denotes the power injected at the origin side and `ex_mw` the power injected at the `extremity`
+        side.
+
+    .. note::
+        By convention, a dc powerline adopts the `load convention`.
+
+        This means that if `or_mw` is positive then power is consumed at the `or` side, so the
+        power flows from `or` to `ex` and vice versa.
 
 )mydelimiter";
 
+const std::string DocIterator::loss_pct = R"mydelimiter(
+    The value of the `loss percent` parameter for the dc line.
+
+)mydelimiter" + DocIterator::dc_line_formula;
+
+const std::string DocIterator::loss_mw = R"mydelimiter(
+    The value of the `loss_mw` parameter for the dc line.
+
+)mydelimiter" + DocIterator::dc_line_formula;
+
+const std::string DocIterator::res_p_or_mw_dcline = R"mydelimiter(
+    The amount of active power injected at the `or` side of the dc powerline (in MW).
+
+)mydelimiter" + DocIterator::only_avail_res + DocIterator::dc_line_formula;
+
+const std::string DocIterator::res_p_ex_mw_dcline = R"mydelimiter(
+    The amount of active power injected at the `ex` side of the dc powerline (in MW).
+
+)mydelimiter" + DocIterator::only_avail_res + DocIterator::dc_line_formula;
+
+const std::string DocIterator::res_q_or_mvar_dcline = R"mydelimiter(
+    The amount of reactive power injected at the `or` side of the dc powerline (in MVAr).
+
+)mydelimiter" + DocIterator::only_avail_res;
+
+const std::string DocIterator::res_q_ex_mvar_dcline = R"mydelimiter(
+    The amount of reactive power injected at the `ex` side of the dc powerline (in MVAr).
+
+)mydelimiter" + DocIterator::only_avail_res;
+
+const std::string DocIterator::res_v_or_kv_dcline = R"mydelimiter(
+    Get the magnitude of the complex voltage (in kV) of the bus at which this "or" side of the dc line is connected.
+
+    .. note::
+        All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_v_kv"
+
+)mydelimiter" + DocIterator::only_avail_res;
+
+const std::string DocIterator::res_v_ex_kv_dcline = R"mydelimiter(
+    Get the magnitude of the complex voltage (in kV) of the bus at which this "ex" side of the dc line is connected.
+
+    .. note::
+        All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_v_kv"
+
+)mydelimiter" + DocIterator::only_avail_res;
+
+const std::string DocIterator::res_theta_or_deg_dcline = R"mydelimiter(
+    Get the angle of the complex voltage (in degree, not in radian) of the bus at which this "or" side of the dc line is connected.
+
+    .. note::
+        All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_theta_deg"
+
+)mydelimiter" + DocIterator::only_avail_res;
+
+const std::string DocIterator::res_theta_ex_deg_dcline = R"mydelimiter(
+    Get the angle of the complex voltage (in degree, not in radian) of the bus at which this "ex" side of the dc line is connected.
+
+    .. note::
+        All elements (load, generators, side of powerline etc.) connected at the same bus have the same "res_theta_deg"
+
+)mydelimiter" + DocIterator::only_avail_res;
+
+const std::string DocIterator::gen_or = R"mydelimiter(
+    Direct access to the "or" generators, directly returns a :class:`lightsim2grid.elements.GenInfo`
+)mydelimiter" + DocIterator::dc_line_formula;
+
+const std::string DocIterator::gen_ex = R"mydelimiter(
+    Direct access to the "ex" generators, directly returns a :class:`lightsim2grid.elements.GenInfo`
+)mydelimiter" + DocIterator::dc_line_formula;
+
 const std::string DocGridModel::GridModel = R"mydelimiter(
     This class represent a lightsim2grid power network. All the elements that can be manipulated by
     lightsim2grid are represented here.
 
     We do not recommend to use this class directly, but rather to use a :class:`lightsim2grid.LightSimBackend.LightSimBackend`.
 
     Examples
@@ -1558,14 +1706,34 @@
         pp_net = ...  # any pandapower grid
         lightsim_grid_model = init(pp_net)  # some warnings might be issued as well as some warnings
 
         # print the target consumption of each loads
         print([el.target_p_mw for el in lightsim_grid_model.get_loads()]) # to print the active consumption for each load
 
 )mydelimiter";
+
+const std::string DocGridModel::get_dclines = R"mydelimiter(
+    This function allows to retrieve the dc powerlines (as a :class:`lightsim2grid.elements.DataDCLine` object,
+    see :ref:`elements-modeled` for more information)
+
+    Examples
+    ---------
+
+    .. code-block:: python
+        
+        # init the grid model
+        from lightsim2grid.gridmodel import init
+        pp_net = ...  # any pandapower grid
+        lightsim_grid_model = init(pp_net)  # some warnings might be issued as well as some warnings
+
+        # usage example: print some information about the powerlines
+        print([el.x_pu for el in lightsim_grid_model.get_dclines()]) # to print the "x" for each powerlines
+
+)mydelimiter";
+
 const std::string DocGridModel::_internal_do_not_use = R"mydelimiter(
         INTERNAL
 
         .. warning:: /!\\ Internal, do not use unless you know what you are doing /!\\
 
         This is used as part of a dedicated code for :class:`lightsim2grid.LightSimBackend.LightSimBackend`
```

### Comparing `LightSim2Grid-0.7.2.dev0/src/main.cpp` & `LightSim2Grid-0.7.2.dev1/src/main.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -411,14 +411,45 @@
         .def_readonly("res_p_ex_mw", &DataLine::LineInfo::res_p_ex_mw, DocIterator::res_p_ex_mw.c_str())
         .def_readonly("res_q_ex_mvar", &DataLine::LineInfo::res_q_ex_mvar, DocIterator::res_q_ex_mvar.c_str())
         .def_readonly("res_v_ex_kv", &DataLine::LineInfo::res_v_ex_kv, DocIterator::res_v_ex_kv.c_str())
         .def_readonly("res_a_ex_ka", &DataLine::LineInfo::res_a_ex_ka, DocIterator::res_a_ex_ka.c_str())
         .def_readonly("res_theta_or_deg", &DataLine::LineInfo::res_theta_or_deg, DocIterator::res_theta_or_deg.c_str())
         .def_readonly("res_theta_ex_deg", &DataLine::LineInfo::res_theta_ex_deg, DocIterator::res_theta_ex_deg.c_str());
 
+    // iterator for dc lines
+    py::class_<DataDCLine>(m, "DataDCLine", DocIterator::DataDCLine.c_str())
+        .def("__len__", [](const DataDCLine & data) { return data.nb(); })
+        .def("__getitem__", [](const DataDCLine & data, int k){return data[k]; } )
+        .def("__iter__", [](const DataDCLine & data) {
+       return py::make_iterator(data.begin(), data.end());
+    }, py::keep_alive<0, 1>()); /* Keep vector alive while iterator is used */
+
+    py::class_<DataDCLine::DCLineInfo>(m, "DCLineInfo", DocIterator::DCLineInfo.c_str())
+        .def_readonly("id", &DataDCLine::DCLineInfo::id, DocIterator::id.c_str())
+        .def_readonly("connected", &DataDCLine::DCLineInfo::connected, DocIterator::connected.c_str())
+        .def_readonly("bus_or_id", &DataDCLine::DCLineInfo::bus_or_id, DocIterator::bus_or_id.c_str())
+        .def_readonly("bus_ex_id", &DataDCLine::DCLineInfo::bus_ex_id, DocIterator::bus_ex_id.c_str())
+        .def_readonly("target_p_or_mw", &DataDCLine::DCLineInfo::target_p_or_mw, DocIterator::target_p_or_mw.c_str())
+        .def_readonly("target_vm_or_pu", &DataDCLine::DCLineInfo::target_vm_or_pu, DocIterator::target_vm_or_pu.c_str())
+        .def_readonly("target_vm_ex_pu", &DataDCLine::DCLineInfo::target_vm_ex_pu, DocIterator::target_vm_ex_pu.c_str())
+        .def_readonly("loss_pct", &DataDCLine::DCLineInfo::loss_pct, DocIterator::loss_pct.c_str())
+        .def_readonly("loss_mw", &DataDCLine::DCLineInfo::loss_mw, DocIterator::loss_mw.c_str())
+        .def_readonly("gen_or", &DataDCLine::DCLineInfo::gen_or, DocIterator::gen_or.c_str())
+        .def_readonly("gen_ex", &DataDCLine::DCLineInfo::gen_ex, DocIterator::gen_ex.c_str())
+        .def_readonly("has_res", &DataDCLine::DCLineInfo::has_res, DocIterator::has_res.c_str())
+        .def_readonly("res_p_or_mw", &DataDCLine::DCLineInfo::res_p_or_mw, DocIterator::res_p_or_mw_dcline.c_str())
+        .def_readonly("res_p_ex_mw", &DataDCLine::DCLineInfo::res_p_ex_mw, DocIterator::res_p_ex_mw_dcline.c_str())
+        .def_readonly("res_q_or_mvar", &DataDCLine::DCLineInfo::res_q_or_mvar, DocIterator::res_q_or_mvar_dcline.c_str())
+        .def_readonly("res_q_ex_mvar", &DataDCLine::DCLineInfo::res_q_ex_mvar, DocIterator::res_q_ex_mvar_dcline.c_str())
+        .def_readonly("res_v_or_kv", &DataDCLine::DCLineInfo::res_v_or_kv, DocIterator::res_v_or_kv_dcline.c_str())
+        .def_readonly("res_v_ex_kv", &DataDCLine::DCLineInfo::res_v_ex_kv, DocIterator::res_v_ex_kv_dcline.c_str())
+        .def_readonly("res_theta_or_deg", &DataDCLine::DCLineInfo::res_theta_or_deg, DocIterator::res_theta_or_deg_dcline.c_str())
+        .def_readonly("res_theta_ex_deg", &DataDCLine::DCLineInfo::res_theta_ex_deg, DocIterator::res_theta_ex_deg_dcline.c_str())
+        ;
+
     // converters
     py::class_<PandaPowerConverter>(m, "PandaPowerConverter")
         .def(py::init<>())
         .def("set_f_hz", &PandaPowerConverter::set_f_hz)
         .def("set_sn_mva", &PandaPowerConverter::set_sn_mva)
         .def("get_line_param", &PandaPowerConverter::get_line_param)
         .def("get_trafo_param", &PandaPowerConverter::get_trafo_param);
@@ -470,19 +501,21 @@
         .def("init_powerlines", &GridModel::init_powerlines, DocGridModel::_internal_do_not_use.c_str())  // TODO code the possibility to add / remove a powerline after creation
         .def("init_shunt", &GridModel::init_shunt, DocGridModel::_internal_do_not_use.c_str())  // same
         .def("init_trafo", &GridModel::init_trafo, DocGridModel::_internal_do_not_use.c_str())  // same 
         .def("init_generators", &GridModel::init_generators, DocGridModel::_internal_do_not_use.c_str())  // same
         .def("init_loads", &GridModel::init_loads, DocGridModel::_internal_do_not_use.c_str())  // same
         .def("init_storages", &GridModel::init_storages, DocGridModel::_internal_do_not_use.c_str())  // same
         .def("init_sgens", &GridModel::init_sgens, DocGridModel::_internal_do_not_use.c_str())  // same
+        .def("init_dclines", &GridModel::init_dclines, DocGridModel::_internal_do_not_use.c_str())  // same
         .def("add_gen_slackbus", &GridModel::add_gen_slackbus, DocGridModel::_internal_do_not_use.c_str()) // same
         .def("remove_gen_slackbus", &GridModel::remove_gen_slackbus, DocGridModel::_internal_do_not_use.c_str())  // same
 
         // inspect the grid
         .def("get_lines", &GridModel::get_lines, DocGridModel::get_lines.c_str())
+        .def("get_dclines", &GridModel::get_dclines, DocGridModel::get_dclines.c_str())
         .def("get_trafos", &GridModel::get_trafos, DocGridModel::get_trafos.c_str())
         .def("get_generators", &GridModel::get_generators, DocGridModel::get_generators.c_str())
         .def("get_static_generators", &GridModel::get_static_generators, DocGridModel::get_static_generators.c_str())
         .def("get_shunts", &GridModel::get_shunts, DocGridModel::get_shunts.c_str())
         .def("get_storages", &GridModel::get_storages, DocGridModel::get_storages.c_str())
         .def("get_loads", &GridModel::get_loads, DocGridModel::get_loads.c_str())
 
@@ -541,14 +574,24 @@
         .def("deactivate_storage", &GridModel::deactivate_storage, DocGridModel::_internal_do_not_use.c_str())
         .def("reactivate_storage", &GridModel::reactivate_storage, DocGridModel::_internal_do_not_use.c_str())
         .def("change_bus_storage", &GridModel::change_bus_storage, DocGridModel::_internal_do_not_use.c_str())
         .def("get_bus_storage", &GridModel::get_bus_storage, DocGridModel::_internal_do_not_use.c_str())
         .def("change_p_storage", &GridModel::change_p_storage, DocGridModel::_internal_do_not_use.c_str())
         .def("change_q_storage", &GridModel::change_q_storage, DocGridModel::_internal_do_not_use.c_str())
 
+        .def("deactivate_dcline", &GridModel::deactivate_dcline, DocGridModel::_internal_do_not_use.c_str())
+        .def("reactivate_dcline", &GridModel::reactivate_dcline, DocGridModel::_internal_do_not_use.c_str())
+        .def("change_p_dcline", &GridModel::change_p_dcline, DocGridModel::_internal_do_not_use.c_str())
+        .def("change_v_or_dcline", &GridModel::change_v_or_dcline, DocGridModel::_internal_do_not_use.c_str())
+        .def("change_v_ex_dcline", &GridModel::change_v_ex_dcline, DocGridModel::_internal_do_not_use.c_str())
+        .def("change_bus_dcline_or", &GridModel::change_bus_dcline_or, DocGridModel::_internal_do_not_use.c_str())
+        .def("change_bus_dcline_ex", &GridModel::change_bus_dcline_ex, DocGridModel::_internal_do_not_use.c_str())
+        .def("get_bus_dcline_or", &GridModel::get_bus_dcline_or, DocGridModel::_internal_do_not_use.c_str())
+        .def("get_bus_dcline_ex", &GridModel::get_bus_dcline_ex, DocGridModel::_internal_do_not_use.c_str())
+
         // get back the results
         .def("get_V", &GridModel::get_V, DocGridModel::get_V.c_str())
         .def("get_Va", &GridModel::get_Va, DocGridModel::get_Va.c_str())
         .def("get_Vm", &GridModel::get_Vm, DocGridModel::get_Vm.c_str())
         .def("get_J", &GridModel::get_J_python, DocGridModel::get_J_python.c_str())
         .def("id_me_to_ac_solver", &GridModel::id_me_to_ac_solver, DocGridModel::id_me_to_ac_solver.c_str())
         .def("id_ac_solver_to_me", &GridModel::id_ac_solver_to_me, DocGridModel::id_ac_solver_to_me.c_str())
@@ -603,14 +646,15 @@
         .def("tell_topo_changed", &GridModel::tell_topo_changed, DocGridModel::_internal_do_not_use.c_str())
         .def("compute_newton", &GridModel::ac_pf, DocGridModel::ac_pf.c_str())
 
          // apply action faster (optimized for grid2op representation)
          // it is not recommended to use it outside of grid2Op.
         .def("update_bus_status", &GridModel::update_bus_status, DocGridModel::_internal_do_not_use.c_str())
         .def("update_gens_p", &GridModel::update_gens_p, DocGridModel::_internal_do_not_use.c_str())
+        .def("update_sgens_p", &GridModel::update_sgens_p, DocGridModel::_internal_do_not_use.c_str())
         .def("update_gens_v", &GridModel::update_gens_v, DocGridModel::_internal_do_not_use.c_str())
         .def("update_loads_p", &GridModel::update_loads_p, DocGridModel::_internal_do_not_use.c_str())
         .def("update_loads_q", &GridModel::update_loads_q, DocGridModel::_internal_do_not_use.c_str())
         .def("update_topo", &GridModel::update_topo, DocGridModel::_internal_do_not_use.c_str())
         .def("update_storages_p", &GridModel::update_storages_p, DocGridModel::_internal_do_not_use.c_str())
 
         // auxiliary functions
```

