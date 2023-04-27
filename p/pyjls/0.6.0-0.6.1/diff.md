# Comparing `tmp/pyjls-0.6.0.tar.gz` & `tmp/pyjls-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.6.0.tar", last modified: Wed Apr 26 20:14:11 2023, max compression
+gzip compressed data, was "pyjls-0.6.1.tar", last modified: Thu Apr 27 22:12:27 2023, max compression
```

## Comparing `pyjls-0.6.0.tar` & `pyjls-0.6.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.177720 pyjls-0.6.0/
--rw-rw-rw-   0        0        0     4058 2023-04-26 19:37:06.000000 pyjls-0.6.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.6.0/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0    14665 2023-04-26 20:14:11.177720 pyjls-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.146674 pyjls-0.6.0/include/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.152190 pyjls-0.6.0/include/jls/
--rw-rw-rw-   0        0        0     2729 2023-04-19 20:33:33.000000 pyjls-0.6.0/include/jls/backend.h
--rw-rw-rw-   0        0        0     2068 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/cmacro.h
--rw-rw-rw-   0        0        0     1585 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/crc32c.h
--rw-rw-rw-   0        0        0     4064 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/ec.h
--rw-rw-rw-   0        0        0    24468 2023-04-26 11:42:25.000000 pyjls-0.6.0/include/jls/format.h
--rw-rw-rw-   0        0        0    11561 2023-04-26 14:23:01.000000 pyjls-0.6.0/include/jls/log.h
--rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/raw.h
--rw-rw-rw-   0        0        0    10319 2023-04-26 17:43:17.000000 pyjls-0.6.0/include/jls/reader.h
--rw-rw-rw-   0        0        0     4133 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/statistics.h
--rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/threaded_writer.h
--rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.6.0/include/jls/time.h
--rw-rw-rw-   0        0        0     2760 2023-04-26 19:51:39.000000 pyjls-0.6.0/include/jls/version.h
--rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/writer.h
--rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls.h
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.141663 pyjls-0.6.0/include_prv/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.155690 pyjls-0.6.0/include_prv/jls/
--rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.6.0/include_prv/jls/bit_shift.h
--rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/cdef.h
--rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.6.0/include_prv/jls/datatype.h
--rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/msg_ring_buffer.h
--rw-rw-rw-   0        0        0     1784 2023-04-26 18:12:34.000000 pyjls-0.6.0/include_prv/jls/rd_fsr.h
--rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/util.h
--rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/wr_fsr.h
--rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/wr_prv.h
--rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/wr_ts.h
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.158690 pyjls-0.6.0/pyjls/
--rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.6.0/pyjls/__init__.py
--rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/__main__.py
--rw-rw-rw-   0        0        0  1587118 2023-04-26 19:59:45.000000 pyjls-0.6.0/pyjls/binding.c
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.168206 pyjls-0.6.0/pyjls/entry_points/
--rw-rw-rw-   0        0        0      853 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/entry_points/__init__.py
--rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/entry_points/annotate.py
--rw-rw-rw-   0        0        0     1621 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/entry_points/info.py
--rw-rw-rw-   0        0        0     2206 2023-04-26 14:31:44.000000 pyjls-0.6.0/pyjls/structs.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.169206 pyjls-0.6.0/pyjls/test/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/test/__init__.py
--rw-rw-rw-   0        0        0    10313 2023-04-26 19:18:13.000000 pyjls-0.6.0/pyjls/test/test_binding.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.169206 pyjls-0.6.0/pyjls/v1/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/v1/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-04-26 19:51:39.000000 pyjls-0.6.0/pyjls/version.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.167208 pyjls-0.6.0/pyjls.egg-info/
--rw-rw-rw-   0        0        0    14665 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1310 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 20:14:11.177720 pyjls-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     6960 2023-04-26 19:16:46.000000 pyjls-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.176720 pyjls-0.6.0/src/
--rw-rw-rw-   0        0        0     8684 2023-04-19 20:32:02.000000 pyjls-0.6.0/src/backend_posix.c
--rw-rw-rw-   0        0        0     9046 2023-04-19 20:31:50.000000 pyjls-0.6.0/src/backend_win.c
--rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.6.0/src/bit_shift.c
--rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/crc32c_arm_neon.c
--rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/crc32c_intel_sse4.c
--rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/crc32c_sw.c
--rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.6.0/src/datatype.c
--rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/ec.c
--rw-rw-rw-   0        0        0     1631 2023-04-19 17:02:27.000000 pyjls-0.6.0/src/log.c
--rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.6.0/src/msg_ring_buffer.c
--rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.6.0/src/raw.c
--rw-rw-rw-   0        0        0     5903 2023-04-26 19:35:45.000000 pyjls-0.6.0/src/rd_fsr.c
--rw-rw-rw-   0        0        0    54236 2023-04-26 19:37:31.000000 pyjls-0.6.0/src/reader.c
--rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/statistics.c
--rw-rw-rw-   0        0        0    11268 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/threaded_writer.c
--rw-rw-rw-   0        0        0    22039 2023-04-26 14:52:04.000000 pyjls-0.6.0/src/wr_fsr.c
--rw-rw-rw-   0        0        0     9691 2023-04-26 14:57:54.000000 pyjls-0.6.0/src/wr_ts.c
--rw-rw-rw-   0        0        0    30342 2023-04-26 12:23:06.000000 pyjls-0.6.0/src/writer.c
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.400065 pyjls-0.6.1/
+-rw-rw-rw-   0        0        0     4219 2023-04-27 22:08:49.000000 pyjls-0.6.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.6.1/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    14665 2023-04-27 22:12:27.399565 pyjls-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.369250 pyjls-0.6.1/include/
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.375270 pyjls-0.6.1/include/jls/
+-rw-rw-rw-   0        0        0     2729 2023-04-19 20:33:33.000000 pyjls-0.6.1/include/jls/backend.h
+-rw-rw-rw-   0        0        0     2068 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/cmacro.h
+-rw-rw-rw-   0        0        0     1585 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/crc32c.h
+-rw-rw-rw-   0        0        0     4064 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/ec.h
+-rw-rw-rw-   0        0        0    24468 2023-04-26 11:42:25.000000 pyjls-0.6.1/include/jls/format.h
+-rw-rw-rw-   0        0        0    11561 2023-04-26 14:23:01.000000 pyjls-0.6.1/include/jls/log.h
+-rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/raw.h
+-rw-rw-rw-   0        0        0    10319 2023-04-26 17:43:17.000000 pyjls-0.6.1/include/jls/reader.h
+-rw-rw-rw-   0        0        0     4133 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/statistics.h
+-rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/threaded_writer.h
+-rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.6.1/include/jls/time.h
+-rw-rw-rw-   0        0        0     2760 2023-04-27 22:10:57.000000 pyjls-0.6.1/include/jls/version.h
+-rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/writer.h
+-rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls.h
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.364542 pyjls-0.6.1/include_prv/
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.378770 pyjls-0.6.1/include_prv/jls/
+-rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.6.1/include_prv/jls/bit_shift.h
+-rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/cdef.h
+-rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.6.1/include_prv/jls/datatype.h
+-rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/msg_ring_buffer.h
+-rw-rw-rw-   0        0        0     1784 2023-04-26 18:12:34.000000 pyjls-0.6.1/include_prv/jls/rd_fsr.h
+-rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/util.h
+-rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/wr_fsr.h
+-rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/wr_prv.h
+-rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/wr_ts.h
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.381783 pyjls-0.6.1/pyjls/
+-rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.6.1/pyjls/__init__.py
+-rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/__main__.py
+-rw-rw-rw-   0        0        0  1587118 2023-04-26 19:59:45.000000 pyjls-0.6.1/pyjls/binding.c
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.390296 pyjls-0.6.1/pyjls/entry_points/
+-rw-rw-rw-   0        0        0      853 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/entry_points/annotate.py
+-rw-rw-rw-   0        0        0     1621 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/entry_points/info.py
+-rw-rw-rw-   0        0        0     2206 2023-04-26 14:31:44.000000 pyjls-0.6.1/pyjls/structs.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.390796 pyjls-0.6.1/pyjls/test/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/test/__init__.py
+-rw-rw-rw-   0        0        0    10313 2023-04-26 19:18:13.000000 pyjls-0.6.1/pyjls/test/test_binding.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.390796 pyjls-0.6.1/pyjls/v1/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/v1/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-04-27 22:10:57.000000 pyjls-0.6.1/pyjls/version.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.388793 pyjls-0.6.1/pyjls.egg-info/
+-rw-rw-rw-   0        0        0    14665 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1310 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 22:12:27.400065 pyjls-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     6742 2023-04-27 15:16:07.000000 pyjls-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.399061 pyjls-0.6.1/src/
+-rw-rw-rw-   0        0        0     8684 2023-04-19 20:32:02.000000 pyjls-0.6.1/src/backend_posix.c
+-rw-rw-rw-   0        0        0     9046 2023-04-19 20:31:50.000000 pyjls-0.6.1/src/backend_win.c
+-rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.6.1/src/bit_shift.c
+-rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/crc32c_arm_neon.c
+-rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/crc32c_intel_sse4.c
+-rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/crc32c_sw.c
+-rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.6.1/src/datatype.c
+-rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/ec.c
+-rw-rw-rw-   0        0        0     1631 2023-04-19 17:02:27.000000 pyjls-0.6.1/src/log.c
+-rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.6.1/src/msg_ring_buffer.c
+-rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.6.1/src/raw.c
+-rw-rw-rw-   0        0        0     5903 2023-04-26 19:35:45.000000 pyjls-0.6.1/src/rd_fsr.c
+-rw-rw-rw-   0        0        0    54497 2023-04-27 17:06:33.000000 pyjls-0.6.1/src/reader.c
+-rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/statistics.c
+-rw-rw-rw-   0        0        0    11622 2023-04-27 15:21:50.000000 pyjls-0.6.1/src/threaded_writer.c
+-rw-rw-rw-   0        0        0    27653 2023-04-27 21:59:42.000000 pyjls-0.6.1/src/wr_fsr.c
+-rw-rw-rw-   0        0        0     9691 2023-04-26 14:57:54.000000 pyjls-0.6.1/src/wr_ts.c
+-rw-rw-rw-   0        0        0    30342 2023-04-26 12:23:06.000000 pyjls-0.6.1/src/writer.c
```

### Comparing `pyjls-0.6.0/CHANGELOG.md` & `pyjls-0.6.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the JLS project.
 
 
+## 0.6.1
+
+2023 Apr 27
+
+* Added FSR support for missing and duplicate data.
+* Added FSR support for unaligned u1 and u4 data.
+* Improved log messages.
+
+
 ## 0.6.0
 
 2023 Apr 26
 
 * Fixed JLS to handle non-zero sample_id for first FSR data sample.
 * Added pyjls.Reader.timestamp_to_sample_id and sample_id_to_timestamp.
