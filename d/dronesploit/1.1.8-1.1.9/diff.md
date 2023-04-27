# Comparing `tmp/dronesploit-1.1.8.tar.gz` & `tmp/dronesploit-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronesploit-1.1.8.tar", last modified: Sat Feb 26 17:29:56 2022, max compression
+gzip compressed data, was "dronesploit-1.1.9.tar", last modified: Sun Feb 27 10:33:17 2022, max compression
```

## Comparing `dronesploit-1.1.8.tar` & `dronesploit-1.1.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.846593 dronesploit-1.1.8/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    35186 2021-02-15 20:28:15.000000 dronesploit-1.1.8/LICENSE
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     4736 2022-02-26 17:29:56.846593 dronesploit-1.1.8/PKG-INFO
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     3912 2022-02-08 10:48:05.000000 dronesploit-1.1.8/README.md
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)        7 2022-02-26 17:29:43.000000 dronesploit-1.1.8/dronesploit/VERSION.txt
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      344 2022-02-07 07:38:20.000000 dronesploit-1.1.8/dronesploit/__info__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     2333 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      832 2021-05-31 21:10:38.000000 dronesploit-1.1.8/dronesploit/__main__.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/banners/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2041 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/banners/banner1.asc
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1387 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/banners/banner2.asc
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     2094 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/banners/banner3.asc
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1871 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/banners/banner4.asc
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1608 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/banners/banner5.asc
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1385 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/banners/banner6.asc
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/commands/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      864 2021-02-18 18:32:12.000000 dronesploit-1.1.8/dronesploit/_src/commands/generic.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     6763 2021-02-18 18:24:39.000000 dronesploit-1.1.8/dronesploit/_src/commands/wifi.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/modules/
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/wifi/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3570 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/wifi/crack.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1932 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/wifi/deauth.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1046 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/wifi/sniff.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      167 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/wifi/wordlist.txt
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/modules/command/
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/modules/command/dji/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2194 2021-02-18 14:34:51.000000 dronesploit-1.1.8/dronesploit/_src/modules/command/dji/tello.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/modules/command/hobicco/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2432 2021-02-18 14:31:41.000000 dronesploit-1.1.8/dronesploit/_src/modules/command/hobicco/cme.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2048 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/modules/command/hobicco/flitt.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/modules/exploit/
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit/_src/modules/exploit/hobbico/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      680 2021-02-15 20:28:15.000000 dronesploit-1.1.8/dronesploit/_src/modules/exploit/hobbico/cme.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      760 2021-02-18 12:29:12.000000 dronesploit-1.1.8/dronesploit/_src/modules/exploit/hobbico/flitt.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.846593 dronesploit-1.1.8/dronesploit/drones/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4575 2021-02-18 12:54:54.000000 dronesploit-1.1.8/dronesploit/drones/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2635 2021-02-18 14:33:23.000000 dronesploit-1.1.8/dronesploit/drones/dji.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4659 2021-02-18 12:42:02.000000 dronesploit-1.1.8/dronesploit/drones/hobbico.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.846593 dronesploit-1.1.8/dronesploit/generic/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      169 2021-02-18 12:28:54.000000 dronesploit-1.1.8/dronesploit/generic/__init__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     4199 2021-02-18 18:30:59.000000 dronesploit-1.1.8/dronesploit/generic/decorators.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      985 2021-05-07 17:40:47.000000 dronesploit-1.1.8/dronesploit/generic/mixins.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.846593 dronesploit-1.1.8/dronesploit/wifi/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2029 2021-02-18 18:30:04.000000 dronesploit-1.1.8/dronesploit/wifi/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1056 2022-02-26 17:27:37.000000 dronesploit-1.1.8/dronesploit/wifi/drone.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     7838 2021-02-18 14:39:20.000000 dronesploit-1.1.8/dronesploit/wifi/mixin.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-26 17:29:56.842593 dronesploit-1.1.8/dronesploit.egg-info/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     4736 2022-02-26 17:29:56.000000 dronesploit-1.1.8/dronesploit.egg-info/PKG-INFO
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1344 2022-02-26 17:29:56.000000 dronesploit-1.1.8/dronesploit.egg-info/SOURCES.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        1 2022-02-26 17:29:56.000000 dronesploit-1.1.8/dronesploit.egg-info/dependency_links.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       59 2022-02-26 17:29:56.000000 dronesploit-1.1.8/dronesploit.egg-info/entry_points.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       17 2022-02-26 17:29:56.000000 dronesploit-1.1.8/dronesploit.egg-info/requires.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       12 2022-02-26 17:29:56.000000 dronesploit-1.1.8/dronesploit.egg-info/top_level.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1114 2022-02-26 17:29:56.846593 dronesploit-1.1.8/setup.cfg
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      383 2021-02-15 20:28:15.000000 dronesploit-1.1.8/setup.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.702025 dronesploit-1.1.9/
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)    35186 2021-02-15 20:28:15.000000 dronesploit-1.1.9/LICENSE
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     4736 2022-02-27 10:33:17.702025 dronesploit-1.1.9/PKG-INFO
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     3912 2022-02-08 10:48:05.000000 dronesploit-1.1.9/README.md
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)        7 2022-02-27 10:32:01.000000 dronesploit-1.1.9/dronesploit/VERSION.txt
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      344 2022-02-07 07:38:20.000000 dronesploit-1.1.9/dronesploit/__info__.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     2333 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      832 2021-05-31 21:10:38.000000 dronesploit-1.1.9/dronesploit/__main__.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.694025 dronesploit-1.1.9/dronesploit/_src/
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/_src/banners/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2041 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/banners/banner1.asc
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     1387 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/banners/banner2.asc
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     2094 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/banners/banner3.asc
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     1871 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/banners/banner4.asc
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     1608 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/banners/banner5.asc
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     1385 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/banners/banner6.asc
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/_src/commands/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      864 2021-02-18 18:32:12.000000 dronesploit-1.1.9/dronesploit/_src/commands/generic.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     6763 2021-02-18 18:24:39.000000 dronesploit-1.1.9/dronesploit/_src/commands/wifi.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.694025 dronesploit-1.1.9/dronesploit/_src/modules/
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.694025 dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/wifi/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3570 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/wifi/crack.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1932 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/wifi/deauth.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1046 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/wifi/sniff.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      167 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/wifi/wordlist.txt
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.694025 dronesploit-1.1.9/dronesploit/_src/modules/command/
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/_src/modules/command/dji/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2194 2021-02-18 14:34:51.000000 dronesploit-1.1.9/dronesploit/_src/modules/command/dji/tello.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/_src/modules/command/hobicco/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2432 2021-02-18 14:31:41.000000 dronesploit-1.1.9/dronesploit/_src/modules/command/hobicco/cme.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2048 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/modules/command/hobicco/flitt.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.694025 dronesploit-1.1.9/dronesploit/_src/modules/exploit/
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/_src/modules/exploit/hobbico/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      680 2021-02-15 20:28:15.000000 dronesploit-1.1.9/dronesploit/_src/modules/exploit/hobbico/cme.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      760 2021-02-18 12:29:12.000000 dronesploit-1.1.9/dronesploit/_src/modules/exploit/hobbico/flitt.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/drones/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4575 2021-02-18 12:54:54.000000 dronesploit-1.1.9/dronesploit/drones/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2635 2021-02-18 14:33:23.000000 dronesploit-1.1.9/dronesploit/drones/dji.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4659 2021-02-18 12:42:02.000000 dronesploit-1.1.9/dronesploit/drones/hobbico.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit/generic/
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)      169 2021-02-18 12:28:54.000000 dronesploit-1.1.9/dronesploit/generic/__init__.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     4199 2021-02-18 18:30:59.000000 dronesploit-1.1.9/dronesploit/generic/decorators.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)      985 2021-05-07 17:40:47.000000 dronesploit-1.1.9/dronesploit/generic/mixins.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.702025 dronesploit-1.1.9/dronesploit/wifi/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2029 2021-02-18 18:30:04.000000 dronesploit-1.1.9/dronesploit/wifi/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1056 2022-02-26 17:27:37.000000 dronesploit-1.1.9/dronesploit/wifi/drone.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     7838 2021-02-18 14:39:20.000000 dronesploit-1.1.9/dronesploit/wifi/mixin.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-02-27 10:33:17.698025 dronesploit-1.1.9/dronesploit.egg-info/
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     4736 2022-02-27 10:33:17.000000 dronesploit-1.1.9/dronesploit.egg-info/PKG-INFO
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     1344 2022-02-27 10:33:17.000000 dronesploit-1.1.9/dronesploit.egg-info/SOURCES.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)        1 2022-02-27 10:33:17.000000 dronesploit-1.1.9/dronesploit.egg-info/dependency_links.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)       59 2022-02-27 10:33:17.000000 dronesploit-1.1.9/dronesploit.egg-info/entry_points.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)       17 2022-02-27 10:33:17.000000 dronesploit-1.1.9/dronesploit.egg-info/requires.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)       12 2022-02-27 10:33:17.000000 dronesploit-1.1.9/dronesploit.egg-info/top_level.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     1114 2022-02-27 10:33:17.702025 dronesploit-1.1.9/setup.cfg
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)      383 2021-02-15 20:28:15.000000 dronesploit-1.1.9/setup.py
```

### Comparing `dronesploit-1.1.8/LICENSE` & `dronesploit-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/PKG-INFO` & `dronesploit-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronesploit
-Version: 1.1.8
+Version: 1.1.9
 Summary: Drone pentesting framework console
 Home-page: https://github.com/dhondta/dronesploit
 Author: Alexandre D'Hondt
 Author-email: alexandre.dhondt@gmail.com
 License: AGPLv3
 Keywords: drone,pentesting,framework
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dronesploit Version: 1.1.8 Summary: Drone
+Metadata-Version: 2.1 Name: dronesploit Version: 1.1.9 Summary: Drone
 pentesting framework console Home-page: https://github.com/dhondta/dronesploit
 Author: Alexandre D'Hondt Author-email: alexandre.dhondt@gmail.com License:
 AGPLv3 Keywords: drone,pentesting,framework Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dronesploit-1.1.8/README.md` & `dronesploit-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/__init__.py` & `dronesploit-1.1.9/dronesploit/__init__.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/__main__.py` & `dronesploit-1.1.9/dronesploit/__main__.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/banners/banner1.asc` & `dronesploit-1.1.9/dronesploit/_src/banners/banner1.asc`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/banners/banner2.asc` & `dronesploit-1.1.9/dronesploit/_src/banners/banner2.asc`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/banners/banner3.asc` & `dronesploit-1.1.9/dronesploit/_src/banners/banner3.asc`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/banners/banner4.asc` & `dronesploit-1.1.9/dronesploit/_src/banners/banner4.asc`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/banners/banner5.asc` & `dronesploit-1.1.9/dronesploit/_src/banners/banner5.asc`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/banners/banner6.asc` & `dronesploit-1.1.9/dronesploit/_src/banners/banner6.asc`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/commands/generic.py` & `dronesploit-1.1.9/dronesploit/_src/commands/generic.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/commands/wifi.py` & `dronesploit-1.1.9/dronesploit/_src/commands/wifi.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/wifi/crack.py` & `dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/wifi/crack.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/wifi/deauth.py` & `dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/wifi/deauth.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/modules/auxiliary/wifi/sniff.py` & `dronesploit-1.1.9/dronesploit/_src/modules/auxiliary/wifi/sniff.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/modules/command/dji/tello.py` & `dronesploit-1.1.9/dronesploit/_src/modules/command/dji/tello.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/modules/command/hobicco/cme.py` & `dronesploit-1.1.9/dronesploit/_src/modules/command/hobicco/cme.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/modules/command/hobicco/flitt.py` & `dronesploit-1.1.9/dronesploit/_src/modules/command/hobicco/flitt.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/modules/exploit/hobbico/cme.py` & `dronesploit-1.1.9/dronesploit/_src/modules/exploit/hobbico/cme.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/_src/modules/exploit/hobbico/flitt.py` & `dronesploit-1.1.9/dronesploit/_src/modules/exploit/hobbico/flitt.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/drones/__init__.py` & `dronesploit-1.1.9/dronesploit/drones/__init__.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/drones/dji.py` & `dronesploit-1.1.9/dronesploit/drones/dji.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/drones/hobbico.py` & `dronesploit-1.1.9/dronesploit/drones/hobbico.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/generic/decorators.py` & `dronesploit-1.1.9/dronesploit/generic/decorators.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/generic/mixins.py` & `dronesploit-1.1.9/dronesploit/generic/mixins.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/wifi/__init__.py` & `dronesploit-1.1.9/dronesploit/wifi/__init__.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/wifi/drone.py` & `dronesploit-1.1.9/dronesploit/wifi/drone.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit/wifi/mixin.py` & `dronesploit-1.1.9/dronesploit/wifi/mixin.py`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/dronesploit.egg-info/PKG-INFO` & `dronesploit-1.1.9/dronesploit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronesploit
-Version: 1.1.8
+Version: 1.1.9
 Summary: Drone pentesting framework console
 Home-page: https://github.com/dhondta/dronesploit
 Author: Alexandre D'Hondt
 Author-email: alexandre.dhondt@gmail.com
 License: AGPLv3
 Keywords: drone,pentesting,framework
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dronesploit Version: 1.1.8 Summary: Drone
+Metadata-Version: 2.1 Name: dronesploit Version: 1.1.9 Summary: Drone
 pentesting framework console Home-page: https://github.com/dhondta/dronesploit
 Author: Alexandre D'Hondt Author-email: alexandre.dhondt@gmail.com License:
 AGPLv3 Keywords: drone,pentesting,framework Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dronesploit-1.1.8/dronesploit.egg-info/SOURCES.txt` & `dronesploit-1.1.9/dronesploit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dronesploit-1.1.8/setup.cfg` & `dronesploit-1.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	Programming Language :: Python :: 3.8
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
 include_package_data = False
 install_requires = 
-	sploitkit>=0.5.3
+	sploitkit>=0.5.4
 setup_requires = setuptools
 python_requires = >=3.6,<4
 
 [options.package_data]
 * = *.txt
 
 [options.entry_points]
```

