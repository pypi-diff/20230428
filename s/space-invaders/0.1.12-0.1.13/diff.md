# Comparing `tmp/space-invaders-0.1.12.tar.gz` & `tmp/space-invaders-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.1.12.tar", last modified: Fri Apr 28 12:40:36 2023, max compression
+gzip compressed data, was "space-invaders-0.1.13.tar", last modified: Fri Apr 28 12:59:54 2023, max compression
```

## Comparing `space-invaders-0.1.12.tar` & `space-invaders-0.1.13.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 12:40:36.971129 space-invaders-0.1.12/
--rw-rw-rw-   0        0        0     1137 2023-04-28 12:40:36.971129 space-invaders-0.1.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 12:40:36.972129 space-invaders-0.1.12/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-04-28 12:40:26.000000 space-invaders-0.1.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:40:36.957695 space-invaders-0.1.12/space-invaders/
--rw-rw-rw-   0        0        0        0 2023-04-28 12:21:47.000000 space-invaders-0.1.12/space-invaders/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-04-28 09:58:23.000000 space-invaders-0.1.12/space-invaders/config.py
--rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.12/space-invaders/entity.py
--rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.12/space-invaders/level.py
--rw-rw-rw-   0        0        0    15947 2023-04-28 10:52:57.000000 space-invaders-0.1.12/space-invaders/main.py
--rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.12/space-invaders/pickup.py
--rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.12/space-invaders/spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:40:36.970130 space-invaders-0.1.12/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     1137 2023-04-28 12:40:36.000000 space-invaders-0.1.12/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-04-28 12:40:36.000000 space-invaders-0.1.12/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 12:40:36.000000 space-invaders-0.1.12/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-28 12:40:36.000000 space-invaders-0.1.12/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 12:40:36.000000 space-invaders-0.1.12/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       57 2023-04-28 12:40:36.000000 space-invaders-0.1.12/space_invaders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 12:59:54.626088 space-invaders-0.1.13/
+-rw-rw-rw-   0        0        0     2340 2023-04-28 12:59:54.625087 space-invaders-0.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 12:59:54.626088 space-invaders-0.1.13/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-04-28 12:44:35.000000 space-invaders-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:59:54.614578 space-invaders-0.1.13/space-invaders/
+-rw-rw-rw-   0        0        0     2116 2023-04-28 12:58:34.000000 space-invaders-0.1.13/space-invaders/README.md
+-rw-rw-rw-   0        0        0        0 2023-04-28 12:21:47.000000 space-invaders-0.1.13/space-invaders/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.13/space-invaders/config.py
+-rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.13/space-invaders/entity.py
+-rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.13/space-invaders/level.py
+-rw-rw-rw-   0        0        0    15947 2023-04-28 10:52:57.000000 space-invaders-0.1.13/space-invaders/main.py
+-rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.13/space-invaders/pickup.py
+-rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.13/space-invaders/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:59:54.625087 space-invaders-0.1.13/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     2340 2023-04-28 12:59:54.000000 space-invaders-0.1.13/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-04-28 12:59:54.000000 space-invaders-0.1.13/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 12:59:54.000000 space-invaders-0.1.13/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-28 12:59:54.000000 space-invaders-0.1.13/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 12:59:54.000000 space-invaders-0.1.13/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       57 2023-04-28 12:59:54.000000 space-invaders-0.1.13/space_invaders.egg-info/top_level.txt
```

### Comparing `space-invaders-0.1.12/setup.py` & `space-invaders-0.1.13/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='space-invaders',
-    version='0.1.12',
+    version='0.1.13',
     packages=find_packages(),
     py_modules=['main', 'config', 'entity', 'level', 'pickup', 'spaceship'],
     install_requires=[
         'pygame',
         'shapely',
     ],
     author='Bódi Martin',
@@ -17,10 +17,10 @@
     entry_points={
         'console_scripts': [
             'space-invaders = main:main'
         ]
     },
     include_package_data=True,
     package_data={
-        'space-invader': ['*']
+        '': ['*']
     }
 )
```

### Comparing `space-invaders-0.1.12/space-invaders/config.py` & `space-invaders-0.1.13/space-invaders/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 RESET_SWITCH_DELAY = 200
 PICKUP_SPEED = 5
 PICKUP_SPAWN_INTERVAL = (4, 8)
 score = 0
 
 SHOW_HIT_BOXES = False
 WINDOW_WIDTH = 1400
-WINDOW_HEIGHT = 1000
+WINDOW_HEIGHT = 950
 CAPTION = "Space Invader"
 BACKGROUND_IMAGE = "sprites/background.png"
 
 
 def get_credits_text():
     return f"""CONGRATULATIONS!
 YOU HAVE SUCCESSFULLY BEATEN THE GAME!
```

### Comparing `space-invaders-0.1.12/space-invaders/entity.py` & `space-invaders-0.1.13/space-invaders/entity.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.12/space-invaders/level.py` & `space-invaders-0.1.13/space-invaders/level.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.12/space-invaders/main.py` & `space-invaders-0.1.13/space-invaders/main.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.12/space-invaders/pickup.py` & `space-invaders-0.1.13/space-invaders/pickup.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.12/space-invaders/spaceship.py` & `space-invaders-0.1.13/space-invaders/spaceship.py`

 * *Files identical despite different names*

