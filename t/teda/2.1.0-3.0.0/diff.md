# Comparing `tmp/teda-2.1.0.tar.gz` & `tmp/teda-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/teda-2.1.0.tar", last modified: Thu Nov 12 13:39:29 2020, max compression
+gzip compressed data, was "teda-3.0.0.tar", max compression
```

## Comparing `teda-2.1.0.tar` & `teda-3.0.0.tar`

### file list

```diff
@@ -1,85 +1,74 @@
-drwxr-xr-x   0 mka        (501) staff       (20)        0 2020-11-12 13:39:29.000000 teda-2.1.0/
--rw-r--r--   0 mka        (501) staff       (20)     6114 2020-11-12 13:39:29.000000 teda-2.1.0/PKG-INFO
--rw-r--r--   0 mka        (501) staff       (20)     4719 2020-11-10 13:23:11.000000 teda-2.1.0/README.md
--rw-r--r--   0 mka        (501) staff       (20)       38 2020-11-12 13:39:29.000000 teda-2.1.0/setup.cfg
--rw-r--r--   0 mka        (501) staff       (20)      983 2020-07-01 12:39:55.000000 teda-2.1.0/setup.py
-drwxr-xr-x   0 mka        (501) staff       (20)        0 2020-11-12 13:39:29.000000 teda-2.1.0/teda/
--rw-r--r--   0 mka        (501) staff       (20)       32 2020-06-04 16:24:35.000000 teda-2.1.0/teda/__init__.py
--rw-r--r--   0 mka        (501) staff       (20)     2117 2020-06-06 15:30:17.000000 teda-2.1.0/teda/command_line.py
--rw-r--r--   0 mka        (501) staff       (20)     1958 2020-07-01 12:39:55.000000 teda-2.1.0/teda/console.py
--rw-r--r--   0 mka        (501) staff       (20)     2105 2020-04-22 14:55:56.000000 teda-2.1.0/teda/fitsopen.py
--rw-r--r--   0 mka        (501) staff       (20)     2043 2020-05-20 13:57:09.000000 teda-2.1.0/teda/fitting.py
-drwxr-xr-x   0 mka        (501) staff       (20)        0 2020-11-12 13:39:29.000000 teda-2.1.0/teda/icons/
--rw-r--r--   0 mka        (501) staff       (20)     2716 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/1-2-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)     2238 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/1-4-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      298 2020-06-10 13:51:52.000000 teda-2.1.0/teda/icons/add_circle_outline-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      380 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/autopause-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      222 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/autopause_disabled-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      262 2020-06-10 13:51:52.000000 teda-2.1.0/teda/icons/circle-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      249 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/count1-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      315 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/count2-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      343 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/count3-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      270 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/count4-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      296 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/count5-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      349 2020-06-10 13:51:52.000000 teda-2.1.0/teda/icons/delete_forever-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      518 2020-05-14 14:33:36.000000 teda-2.1.0/teda/icons/file-earmark-plus.svg
--rw-r--r--   0 mka        (501) staff       (20)      402 2020-07-01 12:47:01.000000 teda-2.1.0/teda/icons/filter_alt-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      257 2020-07-01 12:47:01.000000 teda-2.1.0/teda/icons/folder-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      217 2020-06-08 17:33:08.000000 teda-2.1.0/teda/icons/home-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      343 2020-06-08 17:32:29.000000 teda-2.1.0/teda/icons/house-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      196 2020-06-08 17:30:35.000000 teda-2.1.0/teda/icons/keyboard_arrow_left-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      194 2020-06-08 17:30:21.000000 teda-2.1.0/teda/icons/keyboard_arrow_right-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      977 2020-06-05 15:03:11.000000 teda-2.1.0/teda/icons/new.png
--rw-r--r--   0 mka        (501) staff       (20)      367 2020-06-10 13:51:52.000000 teda-2.1.0/teda/icons/not_started-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      261 2020-06-08 17:13:41.000000 teda-2.1.0/teda/icons/note_add-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      245 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/panning-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      292 2020-06-08 17:34:43.000000 teda-2.1.0/teda/icons/pause_circle_outline-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      344 2020-07-01 12:47:01.000000 teda-2.1.0/teda/icons/photo_filter-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      285 2020-06-08 17:34:37.000000 teda-2.1.0/teda/icons/play_circle_outline-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      379 2020-07-01 12:39:55.000000 teda-2.1.0/teda/icons/push_pin-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      304 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/save-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      203 2020-06-08 17:29:29.000000 teda-2.1.0/teda/icons/skip_next-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      206 2020-06-08 17:29:33.000000 teda-2.1.0/teda/icons/skip_previous-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      385 2020-06-08 17:34:40.000000 teda-2.1.0/teda/icons/stop_circle-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)     2638 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/x2-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)     2159 2020-07-01 13:22:36.000000 teda-2.1.0/teda/icons/x4-24px.svg
--rw-r--r--   0 mka        (501) staff       (20)      571 2020-06-08 17:51:20.000000 teda-2.1.0/teda/icons.py
-drwxr-xr-x   0 mka        (501) staff       (20)        0 2020-11-12 13:39:29.000000 teda-2.1.0/teda/models/
--rw-r--r--   0 mka        (501) staff       (20)        0 2020-06-04 14:08:12.000000 teda-2.1.0/teda/models/__init__.py
--rw-r--r--   0 mka        (501) staff       (20)     1014 2020-06-04 10:29:56.000000 teda-2.1.0/teda/models/cmaps.py
--rw-r--r--   0 mka        (501) staff       (20)     2896 2020-09-11 15:09:21.000000 teda-2.1.0/teda/models/coordinates.py
--rw-r--r--   0 mka        (501) staff       (20)     5435 2020-11-10 13:24:04.000000 teda-2.1.0/teda/models/scalesModel.py
--rw-r--r--   0 mka        (501) staff       (20)    16147 2020-11-12 13:22:12.000000 teda-2.1.0/teda/painterComponent.py
-drwxr-xr-x   0 mka        (501) staff       (20)        0 2020-11-12 13:39:29.000000 teda-2.1.0/teda/painterShapes/
--rw-r--r--   0 mka        (501) staff       (20)     2967 2020-05-26 15:12:18.000000 teda-2.1.0/teda/painterShapes/CircleCenterShape.py
--rw-r--r--   0 mka        (501) staff       (20)        0 2020-06-04 11:27:56.000000 teda-2.1.0/teda/painterShapes/__init__.py
--rw-r--r--   0 mka        (501) staff       (20)     1885 2020-05-26 15:12:18.000000 teda-2.1.0/teda/painterShapes/circleShape.py
--rw-r--r--   0 mka        (501) staff       (20)     2227 2020-05-26 15:12:18.000000 teda-2.1.0/teda/painterShapes/rectangleMinatureShape.py
--rwxr-xr-x   0 mka        (501) staff       (20)     1411 2020-07-01 12:04:23.000000 teda-2.1.0/teda/teda_fits.py
--rw-r--r--   0 mka        (501) staff       (20)      123 2020-11-12 13:22:12.000000 teda-2.1.0/teda/version.py
--rw-r--r--   0 mka        (501) staff       (20)    32277 2020-11-12 13:22:12.000000 teda-2.1.0/teda/viewer_mainwindow.py
-drwxr-xr-x   0 mka        (501) staff       (20)        0 2020-11-12 13:39:29.000000 teda-2.1.0/teda/views/
--rw-r--r--   0 mka        (501) staff       (20)        0 2020-06-04 14:07:28.000000 teda-2.1.0/teda/views/__init__.py
--rw-r--r--   0 mka        (501) staff       (20)    17603 2020-11-10 13:24:04.000000 teda-2.1.0/teda/views/fitsplot.py
--rw-r--r--   0 mka        (501) staff       (20)     2454 2020-09-11 15:09:21.000000 teda-2.1.0/teda/views/fitsplot_fitsfile.py
--rw-r--r--   0 mka        (501) staff       (20)     2498 2020-11-10 13:24:04.000000 teda-2.1.0/teda/views/fitsplotcontrolled.py
--rw-r--r--   0 mka        (501) staff       (20)     1143 2020-06-04 11:45:26.000000 teda-2.1.0/teda/views/fitsplotzoomed.py
-drwxr-xr-x   0 mka        (501) staff       (20)        0 2020-11-12 13:39:29.000000 teda-2.1.0/teda/widgets/
--rw-r--r--   0 mka        (501) staff       (20)        0 2020-06-04 14:10:29.000000 teda-2.1.0/teda/widgets/__init__.py
--rw-r--r--   0 mka        (501) staff       (20)     6441 2020-07-01 12:47:01.000000 teda-2.1.0/teda/widgets/fileSystemWidget.py
--rw-r--r--   0 mka        (501) staff       (20)     2976 2020-06-04 14:13:24.000000 teda-2.1.0/teda/widgets/fullViewWidget.py
--rw-r--r--   0 mka        (501) staff       (20)     3270 2020-07-01 12:04:23.000000 teda-2.1.0/teda/widgets/headerTableWidget.py
--rw-r--r--   0 mka        (501) staff       (20)     2295 2020-06-04 11:45:26.000000 teda-2.1.0/teda/widgets/info.py
--rw-r--r--   0 mka        (501) staff       (20)     3293 2020-06-05 13:53:25.000000 teda-2.1.0/teda/widgets/radialprofile.py
--rw-r--r--   0 mka        (501) staff       (20)     5299 2020-06-10 16:08:34.000000 teda-2.1.0/teda/widgets/radialprofileIRAF.py
--rw-r--r--   0 mka        (501) staff       (20)    24112 2020-11-10 13:24:04.000000 teda-2.1.0/teda/widgets/scaleWidget.py
--rw-r--r--   0 mka        (501) staff       (20)    12509 2020-07-01 13:22:36.000000 teda-2.1.0/teda/widgets/scanToolbar.py
--rw-r--r--   0 mka        (501) staff       (20)     6207 2020-11-10 13:24:04.000000 teda-2.1.0/teda/widgets/slider.py
--rw-r--r--   0 mka        (501) staff       (20)     1357 2020-06-04 14:10:39.000000 teda-2.1.0/teda/widgets/zoomViewWidget.py
-drwxr-xr-x   0 mka        (501) staff       (20)        0 2020-11-12 13:39:29.000000 teda-2.1.0/teda.egg-info/
--rw-r--r--   0 mka        (501) staff       (20)     6114 2020-11-12 13:39:29.000000 teda-2.1.0/teda.egg-info/PKG-INFO
--rw-r--r--   0 mka        (501) staff       (20)     2075 2020-11-12 13:39:29.000000 teda-2.1.0/teda.egg-info/SOURCES.txt
--rw-r--r--   0 mka        (501) staff       (20)        1 2020-11-12 13:39:29.000000 teda-2.1.0/teda.egg-info/dependency_links.txt
--rw-r--r--   0 mka        (501) staff       (20)       49 2020-11-12 13:39:29.000000 teda-2.1.0/teda.egg-info/entry_points.txt
--rw-r--r--   0 mka        (501) staff       (20)       43 2020-11-12 13:39:29.000000 teda-2.1.0/teda.egg-info/requires.txt
--rw-r--r--   0 mka        (501) staff       (20)        5 2020-11-12 13:39:29.000000 teda-2.1.0/teda.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1066 2020-06-04 16:42:55.000000 teda-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4719 2020-12-02 21:00:51.000070 teda-3.0.0/README.md
+-rw-r--r--   0        0        0      454 2023-04-28 02:35:30.794102 teda-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2020-06-04 16:24:35.000000 teda-3.0.0/teda/__init__.py
+-rw-r--r--   0        0        0     2117 2023-04-28 02:39:09.920354 teda-3.0.0/teda/command_line.py
+-rw-r--r--   0        0        0     1958 2020-07-01 12:39:55.000000 teda-3.0.0/teda/console.py
+-rw-r--r--   0        0        0     1531 2020-12-03 12:27:12.916427 teda-3.0.0/teda/draggingComponent.py
+-rw-r--r--   0        0        0     2105 2020-04-22 14:55:56.000000 teda-3.0.0/teda/fitsopen.py
+-rw-r--r--   0        0        0     2043 2020-05-20 13:57:09.000000 teda-3.0.0/teda/fitting.py
+-rw-r--r--   0        0        0     2716 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/1-2-24px.svg
+-rw-r--r--   0        0        0     2238 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/1-4-24px.svg
+-rw-r--r--   0        0        0      298 2020-06-10 13:51:52.000000 teda-3.0.0/teda/icons/add_circle_outline-24px.svg
+-rw-r--r--   0        0        0      380 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/autopause-24px.svg
+-rw-r--r--   0        0        0      222 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/autopause_disabled-24px.svg
+-rw-r--r--   0        0        0      262 2020-06-10 13:51:52.000000 teda-3.0.0/teda/icons/circle-24px.svg
+-rw-r--r--   0        0        0      249 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count1-24px.svg
+-rw-r--r--   0        0        0      315 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count2-24px.svg
+-rw-r--r--   0        0        0      343 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count3-24px.svg
+-rw-r--r--   0        0        0      270 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count4-24px.svg
+-rw-r--r--   0        0        0      296 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count5-24px.svg
+-rw-r--r--   0        0        0      349 2020-06-10 13:51:52.000000 teda-3.0.0/teda/icons/delete_forever-24px.svg
+-rw-r--r--   0        0        0      518 2020-05-14 14:33:36.000000 teda-3.0.0/teda/icons/file-earmark-plus.svg
+-rw-r--r--   0        0        0      402 2020-07-01 12:47:01.000000 teda-3.0.0/teda/icons/filter_alt-24px.svg
+-rw-r--r--   0        0        0      257 2020-07-01 12:47:01.000000 teda-3.0.0/teda/icons/folder-24px.svg
+-rw-r--r--   0        0        0      217 2020-06-08 17:33:08.000000 teda-3.0.0/teda/icons/home-24px.svg
+-rw-r--r--   0        0        0      343 2020-06-08 17:32:29.000000 teda-3.0.0/teda/icons/house-24px.svg
+-rw-r--r--   0        0        0      196 2020-06-08 17:30:35.000000 teda-3.0.0/teda/icons/keyboard_arrow_left-24px.svg
+-rw-r--r--   0        0        0      194 2020-06-08 17:30:21.000000 teda-3.0.0/teda/icons/keyboard_arrow_right-24px.svg
+-rw-r--r--   0        0        0      977 2020-06-05 15:03:11.000000 teda-3.0.0/teda/icons/new.png
+-rw-r--r--   0        0        0      367 2020-06-10 13:51:52.000000 teda-3.0.0/teda/icons/not_started-24px.svg
+-rw-r--r--   0        0        0      261 2020-06-08 17:13:41.000000 teda-3.0.0/teda/icons/note_add-24px.svg
+-rw-r--r--   0        0        0      245 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/panning-24px.svg
+-rw-r--r--   0        0        0      292 2020-06-08 17:34:43.000000 teda-3.0.0/teda/icons/pause_circle_outline-24px.svg
+-rw-r--r--   0        0        0      344 2020-07-01 12:47:01.000000 teda-3.0.0/teda/icons/photo_filter-24px.svg
+-rw-r--r--   0        0        0      285 2020-06-08 17:34:37.000000 teda-3.0.0/teda/icons/play_circle_outline-24px.svg
+-rw-r--r--   0        0        0      379 2020-07-01 12:39:55.000000 teda-3.0.0/teda/icons/push_pin-24px.svg
+-rw-r--r--   0        0        0      304 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/save-24px.svg
+-rw-r--r--   0        0        0      203 2020-06-08 17:29:29.000000 teda-3.0.0/teda/icons/skip_next-24px.svg
+-rw-r--r--   0        0        0      206 2020-06-08 17:29:33.000000 teda-3.0.0/teda/icons/skip_previous-24px.svg
+-rw-r--r--   0        0        0     1245 2020-12-03 12:27:12.917053 teda-3.0.0/teda/icons/slider-24px.svg
+-rw-r--r--   0        0        0      385 2020-06-08 17:34:40.000000 teda-3.0.0/teda/icons/stop_circle-24px.svg
+-rw-r--r--   0        0        0     2638 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/x2-24px.svg
+-rw-r--r--   0        0        0     2159 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/x4-24px.svg
+-rw-r--r--   0        0        0      571 2023-04-28 02:39:09.916622 teda-3.0.0/teda/icons.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:08:12.000000 teda-3.0.0/teda/models/__init__.py
+-rw-r--r--   0        0        0     1014 2020-06-04 10:29:56.000000 teda-3.0.0/teda/models/cmaps.py
+-rw-r--r--   0        0        0     2920 2020-12-03 12:21:15.954502 teda-3.0.0/teda/models/coordinates.py
+-rw-r--r--   0        0        0     5435 2020-12-02 21:00:51.002196 teda-3.0.0/teda/models/scalesModel.py
+-rw-r--r--   0        0        0    16439 2023-04-28 03:24:57.907274 teda-3.0.0/teda/painterComponent.py
+-rw-r--r--   0        0        0     2967 2023-04-28 02:39:09.864767 teda-3.0.0/teda/painterShapes/CircleCenterShape.py
+-rw-r--r--   0        0        0        0 2020-06-04 11:27:56.000000 teda-3.0.0/teda/painterShapes/__init__.py
+-rw-r--r--   0        0        0     1885 2023-04-28 02:39:09.885266 teda-3.0.0/teda/painterShapes/circleShape.py
+-rw-r--r--   0        0        0     2227 2023-04-28 02:39:09.889630 teda-3.0.0/teda/painterShapes/rectangleMinatureShape.py
+-rwxr-xr-x   0        0        0     1410 2023-04-28 02:57:03.732713 teda-3.0.0/teda/teda_fits.py
+-rw-r--r--   0        0        0      123 2023-04-28 02:20:49.771269 teda-3.0.0/teda/version.py
+-rw-r--r--   0        0        0    34219 2023-04-28 02:50:04.151992 teda-3.0.0/teda/viewer_mainwindow.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:07:28.000000 teda-3.0.0/teda/views/__init__.py
+-rw-r--r--   0        0        0    17605 2023-04-28 03:13:13.702006 teda-3.0.0/teda/views/fitsplot.py
+-rw-r--r--   0        0        0     2602 2020-12-03 12:21:15.958669 teda-3.0.0/teda/views/fitsplot_fitsfile.py
+-rw-r--r--   0        0        0     2498 2020-12-02 21:00:51.007550 teda-3.0.0/teda/views/fitsplotcontrolled.py
+-rw-r--r--   0        0        0     1143 2020-06-04 11:45:26.000000 teda-3.0.0/teda/views/fitsplotzoomed.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:10:29.000000 teda-3.0.0/teda/widgets/__init__.py
+-rw-r--r--   0        0        0     6563 2023-04-28 02:49:22.960395 teda-3.0.0/teda/widgets/fileSystemWidget.py
+-rw-r--r--   0        0        0     2976 2023-04-28 02:39:09.907291 teda-3.0.0/teda/widgets/fullViewWidget.py
+-rw-r--r--   0        0        0     3270 2023-04-28 02:39:09.874014 teda-3.0.0/teda/widgets/headerTableWidget.py
+-rw-r--r--   0        0        0     2295 2023-04-28 02:39:09.924105 teda-3.0.0/teda/widgets/info.py
+-rw-r--r--   0        0        0     3293 2023-04-28 02:39:09.869422 teda-3.0.0/teda/widgets/radialprofile.py
+-rw-r--r--   0        0        0     5299 2023-04-28 02:39:09.899380 teda-3.0.0/teda/widgets/radialprofileIRAF.py
+-rw-r--r--   0        0        0    24112 2023-04-28 02:39:09.928943 teda-3.0.0/teda/widgets/scaleWidget.py
+-rw-r--r--   0        0        0    12534 2023-04-28 02:48:42.836537 teda-3.0.0/teda/widgets/scanToolbar.py
+-rw-r--r--   0        0        0     6207 2023-04-28 02:39:09.903950 teda-3.0.0/teda/widgets/slider.py
+-rw-r--r--   0        0        0     1357 2023-04-28 02:39:09.895011 teda-3.0.0/teda/widgets/zoomViewWidget.py
+-rw-r--r--   0        0        0    49708 1970-01-01 00:00:00.000000 teda-3.0.0/setup.py
+-rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 teda-3.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `teda-2.1.0/PKG-INFO` & `teda-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,156 +1,167 @@
 Metadata-Version: 2.1
 Name: teda
-Version: 2.1.0
-Summary: TeDa FITS Viewer
-Home-page: https://github.com/majkelx/teda
-Author: Akond Lab
-Author-email: 
+Version: 3.0.0
+Summary: Yet Another FITS Viewer
 License: MIT
-Description: # TeDa FITS Viewer
-        
-        Observatory optimized FITS Images viewer
-        
-        ![](img/teda.png)
-        
-        ## Key Features
-        * Flexible windows and widgets layout
-        * WCS support
-        * Radial Profile with gaussoide fit (try `r`-key)
-        * Scan mode: observes directory for changes and automatically opens new FITS
-        * Integrated ipython console with direct access to data and application
-        
-        ## Installation
-        ``` bash
-           pip install teda
-           teda_viewer 
-        ``` 
-        ### Optional dependencies
-        To use ipython console the `qtconsole` package is needed, additionally:
-        ``` bash
-            pip install qtconsole
-        ``` 
-        For directory scanning functionality, the `watchdog` package should be installed, e.g. 
-        ``` bash
-            pip install watchdog
-        ``` 
-        
-        ## Run
-        The installation scripts should install the command:
-        ```
-            teda_viewer
-        ```
-        Try 
-        ```
-            teda_viewer --help
-        ```
-        for list of command line parameters.
-        
-        ## Dynamic Scale and Color
-        The dynamic scale of the image, and color mapping can be adjusted form 
-        the **Dynamic Scale** panel. From menu: **View/Dynamic Scale**
-        
-        ## Fits Header Cards Pinning
-        On the FITS Header panel, selected keys can be *pinned* to appear
-        on the top ot the list. This can be done via context (right-click) menu.
-        
-        The set of pinned keys is saved and preserved between sessions.  
-        
-        ## Radial Profile
-        The **Radial Profile** button turns on the mode of selecting targets for 
-        the radial profile analysis. Make sure the radial profile panel is visible 
-        (View/Radial Profile). The shortcut for displaying radial profile of the star 
-        under cursor is the **R**-key.
-        
-        The centroid of the star is corrected within small (be precise!) radius
-        using the bivariate gaussoide fit.
-        
-        Together with the pixels values, the radial profile presents 1D fit of
-        "gaussian(r) + sky". This fit provides information of presented fwhm and sky level.
-           
-        
-        ## Integrated Python Console
-        In order to use integrated python console the `qtconsole` module, and it's
-        dependencies (jupyter related) have to be installed. This is not done by
-        default `pip` installation to keep number of dependencies reasonably small.
-        Install `qtconsole` by:
-        ``` bash
-            pip install qtconsole
-        ``` 
-        
-        The console is available form menu **View/Python Console**
-        ### Predefined variables
-        The console has a number of predefined variables set:
-        * `ax: WCSAxesSubplot` main plotting axes.
-        * `window: MainWindow` main window
-        * `data: numpy.ndarray` current HDU data
-        * `header: astropy.fits.Header` current HDU header
-        * `wcs: astropy.wcs.WCS` the WCS transformer
-        
-        ### Plotting
-        To plot directly on the console, run the following magic command `%matplotlib inline`.
-        
-        When plotting on the main canvas, the result will appear after redrawing
-        main figure by `ax.figure.canvas.draw()`.
-        
-        The example below, draws linear profile on the console and corresponding
-        line on the main FITS display:    
-          
-        ``` python
-        %matplotlib inline
-        import matplotlib.pyplot as plt
-        ax.plot([10,30], [10,10])
-        ax.figure.canvas.draw()
-        plt.plot(data[10,10:30])
-        ```
-        
-        ## Directory Scan
-        The **Scan Toolbar** (hidden by default) provides controls for the 
-        directory scanning mode.
-        
-        This mode is intended to observe newly created FITS files in observatory.
-        
-        After pressing **Scan** button, and choosing directory, TeDa Fits Viewer will
-        load most recent FITS file from that directory, and keep watching the directory 
-        for changes. When new FITS file is added to directory, it will be loaded 
-        automatically.
-        
-        User can pause scanning using **Pause** button. There is also **auto pause** feature,
-        when active, any mouse movement in the main area pauses scanning for 5 seconds,
-        avoiding FITS reload when working.
-        
-        After un-pausing (manually or after idle 5 seconds when auto-pause) the newest
-        FITS will be loaded if any new files appeared during the pause.
-        
-        Directory scanning needs the [`watchdog`](https://pypi.org/project/watchdog/) component to be 
-        installed manually (optional dependence).
-        
-        ## Directory Panel
-        The Directory Panel can be shown using menu command **View-Directory view**.
-        
-        The Directory Panel is convenient files navigator. The panel has two views:
-        * Directory Tree
-        * Files List
-        
-        User can collapse any of them using divider handle and use only remaining one.
-        If the tree view is the only visible, it shows directories and files as well.      
-        
-        ## Development version install
-        ``` bash
-        
-            git clone https://github.com/majkelx/teda.git
-            cd teda
-            python -m venv venv
-            source ./venv/bin/activate
-            pip install -r requirements.txt
-            pip install -e .
-        ```
-        
-        ## Bugs, remarks, greetings and contribution 
-        Please use [GitHub issues tracker](https://github.com/majkelx/teda/issues) 
-        and [pull requests](https://github.com/majkelx/teda/pulls).
-        
-        
-        @2020  [AkondLab](http://www.akond.com) for the [Araucaria Project](https://araucaria.camk.edu.pl).
-        
-Platform: UNKNOWN
+Author: majkelx
+Author-email: mkalusz@camk.edu.pl
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astropy (>=5.2.2,<6.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: pyside6 (>=6.5.0,<7.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: traitlets (>=5.9.0,<6.0.0)
 Description-Content-Type: text/markdown
+
+# TeDa FITS Viewer
+
+Observatory optimized FITS Images viewer
+
+![](img/teda.png)
+
+## Key Features
+* Flexible windows and widgets layout
+* WCS support
+* Radial Profile with gaussoide fit (try `r`-key)
+* Scan mode: observes directory for changes and automatically opens new FITS
+* Integrated ipython console with direct access to data and application
+
+## Installation
+``` bash
+   pip install teda
+   teda_viewer 
+``` 
+### Optional dependencies
+To use ipython console the `qtconsole` package is needed, additionally:
+``` bash
+    pip install qtconsole
+``` 
+For directory scanning functionality, the `watchdog` package should be installed, e.g. 
+``` bash
+    pip install watchdog
+``` 
+
+## Run
+The installation scripts should install the command:
+```
+    teda_viewer
+```
+Try 
+```
+    teda_viewer --help
+```
+for list of command line parameters.
+
+## Dynamic Scale and Color
+The dynamic scale of the image, and color mapping can be adjusted form 
+the **Dynamic Scale** panel. From menu: **View/Dynamic Scale**
+
+## Fits Header Cards Pinning
+On the FITS Header panel, selected keys can be *pinned* to appear
+on the top ot the list. This can be done via context (right-click) menu.
+
+The set of pinned keys is saved and preserved between sessions.  
+
+## Radial Profile
+The **Radial Profile** button turns on the mode of selecting targets for 
+the radial profile analysis. Make sure the radial profile panel is visible 
+(View/Radial Profile). The shortcut for displaying radial profile of the star 
+under cursor is the **R**-key.
+
+The centroid of the star is corrected within small (be precise!) radius
+using the bivariate gaussoide fit.
+
+Together with the pixels values, the radial profile presents 1D fit of
+"gaussian(r) + sky". This fit provides information of presented fwhm and sky level.
+   
+
+## Integrated Python Console
+In order to use integrated python console the `qtconsole` module, and it's
+dependencies (jupyter related) have to be installed. This is not done by
+default `pip` installation to keep number of dependencies reasonably small.
+Install `qtconsole` by:
+``` bash
+    pip install qtconsole
+``` 
+
+The console is available form menu **View/Python Console**
+### Predefined variables
+The console has a number of predefined variables set:
+* `ax: WCSAxesSubplot` main plotting axes.
+* `window: MainWindow` main window
+* `data: numpy.ndarray` current HDU data
+* `header: astropy.fits.Header` current HDU header
+* `wcs: astropy.wcs.WCS` the WCS transformer
+
+### Plotting
+To plot directly on the console, run the following magic command `%matplotlib inline`.
+
+When plotting on the main canvas, the result will appear after redrawing
+main figure by `ax.figure.canvas.draw()`.
+
+The example below, draws linear profile on the console and corresponding
+line on the main FITS display:    
+  
+``` python
+%matplotlib inline
+import matplotlib.pyplot as plt
+ax.plot([10,30], [10,10])
+ax.figure.canvas.draw()
+plt.plot(data[10,10:30])
+```
+
+## Directory Scan
+The **Scan Toolbar** (hidden by default) provides controls for the 
+directory scanning mode.
+
+This mode is intended to observe newly created FITS files in observatory.
+
+After pressing **Scan** button, and choosing directory, TeDa Fits Viewer will
+load most recent FITS file from that directory, and keep watching the directory 
+for changes. When new FITS file is added to directory, it will be loaded 
+automatically.
+
+User can pause scanning using **Pause** button. There is also **auto pause** feature,
+when active, any mouse movement in the main area pauses scanning for 5 seconds,
+avoiding FITS reload when working.
+
+After un-pausing (manually or after idle 5 seconds when auto-pause) the newest
+FITS will be loaded if any new files appeared during the pause.
+
+Directory scanning needs the [`watchdog`](https://pypi.org/project/watchdog/) component to be 
+installed manually (optional dependence).
+
+## Directory Panel
+The Directory Panel can be shown using menu command **View-Directory view**.
+
+The Directory Panel is convenient files navigator. The panel has two views:
+* Directory Tree
+* Files List
+
+User can collapse any of them using divider handle and use only remaining one.
+If the tree view is the only visible, it shows directories and files as well.      
+
+## Development version install
+``` bash
+
+    git clone https://github.com/majkelx/teda.git
+    cd teda
+    python -m venv venv
+    source ./venv/bin/activate
+    pip install -r requirements.txt
+    pip install -e .
+```
+
+## Bugs, remarks, greetings and contribution 
+Please use [GitHub issues tracker](https://github.com/majkelx/teda/issues) 
+and [pull requests](https://github.com/majkelx/teda/pulls).
+
+
+@2020  [AkondLab](http://www.akond.com) for the [Araucaria Project](https://araucaria.camk.edu.pl).
+
```

