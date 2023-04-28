# Comparing `tmp/dbus-python-client-gen-0.8.2.tar.gz` & `tmp/dbus-python-client-gen-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbus-python-client-gen-0.8.2.tar", last modified: Thu Feb 23 03:37:59 2023, max compression
+gzip compressed data, was "dbus-python-client-gen-0.8.3.tar", last modified: Fri Apr 28 00:38:13 2023, max compression
```

## Comparing `dbus-python-client-gen-0.8.2.tar` & `dbus-python-client-gen-0.8.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-02-23 03:37:59.760674 dbus-python-client-gen-0.8.2/
--rw-rw----   0 mulhern   (1000) mulhern   (1000)    16726 2021-06-03 20:42:52.000000 dbus-python-client-gen-0.8.2/LICENSE
--rw-r--r--   0 mulhern   (1000) mulhern   (1000)     4744 2023-02-23 03:37:59.760674 dbus-python-client-gen-0.8.2/PKG-INFO
--rw-rw----   0 mulhern   (1000) mulhern   (1000)     3822 2021-06-03 20:42:52.000000 dbus-python-client-gen-0.8.2/README.rst
--rw-rw----   0 mulhern   (1000) mulhern   (1000)       81 2023-02-23 01:29:29.000000 dbus-python-client-gen-0.8.2/pyproject.toml
--rw-rw----   0 mulhern   (1000) mulhern   (1000)     1052 2023-02-23 03:37:59.761674 dbus-python-client-gen-0.8.2/setup.cfg
--rw-rw----   0 mulhern   (1000) mulhern   (1000)      106 2023-02-23 01:29:29.000000 dbus-python-client-gen-0.8.2/setup.py
-drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-02-23 03:37:59.758674 dbus-python-client-gen-0.8.2/src/
-drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-02-23 03:37:59.759673 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen/
--rw-rw----   0 mulhern   (1000) mulhern   (1000)      612 2021-06-03 20:42:52.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen/__init__.py
--rw-rw----   0 mulhern   (1000) mulhern   (1000)     5357 2021-06-03 20:42:52.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen/_errors.py
--rw-rw----   0 mulhern   (1000) mulhern   (1000)    16119 2023-02-22 22:52:57.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen/_invokers.py
--rw-rw----   0 mulhern   (1000) mulhern   (1000)      376 2023-02-23 03:37:11.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen/_version.py
-drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-02-23 03:37:59.760674 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen.egg-info/
--rw-r--r--   0 mulhern   (1000) mulhern   (1000)     4744 2023-02-23 03:37:59.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen.egg-info/PKG-INFO
--rw-r--r--   0 mulhern   (1000) mulhern   (1000)      481 2023-02-23 03:37:59.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen.egg-info/SOURCES.txt
--rw-r--r--   0 mulhern   (1000) mulhern   (1000)        1 2023-02-23 03:37:59.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen.egg-info/dependency_links.txt
--rw-r--r--   0 mulhern   (1000) mulhern   (1000)       34 2023-02-23 03:37:59.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen.egg-info/requires.txt
--rw-r--r--   0 mulhern   (1000) mulhern   (1000)       23 2023-02-23 03:37:59.000000 dbus-python-client-gen-0.8.2/src/dbus_python_client_gen.egg-info/top_level.txt
-drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-02-23 03:37:59.760674 dbus-python-client-gen-0.8.2/tests/
--rw-rw----   0 mulhern   (1000) mulhern   (1000)     3610 2021-08-27 18:57:14.000000 dbus-python-client-gen-0.8.2/tests/test_generated.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-04-28 00:38:13.624980 dbus-python-client-gen-0.8.3/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)    16726 2021-06-03 20:42:52.000000 dbus-python-client-gen-0.8.3/LICENSE
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     4744 2023-04-28 00:38:13.624980 dbus-python-client-gen-0.8.3/PKG-INFO
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     3822 2021-06-03 20:42:52.000000 dbus-python-client-gen-0.8.3/README.rst
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)       81 2023-02-23 01:29:29.000000 dbus-python-client-gen-0.8.3/pyproject.toml
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     1051 2023-04-28 00:38:13.625980 dbus-python-client-gen-0.8.3/setup.cfg
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      106 2023-04-27 21:36:03.000000 dbus-python-client-gen-0.8.3/setup.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-04-28 00:38:13.609980 dbus-python-client-gen-0.8.3/src/
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-04-28 00:38:13.623980 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      646 2023-04-28 00:21:08.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen/__init__.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     5357 2023-04-28 00:24:46.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen/_errors.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)    16119 2023-04-28 00:24:46.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen/_invokers.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      376 2023-04-28 00:34:33.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen/_version.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-04-28 00:38:13.624980 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen.egg-info/
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     4744 2023-04-28 00:38:13.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen.egg-info/PKG-INFO
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)      481 2023-04-28 00:38:13.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)        1 2023-04-28 00:38:13.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)       34 2023-04-28 00:38:13.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen.egg-info/requires.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)       23 2023-04-28 00:38:13.000000 dbus-python-client-gen-0.8.3/src/dbus_python_client_gen.egg-info/top_level.txt
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-04-28 00:38:13.624980 dbus-python-client-gen-0.8.3/tests/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     3610 2023-04-28 00:24:46.000000 dbus-python-client-gen-0.8.3/tests/test_generated.py
```

### Comparing `dbus-python-client-gen-0.8.2/LICENSE` & `dbus-python-client-gen-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbus-python-client-gen-0.8.2/PKG-INFO` & `dbus-python-client-gen-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbus-python-client-gen
-Version: 0.8.2
+Version: 0.8.3
 Summary: transforms values into properly wrapped dbus-python objects
 Home-page: https://github.com/stratis-storage/dbus-python-client-gen
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
 License: MPL-2.0
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbus-python-client-gen-0.8.2/README.rst` & `dbus-python-client-gen-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `dbus-python-client-gen-0.8.2/src/dbus_python_client_gen/__init__.py` & `dbus-python-client-gen-0.8.3/src/dbus_python_client_gen/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,7 +15,8 @@
     DPClientKeywordError,
     DPClientMarshallingError,
     DPClientMethodCallContext,
     DPClientRuntimeError,
     DPClientSetPropertyContext,
 )
 from ._invokers import make_class
+from ._version import __version__
```

### Comparing `dbus-python-client-gen-0.8.2/src/dbus_python_client_gen/_errors.py` & `dbus-python-client-gen-0.8.3/src/dbus_python_client_gen/_errors.py`

 * *Files identical despite different names*

### Comparing `dbus-python-client-gen-0.8.2/src/dbus_python_client_gen/_invokers.py` & `dbus-python-client-gen-0.8.3/src/dbus_python_client_gen/_invokers.py`

 * *Files identical despite different names*

### Comparing `dbus-python-client-gen-0.8.2/src/dbus_python_client_gen.egg-info/PKG-INFO` & `dbus-python-client-gen-0.8.3/src/dbus_python_client_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbus-python-client-gen
-Version: 0.8.2
+Version: 0.8.3
 Summary: transforms values into properly wrapped dbus-python objects
 Home-page: https://github.com/stratis-storage/dbus-python-client-gen
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
 License: MPL-2.0
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbus-python-client-gen-0.8.2/tests/test_generated.py` & `dbus-python-client-gen-0.8.3/tests/test_generated.py`

 * *Files identical despite different names*

