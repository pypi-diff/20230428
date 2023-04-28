# Comparing `tmp/charidotella-0.8.tar.gz` & `tmp/charidotella-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charidotella-0.8.tar", last modified: Sun Apr 23 18:53:36 2023, max compression
+gzip compressed data, was "charidotella-0.9.tar", last modified: Fri Apr 28 12:39:27 2023, max compression
```

## Comparing `charidotella-0.8.tar` & `charidotella-0.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-23 18:53:36.000000 charidotella-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-23 18:53:36.595095 charidotella-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-23 18:52:34.000000 charidotella-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.583095 charidotella-0.8/charidotella/
--rw-r--r--   0 runner    (1001) docker     (123)    40036 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/animals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.587095 charidotella-0.8/charidotella/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/assets/configuration-schema.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-04-23 18:53:23.000000 charidotella-0.8/charidotella/assets/es_to_frames
--rwxr-xr-x   0 runner    (1001) docker     (123)   281936 2023-04-23 18:53:33.000000 charidotella-0.8/charidotella/assets/event_rate
--rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella/assets/size
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/charidotella_extension_placeholder.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.587095 charidotella-0.8/charidotella/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/arbiter_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/hot_pixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.587095 charidotella-0.8/charidotella/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/colourtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/event_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/wiggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.583095 charidotella-0.8/charidotella.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.587095 charidotella-0.8/command_line_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/premake4.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.591095 charidotella-0.8/command_line_tools/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/crop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/cut.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/dat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/dat_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/es_to_csv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/es_to_frames.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/es_to_ply.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23197 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/event_rate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/evt3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/evt3_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/font.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/html.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/rainbow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/rainmaker.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/statistics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/synth.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/timecode.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/command_line_tools/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/third_party/monaco.ttf.base64.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.579095 charidotella-0.8/command_line_tools/third_party/pontella/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/command_line_tools/third_party/pontella/source/
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-23 18:52:40.000000 charidotella-0.8/command_line_tools/third_party/pontella/source/pontella.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.579095 charidotella-0.8/command_line_tools/third_party/sepia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/command_line_tools/third_party/sepia/source/
--rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-04-23 18:52:42.000000 charidotella-0.8/command_line_tools/third_party/sepia/source/sepia.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/third_party/stb_truetype.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.579095 charidotella-0.8/command_line_tools/third_party/tarsier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/command_line_tools/third_party/tarsier/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-23 18:52:47.000000 charidotella-0.8/command_line_tools/third_party/tarsier/source/replicate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-23 18:52:47.000000 charidotella-0.8/command_line_tools/third_party/tarsier/source/stitch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-23 18:52:34.000000 charidotella-0.8/configuration-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-23 18:52:34.000000 charidotella-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:53:36.595095 charidotella-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-23 18:52:34.000000 charidotella-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.969420 charidotella-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-28 12:39:27.000000 charidotella-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-28 12:39:27.969420 charidotella-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-28 12:38:45.000000 charidotella-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.961419 charidotella-0.9/charidotella/
+-rw-r--r--   0 runner    (1001) docker     (123)    40233 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/animals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.965419 charidotella-0.9/charidotella/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/assets/configuration-schema.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-04-28 12:39:17.000000 charidotella-0.9/charidotella/assets/es_to_frames
+-rwxr-xr-x   0 runner    (1001) docker     (123)   281936 2023-04-28 12:39:25.000000 charidotella-0.9/charidotella/assets/event_rate
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-04-28 12:39:27.000000 charidotella-0.9/charidotella/assets/size
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/charidotella_extension_placeholder.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.965419 charidotella-0.9/charidotella/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/filters/arbiter_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/filters/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/filters/hot_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/filters/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.965419 charidotella-0.9/charidotella/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/tasks/colourtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/tasks/event_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/tasks/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/tasks/wiggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 12:38:45.000000 charidotella-0.9/charidotella/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.961419 charidotella-0.9/charidotella.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-28 12:39:27.000000 charidotella-0.9/charidotella.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-28 12:39:27.000000 charidotella-0.9/charidotella.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:39:27.000000 charidotella-0.9/charidotella.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 12:39:27.000000 charidotella-0.9/charidotella.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 12:39:27.000000 charidotella-0.9/charidotella.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 12:39:27.000000 charidotella-0.9/charidotella.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.965419 charidotella-0.9/command_line_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/premake4.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.969420 charidotella-0.9/command_line_tools/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/crop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/cut.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/dat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/dat_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/es_to_csv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/es_to_frames.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/es_to_ply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23197 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/event_rate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/evt3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/evt3_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/font.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/html.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/rainbow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/rainmaker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/statistics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/synth.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/source/timecode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.969420 charidotella-0.9/command_line_tools/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/third_party/monaco.ttf.base64.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.957419 charidotella-0.9/command_line_tools/third_party/pontella/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.969420 charidotella-0.9/command_line_tools/third_party/pontella/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-28 12:38:48.000000 charidotella-0.9/command_line_tools/third_party/pontella/source/pontella.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.957419 charidotella-0.9/command_line_tools/third_party/sepia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.969420 charidotella-0.9/command_line_tools/third_party/sepia/source/
+-rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-04-28 12:38:49.000000 charidotella-0.9/command_line_tools/third_party/sepia/source/sepia.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-04-28 12:38:45.000000 charidotella-0.9/command_line_tools/third_party/stb_truetype.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.957419 charidotella-0.9/command_line_tools/third_party/tarsier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:39:27.969420 charidotella-0.9/command_line_tools/third_party/tarsier/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-28 12:38:52.000000 charidotella-0.9/command_line_tools/third_party/tarsier/source/replicate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 12:38:52.000000 charidotella-0.9/command_line_tools/third_party/tarsier/source/stitch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-28 12:38:45.000000 charidotella-0.9/configuration-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-28 12:38:45.000000 charidotella-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:39:27.969420 charidotella-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-28 12:38:45.000000 charidotella-0.9/setup.py
```

### Comparing `charidotella-0.8/MANIFEST.in` & `charidotella-0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/PKG-INFO` & `charidotella-0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charidotella
-Version: 0.8
+Version: 0.9
 Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
 Home-page: https://github.com/neuromorphicsystems/charidotella
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -19,39 +19,54 @@
 - [Contribute](#contribute)
 
 ## Dependencies
 
 -   **Debian / Ubuntu**
 
     ```sh
-    sudo apt install ffmpeg
+    sudo apt install ffmpeg python3 python3-pip vlc
     ```
 
 -   **macOS**
 
     1. Install Homebrew (https://brew.sh)
     2. Run in a terminal
         ```sh
-        brew install ffmpeg
+        brew install ffmpeg python3
         ```
 
 -   **Windows**
-    1. Install Chocolatey (https://chocolatey.org/)
-    2. Open Powershell as administrator and run
-        ```sh
-        choco install -y ffmpeg
-        ```
+
+    Run in an elevated Powershell (right-click > Run as Administrator)
+    ```powershell
+    winget install python3 --scope machine
+    winget install ffmpeg --scope machine
+    ```
 
 ## Get started
 
 1. Install the Python package
 
-    ```sh
-    python3 -m pip install charidotella
-    ```
+    -   **Debian / Ubuntu**
+        ```sh
+        sudo python3 -m pip install charidotella
+        ```
+
+    -   **macOS**
+        ```sh
+        python3 -m pip install charidotella
+        ```
+
+    -   **Windows**
+
+        Run in an elevated Powershell (right-click > Run as Administrator)
+        ```powershell
+        & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
+        ```
+
 
 2. Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
 
     ```txt
     my-wonderful-project
     └── recordings
         ├── file_1.es
```

### Comparing `charidotella-0.8/README.md` & `charidotella-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,39 +7,54 @@
 - [Contribute](#contribute)
 
 ## Dependencies
 
 -   **Debian / Ubuntu**
 
     ```sh
-    sudo apt install ffmpeg
+    sudo apt install ffmpeg python3 python3-pip vlc
     ```
 
 -   **macOS**
 
     1. Install Homebrew (https://brew.sh)
     2. Run in a terminal
         ```sh
-        brew install ffmpeg
+        brew install ffmpeg python3
         ```
 
 -   **Windows**
-    1. Install Chocolatey (https://chocolatey.org/)
-    2. Open Powershell as administrator and run
-        ```sh
-        choco install -y ffmpeg
-        ```
+
+    Run in an elevated Powershell (right-click > Run as Administrator)
+    ```powershell
+    winget install python3 --scope machine
+    winget install ffmpeg --scope machine
+    ```
 
 ## Get started
 
 1. Install the Python package
 
-    ```sh
-    python3 -m pip install charidotella
-    ```
+    -   **Debian / Ubuntu**
+        ```sh
+        sudo python3 -m pip install charidotella
+        ```
+
+    -   **macOS**
+        ```sh
+        python3 -m pip install charidotella
+        ```
+
+    -   **Windows**
+
+        Run in an elevated Powershell (right-click > Run as Administrator)
+        ```powershell
+        & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
+        ```
+
 
 2. Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
 
     ```txt
     my-wonderful-project
     └── recordings
         ├── file_1.es
```

### Comparing `charidotella-0.8/charidotella/__init__.py` & `charidotella-0.9/charidotella/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,20 +194,20 @@
                 )
             )
         ) as configuration_schema_file:
             return json.load(configuration_schema_file)
 
     def load_parameters(path: pathlib.Path):
         if path.is_file():
-            with open(path) as file:
+            with open(path, "r", encoding="utf-8") as file:
                 return toml.load(file)
         return None
 
     def save_parameters(path: pathlib.Path, parameters: dict[str, typing.Any]):
-        with open(path.with_suffix(".part"), "w") as file:
+        with open(path.with_suffix(".part"), "w", encoding="utf-8") as file:
             toml.dump(parameters, file)
         path.with_suffix(".part").rename(path)
 
     def compare_parameters(a: dict[str, typing.Any], b: dict[str, typing.Any]):
         return json.dumps(a, sort_keys=True, separators=(",", ":")) == json.dumps(
             b, sort_keys=True, separators=(",", ":")
         )
@@ -383,15 +383,17 @@
                         "event-rate-.+",
                         "wiggle-.+",
                         "video-real-time",
                     ],
                 }
             )
         with open(
-            utilities.with_suffix(configuration_path, ".part"), "w"
+            utilities.with_suffix(configuration_path, ".part"),
+            "w",
+            encoding="utf-8",
         ) as configuration_file:
             configuration_file.write("# output directory\n")
             toml.dump({"directory": "renders"}, configuration_file, encoder=Encoder())
             configuration_file.write(
                 "\n\n# filters configuration (filters are applied before tasks)\n\n"
             )
             toml.dump(
@@ -473,15 +475,15 @@
                 {
                     "tasks": {
                         "video-real-time": {
                             "type": "video",
                             "icon": "🎬",
                             "frametime": utilities.timestamp_to_timecode(20000),
                             "tau": utilities.timestamp_to_timecode(200000),
-                            "style": "cumulative",
+                            "style": "exponential",
                             "on_color": "#F4C20D",
                             "off_color": "#1E88E5",
                             "idle_color": "#191919",
                             "cumulative_ratio": 0.01,
                             "timecode": True,
                             "h264_crf": 15,
                             "ffmpeg": "ffmpeg",
@@ -642,26 +644,28 @@
             )
             toml.dump(
                 {"attachments": attachments},
                 configuration_file,
                 encoder=Encoder(),
             )
         with open(
-            utilities.with_suffix(configuration_path, ".part")
+            utilities.with_suffix(configuration_path, ".part"),
+            "r",
+            encoding="utf-8",
         ) as configuration_file:
             jsonschema.validate(
                 toml.load(configuration_file),
                 configuration_schema(),
             )
         utilities.with_suffix(configuration_path, ".part").rename(configuration_path)
         sys.exit(0)
 
     if args.command == "run":
         configuration_path = pathlib.Path(args.configuration).resolve()
-        with open(configuration_path) as configuration_file:
+        with open(configuration_path, "r", encoding="utf-8") as configuration_file:
             configuration = toml.load(configuration_file)
         jsonschema.validate(configuration, configuration_schema())
         if not "filters" in configuration:
             configuration["filters"] = {}
         if not "tasks" in configuration:
             configuration["tasks"] = {}
         if not "jobs" in configuration:
@@ -902,26 +906,26 @@
 
             if index < len(configuration["jobs"]) - 1:
                 sys.stdout.write("\n")
         sys.exit(0)
 
     if args.command == "resolve":
         configuration_path = pathlib.Path(args.configuration).resolve()
-        with open(configuration_path) as configuration_file:
+        with open(configuration_path, "r", encoding="utf-8") as configuration_file:
             configuration = toml.load(configuration_file)
         jsonschema.validate(configuration, configuration_schema())
         if not "filters" in configuration:
             configuration["filters"] = {}
         if not "tasks" in configuration:
             configuration["tasks"] = {}
         if not "jobs" in configuration:
             configuration["jobs"] = []
         if not "attachments" in configuration:
             configuration["attachments"] = []
         run_generators(configuration)
         jsonschema.validate(configuration, configuration_schema())
-        with open(pathlib.Path(args.output), "w") as output_file:
+        with open(pathlib.Path(args.output), "w", encoding="utf-8") as output_file:
             json.dump(configuration, output_file, indent=4)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `charidotella-0.8/charidotella/animals.py` & `charidotella-0.9/charidotella/animals.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/assets/configuration-schema.json` & `charidotella-0.9/charidotella/assets/configuration-schema.json`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/assets/es_to_frames` & `charidotella-0.9/charidotella/assets/es_to_frames`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/assets/event_rate` & `charidotella-0.9/charidotella/assets/event_rate`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/assets/size` & `charidotella-0.9/charidotella/assets/size`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/charidotella_extension_placeholder.c` & `charidotella-0.9/charidotella/charidotella_extension_placeholder.c`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/filters/arbiter_saturation.py` & `charidotella-0.9/charidotella/filters/arbiter_saturation.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/filters/default.py` & `charidotella-0.9/charidotella/filters/default.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/filters/hot_pixels.py` & `charidotella-0.9/charidotella/filters/hot_pixels.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/filters/transpose.py` & `charidotella-0.9/charidotella/filters/transpose.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/tasks/colourtime.py` & `charidotella-0.9/charidotella/tasks/colourtime.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/tasks/event_rate.py` & `charidotella-0.9/charidotella/tasks/event_rate.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/tasks/video.py` & `charidotella-0.9/charidotella/tasks/video.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/tasks/wiggle.py` & `charidotella-0.9/charidotella/tasks/wiggle.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella/utilities.py` & `charidotella-0.9/charidotella/utilities.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/charidotella.egg-info/PKG-INFO` & `charidotella-0.9/charidotella.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charidotella
-Version: 0.8
+Version: 0.9
 Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
 Home-page: https://github.com/neuromorphicsystems/charidotella
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -19,39 +19,54 @@
 - [Contribute](#contribute)
 
 ## Dependencies
 
 -   **Debian / Ubuntu**
 
     ```sh
-    sudo apt install ffmpeg
+    sudo apt install ffmpeg python3 python3-pip vlc
     ```
 
 -   **macOS**
 
     1. Install Homebrew (https://brew.sh)
     2. Run in a terminal
         ```sh
-        brew install ffmpeg
+        brew install ffmpeg python3
         ```
 
 -   **Windows**
-    1. Install Chocolatey (https://chocolatey.org/)
-    2. Open Powershell as administrator and run
-        ```sh
-        choco install -y ffmpeg
-        ```
+
+    Run in an elevated Powershell (right-click > Run as Administrator)
+    ```powershell
+    winget install python3 --scope machine
+    winget install ffmpeg --scope machine
+    ```
 
 ## Get started
 
 1. Install the Python package
 
-    ```sh
-    python3 -m pip install charidotella
-    ```
+    -   **Debian / Ubuntu**
+        ```sh
+        sudo python3 -m pip install charidotella
+        ```
+
+    -   **macOS**
+        ```sh
+        python3 -m pip install charidotella
+        ```
+
+    -   **Windows**
+
+        Run in an elevated Powershell (right-click > Run as Administrator)
+        ```powershell
+        & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
+        ```
+
 
 2. Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
 
     ```txt
     my-wonderful-project
     └── recordings
         ├── file_1.es
```

### Comparing `charidotella-0.8/charidotella.egg-info/SOURCES.txt` & `charidotella-0.9/charidotella.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/premake4.lua` & `charidotella-0.9/command_line_tools/premake4.lua`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/crop.cpp` & `charidotella-0.9/command_line_tools/source/crop.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/cut.cpp` & `charidotella-0.9/command_line_tools/source/cut.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/dat.hpp` & `charidotella-0.9/command_line_tools/source/dat.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/dat_to_es.cpp` & `charidotella-0.9/command_line_tools/source/dat_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/es_to_csv.cpp` & `charidotella-0.9/command_line_tools/source/es_to_csv.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/es_to_frames.cpp` & `charidotella-0.9/command_line_tools/source/es_to_frames.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/es_to_ply.cpp` & `charidotella-0.9/command_line_tools/source/es_to_ply.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/event_rate.cpp` & `charidotella-0.9/command_line_tools/source/event_rate.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/evt3.hpp` & `charidotella-0.9/command_line_tools/source/evt3.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/evt3_to_es.cpp` & `charidotella-0.9/command_line_tools/source/evt3_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/font.hpp` & `charidotella-0.9/command_line_tools/source/font.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/html.hpp` & `charidotella-0.9/command_line_tools/source/html.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/rainbow.cpp` & `charidotella-0.9/command_line_tools/source/rainbow.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/rainmaker.cpp` & `charidotella-0.9/command_line_tools/source/rainmaker.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/size.cpp` & `charidotella-0.9/command_line_tools/source/size.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/statistics.cpp` & `charidotella-0.9/command_line_tools/source/statistics.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/synth.cpp` & `charidotella-0.9/command_line_tools/source/synth.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/source/timecode.hpp` & `charidotella-0.9/command_line_tools/source/timecode.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/third_party/monaco.ttf.base64.hpp` & `charidotella-0.9/command_line_tools/third_party/monaco.ttf.base64.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/third_party/pontella/source/pontella.hpp` & `charidotella-0.9/command_line_tools/third_party/pontella/source/pontella.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/third_party/sepia/source/sepia.hpp` & `charidotella-0.9/command_line_tools/third_party/sepia/source/sepia.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/third_party/stb_truetype.hpp` & `charidotella-0.9/command_line_tools/third_party/stb_truetype.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/third_party/tarsier/source/replicate.hpp` & `charidotella-0.9/command_line_tools/third_party/tarsier/source/replicate.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/command_line_tools/third_party/tarsier/source/stitch.hpp` & `charidotella-0.9/command_line_tools/third_party/tarsier/source/stitch.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/configuration-schema.json` & `charidotella-0.9/configuration-schema.json`

 * *Files identical despite different names*

### Comparing `charidotella-0.8/setup.py` & `charidotella-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         content = "\n".join(manifest_lines)
         manifest.write(f"{content}\n")
 
 exec(open(dirname / "charidotella" / "version.py").read())
 
 setuptools.setup(
     name="charidotella",
-    version=__version__, # type: ignore
+    version=__version__,  # type: ignore
     url="https://github.com/neuromorphicsystems/charidotella",
     author="Alexandre Marcireau",
     author_email="alexandre.marcireau@gmail.com",
     description="Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
@@ -111,14 +111,15 @@
     package_data={"": ["charidotella/assets/*"]},
     install_requires=[
         "colourtime",
         "coolname",
         "event_stream",
         "jsonschema",
         "matplotlib",
+        "pillow>=9.4",
         "scipy",
         "toml",
     ],
     ext_modules=[
         setuptools.extension.Extension(
             "charidotella_extension_placeholder",
             language="cpp",
```

