# Comparing `tmp/autosubmitconfigparser-1.0.25.tar.gz` & `tmp/autosubmitconfigparser-1.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.25.tar", last modified: Tue Apr 25 20:05:58 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.26.tar", last modified: Fri Apr 28 14:06:54 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.25.tar` & `autosubmitconfigparser-1.0.26.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.267113 autosubmitconfigparser-1.0.25/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.25/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.25/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-04-25 20:05:58.267113 autosubmitconfigparser-1.0.25/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.25/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-04-25 20:05:27.000000 autosubmitconfigparser-1.0.25/VERSION
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.25/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.263113 autosubmitconfigparser-1.0.25/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.263113 autosubmitconfigparser-1.0.25/autosubmitconfigparser/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.263113 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.263113 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4187 2022-12-19 09:28:49.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    74789 2023-04-05 09:03:32.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    99361 2023-04-25 18:15:19.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.267113 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      408 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.263113 autosubmitconfigparser-1.0.25/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-04-25 20:05:58.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1514 2023-04-25 20:05:58.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-04-25 20:05:58.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      305 2023-04-25 20:05:58.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-04-25 20:05:58.000000 autosubmitconfigparser-1.0.25/autosubmitconfigparser.egg-info/top_level.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      591 2022-10-26 08:55:26.000000 autosubmitconfigparser-1.0.25/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.267113 autosubmitconfigparser-1.0.25/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.25/log/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-25 20:05:58.267113 autosubmitconfigparser-1.0.25/log/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.25/log/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.25/log/__pycache__/log.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.25/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.25/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      416 2023-02-07 12:12:28.000000 autosubmitconfigparser-1.0.25/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-04-25 20:05:58.267113 autosubmitconfigparser-1.0.25/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1465 2023-04-25 20:05:27.000000 autosubmitconfigparser-1.0.25/setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.25/test_config.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.714023 autosubmitconfigparser-1.0.26/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.26/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.26/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-04-28 14:06:54.714023 autosubmitconfigparser-1.0.26/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.26/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-04-28 14:06:17.000000 autosubmitconfigparser-1.0.26/VERSION
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.26/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.710023 autosubmitconfigparser-1.0.26/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.710023 autosubmitconfigparser-1.0.26/autosubmitconfigparser/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.710023 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.710023 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4187 2022-12-19 09:28:49.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    74789 2023-04-05 09:03:32.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    99989 2023-04-28 10:03:58.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.714023 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      408 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.710023 autosubmitconfigparser-1.0.26/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-04-28 14:06:54.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1514 2023-04-28 14:06:54.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-04-28 14:06:54.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      305 2023-04-28 14:06:54.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-04-28 14:06:54.000000 autosubmitconfigparser-1.0.26/autosubmitconfigparser.egg-info/top_level.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      591 2022-10-26 08:55:26.000000 autosubmitconfigparser-1.0.26/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.714023 autosubmitconfigparser-1.0.26/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.26/log/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-28 14:06:54.714023 autosubmitconfigparser-1.0.26/log/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.26/log/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.26/log/__pycache__/log.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.26/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.26/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      416 2023-02-07 12:12:28.000000 autosubmitconfigparser-1.0.26/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-04-28 14:06:54.714023 autosubmitconfigparser-1.0.26/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1465 2023-04-28 14:06:17.000000 autosubmitconfigparser-1.0.26/setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.26/test_config.py
```

### Comparing `autosubmitconfigparser-1.0.25/PKG-INFO` & `autosubmitconfigparser-1.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.25
+Version: 1.0.26
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.25/README.md` & `autosubmitconfigparser-1.0.26/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/configcommon.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         :return: percentage of scratch free space needed
         :rtype: int
         """
         return int(self.get_section([section, 'SCRATCH_FREE_SPACE'], ""))
 
     def get_memory(self, section):
         """
-        Gets memory needed for the given job type
+        Gets memory needed for the given job typemissing_
         :param section: job type
         :type section: str
         :return: memory needed
         :rtype: str
         """
         return str(self.get_section([section, 'MEMORY'], ""))
 
@@ -1359,22 +1359,36 @@
                 self.experiment_data = starter_conf
             # This part is useless, as it is already done
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data, max_deep=25)
             user_data = self.load_custom_config_section(self.experiment_data, filenames_to_load["POST"])
             self.experiment_data = self.substitute_dynamic_variables(self.unify_conf(self.experiment_data,user_data))
             ###
             self.current_loaded_files.update(non_minimal_files)
-
-            # IF expid and hpcarch are not defined, use the ones from the minimal.yml file
-            for key in starter_conf.keys():
-                if key not in self.experiment_data.keys():
-                    self.experiment_data[key] = starter_conf[key]
             if "AS_TEMP" in self.experiment_data.keys():
                 del self.experiment_data["AS_TEMP"]
+            # IF expid and hpcarch are not defined, use the ones from the minimal.yml file
+            self.deep_add_missing_starter_conf(self.experiment_data,starter_conf)
+
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data)
+            self.experiment_data = self.normalize_variables(self.experiment_data)
+            pass
+
+    def deep_add_missing_starter_conf(self,experiment_data,starter_conf):
+        """
+        Add the missing keys from starter_conf to experiment_data
+        :param experiment_data:
+        :param starter_conf:
+        :return:
+        """
+        for key in starter_conf.keys():
+            if key not in experiment_data.keys():
+                experiment_data[key] = starter_conf[key]
+            elif isinstance(starter_conf[key], collections.abc.Mapping):
+                experiment_data[key] = self.deep_add_missing_starter_conf(experiment_data[key],starter_conf[key])
+        return experiment_data
 
     def deep_get_long_key(self,section_data,long_key):
         parameters_dict = dict()
         for key, val in section_data.items():
             if isinstance(val, collections.abc.Mapping ):
                 parameters_dict.update(self.deep_get_long_key(section_data.get(key, {}),long_key+"."+key))
             else:
```

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.25
+Version: 1.0.26
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.25/autosubmitconfigparser.egg-info/SOURCES.txt` & `autosubmitconfigparser-1.0.26/autosubmitconfigparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/environment.yml` & `autosubmitconfigparser-1.0.26/environment.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/log/__pycache__/log.cpython-37.pyc` & `autosubmitconfigparser-1.0.26/log/__pycache__/log.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/log/fd_show.py` & `autosubmitconfigparser-1.0.26/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/log/log.py` & `autosubmitconfigparser-1.0.26/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.25/setup.py` & `autosubmitconfigparser-1.0.26/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.25",
+    version="1.0.26",
     author="Daniel Beltran Mora",
     author_email="daniel.beltran@bsc.es",
     description="An utility library that allows to read an Autosubmit 4 experiment configuration.",
     keywords=['climate', 'weather', 'workflow', 'HPC'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git",
```

### Comparing `autosubmitconfigparser-1.0.25/test_config.py` & `autosubmitconfigparser-1.0.26/test_config.py`

 * *Files identical despite different names*

