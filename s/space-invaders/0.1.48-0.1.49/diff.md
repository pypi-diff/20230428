# Comparing `tmp/space-invaders-0.1.48.tar.gz` & `tmp/space-invaders-0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.1.48.tar", last modified: Fri Apr 28 15:25:04 2023, max compression
+gzip compressed data, was "space-invaders-0.1.49.tar", last modified: Fri Apr 28 15:27:26 2023, max compression
```

## Comparing `space-invaders-0.1.48.tar` & `space-invaders-0.1.49.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 15:25:04.449155 space-invaders-0.1.48/
--rw-rw-rw-   0        0        0      261 2023-04-28 13:39:07.000000 space-invaders-0.1.48/MANIFEST.in
--rw-rw-rw-   0        0        0     2340 2023-04-28 15:25:04.448155 space-invaders-0.1.48/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 15:25:04.449155 space-invaders-0.1.48/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-04-28 15:24:49.000000 space-invaders-0.1.48/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:25:04.407455 space-invaders-0.1.48/space-invaders/
-drwxrwxrwx   0        0        0        0 2023-04-28 15:25:04.409454 space-invaders-0.1.48/space-invaders/Fonts/
--rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.1.48/space-invaders/Fonts/AGENCYB.TTF
--rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.1.48/space-invaders/Fonts/AGENCYR.TTF
--rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.1.48/space-invaders/Fonts/Alien Invader Italic.ttf
--rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.1.48/space-invaders/Fonts/Alien Invader.ttf
--rw-rw-rw-   0        0        0     2116 2023-04-28 12:58:34.000000 space-invaders-0.1.48/space-invaders/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 15:25:04.422479 space-invaders-0.1.48/space-invaders/Sounds/
--rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.1.48/space-invaders/Sounds/122255__jivatma07__level_complete.wav
--rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.1.48/space-invaders/Sounds/156895__halgrimm__a-shot.wav
--rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.1.48/space-invaders/Sounds/18380__inferno__hvrl.wav
--rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.1.48/space-invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
--rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.1.48/space-invaders/Sounds/340452__zagi2__dondolan2-loop.wav
--rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.1.48/space-invaders/Sounds/353775__samueloak89__next-scene.mp3
--rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.1.48/space-invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
--rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.1.48/space-invaders/Sounds/565481__jakegwizdak__small-explosion.wav
--rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.1.48/space-invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
--rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.1.48/space-invaders/Sounds/648200__strangehorizon__glitch_blip.wav
--rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.1.48/space-invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
-drwxrwxrwx   0        0        0        0 2023-04-28 15:25:04.436646 space-invaders-0.1.48/space-invaders/Sprites/
--rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.1.48/space-invaders/Sprites/background.png
--rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.1.48/space-invaders/Sprites/default_enemy_gun.png
--rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.1.48/space-invaders/Sprites/default_enemy_projectile.png
--rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.1.48/space-invaders/Sprites/default_enemy_ship.png
--rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.1.48/space-invaders/Sprites/default_gun.png
--rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.1.48/space-invaders/Sprites/default_gun_pickup.png
--rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.1.48/space-invaders/Sprites/default_projectile.png
--rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.1.48/space-invaders/Sprites/default_ship.png
--rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.1.48/space-invaders/Sprites/explosion.png
--rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.1.48/space-invaders/Sprites/fire_rate_booster.png
--rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.1.48/space-invaders/Sprites/life.png
--rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.1.48/space-invaders/Sprites/medium_heal.png
--rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.1.48/space-invaders/Sprites/minigun.png
--rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.1.48/space-invaders/Sprites/minigun_pickup.png
--rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.1.48/space-invaders/Sprites/minigun_projectile.png
--rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.1.48/space-invaders/Sprites/repair.png
--rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.1.48/space-invaders/Sprites/rocket_gun.png
--rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.1.48/space-invaders/Sprites/rocket_gun_pickup.png
--rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.1.48/space-invaders/Sprites/rocket_projectile.png
--rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.1.48/space-invaders/Sprites/ship_explosion.png
--rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.1.48/space-invaders/Sprites/small_heal.png
-drwxrwxrwx   0        0        0        0 2023-04-28 15:25:04.437645 space-invaders-0.1.48/space-invaders/TestResults/
--rw-rw-rw-   0        0        0      157 2023-04-28 10:17:05.000000 space-invaders-0.1.48/space-invaders/TestResults/flake8.txt
--rw-rw-rw-   0        0        0      146 2023-04-28 10:06:54.000000 space-invaders-0.1.48/space-invaders/TestResults/pycodestyle.txt
--rw-rw-rw-   0        0        0        2 2023-04-28 14:44:34.000000 space-invaders-0.1.48/space-invaders/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.48/space-invaders/config.py
--rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.48/space-invaders/entity.py
--rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.48/space-invaders/level.py
--rw-rw-rw-   0        0        0    15947 2023-04-28 14:28:34.000000 space-invaders-0.1.48/space-invaders/main.py
--rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.48/space-invaders/pickup.py
--rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.48/space-invaders/spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:25:04.448155 space-invaders-0.1.48/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     2340 2023-04-28 15:25:04.000000 space-invaders-0.1.48/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2235 2023-04-28 15:25:04.000000 space-invaders-0.1.48/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 15:25:04.000000 space-invaders-0.1.48/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-28 15:25:04.000000 space-invaders-0.1.48/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 15:25:04.000000 space-invaders-0.1.48/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 15:25:04.000000 space-invaders-0.1.48/space_invaders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 15:27:26.124319 space-invaders-0.1.49/
+-rw-rw-rw-   0        0        0      261 2023-04-28 13:39:07.000000 space-invaders-0.1.49/MANIFEST.in
+-rw-rw-rw-   0        0        0     2340 2023-04-28 15:27:26.124319 space-invaders-0.1.49/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 15:27:26.124319 space-invaders-0.1.49/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-04-28 15:27:14.000000 space-invaders-0.1.49/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:27:26.084417 space-invaders-0.1.49/space-invaders/
+drwxrwxrwx   0        0        0        0 2023-04-28 15:27:26.087417 space-invaders-0.1.49/space-invaders/Fonts/
+-rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.1.49/space-invaders/Fonts/AGENCYB.TTF
+-rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.1.49/space-invaders/Fonts/AGENCYR.TTF
+-rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.1.49/space-invaders/Fonts/Alien Invader Italic.ttf
+-rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.1.49/space-invaders/Fonts/Alien Invader.ttf
+-rw-rw-rw-   0        0        0     2116 2023-04-28 12:58:34.000000 space-invaders-0.1.49/space-invaders/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 15:27:26.098893 space-invaders-0.1.49/space-invaders/Sounds/
+-rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.1.49/space-invaders/Sounds/122255__jivatma07__level_complete.wav
+-rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.1.49/space-invaders/Sounds/156895__halgrimm__a-shot.wav
+-rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.1.49/space-invaders/Sounds/18380__inferno__hvrl.wav
+-rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.1.49/space-invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
+-rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.1.49/space-invaders/Sounds/340452__zagi2__dondolan2-loop.wav
+-rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.1.49/space-invaders/Sounds/353775__samueloak89__next-scene.mp3
+-rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.1.49/space-invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
+-rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.1.49/space-invaders/Sounds/565481__jakegwizdak__small-explosion.wav
+-rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.1.49/space-invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
+-rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.1.49/space-invaders/Sounds/648200__strangehorizon__glitch_blip.wav
+-rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.1.49/space-invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
+drwxrwxrwx   0        0        0        0 2023-04-28 15:27:26.112295 space-invaders-0.1.49/space-invaders/Sprites/
+-rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.1.49/space-invaders/Sprites/background.png
+-rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.1.49/space-invaders/Sprites/default_enemy_gun.png
+-rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.1.49/space-invaders/Sprites/default_enemy_projectile.png
+-rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.1.49/space-invaders/Sprites/default_enemy_ship.png
+-rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.1.49/space-invaders/Sprites/default_gun.png
+-rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.1.49/space-invaders/Sprites/default_gun_pickup.png
+-rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.1.49/space-invaders/Sprites/default_projectile.png
+-rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.1.49/space-invaders/Sprites/default_ship.png
+-rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.1.49/space-invaders/Sprites/explosion.png
+-rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.1.49/space-invaders/Sprites/fire_rate_booster.png
+-rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.1.49/space-invaders/Sprites/life.png
+-rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.1.49/space-invaders/Sprites/medium_heal.png
+-rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.1.49/space-invaders/Sprites/minigun.png
+-rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.1.49/space-invaders/Sprites/minigun_pickup.png
+-rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.1.49/space-invaders/Sprites/minigun_projectile.png
+-rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.1.49/space-invaders/Sprites/repair.png
+-rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.1.49/space-invaders/Sprites/rocket_gun.png
+-rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.1.49/space-invaders/Sprites/rocket_gun_pickup.png
+-rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.1.49/space-invaders/Sprites/rocket_projectile.png
+-rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.1.49/space-invaders/Sprites/ship_explosion.png
+-rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.1.49/space-invaders/Sprites/small_heal.png
+drwxrwxrwx   0        0        0        0 2023-04-28 15:27:26.113294 space-invaders-0.1.49/space-invaders/TestResults/
+-rw-rw-rw-   0        0        0      157 2023-04-28 10:17:05.000000 space-invaders-0.1.49/space-invaders/TestResults/flake8.txt
+-rw-rw-rw-   0        0        0      146 2023-04-28 10:06:54.000000 space-invaders-0.1.49/space-invaders/TestResults/pycodestyle.txt
+-rw-rw-rw-   0        0        0        2 2023-04-28 14:44:34.000000 space-invaders-0.1.49/space-invaders/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.49/space-invaders/config.py
+-rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.49/space-invaders/entity.py
+-rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.49/space-invaders/level.py
+-rw-rw-rw-   0        0        0    15947 2023-04-28 14:28:34.000000 space-invaders-0.1.49/space-invaders/main.py
+-rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.49/space-invaders/pickup.py
+-rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.49/space-invaders/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:27:26.123319 space-invaders-0.1.49/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     2340 2023-04-28 15:27:26.000000 space-invaders-0.1.49/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2235 2023-04-28 15:27:26.000000 space-invaders-0.1.49/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 15:27:26.000000 space-invaders-0.1.49/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-28 15:27:26.000000 space-invaders-0.1.49/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 15:27:26.000000 space-invaders-0.1.49/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 15:27:26.000000 space-invaders-0.1.49/space_invaders.egg-info/top_level.txt
```

### Comparing `space-invaders-0.1.48/PKG-INFO` & `space-invaders-0.1.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.48
+Version: 0.1.49
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.1.48/setup.py` & `space-invaders-0.1.49/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='space-invaders',
-    version='0.1.48',
+    version='0.1.49',
     packages=find_packages(),
     py_modules=['main'],
     install_requires=[
         'pygame',
         'shapely'
     ],
     author='Bódi Martin',
     author_email='bodimartin22@gmail.com',
     description='A cool space shooter rouge like game',
     long_description=open('space-invaders/README.md').read(),
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
-            'space-invaders = main:main'
+            'space-invaders = main:foo'
         ]
     },
     include_package_data=True,
     package_data={
         'space-invaders': ['*.md', 'Sprites/*.png', 'Sounds/*.wav', 'Sounds/*.mp3', 'Sounds/*.ogg', 'TestResults/*.txt', 'Fonts/*.ttf', 'Fonts/*.TTF']
     }
 )
