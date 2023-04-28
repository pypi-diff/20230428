# Comparing `tmp/ifes_apt_tc_data_modeling-0.0.6.tar.gz` & `tmp/ifes_apt_tc_data_modeling-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mkuehbach/test-ifes/ifes_apt_tc_data_modeling/dist/.tmp-gwmnsilb/ifes_apt_tc_data_modeling-0.0.6.tar", last modified: Fri Mar 24 22:06:47 2023, max compression
+gzip compressed data, was "ifes_apt_tc_data_modeling-0.0.7.tar", last modified: Fri Apr 28 13:32:38 2023, max compression
```

## Comparing `ifes_apt_tc_data_modeling-0.0.6.tar` & `ifes_apt_tc_data_modeling-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11358 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/LICENSE.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22438 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/PKG-INFO
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8950 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/README.md
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/__init__.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     4149 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_headers.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11187 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_reader.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    19797 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_sections.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    34067 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1553 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_utils.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/epos/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/epos/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7731 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/epos/epos_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/nexus/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/nexus/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1585 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/nexus/nx_field.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8106 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/nexus/nx_ion.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/pos/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/pos/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     3414 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/pos/pos_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rng/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rng/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8153 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rng/rng_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rrng/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rrng/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9558 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rrng/rrng_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1335 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/definitions.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1713 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/mmapped_io.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    17147 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/molecular_ions.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)   164819 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1253 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/string_handling.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8647 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/utils.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling.egg-info/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22438 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling.egg-info/PKG-INFO
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1410 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)        1 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling.egg-info/dependency_links.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      119 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling.egg-info/requires.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       26 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling.egg-info/top_level.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      882 2023-03-24 22:04:05.000000 ifes_apt_tc_data_modeling-0.0.6/pyproject.toml
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       38 2023-03-24 22:06:47.000000 ifes_apt_tc_data_modeling-0.0.6/setup.cfg
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11358 2023-01-13 23:09:44.000000 ifes_apt_tc_data_modeling-0.0.7/LICENSE.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22620 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/PKG-INFO
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9003 2023-04-28 12:07:31.000000 ifes_apt_tc_data_modeling-0.0.7/README.md
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/__init__.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     4149 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_headers.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11187 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_reader.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    19797 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_sections.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    34067 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1553 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_utils.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 09:03:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7731 2023-03-20 09:03:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/epos_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:58:26.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     5731 2023-04-28 13:16:35.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/fig_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:59:34.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1585 2023-03-20 09:02:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/nx_field.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8106 2023-03-20 09:02:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/nx_ion.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-20 08:58:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     3414 2023-03-20 08:59:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/pos_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:58:26.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8153 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/rng_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9558 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/rrng_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1335 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/definitions.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1713 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/mmapped_io.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    16989 2023-04-28 12:58:48.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/molecular_ions.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)   164819 2023-03-20 08:50:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1253 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/string_handling.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8545 2023-04-28 12:42:39.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/utils.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22620 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/PKG-INFO
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1496 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)        1 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/dependency_links.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      139 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/requires.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       26 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/top_level.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1051 2023-04-28 11:50:07.000000 ifes_apt_tc_data_modeling-0.0.7/pyproject.toml
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       38 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ifes_apt_tc_data_modeling-0.0.6/LICENSE.txt` & `ifes_apt_tc_data_modeling-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/PKG-INFO` & `ifes_apt_tc_data_modeling-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifes_apt_tc_data_modeling
-Version: 0.0.6
+Version: 0.0.7
 Summary: Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy.
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -202,19 +202,22 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 # atomprobe-data-modeling
 
 ## Mission:
 Foster exchange about data models and work towards specifications
 of file formats from the research field of atom probe microscopy.
@@ -263,41 +266,41 @@
 immediate benefit to users. The collection of examples and technical discussions
 via issues serves the more long-term aim. This is to arrive at a detailed technical
 specification rather than more robust parsers only so that atom probe data can be
 exchanged across tools irrespective of their formatting.
 
 # Getting started as developer
 
-You should create a virtual environment. We tested on Ubuntu with Python 3.7.
-Newer versions of Python should work similarly (for this change 3.7) to the
-desired version tag.
+You should create a virtual environment. We tested on Ubuntu with Python 3.8.
+Newer versions of Python should work similarly when using the desired version tag.
 
-If you don't have Python 3.7 installed on your computer, follow these commands:
+If you don't have Python 3.8 installed on your computer, follow these commands:
 ```
 sudo add-apt-repository ppa:deadsnakes/ppa
-sudo apt install python3.7 python3-dev libpython3.7-dev python3.7-venv
+sudo apt install python3.8 python3-dev libpython3.8-dev python3.8-venv
 ```
 
