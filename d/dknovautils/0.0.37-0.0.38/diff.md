# Comparing `tmp/dknovautils-0.0.37.tar.gz` & `tmp/dknovautils-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.37.tar", last modified: Fri Apr 28 12:38:05 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.38.tar", last modified: Fri Apr 28 15:26:29 2023, max compression
```

## Comparing `dknovautils-0.0.37.tar` & `dknovautils-0.0.38.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 12:38:05.000000 dknovautils-0.0.37/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 12:38:05.000000 dknovautils-0.0.37/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2308 2023-04-26 05:25:48.000000 dknovautils-0.0.37/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     7672 2023-04-28 12:38:04.000000 dknovautils-0.0.37/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.37/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.37/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-28 12:38:04.000000 dknovautils-0.0.37/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.37/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.37/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.37/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.37/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 12:38:05.000000 dknovautils-0.0.37/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-28 12:38:04.000000 dknovautils-0.0.37/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 12:38:04.000000 dknovautils-0.0.37/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 12:38:04.000000 dknovautils-0.0.37/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-28 12:38:04.000000 dknovautils-0.0.37/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 12:38:04.000000 dknovautils-0.0.37/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.37/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 12:38:05.000000 dknovautils-0.0.37/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.37/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-28 12:38:05.000000 dknovautils-0.0.37/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1158 2023-04-28 12:38:04.000000 dknovautils-0.0.37/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 15:26:29.000000 dknovautils-0.0.38/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 15:26:29.000000 dknovautils-0.0.38/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2474 2023-04-28 15:25:46.000000 dknovautils-0.0.38/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     7672 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.38/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.38/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.38/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.38/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.38/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.38/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 15:26:29.000000 dknovautils-0.0.38/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.38/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 15:26:29.000000 dknovautils-0.0.38/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.38/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-28 15:26:29.000000 dknovautils-0.0.38/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1158 2023-04-28 15:26:28.000000 dknovautils-0.0.38/setup.py
```

### Comparing `dknovautils-0.0.37/dknovautils/commons.py` & `dknovautils-0.0.38/dknovautils/commons.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,18 @@
     if not _log_inited:
         _log_inited = True
 
         # 只在没有配置的时候起作用 不会重复执行
         logging.basicConfig(level=logging.NOTSET,
                             format=AT._LOG_FORMAT_106)
 
+    # 采用这个将级别提升一下。不知为何 NotSET的设置没有生效 并不会打印。
+    if level == LLevel.Trace:
+        level = LLevel.Debug
+
     logging.log(level.value, obj)
 
     return
 
     if False:
 
         otstr2 = datetime.fromtimestamp(time.time()).strftime(
```

### Comparing `dknovautils-0.0.37/dknovautils/dkat.py` & `dknovautils-0.0.38/dknovautils/dkat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.0.37'
+DkAppVer = '0.0.38'
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
```

### Comparing `dknovautils-0.0.37/dknovautils/dkfiles.py` & `dknovautils-0.0.38/dknovautils/dkfiles.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.37/dknovautils/dkipy.py` & `dknovautils-0.0.38/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.37/dknovautils/dk_imports.py` & `dknovautils-0.0.38/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.37/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.38/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.37
+Version: 0.0.38
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.37/PKG-INFO` & `dknovautils-0.0.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.37
+Version: 0.0.38
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.37/setup.py` & `dknovautils-0.0.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.37'
+DkAppVer = '0.0.38'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

