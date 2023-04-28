# Comparing `tmp/spleaf-2.1.5.tar.gz` & `tmp/spleaf-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleaf-2.1.5.tar", last modified: Tue Apr 18 15:42:22 2023, max compression
+gzip compressed data, was "spleaf-2.1.6.tar", last modified: Fri Apr 28 07:31:59 2023, max compression
```

## Comparing `spleaf-2.1.5.tar` & `spleaf-2.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:22.463487 spleaf-2.1.5/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-04-18 15:41:04.000000 spleaf-2.1.5/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-18 15:41:04.000000 spleaf-2.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      802 2023-04-18 15:42:22.463487 spleaf-2.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-18 15:41:04.000000 spleaf-2.1.5/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:42:22.463487 spleaf-2.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-04-18 15:41:04.000000 spleaf-2.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:22.462487 spleaf-2.1.5/spleaf/
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-18 15:41:04.000000 spleaf-2.1.5/spleaf/__info__.py
--rw-rw-rw-   0 root         (0) root         (0)    29194 2023-04-18 15:41:04.000000 spleaf-2.1.5/spleaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16971 2023-04-18 15:41:04.000000 spleaf-2.1.5/spleaf/cov.py
--rw-rw-rw-   0 root         (0) root         (0)    49962 2023-04-18 15:41:04.000000 spleaf-2.1.5/spleaf/fenrir.py
--rw-rw-rw-   0 root         (0) root         (0)    30205 2023-04-18 15:41:04.000000 spleaf-2.1.5/spleaf/libspleaf.c
--rw-rw-rw-   0 root         (0) root         (0)     4571 2023-04-18 15:41:04.000000 spleaf-2.1.5/spleaf/libspleaf.h
--rw-rw-rw-   0 root         (0) root         (0)    61577 2023-04-18 15:41:04.000000 spleaf-2.1.5/spleaf/pywrapspleaf.c
--rw-rw-rw-   0 root         (0) root         (0)    82399 2023-04-18 15:41:04.000000 spleaf-2.1.5/spleaf/term.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:22.463487 spleaf-2.1.5/spleaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      802 2023-04-18 15:42:22.000000 spleaf-2.1.5/spleaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2023-04-18 15:42:22.000000 spleaf-2.1.5/spleaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:42:22.000000 spleaf-2.1.5/spleaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-18 15:42:22.000000 spleaf-2.1.5/spleaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-18 15:42:22.000000 spleaf-2.1.5/spleaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:22.463487 spleaf-2.1.5/test/
--rw-rw-rw-   0 root         (0) root         (0)    27167 2023-04-18 15:41:04.000000 spleaf-2.1.5/test/test_cov.py
--rw-rw-rw-   0 root         (0) root         (0)    11276 2023-04-18 15:41:04.000000 spleaf-2.1.5/test/test_spleaf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:31:59.355665 spleaf-2.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-04-28 07:30:34.000000 spleaf-2.1.6/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-28 07:30:34.000000 spleaf-2.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      802 2023-04-28 07:31:59.355665 spleaf-2.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-28 07:30:34.000000 spleaf-2.1.6/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 07:31:59.355665 spleaf-2.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-04-28 07:30:34.000000 spleaf-2.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:31:59.354665 spleaf-2.1.6/spleaf/
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-28 07:30:34.000000 spleaf-2.1.6/spleaf/__info__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29194 2023-04-28 07:30:34.000000 spleaf-2.1.6/spleaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16986 2023-04-28 07:30:34.000000 spleaf-2.1.6/spleaf/cov.py
+-rw-rw-rw-   0 root         (0) root         (0)    49962 2023-04-28 07:30:34.000000 spleaf-2.1.6/spleaf/fenrir.py
+-rw-rw-rw-   0 root         (0) root         (0)    30205 2023-04-28 07:30:34.000000 spleaf-2.1.6/spleaf/libspleaf.c
+-rw-rw-rw-   0 root         (0) root         (0)     4571 2023-04-28 07:30:34.000000 spleaf-2.1.6/spleaf/libspleaf.h
+-rw-rw-rw-   0 root         (0) root         (0)    61577 2023-04-28 07:30:34.000000 spleaf-2.1.6/spleaf/pywrapspleaf.c
+-rw-rw-rw-   0 root         (0) root         (0)    82399 2023-04-28 07:30:34.000000 spleaf-2.1.6/spleaf/term.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:31:59.355665 spleaf-2.1.6/spleaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      802 2023-04-28 07:31:59.000000 spleaf-2.1.6/spleaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-28 07:31:59.000000 spleaf-2.1.6/spleaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 07:31:59.000000 spleaf-2.1.6/spleaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-28 07:31:59.000000 spleaf-2.1.6/spleaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 07:31:59.000000 spleaf-2.1.6/spleaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:31:59.355665 spleaf-2.1.6/test/
+-rw-rw-rw-   0 root         (0) root         (0)    27167 2023-04-28 07:30:34.000000 spleaf-2.1.6/test/test_cov.py
+-rw-rw-rw-   0 root         (0) root         (0)    11276 2023-04-28 07:30:34.000000 spleaf-2.1.6/test/test_spleaf.py
```

### Comparing `spleaf-2.1.5/COPYING` & `spleaf-2.1.6/COPYING`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/PKG-INFO` & `spleaf-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleaf
-Version: 2.1.5
+Version: 2.1.6
 Summary: Symmetric S+LEAF matrix.
 Home-page: https://gitlab.unige.ch/jean-baptiste.delisle/spleaf
 Author: Jean-Baptiste Delisle
 Author-email: jean-baptiste.delisle@unige.ch
 License: GPLv3
 Requires-Python: >=3.6
 License-File: COPYING
```