```

### Comparing `pyjls-0.6.0/CREDITS.html` & `pyjls-0.6.1/CREDITS.html`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/LICENSE` & `pyjls-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/PKG-INFO` & `pyjls-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.6.0
+Version: 0.6.1
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.6.0/README.md` & `pyjls-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/backend.h` & `pyjls-0.6.1/include/jls/backend.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/cmacro.h` & `pyjls-0.6.1/include/jls/cmacro.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/crc32c.h` & `pyjls-0.6.1/include/jls/crc32c.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/ec.h` & `pyjls-0.6.1/include/jls/ec.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/format.h` & `pyjls-0.6.1/include/jls/format.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/log.h` & `pyjls-0.6.1/include/jls/log.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/raw.h` & `pyjls-0.6.1/include/jls/raw.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/reader.h` & `pyjls-0.6.1/include/jls/reader.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/statistics.h` & `pyjls-0.6.1/include/jls/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/threaded_writer.h` & `pyjls-0.6.1/include/jls/threaded_writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/time.h` & `pyjls-0.6.1/include/jls/time.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls/version.h` & `pyjls-0.6.1/include/jls/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  */
 
 JLS_CPP_GUARD_START
 
 // Use version_update.py to update.
 #define JLS_VERSION_MAJOR 0
 #define JLS_VERSION_MINOR 6
-#define JLS_VERSION_PATCH 0
+#define JLS_VERSION_PATCH 1
 
 /**
  * \brief Macro to encode version to uint32_t.
  *
  * \param major The major release number (0 to 255)
  * \param minor The minor release number (0 to 255)
  * \param patch The patch release number (0 to 65535)
```

