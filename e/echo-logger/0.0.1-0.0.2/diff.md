# Comparing `tmp/echo_logger-0.0.1.tar.gz` & `tmp/echo_logger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echo_logger-0.0.1.tar", last modified: Fri Apr 28 05:22:20 2023, max compression
+gzip compressed data, was "echo_logger-0.0.2.tar", last modified: Fri Apr 28 05:37:47 2023, max compression
```

## Comparing `echo_logger-0.0.1.tar` & `echo_logger-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 05:22:20.443267 echo_logger-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-04-28 05:16:22.000000 echo_logger-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      618 2023-04-28 05:22:20.442291 echo_logger-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-04-28 05:18:15.000000 echo_logger-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 05:22:20.430269 echo_logger-0.0.1/echo_logger/
--rw-rw-rw-   0        0        0       90 2023-04-28 05:21:08.000000 echo_logger-0.0.1/echo_logger/__init__.py
--rw-rw-rw-   0        0        0     3847 2023-04-28 05:19:56.000000 echo_logger-0.0.1/echo_logger/echo_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:22:20.440269 echo_logger-0.0.1/echo_logger.egg-info/
--rw-rw-rw-   0        0        0      618 2023-04-28 05:22:20.000000 echo_logger-0.0.1/echo_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-28 05:22:20.000000 echo_logger-0.0.1/echo_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 05:22:20.000000 echo_logger-0.0.1/echo_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-28 05:22:20.000000 echo_logger-0.0.1/echo_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 05:22:20.443267 echo_logger-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-04-28 05:10:39.000000 echo_logger-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:37:47.498410 echo_logger-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 05:16:22.000000 echo_logger-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      659 2023-04-28 05:37:47.498410 echo_logger-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-04-28 05:18:15.000000 echo_logger-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 05:37:47.492413 echo_logger-0.0.2/echo_logger/
+-rw-rw-rw-   0        0        0       90 2023-04-28 05:21:08.000000 echo_logger-0.0.2/echo_logger/__init__.py
+-rw-rw-rw-   0        0        0     3847 2023-04-28 05:19:56.000000 echo_logger-0.0.2/echo_logger/echo_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:37:47.497402 echo_logger-0.0.2/echo_logger.egg-info/
+-rw-rw-rw-   0        0        0      659 2023-04-28 05:37:47.000000 echo_logger-0.0.2/echo_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-28 05:37:47.000000 echo_logger-0.0.2/echo_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 05:37:47.000000 echo_logger-0.0.2/echo_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-28 05:37:47.000000 echo_logger-0.0.2/echo_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 05:37:47.499401 echo_logger-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-04-28 05:37:42.000000 echo_logger-0.0.2/setup.py
```

### Comparing `echo_logger-0.0.1/LICENSE` & `echo_logger-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `echo_logger-0.0.1/PKG-INFO` & `echo_logger-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: echo_logger
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple logger for python, with color and time
-Home-page: 
+Home-page: https://github.com/void-echo/echo_logger/
 Author: Echo Void
 Author-email: void-echo@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echo_logger-0.0.1/echo_logger/echo_logger.py` & `echo_logger-0.0.2/echo_logger/echo_logger.py`

 * *Files identical despite different names*

### Comparing `echo_logger-0.0.1/echo_logger.egg-info/PKG-INFO` & `echo_logger-0.0.2/echo_logger.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: echo-logger
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple logger for python, with color and time
-Home-page: 
+Home-page: https://github.com/void-echo/echo_logger/
 Author: Echo Void
 Author-email: void-echo@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echo_logger-0.0.1/setup.py` & `echo_logger-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="echo_logger",
-    version="0.0.1",
+    version="0.0.2",
     author="Echo Void",
     author_email="void-echo@outlook.com",
     description="A simple logger for python, with color and time",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="",
+    url="https://github.com/void-echo/echo_logger/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         ],
 )
```