### Comparing `teda-2.1.0/README.md` & `teda-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/command_line.py` & `teda-3.0.0/teda/command_line.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
-from PySide2.QtCore import QCommandLineParser, QCommandLineOption, QStringListModel, QCoreApplication
-from PySide2.QtWidgets import QApplication
+from PySide6.QtCore import QCommandLineParser, QCommandLineOption, QStringListModel, QCoreApplication
+from PySide6.QtWidgets import QApplication
 
 
 class CommandLineParseResult(Enum):
     CommandLineOk = 0
     CommandLineError = 1
     CommandLineVersionRequested = 2
     CommandLineHelpRequested = 3
```

### Comparing `teda-2.1.0/teda/console.py` & `teda-3.0.0/teda/console.py`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/fitsopen.py` & `teda-3.0.0/teda/fitsopen.py`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/fitting.py` & `teda-3.0.0/teda/fitting.py`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/icons/1-2-24px.svg` & `teda-3.0.0/teda/icons/1-2-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/icons/1-4-24px.svg` & `teda-3.0.0/teda/icons/1-4-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/icons/file-earmark-plus.svg` & `teda-3.0.0/teda/icons/file-earmark-plus.svg`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/icons/new.png` & `teda-3.0.0/teda/icons/new.png`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/icons/x2-24px.svg` & `teda-3.0.0/teda/icons/x2-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/icons/x4-24px.svg` & `teda-3.0.0/teda/icons/x4-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/icons.py` & `teda-3.0.0/teda/icons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from PySide2.QtGui import QIcon
+from PySide6.QtGui import QIcon
 
 
 class IconFactory(object):
     # subdir = 'icons'
     subdir = 'icons'
     prefix = ''
     suffix = '-24px'
```

