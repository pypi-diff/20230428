# Comparing `tmp/dknovautils-0.0.34.tar.gz` & `tmp/dknovautils-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.34.tar", last modified: Wed Apr 26 05:10:16 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.35.tar", last modified: Fri Apr 28 07:41:11 2023, max compression
```

## Comparing `dknovautils-0.0.34.tar` & `dknovautils-0.0.35.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-26 05:10:16.000000 dknovautils-0.0.34/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2308 2023-04-26 05:09:42.000000 dknovautils-0.0.34/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5866 2023-04-26 05:10:15.000000 dknovautils-0.0.34/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.34/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.34/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-26 05:10:15.000000 dknovautils-0.0.34/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.34/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.34/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.34/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.34/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.34/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-26 05:10:16.000000 dknovautils-0.0.34/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.34/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-26 05:10:16.000000 dknovautils-0.0.34/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-26 05:10:15.000000 dknovautils-0.0.34/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 07:41:11.000000 dknovautils-0.0.35/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 07:41:11.000000 dknovautils-0.0.35/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2308 2023-04-26 05:25:48.000000 dknovautils-0.0.35/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     7621 2023-04-28 07:41:07.000000 dknovautils-0.0.35/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.35/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.35/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-28 07:41:07.000000 dknovautils-0.0.35/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.35/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.35/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.35/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.35/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 07:41:11.000000 dknovautils-0.0.35/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 07:41:10.000000 dknovautils-0.0.35/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.35/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 07:41:11.000000 dknovautils-0.0.35/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.35/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-28 07:41:11.000000 dknovautils-0.0.35/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1158 2023-04-28 07:41:07.000000 dknovautils-0.0.35/setup.py
```

### Comparing `dknovautils-0.0.34/dknovautils/commons.py` & `dknovautils-0.0.35/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.34/dknovautils/dkat.py` & `dknovautils-0.0.35/dknovautils/dkat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.0.34'
+DkAppVer = '0.0.35'
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
 
     _AstErrorCnt_ = 0
 
+    __logger = None
+
+    @classmethod
+    def log(cls, loggerName='dkn'):
+        if cls.__logger is None:
+            logger = logging.getLogger(loggerName)
+            cls.__logger = logger
+
+        return cls.__logger
+
     @staticmethod
     def log_loggerFun(loggerName='dkn', initInnerLoggerFun=True, beepError=True, beepWarn=False):
 
         logger = logging.getLogger(loggerName)
 
         def mloggerFun(obj, llevel):
             assert isinstance(llevel, LLevel)
@@ -49,21 +59,34 @@
 
         return mloggerFun
 
     _LOG_FORMAT_100 = "%(asctime)s - %(levelname)s - %(message)s"
     _DATE_FORMAT_100 = "%m/%d/%Y %H:%M:%S %p"
     # _DATE_FORMAT_iso_simple = "%m/%d/%Y %H:%M:%S %p"
 
-    _LOG_FORMAT_106 = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+    STRFMT_ISO_COMPACT_SIMPLE = "%Y%m%dT%H%M%S"
+    STRFMT_ISO_COMPACT_ALL_A = "%Y%m%dT%H%M%SS%f"
+    STRFMT_ISO_ALL_A = "%Y-%m-%dT%H:%M:%S,%f%Z"
+
+    _LOG_FORMAT_106 = '%(asctime)s %(name)s %(threadName)s %(levelname)s %(message)s'
+
+    '''
+    
+    dtstr = datetime.now().strftime("%Y%m%dT%H%M%S")
+
+        
+    '''
 
     @classmethod
-    def log_basicConfig(cls, filename='my.log', loggerName='dkn', initInnerLoggerFun=True):
+    def log_basicConfig(cls, filename='tmp_test.log', loggerName='dkn', initInnerLoggerFun=True):
 
         logging.basicConfig(filename=filename, level=logging.NOTSET,
-                            format=cls._LOG_FORMAT_100, datefmt=cls._DATE_FORMAT_100, force=True)
+                            format=cls._LOG_FORMAT_106,
+                            # datefmt=cls._DATE_FORMAT_100,
+                            force=True)
 
         logger = logging.getLogger(loggerName)
         logger.setLevel(logging.DEBUG)
 
         # create console handler and set level to debug
         ch = logging.StreamHandler()
         ch.setLevel(logging.DEBUG)
