# Comparing `tmp/Turk_game-1.0.4.tar.gz` & `tmp/Turk_game-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Turk_game-1.0.4.tar", last modified: Fri Apr 28 14:22:03 2023, max compression
+gzip compressed data, was "Turk_game-1.0.5.tar", last modified: Fri Apr 28 14:29:25 2023, max compression
```

## Comparing `Turk_game-1.0.4.tar` & `Turk_game-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 14:22:02.000000 Turk_game-1.0.4/
--rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      277 2023-04-28 14:22:04.000000 Turk_game-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/
--rw-rw-rw-   0        0        0      277 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3783 2023-04-28 14:21:02.000000 Turk_game-1.0.4/Turk_game.py
--rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.4/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-28 14:22:04.000000 Turk_game-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-04-28 14:16:26.000000 Turk_game-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:29:26.000000 Turk_game-1.0.5/
+-rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      239 2023-04-28 14:29:26.000000 Turk_game-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 14:29:26.000000 Turk_game-1.0.5/Turk_game.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-04-28 14:29:26.000000 Turk_game-1.0.5/Turk_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-04-28 14:29:26.000000 Turk_game-1.0.5/Turk_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:29:26.000000 Turk_game-1.0.5/Turk_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-28 14:29:26.000000 Turk_game-1.0.5/Turk_game.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:29:26.000000 Turk_game-1.0.5/Turk_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3783 2023-04-28 14:21:02.000000 Turk_game-1.0.5/Turk_game.py
+-rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.5/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 14:29:26.000000 Turk_game-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      432 2023-04-28 14:29:20.000000 Turk_game-1.0.5/setup.py
```

### Comparing `Turk_game-1.0.4/LICENSE` & `Turk_game-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.4/README.md` & `Turk_game-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.4/Turk_game.py` & `Turk_game-1.0.5/Turk_game.py`

 * *Files identical despite different names*

