# Comparing `tmp/astro-plpy-0.0.1.3.tar.gz` & `tmp/astro-plpy-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-plpy-0.0.1.3.tar", last modified: Thu Apr 13 06:41:15 2023, max compression
+gzip compressed data, was "astro-plpy-0.0.1.4.tar", last modified: Fri Apr 28 04:53:23 2023, max compression
```

## Comparing `astro-plpy-0.0.1.3.tar` & `astro-plpy-0.0.1.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.448483 astro-plpy-0.0.1.3/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    35149 2022-11-28 15:47:52.000000 astro-plpy-0.0.1.3/LICENSE
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      619 2023-04-13 06:41:15.448483 astro-plpy-0.0.1.3/PKG-INFO
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       57 2023-02-06 13:28:21.000000 astro-plpy-0.0.1.3/README.md
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1235 2023-04-02 16:27:41.000000 astro-plpy-0.0.1.3/pyproject.toml
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       35 2023-04-02 16:28:07.000000 astro-plpy-0.0.1.3/requirements.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       38 2023-04-13 06:41:15.448483 astro-plpy-0.0.1.3/setup.cfg
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       37 2023-02-06 13:27:51.000000 astro-plpy-0.0.1.3/setup.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.280477 astro-plpy-0.0.1.3/src/
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.284478 astro-plpy-0.0.1.3/src/astro_plpy.egg-info/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      619 2023-04-13 06:41:15.000000 astro-plpy-0.0.1.3/src/astro_plpy.egg-info/PKG-INFO
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1133 2023-04-13 06:41:15.000000 astro-plpy-0.0.1.3/src/astro_plpy.egg-info/SOURCES.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)        1 2023-04-13 06:41:15.000000 astro-plpy-0.0.1.3/src/astro_plpy.egg-info/dependency_links.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      162 2023-04-13 06:41:15.000000 astro-plpy-0.0.1.3/src/astro_plpy.egg-info/entry_points.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       36 2023-04-13 06:41:15.000000 astro-plpy-0.0.1.3/src/astro_plpy.egg-info/requires.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)        5 2023-04-13 06:41:15.000000 astro-plpy-0.0.1.3/src/astro_plpy.egg-info/top_level.txt
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.304478 astro-plpy-0.0.1.3/src/plpy/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       88 2023-04-08 10:37:08.000000 astro-plpy-0.0.1.3/src/plpy/__init__.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.308478 astro-plpy-0.0.1.3/src/plpy/bak/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     5404 2022-11-28 15:47:52.000000 astro-plpy-0.0.1.3/src/plpy/bak/operations.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2787 2022-11-28 15:47:52.000000 astro-plpy-0.0.1.3/src/plpy/bak/utils.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.348480 astro-plpy-0.0.1.3/src/plpy/bfosc/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      210 2023-03-14 06:01:19.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/__init__.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.384481 astro-plpy-0.0.1.3/src/plpy/bfosc/bak/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    17688 2023-02-06 05:16:25.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_comet_2020.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    14797 2023-02-05 14:35:38.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    15429 2023-02-05 14:35:04.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2021.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    14814 2023-02-05 14:35:22.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2022.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    15273 2023-02-05 14:35:54.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_standard.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    25397 2023-04-11 14:17:01.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/g4.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    19739 2023-02-22 06:49:10.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/g4_old.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.284478 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.420482 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2020a/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    46080 2023-02-05 04:50:01.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2020a/bfosc_g4_slit18_2020a.fits
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      522 2023-02-08 15:20:59.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2020a/bfosc_g4_slit18_2020a.reg
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    46080 2023-02-18 06:25:45.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2020a/bfosc_g4_slit23_2020a.fits
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      505 2023-02-09 07:02:59.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2020a/bfosc_g4_slit23_2020a.reg
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:41:15.436483 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2022b/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    48960 2023-04-02 12:17:57.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2022b/bfosc_g4_slit23_2022b.fits
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2023-04-02 15:34:25.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2022b/bfosc_g4_slit23_2022b.reg
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    10799 2023-04-02 07:04:10.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/phot.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    10323 2023-02-22 07:32:34.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/phot_old.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1225 2023-02-22 06:49:15.000000 astro-plpy-0.0.1.3/src/plpy/bfosc/utils.py
--rwxrwxr-x   0 zrn       (1007) zrn       (1007)     6908 2023-02-06 08:30:39.000000 astro-plpy-0.0.1.3/src/plpy/mst.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3514 2023-02-05 14:36:34.000000 astro-plpy-0.0.1.3/src/plpy/p200_tspec.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2499 2023-04-08 15:26:46.000000 astro-plpy-0.0.1.3/src/plpy/utils.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.393565 astro-plpy-0.0.1.4/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    35149 2022-11-28 15:47:52.000000 astro-plpy-0.0.1.4/LICENSE
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      619 2023-04-28 04:53:23.393565 astro-plpy-0.0.1.4/PKG-INFO
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       57 2023-02-06 13:28:21.000000 astro-plpy-0.0.1.4/README.md
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1259 2023-04-27 18:34:53.000000 astro-plpy-0.0.1.4/pyproject.toml
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       35 2023-04-14 16:58:59.000000 astro-plpy-0.0.1.4/requirements.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       38 2023-04-28 04:53:23.393565 astro-plpy-0.0.1.4/setup.cfg
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       37 2023-02-06 13:27:51.000000 astro-plpy-0.0.1.4/setup.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.077554 astro-plpy-0.0.1.4/src/
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.093555 astro-plpy-0.0.1.4/src/astro_plpy.egg-info/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      619 2023-04-28 04:53:23.000000 astro-plpy-0.0.1.4/src/astro_plpy.egg-info/PKG-INFO
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1132 2023-04-28 04:53:23.000000 astro-plpy-0.0.1.4/src/astro_plpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)        1 2023-04-28 04:53:23.000000 astro-plpy-0.0.1.4/src/astro_plpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      184 2023-04-28 04:53:23.000000 astro-plpy-0.0.1.4/src/astro_plpy.egg-info/entry_points.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       36 2023-04-28 04:53:23.000000 astro-plpy-0.0.1.4/src/astro_plpy.egg-info/requires.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)        5 2023-04-28 04:53:23.000000 astro-plpy-0.0.1.4/src/astro_plpy.egg-info/top_level.txt
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.117555 astro-plpy-0.0.1.4/src/plpy/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       88 2023-04-13 08:15:32.000000 astro-plpy-0.0.1.4/src/plpy/__init__.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.117555 astro-plpy-0.0.1.4/src/plpy/bak/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     5404 2022-11-28 15:47:52.000000 astro-plpy-0.0.1.4/src/plpy/bak/operations.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2787 2022-11-28 15:47:52.000000 astro-plpy-0.0.1.4/src/plpy/bak/utils.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.281561 astro-plpy-0.0.1.4/src/plpy/bfosc/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      210 2023-03-14 06:01:19.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/__init__.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.309562 astro-plpy-0.0.1.4/src/plpy/bfosc/bak/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    17688 2023-02-06 05:16:25.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_comet_2020.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    14797 2023-02-05 14:35:38.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    15429 2023-02-05 14:35:04.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2021.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    14814 2023-02-05 14:35:22.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2022.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    15273 2023-02-05 14:35:54.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_standard.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    40459 2023-04-24 05:56:26.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/g4.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    19739 2023-02-22 06:49:10.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/g4_old.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.345563 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.373564 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/2020a/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      522 2023-02-08 15:20:59.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/2020a/bfosc_g4_slit18_2020a.reg
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      505 2023-02-09 07:02:59.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/2020a/bfosc_g4_slit23_2020a.reg
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:53:23.381564 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/2022b/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      801 2023-04-17 06:32:28.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/2022b/bfosc_g4_slit23_2022b.reg
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    46080 2023-02-05 04:50:01.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/bfosc_g4_slit18_2020a.fits
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    46080 2023-02-18 06:25:45.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/bfosc_g4_slit23_2020a.fits
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    48960 2023-04-02 12:17:57.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/lib/bfosc_g4_slit23_2022b.fits
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    10799 2023-04-02 07:04:10.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/phot.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    10323 2023-02-22 07:32:34.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/phot_old.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1225 2023-02-22 06:49:15.000000 astro-plpy-0.0.1.4/src/plpy/bfosc/utils.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    42989 2023-04-27 20:54:50.000000 astro-plpy-0.0.1.4/src/plpy/fire.py
+-rwxrwxr-x   0 zrn       (1007) zrn       (1007)     6908 2023-02-06 08:30:39.000000 astro-plpy-0.0.1.4/src/plpy/mst.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3514 2023-02-05 14:36:34.000000 astro-plpy-0.0.1.4/src/plpy/p200_tspec.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2929 2023-04-27 19:10:40.000000 astro-plpy-0.0.1.4/src/plpy/utils.py
```

### Comparing `astro-plpy-0.0.1.3/LICENSE` & `astro-plpy-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/PKG-INFO` & `astro-plpy-0.0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-plpy
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Data reduction pipelines developed based on astro-drpy.
 Author-email: Ruining ZHAO <ruiningzhao@mail.bnu.edu.cn>
 Project-URL: Homepage, https://github.com/RuiningZHAO/plpy
 Project-URL: Tracker, https://github.com/RuiningZHAO/plpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `astro-plpy-0.0.1.3/pyproject.toml` & `astro-plpy-0.0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 dynamic = ["version", "dependencies"]
 
 [project.scripts]
 bfosc_g4_old = "plpy.bfosc.g4_old:main"
 bfosc_phot_old = "plpy.bfosc.phot_old:main"
 bfosc_g4 = "plpy.bfosc.g4:main"
 bfosc_phot = "plpy.bfosc.phot:main"
