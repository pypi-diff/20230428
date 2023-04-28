# Comparing `tmp/pygrille-0.3.0.tar.gz` & `tmp/pygrille-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygrille-0.3.0.tar", last modified: Fri Apr 28 09:30:22 2023, max compression
+gzip compressed data, was "dist\pygrille-0.3.1.tar", last modified: Fri Apr 28 10:09:01 2023, max compression
```

## Comparing `pygrille-0.3.0.tar` & `pygrille-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 09:30:22.387229 pygrille-0.3.0/
--rw-rw-rw-   0        0        0     3849 2023-04-28 09:30:22.387229 pygrille-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2989 2023-04-28 09:24:50.000000 pygrille-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 09:30:22.387229 pygrille-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-04-28 09:25:37.000000 pygrille-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:30:22.371603 pygrille-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 09:30:22.387229 pygrille-0.3.0/src/pygrille.egg-info/
--rw-rw-rw-   0        0        0     3849 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 09:30:22.000000 pygrille-0.3.0/src/pygrille.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18057 2023-04-28 09:25:53.000000 pygrille-0.3.0/src/pygrille.py
--rw-rw-rw-   0        0        0     1620 2022-12-06 18:13:29.000000 pygrille-0.3.0/src/text.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:09:01.890358 pygrille-0.3.1/
+-rw-rw-rw-   0        0        0     3849 2023-04-28 10:09:01.874735 pygrille-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2989 2023-04-28 09:24:50.000000 pygrille-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 10:09:01.890358 pygrille-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-04-28 10:08:03.000000 pygrille-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:09:01.859111 pygrille-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 10:09:01.874735 pygrille-0.3.1/src/pygrille.egg-info/
+-rw-rw-rw-   0        0        0     3849 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 10:09:01.000000 pygrille-0.3.1/src/pygrille.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18059 2023-04-28 10:08:19.000000 pygrille-0.3.1/src/pygrille.py
+-rw-rw-rw-   0        0        0     1620 2022-12-06 18:13:29.000000 pygrille-0.3.1/src/text.py
```

### Comparing `pygrille-0.3.0/PKG-INFO` & `pygrille-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrille
-Version: 0.3.0
+Version: 0.3.1
 Summary: A quick way to write and visualise any code involving grids of squares in python.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Pygrille
         
         Pygrille is a Python library that uses Pygame to make it easier to do many things involving a square grid.
```

### Comparing `pygrille-0.3.0/README.md` & `pygrille-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pygrille-0.3.0/src/pygrille.egg-info/PKG-INFO` & `pygrille-0.3.1/src/pygrille.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrille
-Version: 0.3.0
+Version: 0.3.1
 Summary: A quick way to write and visualise any code involving grids of squares in python.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Pygrille
         
         Pygrille is a Python library that uses Pygame to make it easier to do many things involving a square grid.
```

### Comparing `pygrille-0.3.0/src/pygrille.py` & `pygrille-0.3.1/src/pygrille.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                     lower_limit = self.ui[image_name]["coords"]
                     upper_limit = [self.ui[image_name]["coords"][i] +
                                    self.ui[image_name]["image"].get_size()[i] for i in (0, 1)]
                     if all([lower_limit[i] <= pos[i] <= upper_limit[i] for i in (0, 1)]):
                         if not self.new_mouse_down_ui:
                             self.mouse_down_ui = []
                         self.new_mouse_down_ui = True
-                        self.mouse_up_ui.append(image_name)
+                        self.mouse_down_ui.append(image_name)
 
             # If the event is a KEYDOWN event (a key is pressed)
             elif event.type == pygame.KEYDOWN:
                 # Add the key that was pressed to the list of keys
                 self.keylist.append(pygame.key.name(event.key))
                 # Store the last key that was pressed
                 self.lastkey = pygame.key.name(event.key)
```

### Comparing `pygrille-0.3.0/src/text.py` & `pygrille-0.3.1/src/text.py`

 * *Files identical despite different names*