### Comparing `teda-2.1.0/teda/models/cmaps.py` & `teda-3.0.0/teda/models/cmaps.py`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/models/coordinates.py` & `teda-3.0.0/teda/models/coordinates.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def calc_wcs(self):
         change = False
         try:
             if self.wcs is None or self.img_x is None or self.img_y is None:
                 raise ValueError()
             world = SkyCoord.from_pixel(self.img_x, self.img_y, wcs=self.wcs)
-            if self.wcs_coo != world:
+            if self.wcs_coo is None or self.wcs_coo != world:
                 self.wcs_coo = world
                 change = True
 
         except ValueError:
             if self.wcs_coo is not None:
                 self.wcs_coo = None
                 change = True
```

### Comparing `teda-2.1.0/teda/models/scalesModel.py` & `teda-3.0.0/teda/models/scalesModel.py`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/painterComponent.py` & `teda-3.0.0/teda/painterComponent.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,20 @@
         if type == "rectangleMiniature":
             self.rectangleMiniature = []
             c = RectangleMiniatureShape(x, y, size, size2)
             self.rectangleMiniature.append(c)
 
 
     def paintAllShapes(self, axes):
-        axes.patches.clear()
-        axes.lines.clear()
+        # axes.patches.clear()
+        # axes.lines.clear()
+        for p in axes.patches:
+            p.remove()
+        for p in axes.lines:
+            p.remove()
         self.listOfPaintedShapes = []
         self.drs = []
         for shape in self.shapes:
             shap=shape.paintShape(axes)
             self.listOfPaintedShapes.append(shap)
             dr = DraggablePoint(shap, shape, self)
             dr.connect()
@@ -80,16 +84,20 @@
             dr = DraggablePoint(shap, shape, self)
             dr.connect()
             self.drs.append(dr)
         self.tempCanvas.draw_idle()
 
     def makeAllShapesDraggable(self, axes):
         self.draggableActive = True
-        axes.patches.clear()
-        axes.lines.clear()
+        # axes.patches.clear()
+        # axes.lines.clear()
+        for p in axes.patches:
+            p.remove()
+        for p in axes.lines:
+            p.remove()
         self.drs = []
         for shape in self.shapes:
             shap = shape.paintShape(axes)
             dr = DraggablePoint(shap, shape, self)
             dr.connect()
             self.drs.append(dr)
         for shape in self.centerCircle:
@@ -124,39 +132,41 @@
         self.removeCanvasEvents(canvas)
 
     def stopMovingEvents(self, canvas):
         self.removeCanvasEvents(canvas)
 
     def startLine(self,canvas,x1,y1):
         ax = canvas.figure.axes[0]
-        self.tempLines = ax.lines.copy()
+        self.tempLines = [l for l in ax.lines]   # .copy()
         canvas.draw_idle()
 
     def paintLine(self,canvas,x1,x2,y1,y2):
         ax = canvas.figure.axes[0]
         if self.templine != None:
             self.templine = None
-            ax.lines = ax.lines[:-1]
+            ax.lines[-1].remove()
         if self.tempcircle != None:
-            ax.patches.remove(self.tempcircle)
+            self.tempcircle.remove()
             self.tempcircle = None
         xcord = [x1,x2]
         ycord = [y1,y2]
         r = sqrt(pow((x2 - x1), 2) + pow((y2 - y1), 2))
         self.tempcircle = plt.Circle((x1, y1), r, color='g', fill=False)
         ax.add_patch(self.tempcircle)
         self.templine = ax.plot(xcord, ycord, linewidth=1, color='g')
         canvas.draw_idle()
 
     def hideLine(self,canvas):
         # restore the background region
         ax = canvas.figure.axes[0]
         self.templine = None
         self.tempcircle = None
-        ax.lines = self.tempLines.copy()
+        for l in self.tempLines:
+            ax.add_line(l)
+        # ax.lines = self.tempLines    #.copy()
         canvas.draw_idle()
 
     def setCanvas(self, canvas):
         self.tempCanvas = canvas
 
     def setCanvasEvents(self,canvas, mode):
         self.tempCanvas = canvas
```

