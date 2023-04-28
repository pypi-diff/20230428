# Comparing `tmp/objectwalker-1.9.5.tar.gz` & `tmp/objectwalker-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectwalker-1.9.5.tar", last modified: Thu Apr 27 19:35:49 2023, max compression
+gzip compressed data, was "objectwalker-2.0.tar", last modified: Fri Apr 28 12:10:26 2023, max compression
```

## Comparing `objectwalker-1.9.5.tar` & `objectwalker-2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:49.281328 objectwalker-1.9.5/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-1.9.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      457 2023-04-27 19:35:49.281328 objectwalker-1.9.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-26 14:54:45.000000 objectwalker-1.9.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:49.277328 objectwalker-1.9.5/objectwalker/
--rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-1.9.5/objectwalker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7898 2023-04-27 19:35:36.000000 objectwalker-1.9.5/objectwalker/__main__.py
--rw-rw-r--   0 root         (0) root         (0)    11371 2023-04-27 18:48:15.000000 objectwalker-1.9.5/objectwalker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:49.281328 objectwalker-1.9.5/objectwalker/filters/
--rw-rw-r--   0 root         (0) root         (0)     1567 2023-04-27 10:44:13.000000 objectwalker-1.9.5/objectwalker/filters/EmptyFilter.py
--rw-rw-r--   0 root         (0) root         (0)     1054 2023-04-27 10:44:18.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectNameContains.py
--rw-rw-r--   0 root         (0) root         (0)     1061 2023-04-27 10:44:22.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectNameEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1044 2023-04-27 10:44:25.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectNameEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1742 2023-04-27 11:37:42.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectNameIsPythonBuiltin.py
--rw-rw-r--   0 root         (0) root         (0)     1073 2023-04-27 10:44:32.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectNameStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1047 2023-04-27 10:44:35.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectValueContains.py
--rw-rw-r--   0 root         (0) root         (0)     1054 2023-04-27 10:44:38.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectValueEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1037 2023-04-27 10:44:41.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectValueEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1066 2023-04-27 10:44:44.000000 objectwalker-1.9.5/objectwalker/filters/FilterObjectValueStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1016 2023-04-27 10:44:47.000000 objectwalker-1.9.5/objectwalker/filters/FilterPathContains.py
--rw-rw-r--   0 root         (0) root         (0)     1023 2023-04-27 10:44:05.000000 objectwalker-1.9.5/objectwalker/filters/FilterPathEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1033 2023-04-27 10:44:53.000000 objectwalker-1.9.5/objectwalker/filters/FilterPathStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      815 2023-04-27 10:35:32.000000 objectwalker-1.9.5/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py
--rw-rw-r--   0 root         (0) root         (0)      762 2023-04-27 10:35:30.000000 objectwalker-1.9.5/objectwalker/filters/FilterTypeIsMethodWrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2544 2023-04-27 10:45:04.000000 objectwalker-1.9.5/objectwalker/filters/FilterTypeIsModule.py
--rw-rw-r--   0 root         (0) root         (0)     1267 2023-04-27 10:23:43.000000 objectwalker-1.9.5/objectwalker/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:49.281328 objectwalker-1.9.5/objectwalker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      457 2023-04-27 19:35:49.000000 objectwalker-1.9.5/objectwalker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1106 2023-04-27 19:35:49.000000 objectwalker-1.9.5/objectwalker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:35:49.000000 objectwalker-1.9.5/objectwalker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-27 19:35:49.000000 objectwalker-1.9.5/objectwalker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 19:35:49.000000 objectwalker-1.9.5/objectwalker.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-1.9.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 19:35:49.281328 objectwalker-1.9.5/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1165 2023-04-27 19:35:40.000000 objectwalker-1.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:10:26.030876 objectwalker-2.0/
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-28 12:10:26.030876 objectwalker-2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-26 14:54:45.000000 objectwalker-2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:10:26.026876 objectwalker-2.0/objectwalker/
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.0/objectwalker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7866 2023-04-28 12:02:50.000000 objectwalker-2.0/objectwalker/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)    11371 2023-04-27 18:48:15.000000 objectwalker-2.0/objectwalker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:10:26.030876 objectwalker-2.0/objectwalker/filters/
+-rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.0/objectwalker/filters/EmptyFilter.py
+-rw-rw-r--   0 root         (0) root         (0)     1049 2023-04-28 10:21:25.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1061 2023-04-27 10:44:22.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1044 2023-04-27 10:44:25.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1742 2023-04-27 11:37:42.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameIsPythonBuiltin.py
+-rw-rw-r--   0 root         (0) root         (0)     1073 2023-04-27 10:44:32.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1047 2023-04-27 10:44:35.000000 objectwalker-2.0/objectwalker/filters/FilterObjectValueContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1054 2023-04-27 10:44:38.000000 objectwalker-2.0/objectwalker/filters/FilterObjectValueEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1037 2023-04-27 10:44:41.000000 objectwalker-2.0/objectwalker/filters/FilterObjectValueEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1066 2023-04-27 10:44:44.000000 objectwalker-2.0/objectwalker/filters/FilterObjectValueStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1016 2023-04-27 10:44:47.000000 objectwalker-2.0/objectwalker/filters/FilterPathContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1023 2023-04-27 10:44:05.000000 objectwalker-2.0/objectwalker/filters/FilterPathEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1033 2023-04-27 10:44:53.000000 objectwalker-2.0/objectwalker/filters/FilterPathStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      815 2023-04-27 10:35:32.000000 objectwalker-2.0/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py
+-rw-rw-r--   0 root         (0) root         (0)      762 2023-04-27 10:35:30.000000 objectwalker-2.0/objectwalker/filters/FilterTypeIsMethodWrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2544 2023-04-27 10:45:04.000000 objectwalker-2.0/objectwalker/filters/FilterTypeIsModule.py
+-rw-rw-r--   0 root         (0) root         (0)     1267 2023-04-27 10:23:43.000000 objectwalker-2.0/objectwalker/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:10:26.030876 objectwalker-2.0/objectwalker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 12:10:26.030876 objectwalker-2.0/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     2490 2023-04-28 12:09:48.000000 objectwalker-2.0/setup.py
```

### Comparing `objectwalker-1.9.5/README.md` & `objectwalker-2.0/README.md`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/__main__.py` & `objectwalker-2.0/objectwalker/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import argparse
 import sys
 import objectwalker
 from objectwalker.filters import *
 
 
-VERSION = "1.9.5"
+VERSION = "2.0"
 
 
 banner = r"""
        ____  __      _           __ _       __      ____            
       / __ \/ /_    (_)__  _____/ /| |     / /___ _/ / /_____  _____
      / / / / __ \  / / _ \/ ___/ __/ | /| / / __ `/ / //_/ _ \/ ___/
     / /_/ / /_/ / / /  __/ /__/ /_ | |/ |/ / /_/ / / ,< /  __/ /      v%s 
