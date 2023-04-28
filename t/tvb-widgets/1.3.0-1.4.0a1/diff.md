# Comparing `tmp/tvb-widgets-1.3.0.tar.gz` & `tmp/tvb-widgets-1.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-widgets-1.3.0.tar", last modified: Thu Apr  6 20:28:51 2023, max compression
+gzip compressed data, was "tvb-widgets-1.4.0a1.tar", last modified: Fri Apr 28 15:56:49 2023, max compression
```

## Comparing `tvb-widgets-1.3.0.tar` & `tvb-widgets-1.4.0a1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.422724 tvb-widgets-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35796 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 20:28:51.422724 tvb-widgets-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/tvb_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-06 20:28:51.000000 tvb-widgets-1.3.0/tvb_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-06 20:28:51.000000 tvb-widgets-1.3.0/tvb_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 20:28:51.000000 tvb-widgets-1.3.0/tvb_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-06 20:28:51.000000 tvb-widgets-1.3.0/tvb_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 20:28:51.000000 tvb-widgets-1.3.0/tvb_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/tvbwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/tvbwidgets/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/ini_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/tvbwidgets/core/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/logger/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/logger/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/tvbwidgets/core/pse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/pse/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/pse/pse_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/tvbwidgets/core/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/simulator/model_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/core/simulator/tvb_integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/tvbwidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/test_drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/test_head_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/test_phase_plane_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/test_ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/test_tvb_integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/tests/ts_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:51.418723 tvb-widgets-1.3.0/tvbwidgets/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/head_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    36149 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/phase_plane_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/pse_launcher_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/pse_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/storage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/ts_widget_help.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-06 20:28:45.000000 tvb-widgets-1.3.0/tvbwidgets/ui/widget_with_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.670086 tvb-widgets-1.4.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35796 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-28 15:56:49.670086 tvb-widgets-1.4.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 15:56:49.670086 tvb-widgets-1.4.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.666086 tvb-widgets-1.4.0a1/tvb_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-28 15:56:49.000000 tvb-widgets-1.4.0a1/tvb_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-28 15:56:49.000000 tvb-widgets-1.4.0a1/tvb_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:56:49.000000 tvb-widgets-1.4.0a1/tvb_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-28 15:56:49.000000 tvb-widgets-1.4.0a1/tvb_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 15:56:49.000000 tvb-widgets-1.4.0a1/tvb_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.666086 tvb-widgets-1.4.0a1/tvbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.666086 tvb-widgets-1.4.0a1/tvbwidgets/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/ini_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.666086 tvb-widgets-1.4.0a1/tvbwidgets/core/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/logger/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/logger/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.666086 tvb-widgets-1.4.0a1/tvbwidgets/core/pse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/pse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/pse/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/pse/pse_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.666086 tvb-widgets-1.4.0a1/tvbwidgets/core/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/simulator/model_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/core/simulator/tvb_integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.666086 tvb-widgets-1.4.0a1/tvbwidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/test_drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/test_head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/test_phase_plane_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/test_ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/test_tvb_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/tests/ts_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:49.670086 tvb-widgets-1.4.0a1/tvbwidgets/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36149 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/phase_plane_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/pse_launcher_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/pse_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/storage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/ts_widget_help.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-28 15:56:42.000000 tvb-widgets-1.4.0a1/tvbwidgets/ui/widget_with_browser.py
```

### Comparing `tvb-widgets-1.3.0/LICENSE` & `tvb-widgets-1.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/PKG-INFO` & `tvb-widgets-1.4.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.3.0
+Version: 1.4.0a1
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-1.3.0/README.md` & `tvb-widgets-1.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/setup.py` & `tvb-widgets-1.4.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvb_widgets.egg-info/PKG-INFO` & `tvb-widgets-1.4.0a1/tvb_widgets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.3.0
+Version: 1.4.0a1
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-1.3.0/tvb_widgets.egg-info/SOURCES.txt` & `tvb-widgets-1.4.0a1/tvb_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/__init__.py` & `tvb-widgets-1.4.0a1/tvbwidgets/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from .core.logger.builder import get_logger
 
 LOGGER = get_logger(__name__)
 
 
 def _fetch_version():
     here = Path(__file__).parent.parent.resolve()
