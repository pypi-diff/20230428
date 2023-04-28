# Comparing `tmp/LiSE-0.14.2.tar.gz` & `tmp/LiSE-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiSE-0.14.2.tar", last modified: Fri Apr 28 02:12:02 2023, max compression
+gzip compressed data, was "dist/LiSE-0.9.1.tar", last modified: Tue Oct 30 13:40:31 2018, max compression
```

## Comparing `LiSE-0.14.2.tar` & `LiSE-0.9.1.tar`

### file list

```diff
@@ -1,67 +1,40 @@
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-28 02:12:02.859269 LiSE-0.14.2/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    34523 2023-02-01 14:04:01.000000 LiSE-0.14.2/LICENSE
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-28 02:12:02.851269 LiSE-0.14.2/LiSE/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      750 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    16541 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/alchemy.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-28 02:12:02.851269 LiSE-0.14.2/LiSE/allegedb/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    79275 2023-04-27 23:41:08.000000 LiSE-0.14.2/LiSE/allegedb/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    14947 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/allegedb/alchemy.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    46612 2023-04-08 02:47:11.000000 LiSE-0.14.2/LiSE/allegedb/cache.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    31321 2023-03-25 04:26:29.000000 LiSE-0.14.2/LiSE/allegedb/graph.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    25892 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/allegedb/query.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-28 02:12:02.855269 LiSE-0.14.2/LiSE/allegedb/tests/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)        0 2021-07-09 20:18:57.000000 LiSE-0.14.2/LiSE/allegedb/tests/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      318 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/allegedb/tests/conftest.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    12217 2023-04-06 16:58:07.000000 LiSE-0.14.2/LiSE/allegedb/tests/test_all.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3424 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/allegedb/tests/test_branch_plan.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     7498 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/allegedb/tests/test_load.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4594 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/allegedb/tests/test_window.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    20686 2023-04-05 02:07:38.000000 LiSE-0.14.2/LiSE/allegedb/window.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     8504 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/allegedb/wrap.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    26142 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/cache.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    48041 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/character.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    56126 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/engine.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-28 02:12:02.855269 LiSE-0.14.2/LiSE/examples/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      722 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/examples/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     7592 2023-03-29 12:48:53.000000 LiSE-0.14.2/LiSE/examples/college.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     6036 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/examples/kobold.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4294 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/examples/polygons.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5985 2023-04-08 02:47:28.000000 LiSE-0.14.2/LiSE/examples/sickle.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4268 2023-04-05 03:51:56.000000 LiSE-0.14.2/LiSE/examples/wolfsheep.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3493 2023-03-12 00:22:48.000000 LiSE-0.14.2/LiSE/exc.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    44184 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/handle.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    20966 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/node.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     6404 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/portal.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    72217 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/proxy.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    47789 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/query.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    20947 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/rule.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-28 02:12:02.855269 LiSE-0.14.2/LiSE/server/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3139 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/server/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1700 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/server/__main__.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-28 02:12:02.859269 LiSE-0.14.2/LiSE/tests/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      722 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/tests/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1041 2023-04-05 03:52:31.000000 LiSE-0.14.2/LiSE/tests/conftest.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    18167 2023-03-19 01:50:32.000000 LiSE-0.14.2/LiSE/tests/data.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     7709 2023-03-25 11:49:17.000000 LiSE-0.14.2/LiSE/tests/test_character.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3445 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/tests/test_contents.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1806 2023-04-08 01:10:03.000000 LiSE-0.14.2/LiSE/tests/test_examples.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3620 2023-04-05 01:17:14.000000 LiSE-0.14.2/LiSE/tests/test_load.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5127 2023-03-19 17:35:16.000000 LiSE-0.14.2/LiSE/tests/test_next_turn.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3179 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/tests/test_place.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4300 2023-02-12 18:19:27.000000 LiSE-0.14.2/LiSE/tests/test_proxy.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    12808 2023-04-22 15:41:11.000000 LiSE-0.14.2/LiSE/tests/test_query.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      477 2023-04-05 01:17:14.000000 LiSE-0.14.2/LiSE/tests/test_resume.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4641 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/tests/test_rule.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2493 2022-09-07 08:44:17.000000 LiSE-0.14.2/LiSE/tests/test_thing.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    24956 2023-04-27 23:18:08.000000 LiSE-0.14.2/LiSE/util.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    12668 2023-04-16 05:58:38.000000 LiSE-0.14.2/LiSE/xcollections.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-28 02:12:02.851269 LiSE-0.14.2/LiSE.egg-info/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    56484 2023-04-28 02:12:02.000000 LiSE-0.14.2/LiSE.egg-info/PKG-INFO
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1304 2023-04-28 02:12:02.000000 LiSE-0.14.2/LiSE.egg-info/SOURCES.txt
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)        1 2023-04-28 02:12:02.000000 LiSE-0.14.2/LiSE.egg-info/dependency_links.txt
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      191 2023-04-28 02:12:02.000000 LiSE-0.14.2/LiSE.egg-info/requires.txt
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)        5 2023-04-28 02:12:02.000000 LiSE-0.14.2/LiSE.egg-info/top_level.txt
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    56484 2023-04-28 02:12:02.859269 LiSE-0.14.2/PKG-INFO
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    15976 2023-04-27 23:18:08.000000 LiSE-0.14.2/README.md
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1153 2023-04-28 00:21:03.000000 LiSE-0.14.2/pyproject.toml
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)       38 2023-04-28 02:12:02.859269 LiSE-0.14.2/setup.cfg
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:31.000000 LiSE-0.9.1/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1537 2018-10-30 13:39:14.000000 LiSE-0.9.1/setup.py
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:31.000000 LiSE-0.9.1/LiSE/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2822 2018-09-26 14:23:51.000000 LiSE-0.9.1/LiSE/reify.py
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:31.000000 LiSE-0.9.1/LiSE/server/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1442 2018-10-19 11:50:10.000000 LiSE-0.9.1/LiSE/server/__main__.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     3907 2018-10-19 11:50:10.000000 LiSE-0.9.1/LiSE/server/__init__.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    43379 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/handle.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    42552 2018-10-20 12:05:14.000000 LiSE-0.9.1/LiSE/sqlite.json
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    12640 2018-10-30 02:15:27.000000 LiSE-0.9.1/LiSE/xcollections.py
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:31.000000 LiSE-0.9.1/LiSE/examples/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     6923 2018-10-25 12:25:34.000000 LiSE-0.9.1/LiSE/examples/kobold.py
+-rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     7189 2018-10-21 20:09:46.000000 LiSE-0.9.1/LiSE/examples/sickle.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     8741 2018-10-25 12:25:34.000000 LiSE-0.9.1/LiSE/examples/college.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5197 2018-10-19 11:50:10.000000 LiSE-0.9.1/LiSE/examples/timecraft.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     4056 2018-10-25 12:25:34.000000 LiSE-0.9.1/LiSE/examples/polygons.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      784 2018-10-19 11:50:10.000000 LiSE-0.9.1/LiSE/examples/__init__.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      350 2017-06-17 19:48:16.000000 LiSE-0.9.1/LiSE/examples/guitest.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    21923 2018-10-20 12:05:14.000000 LiSE-0.9.1/LiSE/rule.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    68206 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/character.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    27779 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/query.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    22623 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/alchemy.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1725 2018-10-19 11:50:10.000000 LiSE-0.9.1/LiSE/place.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     3712 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/exc.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5426 2018-10-19 11:50:10.000000 LiSE-0.9.1/LiSE/util.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     8697 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/portal.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    20876 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/cache.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     9667 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/thing.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    15490 2018-10-19 12:06:53.000000 LiSE-0.9.1/LiSE/node.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    87201 2018-10-30 02:15:25.000000 LiSE-0.9.1/LiSE/proxy.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      812 2018-10-19 11:50:10.000000 LiSE-0.9.1/LiSE/__init__.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    58197 2018-10-25 12:25:34.000000 LiSE-0.9.1/LiSE/engine.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      287 2018-10-30 13:40:31.000000 LiSE-0.9.1/PKG-INFO
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)       38 2018-10-30 13:40:31.000000 LiSE-0.9.1/setup.cfg
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:31.000000 LiSE-0.9.1/LiSE.egg-info/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)       59 2018-10-30 13:40:30.000000 LiSE-0.9.1/LiSE.egg-info/requires.txt
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)        5 2018-10-30 13:40:30.000000 LiSE-0.9.1/LiSE.egg-info/top_level.txt
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      641 2018-10-30 13:40:31.000000 LiSE-0.9.1/LiSE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      287 2018-10-30 13:40:30.000000 LiSE-0.9.1/LiSE.egg-info/PKG-INFO
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)        1 2018-10-30 13:40:30.000000 LiSE-0.9.1/LiSE.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `LiSE-0.14.2/LiSE/__init__.py` & `LiSE-0.9.1/LiSE/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # This file is part of LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from .engine import Engine
+from .engine import Engine
```