+fire = "plpy.fire:main"
 
 [project.urls]
 "Homepage" = "https://github.com/RuiningZHAO/plpy"
 "Tracker" = "https://github.com/RuiningZHAO/plpy/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
```

### Comparing `astro-plpy-0.0.1.3/src/astro_plpy.egg-info/PKG-INFO` & `astro-plpy-0.0.1.4/src/astro_plpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-plpy
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Data reduction pipelines developed based on astro-drpy.
 Author-email: Ruining ZHAO <ruiningzhao@mail.bnu.edu.cn>
 Project-URL: Homepage, https://github.com/RuiningZHAO/plpy
 Project-URL: Tracker, https://github.com/RuiningZHAO/plpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `astro-plpy-0.0.1.3/src/astro_plpy.egg-info/SOURCES.txt` & `astro-plpy-0.0.1.4/src/astro_plpy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/astro_plpy.egg-info/PKG-INFO
 src/astro_plpy.egg-info/SOURCES.txt
 src/astro_plpy.egg-info/dependency_links.txt
 src/astro_plpy.egg-info/entry_points.txt
 src/astro_plpy.egg-info/requires.txt
 src/astro_plpy.egg-info/top_level.txt
 src/plpy/__init__.py
+src/plpy/fire.py
 src/plpy/mst.py
 src/plpy/p200_tspec.py
 src/plpy/utils.py
 src/plpy/bak/operations.py
 src/plpy/bak/utils.py
 src/plpy/bfosc/__init__.py
 src/plpy/bfosc/g4.py