### Comparing `pyjls-0.6.0/include/jls/writer.h` & `pyjls-0.6.1/include/jls/writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include/jls.h` & `pyjls-0.6.1/include/jls.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/bit_shift.h` & `pyjls-0.6.1/include_prv/jls/bit_shift.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/cdef.h` & `pyjls-0.6.1/include_prv/jls/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/datatype.h` & `pyjls-0.6.1/include_prv/jls/datatype.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/msg_ring_buffer.h` & `pyjls-0.6.1/include_prv/jls/msg_ring_buffer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/rd_fsr.h` & `pyjls-0.6.1/include_prv/jls/rd_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/util.h` & `pyjls-0.6.1/include_prv/jls/util.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/wr_fsr.h` & `pyjls-0.6.1/include_prv/jls/wr_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/wr_prv.h` & `pyjls-0.6.1/include_prv/jls/wr_prv.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/include_prv/jls/wr_ts.h` & `pyjls-0.6.1/include_prv/jls/wr_ts.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/__init__.py` & `pyjls-0.6.1/pyjls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/__main__.py` & `pyjls-0.6.1/pyjls/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/binding.c` & `pyjls-0.6.1/pyjls/binding.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/entry_points/__init__.py` & `pyjls-0.6.1/pyjls/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/entry_points/annotate.py` & `pyjls-0.6.1/pyjls/entry_points/annotate.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/entry_points/info.py` & `pyjls-0.6.1/pyjls/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/structs.py` & `pyjls-0.6.1/pyjls/structs.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/test/__init__.py` & `pyjls-0.6.1/pyjls/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/test/test_binding.py` & `pyjls-0.6.1/pyjls/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/v1/__init__.py` & `pyjls-0.6.1/pyjls/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyjls/version.py` & `pyjls-0.6.1/pyjls/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 __title__ = "pyjls"
 __description__ = 'Joulescope™ file format'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjls-0.6.0/pyjls.egg-info/PKG-INFO` & `pyjls-0.6.1/pyjls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.6.0