### Comparing `teda-2.1.0/teda/painterShapes/CircleCenterShape.py` & `teda-3.0.0/teda/painterShapes/CircleCenterShape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide2.QtCore import Qt
+from PySide6.QtCore import Qt
 import matplotlib.pyplot as plt
 
 
 class CircleCenterShape(object):
     """Center Circle"""
 
     def __init__(self,x,y,size,color='r'):
```

### Comparing `teda-2.1.0/teda/painterShapes/circleShape.py` & `teda-3.0.0/teda/painterShapes/circleShape.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide2.QtCore import Qt
+from PySide6.QtCore import Qt
 import matplotlib.pyplot as plt
 
 
 class CircleShape(object):
     """Circle"""
 
     def __init__(self,x,y,size,color='r'):
```

### Comparing `teda-2.1.0/teda/painterShapes/rectangleMinatureShape.py` & `teda-3.0.0/teda/painterShapes/rectangleMinatureShape.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide2.QtCore import Qt
+from PySide6.QtCore import Qt
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 
 
 class RectangleMiniatureShape(object):
     """Center Circle"""
```

### Comparing `teda-2.1.0/teda/teda_fits.py` & `teda-3.0.0/teda/teda_fits.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 """
 TeDa FITS Viewer application
 
 by Akond Lab
 """
 from sys import stderr
 
