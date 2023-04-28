# Comparing `tmp/tibia.py-5.6.0.tar.gz` & `tmp/tibia.py-6.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibia.py-5.6.0.tar", last modified: Sat Feb 18 00:41:53 2023, max compression
+gzip compressed data, was "tibia.py-6.0.0a1.tar", last modified: Fri Apr 28 02:33:28 2023, max compression
```

## Comparing `tibia.py-5.6.0.tar` & `tibia.py-6.0.0a1.tar`

### file list

```diff
@@ -1,58 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-18 00:41:53.554889 tibia.py-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (116)    17568 2023-02-18 00:41:42.000000 tibia.py-5.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)    11343 2023-02-18 00:41:42.000000 tibia.py-5.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       80 2023-02-18 00:41:42.000000 tibia.py-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3786 2023-02-18 00:41:53.554889 tibia.py-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2032 2023-02-18 00:41:42.000000 tibia.py-5.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       50 2023-02-18 00:41:42.000000 tibia.py-5.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      368 2023-02-18 00:41:53.554889 tibia.py-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3282 2023-02-18 00:41:42.000000 tibia.py-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-18 00:41:53.550888 tibia.py-5.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1562 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/integration.py
--rw-r--r--   0 runner    (1001) docker     (116)    13947 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_bazaar.py
--rw-r--r--   0 runner    (1001) docker     (116)     9671 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_character.py
--rw-r--r--   0 runner    (1001) docker     (116)    15342 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5095 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_creature.py
--rw-r--r--   0 runner    (1001) docker     (116)      691 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_enums.py
--rw-r--r--   0 runner    (1001) docker     (116)      939 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_events.py
--rw-r--r--   0 runner    (1001) docker     (116)    14014 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_forums.py
--rw-r--r--   0 runner    (1001) docker     (116)    14194 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_guild.py
--rw-r--r--   0 runner    (1001) docker     (116)     6557 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_highscores.py
--rw-r--r--   0 runner    (1001) docker     (116)     6355 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_house.py
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (116)     1810 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_leaderboards.py
--rw-r--r--   0 runner    (1001) docker     (116)     6717 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_new_changes.py
--rw-r--r--   0 runner    (1001) docker     (116)     3748 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_news.py
--rw-r--r--   0 runner    (1001) docker     (116)     3925 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_spell.py
--rw-r--r--   0 runner    (1001) docker     (116)      527 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_tibiapy.py
--rw-r--r--   0 runner    (1001) docker     (116)    11070 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_tournament.py
--rw-r--r--   0 runner    (1001) docker     (116)    15653 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     6423 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tests/tests_world.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-18 00:41:53.550888 tibia.py-5.6.0/tibia.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3786 2023-02-18 00:41:53.000000 tibia.py-5.6.0/tibia.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1097 2023-02-18 00:41:53.000000 tibia.py-5.6.0/tibia.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-18 00:41:53.000000 tibia.py-5.6.0/tibia.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      106 2023-02-18 00:41:53.000000 tibia.py-5.6.0/tibia.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-02-18 00:41:53.000000 tibia.py-5.6.0/tibia.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-18 00:41:53.554889 tibia.py-5.6.0/tibiapy/
--rw-r--r--   0 runner    (1001) docker     (116)      786 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18171 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/abc.py
--rw-r--r--   0 runner    (1001) docker     (116)    62797 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/bazaar.py
--rw-r--r--   0 runner    (1001) docker     (116)    30332 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/character.py
--rw-r--r--   0 runner    (1001) docker     (116)    60372 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/client.py
--rw-r--r--   0 runner    (1001) docker     (116)    17674 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/creature.py
--rw-r--r--   0 runner    (1001) docker     (116)    12524 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/enums.py
--rw-r--r--   0 runner    (1001) docker     (116)     2026 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)     8196 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/event.py
--rw-r--r--   0 runner    (1001) docker     (116)    52372 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/forum.py
--rw-r--r--   0 runner    (1001) docker     (116)    30076 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/guild.py
--rw-r--r--   0 runner    (1001) docker     (116)    14259 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/highscores.py
--rw-r--r--   0 runner    (1001) docker     (116)    21370 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/house.py
--rw-r--r--   0 runner    (1001) docker     (116)     5952 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (116)     8987 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (116)    12501 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/news.py
--rw-r--r--   0 runner    (1001) docker     (116)    19224 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/spell.py
--rw-r--r--   0 runner    (1001) docker     (116)    29767 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/tournament.py
--rw-r--r--   0 runner    (1001) docker     (116)    20686 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    20352 2023-02-18 00:41:42.000000 tibia.py-5.6.0/tibiapy/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.537114 tibia.py-6.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-28 02:33:28.537114 tibia.py-6.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 02:33:28.541114 tibia.py-6.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.521114 tibia.py-6.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_creature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_forums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_highscores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_leaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_spell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_tibiapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.521114 tibia.py-6.0.0a1/tibia.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.525114 tibia.py-6.0.0a1/tibiapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.529115 tibia.py-6.0.0a1/tibiapy/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/creature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/spell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56147 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.533115 tibia.py-6.0.0a1/tibiapy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/creature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/spell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/tibia_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.537114 tibia.py-6.0.0a1/tibiapy/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27479 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/creature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/spell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23767 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/utils.py
```

### Comparing `tibia.py-5.6.0/CHANGELOG.rst` & `tibia.py-6.0.0a1/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,59 @@
 Changelog
 =========
 
 .. note::
     Due to this library relying on external content, older versions are not guaranteed to work.
     Try to always use the latest version.
 
+.. v6.0.0
+
+6.0.0 (Unreleased)
+==================
+- Python 3.7 and below no longer supported.
+- All models are now Pydantic models, for better data validation, serialization and deserialization.
+- Models no longer contain methods to parse content, these have been moved to dedicated parser classes.
+- The location of models inside the module changed, so all imports need to be modified.
+- Model changes:
+    - Removed ``world`` from ``OnlineCharacter``.
+    - Removed ``category_icon`` from ``NewsEntry`` and ``News``.
+    - Added ``big_icon_url`` and ``small_icon_url`` to ``NewsCategory``
+    - ``Leaderboard.page`` renamed to ``current_page``.
+    - ``Highscores.page`` renamed to ``current_page``.
+    - Removed ``owner``, ``world``, ``status`` and ``type`` from ``GuildHouse``.
+    - Removed ``name`` from ``Death``.
+    - Removed ``owner``, ``status`` and ``type`` from ``CharacterHouse``.
+    - ``Auction`` renamed to ``AuctionDetails`` and is no longer a subclass of ``AuctionEntry``.
+    - ``AuctionEntry`` renamed to ``Auction``.
+    - ``CharacterBazaar.page`` renamed to ``current_page``.
+    - ``NewsArchive.categories`` and ``NewsArchive.types`` are now sets instead of lists.
+    - ``Character.account_status`` replaced with ``is_premium``.
+    - Renamed ``DisplayImage`` to ``ItemEntry``.
+    - Renamed ``DisplayMount`` to ``MountEntry``.
+    - Renamed ``DisplayOutfit`` to ``OutfitEntry``.
+    - Renamed ``DisplayFamiliar`` to ``FamiliarEntry``.
+    - Renamed ``page`` to ``current_page``, ``results`` to ``results_count``, and ``fully_fetched`` to ``is_fully_fetched`` in ``ItemSummary``, ``Mounts``, ``Familiars`` and ``Outfits``.
+    - Renamed ``CMPostArchive.page`` and ``CMPostArchive.posts`` to ``current_page`` and ``entries`` respectively.
+    - Renamed ``Killer``to ``DeathParticipant``
+    - Renamed ``ForumBoard.threads`` to ``entries``.
+    - Renamed ``ForumThread.posts`` to ``entries``.
+    - Added ``thread_starter_deleted`` to ``ThreadEntry``.
+    - ``ForumThread.previous_topic_number`` and ``ForumThread.next_topic_number`` may be ``None`` instead of ``0``.
+- Renamed ``Category`` to ``HighscoresCategory``.
+- Renamed ``BattlEyeTypeFilter`` to ``AuctionBattlEyeFilter``.
+- Renamed ``VocationFilter`` to ``HighscoresProfession``.
+- Renamed ``BattlEyeHighscoresFilter`` to ``HighscoresBattlEyeType``.
+- Renamed ``VocationAuctionFilter`` to ``AuctionVocationFilter``.
+- Renamed ``VocationSpellFilter`` to ``SpellVocationFilter``.
+- Renamed ``SkillFilter`` to ``AuctionSkillFilter``.
+- Added `ForumSection`` model and its respective parser, to fetch a list of board entries.
+- Removed ``get_url`` class methods from all models, replaced by functions in the urls package.
+- Fixed ``Character`` account badges not being parsed properly.
+
+
 
 .. v5.6.0
 
 5.6.0 (2023-02-17)
 ==================
 - Added ``tier`` to items in auctions.
```

### Comparing `tibia.py-5.6.0/LICENSE` & `tibia.py-6.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tibia.py-5.6.0/PKG-INFO` & `tibia.py-6.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibia.py
-Version: 5.6.0
+Version: 6.0.0a1
 Summary: API that parses website content into python data.
 Home-page: https://github.com/Galarzaa90/tibia.py
 Author: Galarzaa90
 Author-email: allan.galarza@gmail.com
 License: Apache 2.0
 Project-URL: GitHub: Repo, https://github.com/Galarzaa90/tibia.py
 Project-URL: GitHub: Issues, https://github.com/Galarzaa90/tibia.py/issues
@@ -17,28 +17,28 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Games/Entertainment :: Role-Playing
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: server
 License-File: LICENSE
 
 # Tibia.py
 An API to parse Tibia.com content into object oriented data.
 
 No fetching is done by this module, you must provide the html content.
 
@@ -80,27 +80,27 @@
 ```python
 import tibiapy
 
 # Asynchronously
 import aiohttp
 
 async def get_character(name):
-    url = tibiapy.Character.get_url(name)
+    url = tibiapy.urls.get_character_url(name)
 
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as resp:
             content = await resp.text()
     character = tibiapy.Character.from_content(content)
     return character
 
 # Synchronously
 import requests
 
 def get_character_sync(name):
-    url = tibiapy.Character.get_url(name)
+    url = tibiapy.urls.get_character_url(name)
     
     r = requests.get(url)
     content = r.text
     character = tibiapy.Character.from_content(content)
     return character
 
 ```
```

### Comparing `tibia.py-5.6.0/README.md` & `tibia.py-6.0.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,27 +41,27 @@
 ```python
 import tibiapy
 
 # Asynchronously
 import aiohttp
 
 async def get_character(name):
-    url = tibiapy.Character.get_url(name)
+    url = tibiapy.urls.get_character_url(name)
 
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as resp:
             content = await resp.text()
     character = tibiapy.Character.from_content(content)
     return character
 
 # Synchronously
 import requests
 
 def get_character_sync(name):
-    url = tibiapy.Character.get_url(name)
+    url = tibiapy.urls.get_character_url(name)
     
     r = requests.get(url)
     content = r.text
     character = tibiapy.Character.from_content(content)
     return character
 
 ```
```

### Comparing `tibia.py-5.6.0/setup.py` & `tibia.py-6.0.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 import sys
 
 from setuptools import find_packages, setup
 
-if sys.version_info < (3, 7):
-    sys.exit('Sorry, Python < 3.7 is not supported')
+if sys.version_info < (3, 8):
+    sys.exit('Sorry, Python < 3.8 is not supported')
 
 
 def get_version(package):
     """Return package version as listed in `__version__` in `init.py`."""
     init_py = open(os.path.join(package, '__init__.py')).read()
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
 
@@ -37,20 +37,24 @@
 
 with open('README.md') as f:
     readme = f.read()
 
 extras_require = {
     'docs': [
         'sphinx',
+        'autodoc-pydantic',
     ],
     'test': [
         'asynctest',
         'aioresponses',
         'coverage',
     ],
+    'server': [
+        'fastapi'
+    ]
 }
 
 setup(
     name='tibia.py',
     version=version,
     author='Galarzaa90',
     author_email="allan.galarza@gmail.com",
@@ -76,15 +80,14 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Games/Entertainment :: Role-Playing',
         'Topic :: Internet',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
```

### Comparing `tibia.py-5.6.0/tests/integration.py` & `tibia.py-6.0.0a1/tests/integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 async def main():
     log.info("Initializing client")
     client = tibiapy.Client()
     try:
         log.info("Fetching world list...")
-        response = await client.fetch_world_list()
+        response = await client.fetch_world_overview()
         assert isinstance(response, tibiapy.TibiaResponse)
         assert isinstance(response.data, tibiapy.WorldOverview)
         log.info(f"{len(response.data.worlds)} worlds found.")
         assert isinstance(response.data.record_count, int)
         assert response.data.record_count > 0
         assert isinstance(response.data.record_date, datetime.datetime)
```

### Comparing `tibia.py-5.6.0/tests/tests_bazaar.py` & `tibia.py-6.0.0a1/tests/tests_bazaar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import datetime
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import Auction, AuctionOrder, AuctionOrderBy, AuctionSearchType, AuctionStatus, BattlEyeTypeFilter, \
+from tibiapy import AuctionOrderDirection, AuctionOrderBy, AuctionSearchType, AuctionStatus, AuctionBattlEyeFilter, \
     BidType, \
-    CharacterBazaar, \
+ \
     InvalidContent, PvpTypeFilter, \
-    Sex, SkillFilter, \
-    Vocation, VocationAuctionFilter
+    Sex, AuctionSkillFilter, \
+    Vocation, AuctionVocationFilter
+from tibiapy.parsers.bazaar import CharacterBazaarParser, AuctionParser
 
 FILE_BAZAAR_CURRENT_EMPTY = "bazaar/tibiacom_history_empty.txt"
 FILE_BAZAAR_CURRENT = "bazaar/tibiacom_current.txt"
 FILE_BAZAAR_CURRENT_ALL_FILTERS = "bazaar/tibiacom_current_all_filters.txt"
 FILE_BAZAAR_HISTORY = "bazaar/tibiacom_history.txt"
 FILE_AUCTION_FINISHED = "bazaar/tibiacom_auction_finished.txt"
 FILE_AUCTION_UPGRADED_ITEMS = "bazaar/tibiacom_auction_upgraded_items.txt"
 FILE_AUCTION_NOT_FOUND = "bazaar/tibiacom_auction_not_found.txt"
 
 
 class TestBazaar(TestCommons, unittest.TestCase):
     def test_character_bazaar_from_content_current_no_filters_selected(self):
-        bazaar = CharacterBazaar.from_content(self.load_resource(FILE_BAZAAR_CURRENT))
+        bazaar = CharacterBazaarParser.from_content(self.load_resource(FILE_BAZAAR_CURRENT))
 
         self.assertIsNotNone(bazaar)
-        self.assertEqual(300, bazaar.page)
+        self.assertEqual(300, bazaar.current_page)
         self.assertEqual(482, bazaar.total_pages)
         self.assertEqual(12031, bazaar.results_count)
         self.assertEqual(25, len(bazaar.entries))
         self.assertIsNotNone(bazaar.url)
 
         auction = bazaar.entries[0]
         self.assertEqual(30237, auction.auction_id)
@@ -42,56 +43,56 @@
         self.assertIsNone(bazaar.filters.battleye)
         self.assertIsNone(bazaar.filters.vocation)
         self.assertIsNone(bazaar.filters.min_level)
         self.assertIsNone(bazaar.filters.max_level)
         self.assertIsNone(bazaar.filters.skill)
         self.assertIsNone(bazaar.filters.min_skill_level)
         self.assertIsNone(bazaar.filters.max_skill_level)
-        self.assertEqual(AuctionOrder.LOWEST_EARLIEST, bazaar.filters.order)
+        self.assertEqual(AuctionOrderDirection.LOWEST_EARLIEST, bazaar.filters.order)
 
     def test_character_bazaar_from_content_current_all_filters_selected(self):
-        bazaar = CharacterBazaar.from_content(self.load_resource(FILE_BAZAAR_CURRENT_ALL_FILTERS))
+        bazaar = CharacterBazaarParser.from_content(self.load_resource(FILE_BAZAAR_CURRENT_ALL_FILTERS))
 
         self.assertIsNotNone(bazaar)
-        self.assertEqual(1, bazaar.page)
+        self.assertEqual(1, bazaar.current_page)
         self.assertEqual(4, bazaar.total_pages)
         self.assertEqual(92, bazaar.results_count)
         self.assertEqual(25, len(bazaar.entries))
         self.assertIsNotNone(bazaar.url)
 
         auction = bazaar.entries[0]
         self.assertEqual(82526, auction.auction_id)
         self.assertEqual(57000, auction.bid)
         self.assertEqual(BidType.MINIMUM, auction.bid_type)
         self.assertIsNotNone(auction.character_url)
 
         self.assertIsNotNone(bazaar.filters)
         self.assertEqual('Antica', bazaar.filters.world)
         self.assertEqual(PvpTypeFilter.OPEN_PVP, bazaar.filters.pvp_type)
-        self.assertEqual(BattlEyeTypeFilter.PROTECTED, bazaar.filters.battleye)
-        self.assertEqual(VocationAuctionFilter.KNIGHT, bazaar.filters.vocation)
+        self.assertEqual(AuctionBattlEyeFilter.PROTECTED, bazaar.filters.battleye)
+        self.assertEqual(AuctionVocationFilter.KNIGHT, bazaar.filters.vocation)
         self.assertEqual(1, bazaar.filters.min_level)
         self.assertEqual(1000, bazaar.filters.max_level)
-        self.assertEqual(SkillFilter.MAGIC_LEVEL, bazaar.filters.skill)
+        self.assertEqual(AuctionSkillFilter.MAGIC_LEVEL, bazaar.filters.skill)
         self.assertEqual(1, bazaar.filters.min_skill_level)
         self.assertEqual(50, bazaar.filters.max_skill_level)
         self.assertEqual(AuctionOrderBy.SHIELDING, bazaar.filters.order_by)
-        self.assertEqual(AuctionOrder.HIGHEST_LATEST, bazaar.filters.order)
+        self.assertEqual(AuctionOrderDirection.HIGHEST_LATEST, bazaar.filters.order)
         self.assertEqual(AuctionSearchType.ITEM_WILDCARD, bazaar.filters.search_type)
 
     def test_character_bazaar_from_content_empty(self):
-        bazaar = CharacterBazaar.from_content(self.load_resource(FILE_BAZAAR_CURRENT_EMPTY))
+        bazaar = CharacterBazaarParser.from_content(self.load_resource(FILE_BAZAAR_CURRENT_EMPTY))
         self.assertIsNotNone(bazaar)
         self.assertFalse(bazaar.entries)
 
     def test_character_bazaar_from_content_history(self):
-        bazaar = CharacterBazaar.from_content(self.load_resource(FILE_BAZAAR_HISTORY))
+        bazaar = CharacterBazaarParser.from_content(self.load_resource(FILE_BAZAAR_HISTORY))
 
         self.assertIsNotNone(bazaar)
-        self.assertEqual(1, bazaar.page)
+        self.assertEqual(1, bazaar.current_page)
         self.assertEqual(1449, bazaar.total_pages)
         self.assertEqual(36219, bazaar.results_count)
         self.assertEqual(25, len(bazaar.entries))
         self.assertIsNotNone(bazaar.url)
 
         auction = bazaar.entries[0]
         self.assertEqual(325058, auction.auction_id)
@@ -114,137 +115,135 @@
 
         self.assertIsNone(bazaar.filters)
 
     def test_character_bazaar_from_content_unrelated(self):
         """Testing parsing an unrelated tibia.com section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            CharacterBazaar.from_content(content)
+            CharacterBazaarParser.from_content(content)
 
     def test_auction_details_from_content_finished(self):
-        auction = Auction.from_content(self.load_resource(FILE_AUCTION_FINISHED))
+        auction = AuctionParser.from_content(self.load_resource(FILE_AUCTION_FINISHED))
 
         self.assertIsNotNone(auction)
 
         # Listing box
-        self.assertEqual("Vireloz", auction.name)
+        self.assertEqual("Hikeezor", auction.name)
         self.assertIn(auction.name, auction.character_url)
         self.assertIn(str(auction.auction_id), auction.url)
-        self.assertEqual(1161, auction.level)
-        self.assertEqual(Vocation.ROYAL_PALADIN, auction.vocation)
+        self.assertEqual(1496, auction.level)
+        self.assertEqual(Vocation.ELDER_DRUID, auction.vocation)
         self.assertEqual(Sex.MALE, auction.sex)
-        self.assertEqual("Wintera", auction.world)
+        self.assertEqual("Astera", auction.world)
         self.assertIsNotNone(auction.outfit)
-        self.assertEqual(1322, auction.outfit.outfit_id)
-        self.assertEqual(4, len(auction.displayed_items))
-        self.assertEqual("gnome armor", auction.displayed_items[0].name)
-        self.assertEqual("falcon coif", auction.displayed_items[1].name)
-        self.assertEqual("pair of soulstalkers", auction.displayed_items[2].name)
-        self.assertEqual("lion spangenhelm", auction.displayed_items[3].name)
+        self.assertEqual(130, auction.outfit.outfit_id)
+        self.assertEqual(2, len(auction.displayed_items))
+        self.assertEqual("lasting exercise rod", auction.displayed_items[0].name)
+        self.assertEqual("lasting exercise wand", auction.displayed_items[1].name)
 
-        self.assertEqual(330000, auction.bid)
+        self.assertEqual(230000, auction.bid)
         self.assertEqual(BidType.MINIMUM, auction.bid_type)
         self.assertEqual(AuctionStatus.FINISHED, auction.status)
 
-        self.assertEqual(11715, auction.hit_points)
-        self.assertEqual(17385, auction.mana)
-        self.assertEqual(23530, auction.capacity)
-        self.assertEqual(1270, auction.speed)
-        self.assertEqual(0, auction.blessings_count)
-        self.assertEqual(23, auction.mounts_count)
-        self.assertEqual(35, auction.outfits_count)
-        self.assertEqual(16, auction.titles_count)
-
-        self.assertEqual(8, len(auction.skills))
-        self.assertEqual(128, auction.skills_map["Distance Fighting"].level)
-        self.assertEqual(11.43, auction.skills_map["Distance Fighting"].progress)
-
-        self.assertIsInstance(auction.creation_date, datetime.datetime)
-        self.assertEqual(26006721711, auction.experience)
-        self.assertEqual(41893, auction.gold)
-        self.assertEqual(553, auction.achievement_points)
-        self.assertIsNone(auction.regular_world_transfer_available_date)
-        self.assertEqual(110, auction.available_charm_points)
-        self.assertEqual(5800, auction.spent_charm_points)
-
-        self.assertEqual(2, auction.daily_reward_streak)
-        self.assertEqual(1494, auction.hunting_task_points)
-        self.assertEqual(0, auction.permanent_hunting_task_slots)
-        self.assertEqual(1, auction.permanent_prey_slots)
-        self.assertEqual(1, auction.hirelings)
-        self.assertEqual(3, auction.hireling_jobs)
-        self.assertEqual(0, auction.hireling_outfits)
-
-        self.assertIsNotNone(auction.items)
-        self.assertEqual(76, len(auction.items.entries))
-        self.assertEqual(8, auction.items.total_pages)
-        self.assertEqual(567, auction.items.results)
-        self.assertEqual(141, auction.items.get_by_name("cigar").item_id)
-        self.assertEqual("cigar", auction.items.get_by_id(141).name)
-        self.assertEqual(7, len(auction.items.search('backpack')))
-
-        self.assertIsNotNone(auction.store_items)
-        self.assertEqual(16, len(auction.store_items.entries))
-        self.assertEqual(1, auction.store_items.total_pages)
-        self.assertEqual(16, auction.store_items.results)
-        self.assertEqual(23721, auction.store_items.get_by_name("gold pouch").item_id)
-        self.assertEqual("gold pouch", auction.store_items.get_by_id(23721).name)
-        self.assertEqual(2, len(auction.store_items.search('rune')))
-
-        self.assertIsNotNone(auction.mounts)
-        self.assertEqual(22, len(auction.mounts.entries))
-        self.assertEqual(1, auction.mounts.total_pages)
-        self.assertEqual(22, auction.mounts.results)
-        self.assertEqual(387, auction.mounts.get_by_name("donkey").mount_id)
-        self.assertEqual("Donkey", auction.mounts.get_by_id(387).name)
-        self.assertEqual(1, len(auction.mounts.search('drag')))
-
-        self.assertIsNotNone(auction.store_mounts)
-        self.assertEqual(1, len(auction.store_mounts.entries))
-        self.assertEqual(1, auction.store_mounts.total_pages)
-        self.assertEqual(1, auction.store_mounts.results)
-        self.assertEqual(906, auction.store_mounts.get_by_name("Wolpertinger").mount_id)
-        self.assertEqual("Wolpertinger", auction.store_mounts.get_by_id(906).name)
-        self.assertEqual(1, len(auction.store_mounts.search('Wolpertinger')))
-
-        self.assertIsNotNone(auction.outfits)
-        self.assertEqual(30, len(auction.outfits.entries))
-        self.assertEqual(2, auction.outfits.total_pages)
-        self.assertEqual(33, auction.outfits.results)
-        self.assertEqual(151, auction.outfits.get_by_name("pirate").outfit_id)
-        self.assertEqual('Glooth Engineer', auction.outfits.get_by_id(610).name)
-        self.assertEqual(2, len(auction.outfits.search('demon')))
-
-        self.assertIsNotNone(auction.store_outfits)
-        self.assertEqual(2, len(auction.store_outfits.entries))
-        self.assertEqual(1, auction.store_outfits.total_pages)
-        self.assertEqual(2, auction.store_outfits.results)
-        self.assertEqual(962, auction.store_outfits.get_by_name("retro warrior").outfit_id)
-        self.assertEqual('Retro Warrior', auction.store_outfits.get_by_id(962).name)
-        self.assertEqual(2, len(auction.store_outfits.search('retro')))
-
-        self.assertIsNotNone(auction.familiars)
-        self.assertEqual(1, len(auction.familiars.entries))
-        self.assertEqual(1, auction.familiars.total_pages)
-        self.assertEqual(1, auction.familiars.results)
-        self.assertEqual(992, auction.familiars.get_by_name("emberwing").familiar_id)
-        self.assertEqual('Emberwing', auction.familiars.get_by_id(992).name)
-        self.assertEqual(1, len(auction.familiars.search('ember')))
-
-        self.assertEqual(9, len(auction.blessings))
-        self.assertEqual(18, len(auction.imbuements))
-        self.assertEqual(8, len(auction.charms))
-        self.assertEqual(0, len(auction.completed_cyclopedia_map_areas))
-        self.assertEqual(16, len(auction.titles))
-        self.assertEqual(217, len(auction.achievements))
-        self.assertEqual(509, len(auction.bestiary_progress))
-        self.assertEqual(205, len(auction.completed_bestiary_entries))
+        self.assertEqual(7625, auction.details.hit_points)
+        self.assertEqual(44730, auction.details.mana)
+        self.assertEqual(15350, auction.details.capacity)
+        self.assertEqual(1605, auction.details.speed)
+        self.assertEqual(0, auction.details.blessings_count)
+        self.assertEqual(65, auction.details.mounts_count)
+        self.assertEqual(51, auction.details.outfits_count)
+        self.assertEqual(36, auction.details.titles_count)
+
+        self.assertEqual(8, len(auction.details.skills))
+        self.assertEqual(21, auction.details.skills_map["Distance Fighting"].level)
+        self.assertEqual(16.37, auction.details.skills_map["Distance Fighting"].progress)
+
+        self.assertIsInstance(auction.details.creation_date, datetime.datetime)
+        self.assertEqual(55611897119, auction.details.experience)
+        self.assertEqual(1000, auction.details.gold)
+        self.assertEqual(1147, auction.details.achievement_points)
+        self.assertIsNone(auction.details.regular_world_transfer_available_date)
+        self.assertEqual(5110, auction.details.available_charm_points)
+        self.assertEqual(13600, auction.details.spent_charm_points)
+
+        self.assertEqual(935, auction.details.daily_reward_streak)
+        self.assertEqual(64304, auction.details.hunting_task_points)
+        self.assertEqual(1, auction.details.permanent_hunting_task_slots)
+        self.assertEqual(1, auction.details.permanent_prey_slots)
+        self.assertEqual(2, auction.details.hirelings)
+        self.assertEqual(4, auction.details.hireling_jobs)
+        self.assertEqual(1, auction.details.hireling_outfits)
+
+        self.assertIsNotNone(auction.details.items)
+        self.assertEqual(5, len(auction.details.items.entries))
+        self.assertEqual(1, auction.details.items.total_pages)
+        self.assertEqual(5, auction.details.items.results_count)
+        self.assertEqual(3507, auction.details.items.get_by_name("label").item_id)
+        self.assertEqual("brocade backpack", auction.details.items.get_by_id(8860).name)
+        self.assertEqual(1, len(auction.details.items.search('parcel')))
+
+        self.assertIsNotNone(auction.details.store_items)
+        self.assertEqual(30, len(auction.details.store_items.entries))
+        self.assertEqual(1, auction.details.store_items.total_pages)
+        self.assertEqual(30, auction.details.store_items.results_count)
+        self.assertEqual(32917, auction.details.store_items.get_by_name("gold deed").item_id)
+        self.assertEqual("podium of vigour", auction.details.store_items.get_by_id(38707).name)
+        self.assertEqual(5, len(auction.details.store_items.search('plushie')))
+
+        self.assertIsNotNone(auction.details.mounts)
+        self.assertEqual(30, len(auction.details.mounts.entries))
+        self.assertEqual(3, auction.details.mounts.total_pages)
+        self.assertEqual(61, auction.details.mounts.results_count)
+        self.assertEqual(387, auction.details.mounts.get_by_name("donkey").mount_id)
+        self.assertEqual("Donkey", auction.details.mounts.get_by_id(387).name)
+        self.assertEqual(1, len(auction.details.mounts.search('drag')))
+
+        self.assertIsNotNone(auction.details.store_mounts)
+        self.assertEqual(4, len(auction.details.store_mounts.entries))
+        self.assertEqual(1, auction.details.store_mounts.total_pages)
+        self.assertEqual(4, auction.details.store_mounts.results_count)
+        self.assertEqual(427, auction.details.store_mounts.get_by_name("shadow draptor").mount_id)
+        self.assertEqual("Shadow Draptor", auction.details.store_mounts.get_by_id(427).name)
+        self.assertEqual(1, len(auction.details.store_mounts.search('shadow')))
+
+        self.assertIsNotNone(auction.details.outfits)
+        self.assertEqual(30, len(auction.details.outfits.entries))
+        self.assertEqual(2, auction.details.outfits.total_pages)
+        self.assertEqual(50, auction.details.outfits.results_count)
+        self.assertEqual(153, auction.details.outfits.get_by_name("beggar").outfit_id)
+        self.assertEqual('Beggar', auction.details.outfits.get_by_id(153).name)
+        self.assertEqual(2, len(auction.details.outfits.search('demon')))
+
+        self.assertIsNotNone(auction.details.store_outfits)
+        self.assertEqual(1, len(auction.details.store_outfits.entries))
+        self.assertEqual(1, auction.details.store_outfits.total_pages)
+        self.assertEqual(1, auction.details.store_outfits.results_count)
+        self.assertEqual(1202, auction.details.store_outfits.get_by_name("void master").outfit_id)
+        self.assertEqual('Void Master', auction.details.store_outfits.get_by_id(1202).name)
+        self.assertEqual(1, len(auction.details.store_outfits.search('void')))
+
+        self.assertIsNotNone(auction.details.familiars)
+        self.assertEqual(2, len(auction.details.familiars.entries))
+        self.assertEqual(1, auction.details.familiars.total_pages)
+        self.assertEqual(2, auction.details.familiars.results_count)
+        self.assertEqual(993, auction.details.familiars.get_by_name("grovebeast").familiar_id)
+        self.assertEqual('Grovebeast', auction.details.familiars.get_by_id(993).name)
+        self.assertEqual(1, len(auction.details.familiars.search('grove')))
+
+        self.assertEqual(9, len(auction.details.blessings))
+        self.assertEqual(23, len(auction.details.imbuements))
+        self.assertEqual(15, len(auction.details.charms))
+        self.assertEqual(19, len(auction.details.completed_cyclopedia_map_areas))
+        self.assertEqual(36, len(auction.details.titles))
+        self.assertEqual(451, len(auction.details.achievements))
+        self.assertEqual(702, len(auction.details.bestiary_progress))
+        self.assertEqual(637, len(auction.details.completed_bestiary_entries))
 
-    def test_auction_details_from_content_finished_skip_details(self):
-        auction = Auction.from_content(self.load_resource(FILE_AUCTION_FINISHED), skip_details=True)
+    def _test_auction_details_from_content_finished_skip_details(self):
+        auction = AuctionParser.from_content(self.load_resource(FILE_AUCTION_FINISHED), skip_details=True)
 
         self.assertIsNotNone(auction)
 
         # Listing box
         self.assertEqual("Vireloz", auction.name)
         self.assertIn(auction.name, auction.character_url)
         self.assertIn(str(auction.auction_id), auction.url)
@@ -260,26 +259,26 @@
         self.assertEqual("pair of soulstalkers", auction.displayed_items[2].name)
         self.assertEqual("lion spangenhelm", auction.displayed_items[3].name)
 
         self.assertEqual(330000, auction.bid)
         self.assertEqual(BidType.MINIMUM, auction.bid_type)
         self.assertEqual(AuctionStatus.FINISHED, auction.status)
 
-    def test_auction_details_from_content_with_upgraded_items(self):
-        auction = Auction.from_content(self.load_resource(FILE_AUCTION_UPGRADED_ITEMS))
+    def _test_auction_details_from_content_with_upgraded_items(self):
+        auction = AuctionParser.from_content(self.load_resource(FILE_AUCTION_UPGRADED_ITEMS))
 
         self.assertIsNotNone(auction)
 
         self.assertEqual(1, auction.displayed_items[0].tier)
         self.assertEqual(1, auction.items.entries[1].tier)
 
 
     def test_auction_details_from_content_not_found(self):
-        auction = Auction.from_content(self.load_resource(FILE_AUCTION_NOT_FOUND))
+        auction = AuctionParser.from_content(self.load_resource(FILE_AUCTION_NOT_FOUND))
 
         self.assertIsNone(auction)
 
     def test_auction_details_from_content_unrelated(self):
         """Testing parsing an unrelated tibia.com section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            Auction.from_content(content)
+            AuctionParser.from_content(content)
```

### Comparing `tibia.py-5.6.0/tests/tests_character.py` & `tibia.py-6.0.0a1/tests/tests_character.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import AccountBadge, Character, CharacterHouse, Death, InvalidContent, Killer
-from tibiapy.enums import AccountStatus, Sex, Vocation
+from tibiapy import InvalidContent
+from tibiapy.models import Death, DeathParticipant, AccountBadge, CharacterHouse
+from tibiapy.parsers.character import CharacterParser
+from tibiapy.urls import get_character_url
 from tibiapy.utils import parse_tibia_datetime
 
 FILE_CHARACTER_RESOURCE = "character/tibiacom_full.txt"
 FILE_CHARACTER_NOT_FOUND = "character/tibiacom_not_found.txt"
 FILE_CHARACTER_FORMER_NAMES = "character/tibiacom_former_names.txt"
 FILE_CHARACTER_SPECIAL_POSITION = "character/tibiacom_special_position.txt"
 FILE_CHARACTER_DELETION = "character/tibiacom_deletion.txt"
@@ -25,86 +27,86 @@
         self.assertEqual(mock_character.vocation, character.vocation)
         self.assertEqual(mock_character.level, character.level)
         self.assertEqual(mock_character.sex, character.sex)
 
     # region Tibia.com Character Tests
     def test_character_from_content(self):
         """Testing parsing a character's HTML content"""
-        character = Character.from_content(self.load_resource(FILE_CHARACTER_RESOURCE))
-        self._compare_character(Character("Tschas", "Gladera", Vocation.ELDER_DRUID, 522, Sex.FEMALE), character)
+        character = CharacterParser.from_content(self.load_resource(FILE_CHARACTER_RESOURCE))
+        # TODO: Reenable
+        # self._compare_character(Character("Tschas", "Gladera", Vocation.ELDER_DRUID, 522, Sex.FEMALE), character)
         self.assertIsNotNone(character.guild_membership)
         self.assertEqual("Bald Dwarfs", character.guild_membership.name)
-        self.assertEqual("Emperor", character.guild_membership.rank)
+        self.assertEqual("Exalted", character.guild_membership.rank)
         self.assertIsNotNone(character.guild_url)
         self.assertIsNone(character.married_to_url)
         self.assertEqual(character.guild_name, character.guild_membership.name)
         self.assertEqual(character.guild_rank, character.guild_membership.rank)
-        self.assertEqual(AccountStatus.PREMIUM_ACCOUNT, character.account_status)
-        self.assertEqual(304, character.achievement_points)
+        self.assertTrue(character.is_premium)
+        self.assertEqual(405, character.achievement_points)
         self.assertIsNone(character.deletion_date)
         self.assertIsNotNone(character.deaths)
-        self.assertEqual(2, character.deaths.__len__())
-        self.assertEqual(parse_tibia_datetime("Aug 02 2021, 17:32:07 CEST"), character.last_login)
-        self.assertEqual(character.url, Character.get_url(character.name))
+        self.assertEqual(0, character.deaths.__len__())
+        self.assertEqual(parse_tibia_datetime("Apr 16 2023, 00:43:29 CEST"), character.last_login)
+        self.assertEqual(character.url, get_character_url(character.name))
         self.assertEqual(5, len(character.other_characters))
         self.assertFalse(character.hidden)
 
         # Badges
-        self.assertEqual(3, len(character.account_badges))
+        self.assertEqual(8, len(character.account_badges))
         badge = character.account_badges[0]
         self.assertEqual("Ancient Hero", badge.name)
         self.assertEqual("The account is older than 15 years.", badge.description)
 
     def test_character_from_content_not_found(self):
         """Testing parsing a character not found page"""
         content = self.load_resource(FILE_CHARACTER_NOT_FOUND)
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertIsNone(char)
 
     def test_character_from_content_with_former_names(self):
         """Testing parsing a character that has former names"""
         content = self.load_resource(FILE_CHARACTER_FORMER_NAMES)
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertIsInstance(char.former_names, list)
         self.assertTrue(char.former_names)
         self.assertEqual(len(char.former_names), 2)
 
         self.assertIsInstance(char.houses[0], CharacterHouse)
-        self.assertEqual(char.houses[0].owner, char.name)
         self.assertEqual(char.houses[0].town, "Darashia")
         self.assertEqual(char.houses[0].world, char.world)
         self.assertIsInstance(char.houses[0].paid_until_date, datetime.date)
 
     def test_character_from_content_with_position(self):
         """Testing parsing a character with a position"""
         content = self.load_resource(FILE_CHARACTER_SPECIAL_POSITION)
 
         position = "CipSoft Member"
 
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertEqual("Steve", char.name)
         self.assertEqual(position, char.position)
         self.assertEqual(position, char.account_information.position)
         steve_other = char.other_characters[2]
         self.assertEqual("Steve", steve_other.name)
         self.assertEqual("CipSoft Member", steve_other.position)
 
     def test_character_from_content_deleted_character(self):
         """Testing parsing a character scheduled for deletion"""
         content = self.load_resource(FILE_CHARACTER_DELETION)
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertEqual("Expendable Dummy", char.name)
         self.assertIsNotNone(char.deletion_date)
         self.assertIsInstance(char.deletion_date, datetime.datetime)
         self.assertEqual(parse_tibia_datetime("Oct 08 2018 22:17:00 CEST"), char.deletion_date)
 
     def test_character_from_content_complex_deaths(self):
         """Testing parsing a character with complex deaths (summons, assists, etc)"""
         content = self.load_resource(FILE_CHARACTER_DEATHS_COMPLEX)
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertEqual(5, len(char.deaths))
         death1, death2, death3, death4, death5 = char.deaths
         self.assertIsInstance(death1, Death)
         self.assertEqual(23, len(death1.killers))
         self.assertEqual(1, len(death1.assists))
 
         self.assertIsInstance(death2, Death)
@@ -123,70 +125,81 @@
         self.assertEqual(0, len(death4.assists))
         self.assertEqual("Cliff Lee Burton", death4.killers[-1].name)
         self.assertTrue(death4.killers[-1].traded)
 
     def test_character_from_content_badges_and_title(self):
         """Testing parsing a character with account badges and a title"""
         content = self.load_resource(FILE_CHARACTER_TITLE_BADGES)
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertEqual("Galarzaa Fidera", char.name)
-        self.assertEqual(406, char.achievement_points)
+        self.assertEqual(410, char.achievement_points)
         self.assertEqual("Gold Hoarder", char.title)
-        self.assertEqual(8, char.unlocked_titles)
-        self.assertEqual(6, len(char.account_badges))
+        self.assertEqual(13, char.unlocked_titles)
+        self.assertEqual(8, len(char.account_badges))
         for badge in char.account_badges:
             self.assertIsInstance(badge, AccountBadge)
             self.assertIsInstance(badge.name, str)
             self.assertIsInstance(badge.icon_url, str)
             self.assertIsInstance(badge.description, str)
 
     def test_character_from_content_no_selected_badges(self):
         """Testing parsing a character with visible badges but none selected."""
         content = self.load_resource(FILE_CHARACTER_NO_BADGES_SELECTED)
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertEqual("Cozzackirycerz", char.name)
         self.assertEqual(25, char.achievement_points)
         self.assertIsNone(char.title)
         self.assertEqual(3, char.unlocked_titles)
         self.assertEqual(0, len(char.account_badges))
         self.assertEqual(0, len(char.former_names))
 
     def test_character_from_content_multiple_houses(self):
         """Testing parsing a character with multiple houses."""
         content = self.load_resource(FILE_CHARACTER_MULTIPLE_HOUSES)
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertEqual("Sayuri Nowan", char.name)
         self.assertEqual(2, len(char.houses))
         first_house = char.houses[0]
         second_house = char.houses[1]
         self.assertEqual("Cormaya 10", first_house.name)
         self.assertEqual("Old Heritage Estate", second_house.name)
         self.assertEqual("Edron", first_house.town)
         self.assertEqual("Rathleton", second_house.town)
 
     def test_character_from_content_truncated_deaths(self):
         """Testing parsing a character with truncated daths"""
         content = self.load_resource(FILE_CHARACTER_TRUNCATED_DEATHS)
-        char = Character.from_content(content)
+        char = CharacterParser.from_content(content)
         self.assertEqual("Godlike Terror", char.name)
         self.assertEqual(51, len(char.deaths))
         self.assertTrue(char.deaths_truncated)
 
     def test_character_from_content_unrelated(self):
         """Testing parsing an unrelated tibia.com section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            Character.from_content(content)
+            CharacterParser.from_content(content)
 
     # endregion
 
     def test_death_types(self):
         """Testing different death types"""
-        assisted_suicide = Death("Galarzaa", 280, killers=[Killer("Galarzaa", True), Killer("a pixy")],
+        assisted_suicide = Death(level=280,
+                                 killers=[
+                                     DeathParticipant(name="Galarzaa", player=True, summon=None, traded=False),
+                                     DeathParticipant(name="a pixy", player=False, summon=None, traded=False)
+                                 ],
+                                 assists=[],
                                  time=datetime.datetime.now())
         self.assertEqual(assisted_suicide.killer, assisted_suicide.killers[0])
-        self.assertFalse(assisted_suicide.by_player)
+        self.assertTrue(assisted_suicide.by_player)
 
-        spawn_invasion = Death("Galarza", 270, killers=[Killer("a demon"), Killer("Nezune", True)])
+        spawn_invasion = Death(level=270,
+                               killers=[
+                                   DeathParticipant(name="a demon", player=False, summon=None, traded=False),
+                                   DeathParticipant(name="Nezune", player=True, summon=None, traded=False)
+                               ],
+                               assists=[],
+                               time=datetime.datetime.now())
         self.assertEqual(spawn_invasion.killer, spawn_invasion.killers[0])
         self.assertIsNone(spawn_invasion.killer.url)
         self.assertTrue(spawn_invasion.by_player)
```

### Comparing `tibia.py-5.6.0/tests/tests_client.py` & `tibia.py-6.0.0a1/tests/tests_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 import datetime
 import sys
 import unittest.mock
 
 import aiohttp
-import asynctest
 from aioresponses import aioresponses
 
-import tibiapy
 from tests.tests_bazaar import FILE_BAZAAR_CURRENT, FILE_BAZAAR_HISTORY, FILE_AUCTION_FINISHED
 from tests.tests_character import FILE_CHARACTER_RESOURCE, FILE_CHARACTER_NOT_FOUND
 from tests.tests_events import FILE_EVENT_CALENDAR
 from tests.tests_forums import FILE_BOARD_THREAD_LIST, FILE_CM_POST_ARCHIVE_PAGES, FILE_WORLD_BOARDS
 from tests.tests_guild import FILE_GUILD_FULL, FILE_GUILD_LIST
 from tests.tests_highscores import FILE_HIGHSCORES_FULL
 from tests.tests_house import FILE_HOUSE_FULL, FILE_HOUSE_LIST
 from tests.tests_kill_statistics import FILE_KILL_STATISTICS_FULL
 from tests.tests_leaderboards import FILE_LEADERBOARD_CURRENT
-from tests.tests_news import FILE_NEWS_LIST, FILE_NEWS_ARTICLE
+from tests.tests_news import FILE_NEWS_ARCHIVE_RESULTS, FILE_NEWS_ARTICLE
 from tests.tests_tibiapy import TestCommons
 from tests.tests_world import FILE_WORLD_FULL, FILE_WORLD_LIST
-from tibiapy import BoardEntry, CharacterBazaar, Client, Character, CMPostArchive, ForumBoard, Guild, GuildsSection, \
-    Highscores, \
-    HouseType, \
-    HousesSection, \
-    Leaderboard, NewsArchive, VocationFilter, \
-    Category, \
-    House, HouseEntry, \
-    GuildEntry, \
-    KillStatistics, NewsEntry, News, World, WorldOverview, Forbidden, NetworkError, CreatureEntry, Auction, \
-    EventSchedule
+from tibiapy import Client, Forbidden, NetworkError, HouseType, BazaarType
+from tibiapy.models import BoardEntry, CharacterBazaar, Character, CMPostArchive, ForumBoard, Guild, Highscores, \
+    HousesSection, Leaderboard, HighscoresProfession, HighscoresCategory, House, HouseEntry, GuildEntry, KillStatistics, \
+    World, WorldOverview, Auction, NewsArchive, NewsEntry, News, ItemSummary, ForumSection
+from tibiapy.models.creature import CreatureEntry
+from tibiapy.models.event import EventSchedule
+from tibiapy.urls import get_character_url, get_world_guilds_url, get_guild_url, get_house_url, get_world_overview_url, \
+    get_news_archive_url, get_news_url, get_forum_board_url, get_highscores_url, get_kill_statistics_url, \
+    get_event_schedule_url, get_houses_section_url, get_auction_url, get_bazaar_url, get_cm_post_archive_url, \
+    get_leaderboards_url, get_world_url
 
 
-class TestClient(asynctest.TestCase, TestCommons):
+class TestClient(unittest.IsolatedAsyncioTestCase, TestCommons):
     def setUp(self):
         self.client = Client()
 
-    async def tearDown(self):
+    async def asyncTearDown(self):
         await self.client.session.close()
 
     async def test_client_init_pass_session(self):
         """Testing creating an instance passing a session"""
         headers = {"User-Agent": "Python Unit Test"}
         session = aiohttp.ClientSession(headers=headers)
         client = Client(session=session)
@@ -47,122 +45,122 @@
         self.assertEqual(client.session._default_headers, headers)
 
         await client.session.close()
 
     @aioresponses()
     async def test_client_handle_errors(self, mock):
         """Testing error handling"""
-        mock.get(WorldOverview.get_url(), status=403)
+        mock.get(get_world_overview_url(), status=403)
         with self.assertRaises(Forbidden):
-            await self.client.fetch_world_list()
+            await self.client.fetch_world_overview()
 
-        mock.get(WorldOverview.get_url(), status=404)
+        mock.get(get_world_overview_url(), status=404)
         with self.assertRaises(NetworkError):
-            await self.client.fetch_world_list()
+            await self.client.fetch_world_overview()
 
-        mock.get(NewsEntry.get_list_url(), exception=aiohttp.ClientError())
+        mock.get(get_news_archive_url(), exception=aiohttp.ClientError())
         with self.assertRaises(NetworkError):
-            await self.client.fetch_world_list()
+            await self.client.fetch_world_overview()
 
-        mock.post(NewsEntry.get_list_url(), exception=aiohttp.ClientOSError())
+        mock.post(get_news_archive_url(), exception=aiohttp.ClientOSError())
         with self.assertRaises(NetworkError):
-            await self.client.fetch_recent_news(30)
+            await self.client.fetch_news_archive_by_days(30)
 
     @aioresponses()
     async def test_client_fetch_character(self, mock):
         """Testing fetching a character"""
         name = "Tschas"
         content = self.load_resource(FILE_CHARACTER_RESOURCE)
-        mock.get(Character.get_url(name), status=200, body=content)
+        mock.get(get_character_url(name), status=200, body=content)
         character = await self.client.fetch_character(name)
 
         self.assertIsInstance(character.data, Character)
 
     @aioresponses()
     async def test_client_fetch_character_not_found(self, mock):
         """Testing fetching a non existent character"""
         name = "Nezune"
         content = self.load_resource(FILE_CHARACTER_NOT_FOUND)
-        mock.get(Character.get_url(name), status=200, body=content)
+        mock.get(get_character_url(name), status=200, body=content)
         character = await self.client.fetch_character(name)
 
         self.assertIsNone(character.data)
 
     @aioresponses()
     async def test_client_fetch_guild(self, mock):
         """Testing fetching a guild"""
         name = "Vitam et Mortem"
         content = self.load_resource(FILE_GUILD_FULL)
-        mock.get(Guild.get_url(name), status=200, body=content)
+        mock.get(get_guild_url(name), status=200, body=content)
         guild = await self.client.fetch_guild(name)
 
         self.assertIsInstance(guild.data, Guild)
 
     @aioresponses()
     async def test_client_fetch_world_guilds(self, mock):
         """Testing fetching a world's guild list"""
         world = "Zuna"
         content = self.load_resource(FILE_GUILD_LIST)
-        mock.get(GuildsSection.get_url(world), status=200, body=content)
+        mock.get(get_world_guilds_url(world), status=200, body=content)
         response = await self.client.fetch_world_guilds(world)
         guilds = response.data.entries
 
         self.assertIsInstance(guilds[0], GuildEntry)
 
     @aioresponses()
     async def test_client_fetch_highscores_page(self, mock):
         """Testing fetching a highscores page"""
         world = "Estela"
-        category = Category.MAGIC_LEVEL
-        vocations = VocationFilter.KNIGHTS
+        category = HighscoresCategory.MAGIC_LEVEL
+        vocations = HighscoresProfession.KNIGHTS
         content = self.load_resource(FILE_HIGHSCORES_FULL)
-        mock.get(Highscores.get_url(world, category, vocations), status=200, body=content)
+        mock.get(get_highscores_url(world, category, vocations), status=200, body=content)
         highscores = await self.client.fetch_highscores_page(world, category, vocations)
 
         self.assertIsInstance(highscores.data, Highscores)
 
     @aioresponses()
     async def test_client_fetch_house(self, mock):
         """Testing fetching a house"""
         world = "Antica"
         house_id = 5236
         content = self.load_resource(FILE_HOUSE_FULL)
-        mock.get(House.get_url(house_id, world), status=200, body=content)
+        mock.get(get_house_url(world, house_id), status=200, body=content)
         house = await self.client.fetch_house(house_id, world)
 
         self.assertIsInstance(house.data, House)
 
     @aioresponses()
     async def test_client_fetch_world_houses(self, mock):
         """Testing fetching a world's houses"""
         world = "Antica"
         city = "Edron"
         content = self.load_resource(FILE_HOUSE_LIST)
-        mock.get(HousesSection.get_url(world=world, town=city, house_type=HouseType.HOUSE), status=200, body=content)
-        houses = await self.client.fetch_world_houses(world, city)
+        mock.get(get_houses_section_url(world=world, town=city, house_type=HouseType.HOUSE), status=200, body=content)
+        houses = await self.client.fetch_houses_section(world, city)
 
         self.assertIsInstance(houses.data, HousesSection)
         self.assertIsInstance(houses.data.entries[0], HouseEntry)
 
     @aioresponses()
     async def test_client_fetch_kill_statistics(self, mock):
         """Testing fetching kill statistics"""
         world = "Antica"
         content = self.load_resource(FILE_KILL_STATISTICS_FULL)
-        mock.get(KillStatistics.get_url(world), status=200, body=content)
+        mock.get(get_kill_statistics_url(world), status=200, body=content)
         kill_statistics = await self.client.fetch_kill_statistics(world)
 
         self.assertIsInstance(kill_statistics.data, KillStatistics)
 
     @aioresponses()
     async def test_client_fetch_recent_news(self, mock):
         """Testing fetching recent nows"""
-        content = self.load_resource(FILE_NEWS_LIST)
-        mock.post(NewsArchive.get_url(), status=200, body=content)
-        recent_news = await self.client.fetch_recent_news(30)
+        content = self.load_resource(FILE_NEWS_ARCHIVE_RESULTS)
+        mock.post(get_news_archive_url(), status=200, body=content)
+        recent_news = await self.client.fetch_news_archive_by_days(30)
 
         self.assertIsInstance(recent_news.data, NewsArchive)
         self.assertIsInstance(recent_news.data.entries[0], NewsEntry)
 
     async def test_client_fetch_news_archive_invalid_dates(self):
         """Testing fetching news archive with invalid dates"""
         today = datetime.date.today()
@@ -171,54 +169,54 @@
             await self.client.fetch_news_archive(today, yesterday)
 
     @aioresponses()
     async def test_client_fetch_news(self, mock):
         """Testing fetch news"""
         news_id = 6000
         content = self.load_resource(FILE_NEWS_ARTICLE)
-        mock.get(News.get_url(news_id), status=200, body=content)
+        mock.get(get_news_url(news_id), status=200, body=content)
         news = await self.client.fetch_news(news_id)
 
         self.assertIsInstance(news.data, News)
 
     @aioresponses()
     async def test_client_fetch_world(self, mock):
         """Testing fetching a world"""
         name = "Antica"
         content = self.load_resource(FILE_WORLD_FULL)
-        mock.get(World.get_url(name), status=200, body=content)
+        mock.get(get_world_url(name), status=200, body=content)
         world = await self.client.fetch_world(name)
 
         self.assertIsInstance(world.data, World)
 
     @aioresponses()
     async def test_client_fetch_world_list(self, mock):
         """Testing fetching the world list"""
         content = self.load_resource(FILE_WORLD_LIST)
-        mock.get(WorldOverview.get_url(), status=200, body=content)
-        worlds = await self.client.fetch_world_list()
+        mock.get(get_world_overview_url(), status=200, body=content)
+        worlds = await self.client.fetch_world_overview()
 
         self.assertIsInstance(worlds.data, WorldOverview)
 
     @aioresponses()
     async def test_client_fetch_boosted_creature(self, mock):
         """Testing fetching the boosted creature"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        mock.get(News.get_list_url(), status=200, body=content)
+        mock.get(get_news_archive_url(), status=200, body=content)
         creature = await self.client.fetch_boosted_creature()
 
         self.assertIsInstance(creature.data, CreatureEntry)
 
     @aioresponses()
     async def test_client_fetch_cm_post_archive(self, mock):
         """Testing fetching the CM Post Archive"""
         content = self.load_resource(FILE_CM_POST_ARCHIVE_PAGES)
         start_date = datetime.date.today()-datetime.timedelta(days=40)
         end_date = datetime.date.today()
-        mock.get(CMPostArchive.get_url(start_date, end_date), status=200, body=content)
+        mock.get(get_cm_post_archive_url(start_date, end_date), status=200, body=content)
         cm_post_archive = await self.client.fetch_cm_post_archive(start_date, end_date)
 
         self.assertIsInstance(cm_post_archive.data, CMPostArchive)
 
     async def test_client_fetch_cm_post_archive_invalid_dates(self):
         """Testing fetching the CM Post Archive with invalid dates"""
         end_date = datetime.date.today()-datetime.timedelta(days=40)
@@ -233,118 +231,114 @@
         with self.assertRaises(ValueError):
             await self.client.fetch_cm_post_archive(start_date, end_date, -1)
 
     @aioresponses()
     async def test_client_fetch_current_auctions(self, mock):
         """Testing fetching the current auctions"""
         content = self.load_resource(FILE_BAZAAR_CURRENT)
-        mock.get(CharacterBazaar.get_current_auctions_url(), status=200, body=content)
+        mock.get(get_bazaar_url(BazaarType.CURRENT), status=200, body=content)
         response = await self.client.fetch_current_auctions()
         self.assertIsInstance(response.data, CharacterBazaar)
 
     async def test_client_fetch_current_auctions_invalid_page(self):
         """Testing fetching the current auctions with an invalid page"""
         with self.assertRaises(ValueError):
             await self.client.fetch_current_auctions(-1)
 
     @aioresponses()
     async def test_client_fetch_auction_history(self, mock):
         """Testing fetching the auction history"""
         content = self.load_resource(FILE_BAZAAR_HISTORY)
-        mock.get(CharacterBazaar.get_auctions_history_url(), status=200, body=content)
+        mock.get(get_bazaar_url(BazaarType.HISTORY), status=200, body=content)
         response = await self.client.fetch_auction_history()
         self.assertIsInstance(response.data, CharacterBazaar)
 
     async def test_client_fetch_auction_history_invalid_page(self):
         """Testing fetching the auction history with an incorrect page"""
         with self.assertRaises(ValueError):
             await self.client.fetch_auction_history(-1)
 
     @aioresponses()
     async def test_client_fetch_auction(self, mock):
         """Testing fetching an auction"""
         content = self.load_resource(FILE_AUCTION_FINISHED)
-        mock.get(Auction.get_url(134), status=200, body=content)
+        mock.get(get_auction_url(134), status=200, body=content)
         response = await self.client.fetch_auction(134)
         self.assertIsInstance(response.data, Auction)
 
     async def test_client_fetch_auction_invalid_id(self):
         """Testing fetching an auction with an invalid id"""
         with self.assertRaises(ValueError):
             await self.client.fetch_auction(-1)
 
     @aioresponses()
     async def test_client_fetch_event_calendar(self, mock):
         """Testing fetching the auction history"""
         content = self.load_resource(FILE_EVENT_CALENDAR)
-        mock.get(EventSchedule.get_url(), status=200, body=content)
+        mock.get(get_event_schedule_url(), status=200, body=content)
         response = await self.client.fetch_event_schedule()
         self.assertIsInstance(response.data, EventSchedule)
 
     async def test_client_fetch_event_calendar_invalid_params(self):
         """Testing fetching the auction history"""
         with self.assertRaises(ValueError):
             await self.client.fetch_event_schedule(3)
 
     @aioresponses()
     async def test_client_fetch_forum_community_boards(self, mock):
         """Testing fetching the community boards"""
         content = self.load_resource(FILE_WORLD_BOARDS)
         mock.get(BoardEntry.get_community_boards_url(), status=200, body=content)
         response = await self.client.fetch_forum_community_boards()
-        self.assertIsInstance(response.data[0], BoardEntry)
+        self.assertIsInstance(response.data, ForumSection)
 
     @aioresponses()
     async def test_client_fetch_forum_trade_boards(self, mock):
         """Testing fetching the trade boards"""
         content = self.load_resource(FILE_WORLD_BOARDS)
         mock.get(BoardEntry.get_trade_boards_url(), status=200, body=content)
         response = await self.client.fetch_forum_trade_boards()
-        self.assertIsInstance(response.data[0], BoardEntry)
+        self.assertIsInstance(response.data, ForumSection)
 
     @aioresponses()
     async def test_client_fetch_forum_support_boards(self, mock):
         """Testing fetching the support boards"""
         content = self.load_resource(FILE_WORLD_BOARDS)
         mock.get(BoardEntry.get_support_boards_url(), status=200, body=content)
         response = await self.client.fetch_forum_support_boards()
-        self.assertIsInstance(response.data[0], BoardEntry)
+        self.assertIsInstance(response.data, ForumSection)
 
     @aioresponses()
     async def test_client_fetch_forum_world_boards(self, mock):
         """Testing fetching the world boards"""
         content = self.load_resource(FILE_WORLD_BOARDS)
         mock.get(BoardEntry.get_world_boards_url(), status=200, body=content)
         response = await self.client.fetch_forum_world_boards()
-        self.assertIsInstance(response.data[0], BoardEntry)
+        self.assertIsInstance(response.data, ForumSection)
 
     @aioresponses()
     async def test_client_fetch_forum_board(self, mock):
         """Testing fetching a forum board"""
         content = self.load_resource(FILE_BOARD_THREAD_LIST)
-        mock.get(BoardEntry.get_url(1), status=200, body=content)
+        mock.get(get_forum_board_url(1), status=200, body=content)
         response = await self.client.fetch_forum_board(1)
         self.assertIsInstance(response.data, ForumBoard)
 
     @aioresponses()
     async def test_client_fetch_leaderboards(self, mock):
         """Testing fetching the leaderboards"""
         content = self.load_resource(FILE_LEADERBOARD_CURRENT)
-        mock.get(Leaderboard.get_url("Antica"), status=200, body=content)
+        mock.get(get_leaderboards_url("Antica"), status=200, body=content)
         response = await self.client.fetch_leaderboard("Antica")
         self.assertIsInstance(response.data, Leaderboard)
 
-    @unittest.mock.patch("tibiapy.bazaar.Auction._parse_page_items")
+    @unittest.mock.patch("tibiapy.parsers.bazaar.AuctionParser._parse_page_items")
     @unittest.skipIf(sys.version_info < (3, 8, 0), "AsyncMock was implemented in 3.8")
     async def test_client__fetch_all_pages_success(self, parse_page_items):
         """Testing internal method to fetch all pages of an auction item collection."""
-        paginator = tibiapy.ItemSummary(page=1, total_pages=5)
+        paginator = ItemSummary(page=1, total_pages=5)
         self.client._fetch_ajax_page = unittest.mock.AsyncMock()
 
         await self.client._fetch_all_pages(1, paginator, 1)
 
         self.assertEqual(4, self.client._fetch_ajax_page.await_count)
         self.assertEqual(4, parse_page_items.call_count)
-
-    async def test_client__fetch_all_pages_none_input(self):
-        """Testing internal method to fetch all pages of an auction item collection."""
-        self.assertIsNone(await self.client._fetch_all_pages(1, None, 1))
```

### Comparing `tibia.py-5.6.0/tests/tests_creature.py` & `tibia.py-6.0.0a1/tests/tests_creature.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import BoostableBosses, InvalidContent, CreaturesSection, Creature, CreatureEntry
+from tibiapy import InvalidContent
+from tibiapy.models.creature import CreatureEntry
+from tibiapy.parsers.creature import CreaturesSectionParser, CreatureParser, BoostableBossesParser
 
 FILE_CREATURE_SECTION = "library/creature_list.txt"
 FILE_CREATURE_CONVINCEABLE = "library/creature_convinceable.txt"
 FILE_CREATURE_ELEMENTAL_RESISTANCES = "library/creature_elemental_resistances.txt"
 FILE_BOOSTABLE_BOSSES = "library/boss_list.txt"
 
 
 class TestCreature(TestCommons, unittest.TestCase):
     def test_creatures_section_from_boosted_creature_header_content(self):
         """Testing parsing the boosted creture from any tibia.com page."""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        creature = CreaturesSection.boosted_creature_from_header(content)
+        creature = CreaturesSectionParser.boosted_creature_from_header(content)
 
         self.assertIsInstance(creature, CreatureEntry)
         self.assertEqual("Menacing Carnivor", creature.name)
 
     def test_creatures_section_from_boosted_creature_header_content_not_tibiacom(self):
         """Testing parsing the boosted creature from a page that is not Tibia.com"""
         with self.assertRaises(InvalidContent):
-            CreaturesSection.boosted_creature_from_header("<html><div><p>Nothing</p></div></html>")
+            CreaturesSectionParser.boosted_creature_from_header("<html><div><p>Nothing</p></div></html>")
 
     def test_creature_section_from_content(self):
         """Test parsing the creatures section"""
         content = self.load_resource(FILE_CREATURE_SECTION)
-        creatures = CreaturesSection.from_content(content)
+        creatures = CreaturesSectionParser.from_content(content)
 
         self.assertIsNotNone(creatures)
         self.assertIsNotNone(creatures.boosted_creature)
         self.assertEqual("Blood Crab", creatures.boosted_creature.name)
         self.assertEqual("bloodcrab", creatures.boosted_creature.identifier)
         self.assertIsNotNone(creatures.boosted_creature.image_url)
         self.assertIsNotNone(creatures.boosted_creature.url)
@@ -40,33 +42,33 @@
                 self.assertIsInstance(creature.name, str)
                 self.assertIsInstance(creature.identifier, str)
 
     def test_creatures_section_from_content_invalid_content(self):
         """Testing parsing the creatures section from an invalid section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            CreaturesSection.from_content(content)
+            CreaturesSectionParser.from_content(content)
 
     def test_creature_from_content(self):
         content = self.load_resource(FILE_CREATURE_CONVINCEABLE)
-        creature = Creature.from_content(content)
+        creature = CreatureParser.from_content(content)
 
         self.assertIsNotNone(creature)
         self.assertEqual("Fish", creature.name)
         self.assertEqual("fish", creature.identifier)
         self.assertEqual(25, creature.hitpoints)
         self.assertEqual(0, creature.experience)
         self.assertEqual(0, creature.mana_cost)
         self.assertFalse(creature.summonable)
         self.assertTrue(creature.convinceable)
         self.assertEqual("nothing", creature.loot)
 
     def test_creature_from_content_elemental_resistances(self):
         content = self.load_resource(FILE_CREATURE_ELEMENTAL_RESISTANCES)
-        creature = Creature.from_content(content)
+        creature = CreatureParser.from_content(content)
 
         self.assertIsNotNone(creature)
         self.assertEqual("Dragons", creature.name)
         self.assertEqual("dragon", creature.identifier)
         self.assertEqual(1000, creature.hitpoints)
         self.assertEqual(700, creature.experience)
         self.assertIsNone(creature.mana_cost)
@@ -77,22 +79,22 @@
         self.assertIn("fire", creature.immune_to)
         self.assertIn("ice", creature.weak_against)
 
     def test_creature_from_content_invalid_content(self):
         """Testing parsing the creatures section from an invalid section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
 
-        creature = Creature.from_content(content)
+        creature = CreatureParser.from_content(content)
 
         self.assertIsNone(creature)
 
     def test_boostable_bosses_from_content(self):
         """Test parsing the boostable bosses section"""
         content = self.load_resource(FILE_BOOSTABLE_BOSSES)
-        bosses = BoostableBosses.from_content(content)
+        bosses = BoostableBossesParser.from_content(content)
 
         self.assertIsNotNone(bosses)
         self.assertIsNotNone(bosses.boosted_boss)
         self.assertEqual("Tentugly", bosses.boosted_boss.name)
         self.assertEqual("fakeseamonster", bosses.boosted_boss.identifier)
         self.assertIsNotNone(bosses.boosted_boss.image_url)
         self.assertEqual(88, len(bosses.bosses))
@@ -102,10 +104,10 @@
                 self.assertIsInstance(boss.identifier, str)
 
     def test_boostable_bosses_from_content_invalid_content(self):
         """Testing parsing the creatures section from an invalid section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
 
         with self.assertRaises(InvalidContent):
-            BoostableBosses.from_content(content)
+            BoostableBossesParser.from_content(content)
```

### Comparing `tibia.py-5.6.0/tests/tests_events.py` & `tibia.py-6.0.0a1/tests/tests_events.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import unittest
 import datetime
+import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import EventSchedule
+from tibiapy.models.event import EventSchedule
+from tibiapy.parsers.event import EventScheduleParser
+from tibiapy.urls import get_event_schedule_url
 
-FILE_EVENT_CALENDAR = "events/tibiacom_calendar.txt"
+FILE_EVENT_CALENDAR = "events/event_schedule.txt"
 
 
 class TestEvents(TestCommons, unittest.TestCase):
-    # region Tibia.com Tests
-    def test_event_schedule_from_content(self):
+    def test_event_schedule_parser_from_content(self):
         """Testing parsing the event schedule"""
         content = self.load_resource(FILE_EVENT_CALENDAR)
-        calendar = EventSchedule.from_content(content)
+        calendar = EventScheduleParser.from_content(content)
 
         self.assertIsInstance(calendar, EventSchedule)
         self.assertEqual(9, calendar.month)
         self.assertEqual(2020, calendar.year)
         self.assertEqual(6, len(calendar.events))
-        self.assertEqual(calendar.url, EventSchedule.get_url(calendar.month, calendar.year))
+        self.assertEqual(calendar.url, get_event_schedule_url(calendar.month, calendar.year))
         events_on_day = calendar.get_events_on(datetime.date(2020, 9, 15))
         self.assertEqual(2, len(events_on_day))
         self.assertEqual(4, events_on_day[0].duration)
-    # endregion
```

### Comparing `tibia.py-5.6.0/tests/tests_forums.py` & `tibia.py-6.0.0a1/tests/tests_forums.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import datetime
 import unittest
 
-import tibiapy
 from tests.tests_tibiapy import TestCommons
-from tibiapy import CMPostArchive, ForumAnnouncement, ForumBoard, ForumThread, InvalidContent, LastPost, BoardEntry, \
-    ThreadEntry, ThreadStatus
+from tibiapy import InvalidContent, ThreadStatus
+from tibiapy.models import BoardEntry, LastPost, ThreadEntry, CMPostArchive
+from tibiapy.models.forum import BasePost, ForumSection
+from tibiapy.parsers.forum import ForumBoardParser, ForumAnnouncementParser, ForumThreadParser, \
+    CMPostArchiveParser, ForumSectionParser
+from tibiapy.urls import get_forum_board_url, get_cm_post_archive_url
 
 FILE_WORLD_BOARDS = "forums/tibiacom_section.txt"
 FILE_SECTION_EMPTY_BOARD = "forums/tibiacom_section_empty_board.txt"
 FILE_SECTION_EMPTY = "forums/tibiacom_section_empty.txt"
 FILE_BOARD_THREAD_LIST = "forums/tibiacom_board.txt"
 FILE_BOARD_EMPTY_THREAD_LIST = "forums/tibiacom_board_empty.txt"
 FILE_BOARD_INVALID_PAGE = "forums/tibiacom_board_invalid_page.txt"
@@ -21,73 +24,77 @@
 FILE_CM_POST_ARCHIVE_INITIAL = "forums/tibiacom_cmpostarchive_initial.txt"
 FILE_CM_POST_ARCHIVE_NO_PAGES = "forums/tibiacom_cmpostarchive_no_pages.txt"
 FILE_CM_POST_ARCHIVE_NO_RESULTS = "forums/tibiacom_cmpostarchive_no_results.txt"
 FILE_CM_POST_ARCHIVE_PAGES = "forums/tibiacom_cmpostarchive_pages.txt"
 
 
 class TestForum(TestCommons, unittest.TestCase):
-    def test_listed_board_list_from_content_world_boards(self):
+    def test_forum_section_parser_from_content_world_boards(self):
         content = self.load_resource(FILE_WORLD_BOARDS)
 
-        boards = BoardEntry.list_from_content(content)
+        forum_section = ForumSectionParser.from_content(content)
 
-        self.assertEqual(82, len(boards))
-        for i, board in enumerate(boards):
+        self.assertEqual(2, forum_section.section_id)
+        self.assertEqual(82, len(forum_section.entries))
+        for i, board in enumerate(forum_section.entries):
             with self.subTest(i=i):
                 self.assertIsInstance(board, BoardEntry)
                 self.assertIsNotNone(board.name)
                 self.assertGreater(board.board_id, 0)
                 self.assertGreater(board.posts, 0)
                 self.assertGreater(board.threads, 0)
                 self.assertIsInstance(board.last_post, LastPost)
 
-    def test_listed_board_list_from_content_empty_board(self):
+    def test_forum_section_parser_from_content_empty_board(self):
         content = self.load_resource(FILE_SECTION_EMPTY_BOARD)
 
-        boards = BoardEntry.list_from_content(content)
+        forum_section = ForumSectionParser.from_content(content)
 
-        self.assertEqual(84, len(boards))
-        for i, board in enumerate(boards):
+        self.assertEqual(3, forum_section.section_id)
+        self.assertEqual(84, len(forum_section.entries))
+        for i, board in enumerate(forum_section.entries):
             with self.subTest(i=i):
                 self.assertIsInstance(board, BoardEntry)
                 self.assertIsNotNone(board.name)
                 self.assertGreater(board.board_id, 0)
                 self.assertGreaterEqual(board.posts, 0)
                 self.assertGreaterEqual(board.threads, 0)
                 self.assertIsNotNone(board.url)
 
-    def test_listed_board_list_from_content_empty_section(self):
+    def test_forum_section_parser_from_content_empty_section(self):
         content = self.load_resource(FILE_SECTION_EMPTY)
 
-        boards = BoardEntry.list_from_content(content)
+        forum_section = ForumSectionParser.from_content(content)
 
-        self.assertIsInstance(boards, list)
+        self.assertEqual(10, forum_section.section_id)
+        self.assertIsInstance(forum_section, ForumSection)
+        self.assertEqual(0, len(forum_section.entries))
 
-    def test_listed_board_list_from_content_unrelated_section(self):
+    def test_forum_section_parser_from_content_unrelated_section(self):
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
 
         with self.assertRaises(InvalidContent):
-            BoardEntry.list_from_content(content)
+            ForumSectionParser.from_content(content)
 
     def test_forum_board_from_content(self):
         content = self.load_resource(FILE_BOARD_THREAD_LIST)
 
-        board = ForumBoard.from_content(content)
+        board = ForumBoardParser.from_content(content)
 
         self.assertIsNotNone(board)
         self.assertEqual("Antica", board.name)
         self.assertEqual("World Boards", board.section)
-        self.assertEqual(1, board.page)
+        self.assertEqual(1, board.current_page)
         self.assertEqual(2, board.total_pages)
         self.assertEqual(25, board.board_id)
-        self.assertEqual(30, len(board.threads))
+        self.assertEqual(30, len(board.entries))
         self.assertIsNotNone(board.url)
         self.assertIsNotNone(board.next_page_url)
-        self.assertEqual(board.next_page_url, BoardEntry.get_url(board.board_id, board.page + 1, board.age))
-        for i, thread in enumerate(board.threads):
+        self.assertEqual(board.next_page_url, get_forum_board_url(board.board_id, board.current_page + 1, board.age))
+        for i, thread in enumerate(board.entries):
             with self.subTest(i=i):
                 self.assertIsInstance(thread, ThreadEntry)
                 self.assertIsNotNone(thread.title)
                 self.assertGreater(thread.thread_id, 0)
                 self.assertGreaterEqual(thread.views, 0)
                 self.assertGreaterEqual(thread.replies, 0)
                 self.assertIsInstance(thread.last_post, LastPost)
@@ -101,63 +108,63 @@
         self.assertIsNotNone(BoardEntry.get_support_boards_url())
         self.assertIsNotNone(BoardEntry.get_world_boards_url())
         self.assertIsNotNone(BoardEntry.get_trade_boards_url())
 
     def test_forum_board_from_content_empty_threads(self):
         content = self.load_resource(FILE_BOARD_EMPTY_THREAD_LIST)
 
-        board = ForumBoard.from_content(content)
+        board = ForumBoardParser.from_content(content)
 
         self.assertIsNotNone(board)
         self.assertEqual("Role Playing", board.name)
         self.assertEqual("Community Boards", board.section)
-        self.assertEqual(1, board.page)
+        self.assertEqual(1, board.current_page)
         self.assertEqual(1, board.total_pages)
         self.assertEqual(11, board.board_id)
-        self.assertEqual(0, len(board.threads))
+        self.assertEqual(0, len(board.entries))
         self.assertIsNone(board.next_page_url)
         self.assertIsNone(board.previous_page_url)
 
     def test_forum_board_from_content_unrelated_section(self):
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
 
         with self.assertRaises(InvalidContent):
-            ForumBoard.from_content(content)
+            ForumBoardParser.from_content(content)
 
     def test_forum_board_from_content_invalid_page(self):
         content = self.load_resource(FILE_BOARD_INVALID_PAGE)
 
-        board = ForumBoard.from_content(content)
+        board = ForumBoardParser.from_content(content)
 
         self.assertEqual("Antica", board.name)
         self.assertEqual("World Boards", board.section)
-        self.assertEqual([], board.threads)
+        self.assertEqual([], board.entries)
         self.assertEqual(0, board.board_id)
 
     def test_forum_board_from_content_golden_frame(self):
         content = self.load_resource(FILE_BOARD_GOLDEN_FRAMES)
 
-        board = ForumBoard.from_content(content)
+        board = ForumBoardParser.from_content(content)
 
         self.assertEqual("Proposals (English Only)", board.name)
         self.assertEqual("Community Boards", board.section)
-        self.assertEqual(30, len(board.threads))
+        self.assertEqual(30, len(board.entries))
         self.assertEqual(5, len(board.announcements))
         self.assertEqual(1893, board.total_pages)
-        for i, thread in enumerate(board.threads):
+        for i, thread in enumerate(board.entries):
             with self.subTest(i=i):
                 self.assertTrue(thread.golden_frame)
                 self.assertTrue(thread.status & ThreadStatus.HOT)
                 self.assertTrue(thread.status & ThreadStatus.CLOSED)
                 self.assertIsNotNone(thread.url)
 
     def test_forum_announcement_from_content(self):
         content = self.load_resource(FILE_ANNOUNCEMENT)
 
-        announcement = ForumAnnouncement.from_content(content, 33)
+        announcement = ForumAnnouncementParser.from_content(content, 33)
 
         self.assertIsNotNone(announcement)
         self.assertEqual("Legal Disclaimer", announcement.title)
         self.assertEqual(33, announcement.announcement_id)
         self.assertEqual("Proposals (English Only)", announcement.board)
         self.assertEqual(10, announcement.board_id)
         self.assertEqual("Community Boards", announcement.section)
@@ -169,45 +176,45 @@
         self.assertEqual("Vunira", announcement.author.world)
         self.assertEqual("Community Manager", announcement.author.position)
         self.assertIsNotNone(announcement.url)
 
     def test_forum_announcement_from_content_not_found(self):
         content = self.load_resource(FILE_ANNOUNCEMENT_NOT_FOUND)
 
-        announcement = ForumAnnouncement.from_content(content, 34)
+        announcement = ForumAnnouncementParser.from_content(content, 34)
 
         self.assertIsNone(announcement)
 
     def test_forum_announcement_from_content_unrelated_section(self):
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
 
         with self.assertRaises(InvalidContent):
-            ForumAnnouncement.from_content(content, 34)
+            ForumAnnouncementParser.from_content(content, 34)
 
     def test_forum_thread_from_content(self):
         content = self.load_resource(FILE_THREAD)
 
-        thread = ForumThread.from_content(content)
+        thread = ForumThreadParser.from_content(content)
 
         self.assertEqual("News: Team Finder, Visualisation of Loot Lists", thread.title)
         self.assertEqual(4797985, thread.thread_id)
         self.assertEqual('Auditorium (English Only)', thread.board)
         self.assertEqual('Community Boards', thread.section)
         self.assertEqual(4796826, thread.previous_topic_number)
         self.assertEqual(4797838, thread.next_topic_number)
-        self.assertEqual(1, thread.page)
+        self.assertEqual(1, thread.current_page)
         self.assertEqual(9, thread.total_pages)
-        self.assertEqual(20, len(thread.posts))
+        self.assertEqual(20, len(thread.entries))
         self.assertIsNotNone(thread.url)
         self.assertIsNone(thread.previous_page_url)
         self.assertIsNotNone(thread.next_page_url)
         self.assertIsNotNone(thread.previous_thread_url)
         self.assertIsNotNone(thread.next_thread_url)
 
-        post = thread.posts[0]
+        post = thread.entries[0]
         self.assertEqual("Skerio", post.author.name)
         self.assertEqual("Olima", post.author.world)
         self.assertEqual("Community Manager", post.author.position)
         self.assertEqual(872, post.author.posts)
         self.assertEqual("Mirade", post.edited_by)
         self.assertTrue(post.golden_frame)
         self.assertEqual(38969385, post.post_id)
@@ -215,107 +222,107 @@
 
         with self.assertRaises(ValueError):
             thread.get_page_url(-1)
 
     def test_forum_thread_from_content_invalid_page(self):
         content = self.load_resource(FILE_THREAD_INVALID_PAGE)
 
-        thread = ForumThread.from_content(content)
+        thread = ForumThreadParser.from_content(content)
 
         self.assertEqual("News: Te...", thread.title)
         self.assertEqual(0, thread.thread_id)
         self.assertEqual('Auditorium (English Only)', thread.board)
         self.assertEqual('Community Boards', thread.section)
-        self.assertEqual(0, thread.previous_topic_number)
-        self.assertEqual(0, thread.next_topic_number)
-        self.assertEqual(1, thread.page)
+        self.assertIsNone(thread.previous_topic_number)
+        self.assertIsNone(thread.next_topic_number)
+        self.assertEqual(1, thread.current_page)
         self.assertEqual(1, thread.total_pages)
-        self.assertEqual(0, len(thread.posts))
+        self.assertEqual(0, len(thread.entries))
 
     def test_forum_thread_from_content_not_found(self):
         content = self.load_resource(FILE_THREAD_NOT_FOUND)
 
-        thread = ForumThread.from_content(content)
+        thread = ForumThreadParser.from_content(content)
 
         self.assertIsNone(thread)
 
     def test_forum_thread_from_content_unrelated_section(self):
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
 
         with self.assertRaises(InvalidContent):
-            ForumThread.from_content(content)
+            ForumThreadParser.from_content(content)
 
     def test_cm_post_archive_from_content_initial(self):
         content = self.load_resource(FILE_CM_POST_ARCHIVE_INITIAL)
 
-        cm_post_archive = CMPostArchive.from_content(content)
+        cm_post_archive = CMPostArchiveParser.from_content(content)
 
         self.assertIsNotNone(cm_post_archive)
         self.assertEqual(0, cm_post_archive.results_count)
-        self.assertEqual(1, cm_post_archive.page)
+        self.assertEqual(1, cm_post_archive.current_page)
         self.assertEqual(1, cm_post_archive.total_pages)
 
     def test_cm_post_archive_from_content_no_pages(self):
         content = self.load_resource(FILE_CM_POST_ARCHIVE_NO_PAGES)
 
-        cm_post_archive = CMPostArchive.from_content(content)
+        cm_post_archive = CMPostArchiveParser.from_content(content)
 
         self.assertIsNotNone(cm_post_archive)
         self.assertEqual(5, cm_post_archive.results_count)
-        self.assertEqual(1, cm_post_archive.page)
+        self.assertEqual(1, cm_post_archive.current_page)
         self.assertEqual(1, cm_post_archive.total_pages)
-        self.assertEqual(cm_post_archive.results_count, len(cm_post_archive.posts))
+        self.assertEqual(cm_post_archive.results_count, len(cm_post_archive.entries))
 
-        post = cm_post_archive.posts[0]
-        self.assertIsInstance(post, tibiapy.abc.BasePost)
+        post = cm_post_archive.entries[0]
+        self.assertIsInstance(post, BasePost)
         self.assertEqual('Auditorium (English Only)', post.board)
         self.assertEqual(38974254, post.post_id)
         self.assertEqual('Ticker Messages June 2020', post.thread_title)
 
     def test_cm_post_archive_from_content_no_results(self):
         content = self.load_resource(FILE_CM_POST_ARCHIVE_NO_RESULTS)
 
-        cm_post_archive = CMPostArchive.from_content(content)
+        cm_post_archive = CMPostArchiveParser.from_content(content)
 
         self.assertIsNotNone(cm_post_archive)
         self.assertEqual(0, cm_post_archive.results_count)
-        self.assertEqual(1, cm_post_archive.page)
+        self.assertEqual(1, cm_post_archive.current_page)
         self.assertEqual(1, cm_post_archive.total_pages)
-        self.assertEqual(cm_post_archive.results_count, len(cm_post_archive.posts))
+        self.assertEqual(cm_post_archive.results_count, len(cm_post_archive.entries))
 
     def test_cm_post_archive_from_content_pages(self):
         content = self.load_resource(FILE_CM_POST_ARCHIVE_PAGES)
 
-        cm_post_archive = CMPostArchive.from_content(content)
+        cm_post_archive = CMPostArchiveParser.from_content(content)
 
         self.assertIsNotNone(cm_post_archive)
         self.assertIsNotNone(cm_post_archive.url)
         self.assertIsNotNone(cm_post_archive.previous_page_url)
         self.assertIsNone(cm_post_archive.next_page_url)
         self.assertEqual(8370, cm_post_archive.results_count)
-        self.assertEqual(168, cm_post_archive.page)
+        self.assertEqual(168, cm_post_archive.current_page)
         self.assertEqual(168, cm_post_archive.total_pages)
-        self.assertEqual(20, len(cm_post_archive.posts))
+        self.assertEqual(20, len(cm_post_archive.entries))
 
     def test_cm_post_archive_from_content_unrelated_section(self):
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            CMPostArchive.from_content(content)
+            CMPostArchiveParser.from_content(content)
 
     def test_cm_post_archive_get_page_url_negative_page(self):
         with self.assertRaises(ValueError):
             cmpost_archive = CMPostArchive()
             cmpost_archive.get_page_url(-1)
 
     def test_cm_post_archive_get_url_missing_parameter(self):
         with self.assertRaises(TypeError):
-            CMPostArchive.get_url(None, datetime.date.today())
+            get_cm_post_archive_url(None, datetime.date.today())
         with self.assertRaises(TypeError):
-            CMPostArchive.get_url(datetime.date.today(), None)
+            get_cm_post_archive_url(datetime.date.today(), None)
 
     def test_cm_post_archive_get_url_invalid_dates(self):
         with self.assertRaises(ValueError):
-            CMPostArchive.get_url(datetime.date.today(), datetime.date.today()-datetime.timedelta(days=20))
+            get_cm_post_archive_url(datetime.date.today(), datetime.date.today()-datetime.timedelta(days=20))
 
     def test_cm_post_archive_get_url_invalid_page(self):
         with self.assertRaises(ValueError):
-            CMPostArchive.get_url(datetime.date.today()-datetime.timedelta(days=20), datetime.date.today(), -2)
+            get_cm_post_archive_url(datetime.date.today()-datetime.timedelta(days=20), datetime.date.today(), -2)
```

### Comparing `tibia.py-5.6.0/tests/tests_guild.py` & `tibia.py-6.0.0a1/tests/tests_guild.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import datetime
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import Guild, GuildHouse, GuildInvite, GuildMember, GuildWars, GuildsSection, InvalidContent, GuildEntry
+from tibiapy import InvalidContent
+from tibiapy.builders.guild import GuildBuilder
+from tibiapy.models import Guild, GuildWars
+from tibiapy.models.guild import GuildHouse
+from tibiapy.parsers.guild import GuildParser, GuildWarsParser, GuildsSectionParser
+from tibiapy.urls import get_world_guilds_url, get_guild_url, get_guild_wars_url
 
 FILE_GUILD_FULL = "guild/tibiacom_full.txt"
 FILE_GUILD_NOT_FOUND = "guild/tibiacom_not_found.txt"
 FILE_GUILD_INFO_COMPLETE = "guild/tibiacom_info_complete.txt"
 FILE_GUILD_INFO_MINIMUM = "guild/tibiacom_info_minimum.txt"
 FILE_GUILD_INFO_DISBANDING = "guild/tibiacom_info_disbanding.txt"
 FILE_GUILD_INFO_FORMATION = "guild/tibiacom_info_formation.txt"
@@ -17,23 +22,23 @@
 FILE_GUILD_WAR_ACTIVE_HISTORY = "guild/wars/tibiacom_active_history.txt"
 FILE_GUILD_WAR_EMPTY = "guild/wars/tibiacom_empty.txt"
 FILE_GUILD_WAR_UNACTIVE_HISTORY = "guild/wars/tibiacom_unactive_history.txt"
 
 
 class TestsGuild(TestCommons, unittest.TestCase):
     def setUp(self):
-        self.guild = Guild()
+        self.guild = GuildBuilder()
 
     def test_guild_from_content(self):
         """Testing parsing a guild"""
         content = self.load_resource(FILE_GUILD_FULL)
-        guild = Guild.from_content(content)
+        guild = GuildParser.from_content(content)
         self.assertIsInstance(guild, Guild, "Guild should be a Guild object.")
-        self.assertEqual(guild.url, Guild.get_url(guild.name))
-        self.assertEqual(guild.url_wars, Guild.get_url_wars(guild.name))
+        self.assertEqual(guild.url, get_guild_url(guild.name))
+        self.assertEqual(guild.url_wars, get_guild_wars_url(guild.name))
         self.assertTrue(guild.active, "Guild should be active")
         self.assertIsInstance(guild.founded, datetime.date, "Guild founded date should be an instance of datetime.date")
         self.assertTrue(guild.open_applications, "Guild applications should be open")
         self.assertIsNotNone(guild.description, "Guild should have a description")
         self.assertTrue(guild.members, "Guild should have members")
         self.assertEqual(guild.member_count, len(guild.members))
         self.assertTrue(guild.invites, "Guild should have invites")
@@ -47,178 +52,133 @@
         for invited in guild.invites:
             self.assertIsNotNone(invited.name, "Invited character's name should not be None.")
             self.assertIsInstance(invited.date, datetime.date, "Invited character's date should be datetime.date.")
 
         self.assertEqual(8, len(guild.members_by_rank['Vice Leader']))
 
         self.assertIsInstance(guild.guildhall, GuildHouse)
-        self.assertEqual(guild.guildhall.owner, guild.members[0].name)
-        self.assertEqual(guild.guildhall.world, guild.world)
         self.assertIsInstance(guild.guildhall.paid_until_date, datetime.date)
 
     def test_guild_from_content_not_found(self):
         """Testing parsing a non existent guild"""
         content = self.load_resource(FILE_GUILD_NOT_FOUND)
-        guild = Guild.from_content(content)
+        guild = GuildParser.from_content(content)
         self.assertIsNone(guild)
 
     def test_guild_from_content_unrelated(self):
         """Testing parsing an unrelated tibiacom section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            Guild.from_content(content)
+            GuildParser.from_content(content)
 
     def test_guild_from_content_complete_info(self):
         """Testing parsing a guild with all information possible"""
         content = self.load_parsed_resource(FILE_GUILD_INFO_COMPLETE)
-        self.guild._parse_guild_disband_info(content)
-        self.assertIsNone(self.guild.disband_condition, "Guild should not be under disband warning")
-        self.assertIsNone(self.guild.disband_date, "Guild should not have disband date")
-
-        self.guild._parse_guild_guildhall(content)
-        self.assertIsNotNone(self.guild.guildhall, "Guild should have guildhall")
-        self.assertEqual(self.guild.guildhall.name, "Sky Lane, Guild 1")
-        self.assertEqual(self.guild.guildhall.paid_until_date, datetime.date(2018, 8, 26))
+        GuildParser._parse_guild_disband_info(self.guild, content)
+        self.assertIsNone(self.guild._disband_condition, "Guild should not be under disband warning")
+        self.assertIsNone(self.guild._disband_date, "Guild should not have disband date")
+
+        GuildParser._parse_guild_guildhall(self.guild, content)
+        self.assertIsNotNone(self.guild._guildhall, "Guild should have guildhall")
+        self.assertEqual(self.guild._guildhall.name, "Sky Lane, Guild 1")
+        self.assertEqual(self.guild._guildhall.paid_until_date, datetime.date(2018, 8, 26))
 
-        self.guild._parse_guild_homepage(content)
+        GuildParser._parse_guild_homepage(self.guild, content)
         self.assertIsNotNone(self.guild.homepage, "Guild homepage must exist")
-        self.assertEqual("tibiammo.reddit.com", self.guild.homepage)
+        self.assertEqual("tibiammo.reddit.com", self.guild._homepage)
 
-        self.guild._parse_application_info(content)
-        self.assertTrue(self.guild.open_applications, "Guild should be open to applications")
+        GuildParser._parse_application_info(self.guild, content)
+        self.assertTrue(self.guild._open_applications, "Guild should be open to applications")
 
-        self.guild._parse_guild_info(content)
-        self.assertIsNotNone(self.guild.description, "Guild description must exist")
-        self.assertEqual("Gladera", self.guild.world)
-        self.assertEqual(datetime.date(2015, 7, 23), self.guild.founded)
-        self.assertTrue(self.guild.active, "Guild should be active")
+        GuildParser._parse_guild_info(self.guild, content)
+        self.assertIsNotNone(self.guild._description, "Guild description must exist")
+        self.assertEqual("Gladera", self.guild._world)
+        self.assertEqual(datetime.date(2015, 7, 23), self.guild._founded)
+        self.assertTrue(self.guild._active, "Guild should be active")
 
     def test_guild_from_content_minimum_info(self):
         """Testing parsing a guild with the minimum information possible"""
         content = self.load_parsed_resource(FILE_GUILD_INFO_MINIMUM)
-        self.guild._parse_guild_disband_info(content)
-        self.assertIsNone(self.guild.disband_condition, "Guild should not be under disband warning")
-        self.assertIsNone(self.guild.disband_date, "Guild should not have disband date")
-
-        self.guild._parse_guild_guildhall(content)
-        self.assertIsNone(self.guild.guildhall, "Guild should not have a guildhall")
-
-        self.guild._parse_guild_homepage(content)
-        self.assertIsNone(self.guild.homepage, "Guild should not have a guildhall")
-
-        self.guild._parse_guild_info(content)
-        self.assertIsNone(self.guild.description, "Guild description must not exist")
-        self.assertEqual("Gladera", self.guild.world)
-        self.assertEqual(datetime.date(year=2018, month=5, day=18), self.guild.founded)
+        GuildParser._parse_guild_disband_info(self.guild, content)
+        self.assertIsNone(self.guild._disband_condition, "Guild should not be under disband warning")
+        self.assertIsNone(self.guild._disband_date, "Guild should not have disband date")
+
+        GuildParser._parse_guild_guildhall(self.guild, content)
+        self.assertIsNone(self.guild._guildhall, "Guild should not have a guildhall")
+
+        GuildParser._parse_guild_homepage(self.guild, content)
+        self.assertIsNone(self.guild._homepage, "Guild should not have a guildhall")
+
+        GuildParser._parse_guild_info(self.guild, content)
+        self.assertIsNone(self.guild._description, "Guild description must not exist")
+        self.assertEqual("Gladera", self.guild._world)
+        self.assertEqual(datetime.date(year=2018, month=5, day=18), self.guild._founded)
 
     def test_guild_from_content_in_war(self):
         content = self.load_resource(FILE_GUILD_IN_WAR)
-        guild = Guild.from_content(content)
+        guild = GuildParser.from_content(content)
 
         self.assertIsInstance(guild, Guild)
         self.assertFalse(guild.open_applications)
         self.assertTrue(guild.active_war)
 
     def test_guild_from_content_disbanding(self):
         """Testing parsing a guild that is disbanding"""
         content = self.load_parsed_resource(FILE_GUILD_INFO_DISBANDING)
-        self.guild._parse_guild_info(content)
-        self.assertTrue(self.guild.active, "Guild should be active")
+        GuildParser._parse_guild_info(self.guild, content)
+        self.assertTrue(self.guild._active, "Guild should be active")
 
-        self.guild._parse_guild_disband_info(content)
-        self.assertIsNotNone(self.guild.disband_condition, "Guild should have a disband warning")
-        self.assertEqual(self.guild.disband_date, datetime.date(2018, 8, 17), "Guild should have disband date")
+        GuildParser._parse_guild_disband_info(self.guild, content)
+        self.assertIsNotNone(self.guild._disband_condition, "Guild should have a disband warning")
+        self.assertEqual(self.guild._disband_date, datetime.date(2018, 8, 17), "Guild should have disband date")
 
     def test_guild_from_content_formation(self):
         """Testing parsing a guild that is in formation"""
         content = self.load_parsed_resource(FILE_GUILD_INFO_FORMATION)
-        Guild._parse_guild_info(self.guild, content)
-        self.assertFalse(self.guild["active"], "Guild should not be active")
+        GuildParser._parse_guild_info(self.guild, content)
+        self.assertFalse(self.guild._active, "Guild should not be active")
 
-        Guild._parse_guild_disband_info(self.guild, content)
-        self.assertIsNotNone(self.guild.disband_condition, "Guild should have a disband warning")
-        self.assertEqual(self.guild.disband_date, datetime.date(2018, 8, 16), "Guild should have disband date")
+        GuildParser._parse_guild_disband_info(self.guild, content)
+        self.assertIsNotNone(self.guild._disband_condition, "Guild should have a disband warning")
+        self.assertEqual(self.guild._disband_date, datetime.date(2018, 8, 16), "Guild should have disband date")
 
     def test_listed_guild_from_content(self):
         """Testing parsing the list of guilds of a world"""
         content = self.load_resource(FILE_GUILD_LIST)
-        guilds_section = GuildsSection.from_content(content)
+        guilds_section = GuildsSectionParser.from_content(content)
         guilds = guilds_section.entries
 
         self.assertEqual(7, len(guilds_section.active_guilds))
         self.assertEqual(1, len(guilds_section.in_formation_guilds))
         self.assertEqual(55, len(guilds_section.available_worlds))
-        self.assertEqual(GuildsSection.get_url(guilds_section.world),guilds_section.url)
+        self.assertEqual(get_world_guilds_url(guilds_section.world), guilds_section.url)
         self.assertEqual("Zuna", guilds[0].world)
         self.assertTrue(guilds[0].active)
         self.assertFalse(guilds[-1].active)
 
     def test_listed_guild_from_content_not_found(self):
         """Testing parsing the guild list of a world that doesn't exist"""
         content = self.load_resource(FILE_GUILD_LIST_NOT_FOUND)
-        guilds_section = GuildsSection.from_content(content)
+        guilds_section = GuildsSectionParser.from_content(content)
         self.assertIsNotNone(guilds_section)
         self.assertIsNone(guilds_section.world)
         self.assertEqual(0, len(guilds_section.entries))
 
     def test_listed_guild_from_content_unrelated(self):
         """Testing parsing and unrelated section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            GuildsSection.from_content(content)
+            GuildsSectionParser.from_content(content)
 
-    def test_parse_invited_member_date(self):
-        """Testing the invitation date of a invited member"""
-        name = "Tschas"
-        date = "Invitation Date"
-        values = name, date
-        self.guild._parse_invited_member(values)
-        self.assertIsNotNone(self.guild.invites)
-        self.assertListEqual(self.guild.invites, [])
-
-    def test_parse_invited_member(self):
-        """Testing parsing an invited member"""
-        name = "Tschas"
-        date = "Jun 20 2018"
-        values = name, date
-        Guild._parse_invited_member(self.guild, values)
-        self.assertIsNotNone(self.guild.invites)
-        self.assertIsNotNone(self.guild.invites[0])
-        self.assertEqual(self.guild.invites[0].name, name)
-        self.assertEqual(self.guild.invites[0].date, datetime.date(2018, 6, 20))
-
-    def test_guild_member_init_join_date(self):
-        """Testing different combinations of join dates for instance creation"""
-        self.assertIsInstance(GuildMember(joined="Jul 20 2018").joined, datetime.date)
-        self.assertIsInstance(GuildMember(joined=datetime.date.today()).joined, datetime.date)
-        self.assertIsInstance(GuildMember(joined=datetime.datetime.now()).joined, datetime.date)
-        self.assertIsNone(GuildMember(joined=None).joined)
-        self.assertIsNone(GuildMember(joined="Jul 20").joined)
-
-    def test_guild_invite_init_invite_date(self):
-        """Testing different combinations of invite dates for instance creation"""
-        self.assertIsInstance(GuildInvite(date="Jul 20 2018").date, datetime.date)
-        self.assertIsInstance(GuildInvite(date=datetime.date.today()).date, datetime.date)
-        self.assertIsInstance(GuildInvite(date=datetime.datetime.now()).date, datetime.date)
-        self.assertIsNone(GuildInvite(date=None).date)
-        self.assertIsNone(GuildInvite(date="Jul 20").date)
-
-    def test_guild_init_founded(self):
-        """Testing different founded date inputs for instance creation"""
-        self.assertIsInstance(Guild(founded="Jul 20 2018").founded, datetime.date)
-        self.assertIsInstance(Guild(founded=datetime.date.today()).founded, datetime.date)
-        self.assertIsInstance(Guild(founded=datetime.datetime.now()).founded, datetime.date)
-        self.assertIsNone(Guild(founded=None).founded)
-        self.assertIsNone(Guild(founded="Jul 20").founded)
 
     # region Guild War Tests
     def test_guild_wars_from_content_active_history(self):
         """Testing parsing the guild wars of a guild currently in war and with war history."""
         content = self.load_resource(FILE_GUILD_WAR_ACTIVE_HISTORY)
-        guild_wars = GuildWars.from_content(content)
+        guild_wars = GuildWarsParser.from_content(content)
 
         self.assertIsInstance(guild_wars, GuildWars)
         self.assertEqual("Army Geddon", guild_wars.name)
         self.assertIsNotNone(guild_wars.current)
         self.assertEqual(guild_wars.name, guild_wars.current.guild_name)
         self.assertEqual(178, guild_wars.current.guild_score)
         self.assertEqual("Willyboiis Boys", guild_wars.current.opponent_name)
@@ -240,24 +200,24 @@
         self.assertEqual(491, guild_wars.history[1].opponent_score)
         self.assertEqual(500, guild_wars.history[1].score_limit)
         self.assertEqual(guild_wars.name, guild_wars.history[1].winner)
 
     def test_guild_wars_from_content_empty(self):
         """Testing parsing the guild wars of a guild that has never been in a war"""
         content = self.load_resource(FILE_GUILD_WAR_EMPTY)
-        guild_wars = GuildWars.from_content(content)
+        guild_wars = GuildWarsParser.from_content(content)
 
         self.assertEqual("Redd Alliance", guild_wars.name)
         self.assertIsNone(guild_wars.current)
         self.assertFalse(guild_wars.history)
 
     def test_guild_wars_from_content_unactive_history(self):
         """Testing parsing the guild wars of a war currently not in war and with war history."""
         content = self.load_resource(FILE_GUILD_WAR_UNACTIVE_HISTORY)
-        guild_wars = GuildWars.from_content(content)
+        guild_wars = GuildWarsParser.from_content(content)
 
         self.assertIsInstance(guild_wars, GuildWars)
         self.assertEqual("Dinastia de Perrones", guild_wars.name)
         self.assertIsNone(guild_wars.current)
 
         self.assertEqual(1, len(guild_wars.history))
```

### Comparing `tibia.py-5.6.0/tests/tests_highscores.py` & `tibia.py-6.0.0a1/tests/tests_highscores.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import datetime
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import Category, Highscores, HighscoresEntry, InvalidContent, LoyaltyHighscoresEntry, \
-    Vocation, VocationFilter, BattlEyeHighscoresFilter
+from tibiapy import HighscoresCategory, InvalidContent, \
+    Vocation, HighscoresProfession, HighscoresBattlEyeType
+from tibiapy.models import Highscores, HighscoresEntry, LoyaltyHighscoresEntry
+from tibiapy.parsers.highscores import HighscoresParser
 
 FILE_HIGHSCORES_FULL = "highscores/tibiacom_full.txt"
 FILE_HIGHSCORES_EXPERIENCE = "highscores/tibiacom_experience.txt"
 FILE_HIGHSCORES_LOYALTY = "highscores/tibiacom_loyalty.txt"
 FILE_HIGHSCORES_BATTLEYE_PVP_FILTER = "highscores/tibiacom_battleye_pvp_filters.txt"
 FILE_HIGHSCORES_EMPTY = "highscores/tibiacom_empty.txt"
 FILE_HIGHSCORES_NO_RESULTS = "highscores/tibiacom_no_results.txt"
 
 
 class TestHighscores(unittest.TestCase, TestCommons):
     # region Tibia.com Tests
     def test_highscores_from_content(self):
         """Testing parsing Highscores"""
         content = self.load_resource(FILE_HIGHSCORES_FULL)
-        highscores = Highscores.from_content(content)
+        highscores = HighscoresParser.from_content(content)
 
         self.assertEqual("Estela", highscores.world)
-        self.assertEqual(VocationFilter.KNIGHTS, highscores.vocation)
-        self.assertEqual(Category.MAGIC_LEVEL, highscores.category)
-        self.assertEqual(BattlEyeHighscoresFilter.ANY_WORLD, highscores.battleye_filter)
+        self.assertEqual(HighscoresProfession.KNIGHTS, highscores.vocation)
+        self.assertEqual(HighscoresCategory.MAGIC_LEVEL, highscores.category)
+        self.assertEqual(HighscoresBattlEyeType.ANY_WORLD, highscores.battleye_filter)
         self.assertEqual(1983, highscores.results_count)
         self.assertEqual(38, highscores.from_rank)
         self.assertEqual(38, highscores.to_rank)
-        self.assertEqual(4, highscores.page)
+        self.assertEqual(4, highscores.current_page)
         self.assertEqual(40, highscores.total_pages)
         self.assertIsNotNone(highscores.get_page_url(1))
         self.assertIsNotNone(highscores.url)
         self.assertIsNotNone(highscores.next_page_url)
         self.assertIsNotNone(highscores.previous_page_url)
         self.assertEqual(datetime.timedelta(minutes=6), highscores.last_updated)
 
@@ -43,19 +45,19 @@
             self.assertIsInstance(entry.value, int)
             self.assertIsInstance(entry.level, int)
             self.assertEqual("Estela", entry.world)
 
     def test_highscores_from_content_highscores(self):
         """Testing parsing experience highscores"""
         content = self.load_resource(FILE_HIGHSCORES_EXPERIENCE)
-        highscores = Highscores.from_content(content)
+        highscores = HighscoresParser.from_content(content)
 
         self.assertEqual(highscores.world, "Gladera")
-        self.assertEqual(highscores.vocation, VocationFilter.PALADINS)
-        self.assertEqual(highscores.category, Category.EXPERIENCE)
+        self.assertEqual(highscores.vocation, HighscoresProfession.PALADINS)
+        self.assertEqual(highscores.category, HighscoresCategory.EXPERIENCE)
         self.assertEqual(highscores.results_count, 1000)
         self.assertEqual(highscores.total_pages, 20)
 
         for entry in highscores.entries:
             self.assertIsInstance(entry, HighscoresEntry)
             self.assertIsInstance(entry.name, str)
             self.assertIsInstance(entry.vocation, Vocation)
@@ -63,19 +65,19 @@
             self.assertIsInstance(entry.value, int)
             self.assertIsInstance(entry.level, int)
             self.assertEqual(entry.world, "Gladera")
 
     def test_highscores_from_content_loyalty(self):
         """Testing parsing experience loyalty"""
         content = self.load_resource(FILE_HIGHSCORES_LOYALTY)
-        highscores = Highscores.from_content(content)
+        highscores = HighscoresParser.from_content(content)
 
         self.assertEqual("Calmera", highscores.world)
-        self.assertEqual(VocationFilter.PALADINS, highscores.vocation)
-        self.assertEqual(Category.LOYALTY_POINTS, highscores.category)
+        self.assertEqual(HighscoresProfession.PALADINS, highscores.vocation)
+        self.assertEqual(HighscoresCategory.LOYALTY_POINTS, highscores.category)
         self.assertEqual(1007, highscores.results_count)
         self.assertEqual(21, highscores.total_pages)
 
         for entry in highscores.entries:
             self.assertIsInstance(entry, LoyaltyHighscoresEntry)
             self.assertIsInstance(entry.name, str)
             self.assertIsInstance(entry.vocation, Vocation)
@@ -83,24 +85,24 @@
             self.assertIsInstance(entry.value, int)
             self.assertIsInstance(entry.level, int)
             self.assertIsInstance(entry.title, str)
 
     def test_highscores_from_content_battleye_and_pvp_filters(self):
         """Testing parsing Highscores"""
         content = self.load_resource(FILE_HIGHSCORES_BATTLEYE_PVP_FILTER)
-        highscores = Highscores.from_content(content)
+        highscores = HighscoresParser.from_content(content)
 
         self.assertEqual(None, highscores.world)
-        self.assertEqual(VocationFilter.ALL, highscores.vocation)
-        self.assertEqual(Category.EXPERIENCE, highscores.category)
-        self.assertEqual(BattlEyeHighscoresFilter.INITIALLY_PROTECTED, highscores.battleye_filter)
+        self.assertEqual(HighscoresProfession.ALL, highscores.vocation)
+        self.assertEqual(HighscoresCategory.EXPERIENCE, highscores.category)
+        self.assertEqual(HighscoresBattlEyeType.INITIALLY_PROTECTED, highscores.battleye_filter)
         self.assertEqual(1000, highscores.results_count)
         self.assertEqual(1, highscores.from_rank)
         self.assertEqual(50, highscores.to_rank)
-        self.assertEqual(1, highscores.page)
+        self.assertEqual(1, highscores.current_page)
         self.assertEqual(20, highscores.total_pages)
         self.assertEqual(3, len(highscores.pvp_types_filter))
         self.assertIsNotNone(highscores.url)
         self.assertEqual(datetime.timedelta(minutes=27), highscores.last_updated)
 
         for entry in highscores.entries:
             self.assertIsInstance(entry, HighscoresEntry)
@@ -109,30 +111,30 @@
             self.assertIsInstance(entry.rank, int)
             self.assertIsInstance(entry.value, int)
             self.assertIsInstance(entry.level, int)
 
     def test_highscores_from_content_empty(self):
         """Testing parsing highscores when empty (world doesn't exist)"""
         content = self.load_resource(FILE_HIGHSCORES_EMPTY)
-        highscores = Highscores.from_content(content)
+        highscores = HighscoresParser.from_content(content)
 
         self.assertIsNone(highscores)
 
     def _test_highscores_from_content_no_results(self):
         """Testing parsing highscores with no results (first day of a new world)"""
         content = self.load_resource(FILE_HIGHSCORES_NO_RESULTS)
-        highscores = Highscores.from_content(content)
+        highscores = HighscoresParser.from_content(content)
 
         self.assertIsInstance(highscores, Highscores)
         self.assertEqual(highscores.world, "Unica")
-        self.assertEqual(highscores.category, Category.EXPERIENCE)
-        self.assertEqual(highscores.vocation, VocationFilter.ALL)
+        self.assertEqual(highscores.category, HighscoresCategory.EXPERIENCE)
+        self.assertEqual(highscores.vocation, HighscoresProfession.ALL)
         self.assertEqual(highscores.total_pages, 0)
         self.assertEqual(len(highscores.entries), 0)
 
     def test_highscores_from_content_unrelated_section(self):
         """Testing parsing an unrelated section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            Highscores.from_content(content)
+            HighscoresParser.from_content(content)
 
     # endregion
```

### Comparing `tibia.py-5.6.0/tests/tests_house.py` & `tibia.py-6.0.0a1/tests/tests_house.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import datetime
 import json
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import House, HousesSection, InvalidContent, HouseEntry
+from tibiapy import InvalidContent
+from tibiapy.builders.house import HouseBuilder
 from tibiapy.enums import HouseOrder, HouseStatus, HouseType
+from tibiapy.models import House, HousesSection, HouseEntry
+from tibiapy.parsers.house import HouseParser, HousesSectionParser
+from tibiapy.urls import get_house_url
 
 FILE_HOUSE_FULL = "house/tibiacom_full.txt"
 FILE_HOUSE_STATUS_TRANSFER = "house/tibiacom_status_transfer.txt"
 FILE_HOUSE_STATUS_NO_BIDS = "house/tibiacom_status_no_bids.txt"
 FILE_HOUSE_STATUS_WITH_BIDS = "house/tibiacom_status_with_bids.txt"
 FILE_HOUSE_STATUS_RENTED = "house/tibiacom_status_rented.txt"
 FILE_HOUSE_NOT_FOUND = "house/tibiacom_not_found.txt"
@@ -17,89 +21,88 @@
 FILE_HOUSE_LIST_EMPTY = "house/tibiacom_list_empty.txt"
 
 
 class TestsHouse(TestCommons, unittest.TestCase):
     def test_house_from_content(self):
         """Testing parsing a house"""
         content = self.load_resource(FILE_HOUSE_FULL)
-        house = House.from_content(content)
+        house = HouseParser.from_content(content)
 
         self.assertIsInstance(house, House)
         self.assertEqual(house.name, "Sorcerer's Avenue Labs 2e")
         self.assertEqual(house.beds, 1)
         self.assertTrue(house.rent, 715)
         self.assertEqual(house.status, HouseStatus.AUCTIONED)
-        self.assertEqual(house.url, House.get_url(house.id, house.world))
+        self.assertEqual(house.url, get_house_url(house.world, house.id))
         self.assertIsNone(house.owner)
         self.assertIsNone(house.owner_url)
         self.assertIsNotNone(house.highest_bidder)
         self.assertIsNotNone(house.highest_bidder_url)
         self.assertEqual(house.highest_bid, 0)
 
-        house_json_raw = house.to_json()
+        house_json_raw = house.json()
         house_json = json.loads(house_json_raw)
         self.assertEqual(house.image_url, house_json["image_url"])
 
     def test_house_from_content_transferred(self):
         """Testing parsing a house being transferred"""
-        house = House("Name")
+        house = HouseBuilder().name("Name")
         content = self.load_resource(FILE_HOUSE_STATUS_TRANSFER)
-        house._parse_status(content)
-        self.assertEqual(house.status, HouseStatus.RENTED)
-        self.assertEqual(house.owner, "Xenaris mag")
-        self.assertEqual(house.transferee, "Ivarr Bezkosci")
-        self.assertIsNotNone(house.transferee_url)
-        self.assertTrue(house.transfer_accepted)
-        self.assertEqual(house.transfer_price, 850000)
+        HouseParser._parse_status(house, content)
+        self.assertEqual(house._status, HouseStatus.RENTED)
+        self.assertEqual(house._owner, "Xenaris mag")
+        self.assertEqual(house._transferee, "Ivarr Bezkosci")
+        self.assertTrue(house._transfer_accepted)
+        self.assertEqual(house._transfer_price, 850000)
 
     def test_house_parse_status_rented(self):
         """Testing parsing a rented status"""
-        house = House("Name")
+        house = HouseBuilder().name("Name")
         content = self.load_resource(FILE_HOUSE_STATUS_RENTED)
-        house._parse_status(content)
-        self.assertEqual(house.status, HouseStatus.RENTED)
-        self.assertEqual(house.owner, "Thorcen")
-        self.assertIsInstance(house.paid_until, datetime.datetime)
+        HouseParser._parse_status(house, content)
+        self.assertEqual(house._status, HouseStatus.RENTED)
+        self.assertEqual(house._owner, "Thorcen")
+        self.assertIsInstance(house._paid_until, datetime.datetime)
 
     def test_house_parse_status_with_bids(self):
         """Testing parsing a house status with bids"""
-        house = House("Name")
+        house = HouseBuilder().name("Name")
         content = self.load_resource(FILE_HOUSE_STATUS_WITH_BIDS)
-        house._parse_status(content)
-        self.assertEqual(house.status, HouseStatus.AUCTIONED)
-        self.assertIsNone(house.owner)
-        self.assertEqual(house.highest_bid, 15000)
-        self.assertEqual(house.highest_bidder, "King of Bosnia")
-        self.assertIsInstance(house.auction_end, datetime.datetime)
+        HouseParser._parse_status(house, content)
+        self.assertEqual(house._status, HouseStatus.AUCTIONED)
+        self.assertIsNone(house._owner)
+        self.assertEqual(house._highest_bid, 15000)
+        self.assertEqual(house._highest_bidder, "King of Bosnia")
+        self.assertIsInstance(house._auction_end, datetime.datetime)
 
     def test_house_parse_status_without_bids(self):
         """Testing parsing the status of a house with no bids"""
-        house = House("Name")
+        house = HouseBuilder().name("Name")
         content = self.load_resource(FILE_HOUSE_STATUS_NO_BIDS)
-        house._parse_status(content)
-        self.assertEqual(house.status, HouseStatus.AUCTIONED)
-        self.assertIsNone(house.auction_end)
+        HouseParser._parse_status(house, content)
+        self.assertEqual(house._status, HouseStatus.AUCTIONED)
+        self.assertIsNone(house._auction_end)
 
     def test_house_from_content_not_found(self):
         """Testing parsing a house that doesn't exist"""
         content = self.load_resource(FILE_HOUSE_NOT_FOUND)
-        house = House.from_content(content)
+        house = HouseParser.from_content(content)
 
         self.assertIsNone(house)
 
     def test_house_from_content_unrelated(self):
         """Testing parsing an unrelated section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            House.from_content(content)
+            HouseParser.from_content(content)
 
     def test_house_section_from_content(self):
         """Testing parsing the house list of a world and city"""
         content = self.load_resource(FILE_HOUSE_LIST)
-        house_results = HousesSection.from_content(content)
+        house_results = HousesSectionParser.from_content(content)
 
         self.assertIsInstance(house_results, HousesSection)
         self.assertEqual("Carlin", house_results.town)
         self.assertEqual("Alumbra", house_results.world)
         self.assertEqual(HouseStatus.RENTED, house_results.status)
         self.assertEqual(HouseType.HOUSE, house_results.house_type)
         self.assertEqual(HouseOrder.RENT, house_results.order)
@@ -114,30 +117,30 @@
         self.assertIsInstance(houses[0].id, int)
 
         self.assertEqual(houses[25].status, HouseStatus.RENTED)
 
     def test_house_section_from_content_empty(self):
         """Testing parsing an empty house list"""
         content = self.load_resource(FILE_HOUSE_LIST_EMPTY)
-        house_results = HousesSection.from_content(content)
+        house_results = HousesSectionParser.from_content(content)
 
         self.assertIsInstance(house_results, HousesSection)
         self.assertEqual("Edron", house_results.town)
         self.assertEqual("Antica", house_results.world)
         self.assertEqual(HouseStatus.AUCTIONED, house_results.status)
         self.assertEqual(HouseType.GUILDHALL, house_results.house_type)
         self.assertEqual(HouseOrder.RENT, house_results.order)
         self.assertEqual(len(house_results.entries), 0)
 
     def test_house_section_from_content_not_found(self):
         """Testing parsing an empty house list"""
         content = self.load_resource(FILE_HOUSE_LIST_NOT_FOUND)
-        results = HousesSection.from_content(content)
+        results = HousesSectionParser.from_content(content)
         self.assertIsInstance(results, HousesSection)
         self.assertEqual(0, len(results.entries))
 
     def test_house_section_from_content_unrelated(self):
         """Testing parsing an unrelated section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            HousesSection.from_content(content)
+            HousesSectionParser.from_content(content)
```

### Comparing `tibia.py-5.6.0/tests/tests_kill_statistics.py` & `tibia.py-6.0.0a1/tests/tests_kill_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import KillStatistics, InvalidContent
+from tibiapy import InvalidContent
+from tibiapy.parsers.kill_statistics import KillStatisticsParser
 
 FILE_KILL_STATISTICS_FULL = "kill_statistics/tibiacom_full.txt"
 FILE_KILL_STATISTICS_EMPTY = "kill_statistics/tibiacom_empty.txt"
 
 
 class TestHighscores(TestCommons, unittest.TestCase):
     # region Tibia.com Tests
     def test_kill_statistics_from_content(self):
         """Testing parsing kill statistics"""
         content = self.load_resource(FILE_KILL_STATISTICS_FULL)
-        kill_statistics = KillStatistics.from_content(content)
+        kill_statistics = KillStatisticsParser.from_content(content)
 
         self.assertEqual(kill_statistics.world, "Gladera")
         self.assertEqual(len(kill_statistics.entries), 920)
         self.assertIsNotNone(kill_statistics.total)
         self.assertIsNotNone(kill_statistics.url)
 
         # players shortcurt property
@@ -32,18 +33,18 @@
         self.assertEqual(1, demons_entry.last_day_players_killed)
         self.assertEqual(18484, demons_entry.last_week_killed)
         self.assertEqual(8, demons_entry.last_week_players_killed)
 
     def test_kill_statistics_from_content_empty(self):
         """Testing parsing empty kill statistics"""
         content = self.load_resource(FILE_KILL_STATISTICS_EMPTY)
-        kill_statistics = KillStatistics.from_content(content)
+        kill_statistics = KillStatisticsParser.from_content(content)
 
         self.assertIsNone(kill_statistics)
 
     def test_kill_statistics_from_content_unrelated_section(self):
         """Testing parsing an unrelated section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            KillStatistics.from_content(content)
+            KillStatisticsParser.from_content(content)
 
     # endregion
```

### Comparing `tibia.py-5.6.0/tests/tests_leaderboards.py` & `tibia.py-6.0.0a1/tests/tests_leaderboards.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import datetime
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import InvalidContent, Leaderboard, TournamentEntry, PvpType, RuleSet, ScoreSet, Tournament, \
-    TournamentLeaderboard, \
-    TournamentPhase
+from tibiapy import InvalidContent
+from tibiapy.parsers.leaderboard import LeaderboardParser
+from tibiapy.urls import get_leaderboards_url
 
 FILE_LEADERBOARD_CURRENT = "leaderboards/tibiacom_current_rotation.txt"
 
 
 class TestLeaderboards(TestCommons, unittest.TestCase):
     # region Leaderboard Tests
     def test_leaderboard_from_content(self):
         """Testing parsing a leaderboard's page"""
         content = self.load_resource(FILE_LEADERBOARD_CURRENT)
-        leaderboard = Leaderboard.from_content(content)
+        leaderboard = LeaderboardParser.from_content(content)
 
         self.assertIsNotNone(leaderboard)
         self.assertEqual("Antica", leaderboard.world)
         self.assertEqual(2, leaderboard.rotation.rotation_id)
         self.assertEqual(45, leaderboard.results_count)
         self.assertEqual(2, len(leaderboard.available_rotations))
         self.assertEqual(81, len(leaderboard.available_worlds))
@@ -32,14 +31,14 @@
         self.assertEqual(1, first_entry.rank)
         self.assertEqual(80, first_entry.drome_level)
 
     def test_leaderboard_from_content_unrelated_section(self):
         """Testing parsing a leaderboard's page"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            Leaderboard.from_content(content)
+            LeaderboardParser.from_content(content)
 
     def test_leaderboard_get_url_invalid_page(self):
         with self.assertRaises(ValueError):
-            Leaderboard.get_url("Antica", page=0)
+            get_leaderboards_url("Antica", page=0)
 
     # endregion
```

### Comparing `tibia.py-5.6.0/tests/tests_news.py` & `tibia.py-6.0.0a1/tests/tests_news.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,119 @@
 import datetime
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import NewsEntry, News, InvalidContent, NewsArchive
+from tibiapy import InvalidContent
 from tibiapy.enums import NewsCategory, NewsType
-
-FILE_NEWS_LIST = "news/tibiacom_list.txt"
-FILE_NEWS_LIST_EMPTY = "news/tibiacom_list_empty.txt"
-FILE_NEWS_EMPTY = "news/tibiacom_empty.txt"
-FILE_NEWS_ARTICLE = "news/tibiacom_news.txt"
-FILE_NEWS_TICKER = "news/tibiacom_news_ticker.txt"
+from tibiapy.models.news import NewsEntry, NewsArchive, News
+from tibiapy.parsers.news import NewsArchiveParser, NewsParser
+from tibiapy.urls import get_news_url
+
+FILE_NEWS_ARCHIVE_INITIAL = "news/news_archive_initial.txt"
+FILE_NEWS_ARCHIVE_RESULTS = "news/news_archive_results.txt"
+FILE_NEWS_ARCHIVE_EMPTY = "news/news_archive_empty.txt"
+FILE_NEWS_ARCHIVE_ERROR = "news/news_archive_error.txt"
+FILE_NEWS_NOT_FOUND = "news/news_not_found.txt"
+FILE_NEWS_ARTICLE = "news/news_article.txt"
+FILE_NEWS_TICKER = "news/news_ticker.txt"
 
 
 class TestNews(TestCommons, unittest.TestCase):
-    # region Tibia.com Tests
-    def test_news_archive_from_content(self):
-        """Testing parsing news"""
-        content = self.load_resource(FILE_NEWS_LIST)
-        news_archive = NewsArchive.from_content(content)
+    def test_news_archive_parser_from_content_initial(self):
+        """Test parsing the news archive initial page."""
+        content = self.load_resource(FILE_NEWS_ARCHIVE_INITIAL)
+
+        news_archive = NewsArchiveParser.from_content(content)
+
+        self.assertIsInstance(news_archive, NewsArchive)
+        self.assertEqual(datetime.date(2023, 3, 16), news_archive.start_date)
+        self.assertEqual(datetime.date(2023, 4, 15), news_archive.end_date)
+        self.assertEqual(3, len(news_archive.types))
+        self.assertEqual(5, len(news_archive.categories))
+
+    def test_news_archive_parser_from_content_with_results(self):
+        """Testing parsing the news archive with results."""
+        content = self.load_resource(FILE_NEWS_ARCHIVE_RESULTS)
+
+        news_archive = NewsArchiveParser.from_content(content)
 
         self.assertEqual(datetime.date(2019, 3, 25), news_archive.start_date)
         self.assertEqual(datetime.date(2019, 5, 25), news_archive.end_date)
         self.assertEqual(3, len(news_archive.types))
         self.assertEqual(5, len(news_archive.categories))
-
         news_list = news_archive.entries
         self.assertGreater(len(news_list), 0)
         latest_news = news_list[0]
         self.assertIsInstance(latest_news, NewsEntry)
         self.assertIsInstance(latest_news.id, int)
         self.assertIsInstance(latest_news.category, NewsCategory)
         self.assertIsInstance(latest_news.type, NewsType)
         self.assertIsInstance(latest_news.date, datetime.date)
         self.assertIsNotNone(latest_news.url)
-        self.assertEqual(latest_news.url, NewsEntry.get_url(latest_news.id))
+        self.assertEqual(latest_news.url, get_news_url(latest_news.id))
 
-    def test_news_archive_from_content_empty(self):
+    def test_news_archive_parser_from_content_empty(self):
         """Testing parsing a news article that doesn't exist"""
-        content = self.load_resource(FILE_NEWS_LIST_EMPTY)
-        news_archive = NewsArchive.from_content(content)
+        content = self.load_resource(FILE_NEWS_ARCHIVE_EMPTY)
 
-        self.assertEqual(datetime.date(2019, 5, 23), news_archive.start_date)
-        self.assertEqual(datetime.date(2019, 5, 25), news_archive.end_date)
+        news_archive = NewsArchiveParser.from_content(content)
+
+        self.assertEqual(datetime.date(2023, 4, 13), news_archive.start_date)
+        self.assertEqual(datetime.date(2023, 4, 15), news_archive.end_date)
         self.assertEqual(1, len(news_archive.types))
         self.assertEqual(5, len(news_archive.categories))
+        self.assertEqual(0, len(news_archive.entries))
+
+    def test_news_archive_parser_from_content_error(self):
+        """Testing parsing the news archive resulting in an error message."""
+        content = self.load_resource(FILE_NEWS_ARCHIVE_ERROR)
 
+        news_archive = NewsArchiveParser.from_content(content)
+
+        self.assertIsInstance(news_archive, NewsArchive)
+        self.assertEqual(datetime.date(2019, 3, 25), news_archive.start_date)
+        self.assertEqual(datetime.date(2018, 5, 25), news_archive.end_date)
+        self.assertEqual(3, len(news_archive.types))
+        self.assertEqual(5, len(news_archive.categories))
         self.assertEqual(0, len(news_archive.entries))
 
-    def test_news_archive_from_content_unrelated(self):
+    def test_news_archive_parser_from_content_unrelated(self):
         """Testing parsing an unrelated section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            NewsArchive.from_content(content)
+            NewsArchiveParser.from_content(content)
 
-    def test_news_from_content_empty(self):
+    def test_news_parser_from_content_empty(self):
         """Testing parsing an empty news article"""
-        content = self.load_resource(FILE_NEWS_EMPTY)
-        news = News.from_content(content)
+        content = self.load_resource(FILE_NEWS_NOT_FOUND)
+        news = NewsParser.from_content(content)
         self.assertIsNone(news)
 
-    def test_news_from_content_unrelated(self):
+    def test_news_parser_from_content_unrelated(self):
         """Testing parsing an unrelated section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            News.from_content(content)
+            NewsParser.from_content(content)
 
-    def test_news_from_content_ticker(self):
+    def test_news_parser_from_content_ticker(self):
         """Testing parsing a news ticker"""
         content = self.load_resource(FILE_NEWS_TICKER)
-        news = News.from_content(content)
+        news = NewsParser.from_content(content)
 
         self.assertIsInstance(news, News)
         self.assertEqual(news.category, NewsCategory.TECHNICAL_ISSUES)
         self.assertIsInstance(news.date, datetime.date)
         self.assertEqual(news.title, "News Ticker")
         self.assertIsNone(news.thread_id)
 
-    def test_news_from_content_article(self):
+    def test_news_parser_from_content_article(self):
         """Testing parsing an article"""
         content = self.load_resource(FILE_NEWS_ARTICLE)
-        news = News.from_content(content)
+        news = NewsParser.from_content(content)
 
         self.assertIsInstance(news, News)
         self.assertEqual(news.category, NewsCategory.DEVELOPMENT)
         self.assertIsInstance(news.date, datetime.date)
         self.assertEqual(news.title, "Sign Up for the VANGUARD Tournament")
         self.assertEqual(news.thread_id, 4725194)
 
-    # endregion
+
```

### Comparing `tibia.py-5.6.0/tests/tests_spell.py` & `tibia.py-6.0.0a1/tests/tests_spell.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import unittest
 
 import tibiapy
 from tests.tests_tibiapy import TestCommons
-from tibiapy import Spell, SpellsSection
+from tibiapy.parsers.spell import SpellsSectionParser, SpellParser
 
 FILE_SPELLS_SECTION = "library/spell_list_default.txt"
 FILE_SPELL_RUNE = "library/spell_rune.txt"
 FILE_SPELL_SECONDARY_GROUP = "library/spell_secondary_group.txt"
 
 
 class TestSpell(TestCommons, unittest.TestCase):
     # region Tibia.com Tests
     def test_spells_section_from_content(self):
         """Testing parsing a boosted creature"""
         content = self.load_resource(FILE_SPELLS_SECTION)
-        spells_section = SpellsSection.from_content(content)
+        spells_section = SpellsSectionParser.from_content(content)
 
         self.assertIsNotNone(spells_section)
         self.assertEqual(141, len(spells_section.entries))
 
     def test_spells_section_from_content_unrelated_section(self):
         """Testing parsing a boosted creature"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(tibiapy.InvalidContent):
-            spells_section = SpellsSection.from_content(content)
+            spells_section = SpellsSectionParser.from_content(content)
 
     def test_spell_from_content_rune(self):
         """Testing parsing a rune spell."""
         content = self.load_resource(FILE_SPELL_RUNE)
-        spell = Spell.from_content(content)
+        spell = SpellParser.from_content(content)
 
         self.assertIsNotNone(spell)
         self.assertEqual("Chameleon Rune", spell.name)
         self.assertEqual("adevo ina", spell.words)
         self.assertIn("Druid", spell.vocations)
         self.assertEqual("Support", spell.group.value)
         self.assertEqual("Rune", spell.spell_type.value)
@@ -52,15 +52,15 @@
         self.assertEqual("Support", spell.rune.group.value)
         self.assertEqual(27, spell.rune.exp_level)
         self.assertEqual(4, spell.rune.magic_level)
 
     def test_spell_from_content_secondary_group(self):
         """Testing parsing a spell with a secondary group."""
         content = self.load_resource(FILE_SPELL_SECONDARY_GROUP)
-        spell = Spell.from_content(content)
+        spell = SpellParser.from_content(content)
 
         self.assertIsNotNone(spell)
         self.assertEqual("Protector", spell.name)
         self.assertEqual("utamo tempo", spell.words)
         self.assertIn("Knight", spell.vocations)
         self.assertEqual("Support", spell.group.value)
         self.assertEqual("Focus", spell.group_secondary)
@@ -77,18 +77,18 @@
         self.assertTrue(spell.premium)
 
     def test_spells_from_content_unknown_spell(self):
         """Testing parsing an unknown spell
 
         When trying to fetch a spell that doesn't exist, the website will just show the spells section."""
         content = self.load_resource(FILE_SPELLS_SECTION)
-        spell = Spell.from_content(content)
+        spell = SpellParser.from_content(content)
 
         self.assertIsNone(spell)
 
     def test_spells_from_content_unrelated_section(self):
         """Testing parsing a boosted creature"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(tibiapy.InvalidContent):
-            spell = Spell.from_content(content)
+            spell = SpellParser.from_content(content)
 
     # endregion
```

### Comparing `tibia.py-5.6.0/tests/tests_tibiapy.py` & `tibia.py-6.0.0a1/tests/tests_tibiapy.py`

 * *Files identical despite different names*

### Comparing `tibia.py-5.6.0/tests/tests_utils.py` & `tibia.py-6.0.0a1/tests/tests_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 import unittest
 
-import tibiapy
 from tests.tests_tibiapy import TestCommons
 from tibiapy import enums, utils
 from tibiapy.utils import get_tibia_url, parse_integer, parse_tibia_money
 
 TIBIA_DATETIME_CEST = "Jul 10 2018, 07:13:32 CEST"
 TIBIA_DATETIME_CET = "Jan 10 2018, 07:13:32 CET"
 TIBIA_DATETIME_PST = "Aug 10 2015, 23:13:32 PST"
@@ -13,36 +12,14 @@
 
 TIBIA_DATE = "Jun 20 2018"
 TIBIA_FULL_DATE = "July 23, 2015"
 TIBIA_DATE_INVALID = "8 Nov 2018"
 
 
 class TestUtils(TestCommons, unittest.TestCase):
-    def test_serializable_get_item(self):
-        """Testing the muliple ways to use __get__ for Serializable"""
-        # Class inherits from Serializable
-        world = tibiapy.World("Calmera")
-
-        # Serializable allows accessing attributes like a dictionary
-        self.assertEqual(world.name, world["name"])
-        # And setting values too
-        world["location"] = tibiapy.enums.WorldLocation.NORTH_AMERICA
-        self.assertEqual(world.location, tibiapy.enums.WorldLocation.NORTH_AMERICA)
-
-        # Accessing via __get__ returns KeyError instead of AttributeError to follow dictionary behaviour
-        with self.assertRaises(KeyError):
-            _level = world["level"]  # NOSONAR
-
-        # Accessing an undefined attribute that is defined in __slots__ returns `None` instead of raising an exception.
-        del world.location
-        self.assertIsNone(world["location"])
-
-        # New attributes can't be created by assignation
-        with self.assertRaises(KeyError):
-            world["custom"] = "custom value"
 
     def test_parse_tibia_datetime(self):
         time = utils.parse_tibia_datetime(TIBIA_DATETIME_CEST)
         self.assertIsInstance(time, datetime.datetime)
         self.assertEqual(time.month, 7)
         self.assertEqual(time.day, 10)
         self.assertEqual(time.year, 2018)
@@ -114,22 +91,21 @@
         self.assertEqual(utils.parse_number_words("one hundred two"), 102)
         self.assertEqual(utils.parse_number_words("two thousand forty five"), 2045)
 
     def test_try_enum(self):
         self.assertEqual(utils.try_enum(enums.Sex, "male"), enums.Sex.MALE)
         self.assertEqual(utils.try_enum(enums.TransferType, "", enums.TransferType.REGULAR), enums.TransferType.REGULAR)
         self.assertEqual(utils.try_enum(enums.WorldLocation, enums.WorldLocation.EUROPE), enums.WorldLocation.EUROPE)
-        self.assertEqual(utils.try_enum(enums.VocationFilter, 4), enums.VocationFilter.SORCERERS)
-        self.assertEqual(utils.try_enum(enums.Category, "FISHING"), enums.Category.FISHING)
+        self.assertEqual(utils.try_enum(enums.HighscoresProfession, 4), enums.HighscoresProfession.SORCERERS)
+        self.assertEqual(utils.try_enum(enums.HighscoresCategory, "FISHING"), enums.HighscoresCategory.FISHING)
 
     def test_enum_str(self):
-        self.assertEqual(str(enums.Sex.MALE), enums.Sex.MALE.value)
-        self.assertEqual(enums.VocationFilter.from_name("royal paladin"), enums.VocationFilter.PALADINS)
-        self.assertEqual(enums.VocationFilter.from_name("unknown"), enums.VocationFilter.ALL)
-        self.assertIsNone(enums.VocationFilter.from_name("unknown", False))
+        self.assertEqual(enums.HighscoresProfession.from_name("royal paladin"), enums.HighscoresProfession.PALADINS)
+        self.assertEqual(enums.HighscoresProfession.from_name("unknown"), enums.HighscoresProfession.ALL)
+        self.assertIsNone(enums.HighscoresProfession.from_name("unknown", False))
 
     def test_parse_tibia_money(self):
         self.assertEqual(1000, parse_tibia_money("1k"))
         self.assertEqual(5000000, parse_tibia_money("5kk"))
         self.assertEqual(2500, parse_tibia_money("2.5k"))
         self.assertEqual(50, parse_tibia_money("50"))
         with self.assertRaises(ValueError):
```

### Comparing `tibia.py-5.6.0/tests/tests_world.py` & `tibia.py-6.0.0a1/tests/tests_world.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import datetime
 import json
 import unittest
 
 from tests.tests_tibiapy import TestCommons
-from tibiapy import InvalidContent, TournamentWorldType, World, WorldOverview
+from tibiapy import InvalidContent
 from tibiapy.enums import PvpType, TransferType, WorldLocation
-from tibiapy.world import WorldEntry
+from tibiapy.models.world import WorldOverview, WorldEntry, World
+from tibiapy.parsers.world import WorldOverviewParser, WorldParser
+from tibiapy.urls import get_world_url
 
 FILE_WORLD_FULL = "world/tibiacom_online.txt"
 FILE_WORLD_FULL_OFFLINE = "world/tibiacom_offline.txt"
 FILE_WORLD_TOURNAMENT = "world/tibiacom_tournament.txt"
 FILE_WORLD_NOT_FOUND = "world/tibiacom_not_found.txt"
 FILE_WORLD_LIST = "world/tibiacom_list_online.txt"
 FILE_WORLD_LIST_OFFLINE = "world/tibiacom_list_offline.txt"
@@ -17,122 +19,104 @@
 
 class TestWorld(TestCommons, unittest.TestCase):
 
     # region Tibia.com Tests
     def test_world_from_content_full(self):
         """Testing parsing a world with full information"""
         content = self.load_resource(FILE_WORLD_FULL)
-        world = World.from_content(content)
+        world = WorldParser.from_content(content)
 
         self.assertIsInstance(world, World)
         self.assertEqual(world.name, "Premia")
-        self.assertEqual(world.status, "Online")
+        self.assertTrue(world.online)
         self.assertEqual(world.record_count, 531)
         self.assertIsInstance(world.record_date, datetime.datetime)
         self.assertEqual(world.creation_date, "2002-04")
         self.assertEqual(world.creation_year, 2002)
         self.assertEqual(world.creation_month, 4)
         self.assertEqual(world.location, WorldLocation.EUROPE)
         self.assertEqual(world.pvp_type, PvpType.OPEN_PVP)
         self.assertEqual(world.transfer_type, TransferType.REGULAR)
         self.assertEqual(len(world.world_quest_titles), 4)
         self.assertTrue(world.premium_only)
         self.assertTrue(world.battleye_protected)
         self.assertEqual(world.battleye_date, datetime.date(2017, 9, 5))
         self.assertFalse(world.experimental)
         self.assertEqual(len(world.online_players), world.online_count)
-        self.assertEqual(World.get_url(world.name), world.url)
+        self.assertEqual(get_world_url(world.name), world.url)
 
-        world_json_raw = world.to_json()
+        world_json_raw = world.json()
         world_json = json.loads(world_json_raw)
         self.assertEqual(len(world.online_players), len(world_json["online_players"]))
 
     def test_world_from_content_offline(self):
         """Testing parsing an offline world"""
-        content = self.load_resource(FILE_WORLD_FULL_OFFLINE, )
-        world = World.from_content(content)
+        content = self.load_resource(FILE_WORLD_FULL_OFFLINE)
+        world = WorldParser.from_content(content)
 
         self.assertIsInstance(world, World)
         self.assertEqual(world.name, "Antica")
-        self.assertEqual(world.status, "Offline")
+        self.assertFalse(world.online)
         self.assertEqual(world.record_count, 1052)
         self.assertIsInstance(world.record_date, datetime.datetime)
         self.assertEqual(world.creation_date, "1997-01")
         self.assertEqual(world.creation_year, 1997)
         self.assertEqual(world.creation_month, 1)
         self.assertEqual(world.location, WorldLocation.EUROPE)
         self.assertEqual(world.pvp_type, PvpType.OPEN_PVP)
         self.assertEqual(world.transfer_type, TransferType.REGULAR)
         self.assertEqual(len(world.world_quest_titles), 5)
         self.assertFalse(world.premium_only)
         self.assertTrue(world.battleye_protected)
         self.assertEqual(world.battleye_date, datetime.date(2017, 8, 29))
         self.assertFalse(world.experimental)
         self.assertEqual(len(world.online_players), world.online_count)
-        self.assertEqual(World.get_url(world.name), world.url)
+        self.assertEqual(get_world_url(world.name), world.url)
 
     def test_world_from_content_not_found(self):
         """Testing parsing a world that doesn't exist"""
         content = self.load_resource(FILE_WORLD_NOT_FOUND)
-        world = World.from_content(content)
+        world = WorldParser.from_content(content)
 
         self.assertIsNone(world)
 
     def test_world_from_content_unrelated_section(self):
         """Testing parsing a world using an unrelated section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            World.from_content(content)
+            WorldParser.from_content(content)
 
-    def test_world_from_content_tournament(self):
-        """Testing parsing a tournament world"""
-        content = self.load_resource(FILE_WORLD_TOURNAMENT)
-        world = World.from_content(content)
-
-        self.assertIsInstance(world, World)
-        self.assertIsInstance(world.tournament_world_type, TournamentWorldType)
-        self.assertEqual(world.tournament_world_type, TournamentWorldType.REGULAR)
-        self.assertEqual(world.record_count, 21)
-        self.assertTrue(world.premium_only)
-        self.assertFalse(world.world_quest_titles)
 
     # endregion
 
     # region Tibia.com WorldOverview Tests
-    def _test_world_overview_from_content(self):
+    def test_world_overview_from_content(self):
         """Testing parsing world overview"""
         content = self.load_resource(FILE_WORLD_LIST)
-        world_overview = WorldOverview.from_content(content)
+        world_overview = WorldOverviewParser.from_content(content)
 
         self.assertIsInstance(world_overview, WorldOverview)
-        self.assertEqual(WorldOverview.get_url(), WorldEntry.get_list_url())
         self.assertGreater(len(world_overview.worlds), 0)
         self.assertGreater(world_overview.total_online, 0)
         self.assertIsNotNone(world_overview.record_date)
         self.assertIsNotNone(world_overview.record_count)
-        self.assertEqual(82, len(world_overview.regular_worlds))
-        self.assertEqual(6, len(world_overview.tournament_worlds))
-
-        worlds = WorldEntry.list_from_content(content)
-        self.assertEqual(len(world_overview.worlds), len(worlds))
 
-    # TODO: Enable when we have a sample again
-    def _test_world_overview_from_content_offline(self):
+    def test_world_overview_from_content_offline(self):
         """Testing parsing world overview with offline worlds"""
         content = self.load_resource(FILE_WORLD_LIST_OFFLINE)
-        world_overview = WorldOverview.from_content(content)
+        world_overview = WorldOverviewParser.from_content(content)
 
         self.assertEqual(world_overview.record_count, 64028)
         self.assertIsInstance(world_overview.record_date, datetime.datetime)
         self.assertGreater(len(world_overview.worlds), 0)
         self.assertIsInstance(world_overview.worlds[0], WorldEntry)
         self.assertIsInstance(world_overview.worlds[0].pvp_type, PvpType)
         self.assertIsInstance(world_overview.worlds[0].transfer_type, TransferType)
         self.assertIsInstance(world_overview.worlds[0].location, WorldLocation)
         self.assertIsInstance(world_overview.worlds[0].online_count, int)
 
     def test_world_overview_from_content_unrelated(self):
         """Testing parsing an unrealted tibia section"""
         content = self.load_resource(self.FILE_UNRELATED_SECTION)
         with self.assertRaises(InvalidContent):
-            WorldEntry.list_from_content(content)
+            WorldOverviewParser.from_content(content)
     # endregion
```

### Comparing `tibia.py-5.6.0/tibia.py.egg-info/PKG-INFO` & `tibia.py-6.0.0a1/tibia.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibia.py
-Version: 5.6.0
+Version: 6.0.0a1
 Summary: API that parses website content into python data.
 Home-page: https://github.com/Galarzaa90/tibia.py
 Author: Galarzaa90
 Author-email: allan.galarza@gmail.com
 License: Apache 2.0
 Project-URL: GitHub: Repo, https://github.com/Galarzaa90/tibia.py
 Project-URL: GitHub: Issues, https://github.com/Galarzaa90/tibia.py/issues
@@ -17,28 +17,28 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Games/Entertainment :: Role-Playing
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: server
 License-File: LICENSE
 
 # Tibia.py
 An API to parse Tibia.com content into object oriented data.
 
 No fetching is done by this module, you must provide the html content.
 
@@ -80,27 +80,27 @@
 ```python
 import tibiapy
 
 # Asynchronously
 import aiohttp
 
 async def get_character(name):
-    url = tibiapy.Character.get_url(name)
+    url = tibiapy.urls.get_character_url(name)
 
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as resp:
             content = await resp.text()
     character = tibiapy.Character.from_content(content)
     return character
 
 # Synchronously
 import requests
 
 def get_character_sync(name):
-    url = tibiapy.Character.get_url(name)
+    url = tibiapy.urls.get_character_url(name)
     
     r = requests.get(url)
     content = r.text
     character = tibiapy.Character.from_content(content)
     return character
 
 ```
```

### Comparing `tibia.py-5.6.0/tibiapy/abc.py` & `tibia.py-6.0.0a1/tibiapy/urls.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,703 +1,626 @@
-"""Base classes shared by various models."""
 from __future__ import annotations
 
-import abc
 import datetime
-import enum
-import json
-from collections import OrderedDict
-from typing import Callable, TYPE_CHECKING
+import urllib.parse
+from typing import Optional, TYPE_CHECKING
 
-from tibiapy.utils import get_tibia_url
+from tibiapy import HighscoresCategory, HighscoresProfession, HighscoresBattlEyeType, PvpTypeFilter
 
 if TYPE_CHECKING:
-    from tibiapy import PvpType, WorldLocation
+    from tibiapy.models import AuctionFilters
+    from tibiapy import BazaarType, HouseType, HouseStatus, HouseOrder, SpellVocationFilter, \
+        SpellGroup, SpellType, SpellSorting
 
 
-class Serializable:
-    """Contains methods to make a class convertible to JSON.
+def get_tibia_url(section, subtopic=None, *args, anchor=None, test=False, **kwargs):
+    """Build a URL to Tibia.com with the given parameters.
 
-    Only attributes defined in ``__slots__`` will be serialized.
+    Parameters
+    ----------
+    section: :class:`str`
+        The desired section (e.g. community, abouttibia, manual, library)
+    subtopic: :class:`str`, optional
+        The desired subtopic (e.g. characters, guilds, houses, etc)
+    anchor: :class:`str`
+        A link anchor to add to the link.
+    args:
+        A list of key-value pairs to add as query parameters.
+        This allows passing multiple parameters with the same name.
+    kwargs:
+        Additional parameters to pass to the url as query parameters (e.g name, world, houseid, etc)
+    test: :class:`bool`
+        Whether to use the test website or not.
+
+    Returns
+    -------
+    :class:`str`
+        The generated Tibia.com URL.
+
+    Examples
+    --------
+    >>> get_tibia_url("community", "houses", page="view", houseid=55302, world="Gladera")
+    https://www.tibia.com/community/?subtopic=houses&page=view&houseid=55302&world=Gladera
+
+    You can also build a dictionary and pass it like:
+
+    >>> params = {'world': "Gladera"}
+    >>> get_tibia_url("community", "worlds", **params)
+    https://www.tibia.com/community/?subtopic=worlds&world=Gladera
+    """
+    base_url = "www.tibia.com" if not test else "www.test.tibia.com"
+    url = f"https://{base_url}/{section}/?"
+    params = {'subtopic': subtopic} if subtopic else {}
+    if kwargs:
+        for key, value in kwargs.items():
+            if isinstance(value, str):
+                value = value.encode('iso-8859-1')
+            if value is None:
+                continue
+            params[key] = value
+    url += urllib.parse.urlencode(params)
+    if args:
+        url += "&"
+        url += urllib.parse.urlencode(args)
+    if anchor:
+        url += f"#{anchor}"
+    return url
 
-    .. note::
-        | There's no way to convert JSON strings back to their original object.
-        | Attempting to do so may result in data loss.
-    """
 
-    _serializable_properties = ()
-    """:class:`tuple` of :class:`str`: Additional properties to serialize."""
+def get_static_file_url(*path: str) -> str:
+    """Build a URL to a static file in Tibia.com
 
-    @classmethod
-    def __slots_inherited__(cls):
-        slots = []
-        for base in cls.__bases__:
-            try:
-                # noinspection PyUnresolvedReferences
-                slots.extend(base.__slots_inherited__())
-            except AttributeError:
-                continue
-        slots.extend(getattr(cls, "__slots__", []))
-        slots.extend(getattr(cls, "_serializable_properties", []))
-        return tuple(OrderedDict.fromkeys(slots))
-
-    def keys(self):
-        return list(self.__slots_inherited__())
-
-    def __getitem__(self, item):
-        if item in self.keys():
-            try:
-                return getattr(self, item)
-            except AttributeError:
-                return None
-        else:
-            raise KeyError(item)
-
-    def __setitem__(self, key, value):
-        if key in self.keys():
-            setattr(self, key, value)
-        else:
-            raise KeyError(key)
-
-    @staticmethod
-    def _try_dict(obj):
-        try:
-            if isinstance(obj, datetime.datetime):
-                return obj.isoformat()
-            if isinstance(obj, datetime.timedelta):
-                return int(obj.total_seconds())
-            if isinstance(obj, enum.Flag):
-                return [str(i) for i in obj]
-            if isinstance(obj, enum.Enum):
-                return str(obj)
-            return {k: v for k, v in dict(obj).items() if v is not None}
-        except TypeError:
-            return str(obj)
-
-    def to_json(self, *, indent=None, sort_keys=False):
-        """Get the object's JSON representation.
-
-        Parameters
-        ----------
-        indent: :class:`int`, optional
-            Number of spaces used as indentation, :obj:`None` will return the shortest possible string.
-        sort_keys: :class:`bool`, optional
-            Whether keys should be sorted alphabetically or preserve the order defined by the object.
-
-        Returns
-        -------
-        :class:`str`
-            JSON representation of the object.
-        """
-        return json.dumps({k: v for k, v in dict(self).items() if v is not None}, indent=indent, sort_keys=sort_keys,
-                          default=self._try_dict)
-
-
-class BaseAnnouncement(metaclass=abc.ABCMeta):
-    """Base class for all announcement classes.
+    Parameters
+    ----------
+    path:
+        The path to the static file.
+
+    Examples
+    --------
+    >>> get_static_file_url("images", "global", "content", "newsicon_community_big.gif")
+    https://static.tibia.com/images/global/content/newsicon_community_big.gif
 
-    Implement common properties and methods for announcements.
+    """
+    return urllib.parse.urljoin("https://static.tibia.com/", "/".join(path))
 
-    The following implement this class:
 
-    - :class:`.ForumAnnouncement`
-    - :class:`.AnnouncementEntry`
+def get_character_url(name: str) -> str:
+    """Get the URL to a character in Tibia.com
 
-    Attributes
+    Parameters
     ----------
-    announcement_id: :class:`int`
-        The ID of the announcement.
+    name: :class:`str`
+        The name of the character.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the character's page in Tibia.com.
     """
+    return get_tibia_url("community", "characters", name=name)
 
-    announcement_id: int
-    __slots__ = (
-        "announcement_id",
-    )
 
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return other.announcement_id == self.announcement_id
-        return False
+def get_world_guilds_url(world: str) -> str:
+    """Get the URL to guild list of a specific world.
 
-    @property
-    def url(self):
-        """:class:`str` Get the URL to this announcement."""
-        return self.get_url(self.announcement_id)
+    Parameters
+    ----------
+    world: :class:`str`
+        The name of the world.
 
-    @classmethod
-    def get_url(cls, announcement_id):
-        """Get the URL to an announcement with a given ID.
+    Returns
+    -------
+    :class:`str`
+        The URL to the guild list's page in Tibia.com.
+    """
+    return get_tibia_url("community", "guilds", world=world)
 
-        Parameters
-        ----------
-        announcement_id: :class:`int`
-            The ID of the announcement
 
-        Returns
-        -------
-        :class:`str`
-            The URL of the announcement.
-        """
-        return get_tibia_url("forum", None, action="announcement", announcementid=announcement_id)
+def get_guild_url(name: str) -> str:
+    """Get the URL to a guild's page.
 
+    Parameters
+    ----------
+    name: :class:`str`
+        The name of the guild.
 
-class BaseBoard(metaclass=abc.ABCMeta):
-    """Base class for all board classes.
+    Returns
+    -------
+    :class:`str`
+        The URL to the guild's page in Tibia.com.
+    """
+    return get_tibia_url("community", "guilds", page="view", GuildName=name)
 
-    Implements common properties and methods for boards.
 
-    The following implement this class:
+def get_guild_wars_url(name: str) -> str:
+    """Get the Tibia.com URL for the guild wars of a guild with a given name.
 
-    - :class:`.ForumBoard`
-    - :class:`.BoardEntry`
+    Parameters
+    ------------
+    name: :class:`str`
+        The name of the guild.
 
-    Attributes
-    ----------
-    board_id: :class:`int`
-        The ID of the board.
+    Returns
+    --------
+    :class:`str`
+        The URL to the guild's wars page.
     """
+    return get_tibia_url("community", "guilds", page="guildwars", action="view", GuildName=name)
 
-    __slots__ = (
-        "board_id",
-    )
-
-    def __eq__(self, o: object) -> bool:
-        """Two boards are considered equal if their ids are equal."""
-        if isinstance(o, self.__class__):
-            return self.board_id == o.board_id
-        return False
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} board_id={self.board_id!r}>"
-
-    @property
-    def url(self):
-        """:class:`str`: The URL of this board."""
-        return self.get_url(self.board_id)
-
-    @classmethod
-    def get_url(cls, board_id, page=1, age=30):
-        """Get the Tibia.com URL to a board with a given id.
-
-        Parameters
-        ----------
-        board_id: :class:`int`
-            The ID of the board.
-        page: :class:`int`
-            The page to go to.
-        age: :class:`int`
-            The age in days of the threads to display.
-
-        Returns
-        -------
-        :class:`str`
-            The URL to the board.
-        """
-        return get_tibia_url("forum", None, action="board", boardid=board_id, pagenumber=page, threadage=age)
-
-    @classmethod
-    def get_world_boards_url(cls):
-        """Get the URL to the World Boards section in Tibia.com.
-
-        Returns
-        -------
-        :class:`str`:
-            The URL to the World Boards.
-        """
-        return get_tibia_url("forum", "worldboards")
-
-    @classmethod
-    def get_trade_boards_url(cls):
-        """Get the URL to the Trade Boards section in Tibia.com.
-
-        Returns
-        -------
-        :class:`str`:
-            The URL to the Trade Boards.
-        """
-        return get_tibia_url("forum", "tradeboards")
-
-    @classmethod
-    def get_community_boards_url(cls):
-        """Get the URL to the Community Boards section in Tibia.com.
-
-        Returns
-        -------
-        :class:`str`:
-            The URL to the Community Boards.
-        """
-        return get_tibia_url("forum", "communityboards")
-
-    @classmethod
-    def get_support_boards_url(cls):
-        """Get the URL to the Support Boards section in Tibia.com.
-
-        Returns
-        -------
-        :class:`str`:
-            The URL to the Support Boards.
-        """
-        return get_tibia_url("forum", "supportboards")
-
-
-class BaseCharacter(metaclass=abc.ABCMeta):
-    """Base class for all character classes.
-
-    Implements common properties methods for characters.
-
-    The following implement this class:
-
-    - :class:`.Character`
-    - :class:`.GuildInvite`
-    - :class:`.GuildMember`
-    - :class:`.HighscoresEntry`
-    - :class:`.TournamentLeaderboardEntry`
-    - :class:`.OnlineCharacter`
-    - :class:`.OtherCharacter`
-    - :class:`.AuctionEntry`
-    - :class:`.Auction`
 
-    Attributes
+def get_house_url(world: str, house_id: int) -> str:
+    """Get the URL to a house's page in Tibia.com.
+
+    Parameters
     ----------
-    name: :class:`str`
-        The name of the character.
+    world: :class:`str`
+        The world where the house is located.
+    house_id: :class:`int`
+        The ID of the house.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the house's page in Tibia.com.
     """
+    return get_tibia_url("community", "houses", page="view", houseid=house_id, world=world)
 
-    __slots__ = (
-        "name",
-    )
-
-    def __eq__(self, o: object) -> bool:
-        """Two characters are considered equal if their names are equal."""
-        if isinstance(o, self.__class__):
-            return self.name.lower() == o.name.lower()
-        return False
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name!r}>"
-
-    @property
-    def url(self):
-        """:class:`str`: The URL of the character's information page on Tibia.com."""
-        return self.get_url(self.name)
-
-    @classmethod
-    def get_url(cls, name):
-        """Get the Tibia.com URL for a given character name.
-
-        Parameters
-        ------------
-        name: :class:`str`
-            The name of the character.
-
-        Returns
-        --------
-        :class:`str`
-            The URL to the character's page.
-        """
-        return get_tibia_url("community", "characters", name=name)
-
-
-class BaseGuild(metaclass=abc.ABCMeta):
-    """Base class for Guild classes.
-
-    The following implement this class:
-
-    - :class:`.Guild`
-    - :class:`.GuildMembership`
-    - :class:`.GuildEntry`
 
-    Attributes
-    ----------
-    name: :class:`str`
-        The name of the guild.
+def get_world_overview_url() -> str:
+    """Get the URL to world overview section in Tibia.com
+
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the world overview section in Tibia.com.
     """
+    return get_tibia_url("community", "worlds")
 
-    __slots__ = (
-        "name",
-    )
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name!r}>"
-
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.name == other.name
-        return False
-
-    @property
-    def url(self):
-        """:class:`str`: The URL to the guild's information page on Tibia.com."""
-        return self.get_url(self.name)
-
-    @property
-    def url_wars(self):
-        """:class:`str` The URL to the guild's wars page on Tibia.com.
-
-        .. versionadded:: 3.0.0
-        """
-        return self.get_url_wars(self.name)
-
-    @classmethod
-    def get_url(cls, name):
-        """Get the Tibia.com URL for a given guild name.
-
-        Parameters
-        ------------
-        name: :class:`str`
-            The name of the guild.
-
-        Returns
-        --------
-        :class:`str`
-            The URL to the guild's page.
-        """
-        return get_tibia_url("community", "guilds", page="view", GuildName=name)
-
-    @classmethod
-    def get_url_wars(cls, name):
-        """Get the Tibia.com URL for the guild wars of a guild with a given name.
-
-        .. versionadded:: 3.0.0
-
-        Parameters
-        ------------
-        name: :class:`str`
-            The name of the guild.
-
-        Returns
-        --------
-        :class:`str`
-            The URL to the guild's wars page.
-        """
-        return get_tibia_url("community", "guilds", page="guildwars", action="view", GuildName=name)
-
-
-class BaseHouse(metaclass=abc.ABCMeta):
-    """Base class for all house classes.
-
-    The following implement this class:
-
-    - :class:`.House`
-    - :class:`.GuildHouse`
-    - :class:`.CharacterHouse`
-    - :class:`.HouseEntry`
 
-    Attributes
+def get_world_url(name: str) -> str:
+    """Get the URL to the World's information page on Tibia.com.
+
+    Parameters
     ----------
     name: :class:`str`
-        The name of the house.
+        The name of the world.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the world's information page.
     """
+    return get_tibia_url("community", "worlds", world=name.title())
 
-    __slots__ = (
-        "name",
-    )
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name!r}>"
+def get_news_archive_url() -> str:
+    """Get the URL to Tibia.com's news archive page.
 
-    def __eq__(self, o: object) -> bool:
-        """Two houses are considered equal if their names are equal."""
-        if isinstance(o, self.__class__):
-            return self.name.lower() == o.name.lower()
-        return False
+    Notes
+    -----
+    It is not possible to perform a search using query parameters.
+    News searches can only be performed using POST requests sending the parameters as form-data.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the news archive page.
+    """
+    return get_tibia_url("news", "newsarchive")
 
-    @classmethod
-    def get_url(cls, house_id, world):
-        """Get the Tibia.com URL for a house with the given id and world.
 
-        Parameters
-        ----------
-        house_id: :class:`int`
-            The internal id of the house.
-        world: :class:`str`
-            The world of the house.
+def get_news_url(news_id: int) -> str:
+    """Get the URL to a news article.
 
-        Returns
-        -------
-        The URL to the house in Tibia.com
-        """
-        return get_tibia_url("community", "houses", page="view", houseid=house_id, world=world)
+    Parameters
+    ----------
+    news_id: :class:`int`
+        The ID of the article.
 
+    Returns
+    -------
+    :class:`str`
+        The URL to the article's page on Tibia.com
+    """
+    return get_tibia_url("news", "newsarchive", id=news_id)
 
-class BaseNews(metaclass=abc.ABCMeta):
-    """Base class for all news classes.
 
-    Implements the :py:attr:`id` attribute and common properties.
+def get_forum_section_url(section_id: int) -> str:
+    """Get the URL to a forum section in Tibia.com.
 
-    The following implement this class:
+    Parameters
+    ----------
+    section_id: :class:`int`
+        The ID of the section.
 
-    - :class:`.News`
-    - :class:`.NewsEntry`
+    Returns
+    -------
+    :class:`str`
+        The URL to forum section.
+    """
+    return get_tibia_url("forum", action="main", sectionid=section_id)
 
-    Attributes
+
+def get_forum_section_url_by_name(section_name: str) -> str:
+    """Get the URL to a forum section in Tibia.com by its name.
+
+    Parameters
     ----------
-    id: :class:`int`
-        The internal ID of the news entry.
+    section_name: :class:`str`
+        The name of the section.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to forum section.
     """
+    return get_tibia_url("forum", section_name)
+
+
+def get_forum_board_url(board_id: int, page: int = 1, thread_age: int = None) -> str:
+    """Get the URL to a forum board.
 
-    __slots__ = (
-        "id",
-    )
+    Parameters
+    ----------
+    board_id: :class:`int`
+        The ID of the board.
+    page: :class:`int`
+        The page to display.
+    thread_age: :class:`int`
+        The maximum age in days for the threads to be shown.
 
-    def __eq__(self, o: object) -> bool:
-        """Two news articles are considered equal if their names or ids are equal."""
-        if isinstance(o, self.__class__):
-            return self.id == o.id
-        return False
+        ``-1`` means any age.
 
-    @property
-    def url(self):
-        """:class:`str`: The URL to the Tibia.com page of the news entry."""
-        return self.get_url(self.id)
+    Returns
+    -------
+    :class:`str`
+        The URL to forum board.
+    """
+    return get_tibia_url("forum", None, action="board", boardid=board_id, pagenumber=page, threadage=thread_age)
 
-    @classmethod
-    def get_url(cls, news_id):
-        """Get the Tibia.com URL for a news entry by its id.
 
-        Parameters
-        ------------
-        news_id: :class:`int`
-            The id of the news entry.
+def get_forum_announcement_url(announcement_id: int) -> str:
+    """Get the URL to a forum announcement.
 
-        Returns
-        --------
-        :class:`str`
-            The URL to the news' page
-        """
-        return get_tibia_url("news", "newsarchive", id=news_id)
+    Parameters
+    ----------
+    announcement_id: :class:`int`
+        The ID of the announcement.
 
-    @classmethod
-    def get_list_url(cls):
-        """Get the URL to Tibia.com's news archive page.
+    Returns
+    -------
+    :class:`str`
+        The URL to forum announcement.
+    """
+    return get_tibia_url("forum", None, action="announcement", announcementid=announcement_id)
 
-        Notes
-        -----
-        It is not possible to perform a search using query parameters.
-        News searches can only be performed using POST requests sending the parameters as form-data.
 
-        Returns
-        -------
-        :class:`str`
-            The URL to the news archive page on Tibia.com.
-        """
-        return get_tibia_url("news", "newsarchive")
+def get_forum_thread_url(thread_id: int, page: int = 1) -> str:
+    """Get the URL to a forum board.
 
+    Parameters
+    ----------
+    thread_id: :class:`int`
+        The ID of the thread.
+    page: :class:`int`
+        The page to display.
 
-class BasePost(metaclass=abc.ABCMeta):
-    """Base classs for post classes.
+    Returns
+    -------
+    :class:`str`
+        The URL to forum thread.
+    """
+    return get_tibia_url("forum", None, action="thread", threadid=thread_id, pagenumber=page)
 
-    The following implement this class:
 
-    - :class:`.CMPost`
-    - :class:`.ForumPost`
-    - :class:`.LastPost`
+def get_forum_post_url(post_id):
+    """Get the URL to a specific post.
 
-    Attributes
+    Parameters
     ----------
     post_id: :class:`int`
-        The internal ID of the post.
+        The ID of the desired post.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the post.
     """
+    return get_tibia_url("forum", None, anchor=f"post{post_id}", action="thread", postid=post_id)
 
-    __slots__ = (
-        "post_id",
-    )
 
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.post_id == other.post_id
-        return False
+def get_highscores_url(world: str = None, category: HighscoresCategory = HighscoresCategory.EXPERIENCE,
+                       vocation: HighscoresProfession = HighscoresProfession.ALL, page=1,
+                       battleye_type: HighscoresBattlEyeType = None, pvp_types: PvpTypeFilter = None
+                       ) -> str:
+    """Get the Tibia.com URL of the highscores for the given parameters.
+
+    Parameters
+    ----------
+    world: :class:`str`, optional
+        The game world of the desired highscores. If no world is passed, ALL worlds are shown.
+    category: :class:`.HighscoresCategory`
+        The desired highscores category.
+    vocation: :class:`.HighscoresProfession`
+        The vocation filter to apply. By default, all vocations will be shown.
+    page: :class:`int`
+        The page of highscores to show.
+    battleye_type: :class:`.HighscoresBattlEyeType`, optional
+        The battleEye filters to use.
+    pvp_types: :class:`list` of :class:`.PvpTypeFilter`, optional
+        The list of PvP types to filter the results for.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the Tibia.com highscores.
+    """
+    pvp_types = pvp_types or []
+    pvp_params = [("worldtypes[]", p.value) for p in pvp_types]
+    return get_tibia_url("community", "highscores", *pvp_params, world=world, category=category.value,
+                         profession=vocation.value, currentpage=page,
+                         beprotection=battleye_type.value if battleye_type else None)
 
-    @property
-    def url(self):
-        """:class:`str`: Get the URL to this specific post."""
-        return self.get_url(self.post_id)
 
-    @classmethod
-    def get_url(cls, post_id):
-        """Get the URL to a specific post.
+def get_kill_statistics_url(world: str) -> str:
+    """Get the Tibia.com URL of the kill statistics of a world.
 
-        Parameters
-        ----------
-        post_id: :class:`int`
-            The ID of the desired post.
+    Parameters
+    ----------
+    world: :class:`str`
+        The game world of the desired kill statistics.
 
-        Returns
-        -------
-        :class:`str`
-            The URL to the post.
-        """
-        return get_tibia_url("forum", None, anchor=f"post{post_id}", action="thread", postid=post_id)
+    Returns
+    -------
+    :class:`str`
+        The URL to the Tibia.com kill statistics for this world.
+    """
+    return get_tibia_url("community", "killstatistics", world=world)
 
 
-class BaseThread(metaclass=abc.ABCMeta):
-    """Base class for thread classes.
+def get_event_schedule_url(month: int = None, year: int = None) -> str:
+    """Get the URL to the Event Schedule or Event Calendar on Tibia.com.
 
-    The following implement this class:
+    Notes
+    -----
+    If no parameters are passed, it will show the calendar for the current month and year.
 
-    - :class:`.ThreadEntry`
-    - :class:`.ForumThread`
+    Tibia.com limits the dates that the calendar displays, passing a month and year far from the current ones may
+    result in the response being for the current month and year instead.
 
-    Attributes
+    Parameters
     ----------
-    thread_id: :class:`int`
-        The internal ID of the thread.
-    """
+    month: :class:`int`, optional
+        The desired month.
+    year: :class:`int`, optional
+        The desired year.
 
-    __slots__ = (
-        "thread_id",
-    )
+    Returns
+    -------
+    :class:`str`
+        The URL to the calendar with the given parameters.
+    """
+    return get_tibia_url("news", "eventcalendar", calendarmonth=month, calendaryear=year)
 
-    @property
-    def url(self):
-        """:class:`str`: The URL to the thread in Tibia.com."""
-        return self.get_url(self.thread_id)
 
-    @classmethod
-    def get_url(cls, thread_id, page=1):
-        """Get the URL to a thread with a given id.
+def get_houses_section_url(world: str, town: str, house_type: HouseType, status: HouseStatus = None,
+                           order: HouseOrder = None) -> str:
+    """Get the URL to the house list on Tibia.com with the specified filters.
 
-        Parameters
-        ----------
-        thread_id: :class:`int`
-            The id of the desired thread.
-        page: :class:`int`
-            The desired page, by default 1.
+    Parameters
+    ----------
+    world: :class:`str`
+        The world to search in.
+    town: :class:`str`
+        The town to show results for.
+    house_type: :class:`HouseType`
+        The type of houses to show.
+    status: :class:`HouseStatus`
+        The status of the houses to show.
+    order: :class:`HouseOrder`
+        The sorting parameter to use for the results.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the list matching the parameters.
+    """
+    params = {
+        "world": world,
+        "town": town,
+        "type": house_type.plural if house_type else None,
+        "state": status.value if status else None,
+        "order": order.value if order else None,
+    }
+    return get_tibia_url("community", "houses", **{k: v for k, v in params.items() if v is not None})
 
-        Returns
-        -------
-        :class:`str`
-            The URL to the thread.
-        """
-        return get_tibia_url("forum", None, action="thread", threadid=thread_id, pagenumber=page)
 
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.thread_id == other.thread_id
-        return False
+def get_auction_url(auction_id: int):
+    """Get the URL to the Tibia.com detail page of an auction with a given id.
 
+    Parameters
+    ----------
+    auction_id: :class:`int`
+        The ID of the auction.
 
-class BaseTournament(metaclass=abc.ABCMeta):
-    """Base class for tournament classes.
+    Returns
+    -------
+    :class:`str`
+        The URL to the auction's detail page.
+    """
+    return get_tibia_url("charactertrade", "currentcharactertrades", page="details", auctionid=auction_id)
 
-    The following implement this class:
 
-    - :class:`.TournamentEntry`
-    - :class:`.Tournament`
+def get_bazaar_url(type: BazaarType, page: int = 1, filters: AuctionFilters = None):
+    """Get the URL to the list of current auctions in Tibia.com.
 
-    Attributes
+    Parameters
     ----------
-    title: :class:`str`
-        The tournament's title.
-    cycle: :class:`int`
-        The tournament's cycle.
+    page: :class:`int`
+        The page to show the URL for.
+    filters: :class:`AuctionFilters`
+        The filtering criteria to use.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the current auctions section in Tibia.com
     """
+    query_params = filters.query_params if filters else {}
+    return get_tibia_url("charactertrade", type.subtopic, currentpage=page, **query_params)
 
-    __slots__ = (
-        "title",
-        "cycle",
-    )
 
-    def __eq__(self, other):
-        """Two tournaments are considered the same when they have the same title or cycle."""
-        if isinstance(other, self.__class__):
-            return self.title.lower() == other.title.lower() or (self.cycle > 0 and self.cycle == other.cycle)
-        return False
+def get_cm_post_archive_url(start_date: datetime.datetime, end_date: datetime.datetime, page=1):
+    """Get the URL to the CM Post Archive for the given date range.
 
-    @property
-    def url(self):
-        """:class:`str`: The URL to the tournament's information page."""
-        return self.get_url(self.cycle)
+    Parameters
+    ----------
+    start_date: :class: `datetime.date`
+        The start date to display.
+    end_date: :class: `datetime.date`
+        The end date to display.
+    page: :class:`int`
+        The desired page to display.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the CM Post Archive
+
+    Raises
+    ------
+    TypeError:
+        Either of the dates is not an instance of :class:`datetime.date`
+    ValueError:
+        If ``start_date`` is more recent than ``end_date``.
+    """
+    if not isinstance(start_date, datetime.date):
+        raise TypeError(f"start_date: expected datetime.date instance, {type(start_date)} found.")
+    if not isinstance(end_date, datetime.date):
+        raise TypeError(f"start_date: expected datetime.date instance, {type(start_date)} found.")
+    if end_date < start_date:
+        raise ValueError("start_date can't be more recent than end_date.")
+    if page < 1:
+        raise ValueError("page must be 1 or greater.")
+    return get_tibia_url("forum", "forum", action="cm_post_archive", startday=start_date.day,
+                         startmonth=start_date.month, startyear=start_date.year, endday=end_date.day,
+                         endmonth=end_date.month, endyear=end_date.year, currentpage=page)
 
-    @classmethod
-    def get_url(cls, tournament_cycle):
-        """Get the URL to a tournament's information page.
 
-        If its cycle is provided, otherwise it shows the current tournament.
+def get_leaderboards_url(world: str, rotation_id: int = None, page: int = 1) -> str:
+    """Get the URL to the leaderboards of a world.
 
-        Parameters
-        ----------
-        tournament_cycle: :class:`int`
-            The tournament's cycle.
+    Parameters
+    ----------
+    world: :class:`str`
+        The desired world.
+    rotation_id: :class:`int`
+        The ID of the desired rotation. If undefined, the current rotation is shown.
+    page: :class:`int`
+        The desired page. By default, the first page is returned.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the leaderboard with the desired parameters.
+
+    Raises
+    ------
+    ValueError
+        If the specified page is zer or less.
+    """
+    if page <= 0:
+        raise ValueError("page must be 1 or greater")
+    return get_tibia_url("community", "leaderboards", world=world, rotation=rotation_id, currentpage=page)
 
-        Returns
-        -------
-        :class:`str`
-            The URL to the specified tournament.
-        """
-        params = None
-        if tournament_cycle:
-            params = {
-                "tournamentcycle": tournament_cycle,
-                "action": "archive",
-            }
-        return get_tibia_url("community", "tournament", **params)
 
+def get_creatures_section_url() -> str:
+    """Get the URL to the Tibia.com library section.
 
-class BaseWorld(metaclass=abc.ABCMeta):
-    """Base class for all World classes.
+    Returns
+    -------
+    :class:`str`:
+        The URL to the Tibia.com library section.
+    """
+    return get_tibia_url("library", "creature")
 
-    The following implement this class:
 
-    - :class:`.WorldEntry`
-    - :class:`.World`
+def get_creature_url(identifier: str) -> str:
+    """Get the URL to the creature's detail page on Tibia.com.
 
-    Attributes
+    Parameters
     ----------
-    name: :class:`str`
-        The name of the world.
+    identifier: :class:`str`
+        The race's internal name.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the detail page.
+    """
+    return get_tibia_url("library", "creatures", race=identifier)
+
+
+def get_boostable_bosses_url() -> str:
+    """Get the URL to the Tibia.com boostable bosses.
+
+    Returns
+    -------
+    :class:`str`:
+        The URL to the Tibia.com library section.
     """
+    return get_tibia_url("library", "boostablebosses")
 
-    name: str
-    location: WorldLocation
-    pvp_type: PvpType
-
-    __slots__ = (
-        "name",
-    )
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name!r} location={self.location!r} pvp_type={self.pvp_type!r}>"
-
-    @property
-    def url(self):
-        """:class:`str`: URL to the world's information page on Tibia.com."""
-        return self.get_url(self.name)
-
-    @classmethod
-    def get_url(cls, name):
-        """Get the URL to the World's information page on Tibia.com.
-
-        Parameters
-        ----------
-        name: :class:`str`
-            The name of the world.
-
-        Returns
-        -------
-        :class:`str`
-            The URL to the world's information page.
-        """
-        return get_tibia_url("community", "worlds", world=name.title())
-
-
-class HouseWithId:
-    """Implements the :py:attr:`id` attribute and dependant functions and properties.
-
-    Subclasses mut also implement :class:`.BaseHouse`
-    """
-
-    name: str
-    id: int
-    world: str
-    get_url: Callable[[int, str], str]
-
-    def __eq__(self, o: object) -> bool:
-        """Two houses are considered equal if their names or ids are equal."""
-        if isinstance(o, self.__class__):
-            return self.name.lower() == o.name.lower() or self.id == o.id
-        return False
-
-    @property
-    def url(self):
-        """:class:`str`: The URL to the Tibia.com page of the house."""
-        return self.get_url(self.id, self.world) if self.id and self.world else None
+
+def _to_yes_no(value: Optional[bool]):
+    if value is None:
+        return None
+    return "yes" if value else "no"
+
+
+def get_spells_section_url(vocation: SpellVocationFilter = None, group: SpellGroup = None, spell_type: SpellType = None,
+                           premium: Optional[bool] = None, sort: SpellSorting = None):
+    """Get the URL to the spells section with the desired filtering parameters.
+
+    Parameters
+    ----------
+    vocation: :class:`SpellVocationFilter`, optional
+        The vocation to filter in spells for.
+    group: :class:`SpellGroup`, optional
+        The spell's primary cooldown group.
+    spell_type: :class:`SpellType`, optional
+        The type of spells to show.
+    premium: :class:`bool`, optional
+        The type of premium requirement to filter. :obj:`None` means any premium requirement.
+    sort: :class:`SpellSorting`, optional
+        The field to sort spells by.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the spells section with the provided filtering parameters.
+    """
+    params = {
+        "vocation": vocation.value if vocation else None,
+        "group": group.value if group else None,
+        "type": spell_type.value if spell_type else None,
+        "sort": sort.value if sort else None,
+        "premium": _to_yes_no(premium),
+    }
+    return get_tibia_url("library", "spells", **params)
+
+
+def get_spell_url(identifier: str) -> str:
+    """Get the URL to a spell in the Tibia.com spells section.
+
+    Parameters
+    ----------
+    identifier: :class:`str`
+        The identifier of the spell.
+
+    Returns
+    -------
+    :class:`str`
+        The URL to the spell.
+    """
+    return get_tibia_url("library", "spells", spell=identifier.lower())
```

### Comparing `tibia.py-5.6.0/tibiapy/client.py` & `tibia.py-6.0.0a1/tibiapy/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,122 +1,84 @@
 """Asynchronous Tibia.com client."""
 import asyncio
 import datetime
 import json
 import logging
 import time
-import typing
+from typing import TypeVar, Optional, Callable, Collection, Set
 
 import aiohttp
 import aiohttp_socks
 
 import tibiapy
-from tibiapy import Auction, AuctionFilters, CharacterBazaar, Leaderboard, Spell, SpellsSection, abc
-from tibiapy.character import Character
-from tibiapy.creature import BoostableBosses, BoostedCreatures, Creature, CreatureEntry, CreaturesSection
-from tibiapy.enums import BattlEyeHighscoresFilter, Category, HouseType, NewsCategory, \
-    NewsType, VocationFilter
+from tibiapy.enums import HighscoresBattlEyeType, HighscoresCategory, HouseType, NewsCategory, \
+    NewsType, HighscoresProfession, BazaarType, SpellVocationFilter, SpellGroup, SpellType, SpellSorting, \
+    PvpTypeFilter, HouseStatus, HouseOrder
 from tibiapy.errors import Forbidden, NetworkError, SiteMaintenanceError
-from tibiapy.event import EventSchedule
-from tibiapy.forum import BoardEntry, CMPostArchive, ForumAnnouncement, ForumBoard, ForumPost, ForumThread
-from tibiapy.guild import Guild, GuildWars, GuildsSection
-from tibiapy.highscores import Highscores
-from tibiapy.house import House, HousesSection
-from tibiapy.kill_statistics import KillStatistics
-from tibiapy.news import News, NewsArchive
-from tibiapy.tournament import Tournament, TournamentLeaderboard
-from tibiapy.world import World, WorldOverview
+from tibiapy.models import Character, SpellsSection, Spell, Leaderboard, KillStatistics, House, HousesSection, \
+    Highscores, Guild, GuildWars, GuildsSection, CMPostArchive, BoardEntry, ForumBoard, ForumThread, CharacterBazaar, \
+    Auction, AuctionFilters, ForumSection, TibiaResponse
+from tibiapy.models.creature import BoostableBosses, CreaturesSection, Creature, CreatureEntry
+from tibiapy.models.event import EventSchedule
+from tibiapy.models.news import NewsArchive, News
+from tibiapy.models.pagination import AjaxPaginator
+from tibiapy.models.world import World, WorldOverview
+from tibiapy.parsers.bazaar import AuctionParser, CharacterBazaarParser
+from tibiapy.parsers.character import CharacterParser
+from tibiapy.parsers.creature import BoostedCreaturesParser, BoostableBossesParser, CreaturesSectionParser, \
+    CreatureParser
+from tibiapy.parsers.event import EventScheduleParser
+from tibiapy.parsers.forum import CMPostArchiveParser, ForumBoardParser, ForumThreadParser, \
+    ForumAnnouncementParser, ForumSectionParser
+from tibiapy.parsers.guild import GuildParser, GuildWarsParser, GuildsSectionParser
+from tibiapy.parsers.highscores import HighscoresParser
+from tibiapy.parsers.house import HouseParser, HousesSectionParser
+from tibiapy.parsers.kill_statistics import KillStatisticsParser
+from tibiapy.parsers.leaderboard import LeaderboardParser
+from tibiapy.parsers.news import NewsArchiveParser, NewsParser
+from tibiapy.parsers.spell import SpellsSectionParser, SpellParser
+from tibiapy.parsers.world import WorldParser, WorldOverviewParser
+from tibiapy.urls import get_character_url, get_world_guilds_url, get_guild_url, get_house_url, get_world_overview_url, \
+    get_news_archive_url, get_news_url, get_forum_board_url, get_forum_announcement_url, get_forum_thread_url, \
+    get_highscores_url, get_kill_statistics_url, get_forum_post_url, get_event_schedule_url, get_houses_section_url, \
+    get_auction_url, get_bazaar_url, get_cm_post_archive_url, get_leaderboards_url, get_creatures_section_url, \
+    get_creature_url, get_boostable_bosses_url, get_spells_section_url, get_spell_url, get_world_url, \
+    get_guild_wars_url, get_forum_section_url
 
 __all__ = (
-    "TibiaResponse",
     "Client",
 )
 
-# Tibia.com's cache for the community section is 5 minutes.
-# This limit is not sent anywhere, so there's no way to automate it.
-CACHE_LIMIT = 300
 
-T = typing.TypeVar('T')
+T = TypeVar('T')
 
 log = logging.getLogger("tibiapy")
 
 
-class TibiaResponse(typing.Generic[T], abc.Serializable):
-    """Represents a response from Tibia.com.
-
-    Attributes
-    ----------
-    timestamp: :class:`datetime.datetime`
-        The date and time when the page was fetched, in UTC.
-    cached: :class:`bool`
-        Whether the response is cached or it is a fresh response.
-    age: :class:`int`
-        The age of the cache in seconds.
-    fetching_time: :class:`float`
-        The time in seconds it took for Tibia.com to respond.
-    parsing_time: :class:`float`
-        The time in seconds it took for the response to be parsed into data.
-    data: :class:`T`
-        The data contained in the response.
-    """
-
-    def __init__(self, raw_response, data: T, parsing_time=None):
-        self.timestamp: datetime.datetime = raw_response.timestamp
-        self.cached: bool = raw_response.cached
-        self.age: int = raw_response.age
-        self.fetching_time = raw_response.fetching_time
-        self.parsing_time = parsing_time
-        self.data: T = data
-
-    __slots__ = (
-        'timestamp',
-        'cached',
-        'age',
-        'fetching_time',
-        'parsing_time',
-        'data',
-    )
-
-    _serializable_properties = ("time_left", )
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__}[{type(self.data).__name__}] timestamp={self.timestamp!r} " \
-               f"fetching_time={self.fetching_time!r} parsing_time={self.fetching_time!r} cahed={self.cached!r} " \
-               f"age={self.age!r}>"
-
-    @property
-    def time_left(self):
-        """:class:`datetime.timedelta`: The time left for the cache of this response to expire."""
-        if not self.age:
-            return datetime.timedelta()
-        return (datetime.timedelta(seconds=CACHE_LIMIT - self.age)
-                - (datetime.datetime.now(datetime.timezone.utc) - self.timestamp))
-
-    @property
-    def seconds_left(self):
-        """:class:`int`: The time left in seconds for this response's cache to expire."""
-        return self.time_left.seconds
-
-
-class RawResponse:
+class _RawResponse:
     def __init__(self, response: aiohttp.ClientResponse, fetching_time: float):
         self.timestamp = datetime.datetime.now(datetime.timezone.utc)
         self.fetching_time = fetching_time
+        self.url = response.url
         self.cached = response.headers.get("CF-Cache-Status") == "HIT"
         age = response.headers.get("Age")
-        if age is not None and age.isnumeric():
-            self.age = int(age)
-        else:
-            self.age = 0
+        self.age = int(age) if age is not None and age.isnumeric() else 0
         self.content = None
 
     def __repr__(self):
         return f"<{self.__class__.__name__} timestamp={self.timestamp!r} fetching_time={self.fetching_time!r} " \
                f"cached={self.cached!r} age={self.age!r}>"
 
+    def parse(self, parser: Callable[[str], T]) -> TibiaResponse[T]:
+        start_time = time.perf_counter()
+        data = parser(self.content)
+        parsing_time = time.perf_counter() - start_time
+        log.info("%s | PARSE | %dms", self.url, int(parsing_time * 1000))
+        return TibiaResponse.from_raw(self, data, parsing_time)
+
 
 class Client:
     """An asynchronous client that fetches information from Tibia.com.
 
     The client uses a :class:`aiohttp.ClientSession` to request the information.
     A single session is shared across all operations.
 
@@ -148,15 +110,15 @@
             self.loop.create_task(self._initialize_session(proxy_url))
 
     # region Private Methods
 
     async def _initialize_session(self, proxy_url=None):
         """Initialize the aiohttp session object."""
         headers = {
-            'User-Agent': "Tibia.py/%s (+https://github.com/Galarzaa90/tibia.py)" % tibiapy.__version__,
+            'User-Agent': f"Tibia.py/{tibiapy.__version__} (+https://github.com/Galarzaa90/tibia.py)",
             'Accept-Encoding': "deflate, gzip",
         }
         connector = aiohttp_socks.SocksConnector.from_url(proxy_url) if proxy_url else None
         self.session: aiohttp.ClientSession = aiohttp.ClientSession(
             loop=self.loop,
             headers=headers,
             connector=connector,
@@ -187,15 +149,15 @@
         headers: :class:`dict`
             A mapping representing the headers to send as part of the request.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`RawResponse`
+        :class:`_RawResponse`
             The raw response obtained from the server.
 
         Raises
         ------
         Forbidden:
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
@@ -204,54 +166,53 @@
         """
         await self._session_ready.wait()
         if test:
             url = url.replace("www.tibia.com", "www.test.tibia.com")
         init_time = time.perf_counter()
         try:
             async with self.session.request(method, url, data=data, headers=headers) as resp:
-                diff_time = time.perf_counter()-init_time
+                diff_time = time.perf_counter() - init_time
                 if "maintenance.tibia.com" in str(resp.url):
                     log.info("%s | %s | %s %s | maintenance.tibia.com", url, resp.method, resp.status, resp.reason)
                     raise SiteMaintenanceError("Tibia.com is down for maintenance.")
                 log.info("%s | %s | %s %s | %dms", url, resp.method, resp.status, resp.reason, int(diff_time * 1000))
                 self._handle_status(resp.status, diff_time)
-                response = RawResponse(resp, diff_time)
+                response = _RawResponse(resp, diff_time)
                 response.content = await resp.text()
                 return response
         except aiohttp.ClientError as e:
-            raise NetworkError(f"aiohttp.ClientError: {e}", e, time.perf_counter() - init_time)
+            raise NetworkError(f"aiohttp.ClientError: {e}", e, time.perf_counter() - init_time) from e
         except aiohttp_socks.SocksConnectionError as e:
-            raise NetworkError(f"aiohttp_socks.SocksConnectionError: {e}", e, time.perf_counter() - init_time)
+            raise NetworkError(f"aiohttp_socks.SocksConnectionError: {e}", e, time.perf_counter() - init_time) from e
         except UnicodeDecodeError as e:
-            raise NetworkError(f'UnicodeDecodeError: {e}', e, time.perf_counter() - init_time)
+            raise NetworkError(f'UnicodeDecodeError: {e}', e, time.perf_counter() - init_time) from e
 
-    async def _fetch_all_pages(self, auction_id, paginator, item_type, *, test=False):
+    async def _fetch_all_pages(self, auction_id, paginator: AjaxPaginator, item_type, *, test=False):
         """Fetch all the pages of an auction paginator.
 
         Parameters
         ----------
         auction_id: :class:`int`
             The id of the auction.
         paginator:
             The paginator object
         item_type: :class:`int`
             The item type.
         test: :class:`bool`
             Whether to request the test website instead.
         """
-        if paginator is None or paginator.entry_class is None:
-            return
         current_page = 2
         while current_page <= paginator.total_pages:
             content = await self._fetch_ajax_page(auction_id, item_type, current_page, test=test)
             if content:
-                entries = Auction._parse_page_items(content, paginator.entry_class)
+                # noinspection PyProtectedMember
+                entries = AuctionParser._parse_page_items(content, paginator)
                 paginator.entries.extend(entries)
             current_page += 1
-        paginator.fully_fetched = True
+        paginator.is_fully_fetched = True
 
     async def _fetch_ajax_page(self, auction_id, type_id, page, *, test=False):
         """Fetch an ajax page from the paginated summaries in the auction section.
 
         Parameters
         ----------
         auction_id: :class:`int`
@@ -282,1279 +243,1173 @@
         try:
             return data['AjaxObjects'][0]['Data']
         except KeyError:
             return None
 
     # endregion
 
-    # region Bazaar
-    async def fetch_current_auctions(self, page=1, filters=None, *, test=False):
-        """Fetch the current auctions in the bazaar.
+    # region Front Page
 
-        .. versionadded:: 3.3.0
+    async def fetch_boosted_creature(self, *, test=False) -> TibiaResponse[CreatureEntry]:
+        """Fetch today's boosted creature.
+
+        .. versionadded:: 2.1.0
+        .. versionchanged:: 4.0.0
+            The return type of the data returned was changed to :class:`CreatureEntry`, previous type was removed.
 
         Parameters
         ----------
-        page: :class:`int`
-            The desired page to display.
-        filters: :class:`AuctionFilters`
-            The filtering criteria to use.
+        test: :class:`bool`
+            Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`CharacterBazaar`
-            The current auctions.
+        :class:`TibiaResponse` of :class:`.CreatureEntry`
+            The boosted creature of the day.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
-        ValueError
-            If the page number is not 1 or greater.
         """
-        if page <= 0:
-            raise ValueError('page must be 1 or greater.')
-        response = await self._request("GET", CharacterBazaar.get_current_auctions_url(page, filters), test=test)
-        start_time = time.perf_counter()
-        current_auctions = CharacterBazaar.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, current_auctions, parsing_time)
+        response = await self._request("GET", get_news_archive_url(), test=test)
+        return response.parse(CreaturesSectionParser.boosted_creature_from_header)
 
-    async def fetch_auction_history(self, page=1, filters=None, *, test=False):
-        """Fetch the auction history of the bazaar.
+    async def fetch_boosted_creature_and_boss(self, *, test=False):
+        """Fetch today's boosted creature and boss.
 
-        .. versionadded:: 3.3.0
+        .. versionadded:: 5.3.0
 
         Parameters
         ----------
-        page: :class:`int`
-            The page to display.
-        filters: :class:`AuctionFilters`
-            The filtering criteria to use.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`CharacterBazaar`
-            The character bazaar containing the auction history.
+        :class:`TibiaResponse` of :class:`BoostedCreatures`
+            The boosted creature and boss of the day.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
-        ValueError
-            If the page number is not 1 or greater.
         """
-        if page <= 0:
-            raise ValueError('page must be 1 or greater.')
-        response = await self._request("GET", CharacterBazaar.get_auctions_history_url(page, filters), test=test)
-        start_time = time.perf_counter()
-        auction_history = CharacterBazaar.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, auction_history, parsing_time)
+        response = await self._request("GET", get_news_archive_url(), test=test)
+        return response.parse(BoostedCreaturesParser.from_header)
 
-    async def fetch_auction(self, auction_id, *, fetch_items=False, fetch_mounts=False, fetch_outfits=False,
-                            skip_details=False, test=False):
-        """Fetch an auction by its ID.
+    # region Bosses
+    async def fetch_boosted_boss(self, *, test=False):
+        """Fetch today's boosted boss.
 
-        .. versionadded:: 3.3.0
+        .. versionadded:: 5.3.0
 
         Parameters
         ----------
-        auction_id: :class:`int`
-            The ID of the auction.
-        fetch_items: :class:`bool`
-            Whether to fetch all of the character's items. By default only the first page is fetched.
-        fetch_mounts: :class:`bool`
-            Whether to fetch all of the character's mounts. By default only the first page is fetched.
-        fetch_outfits: :class:`bool`
-            Whether to fetch all of the character's outfits. By default only the first page is fetched.
-        skip_details: :class:`bool`, optional
-            Whether to skip parsing the entire auction and only parse the information shown in lists. False by default.
-
-            This allows fetching basic information like name, level, vocation, world, bid and status, shaving off some
-            parsing time.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`Auction`
-            The auction matching the ID if found.
+        :class:`TibiaResponse` of :class:`BossEntry`
+            The boosted boss of the day.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
-        ValueError
-            If the auction id is not 1 or greater.
         """
-        if auction_id <= 0:
-            raise ValueError('auction_id must be 1 or greater.')
-        response = await self._request("GET", Auction.get_url(auction_id), test=test)
-        start_time = time.perf_counter()
-        auction = Auction.from_content(response.content, auction_id, skip_details)
-        parsing_time = time.perf_counter() - start_time
-        if auction and not skip_details:
-            if fetch_items:
-                await self._fetch_all_pages(auction_id, auction.items, 0, test=test)
-                await self._fetch_all_pages(auction_id, auction.store_items, 1, test=test)
-            if fetch_mounts:
-                await self._fetch_all_pages(auction_id, auction.mounts, 2, test=test)
-                await self._fetch_all_pages(auction_id, auction.store_mounts, 3, test=test)
-            if fetch_outfits:
-                await self._fetch_all_pages(auction_id, auction.outfits, 4, test=test)
-                await self._fetch_all_pages(auction_id, auction.store_outfits, 5, test=test)
-        return TibiaResponse(response, auction, parsing_time)
+        response = await self._request("GET", get_news_archive_url(), test=test)
+        return response.parse(BoostableBossesParser.boosted_boss_from_header)
 
     # endregion
 
-    async def fetch_cm_post_archive(self, start_date, end_date, page=1, *, test=False):
-        """Fetch the CM post archive.
+    # region News
+    async def fetch_news_archive(self, start_date: datetime.date, end_date: datetime.date,
+                                 categories: Set[NewsCategory] = None, types: Set[NewsType] = None,
+                                 *, test=False) -> TibiaResponse[NewsArchive]:
+        """Fetch news from the archive meeting the search criteria.
 
-        .. versionadded:: 3.0.0
+        .. versionchanged:: 5.0.0
+            The data attribute of the response contains an instance of :class:`NewsArchive` instead.
 
         Parameters
         ----------
-        start_date: :class: `datetime.date`
-            The start date to display.
-        end_date: :class: `datetime.date`
-            The end date to display.
-        page: :class:`int`
-            The desired page to display.
+        start_date: :class:`datetime.date`
+            The beginning date to search dates in.
+        end_date: :class:`datetime.date`
+            The end date to search dates in.
+        categories: `list` of :class:`NewsCategory`
+            The allowed categories to show. If left blank, all categories will be searched.
+        types : `list` of :class:`NewsType`
+            The allowed news types to show. if unused, all types will be searched.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`CMPostArchive`
-            The CM Post Archive.
+        :class:`TibiaResponse` of :class:`.NewsArchive`
+            The news meeting the search criteria.
 
         Raises
         ------
+        ValueError:
+            If ``begin_date`` is more recent than ``to_date``.
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
-        ValueError
-            If the start_date is more recent than the end date or page number is not 1 or greater.
         """
         if start_date > end_date:
-            raise ValueError("start_date cannot be more recent than end_date")
-        if page <= 0:
-            raise ValueError("page cannot be lower than 1.")
-        response = await self._request("GET", CMPostArchive.get_url(start_date, end_date, page), test=test)
-        start_time = time.perf_counter()
-        cm_post_archive = CMPostArchive.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, cm_post_archive, parsing_time)
+            raise ValueError("start_date can't be more recent than end_date")
+        form_data = NewsArchiveParser.get_form_data(start_date, end_date, categories, types)
+        response = await self._request("POST", get_news_archive_url(), form_data, test=test)
+        return response.parse(NewsArchiveParser.from_content)
+
+    async def fetch_news_archive_by_days(self, days=30, categories: Collection[NewsCategory] = None,
+                                         types: Collection[NewsType] = None, *,
+                                         test=False) -> TibiaResponse[NewsArchive]:
+        """Fetch all the published news in the last specified days.
 
-    async def fetch_event_schedule(self, month=None, year=None, *, test=False):
-        """Fetch the event calendar. By default, it gets the events for the current month.
+        This is a shortcut for :meth:`fetch_news_archive`, to handle dates more easily.
 
-        .. versionadded:: 3.0.0
+        .. versionchanged:: 5.0.0
+            The data attribute of the response contains an instance of :class:`NewsArchive` instead.
 
         Parameters
         ----------
-        month: :class:`int`
-            The month of the events to display.
-        year: :class:`int`
-            The year of the events to display.
+        days: :class:`int`
+            The number of days to search, by default 30.
+        categories: `list` of :class:`NewsCategory`
+            The allowed categories to show. If left blank, all categories will be searched.
+        types : `list` of :class:`NewsType`
+            The allowed news types to show. if unused, all types will be searched.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`EventSchedule`
-            The event calendar.
+        :class:`TibiaResponse` of :class:`.NewsArchive`
+            The news posted in the last specified days.
 
         Raises
         ------
+        ValueError:
+            If ``days`` is lesser than zero.
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
-        ValueError
-            If only one of year or month are defined.
         """
-        if (year is None and month is not None) or (year is not None and month is None):
-            raise ValueError("both year and month must be defined or neither must be defined.")
-        response = await self._request("GET", EventSchedule.get_url(month, year), test=test)
-        start_time = time.perf_counter()
-        calendar = EventSchedule.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, calendar, parsing_time)
-
-    # region Forums
-    async def fetch_forum_community_boards(self, *, test=False):
-        """Fetch the forum's community boards.
+        if days < 0:
+            raise ValueError("days must be zero or higher")
+        end = datetime.date.today()
+        begin = end - datetime.timedelta(days=days)
+        return await self.fetch_news_archive(begin, end, categories, types, test=test)
 
-        .. versionadded:: 3.0.0
+    async def fetch_news(self, news_id: int, *, test=False) -> TibiaResponse[Optional[News]]:
+        """Fetch a news entry by its id from Tibia.com.
 
         Parameters
         ----------
+        news_id: :class:`int`
+            The ID of the news entry.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of list of :class:`BoardEntry`
-            The forum boards in the community section.
+        :class:`TibiaResponse` of :class:`.News`
+            The news entry if found, :obj:`None` otherwise.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", BoardEntry.get_community_boards_url(), test=test)
-        start_time = time.perf_counter()
-        boards = BoardEntry.list_from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boards, parsing_time)
+        response = await self._request("GET", get_news_url(news_id), test=test)
+        return response.parse(lambda r: NewsParser.from_content(r, news_id))
 
-    async def fetch_forum_support_boards(self, *, test=False):
-        """Fetch the forum's community boards.
+    async def fetch_event_schedule(self, month: int = None, year: int = None, *,
+                                   test=False) -> TibiaResponse[EventSchedule]:
+        """Fetch the event calendar. By default, it gets the events for the current month.
 
         .. versionadded:: 3.0.0
 
         Parameters
         ----------
+        month: :class:`int`
+            The month of the events to display.
+        year: :class:`int`
+            The year of the events to display.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of list of :class:`BoardEntry`
-            The forum boards in the community section.
+        :class:`TibiaResponse` of :class:`EventSchedule`
+            The event calendar.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
+        ValueError
+            If only one of year or month are defined.
         """
-        response = await self._request("GET", BoardEntry.get_support_boards_url(), test=test)
-        start_time = time.perf_counter()
-        boards = BoardEntry.list_from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boards, parsing_time)
+        if (year is None and month is not None) or (year is not None and month is None):
+            raise ValueError("both year and month must be defined or neither must be defined.")
+        response = await self._request("GET", get_event_schedule_url(month, year), test=test)
+        return response.parse(EventScheduleParser.from_content)
 
-    async def fetch_forum_world_boards(self, *, test=False):
-        """Fetch the forum's world boards.
+    # endregion
 
-        .. versionadded:: 3.0.0
+    # region Library
+
+    async def fetch_creatures(self, *, test=False) -> TibiaResponse[CreaturesSection]:
+        """Fetch the creatures from the library section.
+
+        .. versionadded:: 4.0.0
 
         Parameters
         ----------
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of list of :class:`BoardEntry`
-            The forum boards in the world section.
+        :class:`TibiaResponse` of :class:`.CreaturesSection`
+            The creature's section in Tibia.com
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", BoardEntry.get_world_boards_url(), test=test)
-        start_time = time.perf_counter()
-        boards = BoardEntry.list_from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boards, parsing_time)
+        response = await self._request("GET", get_creatures_section_url(), test=test)
+        return response.parse(CreaturesSectionParser.from_content)
 
-    async def fetch_forum_trade_boards(self, *, test=False):
-        """Fetch the forum's trade boards.
+    async def fetch_creature(self, identifier: str, *, test=False) -> TibiaResponse[Optional[Creature]]:
+        """Fetch a creature's information from the Tibia.com library.
 
-        .. versionadded:: 3.0.0
+        .. versionadded:: 4.0.0
 
         Parameters
         ----------
+        identifier: :class:`str`
+            The internal name of the race.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of list of :class:`BoardEntry`
-            The forum boards in the trade section.
+        :class:`TibiaResponse` of :class:`.Creature`
+            The creature's section in Tibia.com
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", BoardEntry.get_trade_boards_url(), test=test)
-        start_time = time.perf_counter()
-        boards = BoardEntry.list_from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boards, parsing_time)
+        response = await self._request("GET", get_creature_url(identifier), test=test)
+        return response.parse(CreatureParser.from_content)
 
-    async def fetch_forum_board(self, board_id, page=1, age=30, *, test=False):
-        """Fetch a forum board with a given id.
+    async def fetch_boostable_bosses(self, *, test=False) -> TibiaResponse[BoostableBosses]:
+        """Fetch the boostable bosses from the library section.
 
-        .. versionadded:: 3.0.0
+        .. versionadded:: 4.0.0
 
         Parameters
         ----------
-        board_id : :class:`int`
-            The id of the board.
-        page: :class:`int`
-            The page number to show.
-        age: :class:`int`
-            The maximum age in days of the threads to display.
-
-            To show threads of all ages, use -1.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`ForumBoard`
-            A response containing the forum, if found.
+        :class:`TibiaResponse` of :class:`,BoostableBosses`
+            The creature's section in Tibia.com
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", ForumBoard.get_url(board_id, page, age), test=test)
-        start_time = time.perf_counter()
-        board = ForumBoard.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, board, parsing_time)
-
-    async def fetch_forum_thread(self, thread_id, page=1, *, test=False):
-        """Fetch a forum thread with a given id.
+        response = await self._request("GET", get_boostable_bosses_url(), test=test)
+        return response.parse(BoostableBossesParser.from_content)
 
-        .. versionadded:: 3.0.0
+    async def fetch_spells(self, *, vocation: SpellVocationFilter = None, group: SpellGroup = None,
+                           spell_type: SpellType = None, premium: bool = None,
+                           sort: SpellSorting = None, test=False) -> TibiaResponse[SpellsSection]:
+        """Fetch the spells section.
 
         Parameters
         ----------
-        thread_id : :class:`int`
-            The id of the thread.
-        page: :class:`int`
-            The desired page to display, by default 1.
+        vocation: :class:`.SpellVocationFilter`, optional
+            The vocation to filter in spells for.
+        group: :class:`.SpellGroup`, optional
+            The spell's primary cooldown group.
+        spell_type: :class:`.SpellType`, optional
+            The type of spells to show.
+        premium: :class:`bool`, optional
+            The type of premium requirement to filter. :obj:`None` means any premium requirement.
+        sort: :class:`.SpellSorting`, optional
+            The field to sort spells by.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`ForumThread`
-            A response containing the forum, if found.
+        :class:`TibiaResponse` of :class:`SpellsSection`
+            The spells section with the results.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", ForumThread.get_url(thread_id, page), test=test)
-        start_time = time.perf_counter()
-        thread = ForumThread.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, thread, parsing_time)
-
-    async def fetch_forum_post(self, post_id, *, test=False):
-        """Fetch a forum post with a given id.
-
-        The thread that contains the post will be returned, containing the desired post in
-        :py:attr:`ForumThread.anchored_post`.
-
-        The displayed page will be the page where the post is located.
+        response = await self._request("GET", get_spells_section_url(vocation=vocation, group=group,
+                                                                     spell_type=spell_type, premium=premium,
+                                                                     sort=sort), test=test)
+        return response.parse(SpellsSectionParser.from_content)
 
-        .. versionadded:: 3.1.0
+    async def fetch_spell(self, identifier: str, *, test=False) -> TibiaResponse[Optional[Spell]]:
+        """Fetch a spell by its identifier.
 
         Parameters
         ----------
-        post_id : :class:`int`
-            The id of the post.
+        identifier: :class:`str`
+            The spell's identifier. This is usually the name of the spell in lowercase and with no spaces.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`ForumThread`
-            A response containing the forum, if found.
+        :class:`TibiaResponse` of :class:`.Spell`
+            The spell if found, :obj:`None` otherwise.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", ForumPost.get_url(post_id), test=test)
-        start_time = time.perf_counter()
-        thread = ForumThread.from_content(response.content)
-        if thread:
-            thread.anchored_post = next((p for p in thread.posts if p.post_id == post_id), None)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, thread, parsing_time)
+        response = await self._request("GET", get_spell_url(identifier), test=test)
+        return response.parse(SpellParser.from_content)
 
-    async def fetch_forum_announcement(self, announcement_id, *, test=False):
-        """Fetch a forum announcement.
+    # endregion
 
-        .. versionadded:: 3.0.0
+    # region Community
+
+    async def fetch_character(self, name: str, *, test=False) -> TibiaResponse[Optional[Character]]:
+        """Fetch a character by its name from Tibia.com.
 
         Parameters
         ----------
-        announcement_id: :class:`int`
-            The id of the desired announcement.
+        name: :class:`str`
+            The name of the character.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`ForumAnnouncement`
-            The forum announcement, if found.
+        :class:`TibiaResponse` of :class:`.Character`
+            A response containing the character, if found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", ForumAnnouncement.get_url(announcement_id), test=test)
-        start_time = time.perf_counter()
-        announcement = ForumAnnouncement.from_content(response.content, announcement_id)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, announcement, parsing_time)
-
-    # endregion
-
-    async def fetch_boosted_creature_and_boss(self, *, test=False):
-        """Fetch today's boosted creature and boss.
+        response = await self._request("GET", get_character_url(name.strip()), test=test)
+        return response.parse(CharacterParser.from_content)
 
-        .. versionadded:: 5.3.0
+    async def fetch_world_overview(self, *, test=False) -> TibiaResponse[WorldOverview]:
+        """Fetch the world overview information from Tibia.com.
 
         Parameters
         ----------
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`BoostedCreatures`
-            The boosted creature and boss of the day.
+        :class:`TibiaResponse` of :class:`WorldOverview`
+            A response containing the world overview information.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", NewsArchive.get_url(), test=test)
-        start_time = time.perf_counter()
-        boosted_creatures = BoostedCreatures.from_header(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boosted_creatures, parsing_time)
-
-    # Region Bosses
-    async def fetch_boosted_boss(self, *, test=False):
-        """Fetch today's boosted boss.
+        response = await self._request("GET", get_world_overview_url(), test=test)
+        return response.parse(WorldOverviewParser.from_content)
 
-        .. versionadded:: 5.3.0
+    async def fetch_world(self, name: str, *, test=False) -> TibiaResponse[Optional[World]]:
+        """Fetch a world from Tibia.com.
 
         Parameters
         ----------
+        name: :class:`str`
+            The name of the world.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`BossEntry`
-            The boosted boss of the day.
+        :class:`TibiaResponse` of :class:`.World`
+            A response containing the world's information if found, :obj:`None` otherwise.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", NewsArchive.get_url(), test=test)
-        start_time = time.perf_counter()
-        boosted_creature = BoostableBosses.boosted_boss_from_header(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boosted_creature, parsing_time)
+        response = await self._request("GET", get_world_url(name), test=test)
+        return response.parse(WorldParser.from_content)
 
-    async def fetch_library_bosses(self, *, test=False):
-        """Fetch the bosses from the library section.
+    async def fetch_highscores_page(self, world: str = None,
+                                    category: HighscoresCategory = HighscoresCategory.EXPERIENCE,
+                                    vocation: HighscoresProfession = HighscoresProfession.ALL, page: int = 1,
+                                    battleye_type: HighscoresBattlEyeType = None, pvp_types: Set[PvpTypeFilter] = None,
+                                    *, test=False) -> TibiaResponse[Highscores]:
+        """Fetch a single highscores page from Tibia.com.
 
-        .. versionadded:: 4.0.0
+        Notes
+        -----
+        It is not possible to use BattlEye or PvPType filters when requesting a specific world.
 
         Parameters
         ----------
+        world: :class:`str`
+            The world to search the highscores in.
+        category: :class:`HighscoresCategory`
+            The highscores category to search, by default Experience.
+        vocation: :class:`HighscoresProfession`
+            The vocation filter to use. No filter used by default.
+        page: :class:`int`
+            The page to fetch, by default the first page is fetched.
+        battleye_type: :class:`HighscoresBattlEyeType`
+            The type of BattlEye protection to display results from.
+        pvp_types: :class:`list` of :class:`PvpTypeFilter`
+            The list of PvP types to filter the results for.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`BoostableBosses`
-            The creature's section in Tibia.com
+        :class:`TibiaResponse` of :class:`Highscores`
+            The highscores information or :obj:`None` if not found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
+        ValueError
+            If an invalid filter combination is passed or an invalid page is provided.
         """
-        response = await self._request("GET", BoostableBosses.get_url(), test=test)
-        start_time = time.perf_counter()
-        boosted_creature = BoostableBosses.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boosted_creature, parsing_time)
-
-    # endregion
+        pvp_types = pvp_types or []
+        if page < 1:
+            raise ValueError("page must be 1 or higher.")
+        if world is not None and ((battleye_type and battleye_type != HighscoresBattlEyeType.ANY_WORLD) or pvp_types):
+            raise ValueError("BattleEye and PvP type filters can only be used when fetching all worlds.")
+        response = await self._request("GET", get_highscores_url(world, category, vocation, page, battleye_type,
+                                                                 pvp_types), test=test)
+        return response.parse(HighscoresParser.from_content)
 
-    # region Creatures
-    async def fetch_boosted_creature(self, *, test=False):
-        """Fetch today's boosted creature.
+    async def fetch_leaderboard(self, world: str, rotation: int = None, page=1, *, test=False) \
+            -> TibiaResponse[Leaderboard]:
+        """Fetch the leaderboards for a specific world and rotation.
 
-        .. versionadded:: 2.1.0
-        .. versionchanged:: 4.0.0
-            The return type of the data returned was changed to :class:`Creature`, previous type was removed.
+        .. versionadded:: 5.0.0
 
         Parameters
         ----------
+        world: :class:`str`
+            The name of the world.
+        rotation: :class:`int`
+            The ID of the rotation. By default, it will get the current rotation.
+        page: :class:`int`
+            The page to get.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`CreatureEntry`
-            The boosted creature of the day.
+        :class:`TibiaResponse` of :class:`Leaderboard`
+            The leaderboards of the world if found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", NewsArchive.get_url(), test=test)
-        start_time = time.perf_counter()
-        boosted_creature = CreaturesSection.boosted_creature_from_header(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boosted_creature, parsing_time)
+        response = await self._request("GET", get_leaderboards_url(world, rotation, page), test=test)
+        return response.parse(LeaderboardParser.from_content)
 
-    async def fetch_library_creatures(self, *, test=False):
-        """Fetch the creatures from the library section.
-
-        .. versionadded:: 4.0.0
+    async def fetch_kill_statistics(self, world: str, *, test=False) -> TibiaResponse[KillStatistics]:
+        """Fetch the kill statistics of a world from Tibia.com.
 
         Parameters
         ----------
+        world: :class:`str`
+            The name of the world.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`CreaturesSection`
-            The creature's section in Tibia.com
+        :class:`TibiaResponse` of :class:`KillStatistics`
+            The kill statistics of the world if found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", CreaturesSection.get_url(), test=test)
-        start_time = time.perf_counter()
-        boosted_creature = CreaturesSection.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boosted_creature, parsing_time)
+        response = await self._request("GET", get_kill_statistics_url(world), test=test)
+        return response.parse(KillStatisticsParser.from_content)
 
-    async def fetch_creature(self, identifier, *, test=False):
-        """Fetch a creature's information from the Tibia.com library.
+    async def fetch_houses_section(self, world: str, town: str, house_type: HouseType = HouseType.HOUSE,
+                                   status: HouseStatus = None, order: HouseOrder = None, *,
+                                   test=False) -> TibiaResponse[HousesSection]:
+        """Fetch the house list of a world and type.
 
-        .. versionadded:: 4.0.0
+        .. versionchanged:: 5.0.0
+            The data attribute of the response contains an instance of :class:`HousesSection` instead.
 
         Parameters
         ----------
-        identifier: :class:`str`
-            The internal name of the race.
+        world: :class:`str`
+            The name of the world.
+        town: :class:`str`
+            The name of the town.
+        house_type: :class:`HouseType`
+            The type of building. House by default.
+        status: :class:`HouseStatus`, optional
+            The house status to filter results. By default, no filters will be applied.
+        order: :class:`HouseOrder`, optional
+            The ordering to use for the results. By default, they are sorted by name.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`Creature`
-            The creature's section in Tibia.com
+        :class:`TibiaResponse` of :class:`HousesSection`
+            A response containing the lists of houses meeting the criteria if found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", Creature.get_url(identifier), test=test)
-        start_time = time.perf_counter()
-        boosted_creature = Creature.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, boosted_creature, parsing_time)
+        response = await self._request("GET", get_houses_section_url(world=world, town=town, house_type=house_type,
+                                                                     status=status, order=order), test=test)
+        return response.parse(HousesSectionParser.from_content)
 
-    # endregion
-
-    async def fetch_character(self, name, *, test=False):
-        """Fetch a character by its name from Tibia.com.
+    async def fetch_house(self, house_id: int, world: str, *, test=False) -> TibiaResponse[Optional[House]]:
+        """Fetch a house in a specific world by its id.
 
         Parameters
         ----------
-        name: :class:`str`
-            The name of the character.
+        house_id: :class:`int`
+            The house's internal id.
+        world: :class:`str`
+            The name of the world to look for.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`Character`
-            A response containing the character, if found.
+        :class:`TibiaResponse` of :class:`House`
+            The house if found, :obj:`None` otherwise.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", Character.get_url(name.strip()), test=test)
-        start_time = time.perf_counter()
-        char = Character.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, char, parsing_time)
+        response = await self._request("GET", get_house_url(world, house_id), test=test)
+        return response.parse(HouseParser.from_content)
 
-    # region Guilds
-    async def fetch_guild(self, name, *, test=False):
-        """Fetch a guild by its name from Tibia.com.
+    async def fetch_world_guilds(self, world: str, *, test=False) -> TibiaResponse[GuildsSection]:
+        """Fetch the list of guilds in a world from Tibia.com.
+
+        If a world that does not exist is passed, the world attribute of the result will be :obj:`None`.
+        If the world attribute is set, but the list is empty, it just means the world has no guilds.
+
+        .. versionchanged:: 5.0.0
+            The data attribute of the response contains an instance of :class:`GuildsSection` instead.
 
         Parameters
         ----------
-        name: :class:`str`
-            The name of the guild. The case must match exactly.
+        world: :class:`str`
+            The name of the world.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`Guild`
-            A response containing the found guild, if any.
+        :class:`TibiaResponse` of :class:`GuildsSection`
+            A response containing the guilds section for the specified world.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", Guild.get_url(name), test=test)
-        start_time = time.perf_counter()
-        guild = Guild.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, guild, parsing_time)
+        response = await self._request("GET", get_world_guilds_url(world), test=test)
+        return response.parse(GuildsSectionParser.from_content)
 
-    async def fetch_guild_wars(self, name, *, test=False):
-        """Fetch a guild's wars by its name from Tibia.com.
-
-        .. versionadded:: 3.0.0
+    async def fetch_guild(self, name: str, *, test=False) -> TibiaResponse[Optional[Guild]]:
+        """Fetch a guild by its name from Tibia.com.
 
         Parameters
         ----------
         name: :class:`str`
             The name of the guild. The case must match exactly.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`GuildWars`
-            A response containing the found guild's wars.
-
-            If the guild doesn't exist, the displayed data will show a guild with no wars instead of indicating the
-            guild doesn't exist.
+        :class:`TibiaResponse` of :class:`Guild`
+            A response containing the found guild, if any.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", GuildWars.get_url(name), test=test)
-        start_time = time.perf_counter()
-        guild_wars = GuildWars.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, guild_wars, parsing_time)
+        response = await self._request("GET", get_guild_url(name), test=test)
+        return response.parse(GuildParser.from_content)
 
-    # endregion
+    async def fetch_guild_wars(self, name: str, *, test=False) -> TibiaResponse[Optional[GuildWars]]:
+        """Fetch a guild's wars by its name from Tibia.com.
 
-    async def fetch_house(self, house_id, world, *, test=False):
-        """Fetch a house in a specific world by its id.
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
-        house_id: :class:`int`
-            The house's internal id.
-        world: :class:`str`
-            The name of the world to look for.
+        name: :class:`str`
+            The name of the guild. The case must match exactly.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`House`
-            The house if found, :obj:`None` otherwise.
+        :class:`TibiaResponse` of :class:`GuildWars`
+            A response containing the found guild's wars.
+
+            If the guild doesn't exist, the displayed data will show a guild with no wars instead of indicating the
+            guild doesn't exist.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", House.get_url(house_id, world), test=test)
-        start_time = time.perf_counter()
-        house = House.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, house, parsing_time)
+        response = await self._request("GET", get_guild_wars_url(name), test=test)
+        return response.parse(GuildWarsParser.from_content)
 
-    async def fetch_highscores_page(self, world=None, category=Category.EXPERIENCE, vocation=VocationFilter.ALL, page=1,
-                                    battleye_type=None, pvp_types=None, *, test=False):
-        """Fetch a single highscores page from Tibia.com.
+    # endregion
 
-        Notes
-        -----
-        It is not possible to use BattlEye or PvPType filters when requesting a specific world.
+    # region Forums
+    async def fetch_forum_section(self, section_id: int, *, test=False) -> TibiaResponse[Optional[ForumSection]]:
+        """Fetch a forum's section by its ID.
 
         Parameters
         ----------
-        world: :class:`str`
-            The world to search the highscores in.
-        category: :class:`Category`
-            The highscores category to search, by default Experience.
-        vocation: :class:`VocationFilter`
-            The vocation filter to use. No filter used by default.
-        page: :class:`int`
-            The page to fetch, by default the first page is fetched.
-        battleye_type: :class:`BattlEyeFilter`
-            The type of BattlEye protection to display results from.
-        pvp_types: :class:`list` of :class:`PvpTypeFilter`
-            The list of PvP types to filter the results for.
+        section_id: :class:`int`
+            The ID of the section.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`Highscores`
-            The highscores information or :obj:`None` if not found.
+        :class:`TibiaResponse` of :class:`ForumSection`
+            The forum section with the provided ID.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
-        ValueError
-            If an invalid filter combination is passed.
         """
-        pvp_types = pvp_types or []
-        if world is not None and ((battleye_type and battleye_type != BattlEyeHighscoresFilter.ANY_WORLD) or pvp_types):
-            raise ValueError("BattleEye and PvP type filters can only be used when fetching all worlds.")
-        response = await self._request("GET", Highscores.get_url(world, category, vocation, page, battleye_type,
-                                                                 pvp_types), test=test)
-        start_time = time.perf_counter()
-        highscores = Highscores.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, highscores, parsing_time)
+        response = await self._request("GET", get_forum_section_url(section_id), test=test)
+        return response.parse(ForumSectionParser.from_content)
 
-    async def fetch_kill_statistics(self, world, *, test=False):
-        """Fetch the kill statistics of a world from Tibia.com.
+    async def fetch_forum_world_boards(self, *, test=False) -> TibiaResponse[Optional[ForumSection]]:
+        """Fetch the forum's world boards.
+
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
-        world: :class:`str`
-            The name of the world.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`KillStatistics`
-            The kill statistics of the world if found.
+        :class:`TibiaResponse` of :class:`ForumSection`
+            The forum boards in the world section.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", KillStatistics.get_url(world), test=test)
-        start_time = time.perf_counter()
-        kill_statistics = KillStatistics.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, kill_statistics, parsing_time)
+        response = await self._request("GET", BoardEntry.get_world_boards_url(), test=test)
+        return response.parse(ForumSectionParser.from_content)
 
-    async def fetch_leaderboard(self, world, rotation=None, page=1, *, test=False):
-        """Fetch the leaderboards for a specific world and rotation.
+    async def fetch_forum_trade_boards(self, *, test=False) -> TibiaResponse[Optional[ForumSection]]:
+        """Fetch the forum's trade boards.
 
-        .. versionadded:: 5.0.0
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
-        world: :class:`str`
-            The name of the world.
-        rotation: :class:`int`
-            The ID of the rotation. By default it will get the current rotation.
-        page: :class:`int`
-            The page to get.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`Leaderboard`
-            The leaderboards of the world if found.
+        :class:`TibiaResponse` of :class:`ForumSection`
+            The forum boards in the trade section.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", Leaderboard.get_url(world, rotation, page), test=test)
-        start_time = time.perf_counter()
-        leaderboard = Leaderboard.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, leaderboard, parsing_time)
+        response = await self._request("GET", BoardEntry.get_trade_boards_url(), test=test)
+        return response.parse(ForumSectionParser.from_content)
 
-    # region Worlds
-    async def fetch_world(self, name, *, test=False):
-        """Fetch a world from Tibia.com.
+    async def fetch_forum_community_boards(self, *, test=False) -> TibiaResponse[Optional[ForumSection]]:
+        """Fetch the forum's community boards.
+
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
-        name: :class:`str`
-            The name of the world.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`World`
-            A response containig the he world's information if found, :obj:`None` otherwise.
+        :class:`TibiaResponse` of :class:`ForumSection`
+            The forum boards in the community section.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", World.get_url(name), test=test)
-        start_time = time.perf_counter()
-        world = World.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, world, parsing_time)
+        response = await self._request("GET", BoardEntry.get_community_boards_url(), test=test)
+        return response.parse(ForumSectionParser.from_content)
 
-    async def fetch_world_houses(self, world, town, house_type=HouseType.HOUSE, status=None, order=None, *, test=False):
-        """Fetch the house list of a world and type.
+    async def fetch_forum_support_boards(self, *, test=False) -> TibiaResponse[Optional[ForumSection]]:
+        """Fetch the forum's community boards.
 
-        .. versionchanged:: 5.0.0
-            The data attribute of the response contains an instance of :class:`HousesSection` instead.
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
-        world: :class:`str`
-            The name of the world.
-        town: :class:`str`
-            The name of the town.
-        house_type: :class:`HouseType`
-            The type of building. House by default.
-        status: :class:`HouseStatus`, optional
-            The house status to filter results. By default, no filters will be applied.
-        order: :class:`HouseOrder`, optional
-            The ordering to use for the results. By default, they are sorted by name.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`HousesSection`
-            A response containing the lists of houses meeting the criteria if found.
+        :class:`TibiaResponse` of :class:`ForumSection`
+            The forum boards in the community section.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", HousesSection.get_url(world=world, town=town, house_type=house_type,
-                                                                    status=status, order=order), test=test)
-        start_time = time.perf_counter()
-        world_houses = HousesSection.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, world_houses, parsing_time)
-
-    async def fetch_world_guilds(self, world: str, *, test=False):
-        """Fetch the list of guilds in a world from Tibia.com.
+        response = await self._request("GET", BoardEntry.get_support_boards_url(), test=test)
+        return response.parse(ForumSectionParser.from_content)
 
-        If a world that does not exist is passed, the world attribute of the result will be :obj:`None`.
-        If the world attribute is set, but the list is empty, it just means the world has no guilds.
+    async def fetch_forum_board(self, board_id: int, page: int = 1, age: int = None, *,
+                                test=False) -> TibiaResponse[ForumBoard]:
+        """Fetch a forum board with a given id.
 
-        .. versionchanged:: 5.0.0
-            The data attribute of the response contains an instance of :class:`GuildsSection` instead.
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
-        world: :class:`str`
-            The name of the world.
+        board_id : :class:`int`
+            The id of the board.
+        page: :class:`int`
+            The page number to show.
+        age: :class:`int`
+            The maximum age in days of the threads to display.
+
+            To show threads of all ages, use -1.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`GuildsSection`
-            A response containing the guilds section for the specified world.
+        :class:`TibiaResponse` of :class:`ForumBoard`
+            A response containing the forum, if found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", GuildsSection.get_url(world), test=test)
-        start_time = time.perf_counter()
-        guilds = GuildsSection.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, guilds, parsing_time)
+        response = await self._request("GET", get_forum_board_url(board_id, page, age), test=test)
+        return response.parse(ForumBoardParser.from_content)
 
-    async def fetch_world_list(self, *, test=False):
-        """Fetch the world overview information from Tibia.com.
+    async def fetch_forum_thread(self, thread_id: int, page: int = 1, *,
+                                 test=False) -> TibiaResponse[Optional[ForumThread]]:
+        """Fetch a forum thread with a given id.
+
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
+        thread_id : :class:`int`
+            The id of the thread.
+        page: :class:`int`
+            The desired page to display, by default 1.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`WorldOverview`
-            A response containing the world overview information.
+        :class:`TibiaResponse` of :class:`ForumThread`
+            A response containing the forum, if found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        response = await self._request("GET", WorldOverview.get_url(), test=test)
-        start_time = time.perf_counter()
-        world_overview = WorldOverview.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, world_overview, parsing_time)
+        response = await self._request("GET", get_forum_thread_url(thread_id, page), test=test)
+        return response.parse(ForumThreadParser.from_content)
 
-    # endregion
+    async def fetch_forum_post(self, post_id: int, *, test=False) -> TibiaResponse[Optional[ForumThread]]:
+        """Fetch a forum post with a given id.
 
-    # region News
-    async def fetch_news_archive(self, start_date, end_date, categories=None, types=None, *, test=False):
-        """Fetch news from the archive meeting the search criteria.
+        The thread that contains the post will be returned, containing the desired post in
+        :py:attr:`ForumThread.anchored_post`.
 
-        .. versionchanged:: 5.0.0
-            The data attribute of the response contains an instance of :class:`NewsArchive` instead.
+        The displayed page will be the page where the post is located.
+
+        .. versionadded:: 3.1.0
 
         Parameters
         ----------
-        start_date: :class:`datetime.date`
-            The beginning date to search dates in.
-        end_date: :class:`datetime.date`
-            The end date to search dates in.
-        categories: `list` of :class:`NewsCategory`
-            The allowed categories to show. If left blank, all categories will be searched.
-        types : `list` of :class:`NewsType`
-            The allowed news types to show. if unused, all types will be searched.
+        post_id : :class:`int`
+            The id of the post.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`NewsArchive`
-            The news meeting the search criteria.
+        :class:`TibiaResponse` of :class:`ForumThread`
+            A response containing the forum, if found.
 
         Raises
         ------
-        ValueError:
-            If ``begin_date`` is more recent than ``to_date``.
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        if start_date > end_date:
-            raise ValueError("start_date can't be more recent than end_date")
-        form_data = NewsArchive.get_form_data(start_date, end_date, categories, types)
-        response = await self._request("POST", NewsArchive.get_url(), form_data, test=test)
-        start_time = time.perf_counter()
-        news = NewsArchive.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, news, parsing_time)
-
-    async def fetch_recent_news(self, days=30, categories=None, types=None, *, test=False):
-        """Fetch all the published news in the last specified days.
+        response = await self._request("GET", get_forum_post_url(post_id), test=test)
+        built_response = response.parse(ForumThreadParser.from_content)
+        if built_response.data is None:
+            return built_response
+        built_response.data.anchored_post = next((p for p in built_response.data.entries if p.post_id == post_id), None)
+        return built_response
 
-        This is a shortcut for :meth:`fetch_news_archive`, to handle dates more easily.
+    async def fetch_forum_announcement(self, announcement_id, *, test=False):
+        """Fetch a forum announcement.
 
-        .. versionchanged:: 5.0.0
-            The data attribute of the response contains an instance of :class:`NewsArchive` instead.
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
-        days: :class:`int`
-            The number of days to search, by default 30.
-        categories: `list` of :class:`NewsCategory`
-            The allowed categories to show. If left blank, all categories will be searched.
-        types : `list` of :class:`NewsType`
-            The allowed news types to show. if unused, all types will be searched.
+        announcement_id: :class:`int`
+            The id of the desired announcement.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`NewsArchive`
-            The news posted in the last specified days.
+        :class:`TibiaResponse` of :class:`ForumAnnouncement`
+            The forum announcement, if found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
         """
-        end = datetime.date.today()
-        begin = end - datetime.timedelta(days=days)
-        return await self.fetch_news_archive(begin, end, categories, types, test=test)
+        response = await self._request("GET", get_forum_announcement_url(announcement_id), test=test)
+        return response.parse(lambda c: ForumAnnouncementParser.from_content(c, announcement_id))
 
-    async def fetch_news(self, news_id, *, test=False):
-        """Fetch a news entry by its id from Tibia.com.
+    async def fetch_cm_post_archive(self, start_date: datetime.datetime, end_date: datetime.datetime, page=1, *,
+                                    test=False) -> TibiaResponse[CMPostArchive]:
+        """Fetch the CM post archive.
+
+        .. versionadded:: 3.0.0
 
         Parameters
         ----------
-        news_id: :class:`int`
-            The id of the news entry.
+        start_date: :class: `datetime.date`
+            The start date to display.
+        end_date: :class: `datetime.date`
+            The end date to display.
+        page: :class:`int`
+            The desired page to display.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`News`
-            The news entry if found, :obj:`None` otherwise.
+        :class:`TibiaResponse` of :class:`CMPostArchive`
+            The CM Post Archive.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
+        ValueError
+            If the start_date is more recent than the end date or page number is not 1 or greater.
         """
-        response = await self._request("GET", News.get_url(news_id), test=test)
-        start_time = time.perf_counter()
-        news = News.from_content(response.content, news_id)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, news, parsing_time)
-    # endregion
-
-    # region Spells
-    async def fetch_spells(self, *, vocation=None, group=None, spell_type=None, premium=None, sort=None, test=False):
-        """Fetch the spells section.
-
-        Parameters
-        ----------
-        vocation: :class:`VocationSpellFilter`, optional
-            The vocation to filter in spells for.
-        group: :class:`SpellGroup`, optional
-            The spell's primary cooldown group.
-        spell_type: :class:`SpellType`, optional
-            The type of spells to show.
-        premium: :class:`bool`, optional
-            The type of premium requirement to filter. :obj:`None` means any premium requirement.
-        sort: :class:`SpellSorting`, optional
-            The field to sort spells by.
+        if start_date > end_date:
+            raise ValueError("start_date cannot be more recent than end_date")
+        if page <= 0:
+            raise ValueError("page cannot be lower than 1.")
+        response = await self._request("GET", get_cm_post_archive_url(start_date, end_date, page), test=test)
+        return response.parse(CMPostArchiveParser.from_content)
 
-        Returns
-        -------
-        :class:`TibiaResponse` of :class:`SpellsSection`
-            The spells section with the results.
+    # endregion
 
-        Raises
-        ------
-        Forbidden
-            If a 403 Forbidden error was returned.
-            This usually means that Tibia.com is rate-limiting the client because of too many requests.
-        NetworkError
-            If there's any connection errors during the request.
-        """
-        response = await self._request("GET", SpellsSection.get_url(vocation=vocation, group=group,
-                                                                    spell_type=spell_type, premium=premium,
-                                                                    sort=sort), test=test)
-        start_time = time.perf_counter()
-        spells = SpellsSection.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, spells, parsing_time)
+    # region Char Bazaar
+    async def fetch_current_auctions(self, page: int = 1, filters: AuctionFilters = None, *,
+                                     test=False) -> TibiaResponse[CharacterBazaar]:
+        """Fetch the current auctions in the bazaar.
 
-    async def fetch_spell(self, identifier, *, test=False):
-        """Fetch a spell by its identifier.
+        .. versionadded:: 3.3.0
 
         Parameters
         ----------
-        identifier: :class:`str`
-            The spell's identifier. This is usually the name of the spell in lowercase and with no spaces.
+        page: :class:`int`
+            The desired page to display.
+        filters: :class:`.AuctionFilters`
+            The filtering criteria to use.
         test: :class:`bool`
-            Whether to request the test website instead.
+            Whether to fetch from the test website or not.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`Spell`
-            The spell if found, :obj:`None` otherwise.
+        :class:`TibiaResponse` of :class:`CharacterBazaar`
+            The current auctions.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
+        ValueError
+            If the page number is not 1 or greater.
         """
-        response = await self._request("GET", Spell.get_url(identifier), test=test)
-        start_time = time.perf_counter()
-        spells = Spell.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, spells, parsing_time)
-    # endregion
+        if page <= 0:
+            raise ValueError('page must be 1 or greater.')
+        response = await self._request("GET", get_bazaar_url(BazaarType.CURRENT, page, filters), test=test)
+        return response.parse(CharacterBazaarParser.from_content)
 
-    # region Tournaments
-    async def fetch_tournament(self, tournament_cycle=0, *, test=False):
-        """Fetch a tournament from Tibia.com.
+    async def fetch_auction_history(self, page: int = 1, filters: AuctionFilters = None, *,
+                                    test=False) -> TibiaResponse[CharacterBazaar]:
+        """Fetch the auction history of the bazaar.
 
-        .. versionadded:: 2.5.0
+        .. versionadded:: 3.3.0
 
         Parameters
         ----------
-        tournament_cycle: :class:`int`
-            The cycle of the tournament. if unspecified, it will get the currently running tournament.
+        page: :class:`int`
+            The page to display.
+        filters: :class:`AuctionFilters`
+            The filtering criteria to use.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`Tournament`
-            The tournament if found, :obj:`None` otherwise.
+        :class:`TibiaResponse` of :class:`CharacterBazaar`
+            The character bazaar containing the auction history.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
+        ValueError
+            If the page number is not 1 or greater.
         """
-        response = await self._request("GET", Tournament.get_url(tournament_cycle), test=test)
-        start_time = time.perf_counter()
-        tournament = Tournament.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, tournament, parsing_time)
+        if page <= 0:
+            raise ValueError('page must be 1 or greater.')
+        response = await self._request("GET", get_bazaar_url(BazaarType.HISTORY, page, filters), test=test)
+        return response.parse(CharacterBazaarParser.from_content)
 
-    async def fetch_tournament_leaderboard(self, tournament_cycle, world, page=1, *, test=False):
-        """Fetch a tournament leaderboard from Tibia.com.
+    async def fetch_auction(self, auction_id: int, *, fetch_items=False, fetch_mounts=False, fetch_outfits=False,
+                            fetch_familiars=False, skip_details=False, test=False) -> TibiaResponse[Optional[Auction]]:
+        """Fetch an auction by its ID.
 
-        .. versionadded:: 2.5.0
+        .. versionadded:: 3.3.0
 
         Parameters
         ----------
-        tournament_cycle: :class:`int`
-            The cycle of the tournament. if unspecified, it will get the currently running tournament.
-        world: :class:`str`
-            The name of the world to get the leaderboards for.
-        page: :class:`int`
-            The desired leaderboards page, by default 1 is used.
+        auction_id: :class:`int`
+            The ID of the auction.
+        fetch_items: :class:`bool`
+            Whether to fetch all the character's items. By default, only the first page is fetched.
+        fetch_mounts: :class:`bool`
+            Whether to fetch all the character's mounts. By default, only the first page is fetched.
+        fetch_outfits: :class:`bool`
+            Whether to fetch all the character's outfits. By default, only the first page is fetched.
+        fetch_familiars: :class:`bool`
+            Whether to fetch all the character's outfits. By default, only the first page is fetched.
+        skip_details: :class:`bool`
+            Whether to skip parsing the entire auction and only parse the information shown in lists. False by default.
+
+            This allows fetching basic information like name, level, vocation, world, bid and status, shaving off some
+            parsing time.
         test: :class:`bool`
             Whether to request the test website instead.
 
         Returns
         -------
-        :class:`TibiaResponse` of :class:`TournamentLeaderboard`
-            The tournament's leaderboard if found, :obj:`None` otherwise.
+        :class:`TibiaResponse` of :class:`Auction`
+            The auction matching the ID if found.
 
         Raises
         ------
         Forbidden
             If a 403 Forbidden error was returned.
             This usually means that Tibia.com is rate-limiting the client because of too many requests.
         NetworkError
             If there's any connection errors during the request.
+        ValueError
+            If the auction id is not 1 or greater.
         """
-        response = await self._request("GET", TournamentLeaderboard.get_url(world, tournament_cycle, page), test=test)
-        start_time = time.perf_counter()
-        tournament_leaderboard = TournamentLeaderboard.from_content(response.content)
-        parsing_time = time.perf_counter() - start_time
-        return TibiaResponse(response, tournament_leaderboard, parsing_time)
+        if auction_id <= 0:
+            raise ValueError('auction_id must be 1 or greater.')
+        response = await self._request("GET", get_auction_url(auction_id), test=test)
+        tibia_response = response.parse(lambda c: AuctionParser.from_content(c, auction_id, skip_details))
+        if tibia_response.data is None:
+            return tibia_response
+        auction = tibia_response.data
+        if auction and not skip_details:
+            if fetch_items:
+                await self._fetch_all_pages(auction_id, auction.details.items, 0, test=test)
+                await self._fetch_all_pages(auction_id, auction.details.store_items, 1, test=test)
+            if fetch_mounts:
+                await self._fetch_all_pages(auction_id, auction.details.mounts, 2, test=test)
+                await self._fetch_all_pages(auction_id, auction.details.store_mounts, 3, test=test)
+            if fetch_outfits:
+                await self._fetch_all_pages(auction_id, auction.details.outfits, 4, test=test)
+                await self._fetch_all_pages(auction_id, auction.details.store_outfits, 5, test=test)
+            if fetch_familiars:
+                await self._fetch_all_pages(auction_id, auction.details.outfits, 6, test=test)
+        return tibia_response
+
     # endregion
```

### Comparing `tibia.py-5.6.0/tibiapy/creature.py` & `tibia.py-6.0.0a1/tibiapy/parsers/creature.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,39 @@
 """Models related to the creatures section in the library."""
 import os
 import re
 import urllib.parse
-from typing import List, Optional
 
 import bs4
 
-from tibiapy import abc
+from tibiapy.builders.creature import CreatureBuilder
 from tibiapy.errors import InvalidContent
+from tibiapy.models.creature import CreatureEntry, CreaturesSection, BoostedCreatures, BossEntry, BoostableBosses
+from tibiapy.utils import parse_tibiacom_content, convert_line_breaks
 
 __all__ = (
-    "BoostedCreatures",
-    "BoostableBosses",
-    "BossEntry",
-    "CreatureEntry",
-    "CreaturesSection",
-    "Creature",
+    "BoostableBossesParser",
+    "BoostedCreaturesParser",
+    "CreatureParser",
+    "CreaturesSectionParser",
 )
 
-from tibiapy.utils import parse_tibiacom_content, get_tibia_url
-
 BOOSTED_ALT = re.compile("Today's boosted \w+: ")
 
 
 HP_PATTERN = re.compile(r"have (\d+) hitpoints")
 EXP_PATTERN = re.compile(r"yield (\d+) experience")
 IMMUNE_PATTERN = re.compile(r"immune to ([^.]+)")
 WEAK_PATTERN = re.compile(r"weak against ([^.]+)")
 STRONG_PATTERN = re.compile(r"strong against ([^.]+)")
 LOOT_PATTERN = re.compile(r"They carry (.*) with them.")
 MANA_COST = re.compile(r"takes (\d+) mana")
 
 
-class BoostedCreatures(abc.Serializable):
-    """Contains both boosted creature and boosted boss.
-
-    Attributes
-    ----------
-    creature: :class:`CreatureEntry`
-        The boosted creature of the day.
-    boss: :class:`BossEntry`
-        The boosted boss of the day.
-    """
-
-    __slots__ = (
-        "creature",
-        "boss",
-    )
-
-    def __init__(self, creature, boss):
-        self.creature: CreatureEntry = creature
-        self.boss: BossEntry = boss
+class BoostedCreaturesParser:
 
     @classmethod
     def _parse_boosted_platform(cls, parsed_content: bs4.BeautifulSoup, tag_id: str):
         img = parsed_content.find("img", attrs={"id": tag_id})
         name = BOOSTED_ALT.sub("", img["title"]).strip()
         image_url = img["src"]
         identifier = image_url.split("/")[-1].replace(".gif", "")
@@ -80,49 +59,23 @@
             If content is not the HTML of a Tibia.com page.
         """
         try:
             parsed_content = bs4.BeautifulSoup(content.replace('ISO-8859-1', 'utf-8'), "lxml",
                                                parse_only=bs4.SoupStrainer("div", attrs={"id": "RightArtwork"}))
             creature_name, creature_identifier = cls._parse_boosted_platform(parsed_content, "Monster")
             boss_name, boss_identifier = cls._parse_boosted_platform(parsed_content, "Boss")
-            return cls(CreatureEntry(creature_name, creature_identifier), BossEntry(boss_name, boss_identifier))
+            return BoostedCreatures(
+                creature=CreatureEntry(name=creature_name, identifier=creature_identifier),
+                boss=BossEntry(name=boss_name, identifier=boss_identifier)
+            )
         except (TypeError, NameError, KeyError) as e:
             raise InvalidContent("content is not from Tibia.com", e)
 
 
-class BoostableBosses(abc.Serializable):
-    """Represents the boostable bosses section in the Tibia.com library
-
-    Attributes
-    ----------
-    boosted_boss: :class:`BossEntry`
-        The current boosted boss.
-    bosses: list of :class:`BossEntry`
-        The list of boostable bosses.
-    """
-
-    __slots__ = (
-        "boosted_boss",
-        "bosses",
-    )
-
-    def __init__(self, boosted_boss, bosses):
-        self.boosted_boss: BossEntry = boosted_boss
-        self.bosses: List[BossEntry] = bosses
-
-    @classmethod
-    def get_url(cls):
-        """Get the URL to the Tibia.com boostable bosses.
-
-        Returns
-        -------
-        :class:`str`:
-            The URL to the Tibia.com library section.
-        """
-        return get_tibia_url("library", "boostablebosses")
+class BoostableBossesParser:
 
     @classmethod
     def from_content(cls, content):
         """Create an instance of the class from the html content of the boostable bosses library's page.
 
         Parameters
         ----------
@@ -144,26 +97,27 @@
             boosted_creature_table = parsed_content.find("div", {"class": "TableContainer"})
             boosted_creature_text = boosted_creature_table.find("div", {"class": "Text"})
             if not boosted_creature_text or "Boosted" not in boosted_creature_text.text:
                 raise InvalidContent("content is not from the boostable bosses section.")
             boosted_boss_tag = boosted_creature_table.find("b")
             boosted_boss_image = boosted_creature_table.find("img")
             image_url = urllib.parse.urlparse(boosted_boss_image["src"])
-            boosted_boss = BossEntry(boosted_boss_tag.text, os.path.basename(image_url.path).replace(".gif", ""))
+            boosted_boss = BossEntry(name=boosted_boss_tag.text,
+                                     identifier=os.path.basename(image_url.path).replace(".gif", ""))
 
             list_table = parsed_content.find("div", style=lambda v: v and 'display: table' in v)
             entries_container = list_table.find_all("div", style=lambda v: v and 'float: left' in v)
             entries = []
             for entry_container in entries_container:
                 name = entry_container.text.strip()
                 image = entry_container.find("img")
                 image_url = urllib.parse.urlparse(image["src"])
                 identifier = os.path.basename(image_url.path).replace(".gif", "")
-                entries.append(BossEntry(name, identifier))
-            return cls(boosted_boss, entries)
+                entries.append(BossEntry(name=name, identifier=identifier))
+            return BoostableBosses(boosted_boss=boosted_boss, bosses=entries)
         except (AttributeError, ValueError) as e:
             raise InvalidContent("content is not the boosted boss's library", e)
 
 
     @classmethod
     def boosted_boss_from_header(cls, content):
         """Get the boosted boss from any Tibia.com page.
@@ -179,80 +133,19 @@
             The boosted boss of the day.
 
         Raises
         ------
         InvalidContent
             If content is not the HTML of a Tibia.com's page.
         """
-        return BoostedCreatures.from_header(content).boss
+        return BoostedCreaturesParser.from_header(content).boss
 
 
-class BossEntry(abc.Serializable):
-    """Represents a boss in the boostable bosses section in the Tibia.com library.
 
-    Attributes
-    ----------
-    name: :class:`str`
-        The name of the boss..
-    identifier: :class:`str`
-        The internal name of the boss. Used for images.
-    """
-
-    __slots__ = (
-        "name",
-        "identifier",
-    )
-
-    _serializable_properties = (
-        "image_url",
-    )
-
-    def __init__(self, name, identifier=None):
-        self.name: str = name
-        self.identifier: str = identifier
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name!r} identifier={self.identifier!r}>"
-
-    @property
-    def image_url(self):
-        """:class:`str`: The URL to this boss's image."""
-        return f"https://static.tibia.com/images/library/{self.identifier}.gif"
-
-
-class CreaturesSection(abc.Serializable):
-    """Represents the creature's section in the Tibia.com library.
-
-    Attributes
-    ----------
-    boosted_creature: :class:`CreatureEntry`
-        The current boosted creature.
-    creatures: list of :class:`CreatureEntry`
-        The list of creatures in the library.
-    """
-
-    __slots__ = (
-        "boosted_creature",
-        "creatures",
-    )
-
-    def __init__(self, boosted_creature, creatures):
-        self.boosted_creature: CreatureEntry = boosted_creature
-        self.creatures: List[CreatureEntry] = creatures or []
-
-    @classmethod
-    def get_url(cls):
-        """Get the URL to the Tibia.com library section.
-
-        Returns
-        -------
-        :class:`str`:
-            The URL to the Tibia.com library section.
-        """
-        return get_tibia_url("library", "creature")
+class CreaturesSectionParser:
 
     @classmethod
     def boosted_creature_from_header(cls, content):
         """Get the boosted creature from any Tibia.com page.
 
         Parameters
         ----------
@@ -265,15 +158,15 @@
             The boosted creature of the day.
 
         Raises
         ------
         InvalidContent
             If content is not the HTML of a Tibia.com's page.
         """
-        return BoostedCreatures.from_header(content).creature
+        return BoostedCreaturesParser.from_header(content).creature
 
     @classmethod
     def from_content(cls, content):
         """Create an instance of the class from the html content of the creature library's page.
 
         Parameters
         ----------
@@ -288,152 +181,41 @@
         Raises
         ------
         InvalidContent
             If content is not the HTML of a creature library's page.
         """
         try:
             parsed_content = parse_tibiacom_content(content)
-            boosted_creature_table = parsed_content.find("div", {"class": "TableContainer"})
-            boosted_creature_text = boosted_creature_table.find("div", {"class": "Text"})
+            boosted_creature_table = parsed_content.select_one("div.TableContainer")
+            boosted_creature_text = boosted_creature_table.select_one("div.Text")
             if not boosted_creature_text or "Boosted" not in boosted_creature_text.text:
                 raise InvalidContent("content is not from the creatures section.")
             boosted_creature_link = boosted_creature_table.find("a")
             url = urllib.parse.urlparse(boosted_creature_link["href"])
             query = urllib.parse.parse_qs(url.query)
-            boosted_creature = CreatureEntry(boosted_creature_link.text, query["race"][0])
+            boosted_creature = CreatureEntry(name=boosted_creature_link.text, identifier=query["race"][0])
 
             list_table = parsed_content.find("div", style=lambda v: v and 'display: table' in v)
             entries_container = list_table.find_all("div", style=lambda v: v and 'float: left' in v)
             entries = []
             for entry_container in entries_container:
                 name = entry_container.text.strip()
-                link = entry_container.find("a")
+                link = entry_container.select_one("a")
                 url = urllib.parse.urlparse(link["href"])
                 query = urllib.parse.parse_qs(url.query)
-                entries.append(CreatureEntry(name, query["race"][0]))
-            return cls(boosted_creature, entries)
+                entries.append(CreatureEntry(name=name, identifier=query["race"][0]))
+            return CreaturesSection(boosted_creature=boosted_creature, creatures=entries)
         except (AttributeError, ValueError) as e:
             raise InvalidContent("content is not the creature's library", e)
 
 
-class CreatureEntry(abc.Serializable):
-    """Represents a creature in the Library section.
-
-    Attributes
-    ----------
-    name: :class:`str`
-        The name of the creature, usually in plural, except for the boosted creature.
-    identifier: :class:`str`
-        The internal name of the creature's race. Used for links and images.
-    """
-
-    __slots__ = (
-        "name",
-        "identifier",
-    )
-
-    _serializable_properties = (
-        "image_url",
-    )
-
-    def __init__(self, name, identifier=None):
-        self.name: str = name
-        self.identifier: str = identifier
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name!r} identifier={self.identifier!r}>"
-
-    @property
-    def url(self):
-        """:class:`str`: The URL to this creature's details."""
-        return self.get_url(self.identifier)
-
-    @property
-    def image_url(self):
-        """:class:`str`: The URL to this creature's image."""
-        return f"https://static.tibia.com/images/library/{self.identifier}.gif"
-
-    @classmethod
-    def get_url(cls, identifier):
-        """Get the URL to the creature's detail page on Tibia.com.
-
-        Parameters
-        ----------
-        identifier: :class:`str`
-            The race's internal name.
-
-        Returns
-        -------
-        :class:`str`
-            The URL to the detail page.
-        """
-        return get_tibia_url("library", "creatures", race=identifier)
-
-
-class Creature(CreatureEntry):
-    """Represents a creature's details on the Tibia.com library.
-
-    Attributes
-    ----------
-    name: :class:`str`
-        The name of the creature, in plural form.
-    identifier: :class:`str`
-        The race's internal name. Used for links and images.
-    description: :class:`str`
-        A description of the creature.
-    hitpoints: :class:`int`
-        The number of hitpoints the creature has.
-    experience: :class:`int`
-        The number of experience points given for killing this creature.
-    immune_to: list of :class:`str`
-        The elements this creature is immune to.
-    weak_against: list of :class:`str`
-        The elements this creature is weak against.
-    strong_against: list of :class:`str`
-        The elements this creature is strong against.
-    loot: :class:`str`
-        Some of the items this creature drops.
-    mana_cost: :class:`int`, optional
-        The mana neccessary to summon or convince this creature.
-    summonable: :class:`bool`
-        Whether this creature can be summoned or not.
-    convinceable: :class:`bool`
-        Whether this creature can be convinced or not.
-    """
+class CreatureParser:
 
     _valid_elements = ["ice", "fire", "earth", "poison", "death", "holy", "physical", "energy"]
 
-    __slots__ = (
-        "name",
-        "identifier",
-        "description",
-        "hitpoints",
-        "experience",
-        "immune_to",
-        "weak_against",
-        "strong_against",
-        "loot",
-        "mana_cost",
-        "summonable",
-        "convinceable",
-    )
-
-    def __init__(self, name, identifier, **kwargs):
-        super().__init__(name, identifier)
-        self.immune_to: List[str] = kwargs.get("immune_to", [])
-        self.weak_against: List[str] = kwargs.get("weak_against", [])
-        self.strong_against: List[str] = kwargs.get("strong_against", [])
-        self.loot: str = kwargs.get("loot")
-        self.mana_cost: Optional[int] = kwargs.get("mana_cost")
-        self.summonable: bool = kwargs.get("summonable", False)
-        self.convinceable: bool = kwargs.get("convinceable", False)
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name!r} identifier={self.identifier!r}>"
-
     @classmethod
     def from_content(cls, content):
         """Create an instance of the class from the html content of the creature library's page.
 
         Parameters
         ----------
         content: :class:`str`
@@ -451,85 +233,84 @@
             title_container, description_container = content_container.find_all("div")
             title = title_container.find("h2")
             name = title.text.strip()
 
             img = title_container.find("img")
             img_url = img["src"]
             race = img_url.split("/")[-1].replace(".gif", "")
-            creature = cls(name, race)
+            builder = CreatureBuilder().name(name).identifier(race)
 
+            convert_line_breaks(description_container)
             paragraph_tags = description_container.find_all("p")
             paragraphs = [p.text for p in paragraph_tags]
-            creature.description = "\n".join(paragraphs[:-2])
+            builder.description("\n".join(paragraphs[:-2]).strip())
             hp_text = paragraphs[-2]
-            creature._parse_hp_text(hp_text)
+            cls._parse_hp_text(builder, hp_text)
 
             exp_text = paragraphs[-1]
-            creature._parse_exp_text(exp_text)
-            return creature
+            cls._parse_exp_text(builder, exp_text)
+            return builder.build()
         except ValueError:
             return None
 
-    def _parse_exp_text(self, exp_text):
+    @classmethod
+    def _parse_exp_text(cls, builder, exp_text):
         """Parse the experience text, containing dropped loot and adds it to the creature.
 
         Parameters
         ----------
         exp_text: :class:`str`
             The text containing experience.
         """
-        m = EXP_PATTERN.search(exp_text)
-        if m:
-            self.experience = int(m.group(1))
-        m = LOOT_PATTERN.search(exp_text)
-        if m:
-            self.loot = m.group(1)
+        if m := EXP_PATTERN.search(exp_text):
+            builder.experience(int(m.group(1)))
+        if m := LOOT_PATTERN.search(exp_text):
+            builder.loot(m.group(1))
 
-    def _parse_hp_text(self, hp_text):
+    @classmethod
+    def _parse_hp_text(cls, builder: CreatureBuilder, hp_text):
         """Parse the text containing the creatures hitpoints, containing weaknesses, immunities and more and adds it.
 
         Parameters
         ----------
         hp_text: :class:`str`
             The text containing hitpoints.
         """
         m = HP_PATTERN.search(hp_text)
         if m:
-            self.hitpoints = int(m.group(1))
+            builder.hitpoints(int(m.group(1)))
         m = IMMUNE_PATTERN.search(hp_text)
+        immune = []
         if m:
-            self._parse_elements(self.immune_to, m.group(1))
+            immune.extend(cls._parse_elements(m.group(1)))
         if "cannot be paralysed" in hp_text:
-            self.immune_to.append("paralyze")
-        m = WEAK_PATTERN.search(hp_text)
-        if m:
-            self._parse_elements(self.weak_against, m.group(1))
-        m = STRONG_PATTERN.search(hp_text)
-        if m:
-            self._parse_elements(self.strong_against, m.group(1))
-        m = MANA_COST.search(hp_text)
-        if m:
-            self.mana_cost = int(m.group(1))
+            immune.append("paralyze")
+        if "sense invisible" in hp_text:
+            immune.append("invisible")
+        builder.immune_to(immune)
+        if m := WEAK_PATTERN.search(hp_text):
+            builder.weak_against(cls._parse_elements(m.group(1)))
+        if m := STRONG_PATTERN.search(hp_text):
+            builder.strong_against(cls._parse_elements(m.group(1)))
+        if m := MANA_COST.search(hp_text):
+            builder.mana_cost(int(m.group(1)))
             if "summon or convince" in hp_text:
-                self.convinceable = True
-                self.summonable = True
+                builder.convinceable(True)
+                builder.summonable(True)
             if "cannot be summoned" in hp_text:
-                self.convinceable = True
+                builder.convinceable(True)
             if "cannot be convinced" in hp_text:
-                self.summonable = True
-        if "sense invisible" in hp_text:
-            self.immune_to.append("invisible")
+                builder.summonable(True)
+
 
     @classmethod
-    def _parse_elements(cls, collection, text):
+    def _parse_elements(cls, text):
         """Parse the elements found in a string, adding them to the collection.
 
         Parameters
         ----------
         collection: :class:`list`
             The collection where found elements will be added to.
         text: :class:`str`
             The text containing the elements.
         """
-        for element in cls._valid_elements:
-            if element in text:
-                collection.append(element)
+        return [element for element in cls._valid_elements if element in text]
```

### Comparing `tibia.py-5.6.0/tibiapy/enums.py` & `tibia.py-6.0.0a1/tibiapy/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,102 @@
 """Enumerations used by models throughout the library."""
-import enum
+from enum import Enum, Flag, IntEnum
+
+import pydantic.errors
+
+from tibiapy.utils import try_enum
 
 __all__ = (
-    'AccountStatus',
-    'AuctionOrder',
+    'AuctionBattlEyeFilter',
     'AuctionOrderBy',
-    'AuctionStatus',
+    'AuctionOrderDirection',
+    'PvpTypeFilter',
     'AuctionSearchType',
-    'Category',
+    'AuctionSkillFilter',
+    'AuctionStatus',
+    'AuctionVocationFilter',
+    'AvailableForumSection',
     'BattlEyeType',
-    'BattlEyeHighscoresFilter',
-    'BattlEyeTypeFilter',
     'BazaarType',
     'BidType',
+    'HighscoresBattlEyeType',
+    'HighscoresCategory',
+    'HighscoresProfession',
     'HouseOrder',
     'HouseStatus',
     'HouseType',
     'NewsCategory',
     'NewsType',
     'PvpType',
-    'PvpTypeFilter',
     'Sex',
-    'SkillFilter',
     'SpellGroup',
     'SpellSorting',
     'SpellType',
+    'SpellVocationFilter',
     'ThreadStatus',
-    'TournamentWorldType',
-    'TournamentPhase',
     'TransferType',
     'Vocation',
-    'VocationAuctionFilter',
-    'VocationFilter',
-    'VocationSpellFilter',
     'WorldLocation',
 )
 
 
-class BaseEnum(enum.Enum):
-    def __str__(self):
-        return self.value
+class StringEnum(str, Enum):
 
-    def __repr__(self):
-        return "%s.%s" % (self.__class__.__name__, self.name)
+    @classmethod
+    def __get_validators__(cls):
+        cls.lookup = {v: k.value for v, k in cls.__members__.items()}
+        yield cls.validate
 
+    @classmethod
+    def validate(cls, v):
+        e = try_enum(cls, v)
+        if e is None:
+            raise pydantic.errors.EnumMemberError(enum_values=list(cls))
+        return e
 
-class NumericEnum(BaseEnum):
+
+class NumericEnum(IntEnum):
     def __str__(self):
         return self.name.lower()
 
+    @classmethod
+    def __get_validators__(cls):
+        cls.lookup = {v: k.value for v, k in cls.__members__.items()}
+        yield cls.validate
 
-class AccountStatus(BaseEnum):
-    """Possible account statuses."""
+    @classmethod
+    def validate(cls, v):
+        e = try_enum(cls, v)
+        if e is None:
+            raise pydantic.errors.EnumMemberError(enum_values=list(cls))
+        return e
 
-    FREE_ACCOUNT = "Free Account"
-    PREMIUM_ACCOUNT = "Premium Account"
 
+class AuctionBattlEyeFilter(NumericEnum):
+    """The possible BattlEye filters that can be used for auctions."""
 
-class AuctionOrder(NumericEnum):
+    INITIALLY_PROTECTED = 1
+    """Worlds protected from the beginning, represented by a green symbol."""
+    PROTECTED = 2
+    """Worlds protected after the world was created, represented by a yellow symbol."""
+    NOT_PROTECTED = 3
+    """Worlds without any BattlEye protection."""
+    YELLOW = PROTECTED
+    """Alias for protected worlds.
+
+    .. versionadded:: 4.0.0
+    """
+    GREEN = INITIALLY_PROTECTED
+    """Alias for initially protected worlds.
+
+    .. versionadded:: 4.0.0
+    """
+
+
+class AuctionOrderDirection(NumericEnum):
     """The possible ordering directions for auctions.
 
     The field or value used for the ordering is defined by :class:`AuctionOrderBy`.
     """
 
     HIGHEST_LATEST = 0
     """Order by the highest or latest value."""
@@ -86,26 +121,36 @@
     FISHING = 13
     FIST_FIGHTING = 11
     MAGIC_LEVEL = 1
     SHIELDING = 6
     SWORD_FIGHTING = 8
 
 
+class PvpTypeFilter(NumericEnum):
+    """The possible PVP filters that can be used for auctions."""
+
+    OPEN_PVP = 0
+    OPTIONAL_PVP = 1
+    HARDCORE_PVP = 2
+    RETRO_OPEN_PVP = 3
+    RETRO_HARDCORE_PVP = 4
+
+
 class AuctionSearchType(NumericEnum):
     """The possible search types."""
 
     ITEM_DEFAULT = 0
     """Searches everything that includes the words on the search string."""
     ITEM_WILDCARD = 1
     """Searches everything that includes the search string"""
     CHARACTER_NAME = 2
     """Searches a character's name."""
 
 
-class AuctionStatus(BaseEnum):
+class AuctionStatus(StringEnum):
     """The possible values an auction might have."""
 
     IN_PROGRESS = 'in progress'
     """The auction is currently active.
 
     Notes
     -----
@@ -116,14 +161,45 @@
     """The auction was finished and was paid, but the character hasn't been transferred to the new owner yet."""
     CANCELLED = 'cancelled'
     """The auction was cancelled as no payment was received in time."""
     FINISHED = 'finished'
     """The auction either finished with no bids or the character was transferred to the new owner already."""
 
 
+class AuctionSkillFilter(NumericEnum):
+    """The different skill filters for auctions."""
+
+    AXE_FIGHTING = 10
+    CLUB_FIGHTING = 9
+    DISTANCE_FIGHTING = 7
+    FISHING = 13
+    FIST_FIGHTING = 11
+    MAGIC_LEVEL = 1
+    SHIELDING = 6
+    SWORD_FIGHTING = 8
+
+
+class AuctionVocationFilter(NumericEnum):
+    """The possible vocation filters for auctions."""
+
+    NONE = 1
+    DRUID = 2
+    KNIGHT = 3
+    PALADIN = 4
+    SORCERER = 5
+
+
+class AvailableForumSection(StringEnum):
+    WORLD_BOARDS = "worldboards"
+    TRADE_BOARDS = "tradeboards"
+    COMMUNITY_BOARDS = "communityboards"
+    SUPPORT_BOARDS = "supportboards"
+    GUILD_BOARDS = "guildboards"
+
+
 class BattlEyeType(NumericEnum):
     """The possible BattlEye statuses a world can have.
 
     .. versionadded:: 4.0.0
     """
 
     UNPROTECTED = 0
@@ -134,15 +210,38 @@
     """Worlds protected from the beginning, represented by a green symbol."""
     YELLOW = PROTECTED
     """Alias for protected worlds."""
     GREEN = INITIALLY_PROTECTED
     """Alias for initially protected worlds."""
 
 
-class BattlEyeHighscoresFilter(NumericEnum):
+class BazaarType(StringEnum):
+    """The possible bazaar types."""
+
+    CURRENT = "Current Auctions"
+    HISTORY = "Auction History"
+
+    @property
+    def subtopic(self):
+        return "currentcharactertrades" if self == self.CURRENT else "pastcharactertrades"
+
+
+class BidType(StringEnum):
+    """The possible bid types for an auction."""
+
+    MINIMUM = "Minimum Bid"
+    """The minimum bid set by the auction author, meaning the auction hasn't received any bids or it finished
+     without bids."""
+    CURRENT = "Current Bid"
+    """The current maximum bid, meaning the auction has received at least one bid."""
+    WINNING = "Winning Bid"
+    """The bid that won the auction."""
+
+
+class HighscoresBattlEyeType(NumericEnum):
     """The possible BattlEye filters that can be used for highscores."""
 
     ANY_WORLD = -1
     """Show all worlds."""
 
     INITIALLY_PROTECTED = 2
     """Worlds protected from the beginning, represented by a green symbol."""
@@ -158,55 +257,15 @@
     GREEN = INITIALLY_PROTECTED
     """Alias for initially protected worlds.
 
     .. versionadded:: 4.0.0
     """
 
 
-class BattlEyeTypeFilter(NumericEnum):
-    """The possible BattlEye filters that can be used for auctions."""
-
-    INITIALLY_PROTECTED = 1
-    """Worlds protected from the beginning, represented by a green symbol."""
-    PROTECTED = 2
-    """Worlds protected after the world was created, represented by a yellow symbol."""
-    NOT_PROTECTED = 3
-    """Worlds without any BattlEye protection."""
-    YELLOW = PROTECTED
-    """Alias for protected worlds.
-
-    .. versionadded:: 4.0.0
-    """
-    GREEN = INITIALLY_PROTECTED
-    """Alias for initially protected worlds.
-
-    .. versionadded:: 4.0.0
-    """
-
-
-class BazaarType(BaseEnum):
-    """The possible bazaar types."""
-
-    CURRENT = "Current Auctions"
-    HISTORY = "Auction History"
-
-
-class BidType(BaseEnum):
-    """The possible bid types for an auction."""
-
-    MINIMUM = "Minimum Bid"
-    """The minimum bid set by the auction author, meaning the auction hasn't received any bids or it finished
-     without bids."""
-    CURRENT = "Current Bid"
-    """The current maximum bid, meaning the auction has received at least one bid."""
-    WINNING = "Winning Bid"
-    """The bid that won the auction."""
-
-
-class Category(NumericEnum):
+class HighscoresCategory(NumericEnum):
     """The different highscores categories."""
 
     ACHIEVEMENTS = 1
     AXE_FIGHTING = 2
     BOSS_POINTS = 15
     CHARM_POINTS = 3
     CLUB_FIGHTING = 4
@@ -218,140 +277,178 @@
     GOSHNARS_TAINT = 9
     LOYALTY_POINTS = 10
     MAGIC_LEVEL = 11
     SHIELDING = 12
     SWORD_FIGHTING = 13
 
 
-class HouseOrder(BaseEnum):
+class HighscoresProfession(NumericEnum):
+    """The vocation filters available for Highscores.
+
+    The numeric values are what the highscores form accepts.
+    """
+
+    ALL = 0
+    NONE = 1
+    KNIGHTS = 2
+    PALADINS = 3
+    SORCERERS = 4
+    DRUIDS = 5
+
+    @classmethod
+    def from_name(cls, name, all_fallback=True):
+        """Get a vocation filter from a vocation's name.
+
+        Parameters
+        ----------
+        name: :class:`str`
+            The name of the vocation.
+        all_fallback: :class:`bool`
+            Whether to return :py:attr:`ALL` if no match is found. Otherwise, :obj:`None` will be returned.
+
+        Returns
+        -------
+        HighscoresProfession, optional:
+            The matching vocation filter.
+        """
+        name = name.upper()
+        for vocation in cls:  # type: HighscoresProfession
+            if vocation.name in name or vocation.name[:-1] in name and vocation != cls.ALL:
+                return vocation
+        if all_fallback or name.upper() == "ALL":
+            return cls.ALL
+        return None
+
+
+class HouseOrder(StringEnum):
     """The possible ordering methods for house lists in Tibia.com"""
 
     NAME = "name"
     SIZE = "size"
     RENT = "rent"
     BID = "bid"
     AUCTION_END = "end"
 
 
-class HouseStatus(BaseEnum):
+class HouseStatus(StringEnum):
     """Renting statuses of a house."""
 
     RENTED = "rented"
     AUCTIONED = "auctioned"
 
 
-class HouseType(BaseEnum):
+class HouseType(StringEnum):
     """The types of house available."""
 
     HOUSE = "house"
     GUILDHALL = "guildhall"
 
     @property
     def plural(self):
         """:class:`str`: The plural for the house type."""
         return f"{self.value}s"
 
 
-class NewsCategory(BaseEnum):
+class NewsCategory(StringEnum):
     """The different news categories."""
 
     CIPSOFT = "cipsoft"
     COMMUNITY = "community"
     DEVELOPMENT = "development"
     SUPPORT = "support"
     TECHNICAL_ISSUES = "technical"
 
     @property
     def filter_name(self):
         return f"filter_{self.value}"
 
+    @property
+    def big_icon_url(self):
+        from tibiapy.urls import get_static_file_url
+        return get_static_file_url("images", "global", "content", f"newsicon_{self.value}_big.gif")
+
+    @property
+    def small_icon_url(self):
+        from tibiapy.urls import get_static_file_url
+        return get_static_file_url("images", "global", "content", f"newsicon_{self.value}_small.gif")
+
 
-class NewsType(BaseEnum):
+class NewsType(StringEnum):
     """The different types of new entries."""
 
     NEWS_TICKER = "News Ticker"
     FEATURED_ARTICLE = "Featured Article"
     NEWS = "News"
 
     @property
     def filter_name(self):
         return f"filter_{self.value.split(' ')[-1].lower()}"
 
+    @property
+    def filter_value(self):
+        return self.value.split(" ")[-1].lower()
+
 
-class PvpType(BaseEnum):
+class PvpType(StringEnum):
     """The possible PvP types a World can have."""
 
     OPEN_PVP = "Open PvP"
     OPTIONAL_PVP = "Optional PvP"
     RETRO_OPEN_PVP = "Retro Open PvP"
     RETRO_HARDCORE_PVP = "Retro Hardcore PvP"
     HARDCORE_PVP = "Hardcore PvP"
 
 
-class PvpTypeFilter(NumericEnum):
-    """The possible PVP filters that can be used for auctions."""
-
-    OPEN_PVP = 0
-    OPTIONAL_PVP = 1
-    HARDCORE_PVP = 2
-    RETRO_OPEN_PVP = 3
-    RETRO_HARDCORE_PVP = 4
-
-
-class Sex(BaseEnum):
+class Sex(StringEnum):
     """Possible character sexes."""
 
     MALE = "male"
     FEMALE = "female"
 
 
-class SkillFilter(NumericEnum):
-    """The different skill filters for auctions."""
-
-    AXE_FIGHTING = 10
-    CLUB_FIGHTING = 9
-    DISTANCE_FIGHTING = 7
-    FISHING = 13
-    FIST_FIGHTING = 11
-    MAGIC_LEVEL = 1
-    SHIELDING = 6
-    SWORD_FIGHTING = 8
-
-
-class SpellGroup(BaseEnum):
+class SpellGroup(StringEnum):
     """The possible cooldown groups.
 
     Note that secondary groups are not enumerated.
     """
 
     ATTACK = "Attack"
     HEALING = "Healing"
     SUPPORT = "Support"
 
 
-class SpellType(BaseEnum):
-    """The possible spell types."""
-
-    INSTANT = "Instant"
-    RUNE = "Rune"
-
-
-class SpellSorting(BaseEnum):
+class SpellSorting(StringEnum):
     """The different sorting options for the spells section."""
 
     NAME = "name"
     GROUP = "group"
     TYPE = "type"
     EXP_LEVEL = "level"
     MANA = "mana"
     PRICE = "price"
     PREMIUM = "premium"
 
 
-class ThreadStatus(enum.Flag):
+class SpellType(StringEnum):
+    """The possible spell types."""
+
+    INSTANT = "Instant"
+    RUNE = "Rune"
+
+
+class SpellVocationFilter(StringEnum):
+    """The possible vocation types to filter out spells."""
+
+    DRUID = "Druid"
+    KNIGHT = "Knight"
+    PALADIN = "Paladin"
+    SORCERER = "Sorcerer"
+
+
+class ThreadStatus(Flag):
     """The possible status a thread can have.
 
     Threads can have a combination of multiple status. The numeric values are arbitrary.
     """
 
     NONE = 0
     HOT = 1  #: Thread has more than 16 replies.
@@ -398,107 +495,47 @@
         for entry in list(cls):
             if entry.name.lower() in icon:
                 flags += entry.value
         # noinspection PyArgumentList
         return cls(flags)
 
 
-class TournamentWorldType(BaseEnum):
-    """The possible types of tournament worlds."""
-
-    REGULAR = "Regular"
-    RESTRICTED = "Restricted Store"
-
-
-class TournamentPhase(BaseEnum):
-    """The possible tournament phases."""
-
-    SIGN_UP = "sign up"
-    RUNNING = "running"
-    ENDED = "ended"
-
-
-class TransferType(BaseEnum):
+class TransferType(StringEnum):
     """The possible special transfer restrictions a world may have."""
 
     REGULAR = "regular"  #: No special transfer restrictions
     BLOCKED = "blocked"  #: Can't transfer to this world, but can transfer out of this world.
     LOCKED = "locked"  #: Can transfer to this world, but can't transfer out of this world.
 
 
-class Vocation(BaseEnum):
+class Vocation(StringEnum):
     """The possible vocation types."""
 
     NONE = "None"
     DRUID = "Druid"
     KNIGHT = "Knight"
     PALADIN = "Paladin"
     SORCERER = "Sorcerer"
     ELDER_DRUID = "Elder Druid"
     ELITE_KNIGHT = "Elite Knight"
     ROYAL_PALADIN = "Royal Paladin"
     MASTER_SORCERER = "Master Sorcerer"
 
-
-class VocationAuctionFilter(NumericEnum):
-    """The possible vocation filters for auctions."""
-
-    NONE = 1
-    DRUID = 2
-    KNIGHT = 3
-    PALADIN = 4
-    SORCERER = 5
-
-
-class VocationFilter(NumericEnum):
-    """The vocation filters available for Highscores.
-
-    The numeric values are what the highscores form accepts.
-    """
-
-    ALL = 0
-    NONE = 1
-    KNIGHTS = 2
-    PALADINS = 3
-    SORCERERS = 4
-    DRUIDS = 5
-
-    @classmethod
-    def from_name(cls, name, all_fallback=True):
-        """Get a vocation filter from a vocation's name.
-
-        Parameters
-        ----------
-        name: :class:`str`
-            The name of the vocation.
-        all_fallback: :class:`bool`
-            Whether to return :py:attr:`ALL` if no match is found. Otherwise, :obj:`None` will be returned.
-
-        Returns
-        -------
-        VocationFilter, optional:
-            The matching vocation filter.
-        """
-        name = name.upper()
-        for vocation in cls:  # type: VocationFilter
-            if vocation.name in name or vocation.name[:-1] in name and vocation != cls.ALL:
-                return vocation
-        if all_fallback or name.upper() == "ALL":
-            return cls.ALL
-        return None
-
-
-class VocationSpellFilter(BaseEnum):
-    """The possible vocation types to filter out spells."""
-
-    DRUID = "Druid"
-    KNIGHT = "Knight"
-    PALADIN = "Paladin"
-    SORCERER = "Sorcerer"
+    @property
+    def base(self):
+        if self == self.ELDER_DRUID:
+            return self.DRUID
+        elif self == self.MASTER_SORCERER:
+            return self.SORCERER
+        elif self == self.ROYAL_PALADIN:
+            return self.PALADIN
+        elif self == self.ELITE_KNIGHT:
+            return self.KNIGHT
+        return self
 
 
-class WorldLocation(BaseEnum):
+class WorldLocation(StringEnum):
     """The possible physical locations for servers."""
 
     EUROPE = "Europe"
     NORTH_AMERICA = "North America"
     SOUTH_AMERICA = "South America"
```

### Comparing `tibia.py-5.6.0/tibiapy/errors.py` & `tibia.py-6.0.0a1/tibiapy/errors.py`

 * *Files identical despite different names*

### Comparing `tibia.py-5.6.0/tibiapy/highscores.py` & `tibia.py-6.0.0a1/tibiapy/parsers/character.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,381 +1,389 @@
-"""Models related to the highscores section in Tibia.com."""
-import datetime
+"""Models related to the Tibia.com character page."""
+from __future__ import annotations
+
 import re
 from collections import OrderedDict
-from typing import List, Optional
+from typing import List, TYPE_CHECKING
 
-from tibiapy import abc
-from tibiapy.enums import Category, Vocation, VocationFilter, BattlEyeTypeFilter, PvpTypeFilter, \
-    BattlEyeHighscoresFilter
+from tibiapy.builders.character import CharacterBuilder
+from tibiapy.enums import Sex, Vocation
 from tibiapy.errors import InvalidContent
-from tibiapy.utils import get_tibia_url, parse_form_data, parse_tibiacom_content, try_enum, parse_integer
-
-__all__ = (
-    "Highscores",
-    "HighscoresEntry",
-    "LoyaltyHighscoresEntry",
-)
-
-results_pattern = re.compile(r'Results: ([\d,]+)')
-numeric_pattern = re.compile(r'(\d+)')
+from tibiapy.models import Achievement, Character, AccountBadge, AccountInformation, OtherCharacter, DeathParticipant, \
+    Death, GuildMembership, CharacterHouse
+from tibiapy.utils import (parse_popup, parse_tibia_date, parse_tibia_datetime, parse_tibiacom_content, split_list,
+                           try_enum, parse_link_info, clean_text, parse_integer)
+
+if TYPE_CHECKING:
+    import bs4
+
+# Extracts the scheduled deletion date of a character."""
+deleted_regexp = re.compile(r'([^,]+), will be deleted at (.*)')
+# Extracts the death's level and killers.
+death_regexp = re.compile(r'Level (?P<level>\d+) by (?P<killers>.*)\.</td>')
+# From the killers list, filters out the assists.
+death_assisted = re.compile(r'(?P<killers>.+)\.<br/>Assisted by (?P<assists>.+)')
+# From a killer entry, extracts the summoned creature
+death_summon = re.compile(r'(?P<summon>an? .+) of (?P<name>[^<]+)')
+link_search = re.compile(r'<a[^>]+>[^<]+</a>')
+# Extracts the contents of a tag
+link_content = re.compile(r'>([^<]+)<')
 
+house_regexp = re.compile(r'paid until (.*)')
 
-class Highscores(abc.Serializable):
-    """Represents the highscores of a world.
+title_regexp = re.compile(r'(.*)\((\d+) titles? unlocked\)')
+badge_popup_regexp = re.compile(r"\$\(this\),\s+'([^']+)',\s+'([^']+)',")
 
-    .. versionadded:: 1.1.0
+traded_label = "(traded)"
 
-    Attributes
-    ----------
-    world: :class:`str`
-        The world the highscores belong to. If this is :obj:`None`, the highscores shown are for all worlds.
-    category: :class:`Category`
-        The selected category to displays the highscores of.
-    vocation: :class:`VocationFilter`
-        The selected vocation to filter out values.
-    battleye_filter: :class:`BattlEyeHighscoresFilter`
-        The selected BattlEye filter. If :obj:`None`, all worlds will be displayed.
-
-        Only applies for global highscores. Only characters from worlds with the matching BattlEye protection will be
-        shown.
-    pvp_types_filter: :class:`list` of :class:`PvpTypeFilter`
-        The selected PvP types filter. If :obj:`None`, all world will be displayed.
-
-        Only applies for global highscores. Only characters from worlds with the matching PvP type will be shown.
-    page: :class:`int`
-        The page number being displayed.
-    total_pages: :class:`int`
-        The total number of pages.
-    results_count: :class:`int`
-        The total amount of highscores entries in this category. These may be shown in another page.
-    last_updated: :class:`datetime.timedelta`
-        How long ago were this results updated. The resolution is 1 minute.
-    entries: :class:`list` of :class:`HighscoresEntry`
-        The highscores entries found.
-    available_worlds: :class:`list` of :class:`str`
-        The worlds available for selection.
-    """
-
-    _ENTRIES_PER_PAGE = 50
-
-    def __init__(self, world, category=Category.EXPERIENCE, **kwargs):
-        self.world: Optional[str] = world
-        self.category: Category = try_enum(Category, category, Category.EXPERIENCE)
-        self.vocation: VocationFilter = try_enum(VocationFilter, kwargs.get("vocation"), VocationFilter.ALL)
-        self.battleye_filter: Optional[BattlEyeTypeFilter] = try_enum(BattlEyeTypeFilter, kwargs.get("battleye_filter"))
-        self.pvp_types_filter: List[PvpTypeFilter] = kwargs.get("pvp_types_filter", [])
-        self.entries: List[HighscoresEntry] = kwargs.get("entries", [])
-        self.results_count: int = kwargs.get("results_count", 0)
-        self.page: int = kwargs.get("page", 1)
-        self.total_pages: int = kwargs.get("total_pages", 1)
-
-    __slots__ = (
-        'world',
-        'category',
-        'vocation',
-        'battleye_filter',
-        "pvp_types_filter",
-        'page',
-        'total_pages',
-        'results_count',
-        'last_updated',
-        'entries',
-        'available_worlds',
-    )
-
-    _serializable_properties = (
-
-    )
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} world={self.world!r} category={self.category!r} vocation={self.vocation!r}>"
-
-    @property
-    def from_rank(self):
-        """:class:`int`: The starting rank of the provided entries."""
-        return self.entries[0].rank if self.entries else 0
-
-    @property
-    def to_rank(self):
-        """:class:`int`: The last rank of the provided entries."""
-        return self.entries[-1].rank if self.entries else 0
-
-    @property
-    def url(self):
-        """:class:`str`: The URL to the highscores page on Tibia.com containing the results."""
-        return self.get_url(self.world, self.category, self.vocation, self.page, self.battleye_filter,
-                            self.pvp_types_filter)
-
-    @property
-    def previous_page_url(self):
-        """:class:`str`: The URL to the previous page of the current highscores, if there's any."""
-        return self.get_page_url(self.page - 1) if self.page > 1 else None
-
-    @property
-    def next_page_url(self):
-        """:class:`str`: The URL to the next page of the current highscores, if there's any."""
-        return self.get_page_url(self.page + 1) if self.page < self.total_pages else None
-
-    def get_page_url(self, page):
-        """Get the URL to a specific page for the current highscores.
-
-        Parameters
-        ----------
-        page: :class:`int`
-            The page to get the URL for.
+__all__ = (
+    "CharacterParser",
+)
 
-        Returns
-        -------
-        :class:`str`
-            The URL to the page of the current highscores.
 
-        Raises
-        ------
-        ValueError
-            The provided page is less or equals than zero.
-        """
-        if page <= 0:
-            raise ValueError("page cannot be less or equals than zero")
-        return self.get_url(self.world, self.category, self.vocation, page, self.battleye_filter, self.pvp_types_filter)
+class CharacterParser:
 
     @classmethod
     def from_content(cls, content):
-        """Create an instance of the class from the html content of a highscores page.
-
-        Notes
-        -----
-        Tibia.com only shows up to 50 entries per page, so in order to obtain the full highscores, all pages must be
-        obtained individually and merged into one.
+        """Create an instance of the class from the html content of the character's page.
 
         Parameters
         ----------
         content: :class:`str`
             The HTML content of the page.
 
         Returns
         -------
-        :class:`Highscores`
-            The highscores results contained in the page.
+        :class:`Character`
+            The character contained in the page, or None if the character doesn't exist
 
         Raises
         ------
         InvalidContent
-            If content is not the HTML of a highscore's page.
+            If content is not the HTML of a character's page.
         """
         parsed_content = parse_tibiacom_content(content)
-        form = parsed_content.find("form")
         tables = cls._parse_tables(parsed_content)
-        if form is None or "Highscores" not in tables:
-            if "Error" in tables and "The world doesn't exist!" in tables["Error"].text:
+        builder = CharacterBuilder()
+        if not tables:
+            messsage_table = parsed_content.select_one("div.TableContainer")
+            if messsage_table and "Could not find character" in messsage_table.text:
                 return None
-            raise InvalidContent("content does is not from the highscores section of Tibia.com")
-        highscores = cls(None)
-        highscores._parse_filters_table(form)
-        last_update_container = parsed_content.find("span", attrs={"class": "RightArea"})
-        if last_update_container:
-            m = numeric_pattern.search(last_update_container.text)
-            highscores.last_updated = datetime.timedelta(minutes=int(m.group(1))) if m else datetime.timedelta()
-        entries_table = tables.get("Highscores")
-        highscores._parse_entries_table(entries_table)
-        return highscores
+        if "Character Information" in tables.keys():
+            cls._parse_character_information(builder, tables["Character Information"])
+        else:
+            raise InvalidContent("content does not contain a tibia.com character information page.")
+        builder.achievements(cls._parse_achievements(tables.get("Account Achievements", [])))
+        if "Account Badges" in tables:
+            builder.account_badges(cls._parse_badges(tables["Account Badges"]))
+        cls._parse_deaths(builder, tables.get("Character Deaths", []))
+        builder.account_information(cls._parse_account_information(tables.get("Account Information", [])))
+        builder.other_characters(cls._parse_other_characters(tables.get("Characters", [])))
+        return builder.build()
 
     @classmethod
-    def get_url(cls, world=None, category=Category.EXPERIENCE, vocation=VocationFilter.ALL, page=1,
-                battleye_type=None, pvp_types=None):
-        """Get the Tibia.com URL of the highscores for the given parameters.
+    def _parse_account_information(cls, rows):
+        """Parse the character's account information.
 
         Parameters
         ----------
-        world: :class:`str`, optional
-            The game world of the desired highscores. If no world is passed, ALL worlds are shown.
-        category: :class:`Category`
-            The desired highscores category.
-        vocation: :class:`VocationFilter`
-            The vocation filter to apply. By default all vocations will be shown.
-        page: :class:`int`
-            The page of highscores to show.
-        battleye_type: :class:`BattlEyeHighscoresFilter`, optional
-            The battleEye filters to use.
-        pvp_types: :class:`list` of :class:`PvpTypeFilter`, optional
-            The list of PvP types to filter the results for.
+        rows: :class:`list` of :class:`bs4.Tag`, optional
+            A list of all rows contained in the table.
+        """
+        acc_info = {}
+        if not rows:
+            return
+        for row in rows:
+            cols_raw = row.select('td')
+            cols = [ele.text.strip() for ele in cols_raw]
+            field, value = cols
+            field = field.replace("\xa0", "_").replace(" ", "_").replace(":", "").lower()
+            value = value.replace("\xa0", " ")
+            acc_info[field] = value
+        created = parse_tibia_datetime(acc_info["created"])
+        loyalty_title = None if acc_info["loyalty_title"] == "(no title)" else acc_info["loyalty_title"]
+        position = acc_info.get("position")
+        return AccountInformation(created=created, loyalty_title=loyalty_title, position=position)
 
-        Returns
-        -------
-        The URL to the Tibia.com highscores.
+    @classmethod
+    def _parse_achievements(cls, rows):
+        """Parse the character's displayed achievements.
+
+        Parameters
+        ----------
+        rows: :class:`list` of :class:`bs4.Tag`
+            A list of all rows contained in the table.
         """
-        pvp_types = pvp_types or []
-        pvp_params = [("worldtypes[]", p.value) for p in pvp_types]
-        return get_tibia_url("community", "highscores", *pvp_params, world=world, category=category.value,
-                             profession=vocation.value, currentpage=page,
-                             beprotection=battleye_type.value if battleye_type else None)
-
-    # region Private methods
-    def _parse_entries_table(self, table):
-        """Parse the table containing the highscore entries.
+        achievements = []
+        for row in rows:
+            cols = row.select('td')
+            if len(cols) != 2:
+                continue
+            field, value = cols
+            grade = str(field).count("achievement-grade-symbol")
+            name = value.text.strip()
+            secret_image = value.find("img")
+            secret = False
+            if secret_image:
+                secret = True
+            achievements.append(Achievement(name=name, grade=grade, secret=secret))
+        return achievements
+
+    @classmethod
+    def _parse_badges(cls, rows: List[bs4.Tag]):
+        """Parse the character's displayed badges.
 
         Parameters
         ----------
-        table: :class:`bs4.Tag`
-            The table containing the entries.
+        rows: :class:`list` of :class:`bs4.Tag`
+            A list of all rows contained in the table.
+        """
+        row = rows[0]
+        columns = row.select("td > span")
+        account_badges = []
+        for column in columns:
+            popup_span = column.select_one("span.HelperDivIndicator")
+            if not popup_span:
+                # Badges are visible, but none selected.
+                return []
+            popup = parse_popup(popup_span['onmouseover'])
+            name = popup[0]
+            description = popup[1].text
+            icon_image = column.select_one("img")
+            icon_url = icon_image['src']
+            account_badges.append(AccountBadge(name=name, icon_url=icon_url, description=description))
+        return account_badges
+
+    @classmethod
+    def _parse_character_information(cls, builder: CharacterBuilder, rows):
+        """
+        Parse the character's basic information and applies the found values.
+
+        Parameters
+        ----------
+        rows: :class:`list` of :class:`bs4.Tag`
+            A list of all rows contained in the table.
         """
-        entries = table.find_all("tr")
-        if entries is None:
-            return
-        _, header, *rows = entries
-        info_row = rows.pop()
-        pages_div, results_div = info_row.find_all("div")
-        page_links = pages_div.find_all("a")
-        listed_pages = [int(p.text) for p in page_links]
-        if listed_pages:
-            self.page = next((x for x in range(1, listed_pages[-1] + 1) if x not in listed_pages), listed_pages[-1] + 1)
-            self.total_pages = max(int(page_links[-1].text), self.page)
-        self.results_count = parse_integer(results_pattern.search(results_div.text).group(1))
         for row in rows:
-            cols_raw = row.find_all('td')
-            if "There is currently no data" in cols_raw[0].text:
+            cols_raw = row.select('td')
+            cols = [clean_text(ele) for ele in cols_raw]
+            field, value = cols
+            field = field.replace(":", "").lower()
+            if field == "name":
+                cls._parse_name_field(builder, value)
+            elif field == "title":
+                cls._parse_titles(builder, value)
+            elif field == "former names":
+                builder.former_names([fn.strip() for fn in value.split(",")])
+            elif field == "former world":
+                builder.former_world(value)
+            elif field == "sex":
+                builder.sex(try_enum(Sex, value))
+            elif field == "vocation":
+                builder.vocation(try_enum(Vocation, value))
+            elif field == "level":
+                builder.level(parse_integer(value))
+            elif field == "achievement points":
+                builder.achievement_points(parse_integer(value))
+            elif field == "world":
+                builder.world(value)
+            elif field == "residence":
+                builder.residence(value)
+            elif field == "last login":
+                if "never logged" in value.lower():
+                    builder.last_login(None)
+                else:
+                    builder.last_login(parse_tibia_datetime(value))
+            elif field == "position":
+                builder.position(value)
+            elif field == "comment":
+                builder.comment(value)
+            elif field == "account status":
+                builder.is_premium("premium" in value.lower())
+            elif field == "married to":
+                builder.married_to(value)
+            elif field == "house":
+                cls._parse_house_column(builder, cols_raw[1])
+            elif field == "guild membership":
+                cls._parse_guild_column(builder, cols_raw[1])
+
+    @classmethod
+    def _parse_name_field(cls, builder: CharacterBuilder, value: str):
+        if m := deleted_regexp.match(value):
+            value = m.group(1)
+            builder.name(value)
+            builder.deletion_date(parse_tibia_datetime(m.group(2)))
+        else:
+            builder.name(value)
+
+        if traded_label in value:
+            builder.name(value.replace(traded_label, "").strip())
+            builder.traded(True)
+
+    @classmethod
+    def _parse_titles(cls, builder: CharacterBuilder, value: str):
+        if m := title_regexp.match(value):
+            name = m.group(1).strip()
+            unlocked = int(m.group(2))
+            if name == "None":
+                name = None
+            builder.title(name)
+            builder.unlocked_titles(unlocked)
+
+    @classmethod
+    def _parse_house_column(cls, builder: CharacterBuilder, column: bs4.Tag):
+        house_text = clean_text(column)
+        m = house_regexp.search(house_text)
+        paid_until = m.group(1)
+        paid_until_date = parse_tibia_date(paid_until)
+        house_link_tag = column.find('a')
+        house_link = parse_link_info(house_link_tag)
+        builder.add_house(
+            CharacterHouse(
+                id=house_link["query"]["houseid"],
+                name=house_link["text"],
+                town=house_link["query"]["town"],
+                paid_until_date=paid_until_date,
+                world=house_link["query"]["world"]
+            )
+        )
+
+    @classmethod
+    def _parse_guild_column(cls, builder: CharacterBuilder, column: bs4.Tag):
+        guild_link = column.select_one('a')
+        value = clean_text(column)
+        rank = value.split("of the")[0]
+        builder.guild_membership(GuildMembership(name=guild_link.text.replace("\xa0", " "), rank=rank.strip()))
+
+    @classmethod
+    def _parse_deaths(cls, builder: CharacterBuilder, rows):
+        """Parse the character's recent deaths.
+
+        Parameters
+        ----------
+        rows: :class:`list` of :class:`bs4.Tag`
+            A list of all rows contained in the table.
+        """
+        for row in rows:
+            cols = row.select('td')
+            if len(cols) != 2:
+                builder.deaths_truncated(True)
                 break
-            if cols_raw[0].text == "Rank":
+            date_column, desc_column = cols
+            death_time = parse_tibia_datetime(date_column.text)
+            if not (death_info := death_regexp.search(str(desc_column))):
                 continue
-            if len(cols_raw) <= 2:
-                break
-            self._parse_entry(cols_raw)
+            level = int(death_info.group("level"))
+            killers_desc = death_info.group("killers")
+            assists_name_list = []
+            # Check if the killers list contains assists
+            if assist_match := death_assisted.search(killers_desc):
+                # Filter out assists
+                killers_desc = assist_match.group("killers")
+                # Split assists into a list.
+                assists_desc = assist_match.group("assists")
+                assists_name_list = link_search.findall(assists_desc)
+            killers_name_list = split_list(killers_desc)
+            killers_list = [cls._parse_killer(k) for k in killers_name_list]
+            assists_list = [cls._parse_killer(k) for k in assists_name_list]
+            builder.add_death(Death(
+                level=level,
+                killers=killers_list,
+                assists=assists_list,
+                time=death_time
+            ))
 
-    def _parse_filters_table(self, form):
+    @classmethod
+    def _parse_killer(cls, killer):
+        """Parse a killer into a dictionary.
+
+        Parameters
+        ----------
+        killer: :class:`str`
+            The killer's raw HTML string.
+
+        Returns
+        -------
+        :class:`dict`: A dictionary containing the killer's info.
         """
-        Parse the filters table found in a highscores page.
+        # If the killer contains a link, it is a player.
+        name = clean_text(killer)
+        player = False
+        traded = False
+        summon = None
+        if traded_label in killer:
+            name = killer.replace('\xa0', ' ').replace(traded_label, "").strip()
+            traded = True
+            player = True
+        if "href" in killer:
+            m = link_content.search(killer)
+            name = clean_text(m.group(1))
+            player = True
+        # Check if it contains a summon.
+        if m := death_summon.search(name):
+            summon = clean_text(m.group("summon"))
+            name = clean_text(m.group("name"))
+        return DeathParticipant(name=name, player=player, summon=summon, traded=traded)
+
+    @classmethod
+    def _parse_other_characters(cls, rows):
+        """Parse the character's other visible characters.
 
         Parameters
         ----------
-        form: :class:`bs4.Tag`
-            The table containing the filters.
+        rows: :class:`list` of :class:`bs4.Tag`
+            A list of all rows contained in the table.
         """
-        data = parse_form_data(form, include_options=True)
-        self.world = data["world"] if data.get("world") else None
-        self.battleye_filter = try_enum(BattlEyeHighscoresFilter, parse_integer(data.get("beprotection"), None))
-        self.category = try_enum(Category, parse_integer(data.get("category"), None))
-        self.vocation = try_enum(VocationFilter, parse_integer(data.get("profession"), None), VocationFilter.ALL)
-        checkboxes = form.find_all("input", {"type": "checkbox", "checked": "checked"})
-        values = [int(c["value"]) for c in checkboxes]
-        self.pvp_types_filter = [try_enum(PvpTypeFilter, v) for v in values]
-        self.available_words = [v for v in data["__options__"]["world"].values() if v]
+        other_characters = []
+        for row in rows[1:]:
+            cols_raw = row.select('td')
+            cols = [ele.text.strip() for ele in cols_raw]
+            if len(cols) != 4:
+                continue
+            name, world, status, *__ = cols
+            _, *name = name.replace("\xa0", " ").split(" ")
+            name = " ".join(name)
+            traded = False
+            if traded_label in name:
+                name = name.replace(traded_label, "").strip()
+                traded = True
+            main_img = cols_raw[0].select_one('img')
+            main = False
+            if main_img and main_img['title'] == "Main Character":
+                main = True
+            position = None
+            if "CipSoft Member" in status:
+                position = "CipSoft Member"
+            other_characters.append(OtherCharacter(name=name, world=world, online="online" in status,
+                                                   deleted="deleted" in status, main=main, position=position,
+                                                   traded=traded))
+        return other_characters
+
 
     @classmethod
     def _parse_tables(cls, parsed_content):
         """
-        Parse the information tables found in a highscores page.
+        Parse the information tables contained in a character's page.
 
         Parameters
         ----------
         parsed_content: :class:`bs4.BeautifulSoup`
             A :class:`BeautifulSoup` object containing all the content.
 
         Returns
         -------
-        :class:`OrderedDict`[:class:`str`, :class:`bs4.Tag`]
+        :class:`OrderedDict`[str, :class:`list`of :class:`bs4.Tag`]
             A dictionary containing all the table rows, with the table headers as keys.
         """
-        tables = parsed_content.find_all('div', attrs={'class': 'TableContainer'})
+        tables = parsed_content.select('table[width="100%"]')
         output = OrderedDict()
         for table in tables:
-            title = table.find("div", attrs={'class': 'Text'}).text
-            title = title.split("[")[0].strip()
-            title = re.sub(r'Last Update.*', '', title)
-            inner_table = table.find("div", attrs={'class': 'InnerTableContainer'})
-            output[title] = inner_table
+            container = table.find_parent("div", {"class": "TableContainer"})
+            if container:
+                caption_container = container.select_one("div.CaptionContainer")
+                title = caption_container.text.strip()
+                offset = 0
+            else:
+                title = table.select_one("td").text.strip()
+                offset = 1
+            output[title] = table.select("tr")[offset:]
         return output
-
-    def _parse_entry(self, cols):
-        """Parse an entry's row and adds the result to py:attr:`entries`.
-
-        Parameters
-        ----------
-        cols: :class:`bs4.ResultSet`
-            The list of columns for that entry.
-        """
-        rank, name, *values = [c.text.replace('\xa0', ' ').strip() for c in cols]
-        rank = int(rank)
-        extra = None
-        if self.category == Category.LOYALTY_POINTS:
-            extra, vocation, world, level, value = values
-        else:
-            vocation, world, level, value = values
-        value = int(value.replace(',', ''))
-        level = int(level)
-        if self.category == Category.LOYALTY_POINTS:
-            entry = LoyaltyHighscoresEntry(rank, name, vocation, world, level, value, extra)
-        else:
-            entry = HighscoresEntry(rank, name, vocation, world, level, value)
-        self.entries.append(entry)
-    # endregion
-
-
-class HighscoresEntry(abc.BaseCharacter, abc.Serializable):
-    """Represents a entry for the highscores.
-
-    Attributes
-    ----------
-    name: :class:`str`
-        The name of the character.
-    rank: :class:`int`
-        The character's rank in the respective highscores.
-    vocation: :class:`Vocation`
-        The character's vocation.
-    world: :class:`str`
-        The character's world.
-    level: :class:`int`
-        The character's level.
-    value: :class:`int`
-        The character's value for the highscores.
-    """
-
-    def __init__(self, rank, name, vocation, world, level, value):
-        self.name: str = name
-        self.rank: int = rank
-        self.vocation = try_enum(Vocation, vocation)
-        self.value: int = value
-        self.world: str = world
-        self.level: int = level
-
-    __slots__ = (
-        'rank',
-        'name',
-        'vocation',
-        'world',
-        'level',
-        'value',
-    )
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} rank={self.rank} name={self.name!r} value={self.value}>"
-
-
-class LoyaltyHighscoresEntry(HighscoresEntry):
-    """Represents a entry for the highscores loyalty points category.
-
-    This is a subclass of :class:`HighscoresEntry`, adding an extra field for title.
-
-    Attributes
-    ----------
-    name: :class:`str`
-        The name of the character.
-    rank: :class:`int`
-        The character's rank in the respective highscores.
-    vocation: :class:`Vocation`
-        The character's vocation.
-    world: :class:`str`
-        The character's world.
-    level: :class:`int`
-        The character's level.
-    value: :class:`int`
-        The character's loyalty points.
-    title: :class:`str`
-        The character's loyalty title.
-    """
-
-    def __init__(self, rank, name, vocation, world, level, value, title):
-        super().__init__(rank, name, vocation, world, level, value)
-        self.title: str = title
-
-    __slots__ = (
-        'title',
-    )
```

### Comparing `tibia.py-5.6.0/tibiapy/tournament.py` & `tibia.py-6.0.0a1/tibiapy/parsers/bazaar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,814 +1,628 @@
-"""Models related to the tournaments section in Tibia.com and the tournaments leaderboards."""
-import datetime
-import math
+"""Contains all classes related to the Character Bazaar sections in Tibia.com"""
+import logging
 import re
-from typing import List, TYPE_CHECKING
+import urllib.parse
+from typing import Dict
 
-from tibiapy import abc
-from tibiapy.enums import PvpType, TournamentPhase, Vocation
-from tibiapy.errors import InvalidContent
-from tibiapy.utils import get_tibia_url, parse_integer, parse_popup, parse_tibia_datetime, parse_tibia_full_date, \
-    parse_tibiacom_content, split_list, try_enum
-
-if TYPE_CHECKING:
-    import bs4
-
-__all__ = (
-    "TournamentLeaderboardEntry",
-    "TournamentEntry",
-    "RewardEntry",
-    "RuleSet",
-    "ScoreSet",
-    "Tournament",
-    "TournamentLeaderboard",
-)
-
-RANGE_PATTERN = re.compile(r'(\d+)(?:-(\d+))?')
-CUP_PATTERN = re.compile(r'(\w+ cup)')
-DEED_PATTERN = re.compile(r'(\w+ deed)')
-ARCHIVE_LIST_PATTERN = re.compile(r'([\w\s]+)\s\(([^-]+)-\s([^)]+)\)')
-RANK_PATTERN = re.compile(r'(\d+)\.\s\(\+?(-?\d+)\)')
-RESULTS_PATTERN = re.compile(r'Results: (\d+)')
-CURRENT_TOURNAMENT_PATTERN = re.compile(r'(?:.*- (\w+))')
-
-TOURNAMENT_LEADERBOARDS_URL = "https://www.tibia.com/community/?subtopic=tournamentleaderboard"
-
-
-class TournamentLeaderboardEntry(abc.BaseCharacter, abc.Serializable):
-    """Represents a single tournament leaderboard's entry.
-
-    .. versionadded:: 2.5.0
-
-    Attributes
-    ----------
-    name: :class:`str`
-        The character's name.
-    rank: :class:`int`
-        The entry's rank.
-    change: :class:`int`
-        The entry's change in rank since the last server save.
-    vocation: :class:`Vocation`
-        The character's vocation. This will always show the base vocation, without promotions.
-    score: :class:`int`
-        The entry's score.
-    """
-
-    __slots__ = (
-        "name",
-        "rank",
-        "change",
-        "vocation",
-        "score",
-    )
-
-    def __init__(self, **kwargs):
-        self.name: str = kwargs.get("name")
-        self.rank: int = kwargs.get("rank")
-        self.change: int = kwargs.get("change")
-        self.vocation: Vocation = kwargs.get("vocation")
-        self.score: int = kwargs.get("score")
-
-    def __repr__(self):
-        return "<{0.__class__.__name__} rank={0.rank} name={0.name!r} vocation={0.vocation!r} " \
-               "points={0.score}>".format(self)
-
-
-class TournamentEntry(abc.BaseTournament, abc.Serializable):
-    """Represents an tournament in the archived tournaments list.
-
-    :py:attr:`start_date` and :py:attr:`end_date` might be :obj:`None` when a tournament that is currently running
-    is on the list (e.g. on the leaderboards tournament selection section).
-
-    .. versionadded:: 2.5.0
-
-    Attributes
-    ----------
-    title: :class:`str`
-        The title of the tournament.
-    cycle: :class:`int`
-        An internal number used to get direct access to a specific tournament in the archive.
-    start_date: :class:`datetime.date`
-        The start date of the tournament.
-    end_date: :class:`datetime.date`
-        The end date of the tournament.
-    """
-
-    __slots__ = (
-        "title",
-        "cycle",
-        "start_date",
-        "end_date",
-    )
-
-    _serializable_properties = ("duration",)
-
-    def __init__(self, title, start_date, end_date, **kwargs):
-        self.title: str = title
-        self.start_date: datetime.date = start_date
-        self.end_date: datetime.date = end_date
-        self.cycle: int = kwargs.get("cycle", 0)
-
-    def __repr__(self):
-        return "<{0.__class__.__name__} title={0.title!r} cycle={0.cycle} start_date={0.start_date!r} " \
-               "end_date={0.end_date!r}>".format(self)
-
-    @property
-    def duration(self):
-        """:class:`datetime.timedelta`: The total duration of the tournament."""
-        if self.start_date and self.end_date:
-            return self.end_date - self.start_date
-        return None
-
-
-class RewardEntry(abc.Serializable):
-    """Represents the rewards for a specific rank range.
-
-    Attributes
-    ----------
-    initial_rank: :class:`int`
-        The highest rank that gets this reward.
-    last_rank: :class:`int`
-        The lowest rank that gets this reward.
-    tibia_coins: :class`int`
-        The amount of tibia coins awarded.
-    tournament_coins: :class:`int`
-        The amount of tournament coins awarded.
-    tournament_ticket_voucher: :class:`int`
-        The amount of tournament ticker vouchers awarded.
-    cup: :class:`str`
-        The type of cup awarded.
-    deed: :class:`str`
-        The type of deed awarded.
-    other_rewards: :class:`str`
-        Other rewards given for this rank.
-    """
-
-    __slots__ = (
-        "initial_rank",
-        "last_rank",
-        "tibia_coins",
-        "tournament_coins",
-        "tournament_ticker_voucher",
-        "cup",
-        "deed",
-        "other_rewards",
-    )
-
-    def __init__(self, **kwargs):
-        self.initial_rank = kwargs.get("initial_rank", 0)
-        self.last_rank = kwargs.get("last_rank", 0)
-        self.tibia_coins = kwargs.get("tibia_coins", 0)
-        self.tournament_coins = kwargs.get("tournament_coins", 0)
-        self.tournament_ticker_voucher = kwargs.get("tournament_ticker_voucher", 0)
-        self.cup = kwargs.get("cup")
-        self.deed = kwargs.get("deed")
-        self.other_rewards = kwargs.get("other_rewards")
-
-    def __repr__(self):
-        attributes = ""
-        for attr in self.__slots__:
-            v = getattr(self, attr)
-            attributes += f" {attr}={v!r}"
-        return f"<{self.__class__.__name__}{attributes}>"
-
-
-class RuleSet(abc.Serializable):
-    """Contains the tournament rule set.
-
-    Attributes
-    ----------
-    pvp_type: :class:`PvPType`
-        The PvP type of the tournament.
-    daily_tournament_playtime: :class:`datetime.timedelta`
-        The maximum amount of time participants can play each day.
-    total_tournament_playtime: :class:`datetime.timedelta`
-        The total amount of time participants can play in the tournament.
-    playtime_reduced_only_in_combat: :class:`bool`
-        Whether playtime will only be reduced while in combat or not.
-    death_penalty_modifier: :class:`float`
-        The modifier for the death penalty.
-    xp_multiplier: :class:`float`
-        The multiplier for experience gained.
-    skill_multiplier: :class:`float`
-        The multiplier for skill gained.
-    spawn_rate_multiplier: :class:`float`
-        The multiplier for the spawn rate.
-    loot_probability: :class:`float`
-        The multiplier for the loot rate.
-    rent_percentage: :class:`int`
-        The percentage of rent prices relative to the regular price.
-    house_auction_durations: :class:`int`
-        The duration of house auctions.
-    shared_xp_bonus: :class:`bool`
-        Whether there is a bonus for sharing experience or not.
-    """
-
-    __slots__ = (
-        "pvp_type",
-        "daily_tournament_playtime",
-        "total_tournament_playtime",
-        "playtime_reduced_only_in_combat",
-        "death_penalty_modifier",
-        "xp_multiplier",
-        "skill_multiplier",
-        "spawn_rate_multiplier",
-        "loot_probability",
-        "rent_percentage",
-        "house_auction_durations",
-        "shared_xp_bonus",
-    )
-
-    def __init__(self, **kwargs):
-        self.pvp_type = try_enum(PvpType, kwargs.get("pvp_type"))
-        self.daily_tournament_playtime = self._try_parse_interval(kwargs.get("daily_tournament_playtime"))
-        self.total_tournament_playtime = self._try_parse_interval(kwargs.get("total_tournament_playtime"))
-        self.playtime_reduced_only_in_combat = kwargs.get("playtime_reduced_only_in_combat")
-        self.death_penalty_modifier = kwargs.get("death_penalty_modifier")
-        self.xp_multiplier = kwargs.get("xp_multiplier")
-        self.skill_multiplier = kwargs.get("skill_multiplier")
-        self.spawn_rate_multiplier = kwargs.get("spawn_rate_multiplier")
-        self.loot_probability = kwargs.get("loot_probability")
-        self.rent_percentage = kwargs.get("rent_percentage")
-        self.house_auction_durations = kwargs.get("house_auction_durations")
-        self.shared_xp_bonus = kwargs.get("shared_xp_bonus")
-
-    def __repr__(self):
-        attributes = ""
-        for attr in self.__slots__:
-            v = getattr(self, attr)
-            attributes += f" {attr}={v!r}"
-        return f"<{self.__class__.__name__}{attributes}>"
-
-    @staticmethod
-    def _try_parse_interval(interval):
-        if interval is None:
-            return None
-        if isinstance(interval, datetime.timedelta):
-            return interval
-        try:
-            t = datetime.datetime.strptime(interval, "%H:%M:%S")
-            return datetime.timedelta(hours=t.hour, minutes=t.minute, seconds=t.second)
-        except ValueError:
-            return None
+import bs4
 
+from tibiapy import InvalidContent, Sex, Vocation
+from tibiapy.builders.bazaar import CharacterBazaarBuilder, AuctionBuilder, AuctionDetailsBuilder
+from tibiapy.enums import (AuctionOrderDirection, AuctionOrderBy, AuctionSearchType, AuctionStatus,
+                           AuctionBattlEyeFilter,
+                           BazaarType, BidType, PvpTypeFilter, AuctionSkillFilter, AuctionVocationFilter)
+from tibiapy.models.bazaar import AuctionFilters, ItemEntry, OutfitImage, SalesArgument, \
+    SkillEntry, BlessingEntry, CharmEntry, AchievementEntry, BestiaryEntry, MountEntry, ItemSummary, \
+    Mounts, Familiars, Outfits, FamiliarEntry, OutfitEntry, CharacterBazaar, Auction
+from tibiapy.models.pagination import AjaxPaginator
+from tibiapy.utils import (convert_line_breaks, parse_form_data, parse_integer, parse_pagination,
+                           parse_tibia_datetime, parse_tibiacom_content, try_enum)
+
+results_pattern = re.compile(r'Results: (\d+)')
+char_info_regex = re.compile(r'Level: (\d+) \| Vocation: ([\w\s]+)\| (\w+) \| World: (\w+)')
+id_addon_regex = re.compile(r'(\d+)_(\d)\.gif')
+id_regex = re.compile(r'(\d+).(?:gif|png)')
+description_regex = re.compile(r'"(?:an?\s)?([^"]+)"')
+amount_regex = re.compile(r'([\d,]+)x')
+tier_regex = re.compile(r"(.*)\s\(tier (\d)\)")
 
-class ScoreSet(abc.Serializable):
-    """Represents the ways to earn or lose points in the tournament.
+log = logging.getLogger("tibiapy")
 
-    .. versionadded:: 2.5.0
+class AuctionFiltersParser:
+    @classmethod
+    def _parse_filter_table(cls, table):
+        """Parse the filters table to extract its values.
 
-    Attributes
-    ----------
-    creature_kills: :class:`dict`
-        Points received for participating in creature kills.
-    level_gain_loss: :class:`int`
-        The points gained for leveling up or lost for losing a level.
-    skill_gain_loss: :class:`int`
-        The points gained for leveling up or lost for losing a skill level.
-    charm_point_multiplier: :class:`int`
-        The multiplier for every charm point.
-    character_death: :class:`int`
-        The points lost for dying.
-    area_discovery: :class:`int`
-        Points that will be added to the score for discovering an area entirely.
-    """
-
-    __slots__ = (
-        "creature_kills",
-        "level_gain_loss",
-        "skill_gain_loss",
-        "charm_point_multiplier",
-        "character_death",
-        "area_discovery",
-    )
-
-    def __init__(self, **kwargs):
-        self.creature_kills = kwargs.get("creature_kills", {})
-        self.level_gain_loss = kwargs.get("level_gain_loss", 0)
-        self.skill_gain_loss = kwargs.get("skill_gain_loss", 0)
-        self.charm_point_multiplier = kwargs.get("charm_point_multiplier", 0)
-        self.character_death = kwargs.get("character_death", 0)
-        self.area_discovery = kwargs.get("area_discovery", 0)
-
-    def __repr__(self):
-        attributes = ""
-        for attr in self.__slots__:
-            v = getattr(self, attr)
-            attributes += f" {attr}={v!r}"
-        return f"<{self.__class__.__name__}{attributes}>"
-
-
-class Tournament(abc.BaseTournament, abc.Serializable):
-    """Represents a tournament's information.
-
-    .. versionadded:: 2.5.0
-
-    Attributes
-    ----------
-    title: :class:`str`
-        The title of the tournament.
-    cycle: :class:`int`
-        An internal number used to get direct access to a specific tournament in the archive.
-
-        This will only be present when viewing an archived tournament, otherwise it will default to 0.
-    phase: :class:`TournamentPhase`
-        The current phase of the tournament.
-    start_date: :class:`datetime.datetime`
-        The start date of the tournament.
-    end_date: :class:`datetime.datetime`
-        The end date of the tournament.
-    worlds: :obj:`list` of :class:`str`
-        The worlds where this tournament is active on.
-    rule_set: :class:`RuleSet`
-        The specific rules for this tournament.
-    score_set: :class:`ScoreSet`
-        The ways to gain points in the tournament.
-    reward_set: :obj:`list` of :class:`RewardEntry`
-        The list of rewards awarded for the specified ranges.
-    archived_tournaments: :obj:`list` of :class:`TournamentEntry`
-        The list of other archived tournaments. This is only present when viewing an archived tournament.
-    """
-
-    __slots__ = (
-        "phase",
-        "start_date",
-        "end_date",
-        "worlds",
-        "rule_set",
-        "score_set",
-        "reward_set",
-        "archived_tournaments",
-    )
-
-    _serializable_properties = (
-        "duration",
-        "rewards_range",
-    )
-
-    def __init__(self, **kwargs):
-        self.title = kwargs.get("title")
-        self.cycle = kwargs.get("cycle", 0)
-        self.phase = try_enum(TournamentPhase, kwargs.get("phase"))
-        self.start_date: datetime.datetime = kwargs.get("start_date")
-        self.end_date: datetime.datetime = kwargs.get("end_date")
-        self.worlds: List[str] = kwargs.get("worlds")
-        self.rule_set: RuleSet = kwargs.get("rule_set")
-        self.score_set: ScoreSet = kwargs.get("score_set")
-        self.reward_set: List[RewardEntry] = kwargs.get("reward_set", [])
-        self.archived_tournaments: List[TournamentEntry] = kwargs.get("archived_tournaments", [])
-
-    def __repr__(self):
-        return ("<{0.__class__.__name__} title={0.title!r} phase={0.phase!r} start_date={0.start_date!r} "
-                "end_date={0.start_date!r}>").format(self)
-
-    @property
-    def rewards_range(self):
-        """:class:`tuple`:The range of ranks that might receive rewards."""
-        return (self.reward_set[0].initial_rank, self.reward_set[-1].last_rank) if self.reward_set else (0, 0)
-
-    @property
-    def duration(self):
-        """:class:`datetime.timedelta`: The total duration of the tournament."""
-        return self.end_date - self.start_date
+        Parameters
+        ----------
+        table: :class:`bs4.Tag`
+            The table containing the filters.
 
-    def rewards_for_rank(self, rank):
-        """Get the rewards for a given rank, if any.
+        Returns
+        -------
+        :class:`AuctionFilters`
+            The currently applied filters.
+        """
+        filters = AuctionFilters()
+        forms = table.select("form")
+        data = parse_form_data(forms[0], include_options=True)
+
+        filters.world = data["filter_world"]
+        filters.available_worlds = [w for w in data.get("__options__", {}).get("filter_world", []) if "(" not in w]
+        filters.pvp_type = try_enum(PvpTypeFilter, parse_integer(data.get("filter_worldpvptype"), None))
+        filters.battleye = try_enum(AuctionBattlEyeFilter, parse_integer(data.get("filter_worldbattleyestate"), None))
+        filters.vocation = try_enum(AuctionVocationFilter, parse_integer(data.get("filter_profession"), None))
+        filters.min_level = parse_integer(data.get("filter_levelrangefrom"), None)
+        filters.max_level = parse_integer(data.get("filter_levelrangeto"), None)
+        filters.skill = try_enum(AuctionSkillFilter, parse_integer(data.get("filter_skillid"), None))
+        filters.min_skill_level = parse_integer(data.get("filter_skillrangefrom"), None)
+        filters.max_skill_level = parse_integer(data.get("filter_skillrangeto"), None)
+        filters.order_by = try_enum(AuctionOrderBy, parse_integer(data.get("order_column"), None))
+        filters.order = try_enum(AuctionOrderDirection, parse_integer(data.get("order_direction"), None))
+        if len(forms) > 1:
+            data_search = parse_form_data(forms[1], include_options=True)
+            filters.search_string = data_search.get("searchstring")
+            filters.search_type = try_enum(AuctionSearchType, parse_integer(data_search.get("searchtype"), None))
+        return filters
+
+
+class CharacterBazaarParser:
+    @classmethod
+    def from_content(cls, content) -> CharacterBazaar:
+        """Get the bazaar's information and list of auctions from Tibia.com.
 
         Parameters
         ----------
-        rank: :class:`int`
-            The rank to check.
+        content: :class:`str`
+            The HTML content of the bazaar section at Tibia.com.
 
         Returns
         -------
-        :class:`RewardEntry`, optional:
-            The rewards for the given rank or None if there are no rewards.
+        :class:`CharacterBazaar`
+            The character bazaar with the entries found.
         """
-        for rewards in self.reward_set:
-            if rewards.initial_rank <= rank <= rewards.last_rank:
-                return rewards
-        return None
+        try:
+            parsed_content = parse_tibiacom_content(content, builder='html5lib')
+            content_table = parsed_content.select_one("div.BoxContent")
+            tables = content_table.select("div.TableContainer")
+            filter_table = None
+            if len(tables) == 1:
+                auctions_table = tables[0]
+            else:
+                filter_table, auctions_table, *_ = tables
+
+            builder = CharacterBazaarBuilder()
+            builder.type(BazaarType.CURRENT if filter_table else BazaarType.HISTORY)
+
+            if filter_table:
+                builder.filters(AuctionFiltersParser._parse_filter_table(filter_table))
+
+            if page_navigation_row := parsed_content.select_one("td.PageNavigation"):
+                page, total_pages, results_count = parse_pagination(page_navigation_row)
+                builder.current_page(page).total_pages(total_pages).results_count(results_count)
+
+            auction_rows = auctions_table.select("div.Auction")
+            for auction_row in auction_rows:
+                auction = AuctionParser._parse_auction(auction_row)
+
+                builder.add_entry(auction)
+            return builder.build()
+        except (ValueError, IndexError) as e:
+            raise InvalidContent("content does not belong to the bazaar at Tibia.com", original=e) from e
+
+
+class AuctionParser:
 
     @classmethod
-    def from_content(cls, content):
-        """Create an instance of the class from the html content of the tournament's page.
+    def from_content(cls, content, auction_id=0, skip_details=False):
+        """Parse an auction detail page from Tibia.com and extracts its data.
 
         Parameters
         ----------
         content: :class:`str`
-            The HTML content of the page.
+            The HTML content of the auction detail page in Tibia.com
+        auction_id: :class:`int`, optional
+            The ID of the auction.
+
+            It is not possible to extract the ID from the page's content, so it may be passed to assign it manually.
+        skip_details: :class:`bool`, optional
+            Whether to skip parsing the entire auction and only parse the information shown in lists. False by default.
+
+            This allows fetching basic information like name, level, vocation, world, bid and status, shaving off some
+            parsing time.
 
         Returns
         -------
-        :class:`Tournament`
-            The tournament contained in the page, or None if the tournament doesn't exist.
+        :class:`Auction`
+            The auction details if found, :obj:`None` otherwise.
 
         Raises
         ------
         InvalidContent
-            If content is not the HTML of a tournament's page.
+            If the content does not belong to a auction detail's page.
         """
-        try:
-            if "An internal error has occurred" in content:
+        parsed_content = parse_tibiacom_content(content, builder='html5lib' if not skip_details else 'lxml')
+        auction_row = parsed_content.select_one("div.Auction")
+        if not auction_row:
+            if "internal error" in content:
                 return None
-            if "Currently there is no Tournament running." in content:
-                return None
-            parsed_content = parse_tibiacom_content(content, builder='html5lib')
-            box_content = parsed_content.find("div", attrs={"class": "BoxContent"})
-            tables = box_content.find_all('table', attrs={"class": "Table5"})
-            archive_table = box_content.find('table', attrs={"class": "Table4"})
-            tournament_details_table = tables[-1]
-            info_tables = tournament_details_table.find_all('table', attrs={'class': 'TableContent'})
-            main_info = info_tables[0]
-            rule_set = info_tables[1]
-            score_set = info_tables[2]
-            reward_set = info_tables[3]
-            tournament = cls()
-            tournament._parse_tournament_info(main_info)
-            tournament._parse_tournament_rules(rule_set)
-            tournament._parse_tournament_scores(score_set)
-            tournament._parse_tournament_rewards(reward_set)
-            if archive_table:
-                tournament._parse_archive_list(archive_table)
-            return tournament
-        except IndexError as e:
-            raise InvalidContent("content does not belong to the Tibia.com's tournament section", e)
-
-    def _parse_tournament_info(self, table):
-        """Parse the tournament info table.
+            raise InvalidContent("content does not belong to a auction details page in Tibia.com")
+        auction = cls._parse_auction(auction_row)
+        builder = AuctionDetailsBuilder()
+        if skip_details:
+            return auction
+
+        details_tables = cls._parse_tables(parsed_content)
+        if "General" in details_tables:
+            cls._parse_general_table(builder, details_tables["General"])
+        if "ItemSummary" in details_tables:
+            builder.items(cls._parse_items_table(details_tables["ItemSummary"]))
+        if "StoreItemSummary" in details_tables:
+            builder.store_items(cls._parse_items_table(details_tables["StoreItemSummary"]))
+        if "Mounts" in details_tables:
+            builder.mounts(cls._parse_mounts_table(details_tables["Mounts"]))
+        if "StoreMounts" in details_tables:
+            builder.store_mounts(cls._parse_mounts_table(details_tables["StoreMounts"]))
+        if "Outfits" in details_tables:
+            builder.outfits(cls._parse_outfits_table(details_tables["Outfits"]))
+        if "StoreOutfits" in details_tables:
+            builder.store_outfits(cls._parse_outfits_table(details_tables["StoreOutfits"]))
+        if "Familiars" in details_tables:
+            builder.familiars(cls._parse_familiars_table(details_tables["Familiars"]))
+        if "Blessings" in details_tables:
+            cls._parse_blessings_table(builder, details_tables["Blessings"])
+        if "Imbuements" in details_tables:
+            builder.imbuements(cls._parse_single_column_table(details_tables["Imbuements"]))
+        if "Charms" in details_tables:
+            cls._parse_charms_table(builder, details_tables["Charms"])
+        if "CompletedCyclopediaMapAreas" in details_tables:
+            builder.completed_cyclopedia_map_areas(cls._parse_single_column_table(
+                details_tables["CompletedCyclopediaMapAreas"]))
+        if "CompletedQuestLines" in details_tables:
+            builder.completed_quest_lines(cls._parse_single_column_table(details_tables["CompletedQuestLines"]))
+        if "Titles" in details_tables:
+            builder.titles(cls._parse_single_column_table(details_tables["Titles"]))
+        if "Achievements" in details_tables:
+            cls._parse_achievements_table(builder, details_tables["Achievements"])
+        if "BestiaryProgress" in details_tables:
+            cls._parse_bestiary_table(builder, details_tables["BestiaryProgress"])
+        if "BosstiaryProgress" in details_tables:
+            cls._parse_bestiary_table(builder, details_tables["BosstiaryProgress"], True)
+        auction.details = builder.build()
+        return auction
 
-        Parameters
-        ----------
-        table: :class:`bs4.BeautifulSoup`
-            The parsed table containing the tournament's information.
-        """
-        rows = table.find_all('tr')
-        date_fields = ("start_date", "end_date")
-        list_fields = ("worlds",)
-        for row in rows:
-            cols_raw = row.find_all('td')
-            cols = [ele.text.strip() for ele in cols_raw]
-            field, value = cols
-            field = field.replace("\xa0", "_").replace(" ", "_").replace(":", "").lower()
-            value = value.replace("\xa0", " ")
-            if field in date_fields:
-                value = parse_tibia_datetime(value)
-            if field in list_fields:
-                value = split_list(value, ",", ",")
-            if field == "phase":
-                value = try_enum(TournamentPhase, value)
-            try:
-                setattr(self, field, value)
-            except AttributeError:
-                pass
-
-    def _parse_tournament_rules(self, table):
-        """Parse the tournament rules table.
-
-        Parameters
-        ----------
-        table: :class:`bs4.BeautifulSoup`
-            The table containing the tournament rule set.
-        """
-        rows = table.find_all('tr')
-        bool_fields = ("playtime_reduced_only_in_combat", "shared_xp_bonus")
-        float_fields = (
-            "death_penalty_modifier",
-            "xp_multiplier",
-            "skill_multiplier",
-            "spawn_rate_multiplier",
-            "loot_probability",
-        )
-        int_fields = ("rent_percentage", "house_auction_durations")
-        rules = {}
-        for row in rows[1:]:
-            cols_raw = row.find_all('td')
-            cols = [ele.text.strip() for ele in cols_raw]
-            field, value, *_ = cols
-            field = field.replace("\xa0", "_").replace(" ", "_").replace(":", "").lower()
-            value = value.replace("\xa0", " ")
-            if field in bool_fields:
-                value = value.lower() == "yes"
-            if field in float_fields:
-                value = float(value.replace("x", ""))
-            if field in int_fields:
-                value = int(value.replace("%", ""))
-            rules[field] = value
-        self.rule_set = RuleSet(**rules)
-
-    def _parse_tournament_scores(self, table):
-        """Parse the tournament scores table.
-
-        Parameters
-        ----------
-        table: :class:`bs4.BeautifulSoup`
-            The parsed table containing the tournament score set.
-        """
-        creatures = {}
-        rows = table.find_all('tr')
-        rules = {}
-        for row in rows[1:]:
-            cols_raw = row.find_all('td')
-            cols = [ele.text.strip() for ele in cols_raw]
-            field, value, *_ = cols
-            icon = cols_raw[2].find("span")
-            field = field.replace("\xa0", "_").replace(" ", "_").replace(":", "").replace("/", "_").lower()
-            value = re.sub(r'[^-0-9]', '', value.replace("+/-", ""))
-            if not icon:
-                creatures[field.replace("_", " ")] = int(value)
-            else:
-                rules[field] = parse_integer(value)
-        if "creature_kills" in rules:
-            rules["creature_kills"] = creatures
-        self.score_set = ScoreSet(**rules)
-
-    def _parse_tournament_rewards(self, table):
-        """Parse the reward section of the tournament information section.
+    @classmethod
+    def _parse_auction(cls, auction_row, auction_id=0) -> Auction:
+        """Parse an auction's table, extracting its data.
 
         Parameters
         ----------
-        table: :class:`bs4.BeautifulSoup`
-            The parsed table containing the information.
-        """
-        rows = table.find_all('tr')
-        rewards = []
-        for row in rows[1:]:
-            cols_raw = row.find_all('td')
-            rank_row, *rewards_cols = cols_raw
-            rank_text = rank_row.text
-            if not rank_text:
-                break
-            first, last = self._parse_rank_range(rank_text)
-            entry = RewardEntry(initial_rank=first, last_rank=last)
-            for col in rewards_cols:
-                self._parse_rewards_column(col, entry)
-            rewards.append(entry)
-        self.reward_set = rewards
-
-    @classmethod
-    def _parse_rewards_column(cls, column, entry):
-        """Parse a column from the tournament's reward section.
+        auction_row: :class:`bs4.Tag`
+            The row containing the auction's information.
+        auction_id: :class:`int`
+            The ID of the auction.
 
-        Parameters
-        ----------
-        column: :class:`bs4.BeautifulSoup`
-            The parsed content of the column.
-        entry: :class:`RewardEntry`
-            The reward entry where the data will be stored to.
-        """
-        col_str = str(column)
-        img = column.find('img')
-        if img and "tibiacoin" in img["src"]:
-            entry.tibia_coins = parse_integer(column.text)
-        if img and "tournamentcoin" in img["src"]:
-            entry.tournament_coins = parse_integer(column.text)
-        if img and "tournamentvoucher" in img["src"]:
-            entry.tournament_ticker_voucher = parse_integer(column.text)
-        if img and "trophy" in img["src"]:
-            m = CUP_PATTERN.search(col_str)
-            if m:
-                entry.cup = m.group(1)
-            m = DEED_PATTERN.search(col_str)
+        Returns
+        -------
+        :class:`Auction`
+            The auction contained in the table.
+        """
+        header_container = auction_row.select_one("div.AuctionHeader")
+        char_name_container = header_container.select_one("div.AuctionCharacterName")
+        char_link = char_name_container.select_one("a")
+        if char_link:
+            url = urllib.parse.urlparse(char_link["href"])
+            query = urllib.parse.parse_qs(url.query)
+            auction_id = int(query["auctionid"][0])
+            name = char_link.text
+        else:
+            name = char_name_container.text
+
+        builder = AuctionBuilder().name(name).auction_id(auction_id)
+        char_name_container.replaceWith('')
+        m = char_info_regex.search(header_container.text)
+        if m:
+            builder.level(int(m.group(1)))
+            builder.vocation(try_enum(Vocation, m.group(2).strip()))
+            builder.sex(try_enum(Sex, m.group(3).strip().lower()))
+            builder.world(m.group(4))
+        outfit_img = auction_row.select_one("img.AuctionOutfitImage")
+        m = id_addon_regex.search(outfit_img["src"])
+        if m:
+            builder.outfit(OutfitImage(image_url=outfit_img["src"], outfit_id=int(m.group(1)), addons=int(m.group(2))))
+        item_boxes = auction_row.select("div.CVIcon")
+        for item_box in item_boxes:
+            item = cls._parse_displayed_item(item_box)
+            if item:
+                builder.add_displayed_item(item)
+        dates_containers = auction_row.select_one("div.ShortAuctionData")
+        start_date_tag, end_date_tag, *_ = dates_containers.select("div.ShortAuctionDataValue")
+        builder.auction_start(parse_tibia_datetime(start_date_tag.text.replace('\xa0', ' ')))
+        builder.auction_end(parse_tibia_datetime(end_date_tag.text.replace('\xa0', ' ')))
+        bids_container = auction_row.select_one("div.ShortAuctionDataBidRow")
+        bid_tag = bids_container.select_one("div.ShortAuctionDataValue")
+        bid_type_tag = bids_container.select("div.ShortAuctionDataLabel")[0]
+        bid_type_str = bid_type_tag.text.replace(":", "").strip()
+        builder.bid_type(try_enum(BidType, bid_type_str))
+        builder.bid(parse_integer(bid_tag.text))
+        auction_body_block = auction_row.select_one("div.CurrentBid")
+        auction_info_tag = auction_body_block.select_one("div.AuctionInfo")
+        status = ""
+        if auction_info_tag:
+            convert_line_breaks(auction_info_tag)
+            status = auction_info_tag.text.replace("\n", " ").replace("  ", " ")
+        builder.status(try_enum(AuctionStatus, status, AuctionStatus.IN_PROGRESS))
+        argument_entries = auction_row.select("div.Entry")
+        for entry in argument_entries:
+            img = entry.select_one("img")
+            img_url = img["src"]
+            category_id = 0
+            m = id_regex.search(img_url)
             if m:
-                entry.deed = m.group(1)
-        if img and "reward" in img["src"]:
-            span = column.find('span', attrs={"class": "HelperDivIndicator"})
-            mouse_over = span["onmouseover"]
-            title, popup = parse_popup(mouse_over)
-            label = popup.find('div', attrs={'class': 'ItemOverLabel'})
-            entry.other_rewards = label.text.strip()
-
-    @staticmethod
-    def _parse_rank_range(rank_text):
-        """Parse the rank range text from the reward set table.
+                category_id = parse_integer(m.group(1))
+            builder.add_sales_argument(SalesArgument(content=entry.text, category_image=img_url,
+                                                     category_id=category_id))
+        return builder.build()
+
+    @classmethod
+    def _parse_tables(cls, parsed_content) -> Dict[str, bs4.Tag]:
+        """Parse the character details tables.
 
         Parameters
         ----------
-        rank_text: :class:`str`
-            The string describing the ranks.
+        parsed_content: :class:`bs4.Tag`
+            The parsed content of the auction.
 
         Returns
         -------
-        :class:`tuple` of :class:`int`
-            A tuple containing the highest and lower rank for this reward bracket.
-
-            If the reward is for a single rank, both tuple elements will be the same.
+        :class:`dict`
+            A dictionary of the tables, grouped by their id.
         """
-        m = RANGE_PATTERN.search(rank_text)
-        first = int(m.group(1))
-        last = first
-        if m.group(2):
-            last = int(m.group(2))
-        return first, last
-
-    def _parse_archive_list(self, archive_table):
-        """Parse the archive list table.
+        details_tables = parsed_content.select("div.CharacterDetailsBlock")
+        return {table["id"]: table for table in details_tables}
 
-        This table is only visible when viewing a tournament from the archive.
+    @classmethod
+    def _parse_data_table(cls, table) -> Dict[str, str]:
+        """Parse a simple data table into a key value mapping.
 
         Parameters
         ----------
-        archive_table: :class:`bs4.Tag`
-            The parsed element containing the table.
-        """
-        _, *options = archive_table.find_all("option")
-        self.archived_tournaments = []
-        for option in options:
-            m = ARCHIVE_LIST_PATTERN.match(option.text)
-            if not m:
-                continue
-            title = m.group(1).strip()
-            start_date = parse_tibia_full_date(m.group(2))
-            end_date = parse_tibia_full_date(m.group(3))
-            value = int(option["value"])
-            if title == self.title:
-                self.cycle = value
-            self.archived_tournaments.append(TournamentEntry(title=title, start_date=start_date, end_date=end_date,
-                                                             cycle=value))
-
-
-class TournamentLeaderboard(abc.Serializable):
-    """Represents a tournament's leaderboards.
-
-    .. versionadded:: 2.5.0
-
-    Attributes
-    ----------
-    world: :class:`str`
-        The world this leaderboard belongs to.
-    tournament: :class:`TournamentEntry`
-        The tournament this leaderboard belongs to.
-    entries: :obj:`list` of :class:`TournamentLeaderboardEntry`
-        The leaderboard entries.
-    results_count: :class:`int`
-        The total number of leaderboard entries. These might be in a different page.
-    """
-
-    ENTRIES_PER_PAGE = 100
-
-    __slots__ = (
-        "world",
-        "tournament",
-        "entries",
-        "results_count",
-    )
-
-    _serializable_properties = (
-        "page",
-        "total_pages",
-    )
-
-    def __init__(self, **kwargs):
-        self.world: str = kwargs.get("world")
-        self.tournament: TournamentEntry = kwargs.get("tournament")
-        self.entries: List[TournamentLeaderboardEntry] = kwargs.get("entries", [])
-        self.results_count = kwargs.get("results_count", 0)
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} world={self.world!r} tournament={self.tournament} " \
-               f"results_count={self.results_count}>"
-
-    @property
-    def from_rank(self):
-        """:class:`int`: The starting rank of the provided entries."""
-        return self.entries[0].rank if self.entries else 0
-
-    @property
-    def to_rank(self):
-        """:class:`int`: The last rank of the provided entries."""
-        return self.entries[-1].rank if self.entries else 0
-
-    @property
-    def page(self):
-        """:class:`int`: The page number the shown results correspond to on Tibia.com."""
-        return int(math.floor(self.from_rank / self.ENTRIES_PER_PAGE)) + 1 if self.from_rank else 0
-
-    @property
-    def total_pages(self):
-        """:class:`int`: The total of pages in the leaderboard."""
-        return int(math.ceil(self.results_count / self.ENTRIES_PER_PAGE))
-
-    @property
-    def url(self):
-        """:class:`str`: Get the URL to the current leaderboard and page."""
-        return self.get_url(self.world, self.tournament.cycle, self.page)
-
-    @classmethod
-    def get_url(cls, world, tournament_cycle, page=1):
-        """Get the URL to the leaderboards of a specific world, tournament and page.
-
-        Parameters
-        ----------
-        world: :class:`str`
-            The world to get the leaderboards for.
-        tournament_cycle: :class:`int`
-            The cycle of the tournament to get the leaderboards for.
-        page: :class:`int`
-            The leader board's page to view. By default 1.
+        table: :class:`bs4.Tag`
+            The table to be parsed.
 
         Returns
         -------
-        The URL to the specified leaderboard.
+        :class:`dict`
+            A mapping containing the table's data.
         """
-        return get_tibia_url("community", "tournamentleaderboards", tournamentworld=world,
-                             tournamentcycle=tournament_cycle, selectedleaderboardpage=page)
+        rows = table.select("tr")
+        data = {}
+        for row in rows:
+            name = row.select_one("span").text
+            value = row.select_one("div").text
+            name = name.lower().strip().replace(" ", "_").replace(":", "")
+            data[name] = value
+        return data
 
     @classmethod
-    def from_content(cls, content):
-        """Create an instance of the class from the html content of the tournament's leaderboards page.
+    def _parse_skills_table(cls, builder, table):
+        """Parse the skills table.
 
         Parameters
         ----------
-        content: :class:`str`
-            The HTML content of the page.
+        table: :class:`bs4.Tag`
+            The table containing the character's skill.
+        """
+        rows = table.select("tr")
+        skills = []
+        for row in rows:
+            cols = row.select("td")
+            name_c, level_c, progress_c = [c.text for c in cols]
+            level = int(level_c)
+            progress = float(progress_c.replace("%", ""))
+            skills.append(SkillEntry(name=name_c, level=level, progress=progress))
+        builder.skills(skills)
 
-        Returns
-        -------
-        :class:`TournamentLeaderboard`
-            The tournament contained in the page, or None if the tournament leaderboard doesn't exist.
+    @classmethod
+    def _parse_blessings_table(cls, builder, table):
+        """Parse the blessings table.
 
-        Raises
-        ------
-        InvalidContent
-            If content is not the HTML of a tournament's leaderboard page.
+        Parameters
+        ----------
+        table: :class:`bs4.Tag`
+            The table containing the character's blessings.
         """
-        try:
-            parsed_content = parse_tibiacom_content(content)
-            tables = parsed_content.find_all('div', attrs={'class': 'TableContainer'})
-            if not tables:
-                raise InvalidContent("content does not belong to the Tibia.com's tournament leaderboards section")
-            selector_table = tables[0]
-            leaderboard = cls()
-            result = leaderboard._parse_leaderboard_selectors(selector_table)
-            if not result:
-                return None
-            ranking_table = tables[1]
-            leaderboard._parse_leaderboard_entries(ranking_table)
-            return leaderboard
-        except AttributeError as e:
-            raise InvalidContent("content does not belong to the Tibia.com's tournament leaderboards section", e)
+        table_content = table.select_one("table.TableContent")
+        _, *rows = table_content.select("tr")
+        blessings = []
+        for row in rows:
+            cols = row.select("td")
+            amount_c, name_c = [c.text for c in cols]
+            amount = int(amount_c.replace("x", ""))
+            blessings.append(BlessingEntry(name=name_c, amount=amount))
+        builder.blessings(blessings)
 
-    def _parse_leaderboard_selectors(self, selector_table):
-        """Parse the option selectors from the leaderboards to get their information.
+    @classmethod
+    def _parse_single_column_table(cls, table):
+        """Parse a table with a single column into an array.
 
         Parameters
         ----------
-        selector_table: :class:`bs4.BeautifulSoup`
+        table: :class:`bs4.Tag`
+            A table with a single column.
 
         Returns
         -------
-        :class:`bool`
-            Whether the selectors could be parsed or not.
+        :class:`list` of :class:`str`
+            A list with the contents of each row.
+        """
+        table_content = table.select("table.TableContent")[-1]
+        _, *rows = table_content.select("tr")
+        ret = []
+        for row in rows:
+            col = row.select_one("td")
+            text = col.text
+            if "more entries" in text:
+                continue
+            ret.append(text)
+        return ret
+
+    @classmethod
+    def _parse_charms_table(cls, builder, table):
+        """Parse the charms table and extracts its information.
+
+        Parameters
+        ----------
+        table: :class:`bs4.Tag`
+            The table containing the charms.
+        """
+        table_content = table.select_one("table.TableContent")
+        _, *rows = table_content.select("tr")
+        charms = []
+        for row in rows:
+            cols = row.select("td")
+            if len(cols) != 2:
+                continue
+            cost_c, name_c = [c.text for c in cols]
+            cost = parse_integer(cost_c.replace("x", ""))
+            charms.append(CharmEntry(name=name_c, cost=cost))
+        builder.charms(charms)
+
+    @classmethod
+    def _parse_achievements_table(cls, builder, table):
+        """Parse the achievements table and extracts its information.
+
+        Parameters
+        ----------
+        table: :class:`bs4.Tag`
+            The table containing the achievements.
         """
-        world_select = selector_table.find("select", attrs={"name": "tournamentworld"})
-        selected_world = world_select.find("option", {"selected": "selected"})
-        if not selected_world:
-            return False
-        self.world = selected_world.text
-        tournament_select = selector_table.find("select", attrs={"name": "tournamentcycle"})
-        selected_tournament = tournament_select.find("option", {"selected": "selected"})
-        tournament_text = selected_tournament.text
-        start_date = None
-        end_date = None
-        cycle = int(selected_tournament["value"])
-        if "current tournament" in tournament_text.lower():
-            tournament_title = CURRENT_TOURNAMENT_PATTERN.sub(r"\g<1>", tournament_text)
+        table_content = table.select_one("table.TableContent")
+        _, *rows = table_content.select("tr")
+        achievements = []
+        for row in rows:
+            col = row.select_one("td")
+            text = col.text.strip()
+            if "more entries" in text:
+                continue
+            secret = col.select_one("img") is not None
+            achievements.append(AchievementEntry(name=text, secret=secret))
+        builder.achievements(achievements)
+
+    @classmethod
+    def _parse_bestiary_table(cls, builder, table, bosstiary=False):
+        """Parse the bestiary table and extracts its information.
+
+        Parameters
+        ----------
+        table: :class:`bs4.Tag`
+            The table containing the bestiary information.
+        """
+        table_content = table.select_one("table.TableContent")
+        _, *rows = table_content.select("tr")
+        bestiary = []
+        for row in rows:
+            cols = row.select("td")
+            if len(cols) != 3:
+                continue
+            step_c, kills_c, name_c = [c.text for c in cols]
+            kills = parse_integer(kills_c.replace("x", ""))
+            step = int(step_c)
+            bestiary.append(BestiaryEntry(name=name_c, kills=kills, step=step))
+        if bosstiary:
+            builder.bosstiary_progress(bestiary)
         else:
-            m = ARCHIVE_LIST_PATTERN.search(tournament_text)
-            tournament_title = m.group(1).strip()
-            start_date = parse_tibia_full_date(m.group(2))
-            end_date = parse_tibia_full_date(m.group(3))
-        self.tournament = TournamentEntry(title=tournament_title, start_date=start_date, end_date=end_date,
-                                          cycle=cycle)
-        return True
+            builder.bestiary_progress(bestiary)
 
-    def _parse_leaderboard_entries(self, ranking_table):
-        """Parse the leaderboards' entries.
+
+    @classmethod
+    def _parse_general_table(cls, builder, table):
+        """Parse the general information table and assigns its values.
 
         Parameters
         ----------
-        ranking_table: :class:`bs4.BeautifulSoup`
-            The table containing the rankings.
+        table: :class:`bs4.Tag`
+            The table with general information.
         """
-        ranking_table_content = ranking_table.find("table", attrs={"class": "TableContent"})
-        header, *rows = ranking_table_content.find_all('tr')
+        content_containers = table.select("table.TableContent")
+        general_stats = cls._parse_data_table(content_containers[0])
+        builder.hit_points(parse_integer(general_stats.get("hit_points", "0")))
+        builder.mana(parse_integer(general_stats.get("mana", "0")))
+        builder.capacity(parse_integer(general_stats.get("capacity", "0")))
+        builder.speed(parse_integer(general_stats.get("speed", "0")))
+        builder.mounts_count(parse_integer(general_stats.get("mounts", "0")))
+        builder.outfits_count(parse_integer(general_stats.get("outfits", "0")))
+        builder.titles_count(parse_integer(general_stats.get("titles", "0")))
+        builder.blessings_count(parse_integer(re.sub(r"/d+", "", general_stats.get("blessings", "0"))))
+
+        cls._parse_skills_table(builder, content_containers[1])
+
+        additional_stats = cls._parse_data_table(content_containers[2])
+        builder.creation_date(parse_tibia_datetime(additional_stats.get("creation_date", "").replace("\xa0", " ")))
+        builder.experience(parse_integer(additional_stats.get("experience", "0")))
+        builder.gold(parse_integer(additional_stats.get("gold", "0")))
+        builder.achievement_points(parse_integer(additional_stats.get("achievement_points", "0")))
+
+        transfer_data = cls._parse_data_table(content_containers[3])
+        transfer_text = transfer_data.get("regular_world_transfer")
+        if "after" in transfer_text:
+            date_string = transfer_text.split("after ")[1]
+            builder.regular_world_transfer_available_date(parse_tibia_datetime(date_string))
+
+        charms_data = cls._parse_data_table(content_containers[4])
+        builder.charm_expansion("yes" in charms_data.get("charm_expansion", ""))
+        builder.available_charm_points(parse_integer(charms_data.get("available_charm_points")))
+        builder.spent_charm_points(parse_integer(charms_data.get("spent_charm_points")))
+
+        daily_rewards_data = cls._parse_data_table(content_containers[5])
+        builder.daily_reward_streak(parse_integer(daily_rewards_data.popitem()[1]))
+
+        hunting_data = cls._parse_data_table(content_containers[6])
+        builder.hunting_task_points(parse_integer(hunting_data.get("hunting_task_points", "")))
+        builder.permanent_hunting_task_slots(parse_integer(hunting_data.get("permanent_hunting_task_slots", "")))
+        builder.permanent_prey_slots(parse_integer(hunting_data.get("permanent_prey_slots", "")))
+        builder.prey_wildcards(parse_integer(hunting_data.get("prey_wildcards", "")))
+
+        hirelings_data = cls._parse_data_table(content_containers[7])
+        builder.hirelings(parse_integer(hirelings_data.get("hirelings", "")))
+        builder.hireling_jobs(parse_integer(hirelings_data.get("hireling_jobs", "")))
+        builder.hireling_outfits(parse_integer(hirelings_data.get("hireling_outfits", "")))
+        if len(content_containers) >= 9:
+            dust_data = cls._parse_data_table(content_containers[8])
+            dust_values = dust_data.get("exalted_dust", "0/0").split("/")
+            builder.exalted_dust(parse_integer(dust_values[0]))
+            builder.exalted_dust_limit(parse_integer(dust_values[1]))
+        if len(content_containers) >= 10:
+            boss_data = cls._parse_data_table(content_containers[9])
+            builder.boss_points(parse_integer(boss_data.get("boss_points", "")))
+
+    @classmethod
+    def _parse_items_table(cls, table: bs4.Tag):
+        if pagination_block := table.select_one("div.BlockPageNavigationRow"):
+            page, total_pages, results = parse_pagination(pagination_block)
+        else:
+            return ItemSummary()
+        summary = ItemSummary(current_page=page, total_pages=total_pages, results_count=results)
+        item_boxes = table.select("div.CVIcon")
+        for item_box in item_boxes:
+            if item := cls._parse_displayed_item(item_box):
+                summary.entries.append(item)
+        return summary
+
+    @classmethod
+    def _parse_mounts_table(cls, table):
+        if pagination_block := table.select_one("div.BlockPageNavigationRow"):
+            page, total_pages, results = parse_pagination(pagination_block)
+        else:
+            return Mounts()
+        summary = Mounts(current_page=page, total_pages=total_pages, results_count=results)
+        mount_boxes = table.select("div.CVIcon")
+        for mount_box in mount_boxes:
+            if mount := cls._parse_displayed_mount(mount_box):
+                summary.entries.append(mount)
+        return summary
+
+    @classmethod
+    def _parse_outfits_table(cls, table):
+        if pagination_block := table.select_one("div.BlockPageNavigationRow"):
+            page, total_pages, results = parse_pagination(pagination_block)
+        else:
+            return Outfits()
+        summary = Outfits(current_page=page, total_pages=total_pages, results_count=results)
+        outfit_boxes = table.select("div.CVIcon")
+        for outfit_box in outfit_boxes:
+            if outfit := cls._parse_displayed_outfit(outfit_box):
+                summary.entries.append(outfit)
+        return summary
+
+    @classmethod
+    def _parse_familiars_table(cls, table):
+        if pagination_block := table.select_one("div.BlockPageNavigationRow"):
+            page, total_pages, results = parse_pagination(pagination_block)
+        else:
+            return Familiars()
+        summary = Familiars(current_page=page, total_pages=total_pages, results_count=results)
+        familiar_boxes = table.select("div.CVIcon")
+        for familiar_box in familiar_boxes:
+            if familiar := cls._parse_displayed_familiar(familiar_box):
+                summary.entries.append(familiar)
+        return summary
+
+    @classmethod
+    def _parse_displayed_item(cls, item_box):
+        title_text = item_box["title"]
+        img_tag = item_box.select_one("img")
+        if not img_tag:
+            return None
+        m = amount_regex.match(title_text)
+        amount = 1
+        if m:
+            amount = parse_integer(m.group(1))
+            title_text = amount_regex.sub("", title_text, 1).strip()
+        name, *desc = title_text.split("\n")
+        description = " ".join(desc) if desc else None
+        tier = 0
+        if m := tier_regex.search(name):
+            tier = int(m.group(2))
+            name = m.group(1)
+        item_id = int(m.group(1)) if (m := id_regex.search(img_tag["src"])) else 0
+        return ItemEntry(image_url=img_tag["src"], name=name, count=amount, item_id=item_id, description=description,
+                         tier=tier)
+
+    @classmethod
+    def _parse_displayed_mount(cls, item_box):
+        description = item_box["title"]
+        img_tag = item_box.select_one("img")
+        if not img_tag:
+            return None
+        mount = MountEntry(image_url=img_tag["src"], name=description, mount_id=0)
+        if m := id_regex.search(mount.image_url):
+            mount.mount_id = int(m.group(1))
+        return mount
+
+    @classmethod
+    def _parse_displayed_outfit(cls, item_box):
+        description = item_box["title"]
+        img_tag = item_box.select_one("img")
+        if not img_tag:
+            return None
+        outfit = OutfitEntry(image_url=img_tag["src"], name=description, outfit_id=0, addons=0)
+        name = outfit.name.split("(")[0].strip()
+        outfit.name = name
+        if m := id_addon_regex.search(outfit.image_url):
+            outfit.outfit_id = int(m.group(1))
+            outfit.addons = int(m.group(2))
+        return outfit
+
+    @classmethod
+    def _parse_displayed_familiar(cls, item_box):
+        description = item_box["title"]
+        img_tag = item_box.select_one("img")
+        if not img_tag:
+            return None
+        familiar = FamiliarEntry(image_url=img_tag["src"], name=description, familiar_id=0)
+        name = familiar.name.split("(")[0].strip()
+        familiar.name = name
+        if m := id_regex.search(familiar.image_url):
+            familiar.familiar_id = int(m.group(1))
+        return familiar
+
+    @classmethod
+    def _parse_page_items(cls, content, paginator: AjaxPaginator):
+        parsed_content = parse_tibiacom_content(content, builder='html5lib')
+        item_boxes = parsed_content.select("div.CVIcon")
         entries = []
-        for row in rows:
-            raw_columns = row.find_all("td")
-            if len(raw_columns) != 4:
-                break
-            cols = [c.text.strip() for c in raw_columns]
-            rank_and_change, character, vocation, score = cols
-            m = RANK_PATTERN.search(rank_and_change)
-            rank = int(m.group(1))
-            change = int(m.group(2))
-            voc = try_enum(Vocation, vocation)
-            score = parse_integer(score, 0)
-            entries.append(TournamentLeaderboardEntry(rank=rank, change=change, name=character, vocation=voc, score=score))
-        # Results footer
-        small = ranking_table.find("small")
-        if small:
-            pagination_text = small.text
-            results_str = RESULTS_PATTERN.search(pagination_text)
-            self.results_count = int(results_str.group(1))
-        self.entries = entries
+        for item_box in item_boxes:
+            if isinstance(paginator, ItemSummary):
+                item = cls._parse_displayed_item(item_box)
+            elif isinstance(paginator, Outfits):
+                item = cls._parse_displayed_outfit(item_box)
+            elif isinstance(paginator, Mounts):
+                item = cls._parse_displayed_mount(item_box)
+            elif isinstance(paginator, Familiars):
+                item = cls._parse_displayed_familiar(item_box)
+            else:
+                raise TypeError("unsupported paginator type")
+            if item:
+                entries.append(item)
+        return entries
```

### Comparing `tibia.py-5.6.0/tibiapy/utils.py` & `tibia.py-6.0.0a1/tibiapy/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 """These are functions used thorough the module that may not be intended for public use."""
 import datetime
 import functools
 import itertools
 import re
 import urllib.parse
 import warnings
-from collections import OrderedDict
-from typing import Dict, Optional, Tuple, Type, TypeVar, Union
+from collections import OrderedDict, defaultdict
+from typing import Dict, Optional, Tuple, Type, TypeVar, Union, List
 
 import bs4
+from pydantic import BaseModel
+
+from tibiapy.errors import InvalidContent
 
 TIBIA_CASH_PATTERN = re.compile(r'(\d*\.?\d*)\s?k*$')
 
 
+def clean_text(tag: Union[bs4.Tag, str]):
+    if isinstance(tag, bs4.Tag):
+        text = tag.text
+    else:
+        text = tag
+    return text.replace("\xa0", " ").strip()
+
+
 def convert_line_breaks(element):
     """Convert the <br> tags in a HTML elements to actual line breaks.
 
     Parameters
     ----------
     element: :class:`bs4.Tag`
         A BeautifulSoup object.
     """
     for br in element.find_all("br"):
         br.replace_with("\n")
 
 
+def get_rows(table_tag: bs4.Tag):
+    return table_tag.select("tr")
+
+
 def get_tibia_url(section, subtopic=None, *args, anchor=None, test=False, **kwargs):
     """Build a URL to Tibia.com with the given parameters.
 
     Parameters
     ----------
     section: :class:`str`
         The desired section (e.g. community, abouttibia, manual, library)
@@ -123,14 +138,70 @@
         selected_radio = next((r for r in radios if r.attrs.get("checked") is not None), None)
         if include_options:
             data["__options__"][name] = {str(r.next_sibling).strip(): r.attrs["value"] for r in radios}
         data[name] = selected_radio.attrs["value"] if selected_radio else None
     return data
 
 
+class FormData(BaseModel):
+    values: Dict[str, str] = {}
+    values_multiple: Dict[str, List[str]] = defaultdict(list)
+    available_options: Dict[str, Dict[str, str]] = defaultdict(dict)
+    action: Optional[str] = None
+    method: Optional[str] = None
+
+
+def parse_form_data_new(form: bs4.Tag):
+    """Parse the currently selected values in a form.
+
+    This should correspond to all the data the form would send if submitted.
+
+    Parameters
+    ----------
+    form: :class:`bs4.Tag`
+        A form tag.
+    include_options: :class:`bool`
+        Whether to also include listings of all the possible options.
+        These will be nested inside the __options__ parameter of the resulting dictionary.
+
+    Returns
+    -------
+    :class:`FormData`
+        A dictionary containing all the data.
+    """
+    form_data = FormData()
+    if "action" in form.attrs:
+        form_data.action = form.attrs["action"]
+    if "method" in form.attrs:
+        form_data.method = form.attrs["method"]
+    for field in form.select("input[type=text], input[type=hidden]"):
+        form_data.values[field.attrs.get("name")] = field.attrs.get("value")
+    for select in form.select("select"):
+        name = select.attrs.get("name")
+        selected_option = select.select_one("option[selected]")
+        options = select.select("option")
+        form_data.available_options[name].update({clean_text(opt): opt.attrs.get("value") for opt in options})
+        form_data.values[name] = selected_option.attrs.get("value") if selected_option else None
+    for checkbox in form.select("input[type=checkbox]"):
+        name = checkbox.attrs.get("name")
+        label = checkbox.parent.text
+        value = checkbox.attrs.get("value")
+        form_data.available_options[name][label] = value
+        if checkbox.has_attr("checked"):
+            form_data.values_multiple[name].append(value)
+    for radio in form.select("input[type=radio]"):
+        name = radio.attrs.get("name")
+        value = radio.attrs.get("value")
+        label = radio.next_sibling.text.strip()
+        form_data.available_options[name][label] = value
+        if radio.has_attr("checked"):
+            form_data.values[name] = value
+    return form_data
+
+
 def parse_integer(number: str, default: Optional[int] = 0):
     """Parse a string representing an integer, ignoring commas or periods.
 
     Parameters
     ----------
     number: :class:`str`
         A string representing a number.
@@ -224,15 +295,15 @@
 
     Returns
     -----------
     :class:`datetime.datetime`, optional
         The represented datetime, in UTC (timezone aware).
     """
     try:
-        datetime_str = datetime_str.replace(",", "").replace("&#160;", " ").strip()
+        datetime_str = datetime_str.replace(",", "").replace("&#160;", " ").replace("\xa0", " ").strip()
         # Extracting timezone
         tz = datetime_str[-4:].strip()
 
         # Convert time string to time object
         # Removing timezone cause CEST and CET are not supported
         try:
             t = datetime.datetime.strptime(datetime_str[:-4].strip(), "%b %d %Y %H:%M:%S")
@@ -293,15 +364,15 @@
 
         Since the timestamps contain no timezone information, it can be passed as an additional parameter.
 
         By default CET (+1) is considered.
 
     Returns
     -------
-    :class:`datetime`
+    :class:`datetime.datetime`
         The represented datetime, in UTC (timezone aware).
     """
     t = datetime.datetime.strptime(datetime_str.strip(), "%d.%m.%Y %H:%M:%S")
     # Add/subtract hours to get the real time
     t = t - datetime.timedelta(hours=utc_offset)
     return t.replace(tzinfo=datetime.timezone.utc)
 
@@ -424,15 +495,27 @@
         return obj
     res = parse_tibia_date(obj)
     if res is not None:
         return res
     return parse_tibia_full_date(obj)
 
 
-def parse_tibiacom_content(content, *, html_class="BoxContent", tag="div", builder="lxml"):
+def parse_tables_map(parsed_content: bs4.BeautifulSoup, selector = "div.TableContentContainer") -> Dict[str, bs4.Tag]:
+    tables = parsed_content.select("div.TableContainer")
+    output = {}
+    for table in tables:
+        caption = table.select_one("div.Text")
+        if not caption:
+            raise InvalidContent("table has no caption")
+        if content_table := table.select_one(selector):
+            output[clean_text(caption)] = content_table
+    return output
+
+
+def parse_tibiacom_content(content, *, html_class="BoxContent", tag="div", builder="lxml") -> bs4.BeautifulSoup:
     """Parse HTML content from Tibia.com into a BeautifulSoup object.
 
     Parameters
     ----------
     content: :class:`str`
         The raw HTML content from Tibia.com
     html_class: :class:`str`
@@ -447,14 +530,15 @@
     :class:`bs4.BeautifulSoup`, optional
         The parsed content.
     """
     strainer = bs4.SoupStrainer(tag, class_=html_class) if builder != "html5lib" else None
     return bs4.BeautifulSoup(content.replace('ISO-8859-1', 'utf-8', 1), builder, parse_only=strainer)
 
 
+
 def parse_tibiacom_tables(parsed_content) -> Dict[str, bs4.Tag]:
     """Parse tables from Tibia.com into a mapping by the tables title.
 
     This is used for the table style used in Tibia.com, where a table is wrapped in a container with a title.
 
     Parameters
     ----------
@@ -631,15 +715,15 @@
     page : :class:`int`
         The current page.
     total_pages : :class:`int`
         The total number of pages.
     results_count : :class:`int`
         The total number of results.
     """
-    pages_div, results_div = pagination_block.find_all("div")
+    pages_div, results_div = pagination_block.select("small > div")
     current_page_link = pages_div.find("span", {"class": "CurrentPageLink"})
     page_links = pages_div.find_all("span", {"class": "PageLink"})
     # pages_with_links = pages_div.select(#)
     first_or_last_pages = pages_div.find_all("span", {"class": "FirstOrLastElement"})
     page = -1
     total_pages = -1
     if first_or_last_pages:
```

