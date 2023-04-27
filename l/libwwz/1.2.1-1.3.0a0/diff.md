# Comparing `tmp/libwwz-1.2.1.tar.gz` & `tmp/libwwz-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libwwz-1.2.1.tar", last modified: Wed Feb 23 23:48:14 2022, max compression
+gzip compressed data, was "libwwz-1.3.0a0.tar", last modified: Thu Apr 27 23:27:15 2023, max compression
```

## Comparing `libwwz-1.2.1.tar` & `libwwz-1.3.0a0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-02-23 23:48:14.443319 libwwz-1.2.1/
--rw-r--r--   0 opq       (1000) opq       (1000)    11358 2020-02-14 00:53:05.000000 libwwz-1.2.1/LICENSE.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       25 2022-02-23 23:42:14.000000 libwwz-1.2.1/MANIFEST.in
--rw-rw-r--   0 opq       (1000) opq       (1000)     3770 2022-02-23 23:48:14.443319 libwwz-1.2.1/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)     3433 2022-02-23 23:35:56.000000 libwwz-1.2.1/README.md
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-02-23 23:48:14.442319 libwwz-1.2.1/libwwz/
--rw-rw-r--   0 opq       (1000) opq       (1000)      164 2020-07-31 02:46:27.000000 libwwz-1.2.1/libwwz/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4929 2020-08-17 19:57:59.000000 libwwz-1.2.1/libwwz/plot_methods.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    12894 2020-09-17 01:01:10.000000 libwwz-1.2.1/libwwz/wwz.py
-drwxrwxr-x   0 opq       (1000) opq       (1000)        0 2022-02-23 23:48:14.443319 libwwz-1.2.1/libwwz.egg-info/
--rw-rw-r--   0 opq       (1000) opq       (1000)     3770 2022-02-23 23:48:14.000000 libwwz-1.2.1/libwwz.egg-info/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)      264 2022-02-23 23:48:14.000000 libwwz-1.2.1/libwwz.egg-info/SOURCES.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)        1 2022-02-23 23:48:14.000000 libwwz-1.2.1/libwwz.egg-info/dependency_links.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       24 2022-02-23 23:48:14.000000 libwwz-1.2.1/libwwz.egg-info/requires.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)        7 2022-02-23 23:48:14.000000 libwwz-1.2.1/libwwz.egg-info/top_level.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)      100 2021-11-29 23:28:21.000000 libwwz-1.2.1/requirements.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       38 2022-02-23 23:48:14.443319 libwwz-1.2.1/setup.cfg
--rw-rw-r--   0 opq       (1000) opq       (1000)      848 2022-02-23 23:37:41.000000 libwwz-1.2.1/setup.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:27:15.262549 libwwz-1.3.0a0/
+-rw-r--r--   0 opq       (1000) opq       (1000)    11343 2023-04-27 20:24:49.000000 libwwz-1.3.0a0/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)       25 2022-02-23 23:42:14.000000 libwwz-1.3.0a0/MANIFEST.in
+-rw-r--r--   0 opq       (1000) opq       (1000)    16764 2023-04-27 23:27:15.262549 libwwz-1.3.0a0/PKG-INFO
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3433 2022-02-23 23:35:56.000000 libwwz-1.3.0a0/README.md
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:27:15.261549 libwwz-1.3.0a0/libwwz/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      164 2020-07-31 02:46:27.000000 libwwz-1.3.0a0/libwwz/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4929 2020-08-17 19:57:59.000000 libwwz-1.3.0a0/libwwz/plot_methods.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    12894 2020-09-17 01:01:10.000000 libwwz-1.3.0a0/libwwz/wwz.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:27:15.261549 libwwz-1.3.0a0/libwwz.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    16764 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)      267 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       55 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        7 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      767 2023-04-27 23:24:30.000000 libwwz-1.3.0a0/pyproject.toml
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:27:15.262549 libwwz-1.3.0a0/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:27:15.261549 libwwz-1.3.0a0/tests/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      221 2020-04-09 01:05:12.000000 libwwz-1.3.0a0/tests/test_wwz.py
```

### Comparing `libwwz-1.2.1/LICENSE.txt` & `libwwz-1.3.0a0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright RedVox, Inc. 2023
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `libwwz-1.2.1/PKG-INFO` & `libwwz-1.3.0a0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: libwwz
-Version: 1.2.1
-Summary: Library for computing the weighted wavelet Z transform.
-Home-page: https://github.com/RedVoxInc/libwwz
-Author: RedVox
-Author-email: dev@redvoxsound.com
-License: Apache
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # libwwz
 
 ### Description
 
 This library provides functions for computing the Weighted Wavelet Z-Transform using Python v3.6+.
 
 The code is based on [Foster's](http://adsabs.harvard.edu/full/1996AJ....112.1709F) and [Templeton's](http://adsabs.harvard.edu/full/2004JAVSO..32...41T) Fortran code as well as [eaydin's Python 2.7 WWZ library](https://github.com/eaydin/WWZ). The code is updated to use modern numpy methods and allow for float value tau.
@@ -100,9 +87,7 @@
 Although that way may not be obvious at first unless you're Dutch.
 Now is better than never.
 Although never is often better than *right* now.
 If the implementation is hard to explain, it's a bad idea.
 If the implementation is easy to explain, it may be a good idea.
 Namespaces are one honking great idea -- let's do more of those!
 ```
-
-
```

### Comparing `libwwz-1.2.1/libwwz/plot_methods.py` & `libwwz-1.3.0a0/libwwz/plot_methods.py`

 * *Files identical despite different names*

### Comparing `libwwz-1.2.1/libwwz/wwz.py` & `libwwz-1.3.0a0/libwwz/wwz.py`

 * *Files identical despite different names*

