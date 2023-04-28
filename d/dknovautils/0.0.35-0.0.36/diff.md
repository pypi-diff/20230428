# Comparing `tmp/dknovautils-0.0.35.tar.gz` & `tmp/dknovautils-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.35.tar", last modified: Fri Apr 28 07:41:11 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.36.tar", last modified: Fri Apr 28 09:56:40 2023, max compression
```

## Comparing `dknovautils-0.0.35.tar` & `dknovautils-0.0.36.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 07:41:11.000000 dknovautils-0.0.35/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 07:41:11.000000 dknovautils-0.0.35/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2308 2023-04-26 05:25:48.000000 dknovautils-0.0.35/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     7621 2023-04-28 07:41:07.000000 dknovautils-0.0.35/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.35/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.35/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-28 07:41:07.000000 dknovautils-0.0.35/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.35/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.35/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.35/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.35/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 07:41:11.000000 dknovautils-0.0.35/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.35/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 07:41:11.000000 dknovautils-0.0.35/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.35/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-28 07:41:11.000000 dknovautils-0.0.35/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1158 2023-04-28 07:41:07.000000 dknovautils-0.0.35/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 09:56:40.000000 dknovautils-0.0.36/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 09:56:40.000000 dknovautils-0.0.36/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2308 2023-04-26 05:25:48.000000 dknovautils-0.0.36/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     7667 2023-04-28 09:56:40.000000 dknovautils-0.0.36/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.36/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.36/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-28 09:56:39.000000 dknovautils-0.0.36/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.36/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.36/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.36/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.36/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 09:56:40.000000 dknovautils-0.0.36/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-28 09:56:40.000000 dknovautils-0.0.36/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 09:56:40.000000 dknovautils-0.0.36/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 09:56:40.000000 dknovautils-0.0.36/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-28 09:56:40.000000 dknovautils-0.0.36/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 09:56:40.000000 dknovautils-0.0.36/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.36/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 09:56:40.000000 dknovautils-0.0.36/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.36/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-28 09:56:40.000000 dknovautils-0.0.36/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1158 2023-04-28 09:56:39.000000 dknovautils-0.0.36/setup.py
```

### Comparing `dknovautils-0.0.35/dknovautils/commons.py` & `dknovautils-0.0.36/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.35/dknovautils/dkat.py` & `dknovautils-0.0.36/dknovautils/dkat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.0.35'
+DkAppVer = '0.0.36'
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
 
@@ -61,15 +61,15 @@
 
     _LOG_FORMAT_100 = "%(asctime)s - %(levelname)s - %(message)s"
     _DATE_FORMAT_100 = "%m/%d/%Y %H:%M:%S %p"
     # _DATE_FORMAT_iso_simple = "%m/%d/%Y %H:%M:%S %p"
 
     STRFMT_ISO_COMPACT_SIMPLE = "%Y%m%dT%H%M%S"
     STRFMT_ISO_COMPACT_ALL_A = "%Y%m%dT%H%M%SS%f"
-    STRFMT_ISO_ALL_A = "%Y-%m-%dT%H:%M:%S,%f%Z"
+    STRFMT_ISO_ALL_A = "%Y-%m-%dT%H:%M:%S.%f%Z"
 
     _LOG_FORMAT_106 = '%(asctime)s %(name)s %(threadName)s %(levelname)s %(message)s'
 
     '''
     
     dtstr = datetime.now().strftime("%Y%m%dT%H%M%S")
 
@@ -178,21 +178,21 @@
     dts = datetime.now().strftime("%Y%m%dT%H%M%S")
     print("date and time =", dts)
     
     
     '''
 
     @staticmethod
-    def sdf_isocompact_format_datetime(dt, *, precise: str = 'a'):
+    def sdf_isocompact_format_datetime(dt, *, precise: str = 's'):
         assert precise in ['a', 'd', 's'], 'err5554 bad precise'
 
         if dt is not None:
             AT.unsupported()
 
-        dt = datetime.now()
+        dt = AT._now_dt()
         dts = dt.strftime(AT.STRFMT_ISO_COMPACT_ALL_A)
 
         if precise == 'a':
             pass
         elif precise == 's':
             dts = dts[:(8+0+1+6)]
         elif precise == 'd':
@@ -204,17 +204,19 @@
 
     @staticmethod
     def sdf_logger():
         pass
 
     @staticmethod
     def _now_dt():
+        dt = datetime.now()
+        return dt
 
     @staticmethod
-    def sdf_logger_format_datetime(dt: int = None, *, precise: str = 'a') -> str:
+    def sdf_logger_format_datetime(dt: int = None, *, precise: str = 's') -> str:
         '''
 https://strftime.org/    
 https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes
 https://man7.org/linux/man-pages/man3/strftime.3.html
 
 2023-12-01T08:30:00.123456
```

### Comparing `dknovautils-0.0.35/dknovautils/dkfiles.py` & `dknovautils-0.0.36/dknovautils/dkfiles.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.35/dknovautils/dkipy.py` & `dknovautils-0.0.36/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.35/dknovautils/dk_imports.py` & `dknovautils-0.0.36/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.35/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.36/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.35
+Version: 0.0.36
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.35/PKG-INFO` & `dknovautils-0.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.35
+Version: 0.0.36
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.35/setup.py` & `dknovautils-0.0.36/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.35'
+DkAppVer = '0.0.36'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