@@ -22,13 +23,13 @@
 src/plpy/bfosc/phot_old.py
 src/plpy/bfosc/utils.py
 src/plpy/bfosc/bak/drpy_bfosc_g4_comet_2020.py
 src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general.py
 src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2021.py
 src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2022.py
 src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_standard.py
-src/plpy/bfosc/lib/2020a/bfosc_g4_slit18_2020a.fits
+src/plpy/bfosc/lib/bfosc_g4_slit18_2020a.fits
+src/plpy/bfosc/lib/bfosc_g4_slit23_2020a.fits
+src/plpy/bfosc/lib/bfosc_g4_slit23_2022b.fits
 src/plpy/bfosc/lib/2020a/bfosc_g4_slit18_2020a.reg
-src/plpy/bfosc/lib/2020a/bfosc_g4_slit23_2020a.fits
 src/plpy/bfosc/lib/2020a/bfosc_g4_slit23_2020a.reg
-src/plpy/bfosc/lib/2022b/bfosc_g4_slit23_2022b.fits
 src/plpy/bfosc/lib/2022b/bfosc_g4_slit23_2022b.reg
```

### Comparing `astro-plpy-0.0.1.3/src/plpy/bak/operations.py` & `astro-plpy-0.0.1.4/src/plpy/bak/operations.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bak/utils.py` & `astro-plpy-0.0.1.4/src/plpy/bak/utils.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_comet_2020.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_comet_2020.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2021.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2021.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2022.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_general_2022.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_standard.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/bak/drpy_bfosc_g4_slit23_standard.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/g4.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/g4_old.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 """
 BFOSC/G4 pipeline
 """
 
-import os, argparse, warnings
+import os, argparse
+from copy import deepcopy
 
 # NumPy
 import numpy as np
 # AstroPy
-import astropy.units as u
-from astropy.io import fits
 from astropy.stats import mad_std
 from astropy.nddata import CCDData
 # ccdproc
 from ccdproc import ImageFileCollection
-from ccdproc.utils.slices import slice_from_string
 # drpy
 from drpy.batch import CCDDataList
 from drpy.image import concatenate
 from drpy.utils import imstatistics
 from drpy.plotting import plot2d, plotSpectrum1D
-from drpy.twodspec.longslit import (response, illumination, align, fitcoords, 
-                                    transform, extract)
+from drpy.twodspec.longslit import (response, illumination, fitcoords, transform, 
+                                    extract)
 from drpy.twodspec.utils import invertCoordinateMap
 from drpy.onedspec import dispcor, saveSpectrum1D
 
 from ..utils import makeDirectory, modifyHeader
 from .utils import LIBRARY_PATH, login, loadLists, getMask
 
 
