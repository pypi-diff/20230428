# Comparing `tmp/weconnect-cli-0.9.0.dev1.tar.gz` & `tmp/weconnect-cli-0.9.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weconnect-cli-0.9.0.dev1.tar", last modified: Wed Jun 23 06:52:17 2021, max compression
+gzip compressed data, was "weconnect-cli-0.9.0.dev2.tar", last modified: Thu Jun 24 20:38:03 2021, max compression
```

## Comparing `weconnect-cli-0.9.0.dev1.tar` & `weconnect-cli-0.9.0.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 06:52:17.501634 weconnect-cli-0.9.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-06-23 06:51:52.000000 weconnect-cli-0.9.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7628 2021-06-23 06:52:17.501634 weconnect-cli-0.9.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5870 2021-06-23 06:51:52.000000 weconnect-cli-0.9.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2937 2021-06-23 06:52:17.501634 weconnect-cli-0.9.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-06-23 06:51:52.000000 weconnect-cli-0.9.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 06:52:17.497634 weconnect-cli-0.9.0.dev1/weconnect_cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-23 06:51:52.000000 weconnect-cli-0.9.0.dev1/weconnect_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-06-23 06:51:52.000000 weconnect-cli-0.9.0.dev1/weconnect_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-23 06:51:52.000000 weconnect-cli-0.9.0.dev1/weconnect_cli/__version.py
--rw-r--r--   0 runner    (1001) docker     (121)    14203 2021-06-23 06:51:52.000000 weconnect-cli-0.9.0.dev1/weconnect_cli/weconnect_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 06:52:17.501634 weconnect-cli-0.9.0.dev1/weconnect_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7628 2021-06-23 06:52:17.000000 weconnect-cli-0.9.0.dev1/weconnect_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      370 2021-06-23 06:52:17.000000 weconnect-cli-0.9.0.dev1/weconnect_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-23 06:52:17.000000 weconnect-cli-0.9.0.dev1/weconnect_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-06-23 06:52:17.000000 weconnect-cli-0.9.0.dev1/weconnect_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-06-23 06:52:17.000000 weconnect-cli-0.9.0.dev1/weconnect_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-06-23 06:52:17.000000 weconnect-cli-0.9.0.dev1/weconnect_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:38:03.841675 weconnect-cli-0.9.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-06-24 20:37:42.000000 weconnect-cli-0.9.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7628 2021-06-24 20:38:03.841675 weconnect-cli-0.9.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5870 2021-06-24 20:37:42.000000 weconnect-cli-0.9.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2937 2021-06-24 20:38:03.841675 weconnect-cli-0.9.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-06-24 20:37:42.000000 weconnect-cli-0.9.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:38:03.841675 weconnect-cli-0.9.0.dev2/weconnect_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-24 20:37:42.000000 weconnect-cli-0.9.0.dev2/weconnect_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-06-24 20:37:42.000000 weconnect-cli-0.9.0.dev2/weconnect_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-24 20:37:42.000000 weconnect-cli-0.9.0.dev2/weconnect_cli/__version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14203 2021-06-24 20:37:42.000000 weconnect-cli-0.9.0.dev2/weconnect_cli/weconnect_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:38:03.841675 weconnect-cli-0.9.0.dev2/weconnect_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7628 2021-06-24 20:38:03.000000 weconnect-cli-0.9.0.dev2/weconnect_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2021-06-24 20:38:03.000000 weconnect-cli-0.9.0.dev2/weconnect_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 20:38:03.000000 weconnect-cli-0.9.0.dev2/weconnect_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-06-24 20:38:03.000000 weconnect-cli-0.9.0.dev2/weconnect_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-06-24 20:38:03.000000 weconnect-cli-0.9.0.dev2/weconnect_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-06-24 20:38:03.000000 weconnect-cli-0.9.0.dev2/weconnect_cli.egg-info/top_level.txt
```

### Comparing `weconnect-cli-0.9.0.dev1/LICENSE` & `weconnect-cli-0.9.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `weconnect-cli-0.9.0.dev1/PKG-INFO` & `weconnect-cli-0.9.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weconnect-cli
-Version: 0.9.0.dev1
+Version: 0.9.0.dev2
 Summary: Commandline Interface to interact with the Volkswagen WeConnect Services
 Home-page: https://github.com/tillsteinbach/WeConnect-cli
 Author: Till Steinbach
 License: MIT
 Description: # WeConnect-cli
         [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/tillsteinbach/WeConnect-cli/)
         [![GitHub release (latest by date)](https://img.shields.io/github/v/release/tillsteinbach/WeConnect-cli)](https://github.com/tillsteinbach/WeConnect-cli/releases/latest)
```

### Comparing `weconnect-cli-0.9.0.dev1/README.md` & `weconnect-cli-0.9.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `weconnect-cli-0.9.0.dev1/setup.cfg` & `weconnect-cli-0.9.0.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `weconnect-cli-0.9.0.dev1/setup.py` & `weconnect-cli-0.9.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `weconnect-cli-0.9.0.dev1/weconnect_cli/weconnect_cli.py` & `weconnect-cli-0.9.0.dev2/weconnect_cli/weconnect_cli.py`

 * *Files identical despite different names*

### Comparing `weconnect-cli-0.9.0.dev1/weconnect_cli.egg-info/PKG-INFO` & `weconnect-cli-0.9.0.dev2/weconnect_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weconnect-cli
-Version: 0.9.0.dev1
+Version: 0.9.0.dev2
 Summary: Commandline Interface to interact with the Volkswagen WeConnect Services
 Home-page: https://github.com/tillsteinbach/WeConnect-cli
 Author: Till Steinbach
 License: MIT
 Description: # WeConnect-cli
         [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/tillsteinbach/WeConnect-cli/)
         [![GitHub release (latest by date)](https://img.shields.io/github/v/release/tillsteinbach/WeConnect-cli)](https://github.com/tillsteinbach/WeConnect-cli/releases/latest)
```

