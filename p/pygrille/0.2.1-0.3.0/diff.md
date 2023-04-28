# Comparing `tmp/pygrille-0.2.1.tar.gz` & `tmp/pygrille-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrille-0.2.1.tar", last modified: Fri Jan 13 15:57:36 2023, max compression
+gzip compressed data, was "dist\pygrille-0.3.0.tar", last modified: Fri Apr 28 09:30:22 2023, max compression
```

## Comparing `pygrille-0.2.1.tar` & `pygrille-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 15:57:36.890946 pygrille-0.2.1/
--rw-rw-rw-   0        0        0     3484 2023-01-13 15:57:36.888951 pygrille-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2656 2023-01-13 15:55:08.000000 pygrille-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-01-13 15:57:36.891943 pygrille-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-01-13 11:30:03.000000 pygrille-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-13 15:57:36.872995 pygrille-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-01-13 15:57:36.885959 pygrille-0.2.1/src/pygrille.egg-info/
--rw-rw-rw-   0        0        0     3484 2023-01-13 15:57:36.000000 pygrille-0.2.1/src/pygrille.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-01-13 15:57:36.000000 pygrille-0.2.1/src/pygrille.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 15:57:36.000000 pygrille-0.2.1/src/pygrille.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-13 15:57:36.000000 pygrille-0.2.1/src/pygrille.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-13 15:57:36.000000 pygrille-0.2.1/src/pygrille.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14702 2023-01-13 11:32:55.000000 pygrille-0.2.1/src/pygrille.py
--rw-rw-rw-   0        0        0     1620 2022-12-06 18:13:29.000000 pygrille-0.2.1/src/text.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:30:22.387229 pygrille-0.3.0/
+-rw-rw-rw-   0        0        0     3849 2023-04-28 09:30:22.387229 pygrille-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2989 2023-04-28 09:24:50.000000 pygrille-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:30:22.387229 pygrille-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-04-28 09:25:37.000000 pygrille-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:30:22.371603 pygrille-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 09:30:22.387229 pygrille-0.3.0/src/pygrille.egg-info/
+-rw-rw-rw-   0        0        0     3849 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18057 2023-04-28 09:25:53.000000 pygrille-0.3.0/src/pygrille.py
+-rw-rw-rw-   0        0        0     1620 2022-12-06 18:13:29.000000 pygrille-0.3.0/src/text.py
```

### Comparing `pygrille-0.2.1/PKG-INFO` & `pygrille-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrille
-Version: 0.2.1
+Version: 0.3.0
 Summary: A quick way to write and visualise any code involving grids of squares in python.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Pygrille
         
         Pygrille is a Python library that uses Pygame to make it easier to do many things involving a square grid.
         
@@ -30,17 +30,17 @@
         
         # Ensures the grid has not been closed each frame. 
         # Also updates the newclick and newkey variables (booleans - True if there is a new click or key press) 
         # And the lastclick (tuple - grid location of most recent click) and lastkey (string - name of most recent key pressed) variables.
         while grid.check_open():
         
             # If the user clicks on a square, set it to a random colour and set the border to a random colour.
-            if grid.newclick:
-                grid[grid.lastclick[0]][grid.lastclick[1]].colour = pygrille.random_colour()
-                grid[grid.lastclick[0]][grid.lastclick[1]].extras["Hello"] = "Clicked"
+            if grid.new_mouse_up:
+                grid[grid.last_mouse_up[0]][grid.last_mouse_up[1]].colour = pygrille.random_colour()
+                grid[grid.last_mouse_up[0]][grid.last_mouse_up[1]].extras["Hello"] = "Clicked"
                 grid.border_colour = pygrille.random_colour()
         
             # If the spacebar is pressed, print the status of the extra value "Hello" in the top left pixel.
             if grid.newkey:
                 if grid.lastkey == "space":
                     print(grid[0][0].extras["Hello"])
         
@@ -53,16 +53,20 @@
         # Once pygrille is closed, finish quitting it.
         grid.quit()
         
         ```
         
         ## Updates
         
+        ### 0.3.0
+        * Added support for border size overrides - this allows for certain border lines to be wider than others.
+        * Added mouse-down and mouse-over support. Replaced "lastclick" and "newclick" with "last_mouse_up" and "new_mouse_up". Please update any past code that used these attributes to reflect this.
+        
         ### 0.2.1
-        * Added a check for clicking UI elements via the grid.newclick_ui and grid.clicked_ui attributes.
+        * Added a check for clicking UI elements via the Grid.newclick_ui and Grid.clicked_ui attributes.
         * Fixed an error in the example code in this README.
         * Other minor changes.
         
         ### 0.2.0.1
         * Reupload due to issue with first upload of 0.2.0.
         
         ### 0.2.0
```