-def pipeline(save_dir, data_dir, hdu, keywords, steps, fits_section, slit_along, 
-             n_piece, sigma, index, custom_mask, reference, combine, keyword, dtype, 
+def pipeline(save_dir, data_dir, hdu, keywords, steps, row_range, col_range, 
+             slit_along, n_piece, sigma, index, rdnoise, gain, custom_mask, reference, 
              mem_limit, show, save, verbose, mode): 
     """BFOSC/G4 pipeline."""
     
     # Login message
     if verbose:
         login('Grism 4')
     
@@ -42,72 +40,66 @@
         print('\n[MAKE DIRECTORIES]')
         print(f'  - Changing working directory to {save_dir}...')
     os.chdir(save_dir)
     fig_path = makeDirectory(parent='', child='fig', verbose=verbose)
     pro_path = makeDirectory(parent='', child='pro', verbose=verbose)
     cal_path = makeDirectory(parent='', child='cal', verbose=verbose)
     
+    # Load lists
+    list_dict = loadLists(list_names=['lamp', 'targ'])
+    
     # Construct image file collection
     ifc = ImageFileCollection(
         location=data_dir, keywords=keywords, find_fits_by_reading=False, 
         filenames=None, glob_include='*.fit', glob_exclude=None, ext=hdu)
-    
+
     # Modify fits header
     #   Note that image file collection is constructed before header modification.
     if 'header' in steps:
         if verbose:
             print('\n[HEADER MODIFICATION]')
         for file_name in ifc.files_filtered(include_path=True):
             modifyHeader(file_name, verbose=verbose)
     
-    # Load gain and readout noise
-    first_file = ifc.files_filtered(include_path=True)[0]
-    gain = fits.getval(first_file, 'GAIN', ext=hdu) * u.photon / u.adu
-    rdnoise = fits.getval(first_file, 'RDNOISE', ext=hdu) * u.photon
-    
     if 'trim' in steps:
-        custom_mask = custom_mask[slice_from_string(fits_section, fits_convention=True)]
+        custom_mask = custom_mask[row_range[0]:row_range[1], col_range[0]:col_range[1]]
         trim = True
     else:
         trim = False
     
     # Bias combination
     if ('bias.combine' in steps) or ('bias' in steps):
         
         if verbose:
             print('\n[BIAS COMBINATION]')
         
-        # Load bias
         if verbose:
             print('  - Loading bias...')
+        # Filter
         ifc_bias = ifc.filter(regex_match=True, imagetyp='Bias Frame')
+        # Load bias
         bias_list = CCDDataList.read(
             file_list=ifc_bias.files_filtered(include_path=True), hdu=hdu)
-
+        
         # Trim
         if trim:
             if verbose:
                 print('  - Trimming...')
-            bias_list = bias_list.trim_image(fits_section=fits_section)
-        
-        # Correct gain
-        if verbose:
-            print('  - Correcting gain...')
-        bias_list_gain_corrected = bias_list.gain_correct(gain=gain)
-        
-        bias_list_gain_corrected.statistics(verbose=verbose)
+            bias_list = bias_list.trim(row_range=row_range, col_range=col_range)
         
+        bias_list.statistics(verbose=verbose)
+
         # Combine bias
         if verbose:
             print('  - Combining...')
-        master_bias = bias_list_gain_corrected.combine(
-            method='average', mem_limit=mem_limit, sigma_clip=True, 
-            sigma_clip_low_thresh=3, sigma_clip_high_thresh=3, 
-            sigma_clip_func=np.ma.median, sigma_clip_dev_func=mad_std, 
-            output_file=os.path.join(cal_path, 'master_bias.fits'), dtype=dtype, 
+        master_bias = bias_list.combine(
+            method='average', sigma_clip=True, sigma_clip_low_thresh=3, 
+            sigma_clip_high_thresh=3, sigma_clip_func=np.ma.median, 
+            sigma_clip_dev_func=mad_std, mem_limit=mem_limit, 
+            output_file=os.path.join(cal_path, 'master_bias.fits'), 
             overwrite_output=True)
         
         imstatistics(master_bias, verbose=verbose)
         
         # Plot master bias
         plot2d(
             master_bias.data, title='master bias', show=show, save=save, path=fig_path)
@@ -120,61 +112,58 @@
         
         if verbose:
             print('\n[LAMP CONCATENATION]')
         
         # Load lamp
         if verbose:
             print('  - Loading lamp...')
-        ifc_lamp = ifc.filter(regex_match=True, obstype='SPECLLAMP')
+        ifc_lamp = ImageFileCollection(
+            location=data_dir, keywords=keywords, find_fits_by_reading=False, 
+            filenames=list_dict['lamp'], glob_include=None, glob_exclude=None, ext=hdu)
         lamp_list = CCDDataList.read(
             file_list=ifc_lamp.files_filtered(include_path=True), hdu=hdu)
-
+        
         # Trim
         if trim:
             if verbose:
                 print('  - Trimming...')
-            lamp_list = lamp_list.trim_image(fits_section=fits_section)
+            lamp_list = lamp_list.trim(row_range=row_range, col_range=col_range)
         
-        # Correct gain
-        if verbose:
-            print('  - Correcting gain...')
-        lamp_list_gain_corrected = lamp_list.gain_correct(gain=gain)
-        
-        lamp_list_gain_corrected.statistics(verbose=verbose)
+        lamp_list.statistics(verbose=verbose)
         
         # Subtract bias
         #   Uncertainties created here (equal to that of ``master_bias``) are useless!!!
         if verbose:
             print('  - Subtracting bias...')
         if 'master_bias' not in locals():
             master_bias = CCDData.read(os.path.join(cal_path, 'master_bias.fits'))
-        lamp_list_bias_subtracted = lamp_list_gain_corrected.subtract_bias(master_bias)
+        lamp_list_bias_subtracted = lamp_list - master_bias
         
         lamp_list_bias_subtracted.statistics(verbose=verbose)
         
         # Create real uncertainty!!!
         if verbose:
             print('  - Creating deviation...')
         lamp_list_bias_subtracted_with_deviation = (
             lamp_list_bias_subtracted.create_deviation(
-                gain=None, readnoise=rdnoise, disregard_nan=True)
+                gain=gain, readnoise=rdnoise, disregard_nan=True)
         )
         
         # Concatenate
         if verbose:
             print('  - Concatenating...')
         # Ensure that the first is the short exposure
         exptime = ifc_lamp.summary['exptime'].data
         if exptime[0] > exptime[1]:
             lamp_list_bias_subtracted_with_deviation = (
                 lamp_list_bias_subtracted_with_deviation[::-1]
             )
         concatenated_lamp = concatenate(
-            lamp_list_bias_subtracted_with_deviation, fits_section=f'[:{index}, :]', 
-            scale=None)
+            lamp_list_bias_subtracted_with_deviation, row_range=(0, None), 
+            col_range=(0, index), scale=None)
         
         # Plot concatenated lamp
         plot2d(
             concatenated_lamp.data, title='concatenated lamp', show=show, save=save, 
             path=fig_path)
         
         # Write concatenated lamp to file
@@ -232,86 +221,85 @@
         
         # Extract 1-dimensional spectrum
         if verbose:
             print('  - Extracting 1-dimensional lamp spectrum')
         if 'transformed_lamp' not in locals():
             transformed_lamp = CCDData.read(
                 os.path.join(cal_path, 'transformed_lamp.fits'))
-        # Of type float64
         lamp1d = extract(
-            ccd=transformed_lamp, slit_along=slit_along, trace1d=750, aper_width=10, 
-            method='sum', n_aper=1, title='lamp', show=show, save=save, path=fig_path)
+            ccd=transformed_lamp, slit_along=slit_along, trace1d=750, n_aper=1, 
+            aper_width=10, show=show, save=save, path=fig_path)
 
         # Correct dispersion
         if verbose:
             print('  - Correcting dispersion axis...')
-        # Of type float64
         calibrated_lamp1d = dispcor(
-            spectrum1d=lamp1d, reverse=True, reference=reference, n_piece=3, 
-            refit=True, n_iter=5, sigma_lower=3, sigma_upper=3, grow=False, 
-            use_mask=True, show=show, save=save, path=fig_path)
+            spectrum1d=lamp1d, reverse=True, reference=reference, n_piece=3, refit=True, 
+            n_iter=5, sigma_lower=3, sigma_upper=3, grow=False, use_mask=True, show=show, 
+            save=save, path=fig_path)
+
+        # Plot calibrated lamp spectrum
+        plotSpectrum1D(
+            spectrum1d=calibrated_lamp1d, title='calibrated lamp', show=show, save=save, 
+            path=fig_path)
 
         # Write calibrated lamp spectrum to file
