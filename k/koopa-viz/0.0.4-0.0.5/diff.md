# Comparing `tmp/koopa-viz-0.0.4.tar.gz` & `tmp/koopa-viz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koopa-viz-0.0.4.tar", last modified: Wed Mar  1 08:08:57 2023, max compression
+gzip compressed data, was "koopa-viz-0.0.5.tar", last modified: Fri Apr 28 09:03:09 2023, max compression
```

## Comparing `koopa-viz-0.0.4.tar` & `koopa-viz-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 beichenberger   (504) staff       (20)        0 2023-03-01 08:08:57.504447 koopa-viz-0.0.4/
--rw-r--r--   0 beichenberger   (504) staff       (20)       96 2022-11-04 16:45:33.000000 koopa-viz-0.0.4/MANIFEST.in
--rw-r--r--   0 beichenberger   (504) staff       (20)     2236 2023-03-01 08:08:57.504505 koopa-viz-0.0.4/PKG-INFO
--rw-r--r--   0 beichenberger   (504) staff       (20)     1058 2022-11-04 16:45:33.000000 koopa-viz-0.0.4/README.md
--rw-r--r--   0 beichenberger   (504) staff       (20)      180 2022-11-04 16:45:33.000000 koopa-viz-0.0.4/pyproject.toml
--rw-r--r--   0 beichenberger   (504) staff       (20)     1651 2023-03-01 08:08:57.511290 koopa-viz-0.0.4/setup.cfg
-drwxr-xr-x   0 beichenberger   (504) staff       (20)        0 2023-03-01 08:08:57.492965 koopa-viz-0.0.4/src/
-drwxr-xr-x   0 beichenberger   (504) staff       (20)        0 2023-03-01 08:08:57.498956 koopa-viz-0.0.4/src/koopa_viz/
--rw-r--r--   0 beichenberger   (504) staff       (20)       84 2023-03-01 08:08:44.000000 koopa-viz-0.0.4/src/koopa_viz/__init__.py
--rw-r--r--   0 beichenberger   (504) staff       (20)    16272 2023-03-01 08:07:11.000000 koopa-viz-0.0.4/src/koopa_viz/_widget.py
--rw-r--r--   0 beichenberger   (504) staff       (20)      270 2022-11-04 16:45:33.000000 koopa-viz-0.0.4/src/koopa_viz/napari.yaml
-drwxr-xr-x   0 beichenberger   (504) staff       (20)        0 2023-03-01 08:08:57.503846 koopa-viz-0.0.4/src/koopa_viz.egg-info/
--rw-r--r--   0 beichenberger   (504) staff       (20)     2236 2023-03-01 08:08:57.000000 koopa-viz-0.0.4/src/koopa_viz.egg-info/PKG-INFO
--rw-r--r--   0 beichenberger   (504) staff       (20)      347 2023-03-01 08:08:57.000000 koopa-viz-0.0.4/src/koopa_viz.egg-info/SOURCES.txt
--rw-r--r--   0 beichenberger   (504) staff       (20)        1 2023-03-01 08:08:57.000000 koopa-viz-0.0.4/src/koopa_viz.egg-info/dependency_links.txt
--rw-r--r--   0 beichenberger   (504) staff       (20)       52 2023-03-01 08:08:57.000000 koopa-viz-0.0.4/src/koopa_viz.egg-info/entry_points.txt
--rw-r--r--   0 beichenberger   (504) staff       (20)      112 2023-03-01 08:08:57.000000 koopa-viz-0.0.4/src/koopa_viz.egg-info/requires.txt
--rw-r--r--   0 beichenberger   (504) staff       (20)       10 2023-03-01 08:08:57.000000 koopa-viz-0.0.4/src/koopa_viz.egg-info/top_level.txt
+drwxr-xr-x   0 beichenberger   (504) staff       (20)        0 2023-04-28 09:03:09.483174 koopa-viz-0.0.5/
+-rw-r--r--   0 beichenberger   (504) staff       (20)       96 2022-11-04 16:45:33.000000 koopa-viz-0.0.5/MANIFEST.in
+-rw-r--r--   0 beichenberger   (504) staff       (20)     2236 2023-04-28 09:03:09.483265 koopa-viz-0.0.5/PKG-INFO
+-rw-r--r--   0 beichenberger   (504) staff       (20)     1058 2022-11-04 16:45:33.000000 koopa-viz-0.0.5/README.md
+-rw-r--r--   0 beichenberger   (504) staff       (20)      180 2022-11-04 16:45:33.000000 koopa-viz-0.0.5/pyproject.toml
+-rw-r--r--   0 beichenberger   (504) staff       (20)     1628 2023-04-28 09:03:09.483737 koopa-viz-0.0.5/setup.cfg
+drwxr-xr-x   0 beichenberger   (504) staff       (20)        0 2023-04-28 09:03:09.463439 koopa-viz-0.0.5/src/
+drwxr-xr-x   0 beichenberger   (504) staff       (20)        0 2023-04-28 09:03:09.475843 koopa-viz-0.0.5/src/koopa_viz/
+-rw-r--r--   0 beichenberger   (504) staff       (20)       84 2023-04-28 08:57:22.000000 koopa-viz-0.0.5/src/koopa_viz/__init__.py
+-rw-r--r--   0 beichenberger   (504) staff       (20)    15926 2023-04-28 09:00:25.000000 koopa-viz-0.0.5/src/koopa_viz/_widget.py
+-rw-r--r--   0 beichenberger   (504) staff       (20)      270 2022-11-04 16:45:33.000000 koopa-viz-0.0.5/src/koopa_viz/napari.yaml
+drwxr-xr-x   0 beichenberger   (504) staff       (20)        0 2023-04-28 09:03:09.482771 koopa-viz-0.0.5/src/koopa_viz.egg-info/
+-rw-r--r--   0 beichenberger   (504) staff       (20)     2236 2023-04-28 09:03:09.000000 koopa-viz-0.0.5/src/koopa_viz.egg-info/PKG-INFO
+-rw-r--r--   0 beichenberger   (504) staff       (20)      347 2023-04-28 09:03:09.000000 koopa-viz-0.0.5/src/koopa_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 beichenberger   (504) staff       (20)        1 2023-04-28 09:03:09.000000 koopa-viz-0.0.5/src/koopa_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 beichenberger   (504) staff       (20)       52 2023-04-28 09:03:09.000000 koopa-viz-0.0.5/src/koopa_viz.egg-info/entry_points.txt
+-rw-r--r--   0 beichenberger   (504) staff       (20)       91 2023-04-28 09:03:09.000000 koopa-viz-0.0.5/src/koopa_viz.egg-info/requires.txt
+-rw-r--r--   0 beichenberger   (504) staff       (20)       10 2023-04-28 09:03:09.000000 koopa-viz-0.0.5/src/koopa_viz.egg-info/top_level.txt
```

### Comparing `koopa-viz-0.0.4/PKG-INFO` & `koopa-viz-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koopa-viz
-Version: 0.0.4
+Version: 0.0.5
 Summary: Vizualization plugin for koopa image analysis
 Home-page: https://github.com/bbquercus/koopa
 Author: Bastian Eichenberger
 Author-email: bastian@eichenbergers.ch
 License: MIT
 Project-URL: Bug Tracker, https://github.com/bbquercus/koopa/issues
 Project-URL: Documentation, https://github.com/bbquercus/koopa#README.md