-from PySide2.QtCore import QCommandLineParser, QCoreApplication
-from PySide2.QtWidgets import QApplication
+from PySide6.QtCore import QCommandLineParser, QCoreApplication
+from PySide6.QtWidgets import QApplication
 
 from teda.command_line import TedaCommandLine, CommandLineParseResult
 from teda.viewer_mainwindow import MainWindow
 from teda.version import __version__
 
 def main():
     import sys
@@ -37,12 +37,12 @@
         return 0
 
 
     mainWin = MainWindow(tcl)
     # mainWin.resize(800, 600)   # now in config, see: MainWindow.readWindowSettings
     mainWin.show()
 
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `teda-2.1.0/teda/viewer_mainwindow.py` & `teda-3.0.0/teda/viewer_mainwindow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """TeDa FITS Viewer main window"""
 import os
 
-import PySide2
-from PySide2 import QtWidgets, QtCore
-from PySide2.QtCore import QFile, Qt, QTextStream, QSettings
-from PySide2.QtGui import QFont, QIcon, QKeySequence
-from PySide2.QtPrintSupport import QPrintDialog, QPrinter
-from PySide2.QtWidgets import (QAction, QApplication, QLabel, QDialog, QDockWidget, QWidget, QPushButton,
+import PySide6
+from PySide6 import QtWidgets, QtCore
+from PySide6.QtCore import QFile, Qt, QTextStream, QSettings
+from PySide6.QtGui import QFont, QIcon, QKeySequence, QKeyEvent, QMouseEvent, QAction
+from PySide6.QtPrintSupport import QPrintDialog, QPrinter
+from PySide6.QtWidgets import (QApplication, QLabel, QDialog, QDockWidget, QWidget, QPushButton,
                                QFileDialog, QMainWindow, QMessageBox, QTableWidgetItem,
                                QComboBox)
 
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 
 from teda.version import __version__
@@ -25,48 +25,51 @@
 from teda.widgets.headerTableWidget import HeaderTableWidget
 from teda.widgets.scaleWidget import ScaleWidget
 from teda.widgets.scanToolbar import ScanToolbar
 from teda.widgets.info import InfoWidget
 from teda.models.cmaps import ColorMaps
 from teda.models.scalesModel import ScalesModel
 from teda.icons import IconFactory
+from teda import draggingComponent
 from . import console
 from .widgets.fileSystemWidget import FileSystemWidget
 
 
 class MainWindow(QMainWindow):
     def __init__(self, tedaCommandLine):
         super().__init__()
         self.tedaCommandLine = tedaCommandLine
         self.cmaps = ColorMaps()
         self.combobox = QComboBox()
         self.filename = None
+        self.isMousePressed = False
+        self.isCmdPressed = False
         self.cursor_coords = CoordinatesModel()
         self.scales_model = ScalesModel()
         fig = Figure(figsize=(14, 10))
         fig.tight_layout()
         self.fits_image = FitsPlotter(figure=fig)
         fig.subplots_adjust(left=0, bottom=0.001, right=1, top=1, wspace=None, hspace=None)
 
         self.fits_image = FitsPlotterFitsFile(figure=fig, cmap_model=self.cmaps,
-                                              scale_model=self.scales_model
-                                              )
+                                              scale_model=self.scales_model)
         self.central_widget = FigureCanvas(fig)
         self.setCentralWidget(self.central_widget)
 
         self.current_x_coord = 0
         self.current_y_coord = 0
 
         self.fullWidgetXcord = 0
         self.fullWidgetYcord = 0
         self.centralWidgetcordX = 0
         self.centralWidgetcordY = 0
 
         self.painterComponent = PainterComponent(self.fits_image)
-        self.painterComponent.startMovingEvents(self.central_widget)
+        # self.painterComponent.startMovingEvents(self.central_widget)
+        self.painterComponent.setCanvas(self.central_widget)
         self.scanObject = ScanToolbar(self)
         self.createActions()
         self.createMenus()
         self.createToolBars()
         self.createStatusBar()
         self.createDockWindows()
         if not self.tedaCommandLine.ignoreSettings:
@@ -76,14 +79,16 @@
 
         self.painterComponent.observe(lambda change: self.onAutoCenterChange(change), ['auto_center'])
 
         self.readWindowSettings()
         self.readAppState()
 
         self.updateHeaderData()
+        self.dragging = draggingComponent.Dragging(widget=self, scale_widget=self.scaleWidget)
+        self.activeLinearAdjustmentByMouseMovement()
 
         # Observing here may be to late for values loaded from settings e.g. via readAppState
         self.painterComponent.observe(lambda change: self.onCenterCircleChange(change), ['ccenter_x', 'ccenter_y'])
         self.painterComponent.observe(lambda change: self.onCenterCircleRadiusChange(change), ['cradius'])
         self.fits_image.observe(lambda change: self.onMouseMoveOnImage(change), ['mouse_xdata', 'mouse_ydata'])
         # self.cmaps.observe(lambda change: self.on_colormap_change(change))
         self.full_view_widget.painterComponent.observe(lambda change: self.onRectangleInWidgetMove(change), ['viewX', 'viewY'])
@@ -92,15 +97,15 @@
 
         # open last fits
         try:
             self.openLastFits()
         except FileNotFoundError:
             print('Błąd w odczycie lub brak ostatio wczytanego pliku')
 
-    def closeEvent(self, event: PySide2.QtGui.QCloseEvent):
+    def closeEvent(self, event: PySide6.QtGui.QCloseEvent):
         self.writeAppState()
         self.writeWindowSettings()
         if not self.tedaCommandLine.ignoreSettings:
             self.scaleWidget.writeSlidersValues()
         super().closeEvent(event)
 
     def keyPressEvent(self, e):
@@ -109,14 +114,28 @@
         if e.key() == Qt.Key_R:
             action = self.dockRadialFit.toggleViewAction()
             if not action.isChecked():
                 action.trigger()
             if (self.cursor_coords.img_x != 0 and self.cursor_coords.img_x != None) and (self.cursor_coords.img_y != 0 and self.cursor_coords.img_y != None):
                 self.painterComponent.add(self.cursor_coords.img_x, self.cursor_coords.img_y, type="circleCenter")
                 self.painterComponent.paintAllShapes(self.central_widget.figure.axes[0])
+        if e.key() == Qt.Key_Control:
+            self.isCmdPressed = True
+
+    def keyReleaseEvent(self, event:PySide6.QtGui.QKeyEvent):
+        if event.key() == Qt.Key_Control:
+            self.isCmdPressed = False
+
+    def canvasMousePressEvent(self, event):
+        self.isMousePressed = not self.isMousePressed
+
+    def mouseMoveEventOnCanvas(self, event):
+        if self.isCmdPressed:
+            if self.isMousePressed:
+                self.dragging.mouseMoveEvent(event)
 
     def print_(self):
         document = self.textEdit.document()
         printer = QPrinter()
 
         dlg = QPrintDialog(printer, self)
         if dlg.exec_() != QDialog.Accepted:
@@ -163,16 +182,16 @@
             try:
                 self.central_widget.figure.savefig(dialog[0])
             except ValueError:
                 print("Unsupported format")
 
     def open_fits(self, fileName):
         """Opens specified FITS file and loads it to user interface"""
+        self.fits_image.set_file(fileName)
         self.filename = fileName
-        self.fits_image.set_file(self.filename)
         self.cursor_coords.set_wcs_from_fits(self.fits_image.header)  # TODO: one up and extract and set wcs in fits_image before plot
         self.fits_image.set_wcs(self.cursor_coords.wcs)
 
         self.fits_image.plot()
 
         self.radial_profile_widget.set_data(self.fits_image.data)
         self.radial_profile_iraf_widget.set_data(self.fits_image.data)
@@ -255,15 +274,15 @@
                           "</ul>"
                           "Created by <a href='https://akond.com'>Akond Lab</a> for The "
                           "<a href='https://araucaria.camk.edu.pl'>Araucaria Project</a><br/>"
                           "Licence: MIT <br/>"
                           "3rd party work used: "
                           "<a href='https://material.io/resources/icons/'> Google Material Icons</a>, "
                           "<a href='https://www.astropy.org'> AstroPy</a>, "
-                          "<a href='https://doc.qt.io/qtforpython/'> Qt5/PySide2</a>, "
+                          "<a href='https://doc.qt.io/qtforpython/'> Qt5/PySide6</a>, "
                           "<a href='https://www.scipy.org'> SciPy</a>, and other..."
                           "<br/><br/>"
                           "Visit the <a href='https://github.com/majkelx/teda'>project's GitHub  page</a> for help"
                           " and the issue tracker"
                           )
 
     def on_console_show(self):
@@ -329,22 +348,30 @@
         self.centerCircleAct = QAction(IconFactory.getIcon('add_circle_outline'), 'Radial profile', self,
                                  statusTip="Radial profile with gaussoide fit [R]-key", triggered=self.changeAddCenterCircleStatus)
         self.autoCenterAct = QAction('Auto Center', self,
                                      statusTip="Automatically center cursor on star centroid",
                                      triggered=self.changeAutoCenter)
         self.deleteAct = QAction(IconFactory.getIcon('delete_forever'), 'Delete selected', self,
                                  statusTip="Delete selected [Del]-key", triggered=self.deleteSelected)
+
+        self.slidersAct = QAction(IconFactory.getIcon('slider'), 'Dynamic Scale Sliders', self,
+                                  statusTip='Show/Hide Dynamic Scale',
+                                  triggered=self.dynamicScaleDockWidgetTriggerActions)
+
         self.panningAct.setCheckable(True)
         self.panningAct.setChecked(True)
         self.circleAct.setCheckable(True)
         self.autoCenterAct.setCheckable(True)
         self.autoCenterAct.setChecked(self.painterComponent.auto_center)
         self.centerCircleAct.setCheckable(True)
 
 
+
+
+
     def createMenus(self):
         self.fileMenu = self.menuBar().addMenu("&File")
         self.fileMenu.addAction(self.openAct)
         self.fileMenu.addAction(self.scanObject.scanAct)
         self.fileMenu.addAction(self.scanObject.stopAct)
         self.fileMenu.addAction(self.scanObject.pauseAct)
         self.fileMenu.addAction(self.scanObject.resumeAct)
@@ -426,20 +453,26 @@
 
         self.mouseActionToolBar = self.addToolBar("Mouse Task Toolbar")
         self.mouseActionToolBar.addAction(self.panningAct)
         self.mouseActionToolBar.addAction(self.circleAct)
         self.mouseActionToolBar.addAction(self.centerCircleAct)
         self.mouseActionToolBar.addAction(self.deleteAct)
 
+        self.sliderToolBar = self.addToolBar("Slider Toolbar")
+        self.slidersAct.setChecked(True)
+        self.sliderToolBar.addAction(self.slidersAct)
+
+
         self.viewMenu.addAction(self.fileToolBar.toggleViewAction())
         self.viewMenu.addAction(self.hduToolBar.toggleViewAction())
         self.viewMenu.addAction(self.scanToolBar.toggleViewAction())
         # self.viewMenu.addAction(self.infoToolBar.toggleViewAction())
         self.viewMenu.addAction(self.zoomToolBar.toggleViewAction())
         self.viewMenu.addAction(self.mouseActionToolBar.toggleViewAction())
+        self.viewMenu.addAction(self.sliderToolBar.toggleViewAction())
         self.viewMenu.addSeparator()
 
     def nextHDU(self):
         self.fits_image.changeHDU(True, 1)
         self.updateHeaderData()
 
     def prevHDU(self):
@@ -513,28 +546,29 @@
 
 
     def createStatusBar(self):
         self.statusBar().showMessage("Ready")
 
     def createDockWindows(self):
         # Scale
-        dock = QDockWidget("Dynamic Scale", self)
-        dock.setObjectName("SCALE")
-        dock.setAllowedAreas(Qt.LeftDockWidgetArea | Qt.RightDockWidgetArea | Qt.TopDockWidgetArea)
+        self.dynamic_scale_dock = QDockWidget("Dynamic Scale", self)
+        self.dynamic_scale_dock.setObjectName("SCALE")
+        self.dynamic_scale_dock.setAllowedAreas(Qt.LeftDockWidgetArea | Qt.RightDockWidgetArea | Qt.TopDockWidgetArea)
         self.scaleWidget = ScaleWidget(self, scales_model=self.scales_model, cmap_model=self.cmaps)
-        dock.setWidget(self.scaleWidget)
-        self.addDockWidget(Qt.RightDockWidgetArea, dock)
-        self.viewMenu.addAction(dock.toggleViewAction())
-        dock.setFloating(True)
-        dock.hide()
+        self.dynamic_scale_dock.setWidget(self.scaleWidget)
+        self.addDockWidget(Qt.RightDockWidgetArea, self.dynamic_scale_dock)
+        self.viewMenu.addAction(self.dynamic_scale_dock.toggleViewAction())
+        self.dynamic_scale_dock.setFloating(True)
+        self.dynamic_scale_dock.hide()
 
 
         #radial profiles
         dock = QDockWidget("Radial Profile Fit", self)
         dock.setObjectName("RADIAL_PROFILE_IRAF")
+
         dock.setAllowedAreas(Qt.LeftDockWidgetArea | Qt.RightDockWidgetArea | Qt.TopDockWidgetArea)
         self.radial_profile_iraf_widget = IRAFRadialProfileWidget(self.fits_image.data)
         dock.setWidget(self.radial_profile_iraf_widget)
         self.addDockWidget(Qt.RightDockWidgetArea, dock)
         self.viewMenu.addAction(dock.toggleViewAction())
         self.dockRadialFit = dock
 
@@ -608,17 +642,25 @@
     #     self.cmaps.set_active_color_map(color)
 
     # def on_colormap_change(self, change):
     #     self.fits_image.cmap = self.cmaps.get_active_color_map()
     #     self.fits_image.plot()
     #     self.updateFitsInWidgets()
 
+
     def onAutoCenterChange(self, change):
         self.autoCenterAct.setChecked(change.new)
 
+    def dynamicScaleDockWidgetTriggerActions(self):
+        if self.dynamic_scale_dock.isHidden():
+            self.dynamic_scale_dock.show()
+        else:
+            self.dynamic_scale_dock.hide()
+
+
     def onCenterCircleChange(self, change):
         self.radial_profile_widget.set_centroid(self.painterComponent.ccenter_x, self.painterComponent.ccenter_y)
         self.radial_profile_iraf_widget.set_centroid(self.painterComponent.ccenter_x, self.painterComponent.ccenter_y)
 
     def onCenterCircleRadiusChange(self, change):
         self.radial_profile_widget.set_radius(self.painterComponent.cradius)
         self.radial_profile_iraf_widget.set_radius(self.painterComponent.cradius)
@@ -663,14 +705,19 @@
             self.zoom_view_widget.setXYofZoom(self.fits_image, self.current_x_coord, self.current_y_coord, self.fits_image.zoom)
             if not self.hasFocus():
                 self.setFocus()
             if self.scanObject.activeScan and self.scanObject.enableAutopause:#reser autopause
                 if not self.scanObject.obserwableValue.autopauseFlag:
                     self.scanObject.obserwableValue.autopauseFlag = True
 
+    def activeLinearAdjustmentByMouseMovement(self):
+        self.central_widget.mpl_connect('motion_notify_event', self.mouseMoveEventOnCanvas)
+        self.central_widget.mpl_connect('button_press_event', self.canvasMousePressEvent)
+        self.central_widget.mpl_connect('button_release_event', self.canvasMousePressEvent)
+
     def onMouseZoomOnImage(self, change):
         changed = False
         if change.new is not None:
             changed = True
         if changed:
             self.full_view_widget.updateMiniatureShape(self.fits_image.viewX,self.fits_image.viewY,self.fits_image.viewW,self.fits_image.viewH)
```