-        # Of type float64
         saveSpectrum1D(
             os.path.join(cal_path, 'lamp1d.fits'), calibrated_lamp1d, overwrite=True)
         
     # Flat combination
     if ('flat.combine' in steps) or ('flat' in steps):
         
         if verbose:
             print('\n[FLAT COMBINATION]')
-        
-        # Load flat
+            
         if verbose:
             print('  - Loading flat...')
-        ifc_flat = ifc.filter(regex_match=True, obstype='SPECLFLAT')
+        # Filter
+        ifc_flat = ifc.filter(regex_match=True, imagetyp='Flat Field')
+        # Load flat
         flat_list = CCDDataList.read(
             file_list=ifc_flat.files_filtered(include_path=True), hdu=hdu)
         
         # Trim
         if trim:
             if verbose:
                 print('  - Trimming...')
-            flat_list = flat_list.trim_image(fits_section=fits_section)
-        
-        # Correct gain
-        if verbose:
-            print('  - Correcting gain...')
-        flat_list_gain_corrected = flat_list.gain_correct(gain=gain)
+            flat_list = flat_list.trim(row_range=row_range, col_range=col_range)
         
-        flat_list_gain_corrected.statistics(verbose=verbose)
+        flat_list.statistics(verbose=verbose)
 
         # Subtract bias
         #   Uncertainties created here (equal to that of ``master_bias``) are useless!!!
         if verbose:
             print('  - Subtracting bias...')
         if 'master_bias' not in locals():
             master_bias = CCDData.read(os.path.join(cal_path, 'master_bias.fits'))
-        flat_list_bias_subtracted = flat_list_gain_corrected.subtract_bias(master_bias)
+        flat_list_bias_subtracted = flat_list - master_bias
         
         flat_list_bias_subtracted.statistics(verbose=verbose)
 
         # Combine flat
         #   Uncertainties created above are overwritten here!!!
         if verbose:
             print('  - Combining...')
         scaling_func = lambda ccd: 1 / np.ma.average(ccd)
         combined_flat = flat_list_bias_subtracted.combine(
-            method='average', scale=scaling_func, mem_limit=mem_limit, sigma_clip=True, 
+            method='average', scale=scaling_func, sigma_clip=True, 
             sigma_clip_low_thresh=3, sigma_clip_high_thresh=3, 
             sigma_clip_func=np.ma.median, sigma_clip_dev_func=mad_std, 
-            output_file=os.path.join(cal_path, 'combined_flat.fits'), dtype=dtype, 
+            mem_limit=mem_limit, 
+            output_file=os.path.join(cal_path, 'combined_flat.fits'), 
             overwrite_output=True)
 
         imstatistics(combined_flat, verbose=verbose)
         
         # Plot combined flat
         plot2d(
-            combined_flat.data, title='combined flat', show=show, save=save, 
+            combined_flat.data, title='combined_flat', show=show, save=save, 
             path=fig_path)
         
         # Release memory
         del flat_list, flat_list_bias_subtracted
 
     # Response
     if ('flat.normalize.response' in steps) or \
@@ -320,19 +308,18 @@
         
         if verbose:
             print('\n[RESPONSE]')
         
         # Response calibration
         if 'combined_flat' not in locals():
             combined_flat = CCDData.read(os.path.join(cal_path, 'combined_flat.fits'))
-        combined_flat.mask |= custom_mask
         reflat = response(
-            ccd=combined_flat, slit_along=slit_along, n_piece=n_piece, n_iter=1, 
-            sigma_lower=7, sigma_upper=7, grow=False, use_mask=True, show=show, 
-            save=save, path=fig_path)
+            ccd=combined_flat, slit_along=slit_along, n_piece=n_piece, n_iter=5, 
+            sigma_lower=3, sigma_upper=3, grow=10, use_mask=True, show=show, save=save, 
+            path=fig_path)
 
         imstatistics(reflat, verbose=verbose)
         
         # Plot response calibrated flat
         plot2d(reflat.data, title='reflat', show=show, save=save, path=fig_path)
         
         # Plot response mask
@@ -350,14 +337,15 @@
 
         if verbose:
             print('\n[ILLUMINATION]')
         
         # Illumination modeling
         if 'reflat' not in locals():
             reflat = CCDData.read(os.path.join(cal_path, 'reflat.fits'))
+        reflat.mask |= custom_mask
         ilflat = illumination(
             ccd=reflat, slit_along=slit_along, method='Gaussian2D', sigma=sigma, 
             bins=10, n_iter=5, sigma_lower=3, sigma_upper=3, grow=5, use_mask=True, 
             show=show, save=save, path=fig_path)
 
         imstatistics(ilflat, verbose=verbose)
 
@@ -370,284 +358,164 @@
             show=show, save=save, path=fig_path)
         
         # Write illumination to file
         ilflat.write(os.path.join(cal_path, 'illumination.fits'), overwrite=True)
 
     # Flat normalization
     if ('flat.normalize' in steps) or ('flat' in steps):
-        
         if verbose:
             print('\n[FLAT NORMALIZATION]')
-        
         # Normalization
-        if 'reflat' not in locals():
-            reflat = CCDData.read(os.path.join(cal_path, 'reflat.fits'))
-        if 'ilflat' not in locals():
-            ilflat = CCDData.read(os.path.join(cal_path, 'ilflat.fits'))
         normalized_flat = reflat.divide(ilflat, handle_meta='first_found')
-        
         # Plot normalized flat
         plot2d(
             normalized_flat.data, title='normalized flat', show=show, save=save, 
             path=fig_path)
