# Comparing `tmp/tvb-widgets-1.4.0.tar.gz` & `tmp/tvb-widgets-1.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-widgets-1.4.0.tar", last modified: Fri Apr 28 19:21:56 2023, max compression
+gzip compressed data, was "tvb-widgets-1.4.0a1.tar", last modified: Fri Apr 28 15:56:49 2023, max compression
```

## Comparing `tvb-widgets-1.4.0.tar` & `tvb-widgets-1.4.0a1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.714704 tvb-widgets-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35796 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-28 19:21:56.714704 tvb-widgets-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:21:56.714704 tvb-widgets-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.706704 tvb-widgets-1.4.0/tvb_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-28 19:21:56.000000 tvb-widgets-1.4.0/tvb_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-28 19:21:56.000000 tvb-widgets-1.4.0/tvb_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:21:56.000000 tvb-widgets-1.4.0/tvb_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-28 19:21:56.000000 tvb-widgets-1.4.0/tvb_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 19:21:56.000000 tvb-widgets-1.4.0/tvb_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.706704 tvb-widgets-1.4.0/tvbwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.710704 tvb-widgets-1.4.0/tvbwidgets/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/ini_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.710704 tvb-widgets-1.4.0/tvbwidgets/core/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/logger/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/logger/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.710704 tvb-widgets-1.4.0/tvbwidgets/core/pse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/pse/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/pse/pse_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.710704 tvb-widgets-1.4.0/tvbwidgets/core/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/simulator/model_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/core/simulator/tvb_integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.710704 tvb-widgets-1.4.0/tvbwidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/test_drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/test_head_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/test_phase_plane_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/test_ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/test_tvb_integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/tests/ts_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:56.714704 tvb-widgets-1.4.0/tvbwidgets/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/head_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    36149 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/phase_plane_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/pse_launcher_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/pse_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/storage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/ts_widget_help.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-28 19:21:49.000000 tvb-widgets-1.4.0/tvbwidgets/ui/widget_with_browser.py
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

### Comparing `tvb-widgets-1.4.0/LICENSE` & `tvb-widgets-1.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/PKG-INFO` & `tvb-widgets-1.4.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.4.0
+Version: 1.4.0a1
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-1.4.0/README.md` & `tvb-widgets-1.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/setup.py` & `tvb-widgets-1.4.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvb_widgets.egg-info/PKG-INFO` & `tvb-widgets-1.4.0a1/tvb_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.4.0
+Version: 1.4.0a1
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-1.4.0/tvb_widgets.egg-info/SOURCES.txt` & `tvb-widgets-1.4.0a1/tvb_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/__init__.py` & `tvb-widgets-1.4.0a1/tvbwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/api.py` & `tvb-widgets-1.4.0a1/tvbwidgets/api.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/auth.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/auth.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/exceptions.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/ini_parser.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/ini_parser.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/logger/builder.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/logger/builder.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/logger/logging.conf` & `tvb-widgets-1.4.0a1/tvbwidgets/core/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/pse/parameters.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/pse/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from joblib import Parallel, delayed
 from tvbwidgets.core.pse.pse_data import PSEData, PSEStorage
 from tvbwidgets.core.logger.builder import get_logger
 
 # Here put explicit module name string, for __name__ == __main__
 LOGGER = get_logger("tvbwidgets.core.pse.parameters")
 
-PROGRESS_STATUS = "progress_status.txt"
+PROGRESS_BAR_STATUS_FILE = "progress_bar_status.txt"
 
 try:
     from dask.distributed import Client
 except ImportError:
     LOGGER.info("ImportError: Dask dependency is not included, so this functionality won't be available")
     Client = object
 
@@ -248,24 +248,25 @@
 
     def monitor_execution(self):
         try:
             if self.update_progress is not None:
                 self.update_progress()
             else:
                 with self.progress_file_lock:
