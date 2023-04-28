# Comparing `tmp/pisces-0.4.0.tar.gz` & `tmp/pisces-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pisces-0.4.0.tar", last modified: Wed Nov 16 23:36:04 2022, max compression
+gzip compressed data, was "pisces-0.4.1.tar", last modified: Fri Apr 28 21:58:59 2023, max compression
```

## Comparing `pisces-0.4.0.tar` & `pisces-0.4.1.tar`

### file list

```diff
@@ -1,47 +1,52 @@
-drwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2022-11-16 23:36:04.000000 pisces-0.4.0/
--rw-r--r--   0 jkmacc    (2081) staff       (20)     2543 2022-11-16 23:36:04.000000 pisces-0.4.0/PKG-INFO
-drwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces/
-drwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces/tables/
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     2080 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/tables/antelope.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)        0 2015-10-09 21:33:40.000000 pisces-0.4.0/pisces/tables/__init__.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)     1891 2015-12-23 17:12:33.000000 pisces-0.4.0/pisces/tables/kbcore.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)     2016 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/tables/css3.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)    22788 2022-11-16 23:12:34.000000 pisces-0.4.0/pisces/util.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     4997 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/client.py
-drwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces/io/
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     1079 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/io/trace.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     1965 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/io/util.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     1997 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/io/mseed.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2015-04-17 03:38:07.000000 pisces-0.4.0/pisces/io/__init__.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     4726 2022-11-16 23:12:34.000000 pisces-0.4.0/pisces/io/readwaveform.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)    28825 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/io/sac.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)    19400 2022-11-16 23:31:39.000000 pisces-0.4.0/pisces/request.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     1028 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/__init__.py
-drwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces/schema/
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)    29149 2022-11-16 23:12:34.000000 pisces-0.4.0/pisces/schema/antelope.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)    15417 2022-11-16 23:12:34.000000 pisces-0.4.0/pisces/schema/util.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2015-10-25 18:48:32.000000 pisces-0.4.0/pisces/schema/__init__.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)    36653 2022-11-16 23:12:34.000000 pisces-0.4.0/pisces/schema/kbcore.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)    31325 2022-11-16 23:12:34.000000 pisces-0.4.0/pisces/schema/css3.py
-drwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces/commands/
--rw-r--r--   0 jkmacc    (2081) staff       (20)      429 2017-12-20 23:00:40.000000 pisces-0.4.0/pisces/commands/create.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)     3351 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/commands/util.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)     3633 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/commands/mseed2db.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)        0 2017-12-20 23:00:40.000000 pisces-0.4.0/pisces/commands/__init__.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     5971 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/commands/sac2db.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)        0 2017-12-20 23:00:40.000000 pisces-0.4.0/pisces/commands/db2db.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     7781 2021-12-17 23:22:19.000000 pisces-0.4.0/pisces/commands/main.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)        0 2017-12-20 23:00:40.000000 pisces-0.4.0/pisces/commands/drop.py
--rw-r--r--   0 jkmacc    (2081) staff       (20)    12524 2022-11-16 23:12:34.000000 pisces-0.4.0/pisces/crud.py
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)      717 2021-12-17 23:22:19.000000 pisces-0.4.0/MANIFEST.in
--rw-r--r--   0 jkmacc    (2081) staff       (20)     1188 2022-11-16 23:12:34.000000 pisces-0.4.0/README.md
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     1860 2022-11-16 23:12:34.000000 pisces-0.4.0/setup.py
-drwxr-xr-x   0 jkmacc    (2081) staff       (20)        0 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces.egg-info/
--rw-r--r--   0 jkmacc    (2081) staff       (20)     2543 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces.egg-info/PKG-INFO
--rw-r--r--   0 jkmacc    (2081) staff       (20)      852 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces.egg-info/SOURCES.txt
--rw-r--r--   0 jkmacc    (2081) staff       (20)       81 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces.egg-info/entry_points.txt
--rw-r--r--   0 jkmacc    (2081) staff       (20)       48 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces.egg-info/requires.txt
--rw-r--r--   0 jkmacc    (2081) staff       (20)        7 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces.egg-info/top_level.txt
--rw-r--r--   0 jkmacc    (2081) staff       (20)        1 2022-11-16 23:36:04.000000 pisces-0.4.0/pisces.egg-info/dependency_links.txt
--rw-r--r--   0 jkmacc    (2081) staff       (20)       38 2022-11-16 23:36:04.000000 pisces-0.4.0/setup.cfg
--rwxr-xr-x   0 jkmacc    (2081) staff       (20)     1687 2015-04-17 03:38:06.000000 pisces-0.4.0/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-04-28 21:58:45.000000 pisces-0.4.1/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-04-28 21:58:45.000000 pisces-0.4.1/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-28 21:58:45.000000 pisces-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-28 21:58:59.545687 pisces-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-28 21:58:45.000000 pisces-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.541687 pisces-0.4.1/pisces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4997 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/pisces/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/db2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/drop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7781 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/mseed2db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/sac2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/crud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/pisces/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/mseed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/readwaveform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28825 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/sac.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1965 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20951 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/pisces/schema/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29149 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/antelope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31325 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/css3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36653 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/kbcore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15417 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/pisces/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/tables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2080 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/tables/antelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/tables/css3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/tables/kbcore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23709 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.541687 pisces-0.4.1/pisces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:58:59.545687 pisces-0.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-04-28 21:58:45.000000 pisces-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-28 21:58:45.000000 pisces-0.4.1/tests/test_readwaveform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8220 2023-04-28 21:58:45.000000 pisces-0.4.1/tests/test_schema_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-28 21:58:45.000000 pisces-0.4.1/tests/test_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pisces-0.4.0/PKG-INFO` & `pisces-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,16 @@
 Metadata-Version: 2.1
 Name: pisces
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Practical Seismological Database Library in Python.
 Home-page: https://github.com/LANL-Seismoacoustics/pisces
+Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.3.2
 Author: Jonathan MacCarthy
 Author-email: jkmacc@lanl.gov
 License: LANL-MIT
-Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.3.2
-Description: # Pisces
-        
-        Pisces is a Python library that connects your geophysical analysis environment
-        to a SQL database that uses the Center for Seismic Studies (CSS) 3.0 or NNSA KB
-        Core table schema.
-        
-        Documentation: <https://lanl-seismoacoustics.github.io/pisces>
-        
-        Repository: <https://github.com/lanl-seismoacoustics/pisces/>
-        
-        ![Build Status](https://github.com/LANL-Seismoacoustics/pisces/workflows/Python%20package/badge.svg?branch=master)
-        
-        
-        ## Features
-        
-        * Import/export waveforms directly to/from your database.  
-        * Build database queries using Python objects and methods
-            ([SQLAlchemy](http:/www.sqlalchemy.org)), not by concatenating SQL strings.
-        * Integration with [ObsPy](http://www.obspy.org).
-        * Geographic filtering of results.
-        
-        
-        ## Installation
-        
-        Requires:
-        
-        * ObsPy
-        * Click
-        * C compiler (for optional `e1` dependency)
-        
-        Install from [PyPI](https://pypi.python.org/pypi):
-        
-        ```
-        pip install pisces
-        ```
-        
-        If you use "e1" format data, you also need to install the `e1` package:
-        
-        ```
-        pip install e1
-        ```
-        
-        You can install them both at the same time with:
-        
-        ```
-        pip install pisces[e1]
-        ```
-        
-        
-        Install current master from GitHub:
-        
-        ```
-        pip install git+https://github.com/LANL-Seismoacoustics/pisces
-        ```
-        
 Keywords: seismology,geophysics,database
 Platform: Mac OS X
 Platform: Linux/Unix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -73,7 +18,64 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 Provides-Extra: e1
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+# Pisces
+
+Pisces is a Python library that connects your geophysical analysis environment
+to a SQL database that uses the Center for Seismic Studies (CSS) 3.0 or NNSA KB
+Core table schema.
+
+Documentation: <https://lanl-seismoacoustics.github.io/pisces>
+
+Repository: <https://github.com/lanl-seismoacoustics/pisces/>
+
+![Build Status](https://github.com/LANL-Seismoacoustics/pisces/workflows/Python%20package/badge.svg?branch=master)
+
+
+## Features
+
+* Import/export waveforms directly to/from your database.  
+* Build database queries using Python objects and methods
+    ([SQLAlchemy](http:/www.sqlalchemy.org)), not by concatenating SQL strings.
+* Integration with [ObsPy](http://www.obspy.org).
+* Geographic filtering of results.
+
+
+## Installation
+
+Requires:
+
+* ObsPy
+* Click
+* C compiler (for optional `e1` dependency)
+
+Install from [PyPI](https://pypi.python.org/pypi):
+
+```
+pip install pisces
+```
+
+If you use "e1" format data, you also need to install the `e1` package:
+
+```
+pip install e1
+```
+
+You can install them both at the same time with:
+
+```
+pip install pisces[e1]
+```
+
+
+Install current master from GitHub:
+
+```
+pip install git+https://github.com/LANL-Seismoacoustics/pisces
+```
```

### Comparing `pisces-0.4.0/pisces/tables/antelope.py` & `pisces-0.4.1/pisces/tables/antelope.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/tables/kbcore.py` & `pisces-0.4.1/pisces/tables/kbcore.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/tables/css3.py` & `pisces-0.4.1/pisces/tables/css3.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/util.py` & `pisces-0.4.1/pisces/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -727,7 +727,41 @@
         m = import_module(module_name)
         tables[table] = getattr(m, class_name)
 
     # put it back
     config['url'] = URL
 
     return session, tables
+
+
+def make_wildcard_list(toList):
+    """
+    Take a list, tuple, or comma separated string of variables and output a list 
+    with sql wildcards '%' and '_'
+
+    Parameters
+    ----------
+    toList : list, tuple, or comma separated string or variables
+
+    Returns
+    -------
+    nowList: list of variables contained in the toList variable
+
+    """
+    
+    # check if toList is a list and if not, make it a list
+    if type(toList) is list:
+        nowList = toList
+        
+    elif type(toList) is tuple:
+        nowList = list(toList)
+        
+    elif type(toList) is str:
+        nowList = toList.split(',')
+    else:
+        raise TypeError('input to function make_wildcard_list is not a list, tuple, or comma separated string of variables')
+            
+    for x in range(len(nowList)):
+       nowList[x] = nowList[x].replace('*','%')
+       nowList[x] = nowList[x].replace('?','_') 
+    
+    return nowList
```

### Comparing `pisces-0.4.0/pisces/client.py` & `pisces-0.4.1/pisces/client.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/io/trace.py` & `pisces-0.4.1/pisces/io/trace.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/io/util.py` & `pisces-0.4.1/pisces/io/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/io/mseed.py` & `pisces-0.4.1/pisces/io/mseed.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/io/readwaveform.py` & `pisces-0.4.1/pisces/io/readwaveform.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/io/sac.py` & `pisces-0.4.1/pisces/io/sac.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/request.py` & `pisces-0.4.1/pisces/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 import numpy as np
 from sqlalchemy import func, or_
 from obspy.core import UTCDateTime, Stream
 import obspy.geodetics as geod
 
 from pisces.io.trace import wfdisc2trace
-
+from pisces.util import make_wildcard_list
 
 def get_wfdisc_rows(session, wfdisc, sta=None, chan=None, t1=None, t2=None,
                     wfids=None, daylong=False, asquery=False, verbose=False):
     """
     Returns a list of wfdisc records from provided SQLAlchemy ORM mapped
     wfdisc table, for given station, channel, and time window combination.
 
@@ -47,17 +47,19 @@
     # seconds in a wfdisc file
     CHUNKSIZE = 24 * 60 * 60
     q = session.query(wfdisc)
     if wfids is not None:
         q = q.filter(wfdisc.wfid.in_(wfids))
     else:
         if sta is not None:
-            q = q.filter(wfdisc.sta == sta)
+            sta = make_wildcard_list(sta)
+            q = q.filter(or_(*[wfdisc.sta.like(stas) for stas in sta]))
         if chan is not None:
-            q = q.filter(wfdisc.chan == chan)
+            chan = make_wildcard_list(chan)
+            q = q.filter(or_(*[wfdisc.chan.like(chans) for chans in chan]))
         if [t1, t2].count(None) == 0:
             q = q.filter(wfdisc.time.between(t1 - CHUNKSIZE, t2))
             q = q.filter(wfdisc.endtime > t1)
         else:
             if t1 is not None:
                 q = q.filter(wfdisc.time >= t1 - CHUNKSIZE)
                 q = q.filter(wfdisc.endtime > t1)
@@ -96,15 +98,15 @@
     Returns
     -------
     list
         Subset of supplied records.
 
     """
     #initial True array to propagate through multiple logical AND comparisons
-    mask0 = np.ones(len(records), dtype=np.bool)
+    mask0 = np.ones(len(records), dtype=bool)
 
     if deg:
         dgen = (geod.locations2degrees(irec.lat, irec.lon, deg[0], deg[1]) \
                 for irec in records)
         degrees = np.fromiter(dgen, dtype=float)
         if deg[2] is not None:
             mask0 = np.logical_and(mask0, deg[2] <= degrees)
@@ -289,15 +291,15 @@
         res = distaz_query(q.all(), deg=deg, km=km, swath=swath)
 
     return res
  
 
 def get_stations(session, site, sitechan=None, affiliation=None, stations=None, 
         channels=None, nets=None, loc=None, region=None, deg=None, km=None, 
-        swath=None, stime=None, asquery=False):
+        swath=None, time_span=None, asquery=False):
     """
     Build common queries for stations.
 
     Parameters
     ----------
     session : sqlalchemy.orm.Session instance
         Must be bound.
@@ -324,14 +326,21 @@
         Azimuth (from North) +/-tolerance from lat,lon point in degrees.
         Currently only works in gnem Oracle.
     asquery : bool, optional
         Return the query object instead of the results.  Default, False.
         Useful if additional you desire additional sorting of filtering, or
         if you have your own in-database geographic query function(s).  If 
         supplied, deg, km, and/or swath are ignored in the returned query.
+    time_span : tuple or list
+        (startdate, enddate) or [startdate, enddate]
+        startdate and enddate are integer julian days of when you want stations (YYYYddd).  
+        If stations were moved one or more times in the time_span, you will 
+        get multiple copies of the station with updated gps values. If you want to be 
+        guaranteed a specific station at a specific time, startdate and enddate must 
+        both be included, even if they are the same.
 
     Notes
     -----
     Each parameter produces an AND clause, list parameters produce IN 
     clauses, a regex produces a REGEXP_LIKE clause (Oracle-specific?).
 
     deg, km, and swath are evaluated out-of-database by evaluating all other 
@@ -356,36 +365,38 @@
     """
     #XXX: remove dependency on func.regexp_like
     Site = site
     Sitechan = sitechan
     Affiliation = affiliation
 
     d = deg
-    t = stime
-
+    
     q = session.query(Site)
-
+    
     if stations:
-        q = q.filter(Site.sta.in_(stations))
-
+        stations = make_wildcard_list(stations)
+        q = q.filter(or_(*[Site.sta.like(stas) for stas in stations]))
+        
     if nets:
+        nets = make_wildcard_list(nets)
         q = q.join(Affiliation, Affiliation.sta==Site.sta)
-        if isinstance(nets, list):
-            q = q.filter(Affiliation.net.in_(nets))
-        else:
-            q = q.filter(func.regexp_like(Affiliation.net, nets))
+        q = q.filter(or_(*[Affiliation.net.like(net) for net in nets]))
 
     if channels:
+        channels = make_wildcard_list(channels)
         q = q.join(Sitechan, Sitechan.sta==Site.sta)
-        if isinstance(channels, str):
-            #interpret string as regexp
-            q = q.filter(func.regexp_like(Sitechan.chan, channnels))
-        else:
-            q = q.filter(Sitechan.chan.in_(channels))
-    
+        q = q.filter(or_(*[Sitechan.chan.like(chans) for chans in channels]))
+
+    if time_span:
+        start_date, end_date = time_span  # start and end days of time period to get stations from
+        if start_date is not None:
+            q = q.filter(Site.ondate <= start_date)
+        if end_date is not None:
+            q = q.filter(Site.offdate >= end_date)
+
     q = geographic_query(q, Site, region=region, asquery=True)
 
     if asquery:
         res = q
     else:
         res = distaz_query(q.all(), deg=deg, km=km, swath=swath)
 
@@ -432,21 +443,24 @@
     Assoc = assoc
 
     t = atime
 
     q = session.query(Arrival)
 
     if stations:
-        q = q.filter(Arrival.sta.in_(stations))
+        stations = make_wildcard_list(stations)
+        q = q.filter(or_(*[Arrival.sta.like(stas) for stas in stations]))
 
     if channels:
-        q = q.filter(Arrival.chan.in_(channels))
+        channels = make_wildcard_list(channels)
+        q = q.filter(or_(*[Arrival.chan.like(chans) for chans in channels]))
 
     if phases:
-        q = q.filter(Arrival.iphase.in_(phase))
+        phases = make_wildcard_list(phases)
+        q = q.filter(or_(*[Arrival.iphase.like(phase) for phase in phases]))
 
     if t:
         if t.count(None) == 0:
             q = q.filter(Arrival.time.between(t[0], t[1]))
         else:
             if t[0]:
                 q = q.filter(Arrival.time > t[0])
@@ -457,26 +471,27 @@
         q = q.filter(Arrival.arid.in_(arids))
 
     if orids:
         q = q.filter(Arrival.arid == Assoc.arid)
         q = q.filter(Assoc.orid.in_(orids))
 
     if auth:
-        q = q.filter(Arrival.auth.in_(auth))
+        auth = make_wildcard_list(auth)
+        q = q.filter(or_(*[Arrival.auth.like(author) for author in auth]))
 
     if asquery:
         res = q
     else:
         res = q.all()
 
     return res
 
 
 def get_waveforms(session, wfdisc, station=None, channel=None, starttime=None,
-                  endtime=None, wfids=None, tol=None):
+                  endtime=None, wfids=None, tol=None, asquery=False):
     """
     Request waveforms.
 
     Parameters
     ----------
     session : sqlalchemy.orm.Session instance
         Must be bound.
@@ -488,39 +503,47 @@
         Traces will be cut to these times.
     wfids : iterable of int, optional
         Wfdisc wfids.  Obviates the above arguments and just returns full Wfdisc
         row waveforms.
     tol : float
         If provided, a warning is fired if any Trace is not within tol seconds
         of starttime and endtime.
+    asquery : bool, optional
+        Return the query object instead of the results.  Default, False.
+        Useful if additional you desire additional sorting of filtering.
 
     Returns
     -------
     obspy.Stream
         Traces are merged and cut to requested times.
 
     """
     # TODO: add evids= option?, use with stawin= option in .execute method?
     # TODO: implement get_arrivals if arrivals=True
     Wfdisc = wfdisc
 
-    st = Stream()
+    # st = Stream()
     if wfids:
         station = channel = starttime = endtime = None
 
     starttime = float(starttime) if starttime is not None else None
     endtime = float(endtime) if endtime is not None else None
 
     t1_utc = UTCDateTime(starttime) if starttime is not None else None
     t2_utc = UTCDateTime(endtime) if endtime is not None else None
 
     wfs = get_wfdisc_rows(session, Wfdisc, station, channel, starttime, endtime,
-                          wfids=wfids)
+                          wfids=wfids, asquery=asquery)
 
-    return wfdisc_rows_to_stream(wfs, t1_utc, t2_utc, tol=tol)
+    if asquery:
+        res = wfs
+    else:
+        res = wfdisc_rows_to_stream(wfs, t1_utc, t2_utc, tol=tol)
+
+    return res
     
 
 def wfdisc_rows_to_stream(wf_rows, start_t, end_t, tol=None):
     """
     Convert wfdisc rows to obspy stream, trim the data to starttime and endtime 
     in the process
 
@@ -542,20 +565,22 @@
         Traces are merged and trimmed to requested times
 
     Raises
     ------
     ValueError:
         Returned Stream contains trace start/end times outside of the tolerance.
     """
-
-    for wf in wfs:
+    st = Stream()
+    
+    for wf in wf_rows:
         try:
             tr = wfdisc2trace(wf)
         except IOError:
             # can't read file
+            # XXX: wow, why the hell would I let unreadable traces slip past
             tr = None
 
         if tr:
             # None utc times will pass through
             tr.trim(start_t, end_t)
             st.append(tr)
             # TODO: do arrival stuff here?
```

### Comparing `pisces-0.4.0/pisces/__init__.py` & `pisces-0.4.1/pisces/__init__.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/schema/antelope.py` & `pisces-0.4.1/pisces/schema/antelope.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/schema/util.py` & `pisces-0.4.1/pisces/schema/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/schema/kbcore.py` & `pisces-0.4.1/pisces/schema/kbcore.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/schema/css3.py` & `pisces-0.4.1/pisces/schema/css3.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/commands/util.py` & `pisces-0.4.1/pisces/commands/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/commands/mseed2db.py` & `pisces-0.4.1/pisces/commands/mseed2db.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/commands/sac2db.py` & `pisces-0.4.1/pisces/commands/sac2db.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/commands/main.py` & `pisces-0.4.1/pisces/commands/main.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/pisces/crud.py` & `pisces-0.4.1/pisces/crud.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/MANIFEST.in` & `pisces-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/README.md` & `pisces-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pisces-0.4.0/setup.py` & `pisces-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 with open('README.md') as readme:
     # https://dustingram.com/articles/2018/03/16/markdown-descriptions-on-pypi
     long_description = readme.read()
 
 doclines = __doc__.split("\n")
 
 setup(name='pisces',
-      version='0.4.0',
+      version='0.4.1',
       description='A Practical Seismological Database Library in Python.',
       long_description=long_description,
       long_description_content_type="text/markdown", # setuptools >= 38.6.0
       author='Jonathan MacCarthy',
       author_email='jkmacc@lanl.gov',
       packages=['pisces','pisces.schema','pisces.io','pisces.tables',
                 'pisces.commands'],
```

### Comparing `pisces-0.4.0/pisces.egg-info/PKG-INFO` & `pisces-0.4.1/pisces.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,16 @@
 Metadata-Version: 2.1
 Name: pisces
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Practical Seismological Database Library in Python.
 Home-page: https://github.com/LANL-Seismoacoustics/pisces
+Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.3.2
 Author: Jonathan MacCarthy
 Author-email: jkmacc@lanl.gov
 License: LANL-MIT
-Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.3.2
-Description: # Pisces
-        
-        Pisces is a Python library that connects your geophysical analysis environment
-        to a SQL database that uses the Center for Seismic Studies (CSS) 3.0 or NNSA KB
-        Core table schema.
-        
-        Documentation: <https://lanl-seismoacoustics.github.io/pisces>
-        
-        Repository: <https://github.com/lanl-seismoacoustics/pisces/>
-        
-        ![Build Status](https://github.com/LANL-Seismoacoustics/pisces/workflows/Python%20package/badge.svg?branch=master)
-        
-        
-        ## Features
-        
-        * Import/export waveforms directly to/from your database.  
-        * Build database queries using Python objects and methods
-            ([SQLAlchemy](http:/www.sqlalchemy.org)), not by concatenating SQL strings.
-        * Integration with [ObsPy](http://www.obspy.org).
-        * Geographic filtering of results.
-        
-        
-        ## Installation
-        
-        Requires:
-        
-        * ObsPy
-        * Click
-        * C compiler (for optional `e1` dependency)
-        
-        Install from [PyPI](https://pypi.python.org/pypi):
-        
-        ```
-        pip install pisces
-        ```
-        
-        If you use "e1" format data, you also need to install the `e1` package:
-        
-        ```
-        pip install e1
-        ```
-        
-        You can install them both at the same time with:
-        
-        ```
-        pip install pisces[e1]
-        ```
-        
-        
-        Install current master from GitHub:
-        
-        ```
-        pip install git+https://github.com/LANL-Seismoacoustics/pisces
-        ```
-        
 Keywords: seismology,geophysics,database
 Platform: Mac OS X
 Platform: Linux/Unix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -73,7 +18,64 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 Provides-Extra: e1
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+# Pisces
+
+Pisces is a Python library that connects your geophysical analysis environment
+to a SQL database that uses the Center for Seismic Studies (CSS) 3.0 or NNSA KB
+Core table schema.
+
+Documentation: <https://lanl-seismoacoustics.github.io/pisces>
+
+Repository: <https://github.com/lanl-seismoacoustics/pisces/>
+
+![Build Status](https://github.com/LANL-Seismoacoustics/pisces/workflows/Python%20package/badge.svg?branch=master)
+
+
+## Features
+
+* Import/export waveforms directly to/from your database.  
+* Build database queries using Python objects and methods
+    ([SQLAlchemy](http:/www.sqlalchemy.org)), not by concatenating SQL strings.
+* Integration with [ObsPy](http://www.obspy.org).
+* Geographic filtering of results.
+
+
+## Installation
+
+Requires:
+
+* ObsPy
+* Click
+* C compiler (for optional `e1` dependency)
+
+Install from [PyPI](https://pypi.python.org/pypi):
+
+```
+pip install pisces
+```
+
+If you use "e1" format data, you also need to install the `e1` package:
+
+```
+pip install e1
+```
+
+You can install them both at the same time with:
+
+```
+pip install pisces[e1]
+```
+
+
+Install current master from GitHub:
+
+```
+pip install git+https://github.com/LANL-Seismoacoustics/pisces
+```
```

### Comparing `pisces-0.4.0/pisces.egg-info/SOURCES.txt` & `pisces-0.4.1/pisces.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+AUTHORS.rst
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 pisces/__init__.py
 pisces/client.py
 pisces/crud.py
@@ -31,8 +32,11 @@
 pisces/schema/antelope.py
 pisces/schema/css3.py
 pisces/schema/kbcore.py
 pisces/schema/util.py
 pisces/tables/__init__.py
 pisces/tables/antelope.py
 pisces/tables/css3.py
-pisces/tables/kbcore.py
+pisces/tables/kbcore.py
+tests/test_readwaveform.py
+tests/test_schema_util.py
+tests/test_util.py
```

### Comparing `pisces-0.4.0/LICENSE.txt` & `pisces-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