### Comparing `teda-2.1.0/teda/views/fitsplot.py` & `teda-3.0.0/teda/views/fitsplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                     interval = vis.MinMaxInterval()
                 elif interval == 'manual':  # args: vmin, vmax
                     interval = vis.ManualInterval(**kwargs)
                 elif interval == 'percentile':  # args: percentile, n_samples
                     interval = vis.PercentileInterval(**kwargs)
                 elif interval == 'asymetric':  # args: lower_percentile, upper_percentile, n_samples
                     interval = vis.AsymmetricPercentileInterval(**kwargs)
-                elif interval == 'zscale':  # args: nsamples=1000, contrast=0.25, max_reject=0.5, min_npixels=5, krej=2.5, max_iterations=5
+                elif interval == 'zscale':  # args: n_samples=1000, contrast=0.25, max_reject=0.5, min_npixels=5, krej=2.5, max_iterations=5
                     interval = vis.ZScaleInterval(**kwargs)
                 else:
                     raise ValueError('Unknown interval:' + interval)
         self.interval = interval
         if self.img is not None:
             self.img.set_norm(vis.ImageNormalize(self.data, interval=self.interval, stretch=self.stretch, clip=True))
 
@@ -213,15 +213,15 @@
         self.figure = None
 
     interval_kws_defaults = {
         'minmax': {},
         'manual': {'vmin': 0.0, 'vmax': 30000},
         'percentile': {'percentile': 0.1, 'n_samples': 1000},
         'asymetric': {'lower_percentile': 0.1, 'upper_percentile': 0.2, 'n_samples': 1000},
-        'zscale': {'nsamples': 1000, 'contrast': 0.25, 'max_reject': 0.5,
+        'zscale': {'n_samples': 1000, 'contrast': 0.25, 'max_reject': 0.5,
                    'min_npixels': 5, 'krej': 2.5, 'max_iterations': 5},
     }
 
     stretch_kws_defaults = {
         'asinh': {'a': 0.1},
         'contrastbias': {'contrast': 2.0, 'bias': 1.0},
         'histogram': {},
```

### Comparing `teda-2.1.0/teda/views/fitsplot_fitsfile.py` & `teda-3.0.0/teda/views/fitsplot_fitsfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 
     def open(self):
         if self._huds is None and self.fitsfile:
             self._huds = fits.open(self.fitsfile, lazy_load_hdus=False)
             self._huds.info()
 
     def set_file(self, filename):
-        self._huds = None
+        if filename is not None:
+            self._huds = fits.open(filename, lazy_load_hdus=False)
+            self._huds.info()
+        else:
+            self._huds = None
         self.fitsfile = filename
 
     @data.setter
     def data(self, d):
         raise TypeError('Can not set data directly in FitsPlotterFitsFile. Set fits file instead')
 
     def changeHDU(self, relative, val):
```

### Comparing `teda-2.1.0/teda/views/fitsplotcontrolled.py` & `teda-3.0.0/teda/views/fitsplotcontrolled.py`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/views/fitsplotzoomed.py` & `teda-3.0.0/teda/views/fitsplotzoomed.py`

 * *Files identical despite different names*

### Comparing `teda-2.1.0/teda/widgets/fileSystemWidget.py` & `teda-3.0.0/teda/widgets/fileSystemWidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PySide2.QtCore import QDir
-from PySide2.QtGui import Qt
-from PySide2.QtWidgets import QWidget, QHBoxLayout, QFileSystemModel, QTreeView, QListView, QAction, QVBoxLayout, \
+from PySide6.QtCore import QDir
+from PySide6.QtGui import Qt, QAction
+from PySide6.QtWidgets import QWidget, QHBoxLayout, QFileSystemModel, QTreeView, QListView, QVBoxLayout, \
     QPushButton, QToolButton, QFileDialog, QSplitter
 
 from teda.icons import IconFactory
 
 
 class FileSystemWidget(QWidget):
 
@@ -105,15 +105,18 @@
 
     def onFilesDoubleClick(self, item):
         index = self.files.selectedIndexes()[0]
         info = self.filesModel.fileInfo(index)
         if info.isDir():
             self.setPath(info.filePath())
         else:
-            self.mainWindow.open_fits(info.filePath())
+            try:
+                self.mainWindow.open_fits(info.filePath())
+            except FileNotFoundError:
+                self.setPath(self.currentPath) # refesh maybe?
 
     def setPath(self, path):
         self.currentPath = path
 
         index = self.dirsModel.index(self.currentPath)
         self.dirs.setCurrentIndex(index)
         self.dirs.setExpanded(index, True)
```

### Comparing `teda-2.1.0/teda/widgets/fullViewWidget.py` & `teda-3.0.0/teda/widgets/fullViewWidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide2.QtWidgets import QWidget, QHBoxLayout
+from PySide6.QtWidgets import QWidget, QHBoxLayout
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from teda.views.fitsplotcontrolled import (FitsPlotterControlled)
 from teda.painterComponent import PainterComponent
 
 
 class FullViewWidget(QWidget):
```

### Comparing `teda-2.1.0/teda/widgets/headerTableWidget.py` & `teda-3.0.0/teda/widgets/headerTableWidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PySide2.QtWidgets import (QTableWidget, QTableWidgetItem, QMenu)
-from PySide2.QtGui import (QIcon)
-import PySide2
+from PySide6.QtWidgets import (QTableWidget, QTableWidgetItem, QMenu)
+from PySide6.QtGui import (QIcon)
+import PySide6
 
 from teda.icons import IconFactory
 
 class HeaderTableWidget(QTableWidget):
 
     def __init__(self, parent = None):
         QTableWidget.__init__(self, parent)
@@ -35,15 +35,15 @@
 
     def createRow(self, pos, key, val, pin):
         newKeyItem = QTableWidgetItem()
         newKeyItem.setText(key)
         newValItem = QTableWidgetItem()
         newValItem.setText(val)
 
-        color = PySide2.QtGui.QColor(200, 220, 200)
+        color = PySide6.QtGui.QColor(200, 220, 200)
         if bool(pin):
             # newKeyItem.setIcon(QIcon.fromTheme('emblem-important'));
             newKeyItem.setIcon(IconFactory.getIcon('push_pin'))
             newKeyItem.setBackground(color)
             newValItem.setBackground(color)
         self.insertRow(pos)
         self.setItem(pos, 0, newKeyItem)
```

### Comparing `teda-2.1.0/teda/widgets/info.py` & `teda-3.0.0/teda/widgets/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from os import path
-from PySide2.QtWidgets import QWidget, QHBoxLayout, QStackedLayout, QLabel, QFormLayout, QLineEdit
+from PySide6.QtWidgets import QWidget, QHBoxLayout, QStackedLayout, QLabel, QFormLayout, QLineEdit
 
 import numpy as np
 
 
 class InfoWidget(QWidget):
 
     def __init__(self, mainwindow, *args, **kwargs):
```

### Comparing `teda-2.1.0/teda/widgets/radialprofile.py` & `teda-3.0.0/teda/widgets/radialprofile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-import PySide2
-from PySide2.QtWidgets import QWidget, QHBoxLayout
+import PySide6
+from PySide6.QtWidgets import QWidget, QHBoxLayout
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 
 
 class RadialProfileWidget(QWidget):
 
     def __init__(self, data, *args, **kwargs):
@@ -28,20 +28,20 @@
         self.setLayout(figure_layout)
         self.setMinimumHeight(50)
 
         # import matplotlib.pyplot as plt
         # axes = plt.axes()
         # axes.set_ylim([0, 1])
 
-    def showEvent(self, event: PySide2.QtGui.QShowEvent):
+    def showEvent(self, event: PySide6.QtGui.QShowEvent):
         super().showEvent(event)
         # self.turn_on()
         self.invalidate()
 
-    # def hideEvent(self, event: PySide2.QtGui.QHideEvent):
+    # def hideEvent(self, event: PySide6.QtGui.QHideEvent):
     #     super().hideEvent(event)
     #     self.turn_off()
 
     def set_centroid(self, x, y, radius=None):
         self.x = x
         self.y = y
         if radius:
```

### Comparing `teda-2.1.0/teda/widgets/radialprofileIRAF.py` & `teda-3.0.0/teda/widgets/radialprofileIRAF.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide2.QtWidgets import QWidget, QHBoxLayout
+from PySide6.QtWidgets import QWidget, QHBoxLayout
 from matplotlib.figure import Figure, Axes
 import matplotlib.ticker as ticker
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from teda.views.fitsplot import coo_data_to_index, coo_index_to_data
 
 import numpy as np
 import math
```

### Comparing `teda-2.1.0/teda/widgets/scaleWidget.py` & `teda-3.0.0/teda/widgets/scaleWidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PySide2.QtCore import Qt, QSettings, Slot, QSize
-from PySide2.QtWidgets import (QLabel, QSlider, QStackedLayout, QVBoxLayout, QHBoxLayout, QWidget, QGridLayout,
+from PySide6.QtCore import Qt, QSettings, Slot, QSize
+from PySide6.QtWidgets import (QLabel, QSlider, QStackedLayout, QVBoxLayout, QHBoxLayout, QWidget, QGridLayout,
                                QComboBox, QFormLayout, QLineEdit, QSizePolicy, QLayout, QCheckBox)
 from traitlets import TraitError
 from .slider import IntSlider, FloatSlider, LabeledSlider
 
 
 class ScaleWidget(QWidget):
     stretches_list = ['powerdist', 'asinh', 'contrastbias', 'histogram', 'linear',
```

### Comparing `teda-2.1.0/teda/widgets/scanToolbar.py` & `teda-3.0.0/teda/widgets/scanToolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import glob
 import os
 
-from PySide2 import QtCore, QtGui
-from PySide2.QtCore import QObject, QEvent, QSettings
-from PySide2.QtWidgets import QFileDialog, QAction, QApplication, QMessageBox
+from PySide6 import QtCore, QtGui
+from PySide6.QtGui import QAction
+from PySide6.QtCore import QObject, QEvent, QSettings
+from PySide6.QtWidgets import QFileDialog, QApplication, QMessageBox
 import time
 from teda.icons import IconFactory
 import threading
 from traitlets import Float, Int, HasTraits, Bool
 
 
 class ScanToolbar(QObject):
```

### Comparing `teda-2.1.0/teda/widgets/slider.py` & `teda-3.0.0/teda/widgets/slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import PySide2
-from PySide2.QtGui import QDoubleValidator, QIntValidator
-from PySide2.QtCore import Qt, Signal, Slot, QLocale
-from PySide2.QtWidgets import QWidget, QSlider, QHBoxLayout, QLineEdit, QSizePolicy
+import PySide6
+from PySide6.QtGui import QDoubleValidator, QIntValidator
+from PySide6.QtCore import Qt, Signal, Slot, QLocale
+from PySide6.QtWidgets import QWidget, QSlider, QHBoxLayout, QLineEdit, QSizePolicy
 
 
 class LabeledSlider(QWidget):
     slider_min = 0
     slider_max = 64
     slider_step = 1
     line_edit_width = 70
```

### Comparing `teda-2.1.0/teda/widgets/zoomViewWidget.py` & `teda-3.0.0/teda/widgets/zoomViewWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide2.QtWidgets import QWidget, QHBoxLayout
+from PySide6.QtWidgets import QWidget, QHBoxLayout
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from teda.views.fitsplotzoomed import FitsPlotterZoomed
 
 
 class ZoomViewWidget(QWidget):
```