-        
         # Write normalized flat to file
         normalized_flat.write(
             os.path.join(cal_path, 'normalized_flat.fits'), overwrite=True)
-        
         # [can be replaced by a pre-defined custom mask]
         normalized_flat.mask = None
 
     # Correct targets
     if ('targ' in steps):
         
         if verbose:
             print('\n[TARGET CORRECTION]')
         
         # Load targ
         if verbose:
             print('  - Loading targ...')
-        ifc_targ = ifc.filter(regex_match=True, obstype='SPECLTARGET|SPECLFLUXREF')
+        ifc_targ = ImageFileCollection(
+            location=data_dir, keywords=keywords, find_fits_by_reading=False, 
+            filenames=list_dict['targ'], glob_include=None, glob_exclude=None, ext=hdu)
         targ_list = CCDDataList.read(
             file_list=ifc_targ.files_filtered(include_path=True), hdu=hdu)
         
         # Trim
         if trim:
             if verbose:
                 print('  - Trimming...')
-            targ_list = targ_list.trim_image(fits_section=fits_section)
-        
-        # Correct gain
-        if verbose:
-            print('  - Correcting gain...')
-        targ_list_gain_corrected = targ_list.gain_correct(gain=gain)
-        
-        targ_list_gain_corrected.statistics(verbose=verbose)
-        
+            targ_list = targ_list.trim(row_range=row_range, col_range=col_range)
+
+        targ_list.statistics(verbose=verbose)
+
         # Subtract bias
         #   Uncertainties created here (equal to that of ``master_bias``) are useless!!!
         if verbose:
             print('  - Subtracting bias...')
         if 'master_bias' not in locals():
             master_bias = CCDData.read(os.path.join(cal_path, 'master_bias.fits'))
-        targ_list_bias_subtracted = targ_list_gain_corrected.subtract_bias(master_bias)
+        targ_list_bias_subtracted = targ_list - master_bias
         
         targ_list_bias_subtracted.statistics(verbose=verbose)
 
         # Create real uncertainty!!!
         if verbose:
             print('  - Creating deviation...')
         targ_list_bias_subtracted_with_deviation = (
             targ_list_bias_subtracted.create_deviation(
-                gain=None, readnoise=rdnoise, disregard_nan=True)
+                gain=gain, readnoise=rdnoise, disregard_nan=True)
         )
         
         # Flat-fielding
         if verbose:
             print('  - Flat-fielding...')
         if 'normalized_flat' not in locals():
-            normalized_flat = CCDData.read(
-                os.path.join(cal_path, 'normalized_flat.fits'))
+            normalized_flat = CCDData.read(os.path.join(cal_path, 'normalized_flat.fits'))
         targ_list_flat_fielded = (
-            targ_list_bias_subtracted_with_deviation.flat_correct(normalized_flat)
+            targ_list_bias_subtracted_with_deviation / normalized_flat
         )
-        
-        # Group
-        ifc_targ_summary = ifc_targ.summary
-        ifc_targ_summary_grouped = ifc_targ_summary.group_by(keyword)
-        keys = ifc_targ_summary_grouped.groups.keys[keyword].data
+
+        # Remove cosmic ray
         if verbose:
-            print('  - Grouping')
-            print(f'    - {keys.shape[0]} groups: ' + ', '.join(keys))
-        
-        for key in keys:
+            print('  - Removing cosmic ray...')
+        targ_list_cosmicray_corrected = targ_list_flat_fielded.cosmicray(
+            method='Laplacian', use_mask=False, gain=gain, readnoise=rdnoise, sigclip=4.5, 
+            sigfrac=0.3, objlim=1, niter=5, verbose=True)
+
+        # Rectify curvature
+        if verbose:
+            print('  - Rectifying curvature...')
+        if 'X' not in locals():
+            X = np.load(os.path.join(cal_path, 'X.npy'))
+        if 'Y' not in locals():
+            Y = np.load(os.path.join(cal_path, 'Y.npy'))
+        for i, targ_cosmicray_corrected in enumerate(targ_list_cosmicray_corrected):
             
-            if verbose:
-                print(f'  - Dealing with group {key}...')
-            mask = ifc_targ_summary[keyword].data == key
+            old_name = targ_cosmicray_corrected.header['FILENAME']
+            new_name = f'{os.path.splitext(old_name)[0]}_corrected.fits'
+
+            transformed_targ = transform(ccd=targ_cosmicray_corrected, X=X, Y=Y)
+
+            # Plot transformed spectrum
+            plot2d(
+                transformed_targ.data, title=old_name, show=show, save=save, 
+                path=fig_path)
             
