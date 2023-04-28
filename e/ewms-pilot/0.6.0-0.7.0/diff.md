# Comparing `tmp/ewms-pilot-0.6.0.tar.gz` & `tmp/ewms-pilot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewms-pilot-0.6.0.tar", last modified: Wed Apr  5 16:57:06 2023, max compression
+gzip compressed data, was "ewms-pilot-0.7.0.tar", last modified: Fri Apr 28 19:47:02 2023, max compression
```

## Comparing `ewms-pilot-0.6.0.tar` & `ewms-pilot-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:57:06.594906 ewms-pilot-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-05 16:57:02.000000 ewms-pilot-0.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2485 2023-04-05 16:57:06.594906 ewms-pilot-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2023-04-05 16:57:02.000000 ewms-pilot-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:57:06.590906 ewms-pilot-0.6.0/ewms_pilot/
--rw-r--r--   0 root         (0) root         (0)      650 2023-04-05 16:57:03.000000 ewms-pilot-0.6.0/ewms_pilot/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-04-05 16:57:02.000000 ewms-pilot-0.6.0/ewms_pilot/config.py
--rw-r--r--   0 root         (0) root         (0)    15500 2023-04-05 16:57:02.000000 ewms-pilot-0.6.0/ewms_pilot/pilot.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:57:02.000000 ewms-pilot-0.6.0/ewms_pilot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:57:06.594906 ewms-pilot-0.6.0/ewms_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2485 2023-04-05 16:57:06.000000 ewms-pilot-0.6.0/ewms_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-04-05 16:57:06.000000 ewms-pilot-0.6.0/ewms_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 16:57:06.000000 ewms-pilot-0.6.0/ewms_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-05 16:57:06.000000 ewms-pilot-0.6.0/ewms_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-05 16:57:06.000000 ewms-pilot-0.6.0/ewms_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1964 2023-04-05 16:57:06.594906 ewms-pilot-0.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-05 16:57:02.000000 ewms-pilot-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 19:47:02.842867 ewms-pilot-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 19:47:02.842867 ewms-pilot-0.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 19:47:02.838867 ewms-pilot-0.7.0/ewms_pilot/
+-rw-r--r--   0 root         (0) root         (0)      650 2023-04-28 19:47:00.000000 ewms-pilot-0.7.0/ewms_pilot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/ewms_pilot/config.py
+-rw-r--r--   0 root         (0) root         (0)    15500 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/ewms_pilot/pilot.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/ewms_pilot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 19:47:02.842867 ewms-pilot-0.7.0/ewms_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-04-28 19:47:02.842867 ewms-pilot-0.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/setup.py
```

### Comparing `ewms-pilot-0.6.0/LICENSE` & `ewms-pilot-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.6.0/PKG-INFO` & `ewms-pilot-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewms-pilot
-Version: 0.6.0
+Version: 0.7.0
 Summary: EWMS Pilot: MQ-Task Interface API
 Home-page: https://github.com/Observation-Management-Service/ewms-pilot
 Download-URL: https://pypi.org/project/ewms-pilot/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/ewms-pilot/issues
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pulsar
 Provides-Extra: rabbitmq
-Provides-Extra: gcp
 Provides-Extra: nats
 Provides-Extra: all
 Provides-Extra: test
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/ewms-pilot)](https://pypi.org/project/ewms-pilot/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Observation-Management-Service/ewms-pilot?include_prereleases)](https://github.com/Observation-Management-Service/ewms-pilot/) [![PyPI - License](https://img.shields.io/pypi/l/ewms-pilot)](https://github.com/Observation-Management-Service/ewms-pilot/blob/main/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/Observation-Management-Service/ewms-pilot)](https://github.com/Observation-Management-Service/ewms-pilot/) [![GitHub issues](https://img.shields.io/github/issues/Observation-Management-Service/ewms-pilot)](https://github.com/Observation-Management-Service/ewms-pilot/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/Observation-Management-Service/ewms-pilot)](https://github.com/Observation-Management-Service/ewms-pilot/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
@@ -39,9 +38,8 @@
 ```
 pip install ewms-pilot[pulsar]
 ```
 
 Options include:
 * pulsar
 * rabbitmq
-* gcp
 * nats
```

### Comparing `ewms-pilot-0.6.0/README.md` & `ewms-pilot-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,8 @@
 ```
 pip install ewms-pilot[pulsar]
 ```
 
 Options include:
 * pulsar
 * rabbitmq
-* gcp
 * nats
```

### Comparing `ewms-pilot-0.6.0/ewms_pilot/__init__.py` & `ewms-pilot-0.7.0/ewms_pilot/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 from .pilot import consume_and_reply, main
 
 __all__ = ["consume_and_reply"]
 
 # version is a human-readable version number.
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
 version_info = (
```

### Comparing `ewms-pilot-0.6.0/ewms_pilot/config.py` & `ewms-pilot-0.7.0/ewms_pilot/config.py`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.6.0/ewms_pilot/pilot.py` & `ewms-pilot-0.7.0/ewms_pilot/pilot.py`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.6.0/ewms_pilot.egg-info/PKG-INFO` & `ewms-pilot-0.7.0/ewms_pilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewms-pilot
-Version: 0.6.0
+Version: 0.7.0
 Summary: EWMS Pilot: MQ-Task Interface API
 Home-page: https://github.com/Observation-Management-Service/ewms-pilot
 Download-URL: https://pypi.org/project/ewms-pilot/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/ewms-pilot/issues
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pulsar
 Provides-Extra: rabbitmq
-Provides-Extra: gcp
 Provides-Extra: nats
 Provides-Extra: all
 Provides-Extra: test
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/ewms-pilot)](https://pypi.org/project/ewms-pilot/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Observation-Management-Service/ewms-pilot?include_prereleases)](https://github.com/Observation-Management-Service/ewms-pilot/) [![PyPI - License](https://img.shields.io/pypi/l/ewms-pilot)](https://github.com/Observation-Management-Service/ewms-pilot/blob/main/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/Observation-Management-Service/ewms-pilot)](https://github.com/Observation-Management-Service/ewms-pilot/) [![GitHub issues](https://img.shields.io/github/issues/Observation-Management-Service/ewms-pilot)](https://github.com/Observation-Management-Service/ewms-pilot/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/Observation-Management-Service/ewms-pilot)](https://github.com/Observation-Management-Service/ewms-pilot/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
@@ -39,9 +38,8 @@
 ```
 pip install ewms-pilot[pulsar]
 ```
 
 Options include:
 * pulsar
 * rabbitmq
-* gcp
 * nats
```

### Comparing `ewms-pilot-0.6.0/setup.cfg` & `ewms-pilot-0.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -57,16 +57,14 @@
 packages = find:
 
 [options.extras_require]
 pulsar = 
 	oms-mqclient[pulsar]
 rabbitmq = 
 	oms-mqclient[rabbitmq]
-gcp = 
-	oms-mqclient[gcp]
 nats = 
 	oms-mqclient[nats]
 all = 
 	oms-mqclient[all]
 test = 
 	asyncstdlib
 	pytest
```

