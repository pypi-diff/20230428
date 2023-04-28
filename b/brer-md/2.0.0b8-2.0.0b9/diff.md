# Comparing `tmp/brer-md-2.0.0b8.tar.gz` & `tmp/brer-md-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/eric/develop/PycharmProjects/run_brer/dist/.tmp-7uok5ooc/brer-md-2.0.0b8.tar", last modified: Thu Apr 27 15:28:24 2023, max compression
+gzip compressed data, was "/Users/eric/develop/PycharmProjects/run_brer/dist/.tmp-wtin0t2k/brer-md-2.0.0b9.tar", last modified: Fri Apr 28 19:16:57 2023, max compression
```

## Comparing `brer-md-2.0.0b8.tar` & `brer-md-2.0.0b9.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:24.032871 brer-md-2.0.0b8/
--rw-r--r--   0 eric       (501) staff       (20)    26526 2020-06-17 12:45:59.000000 brer-md-2.0.0b8/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      178 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)    10504 2023-04-27 15:28:24.032062 brer-md-2.0.0b8/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     9889 2023-04-25 00:36:25.000000 brer-md-2.0.0b8/README.rst
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.936930 brer-md-2.0.0b8/_custom_build/
--rw-r--r--   0 eric       (501) staff       (20)    25208 2022-12-24 14:58:23.000000 brer-md-2.0.0b8/_custom_build/backend.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.942583 brer-md-2.0.0b8/brer_md.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)    10504 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1164 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2022-12-22 15:25:32.000000 brer-md-2.0.0b8/brer_md.egg-info/not-zip-safe
--rw-r--r--   0 eric       (501) staff       (20)       86 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)        5 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)     2161 2023-04-26 22:54:28.000000 brer-md-2.0.0b8/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-04-27 15:28:24.033124 brer-md-2.0.0b8/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      714 2022-12-24 14:57:26.000000 brer-md-2.0.0b8/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.931124 brer-md-2.0.0b8/src/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.954122 brer-md-2.0.0b8/src/brer/
--rw-r--r--   0 eric       (501) staff       (20)      487 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/brer/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     2088 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/brer/_compat.py
--rw-r--r--   0 eric       (501) staff       (20)       24 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/src/brer/_version.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.956401 brer-md-2.0.0b8/src/brer/data/
--rw-r--r--   0 eric       (501) staff       (20)     7360 2022-11-29 14:58:02.000000 brer-md-2.0.0b8/src/brer/data/pair_data.json
--rw-r--r--   0 eric       (501) staff       (20)  7552688 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/brer/data/topol.tpr
--rw-r--r--   0 eric       (501) staff       (20)     4394 2022-11-02 12:54:55.000000 brer-md-2.0.0b8/src/brer/directory_helper.py
--rw-r--r--   0 eric       (501) staff       (20)     6440 2022-11-30 14:57:08.000000 brer-md-2.0.0b8/src/brer/pair_data.py
--rw-r--r--   0 eric       (501) staff       (20)     6490 2022-11-02 12:54:55.000000 brer-md-2.0.0b8/src/brer/plugin_configs.py
--rw-r--r--   0 eric       (501) staff       (20)        0 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/brer/py.typed
--rw-r--r--   0 eric       (501) staff       (20)    30367 2023-04-26 23:00:44.000000 brer-md-2.0.0b8/src/brer/run_config.py
--rw-r--r--   0 eric       (501) staff       (20)    12336 2022-12-22 09:40:59.000000 brer-md-2.0.0b8/src/brer/run_data.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.988483 brer-md-2.0.0b8/src/plugin/
--rw-r--r--   0 eric       (501) staff       (20)     3171 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/CMakeLists.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:24.005318 brer-md-2.0.0b8/src/plugin/cpp/
--rw-r--r--   0 eric       (501) staff       (20)     2847 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/CMakeLists.txt
--rw-r--r--   0 eric       (501) staff       (20)     5959 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/brerpotential.cpp
--rw-r--r--   0 eric       (501) staff       (20)     5932 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/brerpotential.h
--rw-r--r--   0 eric       (501) staff       (20)     2778 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/linearpotential.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2778 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/linearpotential.h
--rw-r--r--   0 eric       (501) staff       (20)     4150 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/linearstoppotential.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4220 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/linearstoppotential.h
--rw-r--r--   0 eric       (501) staff       (20)     1786 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/sessionresources.cpp
--rw-r--r--   0 eric       (501) staff       (20)    13977 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/sessionresources.h
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:24.009788 brer-md-2.0.0b8/src/plugin/pythonmodule/
--rw-r--r--   0 eric       (501) staff       (20)     1049 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/pythonmodule/CMakeLists.txt
--rw-r--r--   0 eric       (501) staff       (20)    24487 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/pythonmodule/export_plugin.cpp
--rw-r--r--   0 eric       (501) staff       (20)      198 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/pythonmodule/export_plugin.h
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:24.024578 brer-md-2.0.0b8/tests/
--rw-r--r--   0 eric       (501) staff       (20)       26 2022-09-23 11:55:27.000000 brer-md-2.0.0b8/tests/pytest.ini
--rw-r--r--   0 eric       (501) staff       (20)      698 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/tests/test_dirhelper.py
--rw-r--r--   0 eric       (501) staff       (20)     1407 2022-11-30 14:32:15.000000 brer-md-2.0.0b8/tests/test_pair_data.py
--rw-r--r--   0 eric       (501) staff       (20)     1977 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/tests/test_plugin_binding.py
--rw-r--r--   0 eric       (501) staff       (20)     1770 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/tests/test_plugin_configs.py
--rw-r--r--   0 eric       (501) staff       (20)     7561 2023-04-27 15:26:23.000000 brer-md-2.0.0b8/tests/test_run_config.py
--rw-r--r--   0 eric       (501) staff       (20)     2910 2023-04-25 00:58:43.000000 brer-md-2.0.0b8/tests/test_run_data.py
--rw-r--r--   0 eric       (501) staff       (20)    49825 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/tests/testdata.json
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.850169 brer-md-2.0.0b9/
+-rw-r--r--   0 eric       (501) staff       (20)    26526 2020-06-17 12:45:59.000000 brer-md-2.0.0b9/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      204 2023-04-28 18:27:58.000000 brer-md-2.0.0b9/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)    10504 2023-04-28 19:16:57.848672 brer-md-2.0.0b9/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     9889 2023-04-25 00:36:25.000000 brer-md-2.0.0b9/README.rst
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.746614 brer-md-2.0.0b9/_custom_build/
+-rw-r--r--   0 eric       (501) staff       (20)    25208 2022-12-24 14:58:23.000000 brer-md-2.0.0b9/_custom_build/backend.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.751883 brer-md-2.0.0b9/brer_md.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)    10504 2023-04-28 19:16:57.000000 brer-md-2.0.0b9/brer_md.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1182 2023-04-28 19:16:57.000000 brer-md-2.0.0b9/brer_md.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-28 19:16:57.000000 brer-md-2.0.0b9/brer_md.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-28 19:16:56.000000 brer-md-2.0.0b9/brer_md.egg-info/not-zip-safe
+-rw-r--r--   0 eric       (501) staff       (20)       86 2023-04-28 19:16:57.000000 brer-md-2.0.0b9/brer_md.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)        5 2023-04-28 19:16:57.000000 brer-md-2.0.0b9/brer_md.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)     2161 2023-04-26 22:54:28.000000 brer-md-2.0.0b9/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-04-28 19:16:57.850482 brer-md-2.0.0b9/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      714 2022-12-24 14:57:26.000000 brer-md-2.0.0b9/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.740645 brer-md-2.0.0b9/src/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.762427 brer-md-2.0.0b9/src/brer/
+-rw-r--r--   0 eric       (501) staff       (20)      487 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/brer/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     2088 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/brer/_compat.py
+-rw-r--r--   0 eric       (501) staff       (20)       24 2023-04-28 19:16:57.000000 brer-md-2.0.0b9/src/brer/_version.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.765092 brer-md-2.0.0b9/src/brer/data/
+-rw-r--r--   0 eric       (501) staff       (20)     7360 2022-11-29 14:58:02.000000 brer-md-2.0.0b9/src/brer/data/pair_data.json
+-rw-r--r--   0 eric       (501) staff       (20)  7552688 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/brer/data/topol.tpr
+-rw-r--r--   0 eric       (501) staff       (20)     4394 2022-11-02 12:54:55.000000 brer-md-2.0.0b9/src/brer/directory_helper.py
+-rw-r--r--   0 eric       (501) staff       (20)     6440 2022-11-30 14:57:08.000000 brer-md-2.0.0b9/src/brer/pair_data.py
+-rw-r--r--   0 eric       (501) staff       (20)     6490 2022-11-02 12:54:55.000000 brer-md-2.0.0b9/src/brer/plugin_configs.py
+-rw-r--r--   0 eric       (501) staff       (20)        0 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/brer/py.typed
+-rw-r--r--   0 eric       (501) staff       (20)    30367 2023-04-26 23:00:44.000000 brer-md-2.0.0b9/src/brer/run_config.py
+-rw-r--r--   0 eric       (501) staff       (20)    12336 2022-12-22 09:40:59.000000 brer-md-2.0.0b9/src/brer/run_data.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.804448 brer-md-2.0.0b9/src/plugin/
+-rw-r--r--   0 eric       (501) staff       (20)     3171 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/CMakeLists.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.819418 brer-md-2.0.0b9/src/plugin/cpp/
+-rw-r--r--   0 eric       (501) staff       (20)     2847 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/CMakeLists.txt
+-rw-r--r--   0 eric       (501) staff       (20)     5959 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/brerpotential.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     5932 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/brerpotential.h
+-rw-r--r--   0 eric       (501) staff       (20)     2778 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/linearpotential.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2778 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/linearpotential.h
+-rw-r--r--   0 eric       (501) staff       (20)     4150 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/linearstoppotential.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4220 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/linearstoppotential.h
+-rw-r--r--   0 eric       (501) staff       (20)     1786 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/sessionresources.cpp
+-rw-r--r--   0 eric       (501) staff       (20)    13977 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/cpp/sessionresources.h
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.828244 brer-md-2.0.0b9/src/plugin/pythonmodule/
+-rw-r--r--   0 eric       (501) staff       (20)     1049 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/pythonmodule/CMakeLists.txt
+-rw-r--r--   0 eric       (501) staff       (20)    24487 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/pythonmodule/export_plugin.cpp
+-rw-r--r--   0 eric       (501) staff       (20)      198 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/src/plugin/pythonmodule/export_plugin.h
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-28 19:16:57.846316 brer-md-2.0.0b9/tests/
+-rw-r--r--   0 eric       (501) staff       (20)    11701 2023-04-25 00:36:25.000000 brer-md-2.0.0b9/tests/conftest.py
+-rw-r--r--   0 eric       (501) staff       (20)       26 2022-09-23 11:55:27.000000 brer-md-2.0.0b9/tests/pytest.ini
+-rw-r--r--   0 eric       (501) staff       (20)      698 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/tests/test_dirhelper.py
+-rw-r--r--   0 eric       (501) staff       (20)     1407 2022-11-30 14:32:15.000000 brer-md-2.0.0b9/tests/test_pair_data.py
+-rw-r--r--   0 eric       (501) staff       (20)     1977 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/tests/test_plugin_binding.py
+-rw-r--r--   0 eric       (501) staff       (20)     1770 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/tests/test_plugin_configs.py
+-rw-r--r--   0 eric       (501) staff       (20)     7561 2023-04-27 15:26:23.000000 brer-md-2.0.0b9/tests/test_run_config.py
+-rw-r--r--   0 eric       (501) staff       (20)     2910 2023-04-25 00:58:43.000000 brer-md-2.0.0b9/tests/test_run_data.py
+-rw-r--r--   0 eric       (501) staff       (20)    49825 2022-10-31 13:13:27.000000 brer-md-2.0.0b9/tests/testdata.json
```

### Comparing `brer-md-2.0.0b8/LICENSE` & `brer-md-2.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/PKG-INFO` & `brer-md-2.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brer-md
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: A set of scripts for running BRER simulations using gmxapi.
 Author: Jennifer M. Hays, Kasson Lab BRER Team
 Author-email: Kasson Lab BRER Team <kassonlab@gmail.com>
 License: LGPL 2.1
 Project-URL: Source, https://github.com/kassonlab/brer-md/
 Project-URL: Documentation, https://kassonlab.github.io/brer-md/
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `brer-md-2.0.0b8/README.rst` & `brer-md-2.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/_custom_build/backend.py` & `brer-md-2.0.0b9/_custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/brer_md.egg-info/PKG-INFO` & `brer-md-2.0.0b9/brer_md.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brer-md
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: A set of scripts for running BRER simulations using gmxapi.
 Author: Jennifer M. Hays, Kasson Lab BRER Team
 Author-email: Kasson Lab BRER Team <kassonlab@gmail.com>
 License: LGPL 2.1
 Project-URL: Source, https://github.com/kassonlab/brer-md/
 Project-URL: Documentation, https://kassonlab.github.io/brer-md/
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `brer-md-2.0.0b8/brer_md.egg-info/SOURCES.txt` & `brer-md-2.0.0b9/brer_md.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 src/plugin/cpp/linearstoppotential.cpp
 src/plugin/cpp/linearstoppotential.h
 src/plugin/cpp/sessionresources.cpp
 src/plugin/cpp/sessionresources.h
 src/plugin/pythonmodule/CMakeLists.txt
 src/plugin/pythonmodule/export_plugin.cpp
 src/plugin/pythonmodule/export_plugin.h
