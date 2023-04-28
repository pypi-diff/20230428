# Comparing `tmp/space-invaders-0.1.8.tar.gz` & `tmp/space-invaders-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.1.8.tar", last modified: Fri Apr 28 12:17:10 2023, max compression
+gzip compressed data, was "space-invaders-0.1.9.tar", last modified: Fri Apr 28 12:27:21 2023, max compression
```

## Comparing `space-invaders-0.1.8.tar` & `space-invaders-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 12:17:10.976266 space-invaders-0.1.8/
--rw-rw-rw-   0        0        0     1138 2023-04-28 11:17:15.000000 space-invaders-0.1.8/LICENSE.md
--rw-rw-rw-   0        0        0     1162 2023-04-28 12:17:10.975267 space-invaders-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      921 2023-04-28 11:11:45.000000 space-invaders-0.1.8/README.md
--rw-rw-rw-   0        0        0     3604 2023-04-28 09:58:23.000000 space-invaders-0.1.8/config.py
--rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.8/entity.py
--rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.8/level.py
--rw-rw-rw-   0        0        0    15947 2023-04-28 10:52:57.000000 space-invaders-0.1.8/main.py
--rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.8/pickup.py
--rw-rw-rw-   0        0        0       42 2023-04-28 12:17:10.976266 space-invaders-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      871 2023-04-28 12:17:08.000000 space-invaders-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:17:10.975267 space-invaders-0.1.8/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     1162 2023-04-28 12:17:10.000000 space-invaders-0.1.8/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-04-28 12:17:10.000000 space-invaders-0.1.8/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 12:17:10.000000 space-invaders-0.1.8/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-28 12:17:10.000000 space-invaders-0.1.8/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 12:17:10.000000 space-invaders-0.1.8/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 12:17:10.000000 space-invaders-0.1.8/space_invaders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.8/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:27:21.993007 space-invaders-0.1.9/
+-rw-rw-rw-   0        0        0     1138 2023-04-28 11:17:15.000000 space-invaders-0.1.9/LICENSE.md
+-rw-rw-rw-   0        0        0     1162 2023-04-28 12:27:21.993007 space-invaders-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2023-04-28 11:11:45.000000 space-invaders-0.1.9/README.md
+-rw-rw-rw-   0        0        0     3604 2023-04-28 09:58:23.000000 space-invaders-0.1.9/config.py
+-rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.9/entity.py
+-rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.9/level.py
+-rw-rw-rw-   0        0        0    15947 2023-04-28 10:52:57.000000 space-invaders-0.1.9/main.py
+-rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.9/pickup.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 12:27:21.993007 space-invaders-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      869 2023-04-28 12:26:54.000000 space-invaders-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:27:21.992008 space-invaders-0.1.9/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     1162 2023-04-28 12:27:21.000000 space-invaders-0.1.9/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-04-28 12:27:21.000000 space-invaders-0.1.9/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 12:27:21.000000 space-invaders-0.1.9/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-28 12:27:21.000000 space-invaders-0.1.9/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 12:27:21.000000 space-invaders-0.1.9/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 12:27:21.000000 space-invaders-0.1.9/space_invaders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.9/spaceship.py
```

### Comparing `space-invaders-0.1.8/LICENSE.md` & `space-invaders-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.8/PKG-INFO` & `space-invaders-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.8
+Version: 0.1.9
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 This game was made as a project for university by BĂłdi Martin
```

### Comparing `space-invaders-0.1.8/README.md` & `space-invaders-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.8/config.py` & `space-invaders-0.1.9/config.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.8/entity.py` & `space-invaders-0.1.9/entity.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.8/level.py` & `space-invaders-0.1.9/level.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.8/main.py` & `space-invaders-0.1.9/main.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.8/pickup.py` & `space-invaders-0.1.9/pickup.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.8/setup.py` & `space-invaders-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='space-invaders',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     py_modules=['main', 'config', 'entity', 'level', 'pickup', 'spaceship'],
     install_requires=[
         'pygame',
         'shapely',
     ],
     author='Bódi Martin',
@@ -22,8 +22,8 @@
     include_package_data=True,
     package_data={
         '': ['*.md'],
         'Sounds': ['*.wav', '*.mp3', '*.ogg'],
         'Sprites': ['*.png'],
         'TestResults': ['TestResults/flake8.txt', 'TestResults/pycodestyle.txt']
     }
-)
+)
```

### Comparing `space-invaders-0.1.8/space_invaders.egg-info/PKG-INFO` & `space-invaders-0.1.9/space_invaders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.8
+Version: 0.1.9
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 This game was made as a project for university by BĂłdi Martin
```

### Comparing `space-invaders-0.1.8/spaceship.py` & `space-invaders-0.1.9/spaceship.py`

 * *Files identical despite different names*