+Version: 0.6.1
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.6.0/pyjls.egg-info/SOURCES.txt` & `pyjls-0.6.1/pyjls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/pyproject.toml` & `pyjls-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/setup.py` & `pyjls-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,30 +18,20 @@
 
 See:
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
 
 # Always prefer setuptools over distutils
-import setuptools
 import setuptools.dist
 import distutils.cmd
 from distutils.errors import DistutilsExecError
+import numpy as np
 import os
 import platform
-import sys
-
-if platform.system() == 'Windows':
-    numpy_req = 'numpy>=1.23'
-else:
-    numpy_req = 'numpy>=1.20'
-
-setuptools.dist.Distribution().fetch_build_eggs(['Cython>=0.29.3', numpy_req])
-
-import numpy as np
 
 
 MYPATH = os.path.dirname(os.path.abspath(__file__))
 VERSION_PATH = os.path.join(MYPATH, 'pyjls', 'version.py')
 
 
 try:
@@ -194,15 +184,15 @@
     include_dirs=[],
     
     # See https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
     python_requires='~=3.8',
 
     # See https://packaging.python.org/en/latest/requirements.html
     install_requires=[
-        numpy_req,
+        'numpy>=1.23',
         "pywin32; platform_system=='Windows'",
     ],
 
     entry_points={
         'console_scripts': [
             'pyjls=pyjls.__main__:run',
         ],
```

### Comparing `pyjls-0.6.0/src/backend_posix.c` & `pyjls-0.6.1/src/backend_posix.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/backend_win.c` & `pyjls-0.6.1/src/backend_win.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/bit_shift.c` & `pyjls-0.6.1/src/bit_shift.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/crc32c_arm_neon.c` & `pyjls-0.6.1/src/crc32c_arm_neon.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/crc32c_intel_sse4.c` & `pyjls-0.6.1/src/crc32c_intel_sse4.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/crc32c_sw.c` & `pyjls-0.6.1/src/crc32c_sw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/datatype.c` & `pyjls-0.6.1/src/datatype.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/ec.c` & `pyjls-0.6.1/src/ec.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/log.c` & `pyjls-0.6.1/src/log.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/msg_ring_buffer.c` & `pyjls-0.6.1/src/msg_ring_buffer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/raw.c` & `pyjls-0.6.1/src/raw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/rd_fsr.c` & `pyjls-0.6.1/src/rd_fsr.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/reader.c` & `pyjls-0.6.1/src/reader.c`

 * *Files 1% similar despite different names*

```diff
@@ -868,30 +868,34 @@
     const int64_t data_length_orig = data_length;
     int32_t rv = 0;
     uint8_t * data_u8 = (uint8_t *) data;
     if (!is_signal_defined_type(self, signal_id, JLS_SIGNAL_TYPE_FSR)) {
         JLS_LOGW("signal_id %d invalid", (int) signal_id);
         return JLS_ERROR_PARAMETER_INVALID;
     }
+    int64_t samples = 0;
+    ROE(jls_rd_fsr_length(self, signal_id, &samples));
+    struct jls_signal_def_s * signal_def = &self->signal_def[signal_id];
     if (data_length <= 0) {
         return 0;
     } else if (start_sample_id < 0) {
-        JLS_LOGW("start_sample_id invalid: %" PRIi64, start_sample_id);
+        JLS_LOGW("rd_fsr %d %s: start_sample_id invalid %" PRIi64 " length=%" PRIi64,
+                 (int) signal_id, signal_def->name,
+                 start_sample_id, samples);
         return JLS_ERROR_PARAMETER_INVALID;
     }
 
-    struct jls_signal_def_s * signal_def = &self->signal_def[signal_id];
     const int64_t sample_id_offset = self->signal_def[signal_id].sample_id_offset;
-    int64_t samples = 0;
     uint8_t entry_size_bits = jls_datatype_parse_size(signal_def->data_type);
 
-    ROE(jls_rd_fsr_length(self, signal_id, &samples));
     if ((start_sample_id + data_length) > samples) {
-        JLS_LOGW("length invalid: %" PRIi64 " > %" PRIi64,
-                 start_sample_id + data_length, samples);
+        JLS_LOGW("rd_fsr %d %s: start=%" PRIi64 " length=%" PRIi64 " > %" PRIi64 " by %" PRIi64,
+                 (int) signal_id, signal_def->name,
+                 start_sample_id, data_length, samples,
+                 start_sample_id + data_length - samples);
         return JLS_ERROR_PARAMETER_INVALID;
     }
 
     uint8_t shift_right_bits = 0;
     if (entry_size_bits < 8) {
         int64_t sample_id = start_sample_id;
         switch (entry_size_bits) {
```

### Comparing `pyjls-0.6.0/src/statistics.c` & `pyjls-0.6.1/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/threaded_writer.c` & `pyjls-0.6.1/src/threaded_writer.c`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,24 @@
 enum message_e {
     MSG_CLOSE,          // no header data, no args
     MSG_FLUSH,          // no header data, no args
     MSG_USER_DATA,      // hdr.user_data, user_data
     MSG_FSR,            // hdr.fsr_f32, data
     MSG_ANNOTATION,     // hdr.annotation, data
     MSG_UTC,            // hdr.utc, data
+    MSG_ITEM_COUNT,
+};
+
+const char * message_str[] = {
+        "close",
+        "flush",
+        "user_data",
+        "fsr",
+        "annotation",
+        "utc",
 };
 
 int32_t jls_twr_run(struct jls_twr_s * self) {
     uint32_t msg_size;
     uint8_t * msg;
     struct msg_header_s hdr;
     uint8_t * payload;
@@ -148,15 +158,18 @@
                     rc = jls_wr_utc(self->wr, hdr.h.utc.signal_id, hdr.h.utc.sample_id, hdr.h.utc.utc);
                 default:
                     break;
             }
             jls_bkt_process_unlock(self->bk);
 
             if (rc) {
-                JLS_LOGW("thread msg %d returned %d", (int) hdr.msg_type, (int) rc);
+                JLS_LOGW("thread msg %d:%s returned %d:%s",
+                         (int) hdr.msg_type,
+                         (hdr.msg_type < MSG_ITEM_COUNT) ? message_str[hdr.msg_type] : "unknown",
+                         (int) rc, jls_error_code_name(rc));
             }
 
             while (!self->quit && jls_bkt_msg_lock(self->bk)) {
                 // retry
             }
             jls_mrb_pop(&self->mrb, &msg_size);
             // stay locked
```

### Comparing `pyjls-0.6.0/src/wr_fsr.c` & `pyjls-0.6.1/src/wr_fsr.c`

 * *Files 21% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 struct jls_wr_fsr_s {
     struct jls_wr_s * wr;
     struct jls_signal_def_s def;
     uint32_t data_length;  // for data, in samples
     struct jls_fsr_data_s * data;  // for level 0
     double * data_f64;
     int64_t sample_id_offset;
+    uint8_t shift_amount;
+    uint8_t shift_buffer;
+    uint64_t buffer_u64[4096];
     struct level_s * level[JLS_SUMMARY_LEVEL_COUNT];  // level 0 unused
 };
 
 static int32_t summaryN(struct jls_wr_fsr_s * self, uint8_t level, int64_t pos);
 static int32_t summary1(struct jls_wr_fsr_s * self, int64_t pos);
 
 static inline uint8_t sample_size_bits(struct jls_wr_fsr_s * self) {
@@ -372,39 +375,51 @@
     }
     ++dst->summary->header.entry_count;
 }
 
 #define SUMMARYN_BODY_TEMPLATE()                                                            \
     for (uint32_t idx = 0; idx < summaries_per; ++idx) {                                    \
         uint32_t sample_idx = idx * self->def.summary_decimate_factor;                      \
+        uint32_t count = 0;                                                                 \
+        double v;                                                                           \
         double v_mean = 0.0;                                                                \
         double v_min = DBL_MAX;                                                             \
         double v_max = -DBL_MAX;                                                            \
         double v_var = 0.0;                                                                 \
         for (uint32_t sample = 0; sample < self->def.summary_decimate_factor; ++sample) {   \
             uint32_t offset = sample_idx * JLS_SUMMARY_FSR_COUNT;                           \
-            v_mean += src_data[offset + JLS_SUMMARY_FSR_MEAN];                              \
-            if (src_data[offset + JLS_SUMMARY_FSR_MIN] < v_min) {                           \
-                v_min = src_data[offset + JLS_SUMMARY_FSR_MIN];                             \
+            v = src_data[offset + JLS_SUMMARY_FSR_MEAN];                                    \
+            if (isfinite(v)) {                                                              \
+                v_mean += v;                                                                \
+                if (src_data[offset + JLS_SUMMARY_FSR_MIN] < v_min) {                       \
+                    v_min = src_data[offset + JLS_SUMMARY_FSR_MIN];                         \
+                }                                                                           \
+                if (src_data[offset + JLS_SUMMARY_FSR_MAX] > v_max) {                       \
+                    v_max = src_data[offset + JLS_SUMMARY_FSR_MAX];                         \
+                }                                                                           \
             }                                                                               \
-            if (src_data[offset + JLS_SUMMARY_FSR_MAX] > v_max) {                           \
-                v_max = src_data[offset + JLS_SUMMARY_FSR_MAX];                             \
-            }                                                                               \
-            ++sample_idx;                                                                   \
-        }                                                                                   \
-        v_mean *= scale;                                                                    \
-        sample_idx = idx * self->def.summary_decimate_factor;                               \
-        for (uint32_t sample = 0; sample < self->def.summary_decimate_factor; ++sample) {   \
-            uint32_t offset = sample_idx * JLS_SUMMARY_FSR_COUNT;                           \
-            double v = src_data[offset + JLS_SUMMARY_FSR_MEAN] - v_mean;                    \
-            double std = src_data[offset + JLS_SUMMARY_FSR_STD];                            \
-            v_var += (std * std) + (v * v);                                                 \
             ++sample_idx;                                                                   \
         }                                                                                   \
-        v_var *= scale;                                                                     \
+        if (count == 0) {                                                                   \
+            v_mean = NAN;                                                                   \
+            v_var = NAN;                                                                    \
+            v_min = NAN;                                                                    \
+            v_max = NAN;                                                                    \
+        } else {                                                                            \
+            v_mean /= count;                                                                    \
+            sample_idx = idx * self->def.summary_decimate_factor;                               \
+            for (uint32_t sample = 0; sample < self->def.summary_decimate_factor; ++sample) {   \
+                uint32_t offset = sample_idx * JLS_SUMMARY_FSR_COUNT;                           \
+                double v = src_data[offset + JLS_SUMMARY_FSR_MEAN] - v_mean;                    \
+                double std = src_data[offset + JLS_SUMMARY_FSR_STD];                            \
+                v_var += (std * std) + (v * v);                                                 \
+                ++sample_idx;                                                                   \
+            }                                                                                   \
+            v_var /= count;                                                                 \
+        }                                                                                    \
         summary_entry_add(self, level, v_mean, v_min, v_max, v_var);                        \
     }
 
 
 static int32_t summaryN(struct jls_wr_fsr_s * self, uint8_t level, int64_t pos) {
     if (level < 2) {
         JLS_LOGE("invalid summaryN level: %d", (int) level);
@@ -414,15 +429,14 @@
     struct level_s * dst = self->level[level];
 
     if (!dst) {
         ROE(summary_alloc(self, level));
         dst = self->level[level];
     }
 
-    const double scale = 1.0 / self->def.summary_decimate_factor;
     JLS_LOGD2("summaryN %d: %" PRIu32 " %" PRIi64, (int) level, dst->index->header.entry_count, pos);
     dst->index->offsets[dst->index->header.entry_count++] = pos;
 
     uint32_t summaries_per = (uint32_t) (src->summary->header.entry_count / self->def.summary_decimate_factor);
     if (summary_entry_size(self) == 64) {
         double * src_data = ((struct jls_fsr_f64_summary_s *) src->summary)->data[0];
         SUMMARYN_BODY_TEMPLATE();
@@ -450,102 +464,204 @@
     if (!dst) {
         ROE(summary_alloc(self, 1));
         dst = self->level[1];
     }
     data_to_f64(self);
 
     double * data = self->data_f64;
-    const double scale = 1.0 / self->def.sample_decimate_factor;
-    const double var_scale = 1.0 / (self->def.sample_decimate_factor - 1);  // for sample variance
     // JLS_LOGI("1 add %" PRIi64 " @ %" PRIi64 " %p", pos, dst->index->offset, &dst->index->data[dst->index->offset]);
     dst->index->offsets[dst->index->header.entry_count++] = pos;
 
     uint32_t summaries_per = (uint32_t) (self->data->header.entry_count / self->def.sample_decimate_factor);
     for (uint32_t idx = 0; idx < summaries_per; ++idx) {
         uint32_t sample_idx = idx * self->def.sample_decimate_factor;
+        uint32_t count = 0;
         double v_mean = 0.0;
         double v_min = DBL_MAX;
         double v_max = -DBL_MAX;
         double v_var = 0.0;
         for (uint32_t sample = 0; sample < self->def.sample_decimate_factor; ++sample) {
             double v = data[sample_idx];
-            v_mean += v;
-            if (v < v_min) {
-                v_min = v;
-            }
-            if (v > v_max) {
-                v_max = v;
+            if (isfinite(v)) {
+                ++count;
+                v_mean += v;
+                if (v < v_min) {
+                    v_min = v;
+                }
+                if (v > v_max) {
+                    v_max = v;
+                }
             }
             ++sample_idx;
         }
-        v_mean *= scale;
-        sample_idx = idx * self->def.sample_decimate_factor;
-        for (uint32_t sample = 0; sample < self->def.sample_decimate_factor; ++sample) {
-            double v = data[sample_idx] - v_mean;
-            v_var += v * v;
-            ++sample_idx;
+        if (count == 0) {
+            v_mean = NAN;
+            v_min = NAN;
+            v_max = NAN;
+            v_var = NAN;
+        } else {
+            v_mean /= count;
+            sample_idx = idx * self->def.sample_decimate_factor;
+            for (uint32_t sample = 0; sample < self->def.sample_decimate_factor; ++sample) {
+                double v = data[sample_idx];
+                if (isfinite(v)) {
+                    v -= v_mean;
+                    v_var += v * v;
+                }
+                ++sample_idx;
+            }
+            if (count == 1) {
+                v_var = 0.0;
+            } else {
+                v_var /= count;
+            }
         }
-        v_var *= var_scale;
         summary_entry_add(self, 1, v_mean, v_min, v_max, v_var);
     }
 
     if (dst->summary->header.entry_count >= dst->summary_entries) {
         ROE(wr_summary(self, 1));
     }
     return 0;
 }
 
-int32_t jls_wr_fsr_data(struct jls_wr_fsr_s * self, int64_t sample_id, const void * data, uint32_t data_length) {
+static int32_t wr_data_inner(struct jls_wr_fsr_s * self, const void * data, uint32_t data_length) {
     struct jls_fsr_data_s * b = self->data;
+    uint8_t sample_size_bits = jls_datatype_parse_size(self->def.data_type);
     const uint8_t * src_u8 = (const uint8_t *) (data);
     uint8_t * dst_u8;
-    uint8_t sample_size_bits = jls_datatype_parse_size(self->def.data_type);
-
-    if (0 == data_length) {
-        return 0;
-    }
-
-    // only support byte-aligned writes for now - enforce
-    switch (sample_size_bits) {
-        case 1:
-            if ((sample_id & 0x7) || (data_length & 0x7)) {
-                return JLS_ERROR_PARAMETER_INVALID;
-            }
-            break;
-        case 4:
-            if ((sample_id & 1) || (data_length & 1)) {
-                return JLS_ERROR_PARAMETER_INVALID;
-            }
-            break;
-        default:
-            break;
-    }
-
-    if (!b) {
-        ROE(sample_buffer_alloc(self));
-        b = self->data;
-        self->sample_id_offset = sample_id;  // can be nonzero
-    }
-
-    // todo check for & handle sample_id skips
-    if (!b->header.entry_count) {
-        b->header.timestamp = sample_id;
-    }
+    uint8_t shift_this = (data_length * sample_size_bits) % 8;
+    uint8_t shift_amount_next = (shift_this + self->shift_amount) % 8;
 
     while (data_length) {
         dst_u8 = (uint8_t *) &b->data[0];
         dst_u8 += (b->header.entry_count * sample_size_bits) / 8;
         uint32_t length = (uint32_t) (self->data_length - b->header.entry_count);
         if (data_length < length) {
             length = data_length;
         }
-        size_t byte_length = (length * sample_size_bits) / 8;
-        memcpy(dst_u8, src_u8, byte_length);
+        if (self->shift_amount) {
+            uint8_t mask = (1 << self->shift_amount) - 1;
+            uint32_t bits = length * sample_size_bits + self->shift_amount;
+            while (bits) {
+                uint16_t v = (self->shift_buffer & mask) | (((uint16_t) (*src_u8++)) << self->shift_amount);
+                if (bits >= 8) {
+                    *dst_u8++ = (uint8_t) v;
+                    bits -= 8;
+                    self->shift_buffer = (uint8_t) (v >> 8);
+                } else {
+                    self->shift_buffer = (uint8_t) v;
+                    break;
+                }
+            }
+        } else {
+            size_t byte_length = (length * sample_size_bits) / 8;
+            if (byte_length) {
+                memcpy(dst_u8, src_u8, byte_length);
+            }
+            self->shift_buffer = src_u8[byte_length];
+            src_u8 += byte_length;
+        }
         b->header.entry_count += length;
-        src_u8 += byte_length;
         data_length -= length;
         if (b->header.entry_count >= self->data_length) {
             ROE(wr_data(self));
         }
     }
+    self->shift_amount = shift_amount_next;
     return 0;
 }
+
+int32_t jls_wr_fsr_data(struct jls_wr_fsr_s * self, int64_t sample_id, const void * data, uint32_t data_length) {
+    uint8_t sample_size_bits = jls_datatype_parse_size(self->def.data_type);
+
+    if (0 == data_length) {
+        return 0;
+    }
+
+    if (!self->data) {
+        ROE(sample_buffer_alloc(self));
+        self->sample_id_offset = sample_id;  // can be nonzero
+        self->data->header.timestamp = sample_id;
+    }
+
+    struct jls_fsr_data_s * b = self->data;
+    int64_t sample_id_next = b->header.timestamp + b->header.entry_count;
+    if (sample_id == sample_id_next) {
+        // normal
+    } else if (sample_id < sample_id_next) {
+        JLS_LOGI("fsr dup: in=%" PRIi64 " expect=%" PRIi64,
+                 sample_id, sample_id_next);
+        if ((sample_id + data_length) <= sample_id_next) {
+            return 0;
+        }
+        const uint8_t * data_u8 = (const uint8_t *) data;
+        const uint8_t * data_end_u8 = data_u8 + (data_length * sample_size_bits + 7) / 8;
+        uint32_t ffwd = (uint32_t) (sample_id_next - sample_id);
+        data_length -= ffwd;
+        if (sample_size_bits >= 8) {
+            data = data_u8 + ffwd * (sample_size_bits / 8);
+        } else {
+            uint32_t shift = 0;
+            uint32_t shift_samples = 0;
+            if (sample_size_bits == 4) {
+                shift = (ffwd & 1) ? 4 : 0;
+                shift_samples = 1;
+            } else if (sample_size_bits == 1) {
+                shift = ffwd % sample_size_bits;
+                shift_samples = shift;
+            }
+            if (shift == 0) {
+                data = data_u8 + ffwd * (sample_size_bits / 8);
+            } else {
+                while (data_u8 < data_end_u8) {
+                    size_t sz = data_end_u8 - data_u8;
+                    if (sz > (sizeof(self->buffer_u64) - 8)) {
+                        sz = sizeof(self->buffer_u64) - 8;
+                    }
+                    memcpy(self->buffer_u64, data_u8, sz);
+                    self->buffer_u64[(sz / 8) + 1] = 0;
+                    size_t sz_words = (sz + 7) / 8;
+                    for (uint64_t idx = 0; idx < sz_words; ++idx) {
+                        self->buffer_u64[idx] = (self->buffer_u64[idx] >> shift)
+                                | (self->buffer_u64[idx + 1] << (64 - shift));
+                    }
+                    size_t entries = sz * (8 / sample_size_bits) - shift_samples;
+                    ROE(wr_data_inner(self, self->buffer_u64, (uint32_t) entries));
+                    data_u8 += sz - 1;
+                }
+                return 0;
+            }
+        }
+    } else {
+        JLS_LOGW("fsr skip: in=%" PRIi64 " expect=%" PRIi64,
+                 sample_id, sample_id_next);
+        size_t skip = (size_t) (sample_id - sample_id_next);
+        size_t buf_sz = 0;
+        if (self->def.data_type == JLS_DATATYPE_F32) {
+            float * f32 = (float *) self->buffer_u64;
+            buf_sz = sizeof(self->buffer_u64);
+            buf_sz /= sizeof(float);
+            for (size_t idx = 0; idx < buf_sz; ++idx) {
+                f32[idx] = NAN;
+            }
+        } else if (self->def.data_type == JLS_DATATYPE_F64) {
+            double * f64 = (double *) self->buffer_u64;
+            buf_sz = sizeof(self->buffer_u64) / sizeof(double);
+            for (size_t idx = 0; idx < sizeof(self->buffer_u64) / sizeof(double); ++idx) {
+                f64[idx] = NAN;
+            }
+        } else {
+            buf_sz = (sizeof(self->buffer_u64) * sample_size_bits) / 8;
+            memset(self->buffer_u64, 0, sizeof(self->buffer_u64));
+        }
+        while (skip) {
+            if (skip < buf_sz) {
+                buf_sz = skip;
+            }
+            ROE(wr_data_inner(self, self->buffer_u64, (uint32_t) buf_sz));
+            skip -= buf_sz;
+        }
+    }
+
+    return wr_data_inner(self, data, data_length);
+}
```

### Comparing `pyjls-0.6.0/src/wr_ts.c` & `pyjls-0.6.1/src/wr_ts.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.0/src/writer.c` & `pyjls-0.6.1/src/writer.c`

 * *Files identical despite different names*

