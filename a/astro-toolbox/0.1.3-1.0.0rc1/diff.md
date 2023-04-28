# Comparing `tmp/astro-toolbox-0.1.3.tar.gz` & `tmp/astro-toolbox-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-toolbox-0.1.3.tar", last modified: Sun Apr 23 08:38:11 2023, max compression
+gzip compressed data, was "astro-toolbox-1.0.0rc1.tar", last modified: Fri Apr 28 18:08:21 2023, max compression
```

## Comparing `astro-toolbox-0.1.3.tar` & `astro-toolbox-1.0.0rc1.tar`

### file list

```diff
@@ -1,70 +1,75 @@
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.164709 astro-toolbox-0.1.3/
--rw-r--r--   0 romain     (501) staff       (20)    35160 2023-02-26 19:51:45.000000 astro-toolbox-0.1.3/LICENSE
--rw-r--r--   0 romain     (501) staff       (20)     4800 2023-04-23 08:38:11.164547 astro-toolbox-0.1.3/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)     3932 2023-04-22 11:23:31.000000 astro-toolbox-0.1.3/README.md
--rw-r--r--   0 romain     (501) staff       (20)       89 2023-04-18 14:37:30.000000 astro-toolbox-0.1.3/REQUIREMENTS
--rw-r--r--   0 romain     (501) staff       (20)     1874 2023-04-23 08:31:44.000000 astro-toolbox-0.1.3/pyproject.toml
--rw-r--r--   0 romain     (501) staff       (20)       38 2023-04-23 08:38:11.164758 astro-toolbox-0.1.3/setup.cfg
--rw-r--r--   0 romain     (501) staff       (20)       68 2023-01-06 19:50:39.000000 astro-toolbox-0.1.3/setup.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.148191 astro-toolbox-0.1.3/src/
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.150927 astro-toolbox-0.1.3/src/astro_toolbox/
--rw-r--r--   0 romain     (501) staff       (20)      968 2023-04-23 08:36:24.000000 astro-toolbox-0.1.3/src/astro_toolbox/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)       88 2023-02-07 20:30:19.000000 astro-toolbox-0.1.3/src/astro_toolbox/__main__.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.153408 astro-toolbox-0.1.3/src/astro_toolbox/angle/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.3/src/astro_toolbox/angle/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     2170 2023-03-10 13:03:07.000000 astro-toolbox-0.1.3/src/astro_toolbox/angle/degrees.py
--rw-r--r--   0 romain     (501) staff       (20)     1665 2023-03-10 13:01:21.000000 astro-toolbox-0.1.3/src/astro_toolbox/angle/dms.py
--rw-r--r--   0 romain     (501) staff       (20)     1579 2023-03-10 13:04:29.000000 astro-toolbox-0.1.3/src/astro_toolbox/angle/hms.py
--rw-r--r--   0 romain     (501) staff       (20)     2230 2023-03-10 13:06:25.000000 astro-toolbox-0.1.3/src/astro_toolbox/angle/radians.py
--rw-r--r--   0 romain     (501) staff       (20)    14643 2023-04-22 13:09:53.000000 astro-toolbox-0.1.3/src/astro_toolbox/command_line.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.154672 astro-toolbox-0.1.3/src/astro_toolbox/coordinates/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.3/src/astro_toolbox/coordinates/__init__.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.154963 astro-toolbox-0.1.3/src/astro_toolbox/coordinates/data/
--rw-r--r--   0 romain     (501) staff       (20)     2451 2023-02-02 19:46:48.000000 astro-toolbox-0.1.3/src/astro_toolbox/coordinates/data/orbital_elements.json
--rw-r--r--   0 romain     (501) staff       (20)     8253 2023-03-10 13:34:41.000000 astro-toolbox-0.1.3/src/astro_toolbox/coordinates/equatorial.py
--rw-r--r--   0 romain     (501) staff       (20)     3299 2023-03-10 13:34:22.000000 astro-toolbox-0.1.3/src/astro_toolbox/coordinates/horizontal.py
--rw-r--r--   0 romain     (501) staff       (20)     6925 2023-04-22 11:14:48.000000 astro-toolbox-0.1.3/src/astro_toolbox/coordinates/location.py
--rw-r--r--   0 romain     (501) staff       (20)    11831 2023-03-10 13:22:52.000000 astro-toolbox-0.1.3/src/astro_toolbox/coordinates/solar_system.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.155837 astro-toolbox-0.1.3/src/astro_toolbox/query/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-08 12:07:57.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     2415 2023-03-10 13:41:22.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/catalogs.py
--rw-r--r--   0 romain     (501) staff       (20)     3925 2023-04-17 19:20:22.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/ephemeris.py
--rw-r--r--   0 romain     (501) staff       (20)     9976 2023-04-22 11:42:30.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.162073 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/
--rw-r--r--   0 romain     (501) staff       (20)      457 2023-04-17 20:13:59.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/cloudy.png
--rw-r--r--   0 romain     (501) staff       (20)      200 2023-04-17 18:29:15.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/direction_down.png
--rw-r--r--   0 romain     (501) staff       (20)      193 2023-04-17 18:29:15.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/direction_down_left.png
--rw-r--r--   0 romain     (501) staff       (20)      220 2023-04-17 18:29:15.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/direction_down_right.png
--rw-r--r--   0 romain     (501) staff       (20)      256 2023-04-17 18:29:15.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/direction_left.png
--rw-r--r--   0 romain     (501) staff       (20)      215 2023-04-17 18:29:15.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/direction_right.png
--rw-r--r--   0 romain     (501) staff       (20)      270 2023-04-17 18:29:15.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/direction_up.png
--rw-r--r--   0 romain     (501) staff       (20)      243 2023-04-17 18:29:15.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/direction_up_left.png
--rw-r--r--   0 romain     (501) staff       (20)      228 2023-04-17 18:29:15.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/direction_up_right.png
--rw-r--r--   0 romain     (501) staff       (20)      519 2023-04-17 20:23:18.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/drizzle.png
--rw-r--r--   0 romain     (501) staff       (20)      388 2023-04-17 20:22:30.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/fog.png
--rw-r--r--   0 romain     (501) staff       (20)      613 2023-04-18 05:58:24.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/mainly_clear.png
--rw-r--r--   0 romain     (501) staff       (20)      329 2023-04-17 20:17:22.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/na.png
--rw-r--r--   0 romain     (501) staff       (20)      467 2023-04-17 21:07:00.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/partly_cloudy.png
--rw-r--r--   0 romain     (501) staff       (20)      555 2023-04-17 20:23:54.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/rain.png
--rw-r--r--   0 romain     (501) staff       (20)      525 2023-04-17 20:25:57.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/showers.png
--rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 20:24:39.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/snow.png
--rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 15:03:01.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/sunny.png
--rw-r--r--   0 romain     (501) staff       (20)      576 2023-04-17 21:16:48.000000 astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/thunderstorm.png
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.162820 astro-toolbox-0.1.3/src/astro_toolbox/scripts/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-17 20:03:46.000000 astro-toolbox-0.1.3/src/astro_toolbox/scripts/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     1780 2023-02-08 13:53:17.000000 astro-toolbox-0.1.3/src/astro_toolbox/scripts/planning.py
--rw-r--r--   0 romain     (501) staff       (20)    18654 2023-04-22 19:46:43.000000 astro-toolbox-0.1.3/src/astro_toolbox/scripts/plots.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.163562 astro-toolbox-0.1.3/src/astro_toolbox/time/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:53:46.000000 astro-toolbox-0.1.3/src/astro_toolbox/time/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     6330 2023-04-17 16:55:55.000000 astro-toolbox-0.1.3/src/astro_toolbox/time/core.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.164165 astro-toolbox-0.1.3/src/astro_toolbox/utils/
--rw-r--r--   0 romain     (501) staff       (20)      441 2023-04-22 09:17:42.000000 astro-toolbox-0.1.3/src/astro_toolbox/utils/python_functions.py
--rw-r--r--   0 romain     (501) staff       (20)      659 2023-04-17 16:11:48.000000 astro-toolbox-0.1.3/src/astro_toolbox/utils/strparser.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-23 08:38:11.152277 astro-toolbox-0.1.3/src/astro_toolbox.egg-info/
--rw-r--r--   0 romain     (501) staff       (20)     4800 2023-04-23 08:38:11.000000 astro-toolbox-0.1.3/src/astro_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)     2302 2023-04-23 08:38:11.000000 astro-toolbox-0.1.3/src/astro_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-04-23 08:38:11.000000 astro-toolbox-0.1.3/src/astro_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 romain     (501) staff       (20)       62 2023-04-23 08:38:11.000000 astro-toolbox-0.1.3/src/astro_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-01-18 11:00:43.000000 astro-toolbox-0.1.3/src/astro_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 romain     (501) staff       (20)      166 2023-04-23 08:38:11.000000 astro-toolbox-0.1.3/src/astro_toolbox.egg-info/requires.txt
--rw-r--r--   0 romain     (501) staff       (20)       14 2023-04-23 08:38:11.000000 astro-toolbox-0.1.3/src/astro_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.076917 astro-toolbox-1.0.0rc1/
+-rw-r--r--   0 romain     (501) staff       (20)    35160 2023-02-26 19:51:45.000000 astro-toolbox-1.0.0rc1/LICENSE
+-rw-r--r--   0 romain     (501) staff       (20)     4961 2023-04-28 18:08:21.076774 astro-toolbox-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)     4090 2023-04-24 19:09:22.000000 astro-toolbox-1.0.0rc1/README.md
+-rw-r--r--   0 romain     (501) staff       (20)       86 2023-04-24 15:49:22.000000 astro-toolbox-1.0.0rc1/REQUIREMENTS
+-rw-r--r--   0 romain     (501) staff       (20)     1935 2023-04-28 18:03:47.000000 astro-toolbox-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 romain     (501) staff       (20)       38 2023-04-28 18:08:21.076964 astro-toolbox-1.0.0rc1/setup.cfg
+-rw-r--r--   0 romain     (501) staff       (20)       68 2023-01-06 19:50:39.000000 astro-toolbox-1.0.0rc1/setup.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.060096 astro-toolbox-1.0.0rc1/src/
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.062656 astro-toolbox-1.0.0rc1/src/astro_toolbox/
+-rw-r--r--   0 romain     (501) staff       (20)      972 2023-04-28 18:07:07.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)       88 2023-02-07 20:30:19.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/__main__.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.066245 astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     2170 2023-03-10 13:03:07.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/degrees.py
+-rw-r--r--   0 romain     (501) staff       (20)     1665 2023-03-10 13:01:21.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/dms.py
+-rw-r--r--   0 romain     (501) staff       (20)     1579 2023-03-10 13:04:29.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/hms.py
+-rw-r--r--   0 romain     (501) staff       (20)     2230 2023-03-10 13:06:25.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/radians.py
+-rw-r--r--   0 romain     (501) staff       (20)    14488 2023-04-28 18:03:47.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/command_line.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.067379 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/__init__.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.067998 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/data/
+-rw-r--r--   0 romain     (501) staff       (20)     2451 2023-02-02 19:46:48.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/data/orbital_elements.json
+-rw-r--r--   0 romain     (501) staff       (20)      419 2023-04-23 08:44:52.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/data/sites.json
+-rw-r--r--   0 romain     (501) staff       (20)     8253 2023-03-10 13:34:41.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/equatorial.py
+-rw-r--r--   0 romain     (501) staff       (20)     3299 2023-03-10 13:34:22.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/horizontal.py
+-rw-r--r--   0 romain     (501) staff       (20)     6932 2023-04-24 11:37:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/location.py
+-rw-r--r--   0 romain     (501) staff       (20)    11827 2023-04-24 14:30:52.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/solar_system.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.068649 astro-toolbox-1.0.0rc1/src/astro_toolbox/gui/
+-rw-r--r--   0 romain     (501) staff       (20)    16328 2023-04-28 18:03:47.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/gui/gui.py
+-rw-r--r--   0 romain     (501) staff       (20)    73253 2023-04-28 18:03:47.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/gui/logo_astro_toolbox.ico
+-rw-r--r--   0 romain     (501) staff       (20)    20264 2023-04-28 18:03:47.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/gui/main.ui
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.069439 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-08 12:07:57.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     2415 2023-03-10 13:41:22.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/catalogs.py
+-rw-r--r--   0 romain     (501) staff       (20)     3925 2023-04-17 19:20:22.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/ephemeris.py
+-rw-r--r--   0 romain     (501) staff       (20)    10659 2023-04-28 18:03:47.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.074877 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/
+-rw-r--r--   0 romain     (501) staff       (20)      457 2023-04-17 20:13:59.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/cloudy.png
+-rw-r--r--   0 romain     (501) staff       (20)      200 2023-04-17 18:29:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/direction_down.png
+-rw-r--r--   0 romain     (501) staff       (20)      193 2023-04-17 18:29:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/direction_down_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      220 2023-04-17 18:29:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/direction_down_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      256 2023-04-17 18:29:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/direction_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      215 2023-04-17 18:29:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/direction_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      270 2023-04-17 18:29:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/direction_up.png
+-rw-r--r--   0 romain     (501) staff       (20)      243 2023-04-17 18:29:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/direction_up_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      228 2023-04-17 18:29:15.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/direction_up_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      519 2023-04-17 20:23:18.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/drizzle.png
+-rw-r--r--   0 romain     (501) staff       (20)      388 2023-04-17 20:22:30.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/fog.png
+-rw-r--r--   0 romain     (501) staff       (20)      613 2023-04-18 05:58:24.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/mainly_clear.png
+-rw-r--r--   0 romain     (501) staff       (20)      329 2023-04-17 20:17:22.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/na.png
+-rw-r--r--   0 romain     (501) staff       (20)      467 2023-04-17 21:07:00.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/partly_cloudy.png
+-rw-r--r--   0 romain     (501) staff       (20)      555 2023-04-17 20:23:54.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/rain.png
+-rw-r--r--   0 romain     (501) staff       (20)      525 2023-04-17 20:25:57.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/showers.png
+-rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 20:24:39.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/snow.png
+-rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 15:03:01.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/sunny.png
+-rw-r--r--   0 romain     (501) staff       (20)      576 2023-04-17 21:16:48.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/thunderstorm.png
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.075538 astro-toolbox-1.0.0rc1/src/astro_toolbox/scripts/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-17 20:03:46.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/scripts/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     1780 2023-02-08 13:53:17.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/scripts/planning.py
+-rw-r--r--   0 romain     (501) staff       (20)    19032 2023-04-28 18:03:47.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/scripts/plots.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.075830 astro-toolbox-1.0.0rc1/src/astro_toolbox/time/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:53:46.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/time/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     6330 2023-04-17 16:55:55.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/time/core.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.076431 astro-toolbox-1.0.0rc1/src/astro_toolbox/utils/
+-rw-r--r--   0 romain     (501) staff       (20)      441 2023-04-22 09:17:42.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/utils/python_functions.py
+-rw-r--r--   0 romain     (501) staff       (20)      659 2023-04-17 16:11:48.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox/utils/strparser.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-28 18:08:21.065163 astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/
+-rw-r--r--   0 romain     (501) staff       (20)     4961 2023-04-28 18:08:21.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)     2452 2023-04-28 18:08:21.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-04-28 18:08:21.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 romain     (501) staff       (20)       62 2023-04-28 18:08:21.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-04-23 08:43:12.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 romain     (501) staff       (20)      165 2023-04-28 18:08:21.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/requires.txt
+-rw-r--r--   0 romain     (501) staff       (20)       14 2023-04-28 18:08:21.000000 astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/top_level.txt
```

### Comparing `astro-toolbox-0.1.3/LICENSE` & `astro-toolbox-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/PKG-INFO` & `astro-toolbox-1.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-toolbox
-Version: 0.1.3
+Version: 1.0.0rc1
 Summary: Toolbox for observationnal astronomy.
 Author-email: Romain Loustalet Palengat <romain.loustalet@gmx.com>
 Project-URL: Homepage, https://github.com/rloustalet/astro_toolbox
 Project-URL: Source, https://github.com/rloustalet/astro_toolbox
 Project-URL: Documentation, https://astro-toolbox.readthedocs.io/en/latest/
 Keywords: astro,toolbox,astro_toolbox,observationnal
 Platform: unix