-            if (mask.sum() > 1) & combine:
-                
-                new_name = f'{key}.fits'
-                
-                # Skip cosmic ray removal
-                if mask.sum() >= 3:
-                
-                    # Rectify curvature
-                    if verbose:
-                        print('    - Rectifying curvature...')
-                    if 'X' not in locals():
-                        X = np.load(os.path.join(cal_path, 'X.npy'))
-                    if 'Y' not in locals():
-                        Y = np.load(os.path.join(cal_path, 'Y.npy'))
-                    targ_list_transformed = targ_list_flat_fielded[mask].apply_over_ccd(
-                        transform, X=X, Y=Y)
-                    
-                else:
-                    
-                    # Remove cosmic ray
-                    if verbose:
-                        print('    - Removing cosmic ray...')
-                    targ_list_cosmicray_corrected = (
-                        targ_list_flat_fielded[mask].cosmicray_lacosmic(
-                            use_mask=False, gain=(1 * u.dimensionless_unscaled), 
-                            readnoise=rdnoise, sigclip=4.5, sigfrac=0.3, objlim=1, 
-                            niter=5, verbose=True)
-                    )
-                    
-                    # Rectify curvature
-                    if verbose:
-                        print('    - Rectifying curvature...')
-                    if 'X' not in locals():
-                        X = np.load(os.path.join(cal_path, 'X.npy'))
-                    if 'Y' not in locals():
-                        Y = np.load(os.path.join(cal_path, 'Y.npy'))
-                    targ_list_transformed = (
-                        targ_list_cosmicray_corrected.apply_over_ccd(
-                            transform, X=X, Y=Y)
-                    )
-                    
-                # Align
-                if verbose:
-                    print('    - Aligning...')
-                targ_list_aligned = align(
-                    targ_list_transformed, slit_along, index=0)
-
-                # Combine
-                if verbose:
-                    print('    - Combining...')
-                exptime = ifc_targ_summary['exptime'].data[mask]
-                scale = exptime.max() / exptime
-                target = targ_list_aligned.combine(
-                    method='average', scale=scale, mem_limit=mem_limit, 
-                    sigma_clip=True, sigma_clip_low_thresh=3, sigma_clip_high_thresh=3, 
-                    sigma_clip_func=np.ma.median, sigma_clip_dev_func=mad_std, 
-                    output_file=os.path.join(pro_path, new_name), dtype=dtype, 
-                    overwrite_output=True)
-                if verbose:
-                    print(f'    - Saving {new_name} to {pro_path}...')
-                
-                # Plot
-                plot2d(
-                    target.data, title=new_name, show=show, save=save, path=fig_path)
-                    
-            else:
-                
-                # Remove cosmic ray
-                if verbose:
-                    print('    - Removing cosmic ray...')
-                targ_list_cosmicray_corrected = (
-                    targ_list_flat_fielded[mask].cosmicray_lacosmic(
-                        use_mask=False, gain=(1 * u.dimensionless_unscaled), 
-                        readnoise=rdnoise, sigclip=4.5, sigfrac=0.3, objlim=1, 
-                        niter=5, verbose=True)
-                )
-
-                # Rectify curvature
-                if verbose:
-                    print('    - Rectifying curvature...')
-                if 'X' not in locals():
-                    X = np.load(os.path.join(cal_path, 'X.npy'))
-                if 'Y' not in locals():
-                    Y = np.load(os.path.join(cal_path, 'Y.npy'))
-                targ_list_transformed = targ_list_cosmicray_corrected.apply_over_ccd(
-                        transform, X=X, Y=Y)
-                
-                n = int(np.log10(mask.sum())) + 1
-                
-                for i, targ_transformed in enumerate(targ_list_transformed):
-
-                    # old_name = targ_transformed.header['FILENAME']
-                    if mask.sum() == 1:
-                        new_name = f'{key}.fits'
-                    else:
-                        new_name = f'{key}_{(i + 1):0{n}d}.fits'
-
-                    # Plot
-                    plot2d(
-                        targ_transformed.data, title=new_name, show=show, save=save, 
-                        path=fig_path)
-
-                    # Write transformed spectrum to file
-                    if verbose:
-                        print(f'    - Saving {new_name} to {pro_path}...')
-                    targ_transformed.write(
-                        os.path.join(pro_path, new_name), overwrite=True)
+            # Write transformed spectrum to file
+            if verbose:
+                print(f'  - Saving {new_name} to {pro_path}...')
+            transformed_targ.write(
+                os.path.join(pro_path, new_name), overwrite=True)
 
 
 def main():
     """Command line tool."""
     
     # External parameters
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        '-i', '--input_dir', required=True, type=str, 
-        help='Input (data) directory.'
+        '-i', '--data_dir', required=True, type=str, 
+        help='Data (input) directory.'
     )
     parser.add_argument(
         '-s', '--semester', required=True, type=str, 
         help='Observation semester.'
     )
     parser.add_argument(
         '-w', '--slit_width', required=True, type=float, choices=[1.8, 2.3], 
         help='Slit width.'
     )
     parser.add_argument(
-        '-o', '--output_dir', default='', type=str, 
-        help='Output (saving) directory.'
+        '-o', '--save_dir', default='', type=str, 
+        help='Saving (output) directory.'
     )
     parser.add_argument(
         '-r', '--reference', default=None, type=str, 
         help='Reference spectrum for wavelength calibration.'
     )
     parser.add_argument(
-        '-c', '--combine', action='store_true', 
-        help='Combine or not.'
-    )
-    parser.add_argument(
-        '-k', '--keyword', default='object', type=str, 
-        help='Keyword for grouping.'
-    )
-    parser.add_argument(
-        '-v', '--verbose', action='store_true', 
-        help='Verbose or not.'
-    )
-    parser.add_argument(
         '-m', '--mode', default='general', type=str, choices=['general', 'standard'], 
         help='General or standard.'
     )
         
     # Parse
     args = parser.parse_args()
-    data_dir = os.path.abspath(args.input_dir)
+    data_dir = os.path.abspath(args.data_dir)
     semester = args.semester
     slit_width = str(args.slit_width).replace('.', '')
-    save_dir = os.path.abspath(args.output_dir)
+    save_dir = os.path.abspath(args.save_dir)
     reference = args.reference
-    combine = args.combine
-    keyword = args.keyword
-    verbose = args.verbose
     mode = args.mode
     
-    # steps = ['header', 'trim', 'bias', 'lamp', 'flat', 'targ']
-    steps = ['trim', 'lamp', 'targ']
-
     # Internal parameters
     hdu = 0
     shape = (2048, 2048)