```

### Comparing `koopa-viz-0.0.4/README.md` & `koopa-viz-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `koopa-viz-0.0.4/setup.cfg` & `koopa-viz-0.0.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = koopa-viz
-version = 0.0.4
+version = 0.0.5
 description = Vizualization plugin for koopa image analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bbquercus/koopa
 author = Bastian Eichenberger
 author_email = bastian@eichenbergers.ch
 license = MIT
@@ -31,17 +31,15 @@
 [options]
 packages = find:
 install_requires = 
 	numpy
 	pandas
 	pyarrow
 	qtpy
-	scikit-image
 	tifffile
-	trackpy
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `koopa-viz-0.0.4/src/koopa_viz/_widget.py` & `koopa-viz-0.0.5/src/koopa_viz/_widget.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     QPushButton,
     QVBoxLayout,
     QWidget,
 )
 import napari
 import numpy as np
 import pandas as pd
-import skimage.io
 import tifffile
-import trackpy as tp
 
 
 class KoopaWidget(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
 
         # General config
@@ -38,14 +36,15 @@
             "gamma",
             "opacity",
             "out_of_slice_display",
             "size",
             "symbol",
             "visible",
         ]
+        self.luigi = False
 
         # Viewer model params - https://napari.org/stable/api/napari.Viewer
         self.image_params = dict(blending="additive")
         self.label_params = dict(
             blending="translucent", num_colors=50, opacity=0.7
         )
         self.point_params = dict(
@@ -57,24 +56,31 @@
         self.track_params = dict(tail_width=8, tail_length=30, head_length=2)
 
         # Build plugin layout
         self.setLayout(QVBoxLayout())
         self.setup_logo_header()
         self.setup_config_parser()
         self.setup_file_dropdown()
-        # self.setup_save_widget() # Hide for now.
         self.setup_file_navigation()
         self.setup_viewing_options()
         self.setup_progress_bar()
 
+    def toggle_old_naming(self):
+        self.luigi = not self.luigi
+        napari.utils.notifications.show_info(
+            f"Turned old naming scheme {'on' if self.luigi else 'off'}."
+        )
+
     def clear_viewer(self):
+        """Reset all layers to an empty window."""
         self.viewer.reset_view()
         self.viewer.layers.clear()
 
     def setup_logo_header(self):
+        """Prepare widget for header."""
         widget = QWidget()
         widget.setLayout(QHBoxLayout())
         widget.layout().addWidget(QLabel("<h1>Koopa</h1>"))
         widget.layout().addWidget(
             QLabel("Keenly optimized obliging picture analysis.")
         )
         self.layout().addWidget(widget)
@@ -84,17 +90,22 @@
         widget = QWidget()
         widget.setLayout(QVBoxLayout())
         widget.layout().addWidget(QLabel("<b>Analysis Directory:</b>"))
 
         btn_widget = QPushButton("Select")
         btn_widget.clicked.connect(self.open_file_dialog)
         widget.layout().addWidget(btn_widget)
+
+        luigi_widget = QPushButton("Toggle old naming")
+        luigi_widget.clicked.connect(self.toggle_old_naming)
+        widget.layout().addWidget(luigi_widget)
         self.layout().addWidget(widget)
 
     def setup_file_dropdown(self):
+        """Prepare widget for single file selection."""
         widget = QWidget()
         widget.setLayout(QVBoxLayout())
         widget.layout().addWidget(QLabel("<b>Current File:</b>"))
 
         self.dropdown_widget = QComboBox()
         widget.layout().addWidget(self.dropdown_widget)
 
@@ -102,27 +113,16 @@
         btn_widget.clicked.connect(self.load_file)
         widget.layout().addWidget(btn_widget)
 
         self.file_dropdown = widget
         self.file_dropdown.setDisabled(True)
         self.layout().addWidget(self.file_dropdown)
 
-    # def setup_save_widget(self):
-    #     widget = QWidget()
-    #     widget.setLayout(QVBoxLayout())
-    #     widget.layout().addWidget(QLabel("<b>Save Edits:</b>"))
-    #     btn_widget = QPushButton("Run")
-    #     btn_widget.clicked.connect(self.save_edits)
-    #     widget.layout().addWidget(btn_widget)
-    #
-    #     self.save_widget = widget
-    #     self.save_widget.setDisabled(True)
-    #     self.layout().addWidget(self.save_widget)
-
     def setup_file_navigation(self):
+        """Prepare widget for file navigation."""
         widget = QWidget()
         widget.setLayout(QVBoxLayout())
         widget.layout().addWidget(QLabel("<b>Navigate Files:</b>"))
         prev_widget = QPushButton("Previous Image")
         prev_widget.clicked.connect(lambda: self.change_file("prev"))
         widget.layout().addWidget(prev_widget)
         next_widget = QPushButton("Next Image")
@@ -130,36 +130,39 @@
         widget.layout().addWidget(next_widget)
 
         self.file_navigation = widget
         self.file_navigation.setDisabled(True)
         self.layout().addWidget(self.file_navigation)
 
     def setup_viewing_options(self):
+        """Prepare widget accessibility options."""
         widget = QWidget()
         widget.setLayout(QVBoxLayout())
         widget.layout().addWidget(QLabel("<b>Viewing Options:</b>"))
 
         hideall_widget = QPushButton("Hide All Layers")
         hideall_widget.clicked.connect(self.hide_layers)
         widget.layout().addWidget(hideall_widget)
 
-        # settings_save_widget = QPushButton("Save Settings")
-        # settings_save_widget.clicked.connect(self.save_settings)
-        # widget.layout().addWidget(settings_save_widget)
+        settings_save_widget = QPushButton("Save Settings")
+        settings_save_widget.clicked.connect(self.save_settings)
+        widget.layout().addWidget(settings_save_widget)
         settings_apply_widget = QPushButton("Apply Settings")
         settings_apply_widget.clicked.connect(self.apply_settings)
         widget.layout().addWidget(settings_apply_widget)
         self.layout().addWidget(widget)
 
     def setup_progress_bar(self):
+        """Prepare widget with data loading progress bar."""
         self.pbar = QProgressBar(self)
         self.pbar.setValue(0)
         self.layout().addWidget(self.pbar)
 
     def open_file_dialog(self):
+        """Dialog to select analysis directory."""
         dialog = QFileDialog()
         dialog.setFileMode(QFileDialog.FileMode.DirectoryOnly)
         if dialog.exec_():
             self.clear_viewer()
             self.analysis_path = dialog.selectedFiles()[0]
             self.run_config_parser()
             self.get_file_list()
@@ -203,74 +206,14 @@
         # Points
         self.load_detection_raw()
         self.pbar.setValue(85)
         if eval(self.config["SpotsColocalization"]["coloc_enabled"]):
             self.load_colocalization()
         self.pbar.setValue(100)
 
-        # self.save_widget.setDisabled(False)
-
-    def save_labels_layer(self, layer):
-        if layer.name == "Segmentation Cyto":
-            folder = "segmentation_cyto"
-        elif layer.name == "Segmentation Nuclei":
-            folder = "segmentation_nuclei"
-        else:
-            folder = f"segmentation_c{layer.name.lstrip('Segmentation C')}"
-        fname = os.path.join(self.analysis_path, folder, f"{self.name}.tif")
-        skimage.io.imsave(fname, layer.data, check_contrast=False)
-
-    def save_points_layer(self, layer):
-        channel = int(layer.name.lstrip("Detection C"))
-
-        # Update spots df
-        refinement_radius = eval(
-            self.config["SpotsDetection"]["refinement_radius"]
-        )
-        image = np.pad(
-            self.image[channel],
-            refinement_radius + 1,
-            mode="constant",
-            constant_values=0,
-        )
-        zyx = layer.data if self.do_3d else layer.data[:, 1:]
-        df = tp.refine_com(
-            raw_image=image,
-            image=image,
-            radius=refinement_radius,
-            coords=zyx + refinement_radius,
-        )
-        df["x"] = zyx.T[2] if self.do_3d else zyx.T[1]
-        df["y"] = zyx.T[1] if self.do_3d else zyx.T[0]
-        df = df.drop("raw_mass", axis=1)
-        df["frame"] = layer.data.T[0] if self.do_3d else 0
-        df["channel"] = channel
-        df.insert(loc=0, column="FileID", value=self.name)
-        if self.do_3d:
-            df["particle"] = df.index.values + 1
-
-        # Save
-        folder = (
-            f"detection_final_c{channel}"
-            if self.do_3d
-            else f"detection_raw_c{channel}"
-        )
-        fname = os.path.join(self.analysis_path, folder, f"{self.name}.parq")
-        df.to_parquet(fname)
-
-    def save_edits(self):
-        for layer in self.viewer.layers:
-            if isinstance(layer, napari.layers.labels.labels.Labels):
-                self.save_label_layer(layer)
-            if isinstance(layer, napari.layers.points.points.Points):
-                self.save_points_layer(layer)
-        napari.utils.notifications.show_info(
-            f"Finished saving edits to {self.name}"
-        )
-
     def change_file(self, option: str):
         """Navigation prev/next to change files faster."""
         file_idx = self.files.index(self.dropdown_widget.currentText())
         if file_idx == 0 and option == "prev":
             raise ValueError("Already at the beginning!")
         if file_idx == len(self.files) and option == "next":
             raise ValueError("Already at the end!")
@@ -282,77 +225,110 @@
     def get_file_list(self):
         """Find all files in analysis directory and update dropdown."""
         files = sorted(
             glob.glob(
                 os.path.join(self.analysis_path, "preprocessed", "*.tif")
             )
         )
-        files = sorted(
-            [os.path.basename(f).replace(".tif", "") for f in files]
-        )
         self.files = sorted(
-            [f[:-17] for f in files]
+            [os.path.basename(f).replace(".tif", "") for f in files]
         )
+        if not self.luigi:
+            self.files = sorted([f[17:] for f in self.files])
 
         self.file_dropdown.setDisabled(False)
         self.file_navigation.setDisabled(False)
         self.dropdown_widget.clear()
         self.dropdown_widget.addItems(self.files)
 
     def load_image(self):
         """Open and display raw image data."""
-        fname = glob.glob(os.path.join(
-            self.analysis_path, "preprocessed", f"{self.name}-*.tif"
-        ))[0]
+        if self.luigi:
+            fname = os.path.join(
+                self.analysis_path, "preprocessed", f"{self.name}.tif"
+            )
+        else:
+            fname = glob.glob(
+                os.path.join(
+                    self.analysis_path, "preprocessed", f"{self.name}-*.tif"
+                )
+            )[0]
         self.image = tifffile.imread(fname)
         for idx, channel in enumerate(self.image):
             self.viewer.add_image(
                 channel, name=f"Channel {idx}", **self.image_params
             )
 
     def load_segmentation_cells(self):
         """Open and display nuclear/cytoplasmic segmentation maps."""
         for name in ["nuclei", "cyto"]:
-            fname = glob.glob(os.path.join(
-                self.analysis_path, f"segmentation_{name}", f"{self.name}-*.tif"
-            ))[0]
+            if self.luigi:
+                fname = os.path.join(
+                    self.analysis_path,
+                    f"segmentation_{name}",
+                    f"{self.name}.tif",
+                )
+            else:
+                fname = glob.glob(
+                    os.path.join(
+                        self.analysis_path,
+                        f"segmentation_{name}",
+                        f"{self.name}-*.tif",
+                    )
+                )[0]
             if not os.path.exists(fname):
                 continue
             segmap = tifffile.imread(fname).astype(int)
             self.viewer.add_labels(
                 segmap,
                 name=f"Segmentation {name.capitalize()}",
                 **self.label_params,
             )
 
     def load_segmentation_other(self):
         """Open and display additional segmentation maps."""
         for channel in eval(self.config["SegmentationOther"]["sego_channels"]):
-            fname = glob.glob(os.path.join(
-                self.analysis_path,
-                f"segmentation_{channel}",
-                f"{self.name}-*.tif",
-            ))[0]
+            if self.luigi:
+                fname = os.path.join(
+                    self.analysis_path,
+                    f"segmentation_{channel}",
+                    f"{self.name}.tif",
+                )
+            else:
+                fname = glob.glob(
+                    os.path.join(
+                        self.analysis_path,
+                        f"segmentation_{channel}",
+                        f"{self.name}-*.tif",
+                    )
+                )[0]
             segmap = tifffile.imread(fname).astype(int)
             self.viewer.add_labels(
                 segmap, name=f"Segmentation C{channel}", **self.label_params
             )
 
     def load_detection_raw(self):
         """Open and display raw spot detection points."""
 
         for channel in eval(self.config["SpotsDetection"]["detect_channels"]):
             folder = (
                 f"detection_final_c{channel}"
                 if self.do_3d or self.do_timeseries
                 else f"detection_raw_c{channel}"
             )
-            fname = glob.glob(os.path.join(
-                self.analysis_path, folder, f"{self.name}-*.parq"
-            ))[0]
+            if self.luigi:
+                fname = os.path.join(
+                    self.analysis_path, folder, f"{self.name}.parq"
+                )
+            else:
+                fname = glob.glob(
+                    os.path.join(
+                        self.analysis_path, folder, f"{self.name}-*.parq"
+                    )
+                )[0]
             df = pd.read_parquet(fname)
 
             if self.do_timeseries:
                 self.viewer.add_tracks(
                     df[self.track_cols],
                     name=f"Track C{channel}",
                     **self.track_params,
@@ -364,19 +340,28 @@
                     **self.point_params,
                 )
 
     def load_colocalization(self):
         """Open and display colocalization pairs (colocalized vs. non)."""
 
         for i, j in eval(self.config["SpotsColocalization"]["coloc_channels"]):
-            fname = glob.glob(os.path.join(
-                self.analysis_path,
-                f"colocalization_{i}-{j}",
-                f"{self.name}-*.parq",
-            ))[0]
+            if self.luigi:
+                fname = os.path.join(
+                    self.analysis_path,
+                    f"colocalization_{i}-{j}",
+                    f"{self.name}.parq",
+                )
+            else:
+                fname = glob.glob(
+                    os.path.join(
+                        self.analysis_path,
+                        f"colocalization_{i}-{j}",
+                        f"{self.name}-*.parq",
+                    )
+                )[0]
             df = pd.read_parquet(fname)
             df_coloc = df[df["channel"] == i]
             df_empty = df[df["channel"] == j]
 
             if self.do_timeseries:
                 df_coloc = df_coloc.loc[
                     df_coloc[f"coloc_particle_{i}-{j}"].isna(), self.track_cols
@@ -416,24 +401,27 @@
                     df_empty,
                     name=f"Detection {i}-{j} Empty",
                     face_color="blue",
                     **bland_point_params,
                 )
 
     def hide_layers(self):
+        """Set visibility of all layers to False."""
         for layer in self.viewer.layers:
             layer.visible = False
 
     @staticmethod
     def rgb_to_hex(rgb: np.ndarray):
+        """Convert (R, G, B) format to #RRGGBB."""
         return ("#{:X}{:X}{:X}").format(
             int(rgb[0] * 255), int(rgb[1] * 255), int(rgb[2] * 255)
         )
 
     def save_settings(self):
+        """Save user specific viewing settings (e.g. contrast)."""
         self.settings = {}
         for idx, layer in enumerate(self.viewer.layers):
             layer_settings = {}
             for param in self.params:
                 if hasattr(layer, param):
                     # NOTE currently doesn't get set properly via interface
                     # Bug in napari not in plugin
@@ -444,14 +432,15 @@
                     else:
                         value = getattr(layer, param)
                     layer_settings[param] = value
             self.settings[idx] = layer_settings
         napari.utils.notifications.show_info("Current settings saved.")
 
     def apply_settings(self):
+        """Apply previously saved user specific viewing settings."""
         if not hasattr(self, "settings"):
             napari.utils.notifications.show_error("No settings saved!")
             return None
 
         for idx, layer in enumerate(self.viewer.layers):
             if idx in self.settings:
                 for param, value in self.settings[idx].items():
```

### Comparing `koopa-viz-0.0.4/src/koopa_viz.egg-info/PKG-INFO` & `koopa-viz-0.0.5/src/koopa_viz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koopa-viz
-Version: 0.0.4
+Version: 0.0.5
 Summary: Vizualization plugin for koopa image analysis
 Home-page: https://github.com/bbquercus/koopa
 Author: Bastian Eichenberger
 Author-email: bastian@eichenbergers.ch
 License: MIT
 Project-URL: Bug Tracker, https://github.com/bbquercus/koopa/issues
 Project-URL: Documentation, https://github.com/bbquercus/koopa#README.md
```