@@ -40,14 +40,19 @@
 
 # Options 1
 
 **-v, \--verbose** Program verbosity.
 
 # Commands
 
+# gui
+
+This command launch the Graphical User Interface (GUI) which allow you
+to use the functions available in command lines in a more intuitive interface.
+
 # airmass
 
 This command allows you to plot airmass map of one or multiple objects.
 
 # *argument*
 
 You can enter one or many objects or a path to a file or a directory. If
```

### Comparing `astro-toolbox-0.1.3/README.md` & `astro-toolbox-1.0.0rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
 # Options 1
 
 **-v, \--verbose** Program verbosity.
 
 # Commands
 
+# gui
+
+This command launch the Graphical User Interface (GUI) which allow you
+to use the functions available in command lines in a more intuitive interface.
+
 # airmass
 
 This command allows you to plot airmass map of one or multiple objects.
 
 # *argument*
 
 You can enter one or many objects or a path to a file or a directory. If
```

### Comparing `astro-toolbox-0.1.3/pyproject.toml` & `astro-toolbox-1.0.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     "astro_toolbox",
     "astro_toolbox.angle",
     "astro_toolbox.coordinates",
     "astro_toolbox.query",
     "astro_toolbox.time",
     "astro_toolbox.scripts",
     "astro_toolbox.utils",
