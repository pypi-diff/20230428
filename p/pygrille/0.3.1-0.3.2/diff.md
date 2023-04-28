# Comparing `tmp/pygrille-0.3.1.tar.gz` & `tmp/pygrille-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygrille-0.3.1.tar", last modified: Fri Apr 28 10:09:01 2023, max compression
+gzip compressed data, was "dist\pygrille-0.3.2.tar", last modified: Fri Apr 28 10:34:05 2023, max compression
```

## Comparing `pygrille-0.3.1.tar` & `pygrille-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 10:09:01.890358 pygrille-0.3.1/
--rw-rw-rw-   0        0        0     3849 2023-04-28 10:09:01.874735 pygrille-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2989 2023-04-28 09:24:50.000000 pygrille-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 10:09:01.890358 pygrille-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-04-28 10:08:03.000000 pygrille-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 10:09:01.859111 pygrille-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 10:09:01.874735 pygrille-0.3.1/src/pygrille.egg-info/
--rw-rw-rw-   0        0        0     3849 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18059 2023-04-28 10:08:19.000000 pygrille-0.3.1/src/pygrille.py
--rw-rw-rw-   0        0        0     1620 2022-12-06 18:13:29.000000 pygrille-0.3.1/src/text.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:34:05.781958 pygrille-0.3.2/
+-rw-rw-rw-   0        0        0     4036 2023-04-28 10:34:05.781958 pygrille-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3128 2023-04-28 10:28:40.000000 pygrille-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 10:34:05.781958 pygrille-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-04-28 10:28:07.000000 pygrille-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:34:05.766331 pygrille-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 10:34:05.781958 pygrille-0.3.2/src/pygrille.egg-info/
+-rw-rw-rw-   0        0        0     4036 2023-04-28 10:34:05.000000 pygrille-0.3.2/src/pygrille.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-04-28 10:34:05.000000 pygrille-0.3.2/src/pygrille.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 10:34:05.000000 pygrille-0.3.2/src/pygrille.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 10:34:05.000000 pygrille-0.3.2/src/pygrille.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 10:34:05.000000 pygrille-0.3.2/src/pygrille.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18408 2023-04-28 10:33:20.000000 pygrille-0.3.2/src/pygrille.py
+-rw-rw-rw-   0        0        0     1620 2022-12-06 18:13:29.000000 pygrille-0.3.2/src/text.py
```

### Comparing `pygrille-0.3.1/PKG-INFO` & `pygrille-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrille
-Version: 0.3.1
+Version: 0.3.2
 Summary: A quick way to write and visualise any code involving grids of squares in python.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Pygrille
         
         Pygrille is a Python library that uses Pygame to make it easier to do many things involving a square grid.
         
@@ -53,14 +53,20 @@
         # Once pygrille is closed, finish quitting it.
         grid.quit()
         
         ```
         
         ## Updates
         
+        ### 0.3.2
+        * Fixed bug with image sizes when images were used multiple times.
+        
+        ### 0.3.1
+        * Fixed bug with mouse-down on UI elements.
+        
         ### 0.3.0
         * Added support for border size overrides - this allows for certain border lines to be wider than others.
         * Added mouse-down and mouse-over support. Replaced "lastclick" and "newclick" with "last_mouse_up" and "new_mouse_up". Please update any past code that used these attributes to reflect this.
         
         ### 0.2.1
         * Added a check for clicking UI elements via the Grid.newclick_ui and Grid.clicked_ui attributes.
         * Fixed an error in the example code in this README.
```

### Comparing `pygrille-0.3.1/README.md` & `pygrille-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 # Once pygrille is closed, finish quitting it.
 grid.quit()
 
 ```
 
 ## Updates
 
+### 0.3.2
+* Fixed bug with image sizes when images were used multiple times.
+
+### 0.3.1
+* Fixed bug with mouse-down on UI elements.
+
 ### 0.3.0
 * Added support for border size overrides - this allows for certain border lines to be wider than others.
 * Added mouse-down and mouse-over support. Replaced "lastclick" and "newclick" with "last_mouse_up" and "new_mouse_up". Please update any past code that used these attributes to reflect this.
 
 ### 0.2.1
 * Added a check for clicking UI elements via the Grid.newclick_ui and Grid.clicked_ui attributes.
 * Fixed an error in the example code in this README.
```

### Comparing `pygrille-0.3.1/src/pygrille.egg-info/PKG-INFO` & `pygrille-0.3.2/src/pygrille.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrille
-Version: 0.3.1
+Version: 0.3.2
 Summary: A quick way to write and visualise any code involving grids of squares in python.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Pygrille
         
         Pygrille is a Python library that uses Pygame to make it easier to do many things involving a square grid.
         
@@ -53,14 +53,20 @@
         # Once pygrille is closed, finish quitting it.
         grid.quit()
         
         ```
         
         ## Updates
         
+        ### 0.3.2
+        * Fixed bug with image sizes when images were used multiple times.
+        
+        ### 0.3.1
+        * Fixed bug with mouse-down on UI elements.
+        
         ### 0.3.0
         * Added support for border size overrides - this allows for certain border lines to be wider than others.
         * Added mouse-down and mouse-over support. Replaced "lastclick" and "newclick" with "last_mouse_up" and "new_mouse_up". Please update any past code that used these attributes to reflect this.
         
         ### 0.2.1
         * Added a check for clicking UI elements via the Grid.newclick_ui and Grid.clicked_ui attributes.
         * Fixed an error in the example code in this README.
```

### Comparing `pygrille-0.3.1/src/pygrille.py` & `pygrille-0.3.2/src/pygrille.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         # return the string representation of the pixel's label
         return str(self.label)
 
     def __getitem__(self, key):
         # allow the extras to be accessed.
         return self.extras[key]
 
+    def __setitem__(self, key, item):
+        # allow the extras to be set.
+        self.extras[key] = item
+
 
 
 class Grid:
     def __init__(self, pixel_size: int, grid_dimensions: tuple[int, int], *, window_name: str = None,
                  default_colour: tuple[int, int, int] = None, extras: list[str] = None, framerate: int = None, border_width: int = None, border_width_override: list[dict[int, int]] = None,
                  border_colour: tuple[int, int, int] = None, default_image: str = None, display_offset_x: int = 0,
                  display_offset_y: int = 0, forced_window_size: tuple[int, int] = None):
@@ -289,15 +293,18 @@
 
     def set_image(self, pos: tuple, image_path: str):
         # Check if the image is already loaded in memory
         if image_path not in self.images.keys():
             # If not, load the image and store it in the images dictionary
             self.images[image_path] = self.load_image(image_path, self.pixel_size)
         # Set the image at the specified position in the game grid
-        self.grid[pos[0]][pos[1]].image = self.images[image_path]
+        if self.images[image_path].get_size() != (self.pixel_size, self.pixel_size):
+            self.grid[pos[0]][pos[1]].image = pygame.transform.scale(self.images[image_path], (self.pixel_size, self.pixel_size))
+        else:
+            self.grid[pos[0]][pos[1]].image = self.images[image_path]
 
     def set_ui(self, name: str, image_path: str, window_coords: tuple, scale: tuple = None):
         # Check if the image is already loaded in memory
         if image_path not in self.images.keys():
             # If not, load the image
             self.images[image_path] = pygame.image.load(image_path)
         # Get the image from the images dictionary
```

### Comparing `pygrille-0.3.1/src/text.py` & `pygrille-0.3.2/src/text.py`

 * *Files identical despite different names*

