# Comparing `tmp/teda-3.0.0.tar.gz` & `tmp/teda-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teda-3.0.0.tar", max compression
+gzip compressed data, was "teda-3.0.1.tar", max compression
```

## Comparing `teda-3.0.0.tar` & `teda-3.0.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1066 2020-06-04 16:42:55.000000 teda-3.0.0/LICENSE
--rw-r--r--   0        0        0     4719 2020-12-02 21:00:51.000070 teda-3.0.0/README.md
--rw-r--r--   0        0        0      454 2023-04-28 02:35:30.794102 teda-3.0.0/pyproject.toml
--rw-r--r--   0        0        0       32 2020-06-04 16:24:35.000000 teda-3.0.0/teda/__init__.py
--rw-r--r--   0        0        0     2117 2023-04-28 02:39:09.920354 teda-3.0.0/teda/command_line.py
--rw-r--r--   0        0        0     1958 2020-07-01 12:39:55.000000 teda-3.0.0/teda/console.py
--rw-r--r--   0        0        0     1531 2020-12-03 12:27:12.916427 teda-3.0.0/teda/draggingComponent.py
--rw-r--r--   0        0        0     2105 2020-04-22 14:55:56.000000 teda-3.0.0/teda/fitsopen.py
--rw-r--r--   0        0        0     2043 2020-05-20 13:57:09.000000 teda-3.0.0/teda/fitting.py
--rw-r--r--   0        0        0     2716 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/1-2-24px.svg
--rw-r--r--   0        0        0     2238 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/1-4-24px.svg
--rw-r--r--   0        0        0      298 2020-06-10 13:51:52.000000 teda-3.0.0/teda/icons/add_circle_outline-24px.svg
--rw-r--r--   0        0        0      380 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/autopause-24px.svg
--rw-r--r--   0        0        0      222 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/autopause_disabled-24px.svg
--rw-r--r--   0        0        0      262 2020-06-10 13:51:52.000000 teda-3.0.0/teda/icons/circle-24px.svg
--rw-r--r--   0        0        0      249 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count1-24px.svg
--rw-r--r--   0        0        0      315 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count2-24px.svg
--rw-r--r--   0        0        0      343 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count3-24px.svg
--rw-r--r--   0        0        0      270 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count4-24px.svg
--rw-r--r--   0        0        0      296 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/count5-24px.svg
--rw-r--r--   0        0        0      349 2020-06-10 13:51:52.000000 teda-3.0.0/teda/icons/delete_forever-24px.svg
--rw-r--r--   0        0        0      518 2020-05-14 14:33:36.000000 teda-3.0.0/teda/icons/file-earmark-plus.svg
--rw-r--r--   0        0        0      402 2020-07-01 12:47:01.000000 teda-3.0.0/teda/icons/filter_alt-24px.svg
--rw-r--r--   0        0        0      257 2020-07-01 12:47:01.000000 teda-3.0.0/teda/icons/folder-24px.svg
--rw-r--r--   0        0        0      217 2020-06-08 17:33:08.000000 teda-3.0.0/teda/icons/home-24px.svg
--rw-r--r--   0        0        0      343 2020-06-08 17:32:29.000000 teda-3.0.0/teda/icons/house-24px.svg
--rw-r--r--   0        0        0      196 2020-06-08 17:30:35.000000 teda-3.0.0/teda/icons/keyboard_arrow_left-24px.svg
--rw-r--r--   0        0        0      194 2020-06-08 17:30:21.000000 teda-3.0.0/teda/icons/keyboard_arrow_right-24px.svg
--rw-r--r--   0        0        0      977 2020-06-05 15:03:11.000000 teda-3.0.0/teda/icons/new.png
--rw-r--r--   0        0        0      367 2020-06-10 13:51:52.000000 teda-3.0.0/teda/icons/not_started-24px.svg
--rw-r--r--   0        0        0      261 2020-06-08 17:13:41.000000 teda-3.0.0/teda/icons/note_add-24px.svg
--rw-r--r--   0        0        0      245 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/panning-24px.svg
--rw-r--r--   0        0        0      292 2020-06-08 17:34:43.000000 teda-3.0.0/teda/icons/pause_circle_outline-24px.svg
--rw-r--r--   0        0        0      344 2020-07-01 12:47:01.000000 teda-3.0.0/teda/icons/photo_filter-24px.svg
--rw-r--r--   0        0        0      285 2020-06-08 17:34:37.000000 teda-3.0.0/teda/icons/play_circle_outline-24px.svg
--rw-r--r--   0        0        0      379 2020-07-01 12:39:55.000000 teda-3.0.0/teda/icons/push_pin-24px.svg
--rw-r--r--   0        0        0      304 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/save-24px.svg
--rw-r--r--   0        0        0      203 2020-06-08 17:29:29.000000 teda-3.0.0/teda/icons/skip_next-24px.svg
--rw-r--r--   0        0        0      206 2020-06-08 17:29:33.000000 teda-3.0.0/teda/icons/skip_previous-24px.svg
--rw-r--r--   0        0        0     1245 2020-12-03 12:27:12.917053 teda-3.0.0/teda/icons/slider-24px.svg
--rw-r--r--   0        0        0      385 2020-06-08 17:34:40.000000 teda-3.0.0/teda/icons/stop_circle-24px.svg
--rw-r--r--   0        0        0     2638 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/x2-24px.svg
--rw-r--r--   0        0        0     2159 2020-07-01 13:22:36.000000 teda-3.0.0/teda/icons/x4-24px.svg
--rw-r--r--   0        0        0      571 2023-04-28 02:39:09.916622 teda-3.0.0/teda/icons.py
--rw-r--r--   0        0        0        0 2020-06-04 14:08:12.000000 teda-3.0.0/teda/models/__init__.py
--rw-r--r--   0        0        0     1014 2020-06-04 10:29:56.000000 teda-3.0.0/teda/models/cmaps.py
--rw-r--r--   0        0        0     2920 2020-12-03 12:21:15.954502 teda-3.0.0/teda/models/coordinates.py
--rw-r--r--   0        0        0     5435 2020-12-02 21:00:51.002196 teda-3.0.0/teda/models/scalesModel.py
--rw-r--r--   0        0        0    16439 2023-04-28 03:24:57.907274 teda-3.0.0/teda/painterComponent.py
--rw-r--r--   0        0        0     2967 2023-04-28 02:39:09.864767 teda-3.0.0/teda/painterShapes/CircleCenterShape.py
--rw-r--r--   0        0        0        0 2020-06-04 11:27:56.000000 teda-3.0.0/teda/painterShapes/__init__.py
--rw-r--r--   0        0        0     1885 2023-04-28 02:39:09.885266 teda-3.0.0/teda/painterShapes/circleShape.py
--rw-r--r--   0        0        0     2227 2023-04-28 02:39:09.889630 teda-3.0.0/teda/painterShapes/rectangleMinatureShape.py
--rwxr-xr-x   0        0        0     1410 2023-04-28 02:57:03.732713 teda-3.0.0/teda/teda_fits.py
--rw-r--r--   0        0        0      123 2023-04-28 02:20:49.771269 teda-3.0.0/teda/version.py
--rw-r--r--   0        0        0    34219 2023-04-28 02:50:04.151992 teda-3.0.0/teda/viewer_mainwindow.py
--rw-r--r--   0        0        0        0 2020-06-04 14:07:28.000000 teda-3.0.0/teda/views/__init__.py
--rw-r--r--   0        0        0    17605 2023-04-28 03:13:13.702006 teda-3.0.0/teda/views/fitsplot.py
--rw-r--r--   0        0        0     2602 2020-12-03 12:21:15.958669 teda-3.0.0/teda/views/fitsplot_fitsfile.py
--rw-r--r--   0        0        0     2498 2020-12-02 21:00:51.007550 teda-3.0.0/teda/views/fitsplotcontrolled.py
--rw-r--r--   0        0        0     1143 2020-06-04 11:45:26.000000 teda-3.0.0/teda/views/fitsplotzoomed.py
--rw-r--r--   0        0        0        0 2020-06-04 14:10:29.000000 teda-3.0.0/teda/widgets/__init__.py
--rw-r--r--   0        0        0     6563 2023-04-28 02:49:22.960395 teda-3.0.0/teda/widgets/fileSystemWidget.py
--rw-r--r--   0        0        0     2976 2023-04-28 02:39:09.907291 teda-3.0.0/teda/widgets/fullViewWidget.py
--rw-r--r--   0        0        0     3270 2023-04-28 02:39:09.874014 teda-3.0.0/teda/widgets/headerTableWidget.py
--rw-r--r--   0        0        0     2295 2023-04-28 02:39:09.924105 teda-3.0.0/teda/widgets/info.py
--rw-r--r--   0        0        0     3293 2023-04-28 02:39:09.869422 teda-3.0.0/teda/widgets/radialprofile.py
--rw-r--r--   0        0        0     5299 2023-04-28 02:39:09.899380 teda-3.0.0/teda/widgets/radialprofileIRAF.py
--rw-r--r--   0        0        0    24112 2023-04-28 02:39:09.928943 teda-3.0.0/teda/widgets/scaleWidget.py
--rw-r--r--   0        0        0    12534 2023-04-28 02:48:42.836537 teda-3.0.0/teda/widgets/scanToolbar.py
--rw-r--r--   0        0        0     6207 2023-04-28 02:39:09.903950 teda-3.0.0/teda/widgets/slider.py
--rw-r--r--   0        0        0     1357 2023-04-28 02:39:09.895011 teda-3.0.0/teda/widgets/zoomViewWidget.py
--rw-r--r--   0        0        0    49708 1970-01-01 00:00:00.000000 teda-3.0.0/setup.py
--rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 teda-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2020-06-04 16:42:55.000000 teda-3.0.1/LICENSE
+-rw-r--r--   0        0        0     4719 2020-12-02 21:00:51.000070 teda-3.0.1/README.md
+-rw-r--r--   0        0        0      454 2023-04-28 04:12:41.900417 teda-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0       32 2020-06-04 16:24:35.000000 teda-3.0.1/teda/__init__.py
+-rw-r--r--   0        0        0     2117 2023-04-28 02:39:09.920354 teda-3.0.1/teda/command_line.py
+-rw-r--r--   0        0        0     1958 2020-07-01 12:39:55.000000 teda-3.0.1/teda/console.py
+-rw-r--r--   0        0        0     1531 2020-12-03 12:27:12.916427 teda-3.0.1/teda/draggingComponent.py
+-rw-r--r--   0        0        0     2105 2020-04-22 14:55:56.000000 teda-3.0.1/teda/fitsopen.py
+-rw-r--r--   0        0        0     2043 2020-05-20 13:57:09.000000 teda-3.0.1/teda/fitting.py
+-rw-r--r--   0        0        0     2716 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/1-2-24px.svg
+-rw-r--r--   0        0        0     2238 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/1-4-24px.svg
+-rw-r--r--   0        0        0      298 2020-06-10 13:51:52.000000 teda-3.0.1/teda/icons/add_circle_outline-24px.svg
+-rw-r--r--   0        0        0      380 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/autopause-24px.svg
+-rw-r--r--   0        0        0      222 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/autopause_disabled-24px.svg
+-rw-r--r--   0        0        0      262 2020-06-10 13:51:52.000000 teda-3.0.1/teda/icons/circle-24px.svg
+-rw-r--r--   0        0        0      249 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/count1-24px.svg
+-rw-r--r--   0        0        0      315 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/count2-24px.svg
+-rw-r--r--   0        0        0      343 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/count3-24px.svg
+-rw-r--r--   0        0        0      270 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/count4-24px.svg
+-rw-r--r--   0        0        0      296 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/count5-24px.svg
+-rw-r--r--   0        0        0      349 2020-06-10 13:51:52.000000 teda-3.0.1/teda/icons/delete_forever-24px.svg
+-rw-r--r--   0        0        0      518 2020-05-14 14:33:36.000000 teda-3.0.1/teda/icons/file-earmark-plus.svg
+-rw-r--r--   0        0        0      402 2020-07-01 12:47:01.000000 teda-3.0.1/teda/icons/filter_alt-24px.svg
+-rw-r--r--   0        0        0      257 2020-07-01 12:47:01.000000 teda-3.0.1/teda/icons/folder-24px.svg
+-rw-r--r--   0        0        0      217 2020-06-08 17:33:08.000000 teda-3.0.1/teda/icons/home-24px.svg
+-rw-r--r--   0        0        0      343 2020-06-08 17:32:29.000000 teda-3.0.1/teda/icons/house-24px.svg
+-rw-r--r--   0        0        0      196 2020-06-08 17:30:35.000000 teda-3.0.1/teda/icons/keyboard_arrow_left-24px.svg
+-rw-r--r--   0        0        0      194 2020-06-08 17:30:21.000000 teda-3.0.1/teda/icons/keyboard_arrow_right-24px.svg
+-rw-r--r--   0        0        0      977 2020-06-05 15:03:11.000000 teda-3.0.1/teda/icons/new.png
+-rw-r--r--   0        0        0      367 2020-06-10 13:51:52.000000 teda-3.0.1/teda/icons/not_started-24px.svg
+-rw-r--r--   0        0        0      261 2020-06-08 17:13:41.000000 teda-3.0.1/teda/icons/note_add-24px.svg
+-rw-r--r--   0        0        0      245 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/panning-24px.svg
+-rw-r--r--   0        0        0      292 2020-06-08 17:34:43.000000 teda-3.0.1/teda/icons/pause_circle_outline-24px.svg
+-rw-r--r--   0        0        0      344 2020-07-01 12:47:01.000000 teda-3.0.1/teda/icons/photo_filter-24px.svg
+-rw-r--r--   0        0        0      285 2020-06-08 17:34:37.000000 teda-3.0.1/teda/icons/play_circle_outline-24px.svg
+-rw-r--r--   0        0        0      379 2020-07-01 12:39:55.000000 teda-3.0.1/teda/icons/push_pin-24px.svg
+-rw-r--r--   0        0        0      304 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/save-24px.svg
+-rw-r--r--   0        0        0      203 2020-06-08 17:29:29.000000 teda-3.0.1/teda/icons/skip_next-24px.svg
+-rw-r--r--   0        0        0      206 2020-06-08 17:29:33.000000 teda-3.0.1/teda/icons/skip_previous-24px.svg
+-rw-r--r--   0        0        0     1245 2020-12-03 12:27:12.917053 teda-3.0.1/teda/icons/slider-24px.svg
+-rw-r--r--   0        0        0      385 2020-06-08 17:34:40.000000 teda-3.0.1/teda/icons/stop_circle-24px.svg
+-rw-r--r--   0        0        0     2638 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/x2-24px.svg
+-rw-r--r--   0        0        0     2159 2020-07-01 13:22:36.000000 teda-3.0.1/teda/icons/x4-24px.svg
+-rw-r--r--   0        0        0      571 2023-04-28 02:39:09.916622 teda-3.0.1/teda/icons.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:08:12.000000 teda-3.0.1/teda/models/__init__.py
+-rw-r--r--   0        0        0     1014 2020-06-04 10:29:56.000000 teda-3.0.1/teda/models/cmaps.py
+-rw-r--r--   0        0        0     3002 2023-04-28 04:32:12.682801 teda-3.0.1/teda/models/coordinates.py
+-rw-r--r--   0        0        0     5435 2020-12-02 21:00:51.002196 teda-3.0.1/teda/models/scalesModel.py
+-rw-r--r--   0        0        0    16439 2023-04-28 03:24:57.907274 teda-3.0.1/teda/painterComponent.py
+-rw-r--r--   0        0        0     2967 2023-04-28 02:39:09.864767 teda-3.0.1/teda/painterShapes/CircleCenterShape.py
+-rw-r--r--   0        0        0        0 2020-06-04 11:27:56.000000 teda-3.0.1/teda/painterShapes/__init__.py
+-rw-r--r--   0        0        0     1885 2023-04-28 02:39:09.885266 teda-3.0.1/teda/painterShapes/circleShape.py
+-rw-r--r--   0        0        0     2227 2023-04-28 02:39:09.889630 teda-3.0.1/teda/painterShapes/rectangleMinatureShape.py
+-rwxr-xr-x   0        0        0     1410 2023-04-28 02:57:03.732713 teda-3.0.1/teda/teda_fits.py
+-rw-r--r--   0        0        0      123 2023-04-28 04:12:31.907290 teda-3.0.1/teda/version.py
+-rw-r--r--   0        0        0    34219 2023-04-28 02:50:04.151992 teda-3.0.1/teda/viewer_mainwindow.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:07:28.000000 teda-3.0.1/teda/views/__init__.py
+-rw-r--r--   0        0        0    17605 2023-04-28 03:13:13.702006 teda-3.0.1/teda/views/fitsplot.py
+-rw-r--r--   0        0        0     2602 2020-12-03 12:21:15.958669 teda-3.0.1/teda/views/fitsplot_fitsfile.py
+-rw-r--r--   0        0        0     2498 2020-12-02 21:00:51.007550 teda-3.0.1/teda/views/fitsplotcontrolled.py
+-rw-r--r--   0        0        0     1143 2020-06-04 11:45:26.000000 teda-3.0.1/teda/views/fitsplotzoomed.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:10:29.000000 teda-3.0.1/teda/widgets/__init__.py
+-rw-r--r--   0        0        0     6563 2023-04-28 02:49:22.960395 teda-3.0.1/teda/widgets/fileSystemWidget.py
+-rw-r--r--   0        0        0     2976 2023-04-28 02:39:09.907291 teda-3.0.1/teda/widgets/fullViewWidget.py
+-rw-r--r--   0        0        0     3270 2023-04-28 02:39:09.874014 teda-3.0.1/teda/widgets/headerTableWidget.py
+-rw-r--r--   0        0        0     2295 2023-04-28 02:39:09.924105 teda-3.0.1/teda/widgets/info.py
+-rw-r--r--   0        0        0     3293 2023-04-28 02:39:09.869422 teda-3.0.1/teda/widgets/radialprofile.py
+-rw-r--r--   0        0        0     5299 2023-04-28 02:39:09.899380 teda-3.0.1/teda/widgets/radialprofileIRAF.py
+-rw-r--r--   0        0        0    24353 2023-04-28 04:12:12.833462 teda-3.0.1/teda/widgets/scaleWidget.py
+-rw-r--r--   0        0        0    12534 2023-04-28 02:48:42.836537 teda-3.0.1/teda/widgets/scanToolbar.py
+-rw-r--r--   0        0        0     6207 2023-04-28 02:39:09.903950 teda-3.0.1/teda/widgets/slider.py
+-rw-r--r--   0        0        0     1357 2023-04-28 02:39:09.895011 teda-3.0.1/teda/widgets/zoomViewWidget.py
+-rw-r--r--   0        0        0    49708 1970-01-01 00:00:00.000000 teda-3.0.1/setup.py
+-rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 teda-3.0.1/PKG-INFO
```

### Comparing `teda-3.0.0/LICENSE` & `teda-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/README.md` & `teda-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/command_line.py` & `teda-3.0.1/teda/command_line.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/console.py` & `teda-3.0.1/teda/console.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/draggingComponent.py` & `teda-3.0.1/teda/draggingComponent.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/fitsopen.py` & `teda-3.0.1/teda/fitsopen.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/fitting.py` & `teda-3.0.1/teda/fitting.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/icons/1-2-24px.svg` & `teda-3.0.1/teda/icons/1-2-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/icons/1-4-24px.svg` & `teda-3.0.1/teda/icons/1-4-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/icons/file-earmark-plus.svg` & `teda-3.0.1/teda/icons/file-earmark-plus.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/icons/new.png` & `teda-3.0.1/teda/icons/new.png`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/icons/slider-24px.svg` & `teda-3.0.1/teda/icons/slider-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/icons/x2-24px.svg` & `teda-3.0.1/teda/icons/x2-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/icons/x4-24px.svg` & `teda-3.0.1/teda/icons/x4-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/icons.py` & `teda-3.0.1/teda/icons.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/models/cmaps.py` & `teda-3.0.1/teda/models/cmaps.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/models/coordinates.py` & `teda-3.0.1/teda/models/coordinates.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,13 +76,15 @@
     def set_img_y(self, y):
         self.img_y = y
         self.calc_wcs()
         self.img_versionno += 1
 
     def format_wcs(self):
         if self.wcs_coo is not None:
-            fmt = 'hmsdms' if self.wcs_sexagesimal else 'decimal'
-            self.wcs_formatted = self.wcs_coo.to_string(fmt, sep=':', precision=3)
+            if self.wcs_sexagesimal:
+                self.wcs_formatted = self.wcs_coo.to_string('hmsdms', sep=':', precision=3)
+            else:
+                self.wcs_formatted = self.wcs_coo.to_string('decimal', precision=3)
             self.wcs_framename = self.wcs_coo.name
         else:
             self.wcs_formatted = ''
             self.wcs_framename = 'WCS'
```