+    "astro_toolbox.gui",
 ]
 zip-safe = false
 platforms = [
     "unix",
     "linux",
     "osx",
     "cygwin",
@@ -75,18 +76,22 @@
 include-package-data = false
 
 [tool.setuptools.package-dir]
 "" = "src"
 
 [tool.setuptools.package-data]
 "astro_toolbox.coordinates" = [
-    "data/orbital_elements.json",
+    "data/*.json",
 ]
 "astro_toolbox.query" = [
     "weather_icons/*.png",
 ]
+"astro_toolbox.gui" = [
+    "*.ui",
+    "*.ico",
+]
 
 [tool.setuptools.dynamic.version]
 attr = "astro_toolbox.__init__.__version__"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["REQUIREMENTS"]}
```

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/__init__.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     "Location",
     "Ephemeris",
     "Simbad",
     "Horizons",
     "OpenMeteo",
 ]
 
-__version__ = "0.1.3"
+__version__ = "1.0.0-rc1"
```

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/angle/degrees.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/degrees.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/angle/dms.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/dms.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/angle/hms.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/hms.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/angle/radians.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/angle/radians.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/command_line.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/command_line.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """This module creates the console interface.
 """
+import sys
 import pathlib
 import json
 import logging
 import pkg_resources
 import click
 from matplotlib.backends.backend_pdf import PdfPages
