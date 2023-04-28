# Comparing `tmp/AISimuToolKit-0.1.2.tar.gz` & `tmp/AISimuToolKit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AISimuToolKit-0.1.2.tar", last modified: Thu Apr 27 09:38:00 2023, max compression
+gzip compressed data, was "AISimuToolKit-0.1.3.tar", last modified: Fri Apr 28 03:17:41 2023, max compression
```

## Comparing `AISimuToolKit-0.1.2.tar` & `AISimuToolKit-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.239215 AISimuToolKit-0.1.2/AISimuToolKit/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.2/AISimuToolKit/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.239215 AISimuToolKit-0.1.2/AISimuToolKit/exp/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.243214 AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      450 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/base_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1512 2023-04-24 17:36:09.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/finetune_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1319 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/instruct_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1965 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/probe_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2524 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/reflect_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1866 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/register.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.243214 AISimuToolKit-0.1.2/AISimuToolKit/exp/agents/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/agents/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)    14347 2023-04-27 09:36:08.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/agents/agent.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9023 2023-04-27 08:40:40.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/agents/memory.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     5388 2023-04-25 11:38:16.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/experiment.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.243214 AISimuToolKit-0.1.2/AISimuToolKit/exp/toolkit/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      158 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/toolkit/TimeStep.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/toolkit/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      537 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/toolkit/register.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1309 2023-04-22 12:07:26.000000 AISimuToolKit-0.1.2/AISimuToolKit/exp/toolkit/toolkit.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/AISimuToolKit/model/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.2/AISimuToolKit/model/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1469 2023-04-25 04:36:11.000000 AISimuToolKit-0.1.2/AISimuToolKit/model/embedding.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9662 2023-04-27 09:32:26.000000 AISimuToolKit-0.1.2/AISimuToolKit/model/model.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2106 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.2/AISimuToolKit/model/register.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/AISimuToolKit/store/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.2/AISimuToolKit/store/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     6652 2023-04-22 11:34:15.000000 AISimuToolKit-0.1.2/AISimuToolKit/store/logger.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/AISimuToolKit/utils/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.2/AISimuToolKit/utils/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1559 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.2/AISimuToolKit/utils/utils.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.239215 AISimuToolKit-0.1.2/AISimuToolKit.egg-info/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-27 09:38:00.000000 AISimuToolKit-0.1.2/AISimuToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1209 2023-04-27 09:38:00.000000 AISimuToolKit-0.1.2/AISimuToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        1 2023-04-27 09:38:00.000000 AISimuToolKit-0.1.2/AISimuToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      132 2023-04-27 09:38:00.000000 AISimuToolKit-0.1.2/AISimuToolKit.egg-info/requires.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       19 2023-04-27 09:38:00.000000 AISimuToolKit-0.1.2/AISimuToolKit.egg-info/top_level.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/PKG-INFO
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     8780 2023-04-23 03:13:54.000000 AISimuToolKit-0.1.2/README.md
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       38 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/setup.cfg
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1157 2023-04-27 09:37:51.000000 AISimuToolKit-0.1.2/setup.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/test/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-23 03:13:55.000000 AISimuToolKit-0.1.2/test/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/test/exp/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.2/test/exp/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:38:00.247214 AISimuToolKit-0.1.2/test/exp/agents/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.2/test/exp/agents/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      224 2023-04-24 18:44:21.000000 AISimuToolKit-0.1.2/test/exp/agents/test_agent.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1151 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.2/test/test_experiment.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.519542 AISimuToolKit-0.1.3/
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.439546 AISimuToolKit-0.1.3/AISimuToolKit/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.3/AISimuToolKit/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.443546 AISimuToolKit-0.1.3/AISimuToolKit/exp/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.451546 AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      450 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/base_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1512 2023-04-24 17:36:09.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/finetune_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1319 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/instruct_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1965 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/probe_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2524 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/reflect_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1866 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/register.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.467545 AISimuToolKit-0.1.3/AISimuToolKit/exp/agents/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/agents/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)    14347 2023-04-27 09:36:08.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/agents/agent.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9031 2023-04-27 13:18:27.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/agents/memory.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     5692 2023-04-28 02:34:52.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/experiment.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.475545 AISimuToolKit-0.1.3/AISimuToolKit/exp/toolkit/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      158 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/toolkit/TimeStep.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/toolkit/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      537 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/toolkit/register.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1309 2023-04-22 12:07:26.000000 AISimuToolKit-0.1.3/AISimuToolKit/exp/toolkit/toolkit.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.495544 AISimuToolKit-0.1.3/AISimuToolKit/model/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.3/AISimuToolKit/model/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1469 2023-04-25 04:36:11.000000 AISimuToolKit-0.1.3/AISimuToolKit/model/embedding.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9662 2023-04-27 09:32:26.000000 AISimuToolKit-0.1.3/AISimuToolKit/model/model.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2106 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.3/AISimuToolKit/model/register.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.495544 AISimuToolKit-0.1.3/AISimuToolKit/store/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.3/AISimuToolKit/store/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     6880 2023-04-27 09:49:39.000000 AISimuToolKit-0.1.3/AISimuToolKit/store/logger.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.507543 AISimuToolKit-0.1.3/AISimuToolKit/utils/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.3/AISimuToolKit/utils/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1559 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.3/AISimuToolKit/utils/utils.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.443546 AISimuToolKit-0.1.3/AISimuToolKit.egg-info/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-28 03:17:41.000000 AISimuToolKit-0.1.3/AISimuToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1209 2023-04-28 03:17:41.000000 AISimuToolKit-0.1.3/AISimuToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        1 2023-04-28 03:17:41.000000 AISimuToolKit-0.1.3/AISimuToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      132 2023-04-28 03:17:41.000000 AISimuToolKit-0.1.3/AISimuToolKit.egg-info/requires.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       19 2023-04-28 03:17:41.000000 AISimuToolKit-0.1.3/AISimuToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-28 03:17:41.519542 AISimuToolKit-0.1.3/PKG-INFO
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     8780 2023-04-23 03:13:54.000000 AISimuToolKit-0.1.3/README.md
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       38 2023-04-28 03:17:41.519542 AISimuToolKit-0.1.3/setup.cfg
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1157 2023-04-28 03:16:19.000000 AISimuToolKit-0.1.3/setup.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.507543 AISimuToolKit-0.1.3/test/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-23 03:13:55.000000 AISimuToolKit-0.1.3/test/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.515543 AISimuToolKit-0.1.3/test/exp/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.3/test/exp/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-28 03:17:41.519542 AISimuToolKit-0.1.3/test/exp/agents/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.3/test/exp/agents/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      224 2023-04-24 18:44:21.000000 AISimuToolKit-0.1.3/test/exp/agents/test_agent.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1151 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.3/test/test_experiment.py
```

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/finetune_action.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/finetune_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/instruct_action.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/instruct_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/probe_action.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/probe_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/reflect_action.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/reflect_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/actions/register.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/actions/register.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/agents/agent.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/agents/agent.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/agents/memory.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/agents/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
         memory_series = pd.Series(memory_item)
         memory_df = memory_series.to_frame().T
         self.memory_df = pd.concat([self.memory_df, memory_df], ignore_index=True)
         self.memory_df["recentness"] = pow(0.99, self.curr_id - self.memory_df["id"])
         self.curr_id += 1
         with open(self.memory_path, "a", encoding="utf-8") as f:
-            last_row = self.memory_df.drop(["similarity", "embedding", "recentness", "score"], axis=1)
+            last_row = self.memory_df.drop(["similarity", "embedding", "recentness", "score"], axis=1).tail(1)
             json_object = last_row.to_json(orient='records')
             f.write(json_object[1:-1] + "\n")
 
         # self.export_memory()
 
     def retrieve_by_interactant(self, interactant: str) -> list[dict]:
         """
```

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/experiment.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 class Experiment:
     def __init__(self, id: str, path: str, agents: List[Agent], config: dict):
         self.id = id
         self.path = path
         self.agents = agents