### Comparing `teda-3.0.0/teda/models/scalesModel.py` & `teda-3.0.1/teda/models/scalesModel.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/painterComponent.py` & `teda-3.0.1/teda/painterComponent.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/painterShapes/CircleCenterShape.py` & `teda-3.0.1/teda/painterShapes/CircleCenterShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/painterShapes/circleShape.py` & `teda-3.0.1/teda/painterShapes/circleShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/painterShapes/rectangleMinatureShape.py` & `teda-3.0.1/teda/painterShapes/rectangleMinatureShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/teda_fits.py` & `teda-3.0.1/teda/teda_fits.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/viewer_mainwindow.py` & `teda-3.0.1/teda/viewer_mainwindow.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/views/fitsplot.py` & `teda-3.0.1/teda/views/fitsplot.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/views/fitsplot_fitsfile.py` & `teda-3.0.1/teda/views/fitsplot_fitsfile.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/views/fitsplotcontrolled.py` & `teda-3.0.1/teda/views/fitsplotcontrolled.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/views/fitsplotzoomed.py` & `teda-3.0.1/teda/views/fitsplotzoomed.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/fileSystemWidget.py` & `teda-3.0.1/teda/widgets/fileSystemWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/fullViewWidget.py` & `teda-3.0.1/teda/widgets/fullViewWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/headerTableWidget.py` & `teda-3.0.1/teda/widgets/headerTableWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/info.py` & `teda-3.0.1/teda/widgets/info.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/radialprofile.py` & `teda-3.0.1/teda/widgets/radialprofile.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/radialprofileIRAF.py` & `teda-3.0.1/teda/widgets/radialprofileIRAF.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/scaleWidget.py` & `teda-3.0.1/teda/widgets/scaleWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -467,45 +467,48 @@
         settings.setValue("interval", self.scalesModel.selected_interval)
 
         # settings.setValue("cmap", self.color_combobox.currentIndex())
 
         settings.endGroup()
 
     def readSlidersValues(self):