+from matplotlib import pyplot as plt
 from rich.progress import track
 from rich.console import Console
 from rich.table import Table
 
+from PyQt6 import QtWidgets, QtGui
+
 from astro_toolbox.angle.degrees import AngleDeg
 from astro_toolbox.angle.hms import AngleHMS
 from astro_toolbox.time.core import AstroDateTime
 from astro_toolbox.coordinates.location import Location
 from astro_toolbox.coordinates.equatorial import Equatorial
 from astro_toolbox.query.ephemeris import Horizons
 from astro_toolbox.query.catalogs import Simbad
 from astro_toolbox.query.weather import OpenMeteo
 from astro_toolbox.scripts.planning import read_observatory_program
 from astro_toolbox.scripts.planning import get_multiple_informations
 from astro_toolbox.scripts.plots import airmas_map
 from astro_toolbox.scripts.plots import polarstar_plt_northern
 from astro_toolbox.scripts.plots import polarstar_plt_southern
 
+from astro_toolbox.gui.gui import Application
+
 from astro_toolbox.query.ephemeris import DICT_OBJECTS
 
+PATH_GUI = pkg_resources.resource_filename('astro_toolbox', 'gui/')
 PATH = pkg_resources.resource_filename('astro_toolbox', 'coordinates/data/')
 PATH_2 = pkg_resources.resource_filename('astro_toolbox', 'query/weather_icons/')
 
 def wmototext(code):
     """Function to convert WMO code to text.
 
     Parameters
@@ -329,14 +336,15 @@
         Date and time.
     """
     location = Location(location)
     if location.latitude.dmstodeg() > 0:
         polarstar_plt_northern(location, time)
     elif location.latitude.dmstodeg() < 0:
         polarstar_plt_southern(location, time)