@@ -32,15 +32,15 @@
     parser.add_argument("--no-colors", dest="no_colors", action="store_true", default=False, help="No colors mode.")
 
     group_source = parser.add_mutually_exclusive_group(required=True)
     group_source.add_argument("-m", "--module", default=None, type=str, help="Python module to explore.")
 
     # Objects
     group_filters_objects = parser.add_argument_group("Filters on objects")
-    group_filters_objects.add_argument("--filter-object-is-module", default=[], type=str, action="append", help="Show paths from the base object leading to a specific module.")
+    group_filters_objects.add_argument("--filter-module", default=[], type=str, action="append", help="Show paths from the base object leading to a specific module.")
     #
     group_filters_objects.add_argument("--filter-object-name-equals", default=[], type=str, action="append", help="Show paths from the base object leading to an object name equals to <string>.")
     group_filters_objects.add_argument("--filter-object-name-contains", default=[], type=str, action="append", help="Show paths from the base object leading to an object name containing <string>.")
     group_filters_objects.add_argument("--filter-object-name-startswith", default=[], type=str, action="append", help="Show paths from the base object leading to an object name starting with <string>.")
     group_filters_objects.add_argument("--filter-object-name-endswith", default=[], type=str, action="append", help="Show paths from the base object leading to an object name ending with <string>.")
     #
     group_filters_objects.add_argument("--filter-object-value-equals", default=[], type=str, action="append", help="Show paths from the base object leading to an object value equals to <string>.")
@@ -69,16 +69,16 @@
     # Disable colored output if stdout is not a TTY
     if not sys.stdout.isatty():
         options.no_colors = True
 
     filters = []
 
     # Filters on types
-    if len(options.filter_object_is_module) != 0:
-        filters.append(FilterTypeIsModule(modules=options.filter_object_is_module, no_colors=options.no_colors))
+    if len(options.filter_module) != 0:
+        filters.append(FilterTypeIsModule(modules=options.filter_module, no_colors=options.no_colors))
     if options.filter_type_module:
         filters.append(FilterTypeIsModule(no_colors=options.no_colors))
     if options.filter_type_method_wrapper:
         filters.append(FilterTypeIsMethodWrapper(no_colors=options.no_colors))
     if options.filter_type_builtin_function_or_method:
         filters.append(FilterTypeIsBuiltinFunctionOrMethod(no_colors=options.no_colors))
```

### Comparing `objectwalker-1.9.5/objectwalker/core.py` & `objectwalker-2.0/objectwalker/core.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/EmptyFilter.py` & `objectwalker-2.0/objectwalker/filters/EmptyFilter.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 # -*- coding: utf-8 -*-
 # File name          : EmptyFilter.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 class EmptyFilter(object):
     """
-    Documentation for class EmptyFilter
+    class EmptyFilter
+
+    Default filter, matches every path without constraints
     """
 
     no_colors = False
     filter_name = "EmptyFilter"
     callback = None
 
     def __init__(self, no_colors=False):
```

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectNameContains.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectNameContains.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 # Date created       : 26 Apr 2023
 
 from .EmptyFilter import EmptyFilter
 
 
 class FilterObjectNameContains(EmptyFilter):
     """
-    Documentation for class FilterObjectNameContains
+    class FilterObjectNameContains
+
+    Filters
     """
     values = []
     no_colors = False
 
     filter_name = "FilterObjectNameContains"
 
     def __init__(self, values, no_colors=False):
```

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectNameEndsWith.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectNameEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectNameEquals.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectNameEquals.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectNameIsPythonBuiltin.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectNameIsPythonBuiltin.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectNameStartsWith.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectNameStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectValueContains.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectValueContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectValueEndsWith.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectValueEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectValueEquals.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectValueEquals.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterObjectValueStartsWith.py` & `objectwalker-2.0/objectwalker/filters/FilterObjectValueStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterPathContains.py` & `objectwalker-2.0/objectwalker/filters/FilterPathContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterPathEndsWith.py` & `objectwalker-2.0/objectwalker/filters/FilterPathEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterPathStartsWith.py` & `objectwalker-2.0/objectwalker/filters/FilterPathStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py` & `objectwalker-2.0/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterTypeIsMethodWrapper.py` & `objectwalker-2.0/objectwalker/filters/FilterTypeIsMethodWrapper.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/FilterTypeIsModule.py` & `objectwalker-2.0/objectwalker/filters/FilterTypeIsModule.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker/filters/__init__.py` & `objectwalker-2.0/objectwalker/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.5/objectwalker.egg-info/SOURCES.txt` & `objectwalker-2.0/objectwalker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