+        float_none = lambda x: float(x) if x is not None else None
+        int_none = lambda x: int(x) if x is not None else None
+
         settings = QSettings()
         settings.beginGroup("Sliders")
 
         self.setModelValue('cmap_idx', settings.value("cmap"), model=self.cmapModel)
         self.setModelValue('selected_stretch', settings.value("stretch"))
         self.setModelValue('selected_interval', settings.value("interval"))
         # self.color_combobox.setCurrentIndex(settings.value("cmap", 3))
 
-        self.setModelValue('stretch_asinh_a', float(settings.value('asinh/a')))
-        self.setModelValue('stretch_contrastbias_contrast', float(settings.value('contrast/contrast')))
-        self.setModelValue('stretch_contrastbias_bias', float(settings.value('contrast/bias')))
-        self.setModelValue('stretch_linear_slope', float(settings.value('linear/slope')))
-        self.setModelValue('stretch_linear_intercept', float(settings.value('linear/intercept')))
-        self.setModelValue('stretch_log_a', float(settings.value('log/a')))
-        self.setModelValue('stretch_powerdist_a', float(settings.value('powerdist/a')))
-        self.setModelValue('stretch_power_a', float(settings.value('power/a')))
-        self.setModelValue('stretch_sinh_a', float(settings.value('sinh/a')))
-
-        self.setModelValue('interval_manual_vmin', float(settings.value('manual/vmin')))
-        self.setModelValue('interval_manual_vmax', int(settings.value('manual/vmax')))
-        self.setModelValue('interval_percentile_percentile', float(settings.value('percentile/percentile')))
-        self.setModelValue('interval_percentile_nsamples', int(settings.value('percentile/nsamples')))
-        self.setModelValue('interval_asymetric_lower_percentile', float(settings.value('asymetric/lpercentile')))
-        self.setModelValue('interval_asymetric_upper_percentile', float(settings.value('asymetric/upercentile')))
-        self.setModelValue('interval_asymetric_nsamples', int(settings.value('asymetric/nsamples')))
-        self.setModelValue('interval_zscale_nsamples', int(settings.value('zscale/nsamples')))
-        self.setModelValue('interval_zscale_contrast', float(settings.value('zscale/contrast')))
-        self.setModelValue('interval_zscale_maxreject', float(settings.value('zscale/maxreject')))
-        self.setModelValue('interval_zscale_minpixels', int(settings.value('zscale/minpixels')))
-        self.setModelValue('interval_zscale_krej', float(settings.value('zscale/krej')))
-        self.setModelValue('interval_zscale_maxiterations', int(settings.value('zscale/maxiterations')))
+        self.setModelValue('stretch_asinh_a', float_none(settings.value('asinh/a')))
+        self.setModelValue('stretch_contrastbias_contrast', float_none(settings.value('contrast/contrast')))
+        self.setModelValue('stretch_contrastbias_bias', float_none(settings.value('contrast/bias')))
+        self.setModelValue('stretch_linear_slope', float_none(settings.value('linear/slope')))
+        self.setModelValue('stretch_linear_intercept', float_none(settings.value('linear/intercept')))
+        self.setModelValue('stretch_log_a', float_none(settings.value('log/a')))
+        self.setModelValue('stretch_powerdist_a', float_none(settings.value('powerdist/a')))
+        self.setModelValue('stretch_power_a', float_none(settings.value('power/a')))
+        self.setModelValue('stretch_sinh_a', float_none(settings.value('sinh/a')))
+
+        self.setModelValue('interval_manual_vmin', float_none(settings.value('manual/vmin')))
+        self.setModelValue('interval_manual_vmax', int_none(settings.value('manual/vmax')))
+        self.setModelValue('interval_percentile_percentile', float_none(settings.value('percentile/percentile')))
+        self.setModelValue('interval_percentile_nsamples', int_none(settings.value('percentile/nsamples')))
+        self.setModelValue('interval_asymetric_lower_percentile', float_none(settings.value('asymetric/lpercentile')))
+        self.setModelValue('interval_asymetric_upper_percentile', float_none(settings.value('asymetric/upercentile')))
+        self.setModelValue('interval_asymetric_nsamples', int_none(settings.value('asymetric/nsamples')))
+        self.setModelValue('interval_zscale_nsamples', int_none(settings.value('zscale/nsamples')))
+        self.setModelValue('interval_zscale_contrast', float_none(settings.value('zscale/contrast')))
+        self.setModelValue('interval_zscale_maxreject', float_none(settings.value('zscale/maxreject')))
+        self.setModelValue('interval_zscale_minpixels', int_none(settings.value('zscale/minpixels')))
+        self.setModelValue('interval_zscale_krej', float_none(settings.value('zscale/krej')))
+        self.setModelValue('interval_zscale_maxiterations', int_none(settings.value('zscale/maxiterations')))
         settings.endGroup()
 
     def setModelValue(self, model_key, value, model=None):
         if model is None:
             model = self.scalesModel
         try:
             setattr(model, model_key, value)