-    print(here)
 
     for settings in here.rglob("package.json"):
         try:
             with settings.open() as f:
                 version = json.load(f)["version"]
                 return (
                     version.replace("-alpha.", "a")
```

### Comparing `tvb-widgets-1.3.0/tvbwidgets/api.py` & `tvb-widgets-1.4.0a1/tvbwidgets/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 #
 
 from .ui.phase_plane_widget import PhasePlaneWidget
 from .ui.storage_widget import StorageWidget
 from .ui.head_widget import HeadBrowser, HeadWidget, HeadWidgetConfig
 from .ui.ts_widget import TimeSeriesWidget, TimeSeriesBrowser
 from .ui.pse_widget import PSEWidget
-from .ui.pse_launcher_widget import PSELauncher
-
+from .ui.pse_launcher_widget import PSELauncher, HPCConfig
 from IPython.core.display_functions import display
 from tvb.datatypes.time_series import TimeSeries
 
 
 def plot_timeseries(data, sample_freq=None, ch_idx=None, backend='matplotlib'):
     """
     Plots a timeseries widget
```

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/auth.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/auth.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/exceptions.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/ini_parser.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/ini_parser.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/logger/builder.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/logger/builder.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/logger/logging.conf` & `tvb-widgets-1.4.0a1/tvbwidgets/core/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/pse/parameters.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/pse/parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,47 +4,56 @@
 #
 # (c) 2022-2023, TVB Widgets Team
 #
 """
 A collection of parameter related classes and functions.
 - Temporary copy from tvb-inversion package
 
-.. moduleauthor:: Fousek Jan <jan.fousek@univ-amu.fr>
+.. moduleauthor: Fousek Jan <jan.fousek@univ-amu.fr>
+.. moduleauthor: Teodora Misan <teodora.misan@codemart.ro>
 """
 
+import os
+import json
+import sys
+import threading
+import numpy as np
 from copy import deepcopy
-from typing import List, Any, Optional
+from typing import List, Any, Optional, Callable
 from dataclasses import dataclass
-import numpy as np
 from tvb.analyzers.metric_variance_global import compute_variance_global_metric
 from tvb.analyzers.metric_kuramoto_index import compute_kuramoto_index_metric
 from tvb.analyzers.metric_proxy_metastability import compute_proxy_metastability_metric
 from tvb.analyzers.metric_variance_of_node_variance import compute_variance_of_node_variance_metric
+from tvb.datatypes.connectivity import Connectivity
 from tvb.datatypes.time_series import TimeSeries
 from tvb.simulator.simulator import Simulator
-import os
 from joblib import Parallel, delayed
-import logging
 from tvbwidgets.core.pse.pse_data import PSEData, PSEStorage
-log = logging.getLogger(__name__)
+from tvbwidgets.core.logger.builder import get_logger
+
+# Here put explicit module name string, for __name__ == __main__
+LOGGER = get_logger("tvbwidgets.core.pse.parameters")
+
+PROGRESS_BAR_STATUS_FILE = "progress_bar_status.txt"
 
 try:
     from dask.distributed import Client
 except ImportError:
-    log.info("ImportError: Dask dependency is not included, so this functionality won't be available")
+    LOGGER.info("ImportError: Dask dependency is not included, so this functionality won't be available")
     Client = object
 
 
 class ParamGetter:
     pass
 
 
 @dataclass
 class SimSeq:
-    "A sequence of simulator configurations."
+    """A sequence of simulator configurations."""
     template: Simulator
     params: List[str]
     values: List[List[Any]]
     getters: Optional[List[Optional[ParamGetter]]] = None  # is the first Optional needed?
 
     # TODO consider transpose, so a param can have a remote data source
     # to load when constructing the sequence
@@ -138,16 +147,16 @@
     def __call__(self, t, y):
         ts = TimeSeries(sample_period=self.sample_period)
         ts.data = y
         return compute_variance_of_node_variance_metric({"time_series": ts, "start_point": self.start_point,
                                                          "segment": self.segment})
 
 
-METRICS = ['GlobalVariance', 'KuramotoIndex', 'ProxyMetastabilitySynchrony Metastability',
-           'ProxyMetastabilitySynchrony Synchrony', 'VarianceNodeVariance']
+METRICS = ['GlobalVariance', 'KuramotoIndex', 'ProxyMetastabilitySynchrony-Metastability',
+           'ProxyMetastabilitySynchrony-Synchrony', 'VarianceNodeVariance']
 
 
 class Reduction:
     pass
 
 
 @dataclass
@@ -183,21 +192,19 @@
         if self.param2 == "connectivity":
             id_values = [val.title[0:25] + "..." for val in self.y_values]
             pse_result.y_value = id_values
         else:
             pse_result.y_value = self.y_values
 
         pse_result.metrics_names = self.metrics
-        pse_result.results = metrics_data_np.reshape(len(self.metrics), len(self.x_values), len(self.y_values))
-        if ".h5" not in self.file_name:
-            self.file_name += ".h5"
+        pse_result.results = metrics_data_np.reshape((len(self.metrics), len(self.x_values), len(self.y_values)))
 
         f = PSEStorage(self.file_name)
         f.store(pse_result)
-        log.info(str(self.file_name) + " file created")
+        LOGGER.info(f"{self.file_name} file created")
         f.close()
 
 
 @dataclass
 class PostProcess:
     metrics: List[Metric]
     reduction: Reduction
@@ -209,14 +216,16 @@
 
 @dataclass
 class JobLibExec:
     seq: SimSeq
     post: PostProcess
     backend: Optional[Any]
     checkpoint_dir: Optional[str]
+    update_progress: Optional[Callable]
+    progress_file_lock: Optional[Any] = threading.Lock()
 
     def _checkpoint(self, result, i):
         if self.checkpoint_dir is not None:
             np.save(os.path.join(self.checkpoint_dir, f'{i}.npy'), result)
 
     def _load_checkpoint(self, i):
         if self.checkpoint_dir is None:
@@ -226,42 +235,68 @@
             return None
         result = np.load(checkpoint_file, allow_pickle=True)
         return result
 
     def _init_checkpoint(self):
         if self.checkpoint_dir is not None:
             if os.path.exists(self.checkpoint_dir):
-                log.info(f"Reusing existing checkpoint dir {self.checkpoint_dir}")
+                LOGGER.info(f"Reusing existing checkpoint dir {self.checkpoint_dir}")
                 # TODO consistency check
             else:
                 os.mkdir(self.checkpoint_dir)
                 np.savetxt(os.path.join(self.checkpoint_dir, 'params.txt'), self.seq.params, fmt='%s')
                 np.save(os.path.join(self.checkpoint_dir, 'param_vals.npy'), self.seq.values)
 
+    def monitor_execution(self):
+        try:
+            if self.update_progress is not None:
+                self.update_progress()
+            else:
+                with self.progress_file_lock:
+                    with open(PROGRESS_BAR_STATUS_FILE, "r+") as f:
+                        # set the cursor to the beginning of the file
+                        f.seek(0)
+                        status = int(f.read())
+                        status += 1
+                        f.seek(0)
+                        f.write(str(status))
+        except Exception as e:
+            LOGGER.error("Could not update the progress bar status", exc_info=e)
+
+
     def __call__(self, n_jobs=-1):
-        log.info("Simulation starts")
+        LOGGER.info("Simulation starts")
         self._init_checkpoint()
-        pool = Parallel(n_jobs)
+        pool = Parallel(n_jobs, prefer="threads")
 
         @delayed
         def job(sim, i):
             result = self._load_checkpoint(i)
             if result is None:
                 if self.backend is not None:
                     runner = self.backend()
                     (t, y), = runner.run_sim(sim.configure())
                 else:
                     (t, y), = sim.configure().run()
-                result = np.hstack([m(t, y) for m in self.post.metrics])
+                result = []
+                for m in self.post.metrics:
+                    try:
+                        result.append(m(t, y))
+                    except Exception:
+                        result.append(np.nan)
+                result = np.hstack(result)
                 self._checkpoint(result, i)
+            LOGGER.info(f"Task {i} finished")
+            self.monitor_execution()
             return result
 
-        metrics = pool(job(_, i) for i, _ in enumerate(self.seq))
-        self.post.reduction(metrics)
-        log.info("Local launch finished")
+        metrics_ = pool(job(_, i) for i, _ in enumerate(self.seq))
+        LOGGER.info(f"Completed tasks: {pool.n_completed_tasks}")
+        self.post.reduction(metrics_)
+        LOGGER.info("Local launch finished")
 
 
 @dataclass
 class DaskExec(JobLibExec):
 
     def __call__(self, client: Client):
         self._init_checkpoint()
@@ -294,43 +329,44 @@
                 result = np.hstack([m(t, y) for m in self.post.metrics])
                 _checkpoint(result, i)
             return result
 
         def reduction(vals):
             return self.post.reduction(vals)
 
-        metrics = client.map(job, *list(zip(*enumerate(self.seq))))
+        metrics_var = client.map(job, *list(zip(*enumerate(self.seq))))
 
         if self.post.reduction is not None:
-            reduced = client.submit(reduction, metrics)
+            reduced = client.submit(reduction, metrics_var)
             return reduced.result()
         else:
-            return metrics
+            return metrics_var
 
 
-def compute_metrics(sim, metrics):
+def compute_metrics(sim, metrics_):
     computed_metrics = []
 
-    for metric in metrics:
+    for metric in metrics_:
         if metric == "GlobalVariance":
-            resulted_metric = (GlobalVariance(sim.monitors[0].period))
+            resulted_metric = GlobalVariance(sim.monitors[0].period)
         elif metric == "KuramotoIndex":
-            resulted_metric = (KuramotoIndex(sim.monitors[0].period))
-        elif metric == "ProxyMetastabilitySynchrony Metastability":
-            resulted_metric = (ProxyMetastabilitySynchrony("Metastability", sim.monitors[0].period))
-        elif metric == "ProxyMetastabilitySynchrony Synchrony":
-            resulted_metric = (ProxyMetastabilitySynchrony("Synchrony", sim.monitors[0].period))
+            resulted_metric = KuramotoIndex(sim.monitors[0].period)
+        elif metric == "ProxyMetastabilitySynchrony-Metastability":
+            resulted_metric = ProxyMetastabilitySynchrony("Metastability", sim.monitors[0].period)
+        elif metric == "ProxyMetastabilitySynchrony-Synchrony":
+            resulted_metric = ProxyMetastabilitySynchrony("Synchrony", sim.monitors[0].period)
         else:
-            resulted_metric = (VarianceNodeVariance(sim.monitors[0].period))
+            resulted_metric = VarianceNodeVariance(sim.monitors[0].period)
         computed_metrics.append(resulted_metric)
 
     return computed_metrics
 
 
-def launch_local_param(simulator, param1, param2, x_values, y_values, metrics, file_name):
+def launch_local_param(simulator, param1, param2, x_values, y_values, metrics, file_name,
+                       update_progress=None, n_threads=4):
     input_values = []
     for elem1 in x_values:
         for elem2 in y_values:
             if param1 == "conduction_speed" or param1 == "connectivity":
                 el1_value = elem1
             else:
                 el1_value = np.array([elem1])
@@ -346,9 +382,33 @@
         params=[param1, param2],
         values=input_values
     )
     pp = PostProcess(
         metrics=compute_metrics(sim, metrics),
         reduction=SaveDataToDisk(param1, param2, x_values, y_values, metrics, file_name),
     )
-    exe = JobLibExec(seq=seq, post=pp, backend=None, checkpoint_dir=None)
-    exe(n_jobs=4)
+    exe = JobLibExec(seq=seq, post=pp, backend=None, checkpoint_dir=None, update_progress=update_progress)
+    exe(n_jobs=n_threads)
+
+
+if __name__ == '__main__':
+    param1 = sys.argv[1]
+    param2 = sys.argv[2]
+    param1_values = json.loads(sys.argv[3])
+    param2_values = json.loads(sys.argv[4])
+    n = len(sys.argv[5])
+    metrics = sys.argv[5][1:n - 1].split(', ')
+    file_name = sys.argv[6]
+    n_threads = int(sys.argv[7])
+
+    LOGGER.info(f"We are now starting PSE for '{param1}' x '{param2}' on {n_threads} threads\n"
+                f"Expect the result in '{file_name}' \n"
+                f"{n} Metrics {metrics}")
+
+    # TODO WID-208 deserialize this instance after being passed from the remote launcher
+    sim = Simulator(connectivity=Connectivity.from_file()).configure()
+
+    with open(PROGRESS_BAR_STATUS_FILE, "w+") as f:
+        f.write("0")
+
+    launch_local_param(sim, param1, param2, param1_values, param2_values, metrics, file_name,
+                       n_threads=n_threads)
```

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/pse/pse_data.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/pse/pse_data.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/simulator/model_exporters.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/simulator/model_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/core/simulator/tvb_integrators.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/simulator/tvb_integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/tests/test_base.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/tests/test_drive_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/tests/test_exporters.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/tests/test_head_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/tests/test_phase_plane_export.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_phase_plane_export.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/tests/test_ts_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/tests/ts_generator.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/ts_generator.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/base_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/base_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/drive_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/head_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/phase_plane_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/phase_plane_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/pse_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/pse_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,42 +54,42 @@
     def _map_names_to_metrics(self):
         for index in range(self.metrics_names.__len__()):
             self.dict_metrics[self.metrics_names[index]] = self.data[index]
 
     def _create_visualizer(self):
         self.param1_value = [str(elem) for elem in self.param1_value]
         self.param2_value = [str(elem) for elem in self.param2_value]
-        pse_layout = go.Layout(width=1000, height=500,
+        pse_layout = go.Layout(width=900, height=600,
                                xaxis=go.layout.XAxis(linecolor='black', linewidth=1, mirror=True,
                                                      title=self.param2_title),
                                yaxis=go.layout.YAxis(linecolor='black', linewidth=1, mirror=True,
                                                      title=self.param1_title),
-                               margin=go.layout.Margin(l=100, r=50, b=100, t=100, pad=4), title="PSE Visualizer",
+                               margin=go.layout.Margin(l=80, r=50, b=50, t=80, pad=4), title="PSE Visualizer",
                                titlefont=dict(size=20, family='Arial, sans-serif'), )
         self.figure = go.FigureWidget(layout=pse_layout)
 
-        self.figure.add_trace(go.Heatmap(z=list(self.dict_metrics.values())[0], x=self.param2_value, y=self.param1_value
-                                         , colorscale='RdBu', connectgaps=False, showscale=True, zsmooth='best'))
+        self.figure.add_trace(go.Heatmap(z=list(self.dict_metrics.values())[0], x=self.param2_value,
+                                         y=self.param1_value, colorscale='RdBu', connectgaps=False,
+                                         showscale=True, zsmooth=False))
 
         self._populate_features()
 
     def _populate_features(self):
         self._smooth_effect()
         self._colors_options()
         self._metrics_options()
-        features_vbox = widgets.VBox(children=[self.smooth_effect_cb, self.change_color_dd,
-                                               self.metrics_change_dd])
-        features_accordion = widgets.Accordion(children=[features_vbox], selected_index=None,
-                                               layout=widgets.Layout(width='25%', marginTop='100px'))
+        features_vbox = widgets.VBox(children=[self.smooth_effect_cb, self.change_color_dd, self.metrics_change_dd])
+        features_accordion = widgets.Accordion(children=[features_vbox], selected_index=0,
+                                               layout=widgets.Layout(width='27%', top='80px'))
         features_accordion.set_title(0, 'Features')
-        table = widgets.HBox([features_accordion, self.figure], layout=self.DEFAULT_BORDER)
+        table = widgets.HBox([self.figure, features_accordion], layout=self.DEFAULT_BORDER)
         display(table)
 
     def _smooth_effect(self):
-        self.smooth_effect_cb = widgets.Checkbox(value=True, description='Smooth visualizer',
+        self.smooth_effect_cb = widgets.Checkbox(value=False, description='Smooth visualizer',
                                                  layout=widgets.Layout(margin='10px 0px 10px 0px'))
 
         def smooth_effect_changed(change):
             if change['type'] != 'change' or change['name'] != 'value':
                 return
 
             if change['new']:
```

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/storage_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/storage_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/ts_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/ts_widget_help.ini` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/ts_widget_help.ini`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.3.0/tvbwidgets/ui/widget_with_browser.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/widget_with_browser.py`

 * *Files identical despite different names*

