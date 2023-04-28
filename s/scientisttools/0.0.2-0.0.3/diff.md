# Comparing `tmp/scientisttools-0.0.2.tar.gz` & `tmp/scientisttools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientisttools-0.0.2.tar", last modified: Thu Apr 27 20:44:14 2023, max compression
+gzip compressed data, was "scientisttools-0.0.3.tar", last modified: Fri Apr 28 00:33:05 2023, max compression
```

## Comparing `scientisttools-0.0.2.tar` & `scientisttools-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 20:44:14.921207 scientisttools-0.0.2/
--rw-rw-rw-   0        0        0     1100 2023-04-25 22:01:46.000000 scientisttools-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      560 2023-04-27 20:44:14.920206 scientisttools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-04-27 20:32:38.000000 scientisttools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 20:44:14.920206 scientisttools-0.0.2/scientisttools.egg-info/
--rw-rw-rw-   0        0        0      560 2023-04-27 20:44:14.000000 scientisttools-0.0.2/scientisttools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-04-27 20:44:14.000000 scientisttools-0.0.2/scientisttools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 20:44:14.000000 scientisttools-0.0.2/scientisttools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-27 20:44:14.000000 scientisttools-0.0.2/scientisttools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 20:44:14.000000 scientisttools-0.0.2/scientisttools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 20:44:14.922206 scientisttools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      941 2023-04-27 20:33:16.000000 scientisttools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:33:05.391162 scientisttools-0.0.3/
+-rw-rw-rw-   0        0        0    44106 2023-04-11 23:13:24.000000 scientisttools-0.0.3/Data_Methodes_Factorielles.xlsx
+-rw-rw-rw-   0        0        0     1100 2023-04-25 22:01:46.000000 scientisttools-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      560 2023-04-28 00:33:05.390157 scientisttools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1124 2023-04-28 00:32:05.000000 scientisttools-0.0.3/README.md
+-rw-rw-rw-   0        0        0   120528 2023-04-27 22:01:37.000000 scientisttools-0.0.3/ca_example.ipynb
+-rw-rw-rw-   0        0        0   407271 2023-04-27 23:57:57.000000 scientisttools-0.0.3/ca_example2.ipynb
+-rw-rw-rw-   0        0        0  5058787 2023-04-27 23:57:44.000000 scientisttools-0.0.3/classic_mds.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-28 00:33:05.355775 scientisttools-0.0.3/dist/
+-rw-rw-rw-   0        0        0     2216 2023-04-27 20:44:15.000000 scientisttools-0.0.3/dist/scientisttools-0.0.2-py3-none-any.whl
+-rw-rw-rw-   0        0        0     2436 2023-04-27 20:44:14.000000 scientisttools-0.0.3/dist/scientisttools-0.0.2.tar.gz
+-rw-rw-rw-   0        0        0   299931 2023-04-28 00:08:17.000000 scientisttools-0.0.3/efa_example.ipynb
+-rw-rw-rw-   0        0        0   917813 2023-04-28 00:13:14.000000 scientisttools-0.0.3/famd_example.ipynb
+-rw-rw-rw-   0        0        0   483619 2023-04-27 16:32:34.000000 scientisttools-0.0.3/ggcorrplot.ipynb
+-rw-rw-rw-   0        0        0   578076 2023-04-28 00:26:39.000000 scientisttools-0.0.3/mca_example.ipynb
+-rw-rw-rw-   0        0        0    46431 2023-04-28 00:27:27.000000 scientisttools-0.0.3/mds_example.ipynb
+-rw-rw-rw-   0        0        0   609316 2023-04-28 00:28:49.000000 scientisttools-0.0.3/partial_pca.ipynb
+-rw-rw-rw-   0        0        0  1375939 2023-04-28 00:29:54.000000 scientisttools-0.0.3/pca_example.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-28 00:33:05.367775 scientisttools-0.0.3/scientisttools/
+-rw-rw-rw-   0        0        0       48 2023-04-27 22:47:24.000000 scientisttools-0.0.3/scientisttools/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:02:28.000000 scientisttools-0.0.3/scientisttools/clustering.py
+-rw-rw-rw-   0        0        0        2 2023-04-27 23:32:54.000000 scientisttools-0.0.3/scientisttools/dashboard.py
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:01:32.000000 scientisttools-0.0.3/scientisttools/datasets.py
+-rw-rw-rw-   0        0        0   138113 2023-04-27 23:50:14.000000 scientisttools-0.0.3/scientisttools/decomposition.py
+-rw-rw-rw-   0        0        0     4154 2023-04-27 22:59:10.000000 scientisttools-0.0.3/scientisttools/discriminant_analysis.py
+-rw-rw-rw-   0        0        0    71182 2023-04-28 00:11:41.000000 scientisttools-0.0.3/scientisttools/extractfactor.py
+-rw-rw-rw-   0        0        0     7549 2023-04-27 23:47:35.000000 scientisttools-0.0.3/scientisttools/ggcorrplot.py
+-rw-rw-rw-   0        0        0     4596 2023-04-27 23:46:51.000000 scientisttools-0.0.3/scientisttools/ggplot.py
+-rw-rw-rw-   0        0        0    19103 2023-04-27 23:54:32.000000 scientisttools-0.0.3/scientisttools/manifold.py
+-rw-rw-rw-   0        0        0    82030 2023-04-27 23:20:52.000000 scientisttools-0.0.3/scientisttools/pyplot.py
+-rw-rw-rw-   0        0        0    20198 2023-04-27 23:29:04.000000 scientisttools-0.0.3/scientisttools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:33:05.388775 scientisttools-0.0.3/scientisttools.egg-info/
+-rw-rw-rw-   0        0        0      560 2023-04-28 00:33:04.000000 scientisttools-0.0.3/scientisttools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-28 00:33:05.000000 scientisttools-0.0.3/scientisttools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 00:33:04.000000 scientisttools-0.0.3/scientisttools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-28 00:33:04.000000 scientisttools-0.0.3/scientisttools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 00:33:04.000000 scientisttools-0.0.3/scientisttools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 00:33:05.391162 scientisttools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-04-28 00:30:00.000000 scientisttools-0.0.3/setup.py
+-rw-rw-rw-   0        0        0    13039 2023-04-27 20:17:21.000000 scientisttools-0.0.3/utils.ipynb
```

### Comparing `scientisttools-0.0.2/LICENSE.txt` & `scientisttools-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scientisttools-0.0.2/PKG-INFO` & `scientisttools-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientisttools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for multidimensional analysis
 Home-page: UNKNOWN
 Author: Duverier DJIFACK ZEBAZE
 Author-email: duverierdjifack@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scientisttools-0.0.2/scientisttools.egg-info/PKG-INFO` & `scientisttools-0.0.3/scientisttools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientisttools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for multidimensional analysis
 Home-page: UNKNOWN
 Author: Duverier DJIFACK ZEBAZE
 Author-email: duverierdjifack@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scientisttools-0.0.2/setup.py` & `scientisttools-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Python library for multidimensional analysis'
 LONG_DESCRIPTION = 'A python package dedicated to multivariate Exploratory Data Analysis'
 
 # Setting up
 setup(
     name="scientisttools",
     version=VERSION,
```

