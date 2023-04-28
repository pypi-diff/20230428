# Comparing `tmp/napari-tomotwin-0.1.1.tar.gz` & `tmp/napari-tomotwin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-tomotwin-0.1.1.tar", last modified: Fri Mar 24 12:44:16 2023, max compression
+gzip compressed data, was "napari-tomotwin-0.1.2.tar", last modified: Fri Apr 28 11:48:14 2023, max compression
```

## Comparing `napari-tomotwin-0.1.1.tar` & `napari-tomotwin-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.735601 napari-tomotwin-0.1.1/.github/
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.735601 napari-tomotwin-0.1.1/.github/workflows/
--rw-r--r--   0 twagner  (22293) domain users (32000)     2903 2023-03-24 12:41:54.000000 napari-tomotwin-0.1.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 twagner  (22293) domain users (32000)      992 2023-03-13 07:06:20.000000 napari-tomotwin-0.1.1/.gitignore
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/.napari-hub/
--rw-r--r--   0 twagner  (22293) domain users (32000)      463 2023-03-13 07:06:20.000000 napari-tomotwin-0.1.1/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 twagner  (22293) domain users (32000)      542 2023-03-13 07:06:20.000000 napari-tomotwin-0.1.1/.napari-hub/config.yml
--rw-r--r--   0 twagner  (22293) domain users (32000)     1275 2023-03-21 12:45:38.000000 napari-tomotwin-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 twagner  (22293) domain users (32000)    16726 2023-03-13 07:06:20.000000 napari-tomotwin-0.1.1/LICENSE
--rw-r--r--   0 twagner  (22293) domain users (32000)       96 2023-03-13 07:06:20.000000 napari-tomotwin-0.1.1/MANIFEST.in
--rw-r--r--   0 twagner  (22293) domain users (32000)     2388 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)     1530 2023-03-21 12:32:28.000000 napari-tomotwin-0.1.1/README.md
--rw-r--r--   0 twagner  (22293) domain users (32000)      264 2023-03-21 12:39:15.000000 napari-tomotwin-0.1.1/pyproject.toml
--rw-r--r--   0 twagner  (22293) domain users (32000)       59 2023-03-21 12:52:24.000000 napari-tomotwin-0.1.1/requirements.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)     1286 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/setup.cfg
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/src/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2023-03-13 14:05:08.000000 napari-tomotwin-0.1.1/src/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/src/napari_tomotwin/
--rw-r--r--   0 twagner  (22293) domain users (32000)       41 2023-03-21 12:30:34.000000 napari-tomotwin-0.1.1/src/napari_tomotwin/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/src/napari_tomotwin/_qt/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2023-03-13 07:17:25.000000 napari-tomotwin-0.1.1/src/napari_tomotwin/_qt/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/src/napari_tomotwin/_tests/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2023-03-13 07:06:20.000000 napari-tomotwin-0.1.1/src/napari_tomotwin/_tests/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)       34 2023-03-24 12:41:54.000000 napari-tomotwin-0.1.1/src/napari_tomotwin/_tests/test_dummy.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      160 2023-03-24 12:44:16.000000 napari-tomotwin-0.1.1/src/napari_tomotwin/_version.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     2446 2023-03-22 11:26:33.000000 napari-tomotwin-0.1.1/src/napari_tomotwin/load_umap.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     2061 2023-03-21 12:28:56.000000 napari-tomotwin-0.1.1/src/napari_tomotwin/make_targets.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      537 2023-03-14 12:22:04.000000 napari-tomotwin-0.1.1/src/napari_tomotwin/napari.yaml
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-24 12:44:16.739601 napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/
--rw-r--r--   0 twagner  (22293) domain users (32000)     2388 2023-03-24 12:44:16.000000 napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)      759 2023-03-24 12:44:16.000000 napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/SOURCES.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)        1 2023-03-24 12:44:16.000000 napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/dependency_links.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       64 2023-03-24 12:44:16.000000 napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/entry_points.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       62 2023-03-24 12:44:16.000000 napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/requires.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       16 2023-03-24 12:44:16.000000 napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/top_level.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)      580 2023-03-21 12:54:16.000000 napari-tomotwin-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.370733 napari-tomotwin-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-28 11:48:14.378733 napari-tomotwin-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/napari_tomotwin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/napari_tomotwin/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/napari_tomotwin/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/_tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/load_umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/make_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/tox.ini
```

### Comparing `napari-tomotwin-0.1.1/.github/workflows/test_and_deploy.yml` & `napari-tomotwin-0.1.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/.gitignore` & `napari-tomotwin-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/.napari-hub/config.yml` & `napari-tomotwin-0.1.2/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/.pre-commit-config.yaml` & `napari-tomotwin-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/LICENSE` & `napari-tomotwin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/PKG-INFO` & `napari-tomotwin-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.1.1/README.md` & `napari-tomotwin-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/setup.cfg` & `napari-tomotwin-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/src/napari_tomotwin/load_umap.py` & `napari-tomotwin-0.1.2/src/napari_tomotwin/load_umap.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,38 +26,40 @@
         umap = pd.concat([label_column, umap], axis=1)
 
     if hasattr(label_layer, "properties"):
         label_layer.properties = umap
     if hasattr(label_layer, "features"):
         label_layer.features = umap
     label_layer.opacity = 0
-
+    label_layer.visible = True
     viewer = napari.current_viewer()
     plotter_widget: PlotterWidget = None
     widget, plotter_widget = viewer.window.add_plugin_dock_widget('napari-clusters-plotter', widget_name='Plotter Widget')
     plotter_widget.plot_x_axis.setCurrentIndex(1)
     plotter_widget.plot_y_axis.setCurrentIndex(2)
 
     plotter_widget.bin_auto.setChecked(True)
     plotter_widget.plotting_type.setCurrentIndex(1)
     plotter_widget.plot_hide_non_selected.setChecked(True)
+
     try:
         plotter_widget.run(
                     umap,
                     "umap_0",
                     "umap_1",
                     plot_cluster_name=None,
                     force_redraw=True
                 )
     except:
         pass
 
     @viewer.mouse_drag_callbacks.append
     def get_event(viewer, event):
         global circle
+        label_layer.visible = 1
         data_coordinates = label_layer.world_to_data(event.position)
         val = label_layer._get_value(data_coordinates)
         umap_coordinates = umap.loc[umap['label']==val,[plotter_widget.plot_x_axis.currentText(),plotter_widget.plot_y_axis.currentText()]]
 
         try:
             center = umap_coordinates.values.tolist()[0]
         except IndexError:
```

### Comparing `napari-tomotwin-0.1.1/src/napari_tomotwin/make_targets.py` & `napari-tomotwin-0.1.2/src/napari_tomotwin/make_targets.py`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/src/napari_tomotwin/napari.yaml` & `napari-tomotwin-0.1.2/src/napari_tomotwin/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/PKG-INFO` & `napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.1.1/src/napari_tomotwin.egg-info/SOURCES.txt` & `napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.1/tox.ini` & `napari-tomotwin-0.1.2/tox.ini`

 * *Files identical despite different names*

