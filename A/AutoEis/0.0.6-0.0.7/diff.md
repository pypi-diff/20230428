# Comparing `tmp/AutoEis-0.0.6.tar.gz` & `tmp/AutoEis-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Personal Document\Studying in Canada\UOT-courses\AutoEis\dist\.tmp-gc3j5e74\AutoEis-0.0.6.tar", last modified: Thu Feb 23 05:23:03 2023, max compression
+gzip compressed data, was "D:\Personal Document\Studying in Canada\UOT-courses\Beta_AutoEis\dist\.tmp-1sxvbsyq\AutoEis-0.0.7.tar", last modified: Fri Apr 28 20:27:06 2023, max compression
```

## Comparing `AutoEis-0.0.6.tar` & `AutoEis-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 05:23:03.790083 AutoEis-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-02-23 05:23:03.701460 AutoEis-0.0.6/AutoEis/
--rw-rw-rw-   0        0        0   158760 2023-02-23 04:16:00.000000 AutoEis-0.0.6/AutoEis/Beta_Demo_AutoEIS.py
--rw-rw-rw-   0        0        0      276 2023-02-23 05:18:40.000000 AutoEis-0.0.6/AutoEis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 05:23:03.719594 AutoEis-0.0.6/AutoEis.egg-info/
--rw-rw-rw-   0        0        0      605 2023-02-23 05:23:03.000000 AutoEis-0.0.6/AutoEis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-02-23 05:23:03.000000 AutoEis-0.0.6/AutoEis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 05:23:03.000000 AutoEis-0.0.6/AutoEis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-02-23 05:23:03.000000 AutoEis-0.0.6/AutoEis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-23 05:23:03.000000 AutoEis-0.0.6/AutoEis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      605 2023-02-23 05:23:03.721629 AutoEis-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       13 2022-07-21 02:14:53.000000 AutoEis-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-02-23 05:23:03.790866 AutoEis-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1582 2023-02-23 05:18:21.000000 AutoEis-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:27:06.898256 AutoEis-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-04-28 20:27:06.881256 AutoEis-0.0.7/AutoEis/
+-rw-rw-rw-   0        0        0    72563 2023-04-28 18:58:01.000000 AutoEis-0.0.7/AutoEis/AutoEIS.py
+-rw-rw-rw-   0        0        0      288 2023-04-28 19:04:43.000000 AutoEis-0.0.7/AutoEis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:27:06.894256 AutoEis-0.0.7/AutoEis.egg-info/
+-rw-rw-rw-   0        0        0      645 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-28 19:52:59.000000 AutoEis-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      645 2023-04-28 20:27:06.897256 AutoEis-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2022-07-21 02:14:53.000000 AutoEis-0.0.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-28 20:17:09.000000 AutoEis-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 20:27:06.898256 AutoEis-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1717 2023-04-28 19:35:47.000000 AutoEis-0.0.7/setup.py
```

### Comparing `AutoEis-0.0.6/setup.py` & `AutoEis-0.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
-DESCRIPTION = 'An Automated EIS analysis packgae'
-LONG_DESCRIPTION = 'A package to perform fully automated EIS analysis based on equivalent circuit models'
+VERSION = '0.0.7'
+DESCRIPTION = 'A demo package to assist EIS analysis by automatically proposing statistically plausible ECM'
+LONG_DESCRIPTION = 'AutoEIS is a novel tool designed to aid EIS analysis by automatically prioritizing statistically optimal ECM by combining evolutionary algorithms and Bayesian inference.'
 
 # Setting up
 setup(
     name="AutoEis",
     version= VERSION,
-    author="Runze zhang, Robert Black, Parisa Karimi, Jason Hattrick-Simpers*",
+    author="Runze zhang, Robert Black, Jason Hattrick-Simpers*",
     author_email="runzee.zhang@mail.utoronto.ca",
     description= DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="",
     packages = find_packages(),
     install_requires = ['matplotlib>=3.3.2',
@@ -27,15 +27,16 @@
                         'pandas>=1.1.3',
                         'impedance>=1.4.0',
                         'regex>=2.2.1',
                         'arviz>=0.12.0',
                         'numpyro>=0.9.1',
                         'dill>=0.3.4',
                         'julia>=0.5.7',
-                        'IPython>=7.19.0'],
-    keywords=['python', 'Electrochemical impedance spectroscopy', 'Fully-automated', 'equivalent circuit models', 'gene-expression programming', 'genetic algorithm'],
+                        'IPython>=7.19.0',
+                        'jax>=0.3.9'],
+    keywords=['Electrochemical impedance spectroscopy', 'equivalent circuit models', 'Bayesian inference', 'evolutionary algorithm'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows :: Windows 10",
     ],
 )
```