@@ -109,14 +132,19 @@
             AT.beep(tone)
 
     @staticmethod
     def beep(tone='ping'):
         beepy.beep(sound=tone)
 
     @staticmethod
+    def beep2():
+        #!wget -q -T 1 http://localhost:333/hello
+        print('\7')
+
+    @staticmethod
     def never(s=None):
         AT.assert_(False,  s if s is not None else 'never come here')
 
     @staticmethod
     def checksys():
         assert sys.version_info >= (3, 11)
 
@@ -150,27 +178,76 @@
     dts = datetime.now().strftime("%Y%m%dT%H%M%S")
     print("date and time =", dts)
     
     
     '''
 
     @staticmethod
+    def sdf_isocompact_format_datetime(dt, *, precise: str = 'a'):
+        assert precise in ['a', 'd', 's'], 'err5554 bad precise'
+
+        if dt is not None:
+            AT.unsupported()
+
+        dt = datetime.now()
+        dts = dt.strftime(AT.STRFMT_ISO_COMPACT_ALL_A)
+
+        if precise == 'a':
+            pass
+        elif precise == 's':
+            dts = dts[:(8+0+1+6)]
+        elif precise == 'd':
+            dts = dts[:(8)]
+        else:
+            AT.never()
+
+        return dts
+
+    @staticmethod
     def sdf_logger():
         pass
 
     @staticmethod
-    def sdf_logger_fomrat_datetime(dt: int = None) -> str:
-        # "yyyy-MM-dd HH:mm:ss"
+    def _now_dt():
+
+    @staticmethod
+    def sdf_logger_format_datetime(dt: int = None, *, precise: str = 'a') -> str:
+        '''
+https://strftime.org/    
+https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes
+https://man7.org/linux/man-pages/man3/strftime.3.html
+
+2023-12-01T08:30:00.123456
+
+"yyyy-MM-ddTHH:mm:ss"
+
+date -I
+
+d date
+s seconds
+a all
+
+        '''
+        assert precise in ['a', 'd', 's'], 'err5554 bad precise'
 
         if dt is not None:
             dt = datetime.fromtimestamp(dt/1000, tz=None)
         else:
             dt = datetime.now()
 
-        dts = dt.strftime("%Y-%m-%d %H:%M:%S")
+        dts = dt.strftime(AT.STRFMT_ISO_ALL_A)
+
+        if precise == 'a':
+            pass
+        elif precise == 's':
+            dts = dts[:(10+1+8)]
+        elif precise == 'd':
+            dts = dts[:(10)]
+        else:
+            AT.never()
 
         return dts
 
     @staticmethod
     def assert_(b: bool, s: str = None):
         # 改成完善的形式
 
@@ -182,17 +259,14 @@
         AT._AstErrorCnt_ += 1
         msg = _unknown_err if s is None else s
 
         dknovautils.commons.iprint_error(msg)
 
         raise DkAstException(msg)
 
-        # assert b,
-        pass
-
     @staticmethod
     def mychdir(s):
         assert isinstance(s, str) and len(s) > 0
         iprint_debug(f'chdir: {s}')
         os.chdir(s)
 
     @staticmethod
```

### Comparing `dknovautils-0.0.34/dknovautils/dkfiles.py` & `dknovautils-0.0.35/dknovautils/dkfiles.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.34/dknovautils/dkipy.py` & `dknovautils-0.0.35/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.34/dknovautils/dk_imports.py` & `dknovautils-0.0.35/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.34/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.35/dknovautils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.34
+Version: 0.0.35
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.34/PKG-INFO` & `dknovautils-0.0.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.34
+Version: 0.0.35
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.34/setup.py` & `dknovautils-0.0.35/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.34'
+DkAppVer = '0.0.35'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
@@ -21,14 +21,15 @@
     # long_description_content_type="text/markdown",
     url="http://example.com",
     install_requires=[
         # 'requests!=2.9.0',
         # 'lxml',
         # 'monotonic>=1.5',
         'numpy',
+        'beepy',
     ],
     packages=setuptools.find_packages(exclude=("test")),
     classifiers=(
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