### Comparing `LiSE-0.14.2/LiSE/examples/__init__.py` & `LiSE-0.9.1/LiSE/examples/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is part of LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
```

### Comparing `LiSE-0.14.2/LiSE/examples/college.py` & `LiSE-0.9.1/LiSE/examples/college.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
@@ -22,206 +23,220 @@
 leveling-up. Otherwise it's wasted.
 
 Some students are slow and some are drunkards. These students will
 randomly show up late (brain cells become useless in proportion to
 how late, recovering immediately afterward) or drunk (some brain
 cells made useless per drink, recovering as time passes).
 
-This is implemented inefficiently. I've been using it as a stress test.
+This script will initialize LiSEworld.db and code libraries to run the
+simulation described. To view it, run ELiDE from the same directory
+as you ran this script from.
 
 """
 
 
-def two_way(orig, dest):
-	orig.new_portal(dest.name)
-	dest.new_portal(orig.name)
-
-
 def install(eng):
-	phys = eng.new_character('physical')
-	phys.stat['hour'] = 0
+    phys = eng.new_character('physical')
+    phys.stat['hour'] = 0
 
-	@phys.rule(always=True)  # runs every tick regardless of the situation
-	def time_passes(character):
-		character.stat['hour'] = (character.stat['hour'] + 1) % 24
-
-	# There's a character with all of the students in it, to make it easy to apply rules to all students.
-	student_body = eng.new_character('student_body')
-
-	classroom = phys.new_place('classroom')
-
-	@student_body.unit.rule
-	def go_to_class(node):
-		# There's just one really long class every day.
-		node.travel_to(node.character.place['classroom'])
-
-	@go_to_class.trigger
-	def absent(node):
-		return node.location != node.character.place['classroom']
-
-	@go_to_class.prereq
-	def class_in_session(node):
-		return 8 <= node.engine.character['physical'].stat['hour'] < 15
-
-	@go_to_class.prereq
-	def be_timely(node):
-		# Even lazy students have a 50% chance of going to class every hour.
-		#
-		# We need to access the student character like this because the
-		# ``character`` passed into the function is ``student_body``, where the
-		# rule was assigned.
-		#
-		# Or we could have put the 'lazy' stat onto the node instead of the
-		# character... or kept the student character in a stat of the node...
-		# or assigned this rule to the student directly.
-		for user in node.user.values():
-			if user.name not in ('physical', 'student_body'):
-				return not user.stat['lazy'] or node.engine.coin_flip()
-
-	@student_body.unit.rule
-	def leave_class(node):
-		for user in node.user.values():
-			if user.name != 'student_body':
-				node.travel_to(user.stat['room'])
-				return
-
-	@leave_class.trigger
-	def in_classroom_after_class(node):
-		phys = node.character
-		return node.location == phys.place[
-			'classroom'] and phys.stat['hour'] >= 15
-
-	# Let's make some rules and not assign them to anything yet.
-	@eng.rule
-	def drink(character):
-		braincells = list(character.node.values())
-		character.engine.shuffle(braincells)
-		for i in range(0, character.engine.randrange(1, 20)):
-			braincells.pop()['drunk'] += 12
-
-	@drink.trigger
-	def party_time(character):
-		phys = character.engine.character['physical']
-		return 23 >= phys.stat['hour'] > 15
-
-	@drink.prereq
-	def is_drunkard(character):
-		return character.stat['drunkard']
-
-	@eng.rule
-	def sloth(character):
-		braincells = list(character.node.values())
-		character.engine.shuffle(braincells)
-		for i in range(0, character.engine.randrange(1, 20)):
-			braincells.pop()['slow'] += 1
-
-	@sloth.trigger
-	def out_of_class(character):
-		# You don't want to use the global variable for the classroom
-		# because it won't be around (or at least, won't work) after
-		# the engine restarts.
-		unit = character.unit['physical'].only
-		classroom = unit.character.place['classroom']
-		return unit.location != classroom
-
-	sloth.prereq(class_in_session)
-
-	@eng.rule
-	def learn(node):
-		for user in node.user.values():
-			if 'xp' in user.stat:
-				user.stat['xp'] += 1
-
-	@learn.trigger
-	def in_class(node):
-		classroom = node.engine.character['physical'].place['classroom']
-		if hasattr(node, 'location'):
-			assert node == node.character.unit['physical'].only
-			return node.location == classroom
-		else:
-			return node.character.unit['physical'].only.location == classroom
-
-	learn.prereq(class_in_session)
-
-	@learn.prereq
-	def pay_attention(node):
-		return node['drunk'] == node['slow'] == 0
-
-	@eng.rule
-	def sober_up(node):
-		node['drunk'] -= 1
-
-	@sober_up.trigger
-	def somewhat_drunk(node):
-		return node['drunk'] > 0
-
-	@eng.rule
-	def catch_up(node):
-		node['slow'] -= 1
-
-	@catch_up.trigger
-	def somewhat_late(node):
-		return node['slow'] > 0
-
-	catch_up.prereq(in_class)
-	catch_up.prereq(class_in_session)
-
-	# 3 dorms of 12 students each.
-	# Each dorm has 6 rooms.
-	# Modeling the teachers would be a logical way to extend this.
-	student_body.stat['characters'] = []
-	for n in range(0, 3):
-		dorm = eng.new_character('dorm{}'.format(n))
-		common = phys.new_place(
-			'common{}'.format(n))  # A common room for students to meet in
-		dorm.add_unit(common)
-		two_way(common, classroom)
-		# All rooms in a dorm are connected via its common room
-		for i in range(0, 6):
-			room = phys.new_place('dorm{}room{}'.format(n, i))
-			dorm.add_unit(room)
-			two_way(room, common)
-			student0 = eng.new_character('dorm{}room{}student0'.format(n, i))
-			body0 = room.new_thing('dorm{}room{}student0'.format(n, i))
-			student0.add_unit(body0)
-			assert (student0 in body0.user.values())
-			student_body.add_unit(body0)
-			assert (student_body in body0.user.values())
-			assert (student0 in body0.user.values())
-			student1 = eng.new_character('dorm{}room{}student1'.format(n, i))
-			body1 = room.new_thing('dorm{}room{}student1'.format(n, i))
-			student1.add_unit(body1)
-			student_body.add_unit(body1)
-			student0.stat['room'] = student1.stat['room'] = room
-			assert student0.stat['room'] == student1.stat['room'] == room
-			student0.stat['roommate'] = student1
-			student1.stat['roommate'] = student0
-			for student in (student0, student1):
-				if student not in student_body.stat['characters']:
-					student_body.stat['characters'].append(student)
-				# Students' nodes are their brain cells.
-				# They are useless if drunk or slow, but recover from both conditions a bit every hour.
-				for k in range(0, 100):
-					cell = student.new_node('cell{}'.format(k),
-											drunk=0,
-											slow=0)
-					#  ``new_node`` is just an alias for ``new_place``;
-					#  perhaps more logical when the places don't really
-					#  represent potential locations
-					student.stat['xp'] = 0
-					student.stat['drunkard'] = eng.coin_flip()
-					student.stat['lazy'] = eng.coin_flip()
-				# Apply these previously written rules to each student
-				for rule in (drink, sloth):
-					student.rule(rule)
-				# Apply these previously written rules to each brain cell
-				for rule in (learn, sober_up, catch_up):
-					student.place.rule(rule)
-	eng.snap_keyframe()
+    @phys.rule(always=True)  # runs every tick regardless of the situation
+    def time_passes(character):
+        character.stat['hour'] = (character.stat['hour'] + 1) % 24
+
+
+    # There's a character with all of the students in it, to make it easy to apply rules to all students.
+    student_body = eng.new_character('student_body')
+
+
+    classroom = phys.new_place('classroom')
+
+
+    @student_body.avatar.rule
+    def go_to_class(node):
+        # There's just one really long class every day.
+        node.travel_to(node.character.place['classroom'])
+
+
+    @go_to_class.trigger
+    def absent(node):
+        return node.location != node.character.place['classroom']
+
+
+    @go_to_class.prereq
+    def class_in_session(node):
+        return 8 <= node.engine.character['physical'].stat['hour'] < 15
+
+
+    @go_to_class.prereq
+    def be_timely(node):
+        # Even lazy students have a 50% chance of going to class every hour.
+        #
+        # We need to access the student character like this because the
+        # ``character`` passed into the function is ``student_body``, where the
+        # rule was assigned.
+        #
+        # Or we could have put the 'lazy' stat onto the node instead of the
+        # character... or kept the student character in a stat of the node...
+        # or assigned this rule to the student directly.
+        for user in node.users.values():
+            if user.name not in ('physical', 'student_body'):
+                return not user.stat['lazy'] or node.engine.coinflip()
+
+
+    @student_body.avatar.rule
+    def leave_class(node):
+        for user in node.users.values():
+            if user.name != 'student_body':
+                node.travel_to(user.stat['room'])
+                return
+
+
+    @leave_class.trigger
+    def in_classroom_after_class(node):
+        phys = node.character
+        return node.location == phys.place['classroom'] \
+               and phys.stat['hour'] >= 15
+
+
+    # Let's make some rules and not assign them to anything yet.
+    @eng.rule
+    def drink(character):
+        braincells = list(character.node.values())
+        character.engine.shuffle(braincells)
+        for i in range(0, character.engine.randrange(1, 20)):
+            braincells.pop()['drunk'] += 12
+
+
+    @drink.trigger
+    def party_time(character):
+        phys = character.engine.character['physical']
+        return 23 >= phys.stat['hour'] > 15
+
+
+    @drink.prereq
+    def is_drunkard(character):
+        return character.stat['drunkard']
+
+
+    @eng.rule
+    def sloth(character):
+        braincells = list(character.node.values())
+        character.engine.shuffle(braincells)
+        for i in range(0, character.engine.randrange(1, 20)):
+            braincells.pop()['slow'] += 1
+
+
+    @sloth.trigger
+    def out_of_class(character):
+        # You don't want to use the global variable for the classroom
+        # because it won't be around (or at least, won't work) after
+        # the engine restarts.
+        avatar = character.avatar['physical'].only
+        classroom = avatar.character.place['classroom']
+        return avatar.location != classroom
+
+    sloth.prereq(class_in_session)
+
+
+    @eng.rule
+    def learn(node):
+        for user in node.users.values():
+            if 'xp' in user.stat:
+                user.stat['xp'] += 1
+
+
+    @learn.trigger
+    def in_class(node):
+        classroom = node.engine.character['physical'].place['classroom']
+        if hasattr(node, 'location'):
+            assert node == node.character.avatar['physical'].only
+            return node.location == classroom
+        else:
+            return node.character.avatar['physical'].only.location == classroom
+
+    learn.prereq(class_in_session)
+
+
+    @learn.prereq
+    def pay_attention(node):
+        return node['drunk'] == node['slow'] == 0
+
+
+    @eng.rule
+    def sober_up(node):
+        node['drunk'] -= 1
+
+
+    @sober_up.trigger
+    def somewhat_drunk(node):
+        return node['drunk'] > 0
+
+
+    @eng.rule
+    def catch_up(node):
+        node['slow'] -= 1
+
+
+    @catch_up.trigger
+    def somewhat_late(node):
+        return node['slow'] > 0
+
+    catch_up.prereq(in_class)
+    catch_up.prereq(class_in_session)
+
+    # 3 dorms of 12 students each.
+    # Each dorm has 6 rooms.
+    # Modeling the teachers would be a logical way to extend this.
+    student_body.stat['characters'] = []
+    for n in range(0, 3):
+        dorm = eng.new_character('dorm{}'.format(n))
+        common = phys.new_place('common{}'.format(n))  # A common room for students to meet in
+        dorm.add_avatar(common)
+        common.two_way(classroom)
+        # All rooms in a dorm are connected via its common room
+        for i in range(0, 6):
+            room = phys.new_place('dorm{}room{}'.format(n, i))
+            dorm.add_avatar(room)
+            room.two_way(common)
+            student0 = eng.new_character('dorm{}room{}student0'.format(n, i))
+            body0 = room.new_thing('dorm{}room{}student0'.format(n, i))
+            student0.add_avatar(body0)
+            assert (student0 in body0.users.values())
+            student_body.add_avatar(body0)
+            assert (student_body in body0.users.values())
+            assert (student0 in body0.users.values())
+            student1 = eng.new_character('dorm{}room{}student1'.format(n, i))
+            body1 = room.new_thing('dorm{}room{}student1'.format(n, i))
+            student1.add_avatar(body1)
+            student_body.add_avatar(body1)
+            student0.stat['room'] = student1.stat['room'] = room
+            assert student0.stat['room'] == student1.stat['room'] == room
+            student0.stat['roommate'] = student1
+            student1.stat['roommate'] = student0
+            for student in (student0, student1):
+                if student not in student_body.stat['characters']:
+                    student_body.stat['characters'].append(student)
+                # Students' nodes are their brain cells.
+                # They are useless if drunk or slow, but recover from both conditions a bit every hour.
+                for k in range(0, 100):
+                    cell = student.new_node('cell{}'.format(k), drunk=0, slow=0)
+                    #  ``new_node`` is just an alias for ``new_place``;
+                    #  perhaps more logical when the places don't really
+                    #  represent potential locations
+                    student.stat['xp'] = 0
+                    student.stat['drunkard'] = eng.coinflip()
+                    student.stat['lazy'] = eng.coinflip()
+                # Apply these previously written rules to each student
+                for rule in (drink, sloth):
+                    student.rule(rule)
+                # Apply these previously written rules to each brain cell
+                for rule in (learn, sober_up, catch_up):
+                    student.place.rule(rule)
 
 
 if __name__ == "__main__":
-	import sys
-	from LiSE.engine import Engine
-
-	with Engine(sys.argv[-1]) as eng:
-		install(eng)
+    from LiSE.engine import Engine
+    with Engine(":memory:") as eng:
+        install(eng)
+        for i in range(72):
+            eng.next_turn()
+            print(i)
```

### Comparing `LiSE-0.14.2/LiSE/exc.py` & `LiSE-0.9.1/LiSE/exc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,126 @@
 # This file is part of LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Exception classes for use in LiSE."""