-        # self.models = models
         # 用户传入的config
         self.config = config
 
     def get_agent_ids(self):
         return [agent.agent_id for agent in self.agents]
 
     @classmethod
@@ -130,7 +129,14 @@
         exp_path = os.path.join(output_dir, exp_id)
         os.makedirs(exp_path, exist_ok=True)
 
         # 实例化一个logger，控制文件位置
         logger = Logger(log_file=os.path.join(exp_path, "log.txt"),
                         history_file=os.path.join(exp_path, "history.txt"))
         return exp_path
+
+    def choose_next_one(self, prompt: str = "Choose one agent to continue: ") -> Agent:
+        for agent in self.agents:
+            agent.desire("How strong is your desire to speak? 1 means you don’t want to speak, 10 means you want to "
+                         "speak very much, give a number from 1-10", prompt=prompt)
+
+
```

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/toolkit/register.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/toolkit/register.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/exp/toolkit/toolkit.py` & `AISimuToolKit-0.1.3/AISimuToolKit/exp/toolkit/toolkit.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/model/embedding.py` & `AISimuToolKit-0.1.3/AISimuToolKit/model/embedding.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/model/model.py` & `AISimuToolKit-0.1.3/AISimuToolKit/model/model.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/model/register.py` & `AISimuToolKit-0.1.3/AISimuToolKit/model/register.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/store/logger.py` & `AISimuToolKit-0.1.3/AISimuToolKit/store/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import multiprocessing
 import os
 import threading
+from typing import Union
 
 
 # TODO 加入memory的功能
 class Logger:
     """
     日志记录器，实现了单例模式（线程安全和进程安全）
     日志包括debug、info、warning、error、critical五个级别,
@@ -152,7 +153,15 @@
         self.logger.removeHandler(self.console_handler)
         self.logger.removeHandler(self.log_handler)
         self.logger.addHandler(self.history_handler)
         self.logger.info(message)
         self.logger.removeHandler(self.history_handler)
         self.logger.addHandler(self.log_handler)
         self.logger.addHandler(self.console_handler)
+
+    def set_level(self, level: Union[int, str]):
+        """
+        设置日志记录器的日志级别
+        :param level:
+        :return:
+        """
+        self.logger.setLevel(level)
```

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit/utils/utils.py` & `AISimuToolKit-0.1.3/AISimuToolKit/utils/utils.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/AISimuToolKit.egg-info/SOURCES.txt` & `AISimuToolKit-0.1.3/AISimuToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/README.md` & `AISimuToolKit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.2/setup.py` & `AISimuToolKit-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 setup(
     name="AISimuToolKit",  # 这里是pip项目发布的名称
-    version="0.1.2",  # 版本号，数值大的会优先被pip
+    version="0.1.3",  # 版本号，数值大的会优先被pip
     keywords=["pip", "AISimuToolKit"],  # 关键字
     description="ICIP's private utils.",  # 描述
     long_description="ICIP's private utils. The development version will be released when it is sufficiently refined",
     license="MIT Licence",  # 许可证
     url="http://git.cipsup.cn/aisimulationplatform/toolkit/aisimulation",  # 项目相关文件地址，一般是github项目地址即可
     author="Ren & Guo",  # 作者
     author_email="renmengjie22@mails.ucas.ac.cn,guoshiguang22@mails.ucas.edu.cn",
```

### Comparing `AISimuToolKit-0.1.2/test/test_experiment.py` & `AISimuToolKit-0.1.3/test/test_experiment.py`

 * *Files identical despite different names*