-In some cases when using Python3.7 it was necessary to install python-numpy in others
+In some cases when using Python3.8 it was necessary to install python-numpy in others
 not. So consider this if you run into issues when continuing this manual.
 The following steps will install the ifes_apt_tc_data_modeling module in the
 latest version.
 
 ```
 mkdir <your-brand-new-folder>
 cd <your-brand-new-folder>
 pip install virtualenv
-virtualenv --python=python3.7 .py37
-source .py37/bin/activate
+virtualenv --python=python3.8 .py38
+source .py38/bin/activate
 
 git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
-pip install .
-pip install --upgrade pip
-pip list
+python -m pip install --upgrade pip
+python -m pip install -e .
+python -m pip install -e ".[dev]"
+python -m pip list
 ```
 
 You can find instructions about how to use this tool in the tests/data jupyter notebook.
 This notebook can be started from the command line inside the ifes_apt_tc_data_modeling
 directory simply by calling.
 
 ```
```

### Comparing `ifes_apt_tc_data_modeling-0.0.6/README.md` & `ifes_apt_tc_data_modeling-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,41 +48,41 @@
 immediate benefit to users. The collection of examples and technical discussions
 via issues serves the more long-term aim. This is to arrive at a detailed technical
 specification rather than more robust parsers only so that atom probe data can be
 exchanged across tools irrespective of their formatting.
 
 # Getting started as developer
 
-You should create a virtual environment. We tested on Ubuntu with Python 3.7.
-Newer versions of Python should work similarly (for this change 3.7) to the
-desired version tag.
+You should create a virtual environment. We tested on Ubuntu with Python 3.8.
+Newer versions of Python should work similarly when using the desired version tag.
 
-If you don't have Python 3.7 installed on your computer, follow these commands:
+If you don't have Python 3.8 installed on your computer, follow these commands:
 ```
 sudo add-apt-repository ppa:deadsnakes/ppa
-sudo apt install python3.7 python3-dev libpython3.7-dev python3.7-venv
+sudo apt install python3.8 python3-dev libpython3.8-dev python3.8-venv
 ```
 
-In some cases when using Python3.7 it was necessary to install python-numpy in others
+In some cases when using Python3.8 it was necessary to install python-numpy in others
 not. So consider this if you run into issues when continuing this manual.
 The following steps will install the ifes_apt_tc_data_modeling module in the
 latest version.
 
 ```
 mkdir <your-brand-new-folder>
 cd <your-brand-new-folder>
 pip install virtualenv
-virtualenv --python=python3.7 .py37
-source .py37/bin/activate
+virtualenv --python=python3.8 .py38
+source .py38/bin/activate
 
 git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
-pip install .
-pip install --upgrade pip
-pip list
+python -m pip install --upgrade pip
+python -m pip install -e .
+python -m pip install -e ".[dev]"
+python -m pip list
 ```
 
 You can find instructions about how to use this tool in the tests/data jupyter notebook.
 This notebook can be started from the command line inside the ifes_apt_tc_data_modeling
 directory simply by calling.
 
 ```
```

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/__init__.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/__init__.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_headers.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_headers.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_reader.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_sections.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_sections.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/apt/apt6_utils.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_utils.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/epos/__init__.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/epos/epos_reader.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/epos_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/nexus/__init__.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/nexus/nx_field.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/nx_field.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/nexus/nx_ion.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/nx_ion.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/pos/__init__.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/pos/pos_reader.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/pos_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rng/__init__.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rng/rng_reader.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/rng_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rrng/__init__.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/rrng/rrng_reader.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/rrng_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/__init__.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/definitions.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/mmapped_io.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/mmapped_io.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/molecular_ions.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/molecular_ions.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,20 +218,16 @@
         # only an isotope_vector whose hashvalues have ALL in common
         # that the number of neutrons is 0, i.e. their hashvalue is the atomic_number
         # element_arr is an isotope_vector/ivec with such hashvalues
         # as an example the molecular ion C:2 H:1 will map to 6, 6, 1
         max_depth = 0  # number of non-zero entries in element_arr
         for hashvalue in element_arr:
             n_protons, n_neutrons = hash_to_isotope(hashvalue)
-            assert n_neutrons == 0, \
-                str(hashvalue) + " in element_arr_in has n_neutrons != 0 !"
             if hashvalue != 0:
                 max_depth += 1
-            # else:
-            #     break
         if self.parms["verbose"] is True:
             print(f"Maximum recursion depth {max_depth}")
         self.candidates = []
         if self.parms["verbose"] is True:
             print(element_arr)
 
         if max_depth > 0:
```

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/string_handling.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/string_handling.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling/utils/utils.py` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,17 +126,15 @@
     """Create a NeXus NXion nuclid list."""
     assert np.shape(ivec) == (MAX_NUMBER_OF_ATOMS_PER_ION,), \
         "Argument isotope_vector needs to be shaped (MAX_NUMBER_OF_ATOMS_PER_ION,) !"
     nuclid_list = np.zeros((2, MAX_NUMBER_OF_ATOMS_PER_ION), np.uint16)
     for idx in np.arange(0, MAX_NUMBER_OF_ATOMS_PER_ION):
         if ivec[idx] != 0:
             protons, neutrons = hash_to_isotope(int(ivec[idx]))