-from .allegedb import HistoricKeyError, OutOfTimelineError
-from .allegedb.query import IntegrityError, TimeError
-from .allegedb.cache import NotInKeyframeError
+from allegedb.query import IntegrityError, TimeError
 
 try:
-	from sqlalchemy.exc import OperationalError as alchemyOpError
-	from sqlite3 import OperationalError as liteOpError
-
-	OperationalError = (alchemyOpError, liteOpError)
+    from sqlalchemy.exc import OperationalError as alchemyOpError
+    from sqlite3 import OperationalError as liteOpError
+    OperationalError = (alchemyOpError, liteOpError)
 except ImportError:
-	from sqlite3 import OperationalError
+    from sqlite3 import OperationalError
 
 
 class NonUniqueError(Exception):
-	"""You tried to look up the only one of something but there wasn't just one"""
+    """For when you tried to look up the only one of something but there wasn't just one"""
 
 
 class AmbiguousAvatarError(NonUniqueError, KeyError):
-	"""An AvatarMapping can't decide what you want."""
+    """An AvatarMapping can't decide what you want."""
 
 
 class AmbiguousUserError(NonUniqueError, AttributeError):
-	"""A user descriptor can't decide what you want."""
+    """A user descriptor can't decide what you want."""
 
 
 class UserFunctionError(SyntaxError):
