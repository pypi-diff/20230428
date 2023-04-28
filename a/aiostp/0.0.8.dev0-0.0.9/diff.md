# Comparing `tmp/aiostp-0.0.8.dev0.tar.gz` & `tmp/aiostp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiostp-0.0.8.dev0.tar", last modified: Fri Feb 26 17:17:09 2021, max compression
+gzip compressed data, was "aiostp-0.0.9.tar", last modified: Tue Mar  2 18:55:28 2021, max compression
```

## Comparing `aiostp-0.0.8.dev0.tar` & `aiostp-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 17:17:09.865433 aiostp-0.0.8.dev0/
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2021-02-26 17:17:09.865433 aiostp-0.0.8.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      920 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 17:17:09.861433 aiostp-0.0.8.dev0/aiostp/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 17:17:09.861433 aiostp-0.0.8.dev0/aiostp/http/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4469 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/http/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 17:17:09.861433 aiostp-0.0.8.dev0/aiostp/resources/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3822 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/resources/ordenes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/resources/saldos.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/aiostp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 17:17:09.861433 aiostp-0.0.8.dev0/aiostp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2021-02-26 17:17:09.000000 aiostp-0.0.8.dev0/aiostp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      668 2021-02-26 17:17:09.000000 aiostp-0.0.8.dev0/aiostp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-26 17:17:09.000000 aiostp-0.0.8.dev0/aiostp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-02-26 17:17:09.000000 aiostp-0.0.8.dev0/aiostp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-02-26 17:17:09.000000 aiostp-0.0.8.dev0/aiostp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      394 2021-02-26 17:17:09.865433 aiostp-0.0.8.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 17:17:09.861433 aiostp-0.0.8.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 17:17:09.861433 aiostp-0.0.8.dev0/tests/http/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/http/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 17:17:09.865433 aiostp-0.0.8.dev0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/resources/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/resources/test_ordenes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/resources/test_saldos.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2021-02-26 17:16:59.000000 aiostp-0.0.8.dev0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:28.348981 aiostp-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2021-03-02 18:55:28.348981 aiostp-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2021-03-02 18:55:19.000000 aiostp-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:28.348981 aiostp-0.0.9/aiostp/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:28.348981 aiostp-0.0.9/aiostp/http/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4469 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/http/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:28.348981 aiostp-0.0.9/aiostp/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3822 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/resources/ordenes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/resources/saldos.py
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-03-02 18:55:19.000000 aiostp-0.0.9/aiostp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:28.348981 aiostp-0.0.9/aiostp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2021-03-02 18:55:28.000000 aiostp-0.0.9/aiostp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2021-03-02 18:55:28.000000 aiostp-0.0.9/aiostp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-02 18:55:28.000000 aiostp-0.0.9/aiostp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-02 18:55:28.000000 aiostp-0.0.9/aiostp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-03-02 18:55:28.000000 aiostp-0.0.9/aiostp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2021-03-02 18:55:28.348981 aiostp-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-03-02 18:55:19.000000 aiostp-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:28.348981 aiostp-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:28.348981 aiostp-0.0.9/tests/http/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/http/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:28.348981 aiostp-0.0.9/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/resources/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2737 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/resources/test_ordenes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/resources/test_saldos.py
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2021-03-02 18:55:19.000000 aiostp-0.0.9/tests/test_utils.py
```

### Comparing `aiostp-0.0.8.dev0/PKG-INFO` & `aiostp-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostp
-Version: 0.0.8.dev0
+Version: 0.0.9
 Summary: asyncio client library for stpmex.com
 Home-page: https://github.com/cuenca-mx/aiostp
 Author: Cuenca
 Author-email: dev@cuenca.com
 License: UNKNOWN
 Description: asyncio client library for stpmex.com
         # STP – Async python client library for stpmex.com
```

### Comparing `aiostp-0.0.8.dev0/README.md` & `aiostp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/aiostp/auth.py` & `aiostp-0.0.9/aiostp/auth.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/aiostp/http/client.py` & `aiostp-0.0.9/aiostp/http/client.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/aiostp/resources/base.py` & `aiostp-0.0.9/aiostp/resources/base.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/aiostp/resources/ordenes.py` & `aiostp-0.0.9/aiostp/resources/ordenes.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/aiostp/resources/saldos.py` & `aiostp-0.0.9/aiostp/resources/saldos.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/aiostp.egg-info/PKG-INFO` & `aiostp-0.0.9/aiostp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostp
-Version: 0.0.8.dev0
+Version: 0.0.9
 Summary: asyncio client library for stpmex.com
 Home-page: https://github.com/cuenca-mx/aiostp
 Author: Cuenca
 Author-email: dev@cuenca.com
 License: UNKNOWN
 Description: asyncio client library for stpmex.com
         # STP – Async python client library for stpmex.com
```

### Comparing `aiostp-0.0.8.dev0/aiostp.egg-info/SOURCES.txt` & `aiostp-0.0.9/aiostp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/setup.py` & `aiostp-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/tests/http/test_client.py` & `aiostp-0.0.9/tests/http/test_client.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/tests/resources/test_base.py` & `aiostp-0.0.9/tests/resources/test_base.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/tests/resources/test_ordenes.py` & `aiostp-0.0.9/tests/resources/test_ordenes.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/tests/resources/test_saldos.py` & `aiostp-0.0.9/tests/resources/test_saldos.py`

 * *Files identical despite different names*

### Comparing `aiostp-0.0.8.dev0/tests/test_utils.py` & `aiostp-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