-            if neutrons != 0:
-                nuclid_list[0, idx] = protons + neutrons
-            # else: leave only element name, i.e. number of protons
+            nuclid_list[0, idx] = protons + neutrons
             nuclid_list[1, idx] = protons
     return nuclid_list
 
 
 def isotope_vector_to_dict_keyword(ivec: np.ndarray) -> str:
     """Create keyword for dictionary from isotope_vector."""
     assert len(ivec) <= MAX_NUMBER_OF_ATOMS_PER_ION, \
```

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling.egg-info/PKG-INFO` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifes-apt-tc-data-modeling
-Version: 0.0.6
+Version: 0.0.7
 Summary: Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy.
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -202,19 +202,22 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 # atomprobe-data-modeling
 
 ## Mission:
 Foster exchange about data models and work towards specifications
 of file formats from the research field of atom probe microscopy.
@@ -263,41 +266,41 @@
 immediate benefit to users. The collection of examples and technical discussions
 via issues serves the more long-term aim. This is to arrive at a detailed technical
 specification rather than more robust parsers only so that atom probe data can be
 exchanged across tools irrespective of their formatting.
 
 # Getting started as developer
 
-You should create a virtual environment. We tested on Ubuntu with Python 3.7.
-Newer versions of Python should work similarly (for this change 3.7) to the
-desired version tag.
+You should create a virtual environment. We tested on Ubuntu with Python 3.8.
+Newer versions of Python should work similarly when using the desired version tag.
 
-If you don't have Python 3.7 installed on your computer, follow these commands:
+If you don't have Python 3.8 installed on your computer, follow these commands:
 ```
 sudo add-apt-repository ppa:deadsnakes/ppa
-sudo apt install python3.7 python3-dev libpython3.7-dev python3.7-venv
+sudo apt install python3.8 python3-dev libpython3.8-dev python3.8-venv
 ```
 
-In some cases when using Python3.7 it was necessary to install python-numpy in others
+In some cases when using Python3.8 it was necessary to install python-numpy in others
 not. So consider this if you run into issues when continuing this manual.
 The following steps will install the ifes_apt_tc_data_modeling module in the
 latest version.
 
 ```
 mkdir <your-brand-new-folder>
 cd <your-brand-new-folder>
 pip install virtualenv
-virtualenv --python=python3.7 .py37
-source .py37/bin/activate
+virtualenv --python=python3.8 .py38
+source .py38/bin/activate
 
 git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
-pip install .
-pip install --upgrade pip
-pip list
+python -m pip install --upgrade pip
+python -m pip install -e .
+python -m pip install -e ".[dev]"
+python -m pip list
 ```
 
 You can find instructions about how to use this tool in the tests/data jupyter notebook.
 This notebook can be started from the command line inside the ifes_apt_tc_data_modeling
 directory simply by calling.
 
 ```
```

### Comparing `ifes_apt_tc_data_modeling-0.0.6/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt` & `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 ifes_apt_tc_data_modeling/apt/apt6_headers.py
 ifes_apt_tc_data_modeling/apt/apt6_reader.py
 ifes_apt_tc_data_modeling/apt/apt6_sections.py
 ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
 ifes_apt_tc_data_modeling/apt/apt6_utils.py
 ifes_apt_tc_data_modeling/epos/__init__.py
 ifes_apt_tc_data_modeling/epos/epos_reader.py
+ifes_apt_tc_data_modeling/fig/__init__.py
+ifes_apt_tc_data_modeling/fig/fig_reader.py
 ifes_apt_tc_data_modeling/nexus/__init__.py
 ifes_apt_tc_data_modeling/nexus/nx_field.py
 ifes_apt_tc_data_modeling/nexus/nx_ion.py
 ifes_apt_tc_data_modeling/pos/__init__.py
 ifes_apt_tc_data_modeling/pos/pos_reader.py
 ifes_apt_tc_data_modeling/rng/__init__.py
 ifes_apt_tc_data_modeling/rng/rng_reader.py
```

### Comparing `ifes_apt_tc_data_modeling-0.0.6/pyproject.toml` & `ifes_apt_tc_data_modeling-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifes_apt_tc_data_modeling"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "The NOMAD Authors" },
 ]
 description = "Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy."
 readme = "README.md"
 license = { file = "LICENSE.txt" }
-requires-python = ">=3.7"
+requires-python = ">=3.8,<3.11"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "h5py>=3.6.0",
     "numpy>=1.21.2",
     "pandas>=1.3.2",
     "ase==3.19.0",
     "radioactivedecay>=0.4.16",
-    "jupyterlab_h5web>=6.5.0",
-    "jupyterlab>=3.5.2"
+    "jupyterlab_h5web>=6.6.1",
+    "jupyterlab>=3.5.2,<3.6.0"
+]
+
+[project.optional-dependencies]
+dev = [
+    "twine",
 ]
 
 # [tool.setuptools]
-# packages = ["apt", "epos", "nexus", "pos", "rng", "rrng", "utils"]
+# packages = ["apt", "epos", "nexus", "pos", "rng", "rrng", "fig", "utils"]
```

