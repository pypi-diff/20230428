# Comparing `tmp/rfswarm-manager-1.1.0.tar.gz` & `tmp/rfswarm-manager-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-manager-1.1.0.tar", last modified: Fri Mar 31 03:19:07 2023, max compression
+gzip compressed data, was "rfswarm-manager-1.1.1.tar", last modified: Fri Apr 28 08:51:30 2023, max compression
```

## Comparing `rfswarm-manager-1.1.0.tar` & `rfswarm-manager-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-31 03:19:07.180688 rfswarm-manager-1.1.0/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-manager-1.1.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3108 2023-03-31 03:19:07.180688 rfswarm-manager-1.1.0/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-03-31 03:05:35.000000 rfswarm-manager-1.1.0/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-31 03:19:07.176688 rfswarm-manager-1.1.0/rfswarm_manager/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-03-31 03:19:06.000000 rfswarm-manager-1.1.0/rfswarm_manager/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)   314437 2023-03-31 03:19:06.000000 rfswarm-manager-1.1.0/rfswarm_manager/rfswarm.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-31 03:19:07.180688 rfswarm-manager-1.1.0/rfswarm_manager.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3108 2023-03-31 03:19:07.000000 rfswarm-manager-1.1.0/rfswarm_manager.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      325 2023-03-31 03:19:07.000000 rfswarm-manager-1.1.0/rfswarm_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-03-31 03:19:07.000000 rfswarm-manager-1.1.0/rfswarm_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      111 2023-03-31 03:19:07.000000 rfswarm-manager-1.1.0/rfswarm_manager.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       78 2023-03-31 03:19:07.000000 rfswarm-manager-1.1.0/rfswarm_manager.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       16 2023-03-31 03:19:07.000000 rfswarm-manager-1.1.0/rfswarm_manager.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1419 2023-03-31 03:19:06.000000 rfswarm-manager-1.1.0/setup-manager.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-03-31 03:19:07.180688 rfswarm-manager-1.1.0/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:30.297140 rfswarm-manager-1.1.1/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-manager-1.1.1/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3108 2023-04-28 08:51:30.297140 rfswarm-manager-1.1.1/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-04-28 08:33:44.000000 rfswarm-manager-1.1.1/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:30.293139 rfswarm-manager-1.1.1/rfswarm_manager/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/rfswarm_manager/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)   314437 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/rfswarm_manager/rfswarm.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:30.297140 rfswarm-manager-1.1.1/rfswarm_manager.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3108 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/rfswarm_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      325 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/rfswarm_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/rfswarm_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      111 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/rfswarm_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       78 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/rfswarm_manager.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       16 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/rfswarm_manager.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1419 2023-04-28 08:51:30.000000 rfswarm-manager-1.1.1/setup-manager.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-04-28 08:51:30.297140 rfswarm-manager-1.1.1/setup.cfg
```

### Comparing `rfswarm-manager-1.1.0/LICENSE` & `rfswarm-manager-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-manager-1.1.0/PKG-INFO` & `rfswarm-manager-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-manager
-Version: 1.1.0
+Version: 1.1.1
 Summary: rfswarm manager
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-manager-1.1.0/README.md` & `rfswarm-manager-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 |Version|Manager|Agent|Reporter|
 |---|---|---|---|
 |[![Latest PyPI version](https://img.shields.io/pypi/v/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Manager PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Agent PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-agent.svg)](https://pypi.python.org/pypi/rfswarm-agent/) | [![Number of Reporter PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-reporter.svg)](https://pypi.python.org/pypi/rfswarm-reporter/) |
 
 | Master | Branch |
 | -- | -- |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.0&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.0&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.1&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.1&label=Regression%20Tests) |
 
 <img align="right" src="Doc/Images/Icon_Information.png">
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
 > _Swarm being the collective noun for Robots, just as Flock is for Birds and Herd for Sheep, so it made sense to use swarm for a performance testing tool using Robot Framework, hence rfswarm_
```

### Comparing `rfswarm-manager-1.1.0/rfswarm_manager/rfswarm.py` & `rfswarm-manager-1.1.1/rfswarm_manager/rfswarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Manager
-#    Version1.1.0"
+#    Version 1.1.1
 #
 
 # 	Helpful links
 #
 #
 
 import argparse
@@ -443,15 +443,15 @@
 	# 	log_request is here to stop BaseHTTPRequestHandler logging to the console
 	# 		https://stackoverflow.com/questions/10651052/how-to-quiet-simplehttpserver/10651257#10651257
 	def log_request(self, code='-', size='-'):
 		pass
 
 
 class RFSwarmBase:
-	version = "1.1.0"
+	version = "1.1.1"
 	debuglvl = 0
 
 	config = None
 	manager_ini = None
 
 	save_ini = True
```

### Comparing `rfswarm-manager-1.1.0/rfswarm_manager.egg-info/PKG-INFO` & `rfswarm-manager-1.1.1/rfswarm_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-manager
-Version: 1.1.0
+Version: 1.1.1
 Summary: rfswarm manager
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-manager-1.1.0/setup-manager.py` & `rfswarm-manager-1.1.1/setup-manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-manager",
-	version="1.1.0",
+	version="1.1.1",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm manager",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_report*", "*fswarm_agen*", "build/*"]),
```