### Comparing `pygrille-0.2.1/README.md` & `pygrille-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 # Ensures the grid has not been closed each frame. 
 # Also updates the newclick and newkey variables (booleans - True if there is a new click or key press) 
 # And the lastclick (tuple - grid location of most recent click) and lastkey (string - name of most recent key pressed) variables.
 while grid.check_open():
 
     # If the user clicks on a square, set it to a random colour and set the border to a random colour.
-    if grid.newclick:
-        grid[grid.lastclick[0]][grid.lastclick[1]].colour = pygrille.random_colour()
-        grid[grid.lastclick[0]][grid.lastclick[1]].extras["Hello"] = "Clicked"
+    if grid.new_mouse_up:
+        grid[grid.last_mouse_up[0]][grid.last_mouse_up[1]].colour = pygrille.random_colour()
+        grid[grid.last_mouse_up[0]][grid.last_mouse_up[1]].extras["Hello"] = "Clicked"
         grid.border_colour = pygrille.random_colour()
 
     # If the spacebar is pressed, print the status of the extra value "Hello" in the top left pixel.
     if grid.newkey:
         if grid.lastkey == "space":
             print(grid[0][0].extras["Hello"])
 
@@ -47,16 +47,20 @@
 # Once pygrille is closed, finish quitting it.
 grid.quit()
 
 ```
 
 ## Updates
 
+### 0.3.0
+* Added support for border size overrides - this allows for certain border lines to be wider than others.
+* Added mouse-down and mouse-over support. Replaced "lastclick" and "newclick" with "last_mouse_up" and "new_mouse_up". Please update any past code that used these attributes to reflect this.
+
 ### 0.2.1
-* Added a check for clicking UI elements via the grid.newclick_ui and grid.clicked_ui attributes.
+* Added a check for clicking UI elements via the Grid.newclick_ui and Grid.clicked_ui attributes.
 * Fixed an error in the example code in this README.
 * Other minor changes.
 
 ### 0.2.0.1
 * Reupload due to issue with first upload of 0.2.0.
 
 ### 0.2.0
```

### Comparing `pygrille-0.2.1/src/pygrille.egg-info/PKG-INFO` & `pygrille-0.3.0/src/pygrille.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrille
-Version: 0.2.1
+Version: 0.3.0
 Summary: A quick way to write and visualise any code involving grids of squares in python.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Pygrille
         
         Pygrille is a Python library that uses Pygame to make it easier to do many things involving a square grid.
         
@@ -30,17 +30,17 @@
         
         # Ensures the grid has not been closed each frame. 
         # Also updates the newclick and newkey variables (booleans - True if there is a new click or key press) 
         # And the lastclick (tuple - grid location of most recent click) and lastkey (string - name of most recent key pressed) variables.
         while grid.check_open():
         
             # If the user clicks on a square, set it to a random colour and set the border to a random colour.
-            if grid.newclick:
-                grid[grid.lastclick[0]][grid.lastclick[1]].colour = pygrille.random_colour()
-                grid[grid.lastclick[0]][grid.lastclick[1]].extras["Hello"] = "Clicked"
+            if grid.new_mouse_up:
+                grid[grid.last_mouse_up[0]][grid.last_mouse_up[1]].colour = pygrille.random_colour()
+                grid[grid.last_mouse_up[0]][grid.last_mouse_up[1]].extras["Hello"] = "Clicked"
                 grid.border_colour = pygrille.random_colour()
         
             # If the spacebar is pressed, print the status of the extra value "Hello" in the top left pixel.
             if grid.newkey:
                 if grid.lastkey == "space":
                     print(grid[0][0].extras["Hello"])
         
@@ -53,16 +53,20 @@
         # Once pygrille is closed, finish quitting it.
         grid.quit()
         
         ```
         
         ## Updates
         
+        ### 0.3.0
+        * Added support for border size overrides - this allows for certain border lines to be wider than others.
+        * Added mouse-down and mouse-over support. Replaced "lastclick" and "newclick" with "last_mouse_up" and "new_mouse_up". Please update any past code that used these attributes to reflect this.
+        
         ### 0.2.1
-        * Added a check for clicking UI elements via the grid.newclick_ui and grid.clicked_ui attributes.
+        * Added a check for clicking UI elements via the Grid.newclick_ui and Grid.clicked_ui attributes.
         * Fixed an error in the example code in this README.
         * Other minor changes.
         
         ### 0.2.0.1
         * Reupload due to issue with first upload of 0.2.0.
         
         ### 0.2.0
```

### Comparing `pygrille-0.2.1/src/text.py` & `pygrille-0.3.0/src/text.py`

 * *Files identical despite different names*