-                    with open(PROGRESS_STATUS, "r+") as f:
+                    with open(PROGRESS_BAR_STATUS_FILE, "r+") as f:
                         # set the cursor to the beginning of the file
                         f.seek(0)
                         status = int(f.read())
                         status += 1
                         f.seek(0)
                         f.write(str(status))
         except Exception as e:
             LOGGER.error("Could not update the progress bar status", exc_info=e)
 
+
     def __call__(self, n_jobs=-1):
         LOGGER.info("Simulation starts")
         self._init_checkpoint()
         pool = Parallel(n_jobs, prefer="threads")
 
         @delayed
         def job(sim, i):
@@ -402,12 +403,12 @@
     LOGGER.info(f"We are now starting PSE for '{param1}' x '{param2}' on {n_threads} threads\n"
                 f"Expect the result in '{file_name}' \n"
                 f"{n} Metrics {metrics}")
 
     # TODO WID-208 deserialize this instance after being passed from the remote launcher
     sim = Simulator(connectivity=Connectivity.from_file()).configure()
 
-    with open(PROGRESS_STATUS, "w+") as f:
+    with open(PROGRESS_BAR_STATUS_FILE, "w+") as f:
         f.write("0")
 
     launch_local_param(sim, param1, param2, param1_values, param2_values, metrics, file_name,
                        n_threads=n_threads)
```

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/pse/pse_data.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/pse/pse_data.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/simulator/model_exporters.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/simulator/model_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/core/simulator/tvb_integrators.py` & `tvb-widgets-1.4.0a1/tvbwidgets/core/simulator/tvb_integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/tests/test_base.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/tests/test_drive_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/tests/test_exporters.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/tests/test_head_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/tests/test_phase_plane_export.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_phase_plane_export.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/tests/test_ts_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/test_ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/tests/ts_generator.py` & `tvb-widgets-1.4.0a1/tvbwidgets/tests/ts_generator.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/base_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/base_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/drive_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/head_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/phase_plane_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/phase_plane_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/pse_launcher_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/pse_launcher_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 
     def _prepare_launch(self, where="Local"):
         self._update_info_message(f"{where} launch in progress ...")
         x_values = self.compute_params_values(self.param_1.value)
         y_values = self.compute_params_values(self.param_2.value)
         file_name = self.verify_file_name()
         self.progress.min = 0
-        self.progress.max = len(x_values) * len(y_values) + 1   # no of simulations + 1 for preparation step
-        self.update_progress(0)
+        self.progress.max = len(x_values) * len(y_values) + 1
+        self.update_progress(1)
         return file_name, x_values, y_values
 
     def handle_launch_buttons(self):
         self.launch_local_button = widgets.Button(
             description='Local launch',
             disabled=False,
             button_style='success',
@@ -138,23 +138,24 @@
             self.logger.info("A file name was not specified. It will be created under the name 'test.h5'.")
             return "test.h5"
         elif ".h5" not in file_name:
             return f"{file_name}.h5"
         else:
             return file_name
 
-    def update_progress(self, jobs_completed=None, error_msg=None):
-        if error_msg is not None:
+    def update_progress(self, value=None, error_msg=None):
+        if error_msg is None:
             self._update_info_message(error_msg, is_error=True)
 
         with self.progress_lock:
-            if jobs_completed is None:
+            if value is None:
                 self.progress.value += 1
-            elif jobs_completed >= 0:
-                self.progress.value = jobs_completed + 1
+            elif value >= 0:
+                self.progress.value = value
+
 
     def create_metrics(self):
         self.metrics_sm = widgets.SelectMultiple(
             options=self.metrics,
             description="<b>Metrics</b>",
             value=[self.metrics[0]],
             disabled=False, layout=widgets.Layout(margin="0px 20px 10px 25px", height="115px", width="340px"))
```

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/pse_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/pse_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/storage_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/storage_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/ts_widget.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/ts_widget_help.ini` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/ts_widget_help.ini`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.0/tvbwidgets/ui/widget_with_browser.py` & `tvb-widgets-1.4.0a1/tvbwidgets/ui/widget_with_browser.py`

 * *Files identical despite different names*

