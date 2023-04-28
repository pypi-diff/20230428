# Comparing `tmp/MOMORING-1.4.1.tar.gz` & `tmp/MOMORING-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MOMORING-1.4.1.tar", last modified: Fri Apr 28 10:34:28 2023, max compression
+gzip compressed data, was "MOMORING-1.4.2.tar", last modified: Fri Apr 28 10:37:14 2023, max compression
```

## Comparing `MOMORING-1.4.1.tar` & `MOMORING-1.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:34:28.139000 MOMORING-1.4.1/
-drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:34:28.137000 MOMORING-1.4.1/MOMORING/
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/__init__.py
-drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:34:28.138000 MOMORING-1.4.1/MOMORING/api/
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/api/__init__.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     1708 2023-04-28 10:33:49.000000 MOMORING-1.4.1/MOMORING/api/create_project.py
-drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:34:28.138000 MOMORING-1.4.1/MOMORING/applications/
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/applications/__init__.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      557 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/applications/cmd.py
-drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:34:28.138000 MOMORING-1.4.1/MOMORING/modules/
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/modules/__init__.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      581 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/modules/create.py
-drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:34:28.139000 MOMORING-1.4.1/MOMORING/modules/files/
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/modules/files/__init__.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      234 2023-04-28 10:18:01.000000 MOMORING-1.4.1/MOMORING/modules/files/applications_init_template.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      118 2023-04-28 10:18:58.000000 MOMORING-1.4.1/MOMORING/modules/files/applications_template.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     1953 2023-04-28 10:20:35.000000 MOMORING-1.4.1/MOMORING/modules/files/git_ignore_template.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      523 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/modules/files/main_template.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     4040 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/modules/files/nitrogen_utils.py
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      447 2023-04-28 10:22:53.000000 MOMORING-1.4.1/MOMORING/modules/files/readme_template.py
-drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:34:28.139000 MOMORING-1.4.1/MOMORING/utils/
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.1/MOMORING/utils/__init__.py
-drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:34:28.138000 MOMORING-1.4.1/MOMORING.egg-info/
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      149 2023-04-28 10:34:27.000000 MOMORING-1.4.1/MOMORING.egg-info/PKG-INFO
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      740 2023-04-28 10:34:28.000000 MOMORING-1.4.1/MOMORING.egg-info/SOURCES.txt
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        1 2023-04-28 10:34:27.000000 MOMORING-1.4.1/MOMORING.egg-info/dependency_links.txt
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)       55 2023-04-28 10:34:27.000000 MOMORING-1.4.1/MOMORING.egg-info/entry_points.txt
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        6 2023-04-28 10:34:27.000000 MOMORING-1.4.1/MOMORING.egg-info/requires.txt
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        9 2023-04-28 10:34:28.000000 MOMORING-1.4.1/MOMORING.egg-info/top_level.txt
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      149 2023-04-28 10:34:28.139000 MOMORING-1.4.1/PKG-INFO
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      218 2023-04-28 10:25:13.000000 MOMORING-1.4.1/README.md
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)       38 2023-04-28 10:34:28.139000 MOMORING-1.4.1/setup.cfg
--rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      408 2023-04-28 10:34:03.000000 MOMORING-1.4.1/setup.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:37:14.797000 MOMORING-1.4.2/
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:37:14.795000 MOMORING-1.4.2/MOMORING/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/__init__.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:37:14.796000 MOMORING-1.4.2/MOMORING/api/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/api/__init__.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     1708 2023-04-28 10:33:49.000000 MOMORING-1.4.2/MOMORING/api/create_project.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:37:14.796000 MOMORING-1.4.2/MOMORING/applications/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/applications/__init__.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      321 2023-04-28 10:36:44.000000 MOMORING-1.4.2/MOMORING/applications/cmd.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:37:14.796000 MOMORING-1.4.2/MOMORING/modules/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/modules/__init__.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      581 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/modules/create.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:37:14.796000 MOMORING-1.4.2/MOMORING/modules/files/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/modules/files/__init__.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      234 2023-04-28 10:18:01.000000 MOMORING-1.4.2/MOMORING/modules/files/applications_init_template.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      118 2023-04-28 10:18:58.000000 MOMORING-1.4.2/MOMORING/modules/files/applications_template.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     1953 2023-04-28 10:20:35.000000 MOMORING-1.4.2/MOMORING/modules/files/git_ignore_template.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      523 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/modules/files/main_template.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     4040 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/modules/files/nitrogen_utils.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      447 2023-04-28 10:22:53.000000 MOMORING-1.4.2/MOMORING/modules/files/readme_template.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:37:14.796000 MOMORING-1.4.2/MOMORING/utils/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.2/MOMORING/utils/__init__.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:37:14.795000 MOMORING-1.4.2/MOMORING.egg-info/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      149 2023-04-28 10:37:14.000000 MOMORING-1.4.2/MOMORING.egg-info/PKG-INFO
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      740 2023-04-28 10:37:14.000000 MOMORING-1.4.2/MOMORING.egg-info/SOURCES.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        1 2023-04-28 10:37:14.000000 MOMORING-1.4.2/MOMORING.egg-info/dependency_links.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)       55 2023-04-28 10:37:14.000000 MOMORING-1.4.2/MOMORING.egg-info/entry_points.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        6 2023-04-28 10:37:14.000000 MOMORING-1.4.2/MOMORING.egg-info/requires.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        9 2023-04-28 10:37:14.000000 MOMORING-1.4.2/MOMORING.egg-info/top_level.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      149 2023-04-28 10:37:14.796000 MOMORING-1.4.2/PKG-INFO
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      218 2023-04-28 10:25:13.000000 MOMORING-1.4.2/README.md
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)       38 2023-04-28 10:37:14.797000 MOMORING-1.4.2/setup.cfg
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      408 2023-04-28 10:36:57.000000 MOMORING-1.4.2/setup.py
```

### Comparing `MOMORING-1.4.1/MOMORING/api/create_project.py` & `MOMORING-1.4.2/MOMORING/api/create_project.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.4.1/MOMORING/modules/create.py` & `MOMORING-1.4.2/MOMORING/modules/create.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.4.1/MOMORING/modules/files/git_ignore_template.py` & `MOMORING-1.4.2/MOMORING/modules/files/git_ignore_template.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.4.1/MOMORING/modules/files/main_template.py` & `MOMORING-1.4.2/MOMORING/modules/files/main_template.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.4.1/MOMORING/modules/files/nitrogen_utils.py` & `MOMORING-1.4.2/MOMORING/modules/files/nitrogen_utils.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.4.1/MOMORING.egg-info/SOURCES.txt` & `MOMORING-1.4.2/MOMORING.egg-info/SOURCES.txt`

 * *Files identical despite different names*

