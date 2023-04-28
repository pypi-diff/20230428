# Comparing `tmp/rils-rols-1.0.tar.gz` & `tmp/rils-rols-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rils-rols-1.0.tar", last modified: Fri Apr 28 07:21:39 2023, max compression
+gzip compressed data, was "dist\rils-rols-1.1.tar", last modified: Fri Apr 28 07:27:13 2023, max compression
```

## Comparing `rils-rols-1.0.tar` & `rils-rols-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:21:39.819861 rils-rols-1.0/
--rw-rw-rw-   0        0        0     1079 2022-08-30 22:23:15.000000 rils-rols-1.0/LICENSE
--rw-rw-rw-   0        0        0     2663 2023-04-28 07:21:39.819861 rils-rols-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-28 07:21:39.814861 rils-rols-1.0/rils_rols/
--rw-rw-rw-   0        0        0        0 2022-12-22 15:10:42.000000 rils-rols-1.0/rils_rols/__init__.py
--rw-rw-rw-   0        0        0    18211 2023-04-11 12:16:34.000000 rils-rols-1.0/rils_rols/node.py
--rw-rw-rw-   0        0        0    29033 2023-04-28 07:11:52.000000 rils-rols-1.0/rils_rols/rils_rols.py
--rw-rw-rw-   0        0        0     3633 2023-04-28 06:53:21.000000 rils-rols-1.0/rils_rols/rils_rols_ensemble.py
--rw-rw-rw-   0        0        0    11918 2023-04-11 12:16:34.000000 rils-rols-1.0/rils_rols/solution.py
--rw-rw-rw-   0        0        0     2627 2023-04-07 12:50:36.000000 rils-rols-1.0/rils_rols/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:21:39.818861 rils-rols-1.0/rils_rols.egg-info/
--rw-rw-rw-   0        0        0     2663 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 07:21:39.820861 rils-rols-1.0/setup.cfg
--rw-rw-rw-   0        0        0      885 2023-04-27 11:53:59.000000 rils-rols-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:27:13.969534 rils-rols-1.1/
+-rw-rw-rw-   0        0        0     1079 2022-08-30 22:23:15.000000 rils-rols-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2663 2023-04-28 07:27:13.968534 rils-rols-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-28 07:27:13.962534 rils-rols-1.1/rils_rols/
+-rw-rw-rw-   0        0        0        0 2022-12-22 15:10:42.000000 rils-rols-1.1/rils_rols/__init__.py
+-rw-rw-rw-   0        0        0    18211 2023-04-11 12:16:34.000000 rils-rols-1.1/rils_rols/node.py
+-rw-rw-rw-   0        0        0    29033 2023-04-28 07:11:52.000000 rils-rols-1.1/rils_rols/rils_rols.py
+-rw-rw-rw-   0        0        0     3633 2023-04-28 06:53:21.000000 rils-rols-1.1/rils_rols/rils_rols_ensemble.py
+-rw-rw-rw-   0        0        0    11918 2023-04-11 12:16:34.000000 rils-rols-1.1/rils_rols/solution.py
+-rw-rw-rw-   0        0        0     2627 2023-04-07 12:50:36.000000 rils-rols-1.1/rils_rols/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:27:13.967534 rils-rols-1.1/rils_rols.egg-info/
+-rw-rw-rw-   0        0        0     2663 2023-04-28 07:27:13.000000 rils-rols-1.1/rils_rols.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-04-28 07:27:13.000000 rils-rols-1.1/rils_rols.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:27:13.000000 rils-rols-1.1/rils_rols.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-28 07:27:13.000000 rils-rols-1.1/rils_rols.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 07:27:13.000000 rils-rols-1.1/rils_rols.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:27:13.969534 rils-rols-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      885 2023-04-28 07:27:07.000000 rils-rols-1.1/setup.py
```

### Comparing `rils-rols-1.0/LICENSE` & `rils-rols-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rils-rols-1.0/PKG-INFO` & `rils-rols-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rils-rols
-Version: 1.0
+Version: 1.1
 Summary: RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares
 Home-page: https://github.com/kartelj/rils-rols
 Author: Aleksandar Kartelj, Marko Đukanović
 Author-email: aleksandar.kartelj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rils-rols-1.0/rils_rols/node.py` & `rils-rols-1.1/rils_rols/node.py`

 * *Files identical despite different names*

### Comparing `rils-rols-1.0/rils_rols/rils_rols.py` & `rils-rols-1.1/rils_rols/rils_rols.py`

 * *Files identical despite different names*

### Comparing `rils-rols-1.0/rils_rols/rils_rols_ensemble.py` & `rils-rols-1.1/rils_rols/rils_rols_ensemble.py`

 * *Files identical despite different names*

### Comparing `rils-rols-1.0/rils_rols/solution.py` & `rils-rols-1.1/rils_rols/solution.py`

 * *Files identical despite different names*

### Comparing `rils-rols-1.0/rils_rols/utils.py` & `rils-rols-1.1/rils_rols/utils.py`

 * *Files identical despite different names*

### Comparing `rils-rols-1.0/rils_rols.egg-info/PKG-INFO` & `rils-rols-1.1/rils_rols.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rils-rols
-Version: 1.0
+Version: 1.1
 Summary: RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares
 Home-page: https://github.com/kartelj/rils-rols
 Author: Aleksandar Kartelj, Marko Đukanović
 Author-email: aleksandar.kartelj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rils-rols-1.0/setup.py` & `rils-rols-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='rils-rols',
-    version='1.0',
+    version='1.1',
     description='RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares',
     long_description= long_description,
     long_description_content_type  = "text/markdown",
     author='Aleksandar Kartelj, Marko Đukanović',
     author_email='aleksandar.kartelj@gmail.com',
     url='https://github.com/kartelj/rils-rols',
     packages = find_packages(),
```