```

### Comparing `space-invaders-0.1.48/space-invaders/Fonts/AGENCYB.TTF` & `space-invaders-0.1.49/space-invaders/Fonts/AGENCYB.TTF`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Fonts/AGENCYR.TTF` & `space-invaders-0.1.49/space-invaders/Fonts/AGENCYR.TTF`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Fonts/Alien Invader Italic.ttf` & `space-invaders-0.1.49/space-invaders/Fonts/Alien Invader Italic.ttf`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Fonts/Alien Invader.ttf` & `space-invaders-0.1.49/space-invaders/Fonts/Alien Invader.ttf`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/README.md` & `space-invaders-0.1.49/space-invaders/README.md`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/122255__jivatma07__level_complete.wav` & `space-invaders-0.1.49/space-invaders/Sounds/122255__jivatma07__level_complete.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/156895__halgrimm__a-shot.wav` & `space-invaders-0.1.49/space-invaders/Sounds/156895__halgrimm__a-shot.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/18380__inferno__hvrl.wav` & `space-invaders-0.1.49/space-invaders/Sounds/18380__inferno__hvrl.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav` & `space-invaders-0.1.49/space-invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/340452__zagi2__dondolan2-loop.wav` & `space-invaders-0.1.49/space-invaders/Sounds/340452__zagi2__dondolan2-loop.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/353775__samueloak89__next-scene.mp3` & `space-invaders-0.1.49/space-invaders/Sounds/353775__samueloak89__next-scene.mp3`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg` & `space-invaders-0.1.49/space-invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/565481__jakegwizdak__small-explosion.wav` & `space-invaders-0.1.49/space-invaders/Sounds/565481__jakegwizdak__small-explosion.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav` & `space-invaders-0.1.49/space-invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/648200__strangehorizon__glitch_blip.wav` & `space-invaders-0.1.49/space-invaders/Sounds/648200__strangehorizon__glitch_blip.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sounds/678384__jocabundus__item-pickup-v1.wav` & `space-invaders-0.1.49/space-invaders/Sounds/678384__jocabundus__item-pickup-v1.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/background.png` & `space-invaders-0.1.49/space-invaders/Sprites/background.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/default_enemy_gun.png` & `space-invaders-0.1.49/space-invaders/Sprites/default_enemy_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/default_enemy_projectile.png` & `space-invaders-0.1.49/space-invaders/Sprites/default_enemy_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/default_enemy_ship.png` & `space-invaders-0.1.49/space-invaders/Sprites/default_enemy_ship.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/default_gun.png` & `space-invaders-0.1.49/space-invaders/Sprites/default_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/default_gun_pickup.png` & `space-invaders-0.1.49/space-invaders/Sprites/default_gun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/default_projectile.png` & `space-invaders-0.1.49/space-invaders/Sprites/default_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/default_ship.png` & `space-invaders-0.1.49/space-invaders/Sprites/default_ship.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/explosion.png` & `space-invaders-0.1.49/space-invaders/Sprites/explosion.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/fire_rate_booster.png` & `space-invaders-0.1.49/space-invaders/Sprites/fire_rate_booster.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/life.png` & `space-invaders-0.1.49/space-invaders/Sprites/life.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/medium_heal.png` & `space-invaders-0.1.49/space-invaders/Sprites/medium_heal.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/minigun.png` & `space-invaders-0.1.49/space-invaders/Sprites/minigun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/minigun_pickup.png` & `space-invaders-0.1.49/space-invaders/Sprites/minigun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/minigun_projectile.png` & `space-invaders-0.1.49/space-invaders/Sprites/minigun_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/repair.png` & `space-invaders-0.1.49/space-invaders/Sprites/repair.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/rocket_gun.png` & `space-invaders-0.1.49/space-invaders/Sprites/rocket_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/rocket_gun_pickup.png` & `space-invaders-0.1.49/space-invaders/Sprites/rocket_gun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/rocket_projectile.png` & `space-invaders-0.1.49/space-invaders/Sprites/rocket_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/ship_explosion.png` & `space-invaders-0.1.49/space-invaders/Sprites/ship_explosion.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/Sprites/small_heal.png` & `space-invaders-0.1.49/space-invaders/Sprites/small_heal.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/config.py` & `space-invaders-0.1.49/space-invaders/config.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/entity.py` & `space-invaders-0.1.49/space-invaders/entity.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/level.py` & `space-invaders-0.1.49/space-invaders/level.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/main.py` & `space-invaders-0.1.49/space-invaders/main.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/pickup.py` & `space-invaders-0.1.49/space-invaders/pickup.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space-invaders/spaceship.py` & `space-invaders-0.1.49/space-invaders/spaceship.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.48/space_invaders.egg-info/PKG-INFO` & `space-invaders-0.1.49/space_invaders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.48
+Version: 0.1.49
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.1.48/space_invaders.egg-info/SOURCES.txt` & `space-invaders-0.1.49/space_invaders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