```

### Comparing `teda-3.0.0/teda/widgets/scanToolbar.py` & `teda-3.0.1/teda/widgets/scanToolbar.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/slider.py` & `teda-3.0.1/teda/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/teda/widgets/zoomViewWidget.py` & `teda-3.0.1/teda/widgets/zoomViewWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.0/setup.py` & `teda-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1171,15 +1171,15 @@
  'traitlets>=5.9.0,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['teda = teda.teda_fits:main']}
 
 setup_kwargs = {
     'name': 'teda',
-    'version': '3.0.0',
+    'version': '3.0.1',
     'description': 'Yet Another FITS Viewer',
     'long_description': '# TeDa FITS Viewer\n\nObservatory optimized FITS Images viewer\n\n![](img/teda.png)\n\n## Key Features\n* Flexible windows and widgets layout\n* WCS support\n* Radial Profile with gaussoide fit (try `r`-key)\n* Scan mode: observes directory for changes and automatically opens new FITS\n* Integrated ipython console with direct access to data and application\n\n## Installation\n``` bash\n   pip install teda\n   teda_viewer \n``` \n### Optional dependencies\nTo use ipython console the `qtconsole` package is needed, additionally:\n``` bash\n    pip install qtconsole\n``` \nFor directory scanning functionality, the `watchdog` package should be installed, e.g. \n``` bash\n    pip install watchdog\n``` \n\n## Run\nThe installation scripts should install the command:\n```\n    teda_viewer\n```\nTry \n```\n    teda_viewer --help\n```\nfor list of command line parameters.\n\n## Dynamic Scale and Color\nThe dynamic scale of the image, and color mapping can be adjusted form \nthe **Dynamic Scale** panel. From menu: **View/Dynamic Scale**\n\n## Fits Header Cards Pinning\nOn the FITS Header panel, selected keys can be *pinned* to appear\non the top ot the list. This can be done via context (right-click) menu.\n\nThe set of pinned keys is saved and preserved between sessions.  \n\n## Radial Profile\nThe **Radial Profile** button turns on the mode of selecting targets for \nthe radial profile analysis. Make sure the radial profile panel is visible \n(View/Radial Profile). The shortcut for displaying radial profile of the star \nunder cursor is the **R**-key.\n\nThe centroid of the star is corrected within small (be precise!) radius\nusing the bivariate gaussoide fit.\n\nTogether with the pixels values, the radial profile presents 1D fit of\n"gaussian(r) + sky". This fit provides information of presented fwhm and sky level.\n   \n\n## Integrated Python Console\nIn order to use integrated python console the `qtconsole` module, and it\'s\ndependencies (jupyter related) have to be installed. This is not done by\ndefault `pip` installation to keep number of dependencies reasonably small.\nInstall `qtconsole` by:\n``` bash\n    pip install qtconsole\n``` \n\nThe console is available form menu **View/Python Console**\n### Predefined variables\nThe console has a number of predefined variables set:\n* `ax: WCSAxesSubplot` main plotting axes.\n* `window: MainWindow` main window\n* `data: numpy.ndarray` current HDU data\n* `header: astropy.fits.Header` current HDU header\n* `wcs: astropy.wcs.WCS` the WCS transformer\n\n### Plotting\nTo plot directly on the console, run the following magic command `%matplotlib inline`.\n\nWhen plotting on the main canvas, the result will appear after redrawing\nmain figure by `ax.figure.canvas.draw()`.\n\nThe example below, draws linear profile on the console and corresponding\nline on the main FITS display:    \n  \n``` python\n%matplotlib inline\nimport matplotlib.pyplot as plt\nax.plot([10,30], [10,10])\nax.figure.canvas.draw()\nplt.plot(data[10,10:30])\n```\n\n## Directory Scan\nThe **Scan Toolbar** (hidden by default) provides controls for the \ndirectory scanning mode.\n\nThis mode is intended to observe newly created FITS files in observatory.\n\nAfter pressing **Scan** button, and choosing directory, TeDa Fits Viewer will\nload most recent FITS file from that directory, and keep watching the directory \nfor changes. When new FITS file is added to directory, it will be loaded \nautomatically.\n\nUser can pause scanning using **Pause** button. There is also **auto pause** feature,\nwhen active, any mouse movement in the main area pauses scanning for 5 seconds,\navoiding FITS reload when working.\n\nAfter un-pausing (manually or after idle 5 seconds when auto-pause) the newest\nFITS will be loaded if any new files appeared during the pause.\n\nDirectory scanning needs the [`watchdog`](https://pypi.org/project/watchdog/) component to be \ninstalled manually (optional dependence).\n\n## Directory Panel\nThe Directory Panel can be shown using menu command **View-Directory view**.\n\nThe Directory Panel is convenient files navigator. The panel has two views:\n* Directory Tree\n* Files List\n\nUser can collapse any of them using divider handle and use only remaining one.\nIf the tree view is the only visible, it shows directories and files as well.      \n\n## Development version install\n``` bash\n\n    git clone https://github.com/majkelx/teda.git\n    cd teda\n    python -m venv venv\n    source ./venv/bin/activate\n    pip install -r requirements.txt\n    pip install -e .\n```\n\n## Bugs, remarks, greetings and contribution \nPlease use [GitHub issues tracker](https://github.com/majkelx/teda/issues) \nand [pull requests](https://github.com/majkelx/teda/pulls).\n\n\n@2020  [AkondLab](http://www.akond.com) for the [Araucaria Project](https://araucaria.camk.edu.pl).\n',
     'author': 'majkelx',
     'author_email': 'mkalusz@camk.edu.pl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `teda-3.0.0/PKG-INFO` & `teda-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teda
-Version: 3.0.0
+Version: 3.0.1
 Summary: Yet Another FITS Viewer
 License: MIT
 Author: majkelx
 Author-email: mkalusz@camk.edu.pl
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

