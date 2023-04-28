# Comparing `tmp/glview-1.5.1.tar.gz` & `tmp/glview-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glview-1.5.1.tar", last modified: Mon Apr 17 10:00:01 2023, max compression
+gzip compressed data, was "glview-1.5.2.tar", last modified: Fri Apr 28 08:34:11 2023, max compression
```

## Comparing `glview-1.5.1.tar` & `glview-1.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-17 10:00:01.560995 glview-1.5.1/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.1/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.1/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-17 10:00:01.560995 glview-1.5.1/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      361 2023-03-13 15:45:56.000000 glview-1.5.1/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-17 10:00:01.560995 glview-1.5.1/glview/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:51:16.000000 glview-1.5.1/glview/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.1/glview/argv.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11563 2023-04-17 09:59:15.000000 glview-1.5.1/glview/glrenderer.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     8958 2023-04-17 09:53:29.000000 glview-1.5.1/glview/glview.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     6950 2023-03-13 15:45:56.000000 glview-1.5.1/glview/imageprovider.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      285 2023-03-13 15:45:56.000000 glview-1.5.1/glview/panzoom.vs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17381 2023-04-17 09:54:42.000000 glview-1.5.1/glview/pygletui.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4478 2023-04-14 11:24:45.000000 glview-1.5.1/glview/texture.fs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-04-17 09:55:11.000000 glview-1.5.1/glview/version.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-17 10:00:01.560995 glview-1.5.1/glview.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/entry_points.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/top_level.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/zip-safe
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      163 2023-03-14 15:45:52.000000 glview-1.5.1/requirements.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-04-17 10:00:01.560995 glview-1.5.1/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.1/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-28 08:34:11.564053 glview-1.5.2/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.2/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.2/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-28 08:34:11.564053 glview-1.5.2/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      361 2023-03-13 15:45:56.000000 glview-1.5.2/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-28 08:34:11.564053 glview-1.5.2/glview/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:51:16.000000 glview-1.5.2/glview/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.2/glview/argv.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    14269 2023-04-25 14:24:08.000000 glview-1.5.2/glview/glrenderer.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     9287 2023-04-28 08:25:57.000000 glview-1.5.2/glview/glview.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     6950 2023-03-13 15:45:56.000000 glview-1.5.2/glview/imageprovider.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      285 2023-03-13 15:45:56.000000 glview-1.5.2/glview/panzoom.vs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17868 2023-04-28 08:27:30.000000 glview-1.5.2/glview/pygletui.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4478 2023-04-25 13:39:44.000000 glview-1.5.2/glview/texture.fs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-04-28 08:27:54.000000 glview-1.5.2/glview/version.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-28 08:34:11.564053 glview-1.5.2/glview.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-28 08:34:11.000000 glview-1.5.2/glview.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-04-28 08:34:11.000000 glview-1.5.2/glview.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-28 08:34:11.000000 glview-1.5.2/glview.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-04-28 08:34:11.000000 glview-1.5.2/glview.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-04-28 08:34:11.000000 glview-1.5.2/glview.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-04-28 08:34:11.000000 glview-1.5.2/glview.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-28 08:34:11.000000 glview-1.5.2/glview.egg-info/zip-safe
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      163 2023-03-14 15:45:52.000000 glview-1.5.2/requirements.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-04-28 08:34:11.564053 glview-1.5.2/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.2/setup.py
```

### Comparing `glview-1.5.1/LICENSE` & `glview-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glview-1.5.1/PKG-INFO` & `glview-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.5.1
+Version: 1.5.2
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glview-1.5.1/glview/argv.py` & `glview-1.5.2/glview/argv.py`

 * *Files identical despite different names*

### Comparing `glview-1.5.1/glview/glview.py` & `glview-1.5.2/glview/glview.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,20 @@
                 pass
 
     def delete(self, idx):
         """ Remove the given image from this FileList and delete the file from disk. """
         with self.mutex:
             try:
                 filespec = self.filespecs[idx]
-                self.drop([idx])
+                self.filespecs = self._drop(self.filespecs, [idx])
+                self.orientations = self._drop(self.orientations, [idx])
+                self.textures = self._drop(self.textures, [idx])
+                self.metadata = self._drop(self.metadata, [idx])
+                self.images = self._drop(self.images, [idx])
+                self._update()
                 os.remove(filespec)
                 print(f"[{threading.current_thread().name}] Deleted {filespec}")
             except IndexError:
                 pass
 
     def _drop(self, arr, indices):
         arr = np.asarray(arr, dtype=object)
```

### Comparing `glview-1.5.1/glview/imageprovider.py` & `glview-1.5.2/glview/imageprovider.py`

 * *Files identical despite different names*

### Comparing `glview-1.5.1/glview/pygletui.py` & `glview-1.5.2/glview/pygletui.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,21 +184,33 @@
         self.need_redraw = True
 
     def _switch_gamut_curve(self):
         # cycle through a predefined selection of gamut compression modes:
         #  0 - off
         #  1 - steep curve, almost like clipping
         #  2 - shallow curve, strong desaturation
-        presets = [None, (10.0, 1.1, 0.8), (3.0, 1.2, 0.8)]
+        presets = [
+            None,
+            #(10.0, 1.1, 0.8),  # steep
+            #(3.0, 1.2, 0.8),  # shallow
+            (10.0, 1.1, 0.8),  # very shallow
+            (10.0, 1.5, 0.8),  # very shallow
+            (10.0, 100, 0.8),  # very shallow
+            #(3.0, 1.2, [0.8, 0.95, 0.95]),  # shallow red
+            #(3.0, 1.2, [0.95, 0.8, 0.95]),  # shallow green
+        ]
         self.gamut_fit = (self.gamut_fit + 1) % len(presets)
         if (selection := presets[self.gamut_fit]) is not None:
             power, limit, threshold = selection
             self.gamut_pow = np.ones(3) * power
             self.gamut_lim = np.ones(3) * limit
             self.gamut_thr = np.ones(3) * threshold
+            self._vprint(f"Gamut curve shape: pow = {power}, lim = {limit}, thr = {threshold}")
+        else:
+            self._vprint("Gamut compression off")
 
     def _setup_events(self):
         self._vprint("setting up Pyglet window event handlers...")
 
         @self.window.event
         def on_draw():
             self._keyboard_zoom_pan()
```

### Comparing `glview-1.5.1/glview/texture.fs` & `glview-1.5.2/glview/texture.fs`

 * *Files identical despite different names*

### Comparing `glview-1.5.1/glview.egg-info/PKG-INFO` & `glview-1.5.2/glview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.5.1
+Version: 1.5.2
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glview-1.5.1/setup.py` & `glview-1.5.2/setup.py`

 * *Files identical despite different names*