-	"""Error condition for when I try to load a user-defined function and
-	something goes wrong.
+    """Error condition for when I try to load a user-defined function and
+    something goes wrong.
 
-	"""
-	pass
+    """
+    pass
 
 
 class WorldIntegrityError(ValueError):
-	"""Error condition for when something breaks the world model, even if
-	it might be allowed by the database schema.
+    """Error condition for when something breaks the world model, even if
+    it might be allowed by the database schema.
 
-	"""
+    """
 
 
 class CacheError(ValueError):
-	"""Error condition for something going wrong with a cache"""
-	pass
+    """Error condition for something going wrong with a cache"""
+    pass
 
 
 class TravelException(Exception):
-	"""Exception for problems with pathfinding.
-
-	Not necessarily an error because sometimes somebody SHOULD get
-	confused finding a path.
-
-	"""
-
-	def __init__(self,
-					message,
-					path=None,
-					followed=None,
-					traveller=None,
-					branch=None,
-					turn=None,
-					lastplace=None):
-		"""Store the message as usual, and also the optional arguments:
-
-		``path``: a list of Place names to show such a path as you found
-
-		``followed``: the portion of the path actually followed
-
-		``traveller``: the Thing doing the travelling
-
-		``branch``: branch during travel
-
-		``tick``: tick at time of error (might not be the tick at the
-		time this exception is raised)
-
-		``lastplace``: where the traveller was, when the error happened
+    """Exception for problems with pathfinding. Not necessarily an error
+    because sometimes somebody SHOULD get confused finding a path.
 