+tests/conftest.py
 tests/pytest.ini
 tests/test_dirhelper.py
 tests/test_pair_data.py
 tests/test_plugin_binding.py
 tests/test_plugin_configs.py
 tests/test_run_config.py
 tests/test_run_data.py
```

### Comparing `brer-md-2.0.0b8/pyproject.toml` & `brer-md-2.0.0b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/setup.py` & `brer-md-2.0.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/brer/_compat.py` & `brer-md-2.0.0b9/src/brer/_compat.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/brer/data/pair_data.json` & `brer-md-2.0.0b9/src/brer/data/pair_data.json`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/brer/data/topol.tpr` & `brer-md-2.0.0b9/src/brer/data/topol.tpr`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/brer/directory_helper.py` & `brer-md-2.0.0b9/src/brer/directory_helper.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/brer/pair_data.py` & `brer-md-2.0.0b9/src/brer/pair_data.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/brer/plugin_configs.py` & `brer-md-2.0.0b9/src/brer/plugin_configs.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/brer/run_config.py` & `brer-md-2.0.0b9/src/brer/run_config.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/brer/run_data.py` & `brer-md-2.0.0b9/src/brer/run_data.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/CMakeLists.txt` & `brer-md-2.0.0b9/src/plugin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/CMakeLists.txt` & `brer-md-2.0.0b9/src/plugin/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/brerpotential.cpp` & `brer-md-2.0.0b9/src/plugin/cpp/brerpotential.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/brerpotential.h` & `brer-md-2.0.0b9/src/plugin/cpp/brerpotential.h`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/linearpotential.cpp` & `brer-md-2.0.0b9/src/plugin/cpp/linearpotential.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/linearpotential.h` & `brer-md-2.0.0b9/src/plugin/cpp/linearpotential.h`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/linearstoppotential.cpp` & `brer-md-2.0.0b9/src/plugin/cpp/linearstoppotential.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/linearstoppotential.h` & `brer-md-2.0.0b9/src/plugin/cpp/linearstoppotential.h`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/sessionresources.cpp` & `brer-md-2.0.0b9/src/plugin/cpp/sessionresources.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/cpp/sessionresources.h` & `brer-md-2.0.0b9/src/plugin/cpp/sessionresources.h`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/pythonmodule/CMakeLists.txt` & `brer-md-2.0.0b9/src/plugin/pythonmodule/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/src/plugin/pythonmodule/export_plugin.cpp` & `brer-md-2.0.0b9/src/plugin/pythonmodule/export_plugin.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/tests/test_dirhelper.py` & `brer-md-2.0.0b9/tests/test_dirhelper.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/tests/test_pair_data.py` & `brer-md-2.0.0b9/tests/test_pair_data.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/tests/test_plugin_binding.py` & `brer-md-2.0.0b9/tests/test_plugin_binding.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/tests/test_plugin_configs.py` & `brer-md-2.0.0b9/tests/test_plugin_configs.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/tests/test_run_config.py` & `brer-md-2.0.0b9/tests/test_run_config.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/tests/test_run_data.py` & `brer-md-2.0.0b9/tests/test_run_data.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b8/tests/testdata.json` & `brer-md-2.0.0b9/tests/testdata.json`

 * *Files identical despite different names*