### Comparing `spleaf-2.1.5/README.rst` & `spleaf-2.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/setup.py` & `spleaf-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/spleaf/__info__.py` & `spleaf-2.1.6/spleaf/__info__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 __title__ = 'spleaf'
 __description__ = 'Symmetric S+LEAF matrix.'
 __author__ = 'Jean-Baptiste Delisle'
 __author_email__ = 'jean-baptiste.delisle@unige.ch'
 __license__ = 'GPLv3'
 __url__ = 'https://gitlab.unige.ch/jean-baptiste.delisle/spleaf'
-__version__ = "2.1.5"
+__version__ = "2.1.6"
```

### Comparing `spleaf-2.1.5/spleaf/__init__.py` & `spleaf-2.1.6/spleaf/__init__.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/spleaf/cov.py` & `spleaf-2.1.6/spleaf/cov.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Indices corresponding to each time series in the merged arrays.
   """
 
   n_series = len(list_t)
   list_n = [tk.size for tk in list_t]
   cum_n = np.insert(np.cumsum(list_n), 0, 0)
   full_t = np.hstack(list_t)
-  ksort = np.argsort(full_t)
+  ksort = np.argsort(full_t, kind='stable')
   full_t = full_t[ksort]
   full_args = [np.hstack(arg)[ksort] for arg in args]
   series_index = [
     np.where((ksort >= cum_n[k]) & (ksort < cum_n[k + 1]))[0]
     for k in range(n_series)
   ]
   return (full_t, *full_args, series_index)
```

### Comparing `spleaf-2.1.5/spleaf/fenrir.py` & `spleaf-2.1.6/spleaf/fenrir.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/spleaf/libspleaf.c` & `spleaf-2.1.6/spleaf/libspleaf.c`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/spleaf/libspleaf.h` & `spleaf-2.1.6/spleaf/libspleaf.h`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/spleaf/pywrapspleaf.c` & `spleaf-2.1.6/spleaf/pywrapspleaf.c`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/spleaf/term.py` & `spleaf-2.1.6/spleaf/term.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/spleaf.egg-info/PKG-INFO` & `spleaf-2.1.6/spleaf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleaf
-Version: 2.1.5
+Version: 2.1.6
 Summary: Symmetric S+LEAF matrix.
 Home-page: https://gitlab.unige.ch/jean-baptiste.delisle/spleaf
 Author: Jean-Baptiste Delisle
 Author-email: jean-baptiste.delisle@unige.ch
 License: GPLv3
 Requires-Python: >=3.6
 License-File: COPYING
```

### Comparing `spleaf-2.1.5/test/test_cov.py` & `spleaf-2.1.6/test/test_cov.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.5/test/test_spleaf.py` & `spleaf-2.1.6/test/test_spleaf.py`

 * *Files identical despite different names*