+    plt.show()
 
 @cli.command('weather')
 @click.option("-l", "--location",
             type=click.STRING,
             default=None,
             help='-l --location the site name default is None if None last site used')
 @click.option(
@@ -346,15 +354,15 @@
     default=1)
 @click.option(
     "-p",
     "--past",
     count=True,
     default=0)
 def weather_command(location, days, past):
-    """Weather forecasts displayed from Open-Meteo
+    """Weather forecasts displayed from Open-Meteo.
 
     Parameters
     ----------
     location : str
         Saved site name.
     days : int
         Number of days displayed.
@@ -372,32 +380,30 @@
                           f"@ {weather_forecasts.location.name}",
                           show_lines=True)
             table.add_column("Time (UT)", justify="center")
             table.add_column("Temperature (°C)", justify="center")
             table.add_column("Humidity (%)", justify="center")
             table.add_column("Precipitation (mm)", justify="center")
             table.add_column("Wind speed (km/h)", justify="center")
-            table.add_column("Wind Direction", justify="center")
-            table.add_column("Cloud Coverage (%)", justify="center")
+            table.add_column("Wind direction", justify="center")
+            table.add_column("Cloud cover (%)", justify="center")
             table.add_column(justify="center")
-            table.add_row(f'{time[11:]}',
-                        f'{weather_forecasts.get_temperature(time)}',
-                        f'{weather_forecasts.get_humidity(time)}',
-                        f'{weather_forecasts.get_precipitation(time)}',
-                        f'{weather_forecasts.get_wind_speed(time)}',
-                        f'{winddirectiontotext(weather_forecasts.get_wind_direction(time))}',
-                        f'{weather_forecasts.get_cloud(time)}',
-                        wmototext(weather_forecasts.get_wmo(time)))
-        else:
-            table.add_row(f'{time[11:]}',
-                        f'{weather_forecasts.get_temperature(time)}',
-                        f'{weather_forecasts.get_humidity(time)}',
-                        f'{weather_forecasts.get_precipitation(time)}',
-                        f'{weather_forecasts.get_wind_speed(time)}',
-                        f'{winddirectiontotext(weather_forecasts.get_wind_direction(time))}',
-                        f'{weather_forecasts.get_cloud(time)}',
-                        wmototext(weather_forecasts.get_wmo(time)))
+        table.add_row(f'{time[11:]}',
+                    f'{weather_forecasts.get_temperature(time)}',
+                    f'{weather_forecasts.get_humidity(time)}',
+                    f'{weather_forecasts.get_precipitation(time)}',
+                    f'{weather_forecasts.get_wind_speed(time)}',
+                    f'{winddirectiontotext(weather_forecasts.get_wind_direction(time))}',
+                    f'{weather_forecasts.get_cloud_cover(time)}',
+                    wmototext(weather_forecasts.get_wmo(time)))
         last_time = time
     console.print(table)
+@cli.command('gui')
+def gui():
+    """GUI function to launch GUI from cli.
+    """
+    app = QtWidgets.QApplication(sys.argv)
+    app.setWindowIcon(QtGui.QIcon(PATH_GUI + 'logo_astro_toolbox.png'))
+    Application(app)
 
 if __name__ == '__main__':
     cli(False)
```

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/coordinates/data/orbital_elements.json` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/data/orbital_elements.json`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/coordinates/equatorial.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/equatorial.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/coordinates/horizontal.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/horizontal.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/coordinates/location.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         if isinstance(longitude, str) and longitude is not None:
             longitude = angle_parser(longitude)
         if elevation is None:
             elevation = dict_site[name]['elevation']
         self.name = name
         self.latitude = AngleDMS(latitude)
         self.longitude = AngleDMS(longitude)
-        self.elevation = elevation
+        self.elevation = float(elevation)
         self.current_site = {self.name:
                             {
                                 'latitude': repr(self.latitude),
                                 'longitude': repr(self.longitude),
                                 'elevation': self.elevation
                             }
             }
```

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/coordinates/solar_system.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/coordinates/solar_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         Returns
         -------
         tuple
             Tuple containing sun position from earth
         """
         earth_orbital_elements = self._get_orbital_elements('EM Bary')
         true_anomaly, radius = self.compute_true_anomaly_distance(**earth_orbital_elements)
-        lonearth = (true_anomaly*180/math.pi + earth_orbital_elements['perihelion'])
+        lonearth = true_anomaly*180/math.pi + earth_orbital_elements['perihelion']
         x_sun = -radius * math.cos(lonearth*math.pi/180)
         y_sun = -radius * math.sin(lonearth*math.pi/180)
         return x_sun, y_sun
 
     def compute_true_anomaly_distance(self, **orbital_elements):
         """Compute object distance and true anomaly.
 
