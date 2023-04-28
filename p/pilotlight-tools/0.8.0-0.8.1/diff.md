# Comparing `tmp/pilotlight_tools-0.8.0.tar.gz` & `tmp/pilotlight_tools-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilotlight_tools-0.8.0.tar", last modified: Thu Apr 27 04:08:28 2023, max compression
+gzip compressed data, was "pilotlight_tools-0.8.1.tar", last modified: Fri Apr 28 03:22:50 2023, max compression
```

## Comparing `pilotlight_tools-0.8.0.tar` & `pilotlight_tools-0.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 04:08:28.362133 pilotlight_tools-0.8.0/
--rw-rw-rw-   0        0        0     1087 2023-04-27 04:07:26.000000 pilotlight_tools-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     3766 2023-04-27 04:08:28.362133 pilotlight_tools-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2721 2023-04-27 04:07:26.000000 pilotlight_tools-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 04:08:28.362133 pilotlight_tools-0.8.0/pilotlight_tools/
--rw-rw-rw-   0        0        0        7 2023-04-27 04:08:09.000000 pilotlight_tools-0.8.0/pilotlight_tools/__init__.py
--rw-rw-rw-   0        0        0   105915 2023-04-27 04:07:26.000000 pilotlight_tools-0.8.0/pilotlight_tools/pl_build.py
-drwxrwxrwx   0        0        0        0 2023-04-27 04:08:28.362133 pilotlight_tools-0.8.0/pilotlight_tools.egg-info/
--rw-rw-rw-   0        0        0     3766 2023-04-27 04:08:28.000000 pilotlight_tools-0.8.0/pilotlight_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-27 04:08:28.000000 pilotlight_tools-0.8.0/pilotlight_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 04:08:28.000000 pilotlight_tools-0.8.0/pilotlight_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-27 04:08:28.000000 pilotlight_tools-0.8.0/pilotlight_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       96 2023-04-27 04:08:09.000000 pilotlight_tools-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 04:08:28.362133 pilotlight_tools-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1811 2023-04-27 04:07:26.000000 pilotlight_tools-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:22:50.069007 pilotlight_tools-0.8.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 03:22:09.000000 pilotlight_tools-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     3766 2023-04-28 03:22:50.069007 pilotlight_tools-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2721 2023-04-28 03:22:09.000000 pilotlight_tools-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 03:22:50.069007 pilotlight_tools-0.8.1/pilotlight_tools/
+-rw-rw-rw-   0        0        0        7 2023-04-28 03:22:34.000000 pilotlight_tools-0.8.1/pilotlight_tools/__init__.py
+-rw-rw-rw-   0        0        0   105915 2023-04-28 03:22:09.000000 pilotlight_tools-0.8.1/pilotlight_tools/pl_build.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:22:50.069007 pilotlight_tools-0.8.1/pilotlight_tools.egg-info/
+-rw-rw-rw-   0        0        0     3766 2023-04-28 03:22:50.000000 pilotlight_tools-0.8.1/pilotlight_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-28 03:22:50.000000 pilotlight_tools-0.8.1/pilotlight_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 03:22:50.000000 pilotlight_tools-0.8.1/pilotlight_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-28 03:22:50.000000 pilotlight_tools-0.8.1/pilotlight_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       96 2023-04-28 03:22:34.000000 pilotlight_tools-0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 03:22:50.069007 pilotlight_tools-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1811 2023-04-28 03:22:09.000000 pilotlight_tools-0.8.1/setup.py
```

### Comparing `pilotlight_tools-0.8.0/LICENSE` & `pilotlight_tools-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pilotlight_tools-0.8.0/PKG-INFO` & `pilotlight_tools-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilotlight_tools
-Version: 0.8.0
+Version: 0.8.1
 Summary: Pilot Light Tools
 Home-page: https://github.com/pilot-light/pilotlight
 Author: Jonathan Hoffstadt
 Author-email: pilot_light@yahoo.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pilotlight_tools Version: 0.8.0 Summary: Pilot
+Metadata-Version: 2.1 Name: pilotlight_tools Version: 0.8.1 Summary: Pilot
 Light Tools Home-page: https://github.com/pilot-light/pilotlight Author:
 Jonathan Hoffstadt Author-email: pilot_light@yahoo.com License: MIT Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows :: Windows 10 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pilotlight_tools-0.8.0/README.md` & `pilotlight_tools-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pilotlight_tools-0.8.0/pilotlight_tools/pl_build.py` & `pilotlight_tools-0.8.1/pilotlight_tools/pl_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 ###############################################################################
 #                                  Info                                       #
 ###############################################################################
 
 # very poorly written & dirty system, to be cleaned up later
```

### Comparing `pilotlight_tools-0.8.0/pilotlight_tools.egg-info/PKG-INFO` & `pilotlight_tools-0.8.1/pilotlight_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilotlight-tools
-Version: 0.8.0
+Version: 0.8.1
 Summary: Pilot Light Tools
 Home-page: https://github.com/pilot-light/pilotlight
 Author: Jonathan Hoffstadt
 Author-email: pilot_light@yahoo.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pilotlight-tools Version: 0.8.0 Summary: Pilot
+Metadata-Version: 2.1 Name: pilotlight-tools Version: 0.8.1 Summary: Pilot
 Light Tools Home-page: https://github.com/pilot-light/pilotlight Author:
 Jonathan Hoffstadt Author-email: pilot_light@yahoo.com License: MIT Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows :: Windows 10 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pilotlight_tools-0.8.0/setup.py` & `pilotlight_tools-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from codecs import open
 import os
 
-wip_version = "0.7.1"
+wip_version = "0.8.1"
 
 def version_number():
     """This function reads the version number which is populated by github actions"""
 
     if os.environ.get('READTHEDOCS') == 'True':
         return wip_version
     try:
```