-		"""
-		self.path = path
-		self.followed = followed
-		self.traveller = traveller
-		self.branch = branch
-		self.turn = turn
-		self.lastplace = lastplace
-		super().__init__(message)
+    """
+    def __init__(
+            self,
+            message,
+            path=None,
+            followed=None,
+            traveller=None,
+            branch=None,
+            turn=None,
+            lastplace=None
+    ):
+        """Store the message as usual, and also the optional arguments:
+
+        ``path``: a list of Place names to show such a path as you found
+
+        ``followed``: the portion of the path actually followed
+
+        ``traveller``: the Thing doing the travelling
+
+        ``branch``: branch during travel
+
+        ``tick``: tick at time of error (might not be the tick at the
+        time this exception is raised)
+
+        ``lastplace``: where the traveller was, when the error happened
+
+        """
+        self.path = path
+        self.followed = followed
+        self.traveller = traveller
+        self.branch = branch
+        self.turn = turn
+        self.lastplace = lastplace
+        super().__init__(message)
 
 
 class PlanError(AttributeError):
-	"""Tried to use an attribute that shouldn't be used while planning"""
+    """Tried to use an attribute that shouldn't be used while planning"""
 
 
 class RulesEngineError(Exception):
-	"""For problems to do with the rules engine
+    """For problems to do with the rules engine
 