@@ -147,15 +147,15 @@
 
         Returns
         -------
         tuple
             Tuple which contains object position around the sun.
         """
         true_anomaly, radius = self.compute_true_anomaly_distance(**orbital_elements)
-        true_longitude = (true_anomaly*180/math.pi + orbital_elements['perihelion'])
+        true_longitude = true_anomaly*180/math.pi + orbital_elements['perihelion']
         x_ecliptic = radius * (math.cos(orbital_elements['longnode']*math.pi/180) *
                                     math.cos(true_longitude*math.pi/180) -
                                     math.sin(orbital_elements['longnode']*math.pi/180) *
                                     math.sin(true_longitude*math.pi/180) *
                                     math.cos(orbital_elements['I']*math.pi/180))
         y_ecliptic = radius * (math.sin(orbital_elements['longnode']*math.pi/180) *
                                     math.cos(true_longitude*math.pi/180) +
```

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/query/catalogs.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/query/catalogs.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/query/ephemeris.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/query/ephemeris.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/query/weather.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             representative string
         """
         return (f'Temperature: {self.get_temperature()} °C' +
                 f'Humidity: {self.get_humidity()} %' +
                 f'Precipitation: {self.get_precipitation()} mm' +
                 f'Wind Speed: {self.get_wind_speed()} km/h' +
                 f'Wind Direction: {self.get_wind_direction()} °' +
-                f'Cloud Coverage: {self.get_cloud()} %')
+                f'Cloud Coverage: {self.get_cloud_cover()} %')
 
     def _get_data(self):
         """Open Meteo query method.
 
         Returns
         -------
         dict
@@ -87,15 +87,17 @@
                 f'temperature_{self.pressure_level}hPa,' +
                 f'relativehumidity_{self.pressure_level}hPa,' +
                 'dewpoint_2m,' +
                 'precipitation_probability,' +
                 'precipitation,' +
                 'weathercode,' +
                 'pressure_msl,' +
-                f'cloudcover_{self.pressure_level}hPa,' +
+                'cloudcover_low,' +
+                'cloudcover_mid,' +
+                'cloudcover_high,' +
                 f'windspeed_{self.pressure_level}hPa,' +
                 f'winddirection_{self.pressure_level}hPa')
 
         link += f'&models={self.model}&current_weather=false&past_days=3&forecast_days=16'
         request=urllib.Request(link)
         with urllib.urlopen(request) as response:
             result = json.loads(response.read().decode('utf-8'))
@@ -251,32 +253,44 @@
             Sea level pressure
         """
         index = self._get_index(datetime)
         if math.isnan(index):
             return float('nan')
         return self.data['hourly']['pressure_msl'][index]
 
-    def get_cloud(self, datetime: str | tuple = None):
+    def get_cloud_cover(self, datetime: str | tuple = None):
         """Get cloud coverage method.
 
         Parameters
         ----------
         datetime : str | tuple, optional
             Date and Time as tuple (``YYYY,MM,DD,hh,mm,ss`` or ``YYYY-MM-DDThh:mm:ss``),
             by default None.
 
         Returns
         -------
         float
             Cloud coverage
         """
+
         index = self._get_index(datetime)
         if math.isnan(index):
             return float('nan')
-        return self.data['hourly'][f'cloudcover_{self.pressure_level}hPa'][index]
+        if float(self.location.elevation) < 2000:
+            cloud_cover = (int(self.data['hourly']['cloudcover_low'][index]) +
+                           int(self.data['hourly']['cloudcover_mid'][index]) +
+                           int(self.data['hourly']['cloudcover_high'][index]))
+        elif 2000 < float(self.location.elevation) < 6000:
+            cloud_cover = (int(self.data['hourly']['cloudcover_mid'][index]) +
+                           int(self.data['hourly']['cloudcover_high'][index]))
+        else:
+            cloud_cover = int(self.data['hourly']['cloudcover_high'][index])
+        if cloud_cover == min(cloud_cover, 100):
+            cloud_cover = 100
+        return cloud_cover
 
     def get_wind_speed(self, datetime: str | tuple = None):
         """Get wind speed method.
 
         Parameters
         ----------
         datetime : str | tuple, optional
```

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/drizzle.png` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/drizzle.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/mainly_clear.png` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/mainly_clear.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/rain.png` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/rain.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/showers.png` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/showers.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/query/weather_icons/thunderstorm.png` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/query/weather_icons/thunderstorm.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/scripts/planning.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/scripts/planning.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/scripts/plots.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/scripts/plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """This module contains scripts functions
 """
 import math
 import numpy as np
 import pkg_resources
 
 from matplotlib import pyplot as plt
+from matplotlib import rcParams
 from matplotlib.offsetbox import OffsetImage, AnnotationBbox, TextArea
 
 from astro_toolbox.angle.hms import AngleHMS
 from astro_toolbox.angle.dms import AngleDMS
 from astro_toolbox.time.core import AstroDateTime
 from astro_toolbox.coordinates.location import Location
 from astro_toolbox.coordinates.equatorial import Equatorial
 from astro_toolbox.query.ephemeris import Horizons
 from astro_toolbox.query.weather import OpenMeteo
 
+rcParams['toolbar'] = 'None'
 
 PATH = pkg_resources.resource_filename('astro_toolbox', 'query/weather_icons/')
 
 def offset_image(name, axis):
     """Add icons from query/weather_icons on plot.
 
     Parameters