+    keywords = ['imagetyp', 'object', 'exptime']
+    steps = ['header', 'trim', 'bias', 'lamp', 'flat', 'targ']
+    # steps = ['trim', 'flat', 'targ']
+    row_range = (329, 1830)
+    col_range = (0, 1900)
     slit_along = 'col'
-    keywords = [
-        'date-obs', 'obstype', 'object', 'ra', 'dec', 'filter', 'exptime', 'rdnoise', 
-        'gain']
-    
-    fits_section = '[1:1900, 330:1830]'
     index = 665
     n_piece = 23
     sigma = (20, 30)
-    dtype = 'float32'
+    rdnoise = 4.64
+    gain = 1.41
     
     semester_path = os.path.join(LIBRARY_PATH, semester)
     if not os.path.exists(semester_path):
         raise ValueError('Semester not found.')
     
     # Note that slit18 can be used to calibrate slit23
     if not reference:
@@ -657,22 +525,16 @@
         reference = os.path.abspath(reference)
     if not os.path.exists(reference):
         raise ValueError('Reference not found.')
     
     region = os.path.join(semester_path, f'bfosc_g4_slit{slit_width}_{semester}.reg')
     custom_mask = getMask(region_name=region, shape=shape)
     
-    with warnings.catch_warnings():
-        
-        # Filter warnings
-        warnings.simplefilter('ignore', RuntimeWarning)
-        
-        # Run pipeline
-        pipeline(
-            save_dir=save_dir, data_dir=data_dir, hdu=hdu, keywords=keywords, 
-            steps=steps, fits_section=fits_section, slit_along=slit_along, 
-            n_piece=n_piece, sigma=sigma, index=index, custom_mask=custom_mask, 
-            reference=reference, combine=combine, keyword=keyword, dtype=dtype, 
-            mem_limit=500e6, show=False, save=True, verbose=verbose, mode=mode)
+    pipeline(
+        save_dir=save_dir, data_dir=data_dir, hdu=hdu, keywords=keywords, steps=steps, 
+        row_range=row_range, col_range=col_range, slit_along=slit_along, 
+        n_piece=n_piece, sigma=sigma, index=index, rdnoise=rdnoise, gain=gain, 
+        custom_mask=custom_mask, reference=reference, mem_limit=500e6, show=False, 
+        save=True, verbose=True, mode=mode)
 
 if __name__ == '__main__':
-        main()
+    main()
```

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2020a/bfosc_g4_slit18_2020a.fits` & `astro-plpy-0.0.1.4/src/plpy/bfosc/lib/bfosc_g4_slit18_2020a.fits`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2020a/bfosc_g4_slit18_2020a.reg` & `astro-plpy-0.0.1.4/src/plpy/bfosc/lib/2020a/bfosc_g4_slit18_2020a.reg`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2020a/bfosc_g4_slit23_2020a.fits` & `astro-plpy-0.0.1.4/src/plpy/bfosc/lib/bfosc_g4_slit23_2020a.fits`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2022b/bfosc_g4_slit23_2022b.fits` & `astro-plpy-0.0.1.4/src/plpy/bfosc/lib/bfosc_g4_slit23_2022b.fits`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/lib/2022b/bfosc_g4_slit23_2022b.reg` & `astro-plpy-0.0.1.4/src/plpy/bfosc/lib/2022b/bfosc_g4_slit23_2022b.reg`

 * *Files 11% similar despite different names*

```diff
@@ -8,7 +8,9 @@
 box(441.26968,1030.0857,32.308961,2156.9363,0)
 box(1027.5799,2020.8376,2100.0306,72.236925,0)
 box(932.12395,142.67756,1888.4796,41.278243,0)
 box(911.92992,1260.223,1837.824,32.34816,0)
 box(911.80985,1358.1799,1838.0641,65.35984,0)
 box(910.82333,1302.8233,1833.3133,21.313333,0)
 box(913.45128,1410.9683,1841.1454,11.007938,0)
+box(-6.5208617,1029.5647,21.182882,2114.6175,0)
+box(1026.5,-1.0876522,2063,7.8246956,0)
```

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/phot.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/phot.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/phot_old.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/phot_old.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/bfosc/utils.py` & `astro-plpy-0.0.1.4/src/plpy/bfosc/utils.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/mst.py` & `astro-plpy-0.0.1.4/src/plpy/mst.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/p200_tspec.py` & `astro-plpy-0.0.1.4/src/plpy/p200_tspec.py`

 * *Files identical despite different names*

### Comparing `astro-plpy-0.0.1.3/src/plpy/utils.py` & `astro-plpy-0.0.1.4/src/plpy/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,21 +14,31 @@
         print(f'  - Making {path}...')
         
     os.makedirs(path, exist_ok=True)
     
     return path
 
 
-def modifyHeader(file_name, verbose=False):
+def modifyHeader(file_name, verbose=False, **kwargs):
     """Modify fits header."""
     
-    with fits.open(file_name, 'update') as f:
+    with fits.open(file_name, mode='update', **kwargs) as f:
         
         for hdu in f:
             
+            # `FILE` to `FILENAME`
+            if ('FILE' in hdu.header) & ('FILENAME' not in hdu.header):
+                
+                if verbose:
+                    print(f'{file_name}: rename `FILE` to `FILENAME`.')
+                
+                hdu.header['FILENAME'] = (
+                    hdu.header['FILE'], hdu.header.comments['FILE'])
+                del hdu.header['FILE']
+            
             # `RADECSYS` -> `RADESYSa`
             if ('RADECSYS' in hdu.header) & ('RADESYSa' not in hdu.header):
                 
                 if verbose:
                     print(f'{file_name}: rename `RADECSYS` to `RADESYSa`.')
                 
                 hdu.header['RADESYSa'] = (
```