-	Rules themselves should never raise this. Only the engine should.
+    Rules themselves should never raise this. Only the engine should.
 
-	"""
+    """
 
 
 class RuleError(RulesEngineError):
-	"""For problems to do with rules
+    """For problems to do with rules
 
-	Rather than the operation of the rules engine as a whole.
+    Rather than the operation of the rules engine as a whole.
 
-	Don't use this in your trigger, prereq, or action functions.
-	It's only for Rule objects as such.
+    Don't use this in your trigger, prereq, or action functions.
+    It's only for Rule objects as such.
 
-	"""
+    """
 
 
 class RedundantRuleError(RuleError):
-	"""Error condition for when you try to run a rule on a (branch,
-	turn) it's already been executed.
+    """Error condition for when you try to run a rule on a (branch,
+    turn) it's already been executed.
 
-	"""
+    """
```

### Comparing `LiSE-0.14.2/LiSE/server/__main__.py` & `LiSE-0.9.1/LiSE/server/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 # This file is part of LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""A simple local server providing access to a LiSE core
-
-Run this as:
-
-	python3 -m LiSE.server
-
-and it will start an HTTP server at localhost:8080. Send msgpack mappings
-to it, with the key 'command' set to the name of one of the methods in
-:class:`LiSE.handle.EngineHandle` and remaining keys set to arguments
-accepted by that method.
-
-Refer to :class:`LiSE.handle.EngineHandle` for documentation on those
-methods.
-
-"""
 import cherrypy
 from argparse import ArgumentParser
 from . import LiSEHandleWebService
 
 parser = ArgumentParser()
-parser.add_argument('--prefix', action='store', default='.')
+parser.add_argument('world', action='store', required=True)
+parser.add_argument('-c', '--code', action='store')
 args = parser.parse_args()
 conf = {
-	'/': {
-		'request.dispatch': cherrypy.dispatch.MethodDispatcher(),
-		'tools.sessions.on': True,
-		'tools.response_headers.on': True,
-		'tools.response_headers.headers':
-		[('Content-Type', 'application/json')],
-		'tools.encode.on': True,
-		'tools.encode.encoding': 'utf-8'
-	}
+    '/': {
+        'request.dispatch': cherrypy.dispatch.MethodDispatcher(),
+        'tools.sessions.on': True,
+        'tools.response_headers.on': True,
+        'tools.response_headers.headers': [('Content-Type', 'application/json')],
+        'tools.encode.on': True,
+        'tools.encode.encoding': 'utf-8'
+    }
 }
-cherrypy.quickstart(LiSEHandleWebService(args.prefix), '/', conf)
+cherrypy.quickstart(LiSEHandleWebService(args.world, args.code), '/', conf)
```