@@ -50,14 +52,15 @@
         Axis object.
 
     Returns
     -------
     Object
         offset_image Object.
     """
+    code = str(code)
     if code == '00':
         icon = offset_image('sunny', axis)
     elif code == '01':
         icon = offset_image('mainly_clear', axis)
     elif code == '02':
         icon = offset_image('partly_cloudy', axis)
     elif code == '03':
@@ -89,14 +92,15 @@
         Axis object.
 
     Returns
     -------
     Object
         offset_image Object.
     """
+    wind_direction = float(wind_direction)
     if 0 <= wind_direction <= 22.5 or 337.5 <= wind_direction <= 360:
         icon = offset_image('direction_up', axis)
     elif 22.5 < wind_direction < 67.5:
         icon = offset_image('direction_up_left', axis)
     elif 67.5 < wind_direction < 112.5:
         icon = offset_image('direction_left', axis)
     elif 112.5 < wind_direction < 157.5:
@@ -105,14 +109,16 @@
         icon = offset_image('direction_down', axis)
     elif 202.5 < wind_direction < 247.5:
         icon = offset_image('direction_down_right', axis)
     elif 247.5 < wind_direction < 292.5:
         icon = offset_image('direction_right', axis)
     elif 292.5 < wind_direction < 337.5:
         icon = offset_image('direction_up_right', axis)
+    else:
+        icon = offset_image('na', axis)
     return icon
 
 def plot_weather(date, location, bounds, axis):
     """Plot weather on airmass map
 
     Parameters
     ----------
@@ -124,32 +130,32 @@
         Tuple containing observation bounds.
     axis : Object
         Pyplot axis object.
     """
     hours = list(np.mod(np.arange(bounds[0],bounds[1]), 24))
     weather_forecast = OpenMeteo(location=location)
     annotation_box = AnnotationBbox(TextArea('Weather\nforecasts',
-                                            textprops=dict(rotation = 90, ha = 'center')),
+                                            textprops={'rotation': 90, 'ha': 'center'}),
                                             (0, 0),
                                             xybox=(-80, -55),
                                             frameon=False,
                                             xycoords='data',
                                             boxcoords="offset points",
                                             pad=0)
     axis.add_artist(annotation_box)
     weather_units = [TextArea('Temperature °C',
-                            textprops=dict(size=6)),
+                            textprops={'size': 6}),
                     TextArea('Humidity %',
-                            textprops=dict(size=6)),
+                            textprops={'size': 6}),
                     TextArea('Precipitation mm',
-                            textprops=dict(size=6)),
+                            textprops={'size': 6}),
                     TextArea('Wind Speed km/h',
-                            textprops=dict(size=6)),
+                            textprops={'size': 6}),
                     TextArea('Wind Direction',
-                            textprops=dict(size=6))]
+                            textprops={'size': 6})]
     for j, item in enumerate(weather_units):
         annotation_box = AnnotationBbox(item,
                                         (0, 0),
                                         xybox=(-40, -35 - 10 * j),
                                         frameon=False,
                                         xycoords='data',
                                         boxcoords="offset points",
@@ -159,21 +165,21 @@
     for time in hours:
         if time - last_time < 0:
             date = AstroDateTime(date).get_gregorian(1)
         last_time = time
         datetime = date + (time, 0, 0)
         weather = [offset_image('na', axis)]
         weather += [TextArea(f'{weather_forecast.get_temperature(datetime)}',
-                            textprops=dict(size=6)),
+                            textprops={'size': 6}),
                     TextArea(f'{weather_forecast.get_humidity(datetime)}',
-                            textprops=dict(size=6)),
+                            textprops={'size': 6}),
                     TextArea(f'{weather_forecast.get_precipitation(datetime)}',
-                            textprops=dict(size=6)),
+                            textprops={'size': 6}),
                     TextArea(f'{weather_forecast.get_wind_speed(datetime)}',
-                            textprops=dict(size=6))]
+                            textprops={'size': 6})]
         weather.append(winddirectiontoimage(
                         weather_forecast.get_wind_direction(datetime), axis))
         weather[0] = wmotoimage(weather_forecast.get_wmo(datetime), axis)
         for j, item in enumerate(weather):
             annotation_box = AnnotationBbox(item,
                                             (hours.index(time) * 10, 0),
                                             xybox=(0., -25 - 10 * j),
@@ -302,15 +308,15 @@
         for i, time in enumerate(np.arange(bounds[0],bounds[1],0.1)):
             time = (int(time),(time-int(time))*60,0)
             ut_time = AstroDateTime(ut_time.date+time)
             airmasses[j][i] = object_dict[key].calculate_airmass(
                                 ut_time.get_lst(site), site)
             if airmasses[j][i] >= 40:
                 alpha_visible[len(object_dict)-j-1][i] = 0
-    fig, axis = plt.subplots(figsize=(8.27, 11.69))
+    fig, axis = plt.subplots(figsize=(8.27, 11.69), num='Airmass', dpi=72)
     moon_times(len(object_dict), site, date, bounds)
     mesh = axis.pcolormesh(airmasses[::-1],
                     cmap='jet',
                     shading='flat',
                     alpha=alpha_visible,
                     vmin = 1,
                     vmax = 3.5)
@@ -323,31 +329,31 @@
                 [item[1].name + ' v='
                 + str(item[1].magnitude)
                 for item in reversed(object_dict.items())])
     plot_weather(ut_time.date, site, bounds, axis)
     axis.add_artist(AnnotationBbox(OffsetImage(np.full((10,80), np.arange(80)),
                                             cmap='Blues',
                                             dpi_cor=False),
-                                    (551, 780),
-                                    xybox=(-10, -10),
+                                    (-10, -10),
+                                    xybox=(551, 780),
                                     frameon=False,
                                     xycoords='figure points',
                                     boxcoords='offset points',
                                     pad=0))
     axis.add_artist(AnnotationBbox(TextArea('Daylight impact'),
                                     (551, 765),
                                     xybox=(-10, -10),
                                     frameon=False,
                                     xycoords='figure points',
                                     boxcoords='offset points',
                                     pad=0))
