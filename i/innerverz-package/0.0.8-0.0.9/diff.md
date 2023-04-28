# Comparing `tmp/innerverz_package-0.0.8.tar.gz` & `tmp/innerverz_package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz_package-0.0.8.tar", last modified: Thu Apr 27 08:41:46 2023, max compression
+gzip compressed data, was "innerverz_package-0.0.9.tar", last modified: Thu Apr 27 09:02:05 2023, max compression
```

## Comparing `innerverz_package-0.0.8.tar` & `innerverz_package-0.0.9.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.382532 innerverz_package-0.0.8/
--rw-r--r--   0 compu     (1000) compu     (1000)     1073 2023-01-27 06:12:58.000000 innerverz_package-0.0.8/LICENSE.txt
--rw-rw-r--   0 compu     (1000) compu     (1000)      213 2023-04-27 08:41:46.382532 innerverz_package-0.0.8/PKG-INFO
--rw-r--r--   0 compu     (1000) compu     (1000)       10 2023-01-27 06:13:12.000000 innerverz_package-0.0.8/README.md
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/
--rw-rw-r--   0 compu     (1000) compu     (1000)      215 2023-04-27 08:18:59.000000 innerverz_package-0.0.8/innerverz_package/__init__.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/deblurrer/
--rwxr-xr-x   0 compu     (1000) compu     (1000)       27 2023-04-24 11:46:39.000000 innerverz_package-0.0.8/innerverz_package/deblurrer/__init__.py
--rwxr-xr-x   0 compu     (1000) compu     (1000)     2113 2023-04-26 12:57:45.000000 innerverz_package-0.0.8/innerverz_package/deblurrer/main.py
--rwxr-xr-x   0 compu     (1000) compu     (1000)     3609 2023-04-24 11:46:39.000000 innerverz_package-0.0.8/innerverz_package/deblurrer/nets.py
--rwxr-xr-x   0 compu     (1000) compu     (1000)     1072 2023-04-24 11:46:37.000000 innerverz_package-0.0.8/innerverz_package/deblurrer/test.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/deep3dmm/
--rwxrwxr-x   0 compu     (1000) compu     (1000)       27 2023-04-26 07:42:20.000000 innerverz_package-0.0.8/innerverz_package/deep3dmm/__init__.py
--rwxrwxr-x   0 compu     (1000) compu     (1000)     2667 2023-04-26 12:03:39.000000 innerverz_package-0.0.8/innerverz_package/deep3dmm/main.py
--rwxrwxr-x   0 compu     (1000) compu     (1000)    25860 2023-04-26 11:57:51.000000 innerverz_package-0.0.8/innerverz_package/deep3dmm/nets.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/face_alignment/
--rw-rw-r--   0 compu     (1000) compu     (1000)       96 2023-04-26 07:00:17.000000 innerverz_package-0.0.8/innerverz_package/face_alignment/__init__.py
--rw-rw-r--   0 compu     (1000) compu     (1000)     6646 2023-04-26 03:08:16.000000 innerverz_package-0.0.8/innerverz_package/face_alignment/graphic_utils.py
--rw-rw-r--   0 compu     (1000) compu     (1000)     5118 2023-04-26 07:01:30.000000 innerverz_package-0.0.8/innerverz_package/face_alignment/landmark.py
--rw-rw-r--   0 compu     (1000) compu     (1000)     4441 2023-04-26 11:54:14.000000 innerverz_package-0.0.8/innerverz_package/face_alignment/main.py
--rw-rw-r--   0 compu     (1000) compu     (1000)    12774 2023-04-26 06:39:54.000000 innerverz_package-0.0.8/innerverz_package/face_alignment/retina_face.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/face_alignment/utils/
--rw-rw-r--   0 compu     (1000) compu     (1000)       49 2023-04-27 08:37:38.000000 innerverz_package-0.0.8/innerverz_package/face_alignment/utils/__init__.py
--rw-rw-r--   0 compu     (1000) compu     (1000)     3354 2023-04-26 03:08:16.000000 innerverz_package-0.0.8/innerverz_package/face_alignment/utils/face_align.py
--rw-rw-r--   0 compu     (1000) compu     (1000)     4933 2023-04-26 05:31:45.000000 innerverz_package-0.0.8/innerverz_package/face_alignment/utils/transform.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/face_parser/
--rw-r--r--   0 compu     (1000) compu     (1000)       59 2023-04-26 05:18:02.000000 innerverz_package-0.0.8/innerverz_package/face_parser/__init__.py
--rw-r--r--   0 compu     (1000) compu     (1000)     4117 2023-04-26 13:12:02.000000 innerverz_package-0.0.8/innerverz_package/face_parser/main.py
--rw-r--r--   0 compu     (1000) compu     (1000)     8472 2023-04-26 05:18:02.000000 innerverz_package-0.0.8/innerverz_package/face_parser/model.py
--rw-r--r--   0 compu     (1000) compu     (1000)     3648 2023-04-26 05:18:02.000000 innerverz_package-0.0.8/innerverz_package/face_parser/resnet.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/face_parser/utils/
--rw-r--r--   0 compu     (1000) compu     (1000)      109 2023-04-26 05:18:02.000000 innerverz_package-0.0.8/innerverz_package/face_parser/utils/__init__.py
--rw-r--r--   0 compu     (1000) compu     (1000)      837 2023-04-26 05:18:02.000000 innerverz_package-0.0.8/innerverz_package/face_parser/utils/mask_utils.py
--rw-r--r--   0 compu     (1000) compu     (1000)     1509 2023-04-26 05:18:02.000000 innerverz_package-0.0.8/innerverz_package/face_parser/utils/utils.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/head_color_transfer/
--rw-r--r--   0 compu     (1000) compu     (1000)       49 2023-04-27 08:36:58.000000 innerverz_package-0.0.8/innerverz_package/head_color_transfer/__init__.py
--rw-r--r--   0 compu     (1000) compu     (1000)     3885 2023-04-27 06:21:48.000000 innerverz_package-0.0.8/innerverz_package/head_color_transfer/main.py
--rw-r--r--   0 compu     (1000) compu     (1000)     5848 2023-04-27 05:04:38.000000 innerverz_package-0.0.8/innerverz_package/head_color_transfer/nets.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/
--rw-r--r--   0 compu     (1000) compu     (1000)      100 2023-04-26 13:01:56.000000 innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 compu     (1000) compu     (1000)     7018 2023-04-26 13:01:56.000000 innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 compu     (1000) compu     (1000)     3642 2023-04-26 13:01:56.000000 innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 compu     (1000) compu     (1000)     3788 2023-04-26 13:01:56.000000 innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 compu     (1000) compu     (1000)     9366 2023-04-26 13:01:56.000000 innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/warp_net.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/id_extractor/
--rw-r--r--   0 compu     (1000) compu     (1000)       29 2023-04-27 05:19:43.000000 innerverz_package-0.0.8/innerverz_package/id_extractor/__init__.py
--rw-r--r--   0 compu     (1000) compu     (1000)     2359 2023-04-27 05:44:11.000000 innerverz_package-0.0.8/innerverz_package/id_extractor/main.py
--rw-r--r--   0 compu     (1000) compu     (1000)     5192 2023-04-27 05:19:43.000000 innerverz_package-0.0.8/innerverz_package/id_extractor/nets.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package/upsampler/
--rw-r--r--   0 compu     (1000) compu     (1000)       28 2023-04-26 10:56:36.000000 innerverz_package-0.0.8/innerverz_package/upsampler/__init__.py
--rwxr-xr-x   0 compu     (1000) compu     (1000)     2231 2023-04-26 12:47:02.000000 innerverz_package-0.0.8/innerverz_package/upsampler/main.py
--rwxr-xr-x   0 compu     (1000) compu     (1000)    36818 2023-04-26 10:58:23.000000 innerverz_package-0.0.8/innerverz_package/upsampler/nets.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.382532 innerverz_package-0.0.8/innerverz_package/utils/
--rw-r--r--   0 compu     (1000) compu     (1000)       88 2023-04-26 05:24:52.000000 innerverz_package-0.0.8/innerverz_package/utils/__init__.py
--rw-r--r--   0 compu     (1000) compu     (1000)     1230 2023-04-26 06:34:23.000000 innerverz_package-0.0.8/innerverz_package/utils/download.py
--rw-r--r--   0 compu     (1000) compu     (1000)     1009 2023-02-06 03:04:22.000000 innerverz_package-0.0.8/innerverz_package/utils/input.py
--rw-rw-r--   0 compu     (1000) compu     (1000)    11916 2023-04-26 12:25:30.000000 innerverz_package-0.0.8/innerverz_package/utils/utils.py
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 08:41:46.378532 innerverz_package-0.0.8/innerverz_package.egg-info/
--rw-rw-r--   0 compu     (1000) compu     (1000)      213 2023-04-27 08:41:46.000000 innerverz_package-0.0.8/innerverz_package.egg-info/PKG-INFO
--rw-rw-r--   0 compu     (1000) compu     (1000)     2048 2023-04-27 08:41:46.000000 innerverz_package-0.0.8/innerverz_package.egg-info/SOURCES.txt
--rw-rw-r--   0 compu     (1000) compu     (1000)        1 2023-04-27 08:41:46.000000 innerverz_package-0.0.8/innerverz_package.egg-info/dependency_links.txt
--rw-rw-r--   0 compu     (1000) compu     (1000)       50 2023-04-27 08:41:46.000000 innerverz_package-0.0.8/innerverz_package.egg-info/requires.txt
--rw-rw-r--   0 compu     (1000) compu     (1000)       18 2023-04-27 08:41:46.000000 innerverz_package-0.0.8/innerverz_package.egg-info/top_level.txt
--rw-r--r--   0 compu     (1000) compu     (1000)       89 2023-01-27 04:47:26.000000 innerverz_package-0.0.8/pyproject.toml
--rw-r--r--   0 compu     (1000) compu     (1000)       38 2023-04-27 08:41:46.382532 innerverz_package-0.0.8/setup.cfg
--rw-r--r--   0 compu     (1000) compu     (1000)      789 2023-04-27 08:40:24.000000 innerverz_package-0.0.8/setup.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.466119 innerverz_package-0.0.9/
+-rw-r--r--   0 compu     (1000) compu     (1000)     1073 2023-01-27 06:12:58.000000 innerverz_package-0.0.9/LICENSE.txt
+-rw-rw-r--   0 compu     (1000) compu     (1000)      213 2023-04-27 09:02:05.466119 innerverz_package-0.0.9/PKG-INFO
+-rw-r--r--   0 compu     (1000) compu     (1000)       10 2023-01-27 06:13:12.000000 innerverz_package-0.0.9/README.md
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/
+-rw-rw-r--   0 compu     (1000) compu     (1000)      215 2023-04-27 08:18:59.000000 innerverz_package-0.0.9/innerverz_package/__init__.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/deblurrer/
+-rwxr-xr-x   0 compu     (1000) compu     (1000)       27 2023-04-24 11:46:39.000000 innerverz_package-0.0.9/innerverz_package/deblurrer/__init__.py
+-rwxr-xr-x   0 compu     (1000) compu     (1000)     2113 2023-04-26 12:57:45.000000 innerverz_package-0.0.9/innerverz_package/deblurrer/main.py
+-rwxr-xr-x   0 compu     (1000) compu     (1000)     3609 2023-04-24 11:46:39.000000 innerverz_package-0.0.9/innerverz_package/deblurrer/nets.py
+-rwxr-xr-x   0 compu     (1000) compu     (1000)     1072 2023-04-24 11:46:37.000000 innerverz_package-0.0.9/innerverz_package/deblurrer/test.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/deep3dmm/
+-rwxrwxr-x   0 compu     (1000) compu     (1000)       27 2023-04-26 07:42:20.000000 innerverz_package-0.0.9/innerverz_package/deep3dmm/__init__.py
+-rwxrwxr-x   0 compu     (1000) compu     (1000)     2667 2023-04-26 12:03:39.000000 innerverz_package-0.0.9/innerverz_package/deep3dmm/main.py
+-rwxrwxr-x   0 compu     (1000) compu     (1000)    25860 2023-04-26 11:57:51.000000 innerverz_package-0.0.9/innerverz_package/deep3dmm/nets.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/face_alignment/
+-rw-rw-r--   0 compu     (1000) compu     (1000)      125 2023-04-27 09:00:32.000000 innerverz_package-0.0.9/innerverz_package/face_alignment/__init__.py
+-rw-rw-r--   0 compu     (1000) compu     (1000)     6646 2023-04-26 03:08:16.000000 innerverz_package-0.0.9/innerverz_package/face_alignment/graphic_utils.py
+-rw-rw-r--   0 compu     (1000) compu     (1000)     5118 2023-04-26 07:01:30.000000 innerverz_package-0.0.9/innerverz_package/face_alignment/landmark.py
+-rw-rw-r--   0 compu     (1000) compu     (1000)     4441 2023-04-26 11:54:14.000000 innerverz_package-0.0.9/innerverz_package/face_alignment/main.py
+-rw-rw-r--   0 compu     (1000) compu     (1000)    12774 2023-04-26 06:39:54.000000 innerverz_package-0.0.9/innerverz_package/face_alignment/retina_face.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/face_alignment/utils/
+-rw-rw-r--   0 compu     (1000) compu     (1000)       49 2023-04-27 08:37:38.000000 innerverz_package-0.0.9/innerverz_package/face_alignment/utils/__init__.py
+-rw-rw-r--   0 compu     (1000) compu     (1000)     3354 2023-04-26 03:08:16.000000 innerverz_package-0.0.9/innerverz_package/face_alignment/utils/face_align.py
+-rw-rw-r--   0 compu     (1000) compu     (1000)     4933 2023-04-26 05:31:45.000000 innerverz_package-0.0.9/innerverz_package/face_alignment/utils/transform.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/face_parser/
+-rw-r--r--   0 compu     (1000) compu     (1000)       59 2023-04-26 05:18:02.000000 innerverz_package-0.0.9/innerverz_package/face_parser/__init__.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     4117 2023-04-26 13:12:02.000000 innerverz_package-0.0.9/innerverz_package/face_parser/main.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     8472 2023-04-26 05:18:02.000000 innerverz_package-0.0.9/innerverz_package/face_parser/model.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     3648 2023-04-26 05:18:02.000000 innerverz_package-0.0.9/innerverz_package/face_parser/resnet.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/face_parser/utils/
+-rw-r--r--   0 compu     (1000) compu     (1000)      109 2023-04-26 05:18:02.000000 innerverz_package-0.0.9/innerverz_package/face_parser/utils/__init__.py
+-rw-r--r--   0 compu     (1000) compu     (1000)      837 2023-04-26 05:18:02.000000 innerverz_package-0.0.9/innerverz_package/face_parser/utils/mask_utils.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     1509 2023-04-26 05:18:02.000000 innerverz_package-0.0.9/innerverz_package/face_parser/utils/utils.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/head_color_transfer/
+-rw-r--r--   0 compu     (1000) compu     (1000)       49 2023-04-27 08:36:58.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/__init__.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     3885 2023-04-27 06:21:48.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/main.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     5848 2023-04-27 05:04:38.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/nets.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/
+-rw-r--r--   0 compu     (1000) compu     (1000)      100 2023-04-26 13:01:56.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     7018 2023-04-26 13:01:56.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     3642 2023-04-26 13:01:56.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     3788 2023-04-26 13:01:56.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     9366 2023-04-26 13:01:56.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/warp_net.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.466119 innerverz_package-0.0.9/innerverz_package/head_color_transfer/utils/
+-rw-rw-r--   0 compu     (1000) compu     (1000)       20 2023-04-27 09:01:45.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/utils/__init__.py
+-rw-r--r--   0 compu     (1000) compu     (1000)      788 2023-04-27 03:12:44.000000 innerverz_package-0.0.9/innerverz_package/head_color_transfer/utils/utils.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.466119 innerverz_package-0.0.9/innerverz_package/id_extractor/
+-rw-r--r--   0 compu     (1000) compu     (1000)       29 2023-04-27 05:19:43.000000 innerverz_package-0.0.9/innerverz_package/id_extractor/__init__.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     2359 2023-04-27 05:44:11.000000 innerverz_package-0.0.9/innerverz_package/id_extractor/main.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     5192 2023-04-27 05:19:43.000000 innerverz_package-0.0.9/innerverz_package/id_extractor/nets.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.466119 innerverz_package-0.0.9/innerverz_package/upsampler/
+-rw-r--r--   0 compu     (1000) compu     (1000)       28 2023-04-26 10:56:36.000000 innerverz_package-0.0.9/innerverz_package/upsampler/__init__.py
+-rwxr-xr-x   0 compu     (1000) compu     (1000)     2231 2023-04-26 12:47:02.000000 innerverz_package-0.0.9/innerverz_package/upsampler/main.py
+-rwxr-xr-x   0 compu     (1000) compu     (1000)    36818 2023-04-26 10:58:23.000000 innerverz_package-0.0.9/innerverz_package/upsampler/nets.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.466119 innerverz_package-0.0.9/innerverz_package/utils/
+-rw-r--r--   0 compu     (1000) compu     (1000)       88 2023-04-26 05:24:52.000000 innerverz_package-0.0.9/innerverz_package/utils/__init__.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     1230 2023-04-26 06:34:23.000000 innerverz_package-0.0.9/innerverz_package/utils/download.py
+-rw-r--r--   0 compu     (1000) compu     (1000)     1009 2023-02-06 03:04:22.000000 innerverz_package-0.0.9/innerverz_package/utils/input.py
+-rw-rw-r--   0 compu     (1000) compu     (1000)    11916 2023-04-26 12:25:30.000000 innerverz_package-0.0.9/innerverz_package/utils/utils.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 09:02:05.462119 innerverz_package-0.0.9/innerverz_package.egg-info/
+-rw-rw-r--   0 compu     (1000) compu     (1000)      213 2023-04-27 09:02:05.000000 innerverz_package-0.0.9/innerverz_package.egg-info/PKG-INFO
+-rw-rw-r--   0 compu     (1000) compu     (1000)     2157 2023-04-27 09:02:05.000000 innerverz_package-0.0.9/innerverz_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 compu     (1000) compu     (1000)        1 2023-04-27 09:02:05.000000 innerverz_package-0.0.9/innerverz_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 compu     (1000) compu     (1000)       50 2023-04-27 09:02:05.000000 innerverz_package-0.0.9/innerverz_package.egg-info/requires.txt
+-rw-rw-r--   0 compu     (1000) compu     (1000)       18 2023-04-27 09:02:05.000000 innerverz_package-0.0.9/innerverz_package.egg-info/top_level.txt
+-rw-r--r--   0 compu     (1000) compu     (1000)       89 2023-01-27 04:47:26.000000 innerverz_package-0.0.9/pyproject.toml
+-rw-r--r--   0 compu     (1000) compu     (1000)       38 2023-04-27 09:02:05.466119 innerverz_package-0.0.9/setup.cfg
+-rw-r--r--   0 compu     (1000) compu     (1000)      789 2023-04-27 09:02:03.000000 innerverz_package-0.0.9/setup.py
```

### Comparing `innerverz_package-0.0.8/LICENSE.txt` & `innerverz_package-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/deblurrer/main.py` & `innerverz_package-0.0.9/innerverz_package/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/deblurrer/nets.py` & `innerverz_package-0.0.9/innerverz_package/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/deblurrer/test.py` & `innerverz_package-0.0.9/innerverz_package/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/deep3dmm/main.py` & `innerverz_package-0.0.9/innerverz_package/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/deep3dmm/nets.py` & `innerverz_package-0.0.9/innerverz_package/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_alignment/graphic_utils.py` & `innerverz_package-0.0.9/innerverz_package/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_alignment/landmark.py` & `innerverz_package-0.0.9/innerverz_package/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_alignment/main.py` & `innerverz_package-0.0.9/innerverz_package/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_alignment/retina_face.py` & `innerverz_package-0.0.9/innerverz_package/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_alignment/utils/face_align.py` & `innerverz_package-0.0.9/innerverz_package/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_alignment/utils/transform.py` & `innerverz_package-0.0.9/innerverz_package/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_parser/main.py` & `innerverz_package-0.0.9/innerverz_package/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_parser/model.py` & `innerverz_package-0.0.9/innerverz_package/face_parser/model.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_parser/resnet.py` & `innerverz_package-0.0.9/innerverz_package/face_parser/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_parser/utils/mask_utils.py` & `innerverz_package-0.0.9/innerverz_package/face_parser/utils/mask_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/face_parser/utils/utils.py` & `innerverz_package-0.0.9/innerverz_package/face_parser/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/head_color_transfer/main.py` & `innerverz_package-0.0.9/innerverz_package/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/head_color_transfer/nets.py` & `innerverz_package-0.0.9/innerverz_package/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/blend_net.py` & `innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/discriminator.py` & `innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/head_color_transfer/sub_nets/warp_net.py` & `innerverz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/id_extractor/main.py` & `innerverz_package-0.0.9/innerverz_package/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/id_extractor/nets.py` & `innerverz_package-0.0.9/innerverz_package/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/upsampler/main.py` & `innerverz_package-0.0.9/innerverz_package/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/upsampler/nets.py` & `innerverz_package-0.0.9/innerverz_package/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/utils/download.py` & `innerverz_package-0.0.9/innerverz_package/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/utils/input.py` & `innerverz_package-0.0.9/innerverz_package/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package/utils/utils.py` & `innerverz_package-0.0.9/innerverz_package/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.8/innerverz_package.egg-info/SOURCES.txt` & `innerverz_package-0.0.9/innerverz_package.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 innerverz_package/head_color_transfer/main.py
 innerverz_package/head_color_transfer/nets.py
 innerverz_package/head_color_transfer/sub_nets/__init__.py
 innerverz_package/head_color_transfer/sub_nets/blend_net.py
 innerverz_package/head_color_transfer/sub_nets/discriminator.py
 innerverz_package/head_color_transfer/sub_nets/vgg19_net.py
 innerverz_package/head_color_transfer/sub_nets/warp_net.py
+innerverz_package/head_color_transfer/utils/__init__.py
+innerverz_package/head_color_transfer/utils/utils.py
 innerverz_package/id_extractor/__init__.py
 innerverz_package/id_extractor/main.py
 innerverz_package/id_extractor/nets.py
 innerverz_package/upsampler/__init__.py
 innerverz_package/upsampler/main.py
 innerverz_package/upsampler/nets.py
 innerverz_package/utils/__init__.py
```

### Comparing `innerverz_package-0.0.8/setup.py` & `innerverz_package-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz_package",
-    version="0.0.8",
+    version="0.0.9",
     author="Innerverz-by.JJY",
     author_email="pensee0.0a@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

