# Comparing `tmp/animegifs-0.3.4.tar.gz` & `tmp/animegifs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.3.4.tar", last modified: Thu Aug 11 16:09:57 2022, max compression
+gzip compressed data, was "animegifs-0.4.0.tar", last modified: Fri Apr 28 21:03:48 2023, max compression
```

## Comparing `animegifs-0.3.4.tar` & `animegifs-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-08-11 16:09:57.487165 animegifs-0.3.4/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     1161 2022-08-11 16:09:57.478165 animegifs-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      580 2022-08-11 16:08:29.000000 animegifs-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2022-08-11 16:09:57.444162 animegifs-0.3.4/animegifs/
--rw-rw-rw-   0        0        0       42 2022-05-20 00:28:53.000000 animegifs-0.3.4/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3621 2022-08-11 16:08:29.000000 animegifs-0.3.4/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2022-08-11 16:09:57.475164 animegifs-0.3.4/animegifs/dis_utils/
--rw-rw-rw-   0        0        0       40 2022-07-22 19:33:20.000000 animegifs-0.3.4/animegifs/dis_utils/__init__.py
--rw-rw-rw-   0        0        0        6 2022-07-22 19:33:20.000000 animegifs-0.3.4/animegifs/dis_utils/infoes.py
-drwxrwxrwx   0        0        0        0 2022-08-11 16:09:57.467162 animegifs-0.3.4/animegifs.egg-info/
--rw-rw-rw-   0        0        0     1161 2022-08-11 16:09:57.000000 animegifs-0.3.4/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2022-08-11 16:09:57.000000 animegifs-0.3.4/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-11 16:09:57.000000 animegifs-0.3.4/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-08-11 16:09:57.000000 animegifs-0.3.4/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-11 16:09:57.487165 animegifs-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      939 2022-08-11 16:08:29.000000 animegifs-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 21:03:48.135555 animegifs-0.4.0/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1156 2023-04-28 21:03:48.134547 animegifs-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-04-28 20:51:38.000000 animegifs-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 21:03:48.122549 animegifs-0.4.0/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-04-28 19:02:26.000000 animegifs-0.4.0/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     2774 2023-04-28 20:51:38.000000 animegifs-0.4.0/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 21:03:48.132547 animegifs-0.4.0/animegifs/dis_utils/
+-rw-rw-rw-   0        0        0        2 2023-04-28 19:01:35.000000 animegifs-0.4.0/animegifs/dis_utils/__init__.py
+-rw-rw-rw-   0        0        0     1313 2023-04-28 20:51:38.000000 animegifs-0.4.0/animegifs/dis_utils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 21:03:48.129548 animegifs-0.4.0/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-04-28 21:03:48.000000 animegifs-0.4.0/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-28 21:03:48.000000 animegifs-0.4.0/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 21:03:48.000000 animegifs-0.4.0/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 21:03:48.000000 animegifs-0.4.0/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 21:03:48.135555 animegifs-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      939 2023-04-28 20:49:04.000000 animegifs-0.4.0/setup.py
```

### Comparing `animegifs-0.3.4/LICENSE` & `animegifs-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.3.4/PKG-INFO` & `animegifs-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.3.4
+Version: 0.4.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif
 Platform: UNKNOWN
@@ -15,27 +15,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # anime-gifs.py
 Get random anime gifs by category. Use Python (intended initially for Discord).
 
-WIP - updated frequently. v0.2.1 doesn't work anymore.
+WIP - updated in time to time. v0.4.0 is the only working release.
 
 `pip install animegifs`
 
 # HOW TO USE
 
 ```py
-from animegifs import animegifs
 
-gifs = animegifs.Animegifs
+from animegifs.animegifs import Animegifs
 
-gif = gifs(category)
-gif = gif.get_gif()
+gif = Animegifs().get_gif(category)
 ```
 
 **Category list:** 
 
 * Attack
 * Bite
 * Bloodsuck
@@ -55,11 +53,12 @@
 * Harass
 * Highfive
 * Hug
 * Icecream
 * Insult
 * Kill
 * Kiss
+* Lick
 
 WIP.
```

### Comparing `animegifs-0.3.4/README.md` & `animegifs-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # anime-gifs.py
 Get random anime gifs by category. Use Python (intended initially for Discord).
 
-WIP - updated frequently. v0.2.1 doesn't work anymore.
+WIP - updated in time to time. v0.4.0 is the only working release.
 
 `pip install animegifs`
 
 # HOW TO USE
 
 ```py
-from animegifs import animegifs
 
-gifs = animegifs.Animegifs
+from animegifs.animegifs import Animegifs
 
-gif = gifs(category)
-gif = gif.get_gif()
+gif = Animegifs().get_gif(category)
 ```
 
 **Category list:** 
 
 * Attack
 * Bite
 * Bloodsuck
@@ -37,9 +35,10 @@
 * Harass
 * Highfive
 * Hug
 * Icecream
 * Insult
 * Kill
 * Kiss
+* Lick
 
 WIP.
```

### Comparing `animegifs-0.3.4/animegifs.egg-info/PKG-INFO` & `animegifs-0.4.0/animegifs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.3.4
+Version: 0.4.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif
 Platform: UNKNOWN
@@ -15,27 +15,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # anime-gifs.py
 Get random anime gifs by category. Use Python (intended initially for Discord).
 
-WIP - updated frequently. v0.2.1 doesn't work anymore.
+WIP - updated in time to time. v0.4.0 is the only working release.
 
 `pip install animegifs`
 
 # HOW TO USE
 
 ```py
-from animegifs import animegifs
 
-gifs = animegifs.Animegifs
+from animegifs.animegifs import Animegifs
 
-gif = gifs(category)
-gif = gif.get_gif()
+gif = Animegifs().get_gif(category)
 ```
 
 **Category list:** 
 
 * Attack
 * Bite
 * Bloodsuck
@@ -55,11 +53,12 @@
 * Harass
 * Highfive
 * Hug
 * Icecream
 * Insult
 * Kill
 * Kiss
+* Lick
 
 WIP.
```

### Comparing `animegifs-0.3.4/setup.py` & `animegifs-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.3.4'
+VERSION = '0.4.0'
 
 setup(
     name='animegifs',
     packages=find_packages(),
     version=VERSION,
     description='Get random anime gifs by category.',
     long_description=LONG_DESCRIPTION,
```