-    axis.add_artist(AnnotationBbox(TextArea('Fully transparent is\n' +
+    axis.add_artist(AnnotationBbox(TextArea('Fully transparent represent\n' +
                                             'astronomical night\n' +
                                             r'$h_{sun} < 18°$',
-                                            textprops=dict(size=6)),
+                                            textprops={'size': 6, 'multialignment': 'center'}),
                                     (551, 745),
                                     xybox=(-10, -10),
                                     frameon=False,
                                     xycoords='figure points',
                                     boxcoords='offset points',
                                     pad=0))
     axis.tick_params(left = False)
@@ -395,15 +401,15 @@
     axis.axis('off')
     axis.set_xlim([-60, 60])
     axis.set_ylim([-60, 60])
     axis.text(20, 60, f"HA = {polar_star_hour_angle}", color='r')
     axis.text(20, 55, f"d (') = {round(polar_star_distance, 2)}", color='r')
     fig.tight_layout()
     fig.patch.set_facecolor('k')
-    plt.show()
+    return fig
 
 def polarstar_plt_southern(location: Location, datetime: tuple=None):
     """Polaris Polar Finder position for southern hemisphere
 
     Parameters
     ----------
     site : Location
@@ -454,10 +460,12 @@
     axis.plot(x_octans_stars, y_octans_stars, 'r', marker='o')
     axis.plot(x_octans_stars[2], y_octans_stars[2], 'ow')
     axis.text(x_octans_stars[0]-10, y_octans_stars[0]-10, '\u03C4', color='r')
     axis.set_aspect('equal', adjustable='box')
     axis.axis('off')
     axis.set_xlim([-160, 160])
     axis.set_ylim([-160, 160])
+    axis.text(40, 120, f"HA = {octans_constellation[2][2]}", color='r')
+    axis.text(40, 110, f"d (') = {round(octans_constellation[1][2], 2)}", color='r')
     fig.tight_layout()
     fig.patch.set_facecolor('k')
-    plt.show()
+    return fig
```

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/time/core.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/time/core.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox/utils/strparser.py` & `astro-toolbox-1.0.0rc1/src/astro_toolbox/utils/strparser.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox.egg-info/PKG-INFO` & `astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-toolbox
-Version: 0.1.3
+Version: 1.0.0rc1
 Summary: Toolbox for observationnal astronomy.
 Author-email: Romain Loustalet Palengat <romain.loustalet@gmx.com>
 Project-URL: Homepage, https://github.com/rloustalet/astro_toolbox
 Project-URL: Source, https://github.com/rloustalet/astro_toolbox
 Project-URL: Documentation, https://astro-toolbox.readthedocs.io/en/latest/
 Keywords: astro,toolbox,astro_toolbox,observationnal
 Platform: unix
@@ -40,14 +40,19 @@
 
 # Options 1
 
 **-v, \--verbose** Program verbosity.
 
 # Commands
 
+# gui
+
+This command launch the Graphical User Interface (GUI) which allow you
+to use the functions available in command lines in a more intuitive interface.
+
 # airmass
 
 This command allows you to plot airmass map of one or multiple objects.
 
 # *argument*
 
 You can enter one or many objects or a path to a file or a directory. If
```

### Comparing `astro-toolbox-0.1.3/src/astro_toolbox.egg-info/SOURCES.txt` & `astro-toolbox-1.0.0rc1/src/astro_toolbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 src/astro_toolbox/angle/radians.py
 src/astro_toolbox/coordinates/__init__.py
 src/astro_toolbox/coordinates/equatorial.py
 src/astro_toolbox/coordinates/horizontal.py
 src/astro_toolbox/coordinates/location.py
 src/astro_toolbox/coordinates/solar_system.py
 src/astro_toolbox/coordinates/data/orbital_elements.json
+src/astro_toolbox/coordinates/data/sites.json
+src/astro_toolbox/gui/gui.py
+src/astro_toolbox/gui/logo_astro_toolbox.ico
+src/astro_toolbox/gui/main.ui
 src/astro_toolbox/query/__init__.py
 src/astro_toolbox/query/catalogs.py
 src/astro_toolbox/query/ephemeris.py
 src/astro_toolbox/query/weather.py
 src/astro_toolbox/query/weather_icons/cloudy.png
 src/astro_toolbox/query/weather_icons/direction_down.png
 src/astro_toolbox/query/weather_icons/direction_down_left.png
```

