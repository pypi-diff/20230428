# Comparing `tmp/movia-1.0.0b3.tar.gz` & `tmp/movia-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movia-1.0.0b3.tar", last modified: Fri Apr 28 13:17:47 2023, max compression
+gzip compressed data, was "movia-1.0a1.tar", last modified: Mon Mar 13 10:04:13 2023, max compression
```

## Comparing `movia-1.0.0b3.tar` & `movia-1.0a1.tar`

### file list

```diff
@@ -1,168 +1,114 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.336669 movia-1.0.0b3/
--rw-------   0 robin     (1000) robin     (1000)    20781 2023-04-26 15:48:49.000000 movia-1.0.0b3/.pylintrc
--rw-r--r--   0 robin     (1000) robin     (1000)    34519 2023-03-28 15:30:25.000000 movia-1.0.0b3/LICENSE
--rw-rw-r--   0 robin     (1000) robin     (1000)     4819 2023-04-28 13:17:47.336669 movia-1.0.0b3/PKG-INFO
--rw-------   0 robin     (1000) robin     (1000)     3252 2023-04-25 10:51:28.000000 movia-1.0.0b3/README.rst
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.516660 movia-1.0.0b3/movia/
--rw-------   0 robin     (1000) robin     (1000)      117 2023-04-25 10:38:13.000000 movia-1.0.0b3/movia/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1126 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/__main__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.536660 movia-1.0.0b3/movia/core/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.540660 movia-1.0.0b3/movia/core/analysis/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/analysis/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1709 2023-04-11 09:32:19.000000 movia-1.0.0b3/movia/core/analysis/_helper_properties.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.564660 movia-1.0.0b3/movia/core/analysis/audio/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-04-10 08:12:25.000000 movia-1.0.0b3/movia/core/analysis/audio/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.608661 movia-1.0.0b3/movia/core/analysis/audio/properties/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-04-10 08:13:07.000000 movia-1.0.0b3/movia/core/analysis/audio/properties/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2600 2023-04-10 23:10:03.000000 movia-1.0.0b3/movia/core/analysis/audio/properties/duration.py
--rw-------   0 robin     (1000) robin     (1000)    22966 2023-04-11 15:47:59.000000 movia-1.0.0b3/movia/core/analysis/stream.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.620661 movia-1.0.0b3/movia/core/analysis/video/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/analysis/video/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.640661 movia-1.0.0b3/movia/core/analysis/video/properties/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/analysis/video/properties/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     5624 2023-04-11 09:26:12.000000 movia-1.0.0b3/movia/core/analysis/video/properties/duration.py
--rw-------   0 robin     (1000) robin     (1000)     5251 2023-04-11 09:46:47.000000 movia-1.0.0b3/movia/core/analysis/video/properties/nb_frames.py
--rw-------   0 robin     (1000) robin     (1000)     3444 2023-04-11 09:47:14.000000 movia-1.0.0b3/movia/core/analysis/video/properties/rate.py
--rw-------   0 robin     (1000) robin     (1000)     7639 2023-04-11 11:11:49.000000 movia-1.0.0b3/movia/core/analysis/video/properties/timestamps.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.732662 movia-1.0.0b3/movia/core/classes/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/classes/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1302 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/classes/container.py
--rw-------   0 robin     (1000) robin     (1000)      965 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/classes/filter.py
--rw-------   0 robin     (1000) robin     (1000)     3601 2023-04-14 09:35:56.000000 movia-1.0.0b3/movia/core/classes/frame.py
--rw-------   0 robin     (1000) robin     (1000)     4785 2023-04-09 23:06:23.000000 movia-1.0.0b3/movia/core/classes/frame_audio.py
--rw-------   0 robin     (1000) robin     (1000)    10984 2023-04-19 09:38:57.000000 movia-1.0.0b3/movia/core/classes/frame_video.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1344 2023-04-28 10:47:52.000000 movia-1.0.0b3/movia/core/classes/meta_filter.py
--rw-------   0 robin     (1000) robin     (1000)     4228 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/classes/node.py
--rw-------   0 robin     (1000) robin     (1000)     6453 2023-04-28 10:45:39.000000 movia-1.0.0b3/movia/core/classes/stream.py
--rw-------   0 robin     (1000) robin     (1000)     4712 2023-04-27 16:12:30.000000 movia-1.0.0b3/movia/core/classes/stream_audio.py
--rw-------   0 robin     (1000) robin     (1000)     4679 2023-04-27 09:05:19.000000 movia-1.0.0b3/movia/core/classes/stream_video.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.776662 movia-1.0.0b3/movia/core/compilation/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/compilation/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.820663 movia-1.0.0b3/movia/core/compilation/export/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/compilation/export/__init__.py
--rw-------   0 robin     (1000) robin     (1000)    28855 2023-03-29 17:43:40.000000 movia-1.0.0b3/movia/core/compilation/export/compatibility.py
--rw-------   0 robin     (1000) robin     (1000)     4362 2023-04-28 10:15:33.000000 movia-1.0.0b3/movia/core/compilation/export/default.py
--rw-------   0 robin     (1000) robin     (1000)      653 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/compilation/export/encodec.py
--rw-------   0 robin     (1000) robin     (1000)      280 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/compilation/export/muxer.py
--rw-------   0 robin     (1000) robin     (1000)      986 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/compilation/export/rate_audio.py
--rw-------   0 robin     (1000) robin     (1000)     1124 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/compilation/export/rate_video.py
--rw-------   0 robin     (1000) robin     (1000)    17036 2023-04-28 07:39:21.000000 movia-1.0.0b3/movia/core/compilation/graph_to_ast.py
--rw-------   0 robin     (1000) robin     (1000)     2823 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/compilation/graph_to_json.py
--rw-------   0 robin     (1000) robin     (1000)     7839 2023-04-28 10:17:24.000000 movia-1.0.0b3/movia/core/compilation/graph_to_tree.py
--rw-------   0 robin     (1000) robin     (1000)     3934 2023-04-26 07:42:01.000000 movia-1.0.0b3/movia/core/compilation/json_to_graph.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    18891 2023-04-27 05:58:58.000000 movia-1.0.0b3/movia/core/compilation/sympy_to_torch.py
--rw-------   0 robin     (1000) robin     (1000)     5664 2023-04-28 10:47:43.000000 movia-1.0.0b3/movia/core/compilation/tree_to_graph.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.824663 movia-1.0.0b3/movia/core/edit/
--rw-------   0 robin     (1000) robin     (1000)      216 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/edit/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.848663 movia-1.0.0b3/movia/core/edit/operation/
--rw-------   0 robin     (1000) robin     (1000)      158 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/edit/operation/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     2362 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/edit/operation/add.py
--rw-------   0 robin     (1000) robin     (1000)    22507 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/edit/operation/remove.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.880664 movia-1.0.0b3/movia/core/edit/resource_estimation/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/edit/resource_estimation/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.900664 movia-1.0.0b3/movia/core/edit/simplify/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/edit/simplify/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1278 2023-04-10 16:50:52.000000 movia-1.0.0b3/movia/core/exceptions.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.904664 movia-1.0.0b3/movia/core/filters/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/filters/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.000665 movia-1.0.0b3/movia/core/filters/basic/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/filters/basic/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    12970 2023-04-27 15:20:10.000000 movia-1.0.0b3/movia/core/filters/basic/add.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2657 2023-04-27 15:23:24.000000 movia-1.0.0b3/movia/core/filters/basic/chain.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     9816 2023-04-27 17:34:43.000000 movia-1.0.0b3/movia/core/filters/basic/cut.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1497 2023-04-27 13:24:23.000000 movia-1.0.0b3/movia/core/filters/basic/identity.py
--rw-------   0 robin     (1000) robin     (1000)     4372 2023-04-27 09:21:46.000000 movia-1.0.0b3/movia/core/filters/basic/translate.py
--rw-------   0 robin     (1000) robin     (1000)     3292 2023-04-27 14:42:30.000000 movia-1.0.0b3/movia/core/filters/basic/truncate.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.004665 movia-1.0.0b3/movia/core/generation/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/generation/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.008665 movia-1.0.0b3/movia/core/generation/audio/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/generation/audio/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     2171 2023-04-05 17:17:40.000000 movia-1.0.0b3/movia/core/generation/audio/empty.py
--rw-------   0 robin     (1000) robin     (1000)     9707 2023-04-09 22:12:45.000000 movia-1.0.0b3/movia/core/generation/audio/noise.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.028665 movia-1.0.0b3/movia/core/generation/video/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/generation/video/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     2294 2023-04-17 10:12:00.000000 movia-1.0.0b3/movia/core/generation/video/empty.py
--rw-------   0 robin     (1000) robin     (1000)    10361 2023-04-27 06:44:07.000000 movia-1.0.0b3/movia/core/generation/video/equation.py
--rw-------   0 robin     (1000) robin     (1000)     5387 2023-04-25 08:57:19.000000 movia-1.0.0b3/movia/core/generation/video/noise.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.076666 movia-1.0.0b3/movia/core/io/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/io/__init__.py
--rw-------   0 robin     (1000) robin     (1000)    28541 2023-04-27 16:12:55.000000 movia-1.0.0b3/movia/core/io/read.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    11971 2023-04-27 15:50:58.000000 movia-1.0.0b3/movia/core/io/scheduler.py
--rw-------   0 robin     (1000) robin     (1000)    12901 2023-04-25 08:41:16.000000 movia-1.0.0b3/movia/core/io/write.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.100666 movia-1.0.0b3/movia/core/optimisation/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/optimisation/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.132666 movia-1.0.0b3/movia/core/optimisation/cache/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/optimisation/cache/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1212 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/optimisation/cache/basic.py
--rw-------   0 robin     (1000) robin     (1000)     2829 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/optimisation/cache/hashes.py
--rw-------   0 robin     (1000) robin     (1000)     1213 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/optimisation/cache/singleton.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.144667 movia-1.0.0b3/movia/core/optimisation/cuda/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/core/optimisation/cuda/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.152667 movia-1.0.0b3/movia/core/optimisation/parallel/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-04-08 09:51:10.000000 movia-1.0.0b3/movia/core/optimisation/parallel/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2176 2023-04-11 16:58:53.000000 movia-1.0.0b3/movia/core/optimisation/parallel/buffer.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.204667 movia-1.0.0b3/movia/gui/
--rw-r--r--   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1230 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/__main__.py
--rw-------   0 robin     (1000) robin     (1000)     2298 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/actions.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.212667 movia-1.0.0b3/movia/gui/app/
--rw-r--r--   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/app/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     8380 2023-04-10 22:28:36.000000 movia-1.0.0b3/movia/gui/app/app.py
--rw-------   0 robin     (1000) robin     (1000)     1750 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/base.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.244668 movia-1.0.0b3/movia/gui/edit_node_state/
--rw-------   0 robin     (1000) robin     (1000)      134 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.272668 movia-1.0.0b3/movia/gui/edit_node_state/all/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/all/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     3006 2023-04-10 22:28:32.000000 movia-1.0.0b3/movia/gui/edit_node_state/all/container_input_ffmpeg.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3299 2023-04-27 18:15:16.000000 movia-1.0.0b3/movia/gui/edit_node_state/all/filter_cut.py
--rw-------   0 robin     (1000) robin     (1000)     1675 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/all/filter_translate.py
--rw-------   0 robin     (1000) robin     (1000)     1632 2023-04-27 17:28:28.000000 movia-1.0.0b3/movia/gui/edit_node_state/all/filter_truncate.py
--rw-------   0 robin     (1000) robin     (1000)      703 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/all/generator_audio_noise.py
--rw-------   0 robin     (1000) robin     (1000)     3638 2023-04-27 08:00:29.000000 movia-1.0.0b3/movia/gui/edit_node_state/all/generator_video_equation.py
--rw-------   0 robin     (1000) robin     (1000)      764 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/all/generator_video_noise.py
--rw-------   0 robin     (1000) robin     (1000)     3017 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/base.py
--rw-------   0 robin     (1000) robin     (1000)      956 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/default.py
--rw-------   0 robin     (1000) robin     (1000)     1590 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/documentation.py
--rw-------   0 robin     (1000) robin     (1000)     3146 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/general.py
--rw-------   0 robin     (1000) robin     (1000)     3647 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/interface.py
--rw-------   0 robin     (1000) robin     (1000)     1537 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/loader.py
--rw-------   0 robin     (1000) robin     (1000)     2496 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edit_node_state/main.py
--rw-------   0 robin     (1000) robin     (1000)     1033 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/edition_tabs.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.288668 movia-1.0.0b3/movia/gui/entry/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/entry/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     4489 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/entry/base.py
--rw-------   0 robin     (1000) robin     (1000)      400 2023-04-19 18:11:03.000000 movia-1.0.0b3/movia/gui/entry/filters.py
--rw-------   0 robin     (1000) robin     (1000)      527 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/entry/generators.py
--rw-------   0 robin     (1000) robin     (1000)     4047 2023-04-10 22:28:10.000000 movia-1.0.0b3/movia/gui/entry/project_files.py
--rw-------   0 robin     (1000) robin     (1000)     1330 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/entry_tabs.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.304668 movia-1.0.0b3/movia/gui/export/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/export/__init__.py
--rw-------   0 robin     (1000) robin     (1000)    20252 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/export/settings.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.316668 movia-1.0.0b3/movia/gui/graph/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/graph/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     5033 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/graph/edge_properties.py
--rw-------   0 robin     (1000) robin     (1000)    20156 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/graph/graph_editor.py
--rw-------   0 robin     (1000) robin     (1000)     8773 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/graph/layout.py
--rw-------   0 robin     (1000) robin     (1000)     5194 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/main.py
--rw-------   0 robin     (1000) robin     (1000)      643 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/menu.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.320669 movia-1.0.0b3/movia/gui/timeline/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/timeline/__init__.py
--rw-------   0 robin     (1000) robin     (1000)      723 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/toolbar.py
--rw-------   0 robin     (1000) robin     (1000)      606 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/gui/tools.py
--rw-------   0 robin     (1000) robin     (1000)    16767 2023-04-09 22:54:11.000000 movia-1.0.0b3/movia/gui/video_viewer.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:47.332669 movia-1.0.0b3/movia/testing/
--rw-------   0 robin     (1000) robin     (1000)      165 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/testing/__init__.py
--rwx--x--x   0 robin     (1000) robin     (1000)      220 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/testing/__main__.py
--rw-------   0 robin     (1000) robin     (1000)     1672 2023-04-27 14:23:38.000000 movia-1.0.0b3/movia/testing/generation.py
--rw-------   0 robin     (1000) robin     (1000)     1499 2023-04-10 12:04:34.000000 movia-1.0.0b3/movia/testing/runtests.py
--rw-------   0 robin     (1000) robin     (1000)      557 2023-03-28 15:30:31.000000 movia-1.0.0b3/movia/utils.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-28 13:17:46.524660 movia-1.0.0b3/movia.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)     4819 2023-04-28 13:17:46.000000 movia-1.0.0b3/movia.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)     4429 2023-04-28 13:17:46.000000 movia-1.0.0b3/movia.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-04-28 13:17:46.000000 movia-1.0.0b3/movia.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)      137 2023-04-28 13:17:46.000000 movia-1.0.0b3/movia.egg-info/entry_points.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)      184 2023-04-28 13:17:46.000000 movia-1.0.0b3/movia.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        6 2023-04-28 13:17:46.000000 movia-1.0.0b3/movia.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-04-28 13:17:47.336669 movia-1.0.0b3/setup.cfg
--rw-------   0 robin     (1000) robin     (1000)     3762 2023-04-08 17:11:13.000000 movia-1.0.0b3/setup.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.899839 movia-1.0a1/
+-rw-r--r--   0 robin     (1000) robin     (1000)    34519 2022-12-05 11:30:47.000000 movia-1.0a1/LICENSE
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4113 2023-03-13 10:04:13.895839 movia-1.0a1/PKG-INFO
+-rw-------   0 robin     (1000) robin     (1000)     2466 2023-03-12 23:41:34.000000 movia-1.0a1/README.rst
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.771842 movia-1.0a1/movia/
+-rw-r--r--   0 robin     (1000) robin     (1000)      115 2023-03-13 09:57:14.000000 movia-1.0a1/movia/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1268 2023-03-06 22:24:38.000000 movia-1.0a1/movia/__main__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.779842 movia-1.0a1/movia/core/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:20.000000 movia-1.0a1/movia/core/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.783842 movia-1.0a1/movia/core/analysis/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:34.000000 movia-1.0a1/movia/core/analysis/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2970 2023-02-21 21:31:11.000000 movia-1.0a1/movia/core/analysis/streams.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.783842 movia-1.0a1/movia/core/analysis/video/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:29.000000 movia-1.0a1/movia/core/analysis/video/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.795842 movia-1.0a1/movia/core/analysis/video/properties/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:29.000000 movia-1.0a1/movia/core/analysis/video/properties/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5958 2023-01-15 15:56:54.000000 movia-1.0a1/movia/core/analysis/video/properties/duration.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4115 2023-03-11 16:13:19.000000 movia-1.0a1/movia/core/analysis/video/properties/framerate.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5152 2023-01-15 15:56:50.000000 movia-1.0a1/movia/core/analysis/video/properties/nb_frames.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3827 2023-01-15 15:56:48.000000 movia-1.0a1/movia/core/analysis/video/properties/parser.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    14907 2023-01-15 15:56:46.000000 movia-1.0a1/movia/core/analysis/video/properties/timestamps.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.799841 movia-1.0a1/movia/core/classes/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:20.000000 movia-1.0a1/movia/core/classes/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1302 2023-03-10 08:40:10.000000 movia-1.0a1/movia/core/classes/container.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      965 2023-02-10 08:33:37.000000 movia-1.0a1/movia/core/classes/filter.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4228 2023-02-10 12:27:07.000000 movia-1.0a1/movia/core/classes/node.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5006 2023-03-04 13:32:43.000000 movia-1.0a1/movia/core/classes/stream.py
+-rw-------   0 robin     (1000) robin     (1000)     4166 2023-03-04 13:08:40.000000 movia-1.0a1/movia/core/classes/stream_audio.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4133 2023-03-04 13:09:02.000000 movia-1.0a1/movia/core/classes/stream_video.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.807841 movia-1.0a1/movia/core/compilation/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:27.000000 movia-1.0a1/movia/core/compilation/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.811841 movia-1.0a1/movia/core/compilation/export/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-03-11 15:36:53.000000 movia-1.0a1/movia/core/compilation/export/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    30589 2023-03-12 17:52:58.000000 movia-1.0a1/movia/core/compilation/export/compatibility.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4357 2023-03-12 18:30:42.000000 movia-1.0a1/movia/core/compilation/export/default.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      653 2023-03-12 18:25:54.000000 movia-1.0a1/movia/core/compilation/export/encodec.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      280 2023-03-12 18:01:03.000000 movia-1.0a1/movia/core/compilation/export/muxer.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      986 2023-03-12 18:53:47.000000 movia-1.0a1/movia/core/compilation/export/rate_audio.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1124 2023-03-12 16:32:11.000000 movia-1.0a1/movia/core/compilation/export/rate_video.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    15006 2023-03-12 16:11:46.000000 movia-1.0a1/movia/core/compilation/graph_to_ast.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7842 2023-03-11 15:20:27.000000 movia-1.0a1/movia/core/compilation/graph_to_tree.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5343 2023-03-08 17:30:41.000000 movia-1.0a1/movia/core/compilation/tree_to_graph.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.811841 movia-1.0a1/movia/core/edit/
+-rw-r--r--   0 robin     (1000) robin     (1000)      216 2023-02-03 16:32:38.000000 movia-1.0a1/movia/core/edit/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.815841 movia-1.0a1/movia/core/edit/operation/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      158 2023-02-03 16:34:25.000000 movia-1.0a1/movia/core/edit/operation/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2362 2023-03-06 22:29:20.000000 movia-1.0a1/movia/core/edit/operation/add.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    22507 2023-03-06 22:37:35.000000 movia-1.0a1/movia/core/edit/operation/remove.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1273 2023-01-07 17:41:19.000000 movia-1.0a1/movia/core/exceptions.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.815841 movia-1.0a1/movia/core/filters/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:18.000000 movia-1.0a1/movia/core/filters/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.819841 movia-1.0a1/movia/core/filters/basic/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:18.000000 movia-1.0a1/movia/core/filters/basic/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4621 2023-03-10 21:57:08.000000 movia-1.0a1/movia/core/filters/basic/truncate.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.819841 movia-1.0a1/movia/core/generation/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:27.000000 movia-1.0a1/movia/core/generation/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.823841 movia-1.0a1/movia/core/generation/audio/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-01-09 19:53:13.000000 movia-1.0a1/movia/core/generation/audio/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2021 2023-02-15 15:34:59.000000 movia-1.0a1/movia/core/generation/audio/empty.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3040 2023-02-15 15:35:27.000000 movia-1.0a1/movia/core/generation/audio/noise.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.831841 movia-1.0a1/movia/core/generation/video/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:25.000000 movia-1.0a1/movia/core/generation/video/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2142 2023-02-15 15:22:43.000000 movia-1.0a1/movia/core/generation/video/empty.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    12941 2023-02-16 08:56:25.000000 movia-1.0a1/movia/core/generation/video/equation.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4592 2023-02-16 08:56:38.000000 movia-1.0a1/movia/core/generation/video/noise.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.835841 movia-1.0a1/movia/core/io/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:23.000000 movia-1.0a1/movia/core/io/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    29782 2023-02-15 15:39:40.000000 movia-1.0a1/movia/core/io/read.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    20239 2023-03-12 13:20:11.000000 movia-1.0a1/movia/core/io/write.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.843840 movia-1.0a1/movia/gui/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:41.000000 movia-1.0a1/movia/gui/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1461 2023-02-15 17:07:40.000000 movia-1.0a1/movia/gui/actions.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.847840 movia-1.0a1/movia/gui/app/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:41.000000 movia-1.0a1/movia/gui/app/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6958 2023-03-12 17:17:41.000000 movia-1.0a1/movia/gui/app/app.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1750 2023-02-09 20:52:27.000000 movia-1.0a1/movia/gui/base.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1033 2023-02-02 14:45:30.000000 movia-1.0a1/movia/gui/edition_tabs.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.867840 movia-1.0a1/movia/gui/entry/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-02-09 20:40:42.000000 movia-1.0a1/movia/gui/entry/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4716 2023-03-12 23:54:04.000000 movia-1.0a1/movia/gui/entry/base.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      386 2023-02-10 13:26:10.000000 movia-1.0a1/movia/gui/entry/filters.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      527 2023-02-11 06:51:40.000000 movia-1.0a1/movia/gui/entry/generators.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3948 2023-02-21 21:36:32.000000 movia-1.0a1/movia/gui/entry/project_files.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1330 2023-02-10 08:16:32.000000 movia-1.0a1/movia/gui/entry_tabs.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.867840 movia-1.0a1/movia/gui/export/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-02-15 16:48:48.000000 movia-1.0a1/movia/gui/export/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    26382 2023-03-12 18:51:01.000000 movia-1.0a1/movia/gui/export/settings.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.875840 movia-1.0a1/movia/gui/graph/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-01-14 21:58:00.000000 movia-1.0a1/movia/gui/graph/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5056 2023-02-05 22:21:29.000000 movia-1.0a1/movia/gui/graph/edge_properties.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    20179 2023-02-09 20:03:15.000000 movia-1.0a1/movia/gui/graph/graph_editor.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     8773 2023-03-06 22:37:40.000000 movia-1.0a1/movia/gui/graph/layout.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3192 2023-02-15 17:06:56.000000 movia-1.0a1/movia/gui/main.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      517 2023-02-15 16:22:54.000000 movia-1.0a1/movia/gui/menu.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.895839 movia-1.0a1/movia/gui/node_properties/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-02-02 09:10:01.000000 movia-1.0a1/movia/gui/node_properties/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4624 2023-02-09 20:05:41.000000 movia-1.0a1/movia/gui/node_properties/container_input_ffmpeg.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2673 2023-03-10 22:20:26.000000 movia-1.0a1/movia/gui/node_properties/filter_truncate.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4581 2023-02-08 10:19:07.000000 movia-1.0a1/movia/gui/node_properties/generator_video_equation.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7206 2023-02-26 23:05:58.000000 movia-1.0a1/movia/gui/node_properties/node_properties.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.895839 movia-1.0a1/movia/gui/timeline/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-01-14 21:57:36.000000 movia-1.0a1/movia/gui/timeline/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      590 2023-02-15 16:23:21.000000 movia-1.0a1/movia/gui/toolbar.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    16538 2023-03-12 16:39:40.000000 movia-1.0a1/movia/gui/video_viewer.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      555 2023-02-09 21:09:03.000000 movia-1.0a1/movia/utils.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.779842 movia-1.0a1/movia.egg-info/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4113 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2809 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/SOURCES.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/dependency_links.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       46 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/entry_points.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)      127 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/requires.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        6 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/top_level.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-03-13 10:04:13.899839 movia-1.0a1/setup.cfg
+-rw-r--r--   0 robin     (1000) robin     (1000)     3174 2023-03-13 09:46:20.000000 movia-1.0a1/setup.py
```

### Comparing `movia-1.0.0b3/LICENSE` & `movia-1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/README.rst` & `movia-1.0a1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 .. rst syntax: https://deusyss.developpez.com/tutoriels/Python/SphinxDoc/
 .. icons: https://specifications.freedesktop.org/icon-naming-spec/latest/ar01s04.html or https://www.pythonguis.com/faq/built-in-qicons-pyqt/
 .. pyqtdoc: https://www.riverbankcomputing.com/static/Docs/PyQt6/
 
 
-*****
-Movia
-*****
-
 .. image:: https://github.com/pytest-dev/pytest/workflows/test/badge.svg
     :target: https://github.com/pytest-dev/pytest/actions?query=workflow%3Atest
 
 .. image:: https://img.shields.io/badge/linting-pylint-yellowgreen
     :target: https://github.com/PyCQA/pylint
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
+**************************************
+movia, a light video editing software!
+**************************************
 
 Decsription
 -----------
 
-This software proposes a graphic interface powered by pyqt6 (run ``movia-qt``).
+This software proposes a graphic interface powered by pyqt6 (run ``movia``).
 The kernel is written in python and is easily integrated in other projects (module ``movia.core``).
 
 This software is **light**, **fast** and **highly configurable** for the following reasons:
 
 1. Based on ffmpeg, this software supports an incredible number of formats and codecs.
 2. Thanks to operations on the assembly graph, it is able to perform nbr_opti optimization operations.
 3. nbr_tests unit tests ensure an excelent kernel reliability.
 4. Unlike other software that offers a timeline, this one allows you to edit an editing graph. This representation is more general and thus allows a greater flexibility.
 5. A compiled version without graphical interface allows to allocate all the resources of the computer to the export.
 6. This software generates at the time of the export a python code which can be edited. This offers an infinite number of possibilities!
 
-
 Installation
 ------------
 
-Movia has hard dependency on the pygraphviz library and on the ffmpeg package (version >= 4). You should install it first, please refer to the `pygraphviz installation guide <https://pygraphviz.github.io/documentation/stable/install.html>`_ and according to your Linux distribution, to the `FFmpeg download page <https://ffmpeg.org/download.html>`_.
+Dependencies
+^^^^^^^^^^^^
 
-In many cases, these commands should work:
+* `ffmpeg5 <https://ubuntuhandbook.org/index.php/2022/02/install-ffmpeg-5-0-ubuntu/>`_
 
 .. code:: bash
 
-    $ sudo apt install ffmpeg
-    $ sudo apt install graphviz graphviz-dev
+    sudo add-apt-repository ppa:savoury1/ffmpeg4
+    sudo add-apt-repository ppa:savoury1/ffmpeg5
+    sudo apt update
+    sudo apt full-upgrade
+    sudo apt install ffmpeg
 
-Although it is installed automatically, it is better to install **av** manually to avoid redundancy. Please refer to the `PyAv installation guide <https://pyav.org/docs/develop/overview/installation.html>`_.
-
-In many cases, these commands should work:
+* `pygraphviz <https://pygraphviz.github.io/documentation/stable/install.html>`_
 
 .. code:: bash
 
-    $ sudo apt install libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev libswscale-dev libswresample-dev libavfilter-dev
-    $ pip install av --no-binary av
+    sudo apt install graphviz graphviz-dev pygraphviz
 
-To install Movia using `PyPI <https://pypi.org/project/movia/>`_, run the following command:
+Depos
+^^^^^
 
 .. code:: bash
 
-    $ pip install movia[gui]
+    git clone https://framagit.org/robinechuca/movia.git
+    cd movia/
+    python -m pip install -e ./
 
-To install Movia from `Framagit <https://framagit.org/robinechuca/movia>`_ source, clone Movia using ``git`` and install it using ``pip``.:
+Run
+^^^
 
 .. code:: bash
 
-    git clone https://framagit.org/robinechuca/movia.git
-    cd movia/
-    pip install -e ./[optional]
-
-In a terminal, simply write the command ``movia-qt`` to launch the GUI.
+    movia
 
 
 What's new ?
 ------------
 
-For the complete list of changes, refer to the `git commits <https://framagit.org/robinechuca/movia/-/network/main?ref_type=heads>`_.
+Nothing new for the moment.
```

### Comparing `movia-1.0.0b3/movia/core/analysis/video/properties/duration.py` & `movia-1.0a1/movia/core/analysis/video/properties/duration.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,160 +4,177 @@
 ** Finds the duration of a video stream. **
 -------------------------------------------
 
 This allows not only the characteristics of the files but also the tags if there are any.
 """
 
 import collections
-import fractions
 import pathlib
 import typing
 
 import cv2 # pip install opencv-contrib-python-headless
 
-from movia.core.analysis._helper_properties import _check_pathexists_index, _mix_and_check
-from movia.core.analysis.stream import (_decode_duration_ffmpeg, _estimate_duration_ffmpeg,
-    _map_index_rel_to_abs)
 from movia.core.exceptions import MissingStreamError, MissingInformation
+from movia.core.analysis.video.properties.parser import (_check_pathexists_index,
+    _decode_duration_frames_ffmpeg, _mix_and_check, _parse_ffprobe_res)
 
 
 
+def _decode_duration_ffmpeg(filename: str, index: int) -> float:
+    """
+    ** Extract the duration by the complete decoding of the stream. **
+
+    Slow but 100% accurate method.
 
-def _decode_duration_cv2(filename: str, index: int) -> fractions.Fraction:
+    Examples
+    --------
+    >>> from movia.core.analysis.video.properties.duration import _decode_duration_ffmpeg
+    >>> _decode_duration_ffmpeg("movia/examples/video.mp4", 0)
+    16.0
+    >>>
+    """
+    duration, _ = _decode_duration_frames_ffmpeg(filename, index)
+    return duration
+
+def _decode_duration_cv2(filename: str, index: int) -> float:
     """
     ** Extract the duration by the complete decoding of the stream. **
 
     Slow but 100% accurate method.
 
     Examples
     --------
     >>> from movia.core.analysis.video.properties.duration import _decode_duration_cv2
     >>> _decode_duration_cv2("movia/examples/video.mp4", 0)
-    Fraction(16, 1)
+    16.0
     >>>
     """
     cap = cv2.VideoCapture(filename, index)
     if not cap.isOpened():
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
-    if (fps := fractions.Fraction(cap.get(cv2.CAP_PROP_FPS)).limit_denominator(1001)) <= 0:
+    if (fps := float(cap.get(cv2.CAP_PROP_FPS))) <= 0:
         one_over_fps = 0
     else:
         one_over_fps = 1 / fps
-    duration = fractions.Fraction(0)
+    duration = .0
     while True:
-        duration = (
-            fractions.Fraction(round(cap.get(cv2.CAP_PROP_POS_MSEC))) / 1000
-            or duration + one_over_fps
-        )
+        duration = (1e-3 * float(cap.get(cv2.CAP_PROP_POS_MSEC))) or (duration + one_over_fps)
         if not cap.read()[0]:
             break
     cap.release()
     if not duration:
         raise MissingStreamError(f"'cv2' did not find duration '{filename}' stream {index}")
-    return duration + one_over_fps
+    return round(duration + one_over_fps, 3)
+
+def _estimate_duration_ffmpeg(filename: str, index: int) -> float:
+    """
+    ** Extract the duration from the metadata. **
+
+    Very fast method but inaccurate. It doesn't work all the time.
 
+    Examples
+    --------
+    >>> from movia.core.analysis.video.properties.duration import _estimate_duration_ffmpeg
+    >>> _estimate_duration_ffmpeg("movia/examples/video.mp4", 0)
+    16.0
+    >>>
+    """
+    cmd = [
+        "ffprobe",
+        "-v", "error",
+        "-select_streams", f"v:{index}",
+        "-show_entries", "format=duration",
+        "-of", "default=noprint_wrappers=1:nokey=1",
+        filename,
+    ]
+    duration = _parse_ffprobe_res(cmd, filename, index)
+    try:
+        duration = float(duration)
+    except ValueError as err:
+        raise MissingInformation(
+            f"'ffprobe' did not get a correct duration in '{filename}' stream {index}"
+        ) from err
+    if duration <= 0:
+        raise MissingInformation(
+            f"'ffprobe' finds a duration of {duration} in '{filename}' stream {index}"
+        )
+    return duration
 
-def _estimate_duration_cv2(filename: str, index: int) -> fractions.Fraction:
+def _estimate_duration_cv2(filename: str, index: int) -> float:
     """
     ** Extract the duration from the metadata. **
 
     Very fast method but inaccurate. It doesn't work all the time.
 
     Examples
     --------
     >>> from movia.core.analysis.video.properties.duration import _estimate_duration_cv2
     >>> _estimate_duration_cv2("movia/examples/video.mp4", 0)
-    Fraction(16, 1)
+    16.0
     >>>
     """
     cap = cv2.VideoCapture(filename, index)
     if not cap.isOpened():
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
-    frames = round(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-    fps = fractions.Fraction(cap.get(cv2.CAP_PROP_FPS)).limit_denominator(1001)
+    frames = float(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+    fps = float(cap.get(cv2.CAP_PROP_FPS))
     duration = frames / fps if fps and frames else 0
     cap.release()
     if duration <= 0:
         raise MissingInformation(
             f"'cv2' does not detect any duration in '{filename}' stream {index}"
         )
     return duration
 
-
-def get_duration_video(
+def get_duration(
     filename: typing.Union[str, bytes, pathlib.Path],
     index: int=0,
     *,
     backend: typing.Union[None, str]=None,
     accurate: bool=False,
-) -> fractions.Fraction:
+) -> float:
     """
     ** Recovers the total duration of a video stream. **
 
     The duration includes the display time o the last frame.
 
     Parameters
     ----------
     filename : pathlike
         The pathlike of the file containing a video stream.
     index : int
-        The relative index of the video stream being considered,
-        by default the first video stream encountered is selected.
+        The index of the video stream being considered,
+        by default the first stream encountered is selected.
     backend : str, optional
         - None (default) : Try to read the stream by trying differents backends.
         - 'ffmpeg' : Uses the modules ``pip3 install ffmpeg-python``
             which are using the ``ffmpeg`` program in the background.
         - 'cv2' : Uses the module ``pip3 install opencv-contrib-python-headless``.
     accurate : boolean, optional
         If True, recovers the duration by fully decoding all the frames in the video.
         It is very accurate but very slow. If False (default),
         first tries to get the duration from the file metadata.
         It's not accurate but very fast.
 
     Returns
     -------
-    duration : fractions.Fraction
+    duration : float
         The total duration of the considerated video stream.
 
     Raises
     ------
     MissingStreamError
         If the file does not contain a playable video stream.
     MissingInformation
         If the information is unavailable.
-
-    Examples
-    --------
-    >>> from movia.core.analysis.video.properties.duration import get_duration_video
-    >>> get_duration_video("movia/examples/video.mp4")
-    Fraction(16, 1)
-    >>> get_duration_video("movia/examples/intro.mkv")
-    Fraction(9809, 1000)
-    >>>
     """
     _check_pathexists_index(filename, index)
 
     return _mix_and_check(
         backend, accurate, (str(pathlib.Path(filename)), index),
         collections.OrderedDict([
-            (
-                (lambda filename, index: _estimate_duration_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"))
-                ),
-                {"accurate": False, "backend": "ffmpeg"}
-            ),
-            (
-                (lambda filename, index: _decode_duration_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"), accurate=False)
-                ),
-                {"accurate": False, "backend": "ffmpeg"}
-            ),
+            (_estimate_duration_ffmpeg, {"accurate": False, "backend": "ffmpeg"}),
             (_estimate_duration_cv2, {"accurate": False, "backend": "cv2"}),
-            (
-                (lambda filename, index: _decode_duration_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"), accurate=True)
-                ),
-                {"accurate": True, "backend": "ffmpeg"}
-            ),
+            (_decode_duration_ffmpeg, {"accurate": True, "backend": "ffmpeg"}),
             (_decode_duration_cv2, {"accurate": True, "backend": "cv2"}),
         ])
     )
```

### Comparing `movia-1.0.0b3/movia/core/analysis/video/properties/nb_frames.py` & `movia-1.0a1/movia/core/analysis/video/properties/nb_frames.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 
 import collections
 import pathlib
 import typing
 
 import cv2 # pip install opencv-contrib-python-headless
 
-from movia.core.analysis._helper_properties import _check_pathexists_index, _mix_and_check
-from movia.core.analysis.stream import (_estimate_len_ffmpeg, _map_index_rel_to_abs,
-    get_slices_metadata)
 from movia.core.exceptions import MissingStreamError, MissingInformation
-
+from movia.core.analysis.video.properties.parser import (_check_pathexists_index,
+    _decode_duration_frames_ffmpeg, _mix_and_check, _parse_ffprobe_res)
 
 
 def _count_frames_ffmpeg(filename: str, index: int) -> int:
     """
     ** Count the number of frames with the ffmpeg decoder. **
 
     Slow but 100% accurate method.
@@ -29,21 +27,17 @@
     Examples
     --------
     >>> from movia.core.analysis.video.properties.nb_frames import _count_frames_ffmpeg
     >>> _count_frames_ffmpeg("movia/examples/video.mp4", 0)
     400
     >>>
     """
-    _, infos = get_slices_metadata(filename, slice_type="frame")
-    if index >= len(infos):
-        raise MissingInformation(f"'ffmpeg' did not decode '{filename}' stream {index}")
-    frames = infos[index].shape[0]
+    _, frames = _decode_duration_frames_ffmpeg(filename, index)
     return frames
 
-
 def _count_frames_cv2(filename: str, index: int) -> int:
     """
     ** Count the number of frames with the cv2 decoder. **
 
     Slow but 100% accurate method.
 
     Examples
@@ -62,14 +56,35 @@
             break
         frames += 1
     cap.release()
     if not frames:
         raise MissingStreamError(f"'cv2' did not find any frames '{filename}' stream {index}")
     return frames
 
+def _estimate_frames_ffmpeg(filename: str, index: int) -> int:
+    """
+    ** Extract the number of frames from the metadata. **
+
+    Very fast method but inaccurate. It doesn't work all the time.
+
+    Examples
+    --------
+    >>> from movia.core.analysis.video.properties.nb_frames import _estimate_frames_ffmpeg
+    >>> _estimate_frames_ffmpeg("movia/examples/video.mp4", 0)
+    400
+    >>>
+    """
+    cmd = [
+        "ffprobe", "-v", "error",
+        "-select_streams", f"v:{index}", "-show_entries", "stream=nb_frames",
+        "-of", "default=nokey=1:noprint_wrappers=1",
+        filename,
+    ]
+    frames = _parse_ffprobe_res(cmd, filename, index)
+    return int(frames)
 
 def _estimate_frames_cv2(filename: str, index: int) -> int:
     """
     ** Extract the number of frames from the metadata. **
 
     Very fast method but inaccurate. It doesn't work all the time.
 
@@ -85,15 +100,14 @@
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
     frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
     cap.release()
     if frames <= 0: # we saw a case at -553402322211286528
         raise MissingInformation(f"'cv2' does not detect any frame in '{filename}' stream {index}")
     return frames
 
-
 def get_nb_frames(
     filename: typing.Union[str, bytes, pathlib.Path],
     index: int=0,
     *,
     backend: typing.Union[None, str]=None,
     accurate: bool=False,
 ) -> int:
@@ -101,15 +115,15 @@
     ** Recovers the number of frames present in a video stream. **
 
     Parameters
     ----------
     filename : pathlike
         The pathlike of the file containing a video stream.
     index : int
-        The relative index of the video stream being considered,
+        The index of the video stream being considered,
         by default the first stream encountered is selected.
     backend : str, optional
         - None (default) : Try to read the stream by trying differents backends.
         - 'ffmpeg' : Uses the modules ``pip3 install ffmpeg-python``
             which are using the ``ffmpeg`` program in the background.
         - 'cv2' : Uses the module ``pip3 install opencv-contrib-python-headless``.
     accurate : boolean, optional
@@ -125,38 +139,19 @@
 
     Raises
     ------
     MissingStreamError
         If the file does not contain a playable video stream.
     MissingInformation
         If the information is unavailable.
-
-    Examples
-    --------
-    >>> from movia.core.analysis.video.properties.nb_frames import get_nb_frames
-    >>> get_nb_frames("movia/examples/video.mp4")
-    400
-    >>> get_nb_frames("movia/examples/intro.mkv")
-    294
-    >>>
     """
     _check_pathexists_index(filename, index)
 
     return _mix_and_check(
         backend, accurate, (str(pathlib.Path(filename)), index),
         collections.OrderedDict([
-            (
-                (lambda filename, index: _estimate_len_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"))
-                ),
-                {"accurate": False, "backend": "ffmpeg"}
-            ),
+            (_estimate_frames_ffmpeg, {"accurate": False, "backend": "ffmpeg"}),
             (_estimate_frames_cv2, {"accurate": False, "backend": "cv2"}),
-            (
-                (lambda filename, index: _count_frames_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"))
-                ),
-                {"accurate": True, "backend": "ffmpeg"}
-            ),
+            (_count_frames_ffmpeg, {"accurate": True, "backend": "ffmpeg"}),
             (_count_frames_cv2, {"accurate": True, "backend": "cv2"}),
         ])
     )
```

### Comparing `movia-1.0.0b3/movia/core/analysis/video/properties/rate.py` & `movia-1.0a1/movia/core/analysis/video/properties/framerate.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,101 +5,124 @@
 -----------------------------------------------------
 
 This information is collected in the metadata of the file.
 Its access is fast but its value is not always accurate.
 Especially since the framerate is not always constant within the same stream.
 """
 
-import collections
 import fractions
+import numbers
 import pathlib
+import re
 import typing
 
 import cv2 # pip install opencv-contrib-python-headless
 
-from movia.core.analysis._helper_properties import _check_pathexists_index, _mix_and_check
-from movia.core.analysis.stream import _estimate_rate_ffmpeg
-from movia.core.analysis.stream import _map_index_rel_to_abs
 from movia.core.exceptions import MissingStreamError, MissingInformation
+from movia.core.analysis.video.properties.parser import _parse_ffprobe_res
 
 
 
-def _estimate_rate_cv2(filename: str, index: int) -> fractions.Fraction:
+def _estimate_fps_cv2(filename: str, index: int) -> float:
     """
     ** Retrieves via cv2, the metadata concerning the fps. **
 
     This function is fast because it reads only the header of the file.
 
     Examples
     --------
-    >>> from movia.core.analysis.video.properties.rate import _estimate_rate_cv2
-    >>> _estimate_rate_cv2("movia/examples/video.mp4", 0)
-    Fraction(25, 1)
+    >>> from movia.core.analysis.video.properties.framerate import _estimate_fps_cv2
+    >>> _estimate_fps_cv2("movia/examples/video.mp4", 0)
+    25.0
     >>>
     """
     cap = cv2.VideoCapture(filename, index)
     if not cap.isOpened():
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
-    fps = fractions.Fraction(cap.get(cv2.CAP_PROP_FPS)).limit_denominator(1001)
+    fps = float(cap.get(cv2.CAP_PROP_FPS))
     cap.release()
     if fps <= 0:
         raise MissingInformation(f"'cv2' finds an fps of {fps} in '{filename}' stream {index}")
     return fps
 
 
-def get_rate_video(
+def _estimate_fps_ffmpeg(filename: str, index: int) -> fractions.Fraction:
+    """
+    ** Retrieves via ffmpeg, the metadata concerning the fps. **
+
+    This function is fast because it reads only the header of the file.
+
+    ffprobe -v quiet -print_format json -show_streams -select_streams v:0 video.mp4
+
+    Examples
+    --------
+    >>> from movia.core.analysis.video.properties.framerate import _estimate_fps_ffmpeg
+    >>> _estimate_fps_ffmpeg("movia/examples/video.mp4", 0)
+    Fraction(25, 1)
+    >>>
+    """
+    cmd = [
+        "ffprobe", "-v", "error",
+        "-select_streams", f"v:{index}", "-show_entries", "stream=r_frame_rate,avg_frame_rate",
+        "-of", "default=nokey=1:noprint_wrappers=1",
+        filename,
+    ]
+    fps_str = _parse_ffprobe_res(cmd, filename, index)
+    for match in re.finditer(r"\d+(/\d+)?", fps_str):
+        try:
+            return fractions.Fraction(match.group())
+        except ZeroDivisionError:
+            continue
+    raise MissingInformation(
+            f"'ffprobe' did not get a correct framerate in '{filename}' stream {index}"
+        )
+
+
+def get_fps(
     filename: typing.Union[str, bytes, pathlib.Path],
     index: int=0,
     *,
     backend: typing.Union[None, str]=None
-) -> fractions.Fraction:
+) -> numbers.Real:
     """
     ** Reads in the metadata, the average frequency of the frames. **
 
     Parameters
     ----------
     filename : pathlike
         The pathlike of the file containing a video stream.
     index : int
-        The relative index of the video stream being considered,
+        The index of the video stream being considered,
         by default the first stream encountered is selected.
     backend : str, optional
         - None (default) : Try to read the stream by trying differents backends.
         - 'ffmpeg' : Uses the modules ``pip install ffmpeg-python``
             which are using the ``ffmpeg`` program in the background.
         - 'cv2' : Uses the module ``pip install opencv-contrib-python-headless``.
 
     Returns
     -------
-    fps : fractions.Fraction
+    fps : numbers.Real
         The average frequency of the frames in hz.
 
     Raises
     ------
     MissingStreamError
         If the file does not contain a playable video stream.
     MissingInformation
         If the information is unavailable.
-
-    Examples
-    --------
-    >>> from movia.core.analysis.video.properties.rate import get_rate_video
-    >>> get_rate_video("movia/examples/video.mp4")
-    Fraction(25, 1)
-    >>> get_rate_video("movia/examples/intro.mkv")
-    Fraction(30000, 1001)
-    >>>
     """
-    _check_pathexists_index(filename, index)
-
-    return _mix_and_check(
-        backend, False, (str(pathlib.Path(filename)), index),
-        collections.OrderedDict([
-            (
-                (lambda filename, index: _estimate_rate_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"))
-                ),
-                {"accurate": False, "backend": "ffmpeg"}
-            ),
-            (_estimate_rate_cv2, {"accurate": False, "backend": "cv2"}),
-        ])
-    )
+    assert pathlib.Path(filename).exists(), filename
+    assert isinstance(index, numbers.Integral), index.__class__.__name__
+    assert backend is None or backend in {"ffmpeg", "cv2"}, backend
+
+    filename = str(pathlib.Path(filename))
+
+    if backend == "ffmpeg":
+        return _estimate_fps_ffmpeg(filename, index)
+    if backend == "cv2":
+        return _estimate_fps_cv2(filename, index)
+
+    try:
+        return _estimate_fps_ffmpeg(filename, index)
+    except (MissingStreamError, MissingInformation):
+        return _estimate_fps_cv2(filename, index)
```

### Comparing `movia-1.0.0b3/movia/core/classes/container.py` & `movia-1.0a1/movia/core/classes/container.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/core/classes/filter.py` & `movia-1.0a1/movia/core/classes/filter.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/core/classes/node.py` & `movia-1.0a1/movia/core/classes/node.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/core/classes/stream.py` & `movia-1.0a1/movia/core/classes/stream.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,53 +3,47 @@
 """
 ** Defines the structure of an abstract multimedia stream. **
 -------------------------------------------------------------
 """
 
 
 import abc
-import fractions
+import math
 import numbers
-import typing
 
 
 
 class Stream(abc.ABC):
     """
     Attributes
     ----------
-    beginning : fractions.Fraction
+    beginning : numbers.Real
         The stream beginning instant in second (readonly).
-    duration : typing.Union[fractions.Fraction, float]
+    duration : numbers.Real
         The duration of the flow in seconds, it can be infinite (readonly).
         This value needs to be accurate.
     index : int
         The stream index from the parent node (0 to n-1) (readonly).
     is_time_continuous : boolean
         True if the data is continuous in the time domain, False if it is discrete (readonly).
     node : movia.core.classes.node.Node
         The node where this stream comes from (readonly).
         Allows back propagation in the assembly graph.
-    node_main : movia.core.classes.node.Node
-        The node used for the compilation. This node has the same output_streams
-        as ``node`` but not nescessary the same input_streams and te same properties.
-        It can be used for factorisation (read and write).
     """
 
     def __init__(self, node):
         """
         Parameters
         ----------
         node : movia.core.classes.node.Node
             The node where this stream comes from.
             The audit must be conducted in the children's classes.
             It is not done here in order to avoid cyclic imports.
         """
         self._node = node
-        self._node_main = node
 
     def __eq__(self, other) -> bool:
         """
         ** 2 streams are equivalent if their parent nodes are similar. **
         """
         if self.__class__ != other.__class__:
             return False
@@ -73,28 +67,26 @@
     def _stream_from_parent_node(node, index):
         """
         ** Return the equivalent stream contained in the parent node. **
         """
         return node.out_streams[index]
 
     @property
-    @abc.abstractmethod
-    def beginning(self) -> fractions.Fraction:
+    def beginning(self) -> numbers.Real:
         """
         ** The stream beginning instant in second. **
         """
-        raise NotImplementedError
+        return 0
 
     @property
-    @abc.abstractmethod
-    def duration(self) -> typing.Union[fractions.Fraction, float]:
+    def duration(self) -> numbers.Real:
         """
-        ** The duration of the flow in seconds, positive fraction or infinite **
+        ** Default infinite flow duration, can be overwritten. **
         """
-        raise NotImplementedError
+        return math.inf
 
     @property
     def index(self) -> int:
         """
         ** The stream index from the parent node (0 to n-1). **
         """
         indexs = [index for index, stream in enumerate(self.node.out_streams) if stream is self]
@@ -114,37 +106,14 @@
     def node(self):
         """
         ** The node where this stream comes from. **
         """
         return self._node
 
     @property
-    def node_main(self):
-        """
-        ** The global node, can be an alias to the classic node. **
-        """
-        return self._node_main
-
-    @node_main.setter
-    def node_main(self, new_node):
-        """
-        ** Change the node if this stream is already present in the new node at the same place. **
-        """
-        for i, stream in enumerate(new_node.out_streams):
-            if stream is self:
-                if self.index != i:
-                    raise AttributeError(
-                        f"the index of the stream {self} in the node {self.node} is {self.index}, "
-                        f"but it is {i} in the node {new_node}"
-                    )
-                self._node_main = new_node
-                return
-        raise AttributeError(f"the stream {self} is not in the node {new_node}")
-
-    @property
     @abc.abstractmethod
     def type(self) -> str:
         """
         ** The type of stream, 'audio', 'subtitle' or 'video'. **
         """
         raise NotImplementedError
 
@@ -172,19 +141,15 @@
         """
         super().__init__(node)
         assert isinstance(index, numbers.Integral) and index >= 0, index
         assert len(node.in_streams) > index, f"only {len(node.in_streams)} streams, no {index}"
         self._index = int(index)
 
     @property
-    def beginning(self) -> fractions.Fraction:
-        return self.stream.beginning
-
-    @property
-    def duration(self) -> typing.Union[fractions.Fraction, float]:
+    def duration(self) -> numbers.Real:
         return self.stream.duration
 
     @property
     def index(self) -> int:
         """
         ** The stream index from the parent node (0 to n-1). **
         """
```

### Comparing `movia-1.0.0b3/movia/core/classes/stream_audio.py` & `movia-1.0a1/movia/core/classes/stream_audio.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,111 +2,105 @@
 
 """
 ** Defines the structure of an abstract audio stream. **
 --------------------------------------------------------
 """
 
 import abc
-import fractions
 import numbers
 import typing
 
+import numpy as np
+
 from movia.core.classes.filter import Filter
-from movia.core.classes.frame_audio import FrameAudio
 from movia.core.classes.stream import Stream, StreamWrapper
+from movia.core.exceptions import OutOfTimeRange
 
 
 
 class StreamAudio(Stream):
     """
     ** Representation of any audio stream. **
 
     Attributes
     ----------
     channels : int
         The number of tracks (readonly).
     """
 
-    @abc.abstractmethod
-    def _snapshot(self, timestamp: fractions.Fraction, rate: int, samples: int) -> FrameAudio:
-        raise NotImplementedError
-
     @property
     @abc.abstractmethod
     def channels(self) -> int:
         """
         ** The number of channels in this audio stream. **
         """
         raise NotImplementedError
 
-    def snapshot(self,
-        timestamp: numbers.Real,
-        rate: typing.Optional[numbers.Integral]=None,
-        samples: numbers.Integral=1,
-    ) -> FrameAudio:
+    @abc.abstractmethod
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        raise NotImplementedError
+
+    def snapshot(
+        self, timestamp: typing.Union[numbers.Real, np.ndarray[numbers.Real]]
+    ) -> np.ndarray[numbers.Real]:
         """
         ** Extract the closest values to the requested date. **
 
         Parameters
         ----------
-        timestamp : numbers.Real
-            The absolute time expressed in seconds, not relative to the beginning of the audio.
-            Is the instant of the first sample of the returned frame.
-            For avoid the inacuracies of round, it is recomended to use fractional number.
-        rate : numbers.Integral, optional
-            If samples == 1, this argument is ignored. Otherwise is the samplerate of the frame.
-            If provide and samples != 1, allows to deduce the timestamps of the non 0 samples.
-            If non provide and samples != 1, try to call the `rate` attribute of the stream.
-        samples : numbers.Integral, default=1
-            The number of audio samples per channels to catch.
+        timestamps : numbers.Real or np.ndarray[numbers.Real]
+            The time expressed in seconds since the beginning of the audio.
+            Vector in 0 or 1 dimension.
 
         Returns
         -------
-        samples : FrameAudio
+        sample : np.ndarray[numbers.Real]
             Audio samples corresponding to the times provided.
             This vector is of shape (nbr_channels, *timestamp_shape).
             The values are between -1 and 1.
 
         Raises
         ------
         movia.core.exception.OutOfTimeRange
-            If we try to get a frame out of the definition range.
-            The valid range is [self.beginning, self.beginning+self.duration].
-            The range taken is [timestamp, timestamp + samples/rate[.
-        AttributeError
-            If the `rate` attribute has to be defined but is not provides or deductable.
-        """
-        # verifications on input
-        assert isinstance(samples, numbers.Integral), samples.__class__.__name__
-        samples = int(samples)
-        assert samples > 0, samples
-        if rate is None:
-            if samples != 1:
-                if (rate := getattr(self, "rate", None)) is None:
-                    raise ValueError("rate attribute has to be provide")
-            else:
-                rate = 1 # ignore default unused stupid value
-        assert isinstance(rate, numbers.Integral), rate.__class__.__name__
-        rate = int(rate)
-        assert rate > 0, rate
-        assert isinstance(timestamp, numbers.Real), timestamp.__class__.__name__
-        timestamp = fractions.Fraction(timestamp)
-
-        # extract samples
-        frame = self._snapshot(timestamp, rate, samples)
-
-        # result verification
-        assert isinstance(frame, FrameAudio), frame.__class__.__name__
-        return frame
+            If we try to read a sample at a negative time or after the end of the stream.
+        """
+        # cast
+        timestamp = np.asarray(timestamp)
+        if timestamp.ndim != 1:
+            return self.snapshot(timestamp.ravel()).reshape((-1, *timestamp.shape))
+
+        # verification
+        if timestamp.dtype == np.dtype("O"):
+            assert all(isinstance(o, numbers.Real) for o in timestamp), timestamp
+            timestamp = timestamp.astype(np.float64)
+        else:
+            assert issubclass(timestamp.dtype.type, numbers.Real), timestamp.dtype.type
+        t_min = np.min(timestamp)
+        if t_min < 0:
+            raise OutOfTimeRange(f"there is no audio frame at timestamp {t_min} (need >= 0)")
+
+        # evaluation
+        sample = self._snapshot(timestamp)
+
+        # verification
+        assert sample.shape[1:] == timestamp.shape, (sample.shape, timestamp.shape)
+        if sample.dtype == np.dtype("O"):
+            assert all(isinstance(o, numbers.Real) for o in sample), sample
+        else:
+            assert issubclass(sample.dtype.type, numbers.Real), sample.dtype.type
+        sample_no_nan = np.nan_to_num(sample)
+        assert -1 <= np.min(sample_no_nan) and np.max(sample_no_nan) <= 1, \
+            (np.nanmin(sample), np.nanmax(sample))
+
+        return sample
 
     @property
     def type(self) -> str:
         return "audio"
 
-
 class StreamAudioWrapper(StreamWrapper, StreamAudio):
     """
     ** Allows to dynamically transfer the methods of an instanced audio stream. **
 
     This can be very useful for implementing filters.
     """
 
@@ -121,13 +115,13 @@
             0 for the first, 1 for the second ...
         """
         assert isinstance(node, Filter), node.__class__.__name__
         assert len(node.in_streams) > index, f"only {len(node.in_streams)} streams, no {index}"
         assert isinstance(node.in_streams[index], StreamAudio), "the stream must be audio type"
         super().__init__(node, index)
 
-    def _snapshot(self, timestamp: fractions.Fraction, rate: int, samples: int) -> FrameAudio:
-        return self.stream._snapshot(timestamp, rate, samples)
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        return self.stream._snapshot(timestamp)
 
     @property
     def channels(self) -> int:
         return self.stream.channels
```

### Comparing `movia-1.0.0b3/movia/core/classes/stream_video.py` & `movia-1.0a1/movia/core/classes/stream_video.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 """
 ** Defines the structure of an abstract video stream. **
 --------------------------------------------------------
 """
 
 import abc
-import fractions
-import math
 import numbers
 
-import torch
+import av
 
 from movia.core.classes.filter import Filter
-from movia.core.classes.frame_video import FrameVideo
 from movia.core.classes.stream import Stream, StreamWrapper
+from movia.core.exceptions import OutOfTimeRange
 
 
 
 class StreamVideo(Stream):
     """
     ** Representation of any video stream. **
 
@@ -28,15 +26,15 @@
         Height of the image in pixels (readonly).
     is_space_continuous : boolean
         True if the data is continuous in the spacial domain, False if it is discrete (readonly).
     width : int
         Width of the image in pixels (readonly).
     """
 
-    def _snapshot(self, timestamp: fractions.Fraction) -> FrameVideo:
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
         raise NotImplementedError
 
     @property
     def height(self) -> int:
         """
         ** Height of all images in the stream. **
         """
@@ -48,46 +46,38 @@
     @abc.abstractmethod
     def is_space_continuous(self) -> bool:
         """
         ** True if the data is continuous in the spacial domain, False if it is discrete. **
         """
         raise NotImplementedError
 
-    def snapshot(self, timestamp: numbers.Real, *, channels=None) -> FrameVideo:
+    def snapshot(self, timestamp: numbers.Real) -> av.video.frame.VideoFrame:
         """
         ** Extract the closest frame to the requested date. **
 
         Parameters
         ----------
         timestamp : numbers.Real
-            The absolute time expressed in seconds, not relative to the beginning of the video.
-            For avoid the inacuracies of round, it is recomended to use fractional number.
-        channels : int, optional
-            Impose the numbers of channels, apply convertion if nescessary.
-            For the interpretation of the layers, see ``movia.core.classes.frame_video.FrameVideo``.
+            The time expressed in seconds since the beginning of the video.
 
         Returns
         -------
-        frame : FrameVideo
+        frame : av.frame.Frame
             Video frame with metadata.
 
         Raises
         ------
         movia.core.exception.OutOfTimeRange
-            If we try to get a frame out of the definition range.
-            The valid range is [self.beginning, self.beginning+self.duration[..
+            If we try to read a frame at a negative time or after the end of the stream.
         """
         assert isinstance(timestamp, numbers.Real), timestamp.__class__.__name__
-        if math.isnan(timestamp): # default transparent video frame
-            frame = FrameVideo(0, torch.zeros((self.height, self.width, 2), dtype=torch.uint8))
-        else:
-            frame = self._snapshot(fractions.Fraction(timestamp))
-        if channels is not None:
-            frame = frame.convert(channels)
-        assert isinstance(frame, FrameVideo), frame.__class__.__name__
+        if timestamp < 0:
+            raise OutOfTimeRange(f"the timestamp must be positive or zero, it is {timestamp}")
+        frame = self._snapshot(float(timestamp))
+        assert isinstance(frame, av.video.frame.VideoFrame), frame.__class__.__name__
         return frame
 
     @property
     def type(self) -> str:
         return "video"
 
     @property
@@ -124,15 +114,15 @@
             0 for the first, 1 for the second ...
         """
         assert isinstance(node, Filter), node.__class__.__name__
         assert len(node.in_streams) > index, f"only {len(node.in_streams)} streams, no {index}"
         assert isinstance(node.in_streams[index], StreamVideo), "the stream must be video type"
         super().__init__(node, index)
 
-    def _snapshot(self, timestamp: fractions.Fraction) -> FrameVideo:
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
         return self.stream._snapshot(timestamp)
 
     @property
     def height(self) -> int:
         return self.stream.height
 
     @property
```

### Comparing `movia-1.0.0b3/movia/core/compilation/export/compatibility.py` & `movia-1.0a1/movia/core/compilation/export/compatibility.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def __init__(self):
         self.codecs_cache = WriteInfos.codecs_init()
         self.encoders_cache = WriteInfos.encoders_init()
         self.muxers_cache = WriteInfos.muxers_init()
         self._compatibilites = {} # all tested combinaisons of (encodec, format) -> is_compatible
 
-    def check_compatibilities(
+    def check_compatibilites(
         self, encodecs: list[str], muxers: list[str]
     ) -> np.ndarray:
         """
         ** Asynchronously checks codec combinations. **
 
         Parameters
         ----------
@@ -82,42 +82,23 @@
             The muxer (format) names.
 
         Returns
         -------
         compatibility_matrix : np.ndarray[bool]
             The 2d boolean compatibility matrix.
             Item (i, j) is True if encodecs[i] is compatible with muxers[j].
-
-        Examples
-        --------
-        >>> from movia.core.compilation.export.compatibility import WriteInfos
-        >>> WriteInfos().check_compatibilities(["h264", "libx265", "opus"], ["matroska", "ogg"])
-        array([[ True, False],
-               [ True, False],
-               [ True,  True]])
-        >>> WriteInfos().check_compatibilities([], [])
-        array([], shape=(1, 0), dtype=bool)
-        >>> WriteInfos().check_compatibilities(["opus"], [])
-        array([], shape=(1, 0), dtype=bool)
-        >>> WriteInfos().check_compatibilities([], ["ogg"])
-        array([], shape=(1, 0), dtype=bool)
-        >>>
         """
         assert isinstance(encodecs, list), encodecs.__class__.__name__
         assert all(isinstance(ec, str) for ec in encodecs), encodecs
         assert set(encodecs).issubset(self.codecs|self.encoders), \
             set(encodecs)-(self.codecs|self.encoders)
         assert isinstance(muxers, list), muxers.__class__.__name__
         assert all(isinstance(f, str) for f in muxers), muxers
         assert set(muxers).issubset(self.muxers), set(muxers)-self.muxers
 
-        # case empty:
-        if len(encodecs) == 0 or len(muxers) == 0:
-            return np.asarray([[]], dtype=bool) # oblige for keep 2d array homogeneous
-
         # makes checks
         if (ecs_ms := [
             ec_m for ec_m in itertools.product(encodecs, muxers) if ec_m not in self._compatibilites
         ]): # only for optimisation
             encodecs_cache = {**self.codecs_cache, **self.encoders_cache}
             with multiprocessing.pool.ThreadPool() as pool: # subprocess release the GIL
                 for encodec_and_muxer, is_compatible in zip(
@@ -268,22 +249,37 @@
         >>>
         """
         assert isinstance(muxer, str), muxer.__class__.__name__
         assert muxer in self.muxers, f"{muxer} not in {self.muxers}"
 
         if "codecs" not in self.muxers_cache[muxer]:
             all_codecs = list(self.codecs)
-            mask = self.check_compatibilities(all_codecs, [muxer])[:, 0]
+            mask = self.check_compatibilites(all_codecs, [muxer])[:, 0]
             codecs = set(np.asarray(all_codecs, dtype=object)[mask])
             self.muxers_cache[muxer]["codecs"] = codecs
         return self.muxers_cache[muxer]["codecs"]
 
     def get_encoder_doc(self, encoder: str) -> str:
         r"""
         ** Retrive the ffmpeg documentation of this encoder. **
+
+        Examples
+        --------
+        >>> from pprint import pprint
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
+        >>> pprint(WriteInfos().get_encoder_doc("libvorbis"))
+        ('Encoder libvorbis [libvorbis]:\n'
+         '    General capabilities: dr1 delay small \n'
+         '    Threading capabilities: none\n'
+         '    Supported sample formats: fltp\n'
+         'libvorbis AVOptions:\n'
+         '  -iblock            <double>     E...A...... Sets the impulse block bias '
+         '(from -15 to 0) (default 0)\n'
+         '\n')
+        >>>
         """
         assert isinstance(encoder, str), encoder.__class__.__name__
         assert encoder in self.encoders, f"{encoder} not in {self.encoders}"
 
         if self.encoders_cache[encoder].get("doc") is None:
             self.encoders_cache[encoder]["doc"] = subprocess.run(
                 ["ffmpeg", "-v", "error", "-h", f"encoder={encoder}"],
@@ -306,22 +302,44 @@
         assert muxer in self.muxers, f"{muxer} not in {self.muxers}"
 
         if "encoders" not in self.muxers_cache[muxer]:
             all_encoders = [
                 encoder for codec in self.get_codecs_for_muxer(muxer)
                 for encoder in CodecInfos(codec).encoders
             ] # more optimised than list(self.encoders)
-            mask = self.check_compatibilities(all_encoders, [muxer])[:, 0]
+            mask = self.check_compatibilites(all_encoders, [muxer])[:, 0]
             encoders = set(np.asarray(all_encoders, dtype=object)[mask])
             self.muxers_cache[muxer]["encoders"] = encoders
         return self.muxers_cache[muxer]["encoders"]
 
     def get_muxer_doc(self, muxer: str) -> str:
         r"""
         ** Retrive the ffmpeg documentation of this format. **
+
+        Examples
+        --------
+        >>> from pprint import pprint
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
+        >>> pprint(WriteInfos().get_muxer_doc("ogg"))
+        ('Muxer ogg [Ogg]:\n'
+         '    Common extensions: ogg.\n'
+         '    Mime type: application/ogg.\n'
+         '    Default video codec: theora.\n'
+         '    Default audio codec: vorbis.\n'
+         'Ogg (audio/video/Speex/Opus) muxer AVOptions:\n'
+         '  -serial_offset     <int>        E.......... serial number offset (from 0 '
+         'to INT_MAX) (default 0)\n'
+         '  -oggpagesize       <int>        E.......... Set preferred Ogg page size. '
+         '(from 0 to 65025) (default 0)\n'
+         '  -pagesize          <int>        E.......... preferred page size in bytes '
+         '(deprecated) (from 0 to 65025) (default 0)\n'
+         '  -page_duration     <int64>      E.......... preferred page duration, in '
+         'microseconds (from 0 to I64_MAX) (default 1000000)\n'
+         '\n')
+        >>>
         """
         assert isinstance(muxer, str), muxer.__class__.__name__
         assert muxer in self.muxers, f"{muxer} not in {self.muxers}"
 
         doc = self.muxers_cache[muxer].get("doc") or subprocess.run(
             ["ffmpeg", "-v", "error", "-h", f"muxer={muxer}"],
             capture_output=True, check=True,
@@ -340,15 +358,15 @@
         ['asf', 'asf_stream', 'avi', ..., 'vob', 'webm', 'wtv']
         >>>
         """
         assert isinstance(codec, str), codec.__class__.__name__
         assert codec in self.codecs, f"{codec} not in {self.codecs}"
 
         all_muxers = list(self.muxers)
-        mask = self.check_compatibilities([codec], all_muxers)[0, :]
+        mask = self.check_compatibilites([codec], all_muxers)[0, :]
         muxers = set(np.asarray(all_muxers, dtype=object)[mask])
         self.codecs_cache[codec]["muxers"] = muxers
         return muxers
 
     @property
     def muxers(self) -> set[str]:
         """
@@ -413,16 +431,16 @@
         Notes
         -----
         No real tests are performed, it is just a documentation parsing.
 
         Examples
         --------
         >>> from movia.core.compilation.export.compatibility import CodecInfos
-        >>> sorted(CodecInfos("opus").encoders)
-        ['libopus', 'opus']
+        >>> sorted(CodecInfos("av1").encoders)
+        ['libaom-av1', 'librav1e', 'libsvtav1']
         >>>
         """
         return self.infos.codecs_cache[self.name]["encoders"]
 
     @property
     def decoding_supported(self):
         """
@@ -532,16 +550,31 @@
         'av1'
         >>>
         """
         return self.infos.encoders_cache[self.name]["codec"]
 
     @property
     def doc(self) -> str:
-        """
+        r"""
         ** The ffmpeg documentation about this encoder. **
+
+        Examples
+        --------
+        >>> from pprint import pprint
+        >>> from movia.core.compilation.export.compatibility import EncoderInfos
+        >>> pprint(EncoderInfos("libvorbis").doc)
+        ('Encoder libvorbis [libvorbis]:\n'
+         '    General capabilities: dr1 delay small \n'
+         '    Threading capabilities: none\n'
+         '    Supported sample formats: fltp\n'
+         'libvorbis AVOptions:\n'
+         '  -iblock            <double>     E...A..... Sets the impulse block bias '
+         '(from -15 to 0) (default 0)\n'
+         '\n')
+        >>>
         """
         return self.infos.get_encoder_doc(self.name)
 
     @property
     def experimental(self) -> bool:
         """
         ** True if the encoder is experimental. **
@@ -645,33 +678,32 @@
     @property
     def codecs(self) -> set[str]:
         """
         ** Tests all codecs to find the compatibles. **
         """
         return self.infos.get_codecs_for_muxer(self.name)
 
-    def contains_encodecs(self, encodecs: typing.Iterable[str]) -> bool:
+    def contains_codecs(self, codecs: typing.Iterable[str]) -> bool:
         """
         ** Returns True if this muxer support all the given codecs. **
 
         Examples
         --------
         >>> from movia.core.compilation.export.compatibility import MuxerInfos
-        >>> MuxerInfos("ogg").contains_encodecs(["theora", "vorbis"])
+        >>> MuxerInfos("ogg").contains_codecs(["theora", "vorbis"])
         True
-        >>> MuxerInfos("ogg").contains_encodecs(["h264"])
+        >>> MuxerInfos("ogg").contains_codecs(["h264"])
         False
         >>>
         """
-        assert hasattr(encodecs, "__iter__"), encodecs.__class__.__name__
-        encodecs = list(encodecs)
-        assert all(isinstance(e, str) for e in encodecs), encodecs
-        assert set(encodecs).issubset(self.infos.codecs|self.infos.encoders), \
-            set(encodecs)-(self.infos.codecs|self.infos.encoders)
-        return self.infos.check_compatibilities(encodecs, [self.name]).all()
+        assert hasattr(codecs, "__iter__"), codecs.__class__.__name__
+        codecs = list(codecs)
+        assert all(isinstance(codec, str) for codec in codecs), codecs
+        assert set(codecs).issubset(self.infos.codecs), set(codecs)-self.infos.codecs
+        return self.infos.check_compatibilites(codecs, [self.name]).all()
 
     @property
     def default_codecs(self) -> dict[str, str]:
         """
         ** Extract the default codecs from the documentation. **
 
         Notes
@@ -691,22 +723,44 @@
             match["type"]: match["codec"] for match in re.finditer(pattern, self.doc)
             if match["codec"] in self.infos.codecs
         }
         if not default:
             return {}
         codecs = list(default.values())
         codecs_rank = {c: i for i, c in enumerate(codecs)}
-        codecs_ok = self.infos.check_compatibilities(codecs, [self.name])[:, 0]
+        codecs_ok = self.infos.check_compatibilites(codecs, [self.name])[:, 0]
         default = {t: c for t, c in default.items() if codecs_ok[codecs_rank[c]]}
         return default
 
     @property
     def doc(self) -> str:
-        """
+        r"""
         ** The ffmpeg documentation about this codec. **
+
+        Examples
+        --------
+        >>> from pprint import pprint
+        >>> from movia.core.compilation.export.compatibility import MuxerInfos
+        >>> pprint(MuxerInfos("ogg").doc)
+        ('Muxer ogg [Ogg]:\n'
+         '    Common extensions: ogg.\n'
+         '    Mime type: application/ogg.\n'
+         '    Default video codec: theora.\n'
+         '    Default audio codec: vorbis.\n'
+         'Ogg (audio/video/Speex/Opus) muxer AVOptions:\n'
+         '  -serial_offset     <int>        E.......... serial number offset (from 0 '
+         'to INT_MAX) (default 0)\n'
+         '  -oggpagesize       <int>        E.......... Set preferred Ogg page size. '
+         '(from 0 to 65025) (default 0)\n'
+         '  -pagesize          <int>        E.......... preferred page size in bytes '
+         '(deprecated) (from 0 to 65025) (default 0)\n'
+         '  -page_duration     <int64>      E.......... preferred page duration, in '
+         'microseconds (from 0 to I64_MAX) (default 1000000)\n'
+         '\n')
+        >>>
         """
         return self.infos.get_muxer_doc(self.name)
 
     @property
     def encoders(self) -> set[str]:
         """
         ** Tests all encoders to find the compatibles. **
@@ -773,40 +827,25 @@
             raise KeyError(f"{suffix} not in {sorted(all_suffix)}")
         muxers = all_suffix[suffix.lower()]
         if len(muxers) == 1:
             return cls(muxers.pop())
 
         # if we have to choose
         muxers = [cls(name) for name in muxers]
-
-        # 1 choice, if one of the muxer supports only this extension
-        if len(criteria := [m for m in muxers if m.extensions == {suffix}]) == 1:
-            return criteria.pop()
-        if len(criteria) > 0:
-            muxers = criteria
-
-        # 2 choice, the variety of available type.
-        cost = {"audio": 2, "video": 4, "subtitle": 1}
-        best = max(criteria := [{cost[CodecInfos(c).type] for c in m.codecs} for m in muxers])
-        if len(criteria := [m for m, cost in zip(muxers, criteria) if cost == best]) == 1:
-            return criteria.pop()
-        muxers = criteria
-
-        # 3 choice, the number of available codecs
-        best = max(criteria := [len(m.codecs) for m in muxers])
-        if len(criteria := [m for m, cost in zip(muxers, criteria) if cost == best]) == 1:
-            return criteria.pop()
-        muxers = criteria
-
-        # 4 choice, the lenght of the documentation
-        best = max(criteria := [len(m.doc) for m in muxers])
-        if len(criteria := [m for m, cost in zip(muxers, criteria) if cost == best]) == 1:
-            return criteria.pop()
-
-        raise NotImplementedError(f"no more criteria for choose {criteria} for {suffix}")
+        # 1 choice, the number of available codecs
+        criteria = [len(mux.codecs) for mux in muxers]
+        best = max(criteria)
+        if len([c for c in criteria if c == best]) == 1:
+            return muxers[criteria.index(best)]
+        # 2 choice, the lenght of the documentation
+        criteria = [len(mux.doc) for mux in muxers]
+        best = max(criteria)
+        if len([c for c in criteria if c == best]) == 1:
+            return muxers[criteria.index(best)]
+        raise NotImplementedError
 
     def get_all(self) -> dict[str]:
         """
         ** Get the complete dictionary. **
         """
         return {
             "codecs": self.codecs,
```

### Comparing `movia-1.0.0b3/movia/core/compilation/export/default.py` & `movia-1.0a1/movia/core/compilation/export/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,10 +95,10 @@
         if stream.type == "audio":
             streams_settings.append({"codec": encodec, "rate": find_optimal_audio_rate(stream)})
         elif stream.type == "video":
             streams_settings.append(
                 {"codec": encodec, "rate": str(find_optimal_video_rate(stream))}
             )
         else:
-            raise NotImplementedError(f"not yet supported {stream.type}")
-    container_settings = {"format": muxer, "options": {}, "container_options": {}}
+            raise TypeError(f"not yet supported {stream.type}")
+    container_settings = {"format": "matroska", "options": {}, "container_options": {}}
     return filename, streams_settings, container_settings
```

### Comparing `movia-1.0.0b3/movia/core/compilation/export/encodec.py` & `movia-1.0a1/movia/core/compilation/export/encodec.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/core/compilation/export/rate_audio.py` & `movia-1.0a1/movia/core/compilation/export/rate_audio.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/core/compilation/export/rate_video.py` & `movia-1.0a1/movia/core/compilation/export/rate_video.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/core/compilation/graph_to_ast.py` & `movia-1.0a1/movia/core/compilation/graph_to_ast.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 ---------------------------------------------------------------------
 """
 
 import ast
 import inspect
 import pathlib
 import re
-import time
 import unidecode
 
 import networkx
 
-from movia.core.classes.container import ContainerOutput
 from movia.core.classes.node import Node
 from movia.utils import get_project_root
 
 
 
 def _node_to_ast(
     node_name: str, graph: networkx.MultiDiGraph
 ) -> tuple[ast.FunctionDef, list[ast.ImportFrom]]:
-    '''
+    """
     ** Creates the ast Function of this node. **
 
     Parameters
     ----------
     node_name : str
         The node name to compile.
     graph : networkx.MultiDiGraph
@@ -48,53 +46,49 @@
 
     Examples
     --------
     >>> import ast
     >>> from movia.core.classes.container import ContainerOutput
     >>> from movia.core.compilation.graph_to_ast import _node_to_ast
     >>> from movia.core.compilation.tree_to_graph import tree_to_graph
-    >>> from movia.core.filters.basic.translate import FilterTranslate
+    >>> from movia.core.filters.basic.truncate import FilterTruncate
     >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
     >>>
     >>> gen = GeneratorAudioNoise.default()
-    >>> filter_2 = FilterTranslate(gen.out_streams, 10)
-    >>> filter_1 = FilterTranslate(filter_2.out_streams, -5)
+    >>> filter_2 = FilterTruncate(gen.out_streams, 10)
+    >>> filter_1 = FilterTruncate(filter_2.out_streams, 1)
     >>> graph = tree_to_graph(ContainerOutput(filter_1.out_streams))
     >>>
     >>> func, modules = _node_to_ast("container_output_1", graph)
     >>> print(ast.unparse(func))
-    def get_container_output_1(filter_translate_1: Node) -> ContainerOutput:
-        """** Creation of the node 'container_output_1'. **"""
+    def get_container_output_1(filter_truncate_1: Node) -> ContainerOutput:
         container_output_1 = ContainerOutput.__new__(ContainerOutput)
-        container_output_1.setstate([filter_translate_1.out_streams[0]], state={})
+        container_output_1.setstate([filter_truncate_1.out_streams[0]], state={})
         return container_output_1
-    >>> func, modules = _node_to_ast("filter_translate_1", graph)
+    >>> func, modules = _node_to_ast("filter_truncate_1", graph)
     >>> print(ast.unparse(func))
-    def get_filter_translate_1(filter_translate_2: Node) -> FilterTranslate:
-        """** Creation of the node 'filter_translate_1'. **"""
-        filter_translate_1 = FilterTranslate.__new__(FilterTranslate)
-        filter_translate_1.setstate([filter_translate_2.out_streams[0]], state={'delay': '-5'})
-        return filter_translate_1
+    def get_filter_truncate_1(filter_truncate_2: Node) -> FilterTruncate:
+        filter_truncate_1 = FilterTruncate.__new__(FilterTruncate)
+        filter_truncate_1.setstate([filter_truncate_2.out_streams[0]], state={'duration_max': '1'})
+        return filter_truncate_1
     >>> func, modules = _node_to_ast("generator_audio_noise_1", graph)
     >>> print(ast.unparse(func))
     def get_generator_audio_noise_1() -> GeneratorAudioNoise:
-        """** Creation of the node 'generator_audio_noise_1'. **"""
         generator_audio_noise_1 = GeneratorAudioNoise.__new__(GeneratorAudioNoise)
         generator_audio_noise_1.setstate([], state={'seed': 0.0})
         return generator_audio_noise_1
     >>>
-    '''
+    """
     modules = []
     body = []
     name = _node_name_to_var_name(node_name)
 
-    # typing annotation returns type and doctring
+    # typing annotaion returns type
     returns = ast.Name(id=graph.nodes[node_name]["class"].__name__, ctx=ast.Load())
     modules.append(_class_to_ast(graph.nodes[node_name]["class"]))
-    body.append(ast.Expr(value=ast.Str(f"** Creation of the node {repr(node_name)}. **")))
 
     # node creation statement
     in_var_index = [
         (_node_name_to_var_name(src), int(key.split("->")[0]))
         for src, _, key in graph.in_edges(node_name, keys=True)
     ]
     state = ast.parse(repr(graph.nodes[node_name]["state"]), mode="eval").body
@@ -136,14 +130,15 @@
                             for var, ind in in_var_index
                         ],
                         ctx=ast.Load(),
                     )
                 ],
                 keywords=[ast.keyword(arg="state", value=state)],
             ),
+            type_ignores=[],
         )
     )
 
     # return statement
     body.append(
         ast.Return(value=ast.Name(id=name, ctx=ast.Load()))
     )
@@ -309,15 +304,15 @@
         name = name.replace("__", "_")
     if name[0].isdigit():
         name = "_" + name
     return name
 
 
 def graph_to_ast(graph: networkx.MultiDiGraph) -> ast.Module:
-    '''
+    """
     ** Creates the complete source code module from the assembly graph. **
 
     Parameters
     ----------
     graph : networkx.MultiDiGraph
         The assembly graph.
 
@@ -334,129 +329,84 @@
     >>> from movia.core.compilation.graph_to_ast import graph_to_ast
     >>> from movia.core.compilation.tree_to_graph import tree_to_graph
     >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
     >>> graph = tree_to_graph(ContainerOutput(GeneratorAudioNoise.default().out_streams))
     >>> graph_to_ast(graph) # doctest: +ELLIPSIS
     <ast.Module object at ...>
     >>> print(ast.unparse(_))
-    """
-    ** Autogenerated project exportation script. **
-    -----------------------------------------------
-    <BLANKLINE>
-    Creation: ...
-    Graph: MultiDiGraph with 2 nodes and 1 edges
-    """
     from movia.core.classes.container import ContainerOutput
     from movia.core.classes.node import Node
     from movia.core.generation.audio.noise import GeneratorAudioNoise
     <BLANKLINE>
     def get_container_output_1(generator_audio_noise_1: Node) -> ContainerOutput:
-        """** Creation of the node 'container_output_1'. **"""
         container_output_1 = ContainerOutput.__new__(ContainerOutput)
         container_output_1.setstate([generator_audio_noise_1.out_streams[0]], state={})
         return container_output_1
     <BLANKLINE>
     def get_generator_audio_noise_1() -> GeneratorAudioNoise:
-        """** Creation of the node 'generator_audio_noise_1'. **"""
         generator_audio_noise_1 = GeneratorAudioNoise.__new__(GeneratorAudioNoise)
         generator_audio_noise_1.setstate([], state={'seed': 0.0})
         return generator_audio_noise_1
     <BLANKLINE>
     def get_complete_tree() -> ContainerOutput:
-        """** Retrives the complete assembly graph. **"""
         generator_audio_noise_1 = get_generator_audio_noise_1()
         container_output_1 = get_container_output_1(generator_audio_noise_1)
         return container_output_1
     if __name__ == '__main__':
         get_complete_tree().write()
     >>>
-    '''
+    """
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
 
     body = []
     imps = []
 
-    # get_final node_name
-    final_var = [n for n, data in graph.nodes.data() if issubclass(data["class"], ContainerOutput)]
-    if len(final_var) != 1:
-        raise RuntimeError(f"must have exactly one ContainerOutput node, {final_var} founded")
-    final_var = _node_name_to_var_name(final_var.pop())
-
-    # extract each final lines in arbitrary order
-    sequence = [] # (ast_func, in_args_set, out_var)
+    sequence = [] # index 0 -> bottom, output, index final -> top
     for node in sorted(graph): # sorted for repetability
-        ast_func, imp = _node_to_ast(node, graph)
-        body.append(ast_func)
+        func, imp = _node_to_ast(node, graph)
+        body.append(func)
         imps.extend(imp)
-        sequence.append(
-            (
-                ast_func, # ast.FunctionDef
-                {ast_arg.arg for ast_arg in ast_func.args.args}, # set[str], input variable
-                _node_name_to_var_name(node), # str, output variable
-            )
-        )
 
-    # sorted func call position in an executable sequence order o(n**2)
-    sorted_sequence = [] # index final -> bottom, output; index 0 -> top
-    defines_out = set()
-    while sequence:
-        for i, (_, in_args_set, out_var) in enumerate(sequence.copy()):
-            if in_args_set.issubset(defines_out):
-                sorted_sequence.append(sequence.pop(i))
-                defines_out.add(out_var)
-                break
-        else:
-            raise RuntimeError("cycle found")
-        if out_var == final_var:
-            break
+        # locate func call position in an executable sequence order o(n**2)
+        out_var = _node_name_to_var_name(node)
+        ref = 0
+        for i, (_, args, _) in enumerate(sequence):
+            if out_var in args: # if func[i] input need curent node func output
+                ref = i + 1
+        sequence.insert(ref, (func, {ast_arg.arg for ast_arg in func.args.args}, out_var))
 
     # import management and simplification
     imps = _mod_sort_factor(imps)
     body = imps + body
 
     # main func management
     tree_body = []
-    for ast_func, in_args_set, out_var in sorted_sequence:
-        tree_body.append(
+    for func, args, out_var in sequence:
+        tree_body.insert(
+            0,
             ast.Assign(
                 targets=[ast.Name(id=out_var, ctx=ast.Store())],
                 value=ast.Call(
-                    func=ast.Name(id=ast_func.name, ctx=ast.Load()),
-                    args=[ast.Name(id=arg, ctx=ast.Load()) for arg in sorted(in_args_set)],
+                    func=ast.Name(id=func.name, ctx=ast.Load()),
+                    args=[ast.Name(id=arg, ctx=ast.Load()) for arg in sorted(args)],
                     keywords=[],
                 ),
             ),
         )
-    tree_body.append(ast.Return(value=ast.Name(id=sorted_sequence[-1][2], ctx=ast.Load())))
-    tree_body.insert(0, ast.Expr(value=ast.Str("** Retrives the complete assembly graph. **")))
+    tree_body.append(ast.Return(value=ast.Name(id=sequence[0][2], ctx=ast.Load())))
     body.append(
         ast.FunctionDef(
             name="get_complete_tree",
             args=ast.arguments(posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[]),
             body=tree_body,
             decorator_list=[],
-            returns=sorted_sequence[-1][0].returns,
+            returns=sequence[0][0].returns,
         )
     )
 
-    # doctstring creation
-    body.insert(
-        0,
-        ast.Expr(
-            value=ast.Str(
-                "\n"
-                "** Autogenerated project exportation script. **\n"
-                "-----------------------------------------------\n"
-                "\n"
-                f"Creation: {time.ctime()}\n"
-                f"Graph: {graph}\n"
-            ),
-        ),
-    )
-
     # main script execution
     body.append(
         ast.If(
             test=ast.Compare(
                 left=ast.Name(id="__name__", ctx=ast.Load()),
                 ops=[ast.Eq()],
                 comparators=[ast.Constant(value="__main__")],
```

### Comparing `movia-1.0.0b3/movia/core/compilation/graph_to_json.py` & `movia-1.0a1/movia/core/generation/audio/empty.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,76 @@
 #!/usr/bin/env python3
 
 """
-** Helper for serialisation of assembly graph **
-------------------------------------------------
+** Dedicated to tests, it is an empty audio stream containing no samples. **
+----------------------------------------------------------------------------
 """
 
 
-import inspect
-import pathlib
+import numbers
+import typing
 
-import networkx
+import numpy as np
 
-from movia.core.classes.node import Node
-from movia.utils import get_project_root
+from movia.core.classes.container import ContainerInput
+from movia.core.classes.stream import Stream
+from movia.core.classes.stream_audio import StreamAudio
+from movia.core.exceptions import OutOfTimeRange
 
 
 
-def _node_cls_to_string(cls: type) -> str:
+class GeneratorAudioEmpty(ContainerInput):
     """
-    ** Convert a Node class in str. **
-
-    Bijection with ``movia.core.compilation.json_to_graph._string_to_node_cls`` function.
-
-    Parameters
-    ----------
-    cls : type
-        The movia.core.classes.node.Node subclass.
-
-    Returns
-    -------
-    str
-        The relative import path of the class.
+    ** Contains an empty audio stream. **
 
     Examples
     --------
-    >>> from movia.core.compilation.graph_to_json import _node_cls_to_string
-    >>> from movia.core.classes.node import Node
-    >>> _node_cls_to_string(Node)
-    'classes.node.Node'
+    >>> from movia.core.exceptions import OutOfTimeRange
+    >>> from movia.core.generation.audio.empty import GeneratorAudioEmpty
+    >>> (stream,) = GeneratorAudioEmpty().out_streams
+    >>> try:
+    ...     _ = stream.snapshot(0)
+    ...     print("unreachable")
+    ... except OutOfTimeRange as err:
+    ...     print(err)
+    ...
+    this stream does not contain any samples
     >>>
     """
-    assert issubclass(cls, Node), cls.__name__
-    root_parts = pathlib.Path(
-        inspect.getsourcefile(cls)).resolve().relative_to(get_project_root() / "core"
-    ).with_suffix("").parts
-    cls_str = ".".join(root_parts) + "." + cls.__name__
-    return cls_str
 
+    def __init__(self):
+        out_streams = [_StreamAudioEmpty(self)]
+        super().__init__(out_streams)
 
-def graph_to_json(graph: networkx.MultiDiGraph) -> dict[str]:
-    """
-    ** Creates the complete json serializable dictionary of the assembly graph. **
+    @classmethod
+    def default(cls):
+        return cls()
 
-    Reverse operation with ``movia.core.compilation.json_to_graph.json_to_graph`` function.
+    def getstate(self) -> dict:
+        return {}
 
-    Parameters
-    ----------
-    graph : networkx.MultiDiGraph
-        The assembly graph.
-
-    Returns
-    -------
-    dict[str]
-        The equivalent graph (without cache) in the dictionary form.
+    def setstate(self, in_streams: typing.Iterable[Stream], state: dict) -> None:
+        assert state == {}, state
+        GeneratorAudioEmpty.__init__(self)
 
-    Examples
-    --------
-    >>> from pprint import pprint
-    >>> from movia.core.classes.container import ContainerOutput
-    >>> from movia.core.compilation.graph_to_json import graph_to_json
-    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
-    >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
-    >>> graph = tree_to_graph(ContainerOutput(GeneratorAudioNoise.default().out_streams))
-    >>> pprint(graph_to_json(graph))
-    {'edges': [['generator_audio_noise_1', 'container_output_1', '0->0']],
-     'nodes': {'container_output_1': {'class': 'classes.container.ContainerOutput',
-                                      'state': {}},
-               'generator_audio_noise_1': {'class': 'generation.audio.noise.GeneratorAudioNoise',
-                                           'state': {'seed': 0.0}}}}
-    >>>
+
+class _StreamAudioEmpty(StreamAudio):
     """
-    assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
+    ** An audio stream containing no sample. **
+    """
+
+    is_time_continuous = True
 
-    json_dict = {
-        "edges": sorted((list(e) for e in graph.edges)),
-        "nodes": {
-            node: {
-                "class": _node_cls_to_string(data["class"]),
-                "state": data["state"],
-            }
-            for node, data in graph.nodes.data()
-        }
-    }
-    return json_dict
+    def __init__(self, node: GeneratorAudioEmpty):
+        assert isinstance(node, GeneratorAudioEmpty), node.__class__.__name__
+        super().__init__(node)
+
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        raise OutOfTimeRange("this stream does not contain any samples")
+
+    @property
+    def channels(self) -> int:
+        raise KeyError("it makes no sense to give a number of channels to an absence of sample")
+
+    @property
+    def duration(self) -> numbers.Real:
+        return 0
```

### Comparing `movia-1.0.0b3/movia/core/compilation/graph_to_tree.py` & `movia-1.0a1/movia/core/compilation/graph_to_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     ** Recursively retrieve the node corresponding to the node of the graph. **
 
     Complete the ``tree`` attribute for this node and for the out streams of this node.
     This function is recursive, so all ancestors are also completed.
 
     Parameters
     ----------
-    node_name : str
+    node : str
         The name of the node that allows to determine the corresponding subgraph.
     graph : networkx.MultiDiGraph
         The complete assembly graph.
 
     Notes
     -----
     If the node is a terminal node, it is the complete dynamic tree.
     """
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
     assert isinstance(node_name, str), node_name.__class__.__name__
-    assert node_name in graph.nodes, sorted(graph.nodes)
+    assert node_name in graph.nodes(), sorted(graph.nodes())
 
     # create node and recursively the parent nodes
     node = graph.nodes[node_name]
     if node["tree"] is None:
         for pred in graph.predecessors(node_name):
             _tree_from_node(pred, graph) # editing by pointer
         in_edges = graph.in_edges(node_name, keys=True)
@@ -97,15 +97,15 @@
     >>>
     """
     # verification and extraction of the termination node
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
     out_nodes = [n for n in graph.nodes if issubclass(graph.nodes[n]["class"], ContainerOutput)]
     assert len(out_nodes) == 1, f"only one output node is possible, not {len(out_nodes)}"
     out_node = out_nodes.pop()
-    assert issubclass(graph.nodes[out_node]["class"], ContainerOutput), \
+    assert issubclass(graph.nodes()[out_node]["class"], ContainerOutput), \
         graph.nodes[out_node]["class"].__name__
 
     # fill
     update_tree(graph)
     container_out = graph.nodes[out_node]["tree"]
     return container_out
 
@@ -190,11 +190,11 @@
         else: # obsolete case (need update)
             node["hash"] = new_hash
             node["tree"] = None
             for edge_name in graph.out_edges(node_name, keys=True):
                 graph.add_edge(*edge_name, tree=None)
 
     # complete graph
-    out_nodes = [node for node in graph.nodes if graph.out_degree(node) == 0]
+    out_nodes = [node for node in graph.nodes() if graph.out_degree(node) == 0]
     assert out_nodes, "the graph is empty or contains cycle"
     for node_name in out_nodes:
         _tree_from_node(node_name, graph)
```

### Comparing `movia-1.0.0b3/movia/core/compilation/tree_to_graph.py` & `movia-1.0a1/movia/core/compilation/tree_to_graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         if _names[id(node)] in graph:
             return None
 
     current_node_name = _node_name(graph, node, _names=_names)
     graph.add_node(current_node_name, **{"class": node.__class__, "state": node.getstate()})
 
     for index_dst, stream in enumerate(node.in_streams):
-        new_node_name = _node_name(graph, stream.node_main, _names=_names)
-        _complete_graph(graph, stream.node_main, _names=_names)
+        new_node_name = _node_name(graph, stream.node, _names=_names)
+        _complete_graph(graph, stream.node, _names=_names)
         key = f"{stream.index}->{index_dst}"
         graph.add_edge(new_node_name, current_node_name, key)
 
     return None
 
 
 def _node_name(graph: networkx.MultiDiGraph, node: Node, *, _names: dict) -> str:
@@ -138,35 +138,26 @@
     assembly_graph : networkx.MultiDiGraph
         The strictly equivalent assembly graph.
 
     Examples
     --------
     >>> from pprint import pprint
     >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.graph_to_tree import graph_to_tree
     >>> from movia.core.compilation.tree_to_graph import tree_to_graph
-    >>> from movia.core.filters.basic.chain import FilterChain
-    >>> from movia.core.filters.basic.truncate import FilterTruncate
-    >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
-    >>>
-    >>> (s_audio_0,) = FilterTruncate(GeneratorAudioNoise(0).out_streams, 10).out_streams
-    >>> (s_audio_1,) = GeneratorAudioNoise(.5).out_streams
-    >>> (s_chain_audio,) = FilterChain([s_audio_0, s_audio_1]).out_streams
-    >>> graph = tree_to_graph(ContainerOutput([s_chain_audio]))
-    >>>
-    >>> pprint(sorted(graph.nodes))
-    ['container_output_1',
-     'filter_chain_1',
-     'filter_truncate_1',
-     'generator_audio_noise_1',
-     'generator_audio_noise_2']
-    >>> pprint(sorted(graph.edges))
-    [('filter_chain_1', 'container_output_1', '0->0'),
-     ('filter_truncate_1', 'filter_chain_1', '0->0'),
-     ('generator_audio_noise_1', 'filter_truncate_1', '0->0'),
-     ('generator_audio_noise_2', 'filter_chain_1', '0->1')]
+    >>> from movia.core.io.read import ContainerInputFFMPEG
+    >>> container_out = ContainerOutput(ContainerInputFFMPEG.default().out_streams)
+    >>> graph = tree_to_graph(container_out)
+    >>> pprint(list(graph.nodes))
+    ['container_output_1', 'container_input_ffmpeg_1']
+    >>> pprint(list(graph.edges))
+    [('container_input_ffmpeg_1', 'container_output_1', '0->0'),
+     ('container_input_ffmpeg_1', 'container_output_1', '1->1'),
+     ('container_input_ffmpeg_1', 'container_output_1', '2->2'),
+     ('container_input_ffmpeg_1', 'container_output_1', '3->3')]
     >>>
     """
     assert isinstance(container_out, ContainerOutput), container_out.__class__.__name__
 
     graph = networkx.MultiDiGraph(title="assembly graph")
     _complete_graph(graph, container_out, _names={})
```

### Comparing `movia-1.0.0b3/movia/core/edit/operation/add.py` & `movia-1.0a1/movia/core/edit/operation/add.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/core/edit/operation/remove.py` & `movia-1.0a1/movia/core/edit/operation/remove.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/core/exceptions.py` & `movia-1.0a1/movia/core/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,47 +4,42 @@
 ** Groups the exceptions specific to ``movia``. **
 --------------------------------------------------
 
 Rather than returning too general exceptions, these exceptions allow a much more precise debugging.
 """
 
 
-
 class MoviaException(Exception):
     """
     ** Base class for exceptions specific to this module. **
     """
 
-
 class MissingFrameError(MoviaException, OSError):
     """
     ** When a frame is missing in a stream. **
 
     This exception can be thrown if the reded frames have a strange behavior.
     """
 
-
 class MissingInformation(MoviaException, ValueError):
     """
     ** When information is unreadable or missing from the metadata. **
 
     It can be raised when trying to access a tag that is not defined
     or that returns a surprising value.
     """
 
-
 class MissingStreamError(MoviaException, OSError):
     """
     ** When a stream is missing in a file. **
 
     This exception can be raised when looking for a video,
     audio or image stream in a media that does not contain any or that is unreadable.
     """
 
-
 class OutOfTimeRange(MoviaException, EOFError):
     """
     ** Access outside the definition range **
 
     This exception is raised when accessing or writing
     outside the range in which the stream is defined.
     """
```

### Comparing `movia-1.0.0b3/movia/core/filters/basic/chain.py` & `movia-1.0a1/movia/core/generation/video/empty.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 #!/usr/bin/env python3
 
 """
-** Allows you to temporarily concatenate several streams. **
-------------------------------------------------------------
+** Dedicated to tests, it is an empty video stream containing no frames. **
+---------------------------------------------------------------------------
 """
 
 
-import logging
-import math
+import numbers
 import typing
 
-from movia.core.classes.meta_filter import MetaFilter
-from movia.core.classes.node import Node
+import av
+
+from movia.core.classes.container import ContainerInput
 from movia.core.classes.stream import Stream
-from movia.core.filters.basic.add import FilterAdd
-from movia.core.filters.basic.translate import FilterTranslate
+from movia.core.classes.stream_video import StreamVideo
+from movia.core.exceptions import OutOfTimeRange
 
 
 
-class FilterChain(MetaFilter):
+class GeneratorVideoEmpty(ContainerInput):
     """
-    ** Concatenate the streams end-to-end. **
+    ** Contains an empty video stream. **
 
     Examples
     --------
-    >>> import torch
-    >>> from movia.core.filters.basic.chain import FilterChain
-    >>> from movia.core.filters.basic.truncate import FilterTruncate
-    >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
-    >>> from movia.core.generation.video.noise import GeneratorVideoNoise
-    >>>
-    >>> (s_audio_0,) = FilterTruncate(GeneratorAudioNoise(0).out_streams, 10).out_streams
-    >>> (s_audio_1,) = GeneratorAudioNoise(.5).out_streams
-    >>> (s_chain_audio,) = FilterChain([s_audio_0, s_audio_1]).out_streams
-    >>> (s_video_0,) = FilterTruncate(GeneratorVideoNoise(0, (3, 3)).out_streams, 10).out_streams
-    >>> (s_video_1,) = GeneratorVideoNoise(.5, (3, 3)).out_streams
-    >>> (s_chain_video,) = FilterChain([s_video_0, s_video_1]).out_streams
-    >>>
-    >>> (
-    ...     s_chain_audio.snapshot(0, 1, 20) == torch.cat(
-    ...         (s_audio_0.snapshot(0, 1, 10), s_audio_1.snapshot(0, 1, 10)), axis=1
-    ...     )
-    ... ).all()
-    tensor(True)
-    >>> (s_video_0.snapshot(0) == s_chain_video.snapshot(0)).all()
-    tensor(True)
-    >>> (s_video_1.snapshot(0) == s_chain_video.snapshot(10)).all()
-    tensor(True)
-    >>> (s_video_1.snapshot(10) == s_chain_video.snapshot(20)).all()
-    tensor(True)
+    >>> from movia.core.exceptions import OutOfTimeRange
+    >>> from movia.core.generation.video.empty import GeneratorVideoEmpty
+    >>> (stream,) = GeneratorVideoEmpty().out_streams
+    >>> try:
+    ...     _ = stream.snapshot(0)
+    ...     print("unreachable")
+    ... except OutOfTimeRange as err:
+    ...     print(err)
+    ...
+    this stream does not contain any frames
     >>>
     """
 
-    def _compile(self, in_streams: tuple[Stream]) -> Node:
-        streams = [in_streams[0]] # can not raise IndexError because none empty
-        pos = streams[0].beginning + streams[0].duration
-        for i, stream in enumerate(in_streams[1:]):
-            if pos == math.inf:
-                logging.warning("the stream %i is infinite, can not chain an other stream after", i)
-                break
-            streams.append(FilterTranslate([stream], pos - stream.beginning).out_streams[0])
-            pos += stream.duration
-        return FilterAdd(streams)
+    def __init__(self):
+        out_streams = [_StreamVideoEmpty(self)]
+        super().__init__(out_streams)
 
     @classmethod
     def default(cls):
-        return cls([])
+        return cls()
 
     def getstate(self) -> dict:
         return {}
 
     def setstate(self, in_streams: typing.Iterable[Stream], state: dict) -> None:
-        assert state == {}
-        FilterChain.__init__(self, in_streams)
+        assert state == {}, state
+        GeneratorVideoEmpty.__init__(self)
+
+
+class _StreamVideoEmpty(StreamVideo):
+    """
+    ** A video stream containing no frames. **
+    """
+
+    is_space_continuous = False
+    is_time_continuous = False
+
+    def __init__(self, node: GeneratorVideoEmpty):
+        assert isinstance(node, GeneratorVideoEmpty), node.__class__.__name__
+        super().__init__(node)
+
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
+        raise OutOfTimeRange("this stream does not contain any frames")
+
+    @property
+    def duration(self) -> numbers.Real:
+        return 0
+
+    @property
+    def height(self) -> int:
+        raise KeyError("it makes no sense to give a dimension to an absence of frames")
+
+    @property
+    def width(self) -> int:
+        raise KeyError("it makes no sense to give a dimension to an absence of frames")
```

### Comparing `movia-1.0.0b3/movia/core/filters/basic/translate.py` & `movia-1.0a1/movia/core/filters/basic/truncate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,131 @@
 #!/usr/bin/env python3
 
 """
-** Allows you to temporarily translate a sequence. **
------------------------------------------------------
+** Allows you to temporarily limit a sequence. **
+-------------------------------------------------
 """
 
+
+
 import fractions
+import math
 import numbers
 import typing
 
+import av
+import numpy as np
+
 from movia.core.classes.filter import Filter
-from movia.core.classes.frame_audio import FrameAudio
-from movia.core.classes.frame_video import FrameVideo
 from movia.core.classes.stream import Stream
-from movia.core.classes.stream_audio import StreamAudioWrapper
-from movia.core.classes.stream_video import StreamVideoWrapper
+from movia.core.classes.stream_audio import StreamAudio, StreamAudioWrapper
+from movia.core.classes.stream_video import StreamVideo, StreamVideoWrapper
+from movia.core.exceptions import OutOfTimeRange
+from movia.core.generation.audio.noise import GeneratorAudioNoise
+from movia.core.generation.video.noise import GeneratorVideoNoise
 
 
 
-class FilterTranslate(Filter):
+class FilterTruncate(Filter):
     """
-    ** Change the beginning time of a stream. **
+    ** Shortens the duration of a stream. **
 
     Attributes
     ----------
-    delay : fractions.Fraction
-        The delay append to the original beginning time of the stream (readonly).
-        a positive value indicates that the output flow is later than the input flow.
-
-    Examples
-    --------
-    >>> from movia.core.filters.basic.translate import FilterTranslate
-    >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
-    >>> from movia.core.generation.video.noise import GeneratorVideoNoise
-    >>>
-    >>> (s_base_audio,) = GeneratorAudioNoise(0).out_streams
-    >>> (s_base_video,) = GeneratorVideoNoise(0, (3, 3)).out_streams
-    >>> s_trans_audio, s_trans_video = FilterTranslate([s_base_audio, s_base_video], 10).out_streams
-    >>>
-    >>> (s_base_audio.snapshot(0) == s_trans_audio.snapshot(10)).all()
-    tensor(True)
-    >>> (s_base_video.snapshot(0) == s_trans_video.snapshot(10)).all()
-    tensor(True)
-    >>> (s_base_audio.snapshot(10) == s_trans_audio.snapshot(10)).all()
-    tensor(False)
-    >>> (s_base_video.snapshot(10) == s_trans_video.snapshot(10)).all()
-    tensor(False)
-    >>>
+    duration_max : fractions.Fraction
+        The maximum duration beyond which the flows do not return anything (readonly).
     """
 
-    def __init__(self, in_streams: typing.Iterable[Stream], delay: numbers.Real):
+    def __init__(self, in_streams: typing.Iterable[Stream], duration_max: numbers.Real):
         """
         Parameters
         ----------
         in_streams : typing.Iterable[Stream]
             Forwarded to ``movia.core.classes.filter.Filter``.
-        delay : numbers.Real
-            The temporal translation value to apply at the output stream.
+        duration_max : numbers.Real
+            The streams will be cut strictly after this duration in seconds.
         """
         assert hasattr(in_streams, "__iter__"), in_streams.__class__.__name__
         in_streams = tuple(in_streams)
         assert all(isinstance(stream, Stream) for stream in in_streams), \
             [stream.__class__.__name__ for stream in in_streams]
-        assert isinstance(delay, numbers.Real), delay.__class__.__name__
+        assert isinstance(duration_max, numbers.Real), duration_max.__class__.__name__
+        assert duration_max >= 0, duration_max
 
-        self._delay = fractions.Fraction(delay)
-        super().__init__(in_streams, in_streams)
-        super().__init__(
-            self.in_streams, # not in_stream without self because generator can be exausted
-            [
-                (
-                    {"audio": _StreamAudioTranslate, "video": _StreamVideoTranslate}
-                )[in_stream.type](self, index) for index, in_stream in enumerate(self.in_streams)
-            ]
+        try:
+            self._duration_max = fractions.Fraction(duration_max)
+        except OverflowError:
+            self._duration_max = math.inf
+        super().__init__(in_streams, in_streams) # solve recusrive initialisation
+        out_streams = [
+            self._select_stream(in_stream, index) for index, in_stream in enumerate(in_streams)
+        ]
+        super().__init__(in_streams, out_streams)
+
+    def _select_stream(self, in_stream, index):
+        if isinstance(in_stream, StreamVideo):
+            return _StreamVideoTruncate(self, index)
+        if isinstance(in_stream, StreamAudio):
+            return _StreamAudioTruncate(self, index)
+        raise NotImplementedError(
+            f"the FilterTruncate does not support {in_stream.__class__.__name__} streams"
         )
 
     @classmethod
     def default(cls):
-        return cls([], 0)
+        audio_stream = GeneratorAudioNoise.default().out_streams[0]
+        video_stream = GeneratorVideoNoise.default().out_streams[0]
+        return cls([audio_stream, video_stream], 1)
 
     @property
-    def delay(self) -> fractions.Fraction:
+    def duration_max(self) -> fractions.Fraction:
         """
-        ** The delay append to the original beginning time of the stream. **
+        ** The maximum duration beyond which the flows do not return anything. **
         """
-        return self._delay
+        return self._duration_max
 
     def getstate(self) -> dict:
-        return {"delay": str(self.delay)}
+        return {"duration_max": str(self.duration_max)}
 
     def setstate(self, in_streams: typing.Iterable[Stream], state: dict) -> None:
-        assert set(state) == {"delay"}, set(state)-{"delay"}
-        FilterTranslate.__init__(self, in_streams, fractions.Fraction(state["delay"]))
-
-
-class _StreamAudioTranslate(StreamAudioWrapper):
-    """
-    ** Translate an audio stream from a certain delay. **
-    """
-
-    def _snapshot(self, timestamp: fractions.Fraction, rate: int, samples: int) -> FrameAudio:
-        frame = self.stream._snapshot(timestamp - self.node.delay, rate, samples)
-        frame = FrameAudio(frame.time + self.node.delay, rate, frame)
-        return frame
+        assert set(state) == {"duration_max"}, set(state)-{"duration_max"}
+        if state["duration_max"] == "inf":
+            duration_max = math.inf
+        else:
+            duration_max = fractions.Fraction(state["duration_max"])
+        FilterTruncate.__init__(self, in_streams, duration_max)
+
+
+class _StreamAudioTruncate(StreamAudioWrapper):
+    """
+    ** Truncates the end of a video stream after a certain time. **
+    """
+
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        if np.max(timestamp) >= self.beginning + self.duration:
+            raise OutOfTimeRange(
+                f"the stream has been truncated over {self.beginning+self.duration} seconds, "
+                f"evaluation at {np.max(timestamp)} seconds"
+            )
+        return self.stream._snapshot(timestamp)
 
     @property
-    def beginning(self) -> fractions.Fraction:
-        return self.stream.beginning + self.node.delay
+    def duration(self):
+        return min(self.node.duration_max, self.stream.duration)
 
 
-class _StreamVideoTranslate(StreamVideoWrapper):
+class _StreamVideoTruncate(StreamVideoWrapper):
     """
-    ** Translate a video stream from a certain delay. **
+    ** Truncates the end of a video stream after a certain time. **
     """
 
-    def _snapshot(self, timestamp: fractions.Fraction) -> FrameVideo:
-        frame = self.stream._snapshot(timestamp - self.node.delay)
-        frame = FrameVideo(frame.time + self.node.delay, frame)
-        return frame
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
+        if timestamp >= self.beginning + self.duration:
+            raise OutOfTimeRange(
+                f"the stream has been truncated over {self.beginning+self.duration} seconds, "
+                f"evaluation at {timestamp} seconds"
+            )
+        return self.stream._snapshot(timestamp)
 
     @property
-    def beginning(self) -> fractions.Fraction:
-        return self.stream.beginning + self.node.delay
+    def duration(self):
+        return min(self.node.duration_max, self.stream.duration)
```

### Comparing `movia-1.0.0b3/movia/core/generation/video/noise.py` & `movia-1.0a1/movia/core/generation/video/noise.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,25 @@
 
 """
 ** Generate a video noise signal. **
 ------------------------------------
 """
 
 import fractions
-import hashlib
-import math
 import numbers
 import random
 import struct
 import typing
 
-import torch
+import av
+import numpy as np
 
 from movia.core.classes.container import ContainerInput
-from movia.core.classes.frame_video import FrameVideo
 from movia.core.classes.stream import Stream
 from movia.core.classes.stream_video import StreamVideo
-from movia.core.exceptions import OutOfTimeRange
 
 
 
 class GeneratorVideoNoise(ContainerInput):
     """
     ** Generate a pure noise video signal. **
 
@@ -34,134 +31,107 @@
     shape : tuple[int, int]
         The vertical and horizontal (i, j) resolution of the image (readonly).
 
     Examples
     --------
     >>> from movia.core.generation.video.noise import GeneratorVideoNoise
     >>> stream = GeneratorVideoNoise(0, shape=(13, 9)).out_streams[0]
-    >>> stream.snapshot(0)[..., 0]
-    tensor([[ 11,  17, 169,  48,   9, 217, 124, 113, 195],
-            [ 51,  79, 173, 237, 176, 201, 124,  23, 177],
-            [167, 187,  49, 153, 107, 249, 128,  89,  51],
-            [174,  30, 173,  31, 127, 146, 134,   2, 123],
-            [ 19, 151,  41, 219,  95, 199, 138, 180, 188],
-            [177, 165,  63,  35, 177, 109, 134, 166, 154],
-            [121, 250, 175, 186,   3, 185, 254, 152,   4],
-            [193, 215, 220, 140, 151, 230, 148, 159, 213],
-            [114, 249, 218, 159, 148, 169, 192, 178, 154],
-            [ 80, 145, 195,  94, 102,  14, 190, 252,  45],
-            [ 32, 103, 243, 155,  61,   9, 116,  55, 134],
-            [255, 154, 249,  56, 146, 217,   0, 102,  48],
-            [ 68, 187,  91, 247, 247,  80, 113, 105,  77]], dtype=torch.uint8)
+    >>> stream.snapshot(0).to_ndarray(format="bgr24")[..., 0]
+    array([[ 95, 217,  15, 215, 248,  69, 205,  61,  29],
+           [ 19,  59,  81, 120, 208,  64,  89, 127, 128],
+           [ 76, 154,  95, 186, 220,   1, 237, 143,  96],
+           [ 55,  77, 208, 190, 120, 240, 100, 126, 149],
+           [115,   8, 207, 179, 166, 216, 247, 127,  58],
+           [220, 168,  51,  56,  20, 185, 214, 207, 108],
+           [ 58, 245, 104,   1, 209, 235, 169, 171, 142],
+           [ 54,  49,  65, 137,  26,  51,  98, 254,  38],
+           [ 63, 206,  24, 113, 243, 175,  57, 127, 188],
+           [215,  62, 105, 188,  99,  10, 175,  21, 148],
+           [179, 106, 241, 134,  27,   2,  24, 108,  95],
+           [179, 134, 227, 172, 121, 156, 136, 152, 165],
+           [107, 146,  45,   8, 163, 184,  36, 148, 158]], dtype=uint8)
     >>>
     """
-
-    def __init__(
-        self,
-        seed: numbers.Real=None,
-        shape: typing.Union[tuple[numbers.Integral, numbers.Integral], list[numbers.Integral]]=(
-            720,
-            720,
-        ),
+    def __init__(self,
+        seed: numbers.Real=None, shape: tuple[numbers.Integral, numbers.Integral]=(720, 720)
     ):
         """
         Parameters
         ----------
         seed : numbers.Real
             The random seed to have a repeatability.
             The value must be between 0 included and 1 excluded.
             If not provided, the seed is chosen randomly.
-        shape : tuple or list, optional
+        shape : tuple[number.Integral, number.Integral], optional
             The pixel dimensions of the generated frames.
             The convention adopted is the numpy convention (height, width)
         """
         # check
         if seed is None:
             seed = random.random()
         assert isinstance(seed, numbers.Real), seed.__class__.__name__
         assert 0 <= seed < 1, seed
-        assert isinstance(shape, (tuple, list)), shape.__class__.__name__
+        assert isinstance(shape, tuple), shape.__class__.__name__
         assert len(shape) == 2, shape
         assert all(isinstance(s, numbers.Integral) and s > 0 for s in shape)
 
         # declaration
         self._seed = float(seed)
         self._height, self._width = int(shape[0]), int(shape[1])
 
         # delegation
         super().__init__([_StreamVideoNoiseUniform(self)])
 
     @classmethod
     def default(cls):
-        return cls(0, [2, 2])
+        return cls(0)
 
     def getstate(self) -> dict:
         return {
             "seed": self.seed,
-            "shape": self.shape,
+            "shape": list(self.shape),
         }
 
     @property
     def seed(self):
         """
         ** The value of the seed between 0 and 1. **
         """
         return self._seed
 
     def setstate(self, in_streams: typing.Iterable[Stream], state: dict) -> None:
         keys = {"seed", "shape"}
-        assert set(state) == keys, set(state) - keys
-        GeneratorVideoNoise.__init__(self, seed=state["seed"], shape=state["shape"])
+        assert set(state) == keys, set(state)-keys
+        GeneratorVideoNoise.__init__(self, seed=state["seed"], shape=tuple(state["shape"]))
 
     @property
-    def shape(self) -> list[int, int]:
+    def shape(self) -> tuple[int, int]:
         """
         ** The vertical and horizontal (i, j) resolution of the image. **
         """
-        return [self._height, self._width]
+        return (self._height, self._width)
 
 
 class _StreamVideoNoiseUniform(StreamVideo):
     """
     ** Random video stream where each pixel follows a uniform law. **
     """
 
     is_space_continuous = True
     is_time_continuous = True
 
     def __init__(self, node: GeneratorVideoNoise):
         assert isinstance(node, GeneratorVideoNoise), node.__class__.__name__
         super().__init__(node)
 
-    def _snapshot(self, timestamp: fractions.Fraction) -> FrameVideo:
-        if timestamp < 0:
-            raise OutOfTimeRange(f"there is no audio frame at timestamp {timestamp} (need >= 0)")
-        return FrameVideo(
-            timestamp,
-            torch.randint(
-                0,
-                256,
-                (self.height, self.width, 3),
-                generator=torch.random.manual_seed(
-                    int.from_bytes(
-                        hashlib.md5(
-                            struct.pack(
-                                "dLL",
-                                self.node.seed,
-                                timestamp.numerator % (1 << 64),
-                                timestamp.denominator % (1 << 64),
-                            )
-                        ).digest(),
-                        byteorder="big",
-                    ) % (1 << 64) # solve RuntimeError: Overflow when unpacking long
-                ),
-                dtype=torch.uint8
-            ),
-        )
-
-    @property
-    def beginning(self) -> fractions.Fraction:
-        return fractions.Fraction(0)
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
+        # random number calculation
+        seed = struct.pack("dd", self.node.seed, timestamp)
+        gen = np.random.default_rng(int.from_bytes(seed, byteorder="big"))
+        img = gen.integers(0, 256, (self.height, self.width, 3), dtype=np.uint8, endpoint=False)
+
+        # av frame cast
+        frame = av.video.frame.VideoFrame.from_ndarray(img, format="bgr24")
+        frame.time_base = fractions.Fraction(1, 300300) # ppcm 1001, 25, 30, 60
+        frame.pts = round(timestamp / frame.time_base)
 
-    @property
-    def duration(self) -> typing.Union[fractions.Fraction, float]:
-        return math.inf
+        return frame
```

### Comparing `movia-1.0.0b3/movia/core/io/read.py` & `movia-1.0a1/movia/core/io/read.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,30 @@
 """
 ** Decodes the streams of a multimedia file based on ffmpeg. **
 ---------------------------------------------------------------
 """
 
 
 import fractions
-import logging
-import math
 import numbers
 import pathlib
-import threading
 import typing
 
 import av
 import numpy as np
-import torch
 
-from movia.core.analysis.audio.properties.duration import get_duration_audio
-from movia.core.analysis.stream import get_streams_type
-from movia.core.analysis.stream import _estimate_rate_ffmpeg
+from movia.core.analysis.streams import get_streams_type
+from movia.core.analysis.video.properties.framerate import get_fps
+from movia.core.analysis.video.properties.nb_frames import get_nb_frames
 from movia.core.classes.container import ContainerInput
-from movia.core.classes.frame_audio import FrameAudio
-from movia.core.classes.frame_video import FrameVideo
 from movia.core.classes.stream import Stream
 from movia.core.classes.stream_audio import StreamAudio
 from movia.core.classes.stream_video import StreamVideo
-from movia.core.exceptions import MissingInformation, MissingStreamError, OutOfTimeRange
+from movia.core.exceptions import (MissingInformation, MissingFrameError, MissingStreamError,
+    OutOfTimeRange)
 from movia.utils import get_project_root
 
 
 
 class ContainerInputFFMPEG(ContainerInput):
     """
     ** Allows to decode a multimedia file with ffmpeg. **
@@ -49,27 +44,30 @@
         ``av.error.InvalidDataError: [Errno 1094995529] Invalid data found when processing input;
         last error log: [libdav1d] Error parsing OBU data``
     Which happens when reading a multi-stream file sparingly, The instances of
     ``av.container.InputContainer`` are new for each stream.
 
     Examples
     --------
+    >>> import numpy as np
+    >>> from movia.core.classes.stream_audio import StreamAudio
+    >>> from movia.core.classes.stream_video import StreamVideo
     >>> from movia.core.io.read import ContainerInputFFMPEG
     >>> with ContainerInputFFMPEG("movia/examples/intro.mkv") as container:
     ...     for stream in container.out_streams:
-    ...         if stream.type == "video":
-    ...             stream.snapshot(0).shape
-    ...         elif stream.type == "audio":
-    ...             stream.snapshot(0, rate=2, samples=3)
+    ...         if isinstance(stream, StreamVideo):
+    ...             stream.snapshot(0).format
+    ...         if isinstance(stream, StreamAudio):
+    ...             stream.snapshot(np.array([0.0, 1.0]))
     ...
-    (720, 1280, 3)
-    (360, 640, 3)
-    FrameAudio(Fraction(0, 1), 2, [[        nan  0.13000917 -0.36198682]
-                                   [        nan  0.02201845  0.04206311]])
-    FrameAudio(Fraction(0, 1), 2, [[        nan  0.12514605 -0.28835574]])
+    <av.VideoFormat yuv420p, 1280x720>
+    <av.VideoFormat yuv420p, 640x360>
+    array([[        nan, -0.34764948],
+           [        nan,  0.07892987]], dtype=float32)
+    array([[        nan, -0.24758172]], dtype=float32)
     >>>
     """
 
     def __init__(self, filename: typing.Union[str, bytes, pathlib.Path], **av_kwargs):
         """
         Parameters
         ----------
@@ -133,15 +131,15 @@
         ContainerInputFFMPEG.__init__(self, state["filename"], **state["av_kwargs"])
 
     def close(self):
         """
         ** Close the file. **
         """
         for stream in self.out_streams:
-            stream.reset()
+            stream.close()
 
     @property
     def av_kwargs(self) -> dict[str]:
         """
         ** The parameters passed to ``av.open``. **
         """
         return self._av_kwargs
@@ -150,17 +148,27 @@
     def filename(self) -> pathlib.Path:
         """
         ** The path to the physical file that contains the extracted video stream. **
         """
         return self._filename
 
 
-class _StreamFFMPEGBase(Stream):
+class _StreamAudioFFMPEG(StreamAudio):
     """
-    ** Factorise share methods between audio and video. **
+    Attributes
+    ----------
+    duration : numbers.Real
+        The exact duration of the stream (readonly).
+        This date corresponds to the end of the last sample.
+    metadata : dict
+        The metadata associated with this stream (readonly).
+    samplerate : int
+        The frequency in Hz of the samples (readonly).
+    time_base : fractions.Fraction
+        The unit of time (in fractional seconds) in which timestamps are expressed (readonly).
     """
 
     is_time_continuous = False
 
     def __init__(self, node: ContainerInputFFMPEG):
         """
         Parameters
@@ -168,221 +176,171 @@
         node : movia.core.io.read.ContainerInputFFMPEG
             Simply allows to keep the graph structure.
         """
         assert isinstance(node, ContainerInputFFMPEG), node.__class__.__name__
         super().__init__(node)
 
         self._av_container = None
-        self._frame_iter = None
+        self._frame_iter = None # we can't recreate it every time because we lose the last frames
+        self._array_buff = [None, None]
         self._prec_frame = self._next_frame = None
-        self._rate = None # optimise about 100 ms par call
+        self._duration = None
 
-    def _seek_backward(self, position: fractions.Fraction) -> None:
+    def __iter__(self):
         """
-        ** Moves backwards in the file. **
-
-        This method guarantees to move before the required position.
-        If this is not possible, we move to the very beginning of the file.
-        After, we always have ``self.get_current_range()[0] <= position``.
+        ** Yields all frames and array of this stream starting from the current position. **
         """
-        if self.type == "audio":
-            dec = fractions.Fraction(self.av_container.streams[self.index].frame_size, self.rate)
-        elif self.type == "video":
-            dec = 1 / self.rate
-        else:
-            dec = 0
-        for pos in (position, position-10, 0):
-            stream = self.av_container.streams[self.index] # must be define in 'for' because reset
+        if self._prec_frame is None:
+            self._update_prec_next()
+        yield self._prec_frame, self._extract_array_prec()
+        if self._next_frame is not self._prec_frame:
+            yield self._next_frame, self._extract_array_next()
+        while True:
             try:
-                self.av_container.seek(
-                    max(0, math.floor((pos - 2*dec) / stream.time_base)),
-                    backward=True, # if there is not a keyframe at the given offset
-                    stream=stream
-                )
-            except av.error.PermissionError: # happens sometimes
-                self.reset()
+                yield self._update_prec_next(), self._extract_array_next()
+            except OutOfTimeRange:
                 break
-            self._prec_frame = self._next_frame = None # takes into account the new position
 
-            # verification and rough adjustment
-            try:
-                if self.get_current_range()[0] <= position:
-                    break
-            except OutOfTimeRange: # if this exception is throw, reset is just done
-                continue
-        else:
-            self.reset()
+    def _extract_array_next(self):
+        if self._array_buff[1] is None:
+            self._array_buff[1] = _clip_convert(self._next_frame.to_ndarray(format="bgr24"))
+        return self._array_buff[1]
+
+    def _extract_array_prec(self):
+        if self._array_buff[0] is None:
+            if self._prec_frame is None:
+                self._update_prec_next()
+            self._array_buff[0] = _clip_convert(self._prec_frame.to_ndarray(format="bgr24"))
+        return self._array_buff[0]
 
-    def _seek_forward(self, position: fractions.Fraction) -> None:
+    def _seek_backward(self, position: numbers.Real):
         """
-        ** Moves forwardwards in the file. **
+        ** Moves backwards in the file. **
 
-        The displacement, if some cases, can be very approximate.
+        This method guarantees to move before the required position.
+        If this is not possible, we move to the very beginning of the file.
         """
-        stream = self.av_container.streams[self.index]
-        if stream.type == "audio":
-            dec = fractions.Fraction(stream.frame_size, self.rate)
-        elif stream.type == "video":
-            dec = 1 / self.rate
-        else:
-            dec = 0
+        if self._prec_frame is None:
+            self._update_prec_next()
+
+        # adjusted displacement
+        seek_request = max(0, int(
+            (position - self._prec_frame.samples/self._prec_frame.rate)
+            / self._prec_frame.time_base
+        ))
         self.av_container.seek(
-            max(0, math.floor((position - dec) / stream.time_base)),
+            seek_request,
             backward=True, # if there is not a keyframe at the given offset
-            stream=stream
+            stream=self.av_container.streams[self.index]
         )
-        self._prec_frame = self._next_frame = None # takes into account the new position
+        self._frame_iter = None # takes into account the new position
+        self._array_buff = [None, None]
+        self._prec_frame = self._next_frame = None
+        self._update_prec_next()
 
-    @property
-    def av_container(self) -> av.container.Container:
+        # verification and rough adjustment
+        if seek_request != 0:
+            if position > _frame_dates(self._prec_frame)[0]:
+                self._seek_backward(0)
+
+    def _seek_forward(self, position: numbers.Real):
         """
-        ** Allows to read the file at the last moment. **
+        ** Moves forwardwards in the file. **
+
+        The displacement, if any, can be very approximate.
         """
-        if self._av_container is None:
-            self._av_container = av.open(str(self.node.filename), "r", **self.node.av_kwargs)
-        return self._av_container
+        self.av_container.seek(
+            max(0, round(position)),
+            backward=True, # if there is not a keyframe at the given offset
+            stream=self.av_container.streams[self.index]
+        )
 
-    @property
-    def beginning(self) -> fractions.Fraction:
-        return fractions.Fraction(0)
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        # borns extraction and simple verification
+        # must be accurate to avoid confusion for the final time
+        t_min = np.min(timestamp)
+        t_max = np.max(timestamp)
+        t_max = fractions.Fraction(t_max).limit_denominator(self.time_base.denominator)
+
+        # seeking if nescessary
+        self.seek(t_min) # seeks only for backward or big forward jump
+
+        # retrive and decode reference samples
+        references = []
+        for frame, array in self:
+            references.append((frame.is_corrupt, _frame_dates(frame), frame.rate, array))
+            if references[-1][1][1] > t_max + self.time_base: # a sample covers [t0, t0+dt[
+                break
+        else: # if the last frame is reached
+            if t_max >= references[-1][1][1]:
+                raise OutOfTimeRange(
+                    f"there is no audio frame at timestamp {t_max} "
+                    f"(need timestamp < {_frame_dates(self._next_frame)[1]})"
+                )
 
-    @property
-    def frame_iter(self) -> typing.Iterable[av.audio.frame.AudioFrame]:
-        """
-        ** Allows to read the file at the last moment. **
-        """
-        if self._frame_iter is None:
-            self._frame_iter = iter(self.av_container.decode(self.av_container.streams[self.index]))
-        return self._frame_iter
+        # verifications
+        if any(is_corrupt for is_corrupt, _, _, _ in references):
+            raise NotImplementedError("an audio frame is corrupted, this case is not handled")
+        if any(rate != self.samplerate for _, _, rate, _ in references):
+            raise NotImplementedError(f"samplerate ({self.samplerate}) doesn't match the frames")
+        cum_shifts = np.cumsum( # cumulative algebraic shifts
+            [
+                tf_prec-ti_next # the algebraic shifts
+                for (_, (_, tf_prec), _, _), (_, (ti_next, _), _, _)
+                in zip(references[:-1], references[1:])
+            ]
+        )
+        if any(np.abs(cum_shifts) >= self._av_container.streams[self.index].time_base):
+            raise MissingFrameError(
+                "there seems to be a gap between some frames, "
+                "here are the cumulative shifts between frames "
+                f"({', '.join(f'{s}={float(s):.4f}' for s in cum_shifts)})"
+            )
 
-    @property
-    def next_frame(self) -> typing.Optional[av.audio.frame.AudioFrame]:
-        """
-        ** The next frame if exists, None else. **
-        """
-        if self._next_frame is None:
-            self._prec_frame = self.prec_frame # iter if needed ("=" is for pylint W0104)
-            try:
-                self._next_frame = next(self.frame_iter)
-            except (StopIteration, av.error.EOFError):
-                self._next_frame = self._frame_iter = None
-                # if self._duration is None: # facultative, it is just optimisation
-                #     self._duration = frame_dates(self._prec_frame)[1]
-        return self._next_frame
+        # assembling references and get the nerest reference
+        t_ref = float(references[0][1][0])
+        samples_ref = np.concatenate([s for _, _, _, s in references], axis=1)
+        indexs = np.rint((timestamp-t_ref)*self.samplerate).astype(int) # not floor float inaccuracy
+        np.maximum(indexs, 0, out=indexs) # some stream doesn't start at t=0
+        np.minimum(indexs, samples_ref.shape[1]-1, out=indexs) # prevention agains IndexError
+        samples = np.where(timestamp<t_ref, np.nan, samples_ref[:, indexs])
+        return samples
+
+    def _update_prec_next(self) -> av.audio.frame.AudioFrame:
+        """
+        ** Iterates on the next audio frame. **
+
+        Returns
+        -------
+        _next_frame : av.audio.frame.AudioFrame
+            The newly decoded frame.
 
-    @property
-    def prec_frame(self) -> av.audio.frame.AudioFrame:
-        """
-        ** The frame at the current position. **
+        Raises
+        ------
+        OutOfTimeRange
+            If the last audio frame has already been reached.
         """
+        self._prec_frame, self._array_buff[0] = self._next_frame, self._array_buff[1]
+        try:
+            self._next_frame = next(self.frame_iter)
+        except StopIteration as err:
+            raise OutOfTimeRange("there is no audio frame left to read") from err
+        self._array_buff[1] = None
         if self._prec_frame is None:
-            try:
-                self._prec_frame = next(self.frame_iter)
-            except (StopIteration, av.error.EOFError) as err:
-                self.reset()
-                raise OutOfTimeRange("there is no frame left to read") from err
-        return self._prec_frame
+            self._prec_frame = self._next_frame
+        return self._next_frame
 
     @property
-    def rate(self) -> fractions.Fraction:
-        """
-        ** Theorical image or sample frequency in the metadata. **
-        """
-        if self._rate is None:
-            self._rate = _estimate_rate_ffmpeg(self.node.filename, self.index)
-        return self._rate
-
-    def reset(self) -> None:
+    def av_container(self) -> av.container.Container:
         """
-        ** Close the file and delete all internal state. **
+        ** Allows to read the file at the last moment. **
         """
-        if self._av_container is not None:
-            self._prec_frame = self._next_frame = None
-            self._frame_iter = None
-            self._av_container.close()
-            self._av_container = None
-
-
-class _StreamAudioFFMPEG(StreamAudio, _StreamFFMPEGBase):
-    """
-    Attributes
-    ----------
-    duration : fractions.Fraction
-        The exact duration of the stream (readonly).
-        This date corresponds to the end of the last sample.
-    rate : int
-        The frequency in Hz of the samples (readonly).
-    """
-
-    def __init__(self, node: ContainerInputFFMPEG):
-        super().__init__(node)
-        self._duration = None
-        self._lock = threading.Lock()
-
-    def _snapshot(self, timestamp: fractions.Fraction, rate: int, samples: int) -> FrameAudio:
-        if timestamp < 0:
-            raise OutOfTimeRange(f"there is no audio frame at timestamp {timestamp} (need >= 0)")
-
-        # resample if needeed
-        if samples != 1 and rate != self.rate:
-            frame = self._snapshot(
-                timestamp,
-                rate=self.rate,
-                samples=math.floor(samples*fractions.Fraction(self.rate, rate))
-            )
-            indexs = torch.arange(samples, dtype=torch.int64)
-            indexs *= self.rate
-            indexs //= rate
-            frame = FrameAudio(timestamp, rate, frame[:, indexs])
-            return frame
-
-        # decode concerned frames
-        slices = []
-        end = timestamp + fractions.Fraction(samples, rate) # apparition of last sample
-        with self._lock:
-            self.seek(timestamp)
-            while True:
-                try:
-                    prec_frame = self.prec_frame
-                except OutOfTimeRange as err:
-                    raise OutOfTimeRange(
-                        f"stream start {self.beginning} and end {self.beginning + self.duration}, "
-                        f"no stream at timestamp {timestamp} to {timestamp} + {samples}/{rate}"
-                    ) from err
-                if prec_frame.is_corrupt:
-                    logging.warning("the frame at %f seconds is corrupted", prec_frame.time)
-                    continue
-                dates = frame_dates(prec_frame)
-                slices.append((dates[0], prec_frame.to_ndarray(format="bgr24")))
-                if end <= dates[1]:
-                    break
-                self._prec_frame, self._next_frame = self._next_frame, None # next frame
-        slices = [(start, _convert_audio_samples(array)) for start, array in slices]
-
-        # create the new empty audio frame
-        dtypes = {a.dtype for _, a in slices}
-        dtypes = sorted(
-            dtypes, key=lambda t: {torch.float16: 2, torch.float32: 1, torch.float64: 0}
-        ) + [torch.float32] # if slice = []
-        frame = FrameAudio(
-            timestamp, rate, torch.full((self.channels, samples), torch.nan, dtype=dtypes[0])
-        )
-
-        # positionning of each slices
-        for start, array in slices:
-            index = math.ceil((start - timestamp) * rate) # time to index
-            if index < 0:
-                array = array[:, -index:]
-                index = 0
-            if index + array.shape[1] > samples: # if slice to long
-                array = array[:, :max(0, samples-index)]
-            if array.shape[1]:
-                frame[:, index:index+array.shape[1]] = array
-
-        return frame
+        if self._av_container is None:
+            self._av_container = av.open(str(self.node.filename), "r", **self.node.av_kwargs)
+        return self._av_container
 
     @property
     def channels(self) -> int:
         """
         ** The number of channels in this audio stream. **
 
         Examples
@@ -393,16 +351,23 @@
         ...     stream.channels
         ...
         1
         >>>
         """
         return self.av_container.streams[self.index].codec_context.channels
 
+    def close(self):
+        """
+        ** Close the file. **
+        """
+        if self._av_container is not None:
+            self._av_container.close()
+
     @property
-    def duration(self) -> typing.Union[fractions.Fraction, float]:
+    def duration(self) -> numbers.Real:
         """
         ** The exact duration in seconds. **
 
         Examples
         --------
         >>> from movia.core.io.read import ContainerInputFFMPEG
         >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
@@ -410,280 +375,420 @@
         ...     stream.duration
         ...
         Fraction(16, 1)
         >>>
         """
         if self._duration is not None:
             return self._duration
-        # seek approximative
-        rel_index = len(
-            [
-                None for i, s in enumerate(self.node.out_streams)
-                if i < self.index and s.type == "audio"
-            ]
-        )
-        with self._lock:
-            self.seek(get_duration_audio(self.node.filename, rel_index, accurate=False) - 10)
-            # decoding until reaching the last frame
-            while self.next_frame is not None:
-                self._prec_frame, self._next_frame = self._next_frame, None # iter in stream
-            # get the time of the last frame + the frame duration
-            self._duration = frame_dates(self._prec_frame)[1]
+
+        while True:
+            try:
+                self._update_prec_next()
+            except OutOfTimeRange:
+                break
+        self._duration = _frame_dates(self._next_frame)[1]
         return self._duration
 
-    def get_current_range(self) -> tuple[fractions.Fraction, fractions.Fraction]:
+    @property
+    def frame_iter(self) -> typing.Iterable:
         """
-        ** Returns the time interval cover by the current frame. **
+        ** Allows to read the file at the last moment. **
         """
-        if (next_frame := self.next_frame) is None:
-            return frame_dates(self.prec_frame)
-        return frame_dates(self.prec_frame)[0], frame_dates(next_frame)[0]
+        if self._frame_iter is None:
+            self._frame_iter = iter(
+                self.av_container.decode(self.av_container.streams[self.index])
+            )
+        return self._frame_iter
 
     @property
-    def rate(self) -> int:
+    def metadata(self) -> int:
         """
-        ** Theorical image or sample frequency in the metadata. **
-        """
-        return int(super().rate)
+        ** The metadata associated with this stream. **
 
-    def seek(self, position: fractions.Fraction) -> None:
+        Examples
+        --------
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
+        ...     (stream,) = container.out_streams
+        ...     stream.metadata
+        ...
+        {'encoder': 'Lavc59.37.100 libvorbis'}
+        >>>
         """
-        ** Moves into the file until reaching the frame at this position. **
-
-        If you are already well placed, this has no effect.
-        Allows backward even a little bit, but only jump forward if the jump is big enough.
+        return self.av_container.streams[self.index].metadata
 
-        Parameters
-        ----------
-        position : fraction.Fraction
-            The target position such as ``self.prec_frame.time <= position < self.next_frame.time``.
-            This position is expressed in seconds.
-
-        Raises
-        ------
-        OutOfTimeRange
-            If the required position is out of the definition range.
+    @property
+    def samplerate(self) -> int:
+        """
+        ** The frequency of the samples. **
 
         Examples
         --------
-        >>> from fractions import Fraction
         >>> from movia.core.io.read import ContainerInputFFMPEG
         >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
         ...     (stream,) = container.out_streams
-        ...     stream.seek(Fraction(15))
-        ...     stream.get_current_range()
-        ...     stream.seek(Fraction(5))
-        ...     stream.get_current_range()
+        ...     stream.samplerate
         ...
-        (Fraction(1872, 125), Fraction(1876, 125))
-        (Fraction(624, 125), Fraction(628, 125))
+        16000
         >>>
         """
-        assert isinstance(position, fractions.Fraction), position.__class__.__name__
+        return self.av_container.streams[self.index].codec_context.rate
+
+    def seek(self, position: numbers.Real):
+        """
+        ** Moves into the file. **
+
+        If you are already well placed, this has no effect.
+        Allows backward even a little bit, but only forward if the jump is big enough.
+        """
+        assert isinstance(position, numbers.Real), position.__class__.__name__
+        if self._prec_frame is None:
+            self._update_prec_next()
 
         # case need to seek
-        if position > self.get_current_range()[1] + 10: # forward if jump more 10 seconds
+        if (
+            position - 10 > (
+                _frame_dates(self._next_frame)[0]
+                + fractions.Fraction(self._next_frame.samples, self._next_frame.rate)
+            )
+        ): # take a leap forward (jump > 10 s)
             self._seek_forward(position) # very approximative
-        if position < self.get_current_range()[0]:
+        if position < _frame_dates(self._prec_frame)[0]:
             self._seek_backward(position) # guaranteed to be before
 
         # fine adjustment
-        while self.get_current_range()[1] <= position:
-            self._prec_frame, self._next_frame = self._next_frame, None # hack for iter in stream
+        while (
+            _frame_dates(self._next_frame)[0]
+            + fractions.Fraction(self._next_frame.samples, self._next_frame.rate)
+            < position
+        ):
+            self._update_prec_next()
 
+    @property
+    def time_base(self) -> fractions.Fraction:
+        """
+        ** The unit of time (in fractional seconds) in which timestamps are expressed. **
 
-class _StreamVideoFFMPEG(StreamVideo, _StreamFFMPEGBase):
+        Examples
+        --------
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
+        ...     (stream,) = container.out_streams
+        ...     stream.time_base
+        ...
+        Fraction(1, 16000)
+        >>>
+        """
+        return self.av_container.streams[self.index].time_base
+
+
+class _StreamVideoFFMPEG(StreamVideo):
     """
     Attributes
     ----------
-    duration : fractions.Fraction
-        The exact duration of the complete stream (readonly).
-        the time include the duration of the last frame.
+    duration : numbers.Real
+        The exact duration of the stream (readonly).
+        This date corresponds to the end of the last frame.
+    framerate : numbers.Real
+        Theoretical image frequency in the metadata (readonly).
+    nb_frames : int
+        The exact number of frames present in this stream (readonly).
+    time_base : fractions.Fraction
+        The unit of time (in fractional seconds) in which timestamps are expressed (readonly).
     """
 
     is_space_continuous = False
+    is_time_continuous = False
 
     def __init__(self, node: ContainerInputFFMPEG):
+        """
+        Parameters
+        ----------
+        node : movia.core.io.read.ContainerInputFFMPEG
+            Simply allows to keep the graph structure.
+        """
+        assert isinstance(node, ContainerInputFFMPEG), node.__class__.__name__
         super().__init__(node)
-        self._duration = None
+
+        self._av_container = None
         self._key_times = None
-        self._lock = threading.Lock()
+        self._frame_iter = None # we can't recreate it every time because we lose the last frames
+        self._prec_frame = self._next_frame = None
+        self._duration = None
+
+    def __iter__(self):
+        """
+        ** Yields all frames of this stream starting from the current position. **
+        """
+        if self._next_frame is None:
+            self._update_prec_next()
+        yield self._next_frame
+        while True:
+            try:
+                yield self._update_prec_next()
+            except OutOfTimeRange:
+                break
+
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
+        # ideal case (select the nearest)
+        if self._prec_frame is None:
+            self._update_prec_next()
+        if self._prec_frame.time <= timestamp <= self._next_frame.time:
+            delta_prec = timestamp - self._prec_frame.time
+            delta_next = self._next_frame.time - timestamp
+            return self._prec_frame if delta_prec <= delta_next else self._next_frame
+
+        key_prec, key_next = _born(self.key_times, timestamp)
+        if key_prec is None:
+            raise OutOfTimeRange(f"there is no frame at timestamp {timestamp} (need >= {key_next})")
 
-    def _snapshot(self, timestamp: fractions.Fraction) -> FrameVideo:
-        if timestamp < 0:
-            raise OutOfTimeRange(f"there is no audio frame at timestamp {timestamp} (need >= 0)")
-        with self._lock:
-            self.seek(timestamp) # adjust position
-            frame_av = self.prec_frame
-            return FrameVideo(frame_dates(frame_av)[0], frame_av.to_ndarray(format="bgr24"))
+        # case need seek (backward or big displacement)
+        if (
+            self._prec_frame.time > timestamp # back to the past
+            or self._next_frame.time < key_prec - .5 # take a leap forward (jump > 500 ms)
+        ):
+            self.av_container.seek(
+                1 + int(key_prec / self.av_container.streams[self.index].time_base),
+                backward=True, # if there is not a keyframe at the given offset
+                any_frame=False, # seek to any frame, not just a keyframe
+                stream=self.av_container.streams[self.index]
+            )
+            self._frame_iter = None # takes into account the new position
+
+        # decoding until reaching the right frame
+        try:
+            while timestamp > self._update_prec_next().time:
+                continue
+        except OutOfTimeRange as err: # management of the time overrun of the last frame
+            if timestamp >= self._next_frame.time + 1/self.framerate:
+                raise err
+            return self._next_frame
+        return self._snapshot(timestamp)
+
+    def _update_prec_next(self) -> av.video.frame.VideoFrame:
+        """
+        ** Iterates on the next frame. **
+
+        Raises
+        ------
+        OutOfTimeRange
+            If the last frame has already been reached.
+        """
+        self._prec_frame = self._next_frame
+        try:
+            self._next_frame = next(self.frame_iter)
+        except StopIteration as err:
+            raise OutOfTimeRange("there is no frame left to read") from err
+        if self._prec_frame is None:
+            self._prec_frame = self._next_frame
+        return self._next_frame
 
     @property
-    def duration(self) -> typing.Union[fractions.Fraction, float]:
+    def av_container(self) -> av.container.Container:
+        """
+        ** Allows to read the file at the last moment. **
+        """
+        if self._av_container is None:
+            self._av_container = av.open(str(self.node.filename), "r", **self.node.av_kwargs)
+        return self._av_container
+
+    def close(self):
+        """
+        ** Close the file. **
+        """
+        if self._av_container is not None:
+            self._av_container.close()
+
+    @property
+    def duration(self) -> numbers.Real:
         """
         ** The exact duration in seconds. **
 
         Examples
         --------
         >>> from movia.core.io.read import ContainerInputFFMPEG
         >>> with ContainerInputFFMPEG("movia/examples/video.mp4") as container:
         ...     (stream,) = container.out_streams
         ...     stream.duration
         ...
-        Fraction(16, 1)
+        16.0
         >>>
         """
         if self._duration is not None:
             return self._duration
-        with self._lock:
-            # jump if need
-            key_times = self.get_key_times()
-            if frame_dates(self.prec_frame)[0] < key_times[-1]:
-                self.seek(key_times[-1])
-            # decoding until reaching the last frame
-            while self.next_frame is not None:
-                self._prec_frame, self._next_frame = self._next_frame, None # iter in stream
-            # get the time of the last frame + the frame duration
-            self._duration = frame_dates(self._prec_frame)[0] + 1/self.rate
+        self._snapshot(self.key_times[-1])
+        self._duration = self.key_times[-1]
+        for frame in self:
+            self._duration = frame.time
+        assert self._duration is not None
+        self._duration += 1/self.framerate # duration of the last frame
         return self._duration
 
-    def get_key_times(self) -> np.ndarray[fractions.Fraction]:
+    @property
+    def frame_iter(self) -> typing.Iterable:
         """
         ** Allows to read the file at the last moment. **
+        """
+        if self._frame_iter is None:
+            self._frame_iter = iter(
+                self.av_container.decode(self.av_container.streams[self.index])
+            )
+        return self._frame_iter
 
-        Examples
-        --------
-        >>> from movia.core.io.read import ContainerInputFFMPEG
-        >>> with ContainerInputFFMPEG("movia/examples/video.mp4") as container:
-        ...     (stream,) = container.out_streams
-        ...     stream.get_key_times()
-        ...
-        array([Fraction(0, 1), Fraction(10, 1)], dtype=object)
-        >>>
+    @property
+    def framerate(self) -> numbers.Real:
+        """
+        ** Theoretical image frequency in the metadata. **
+        """
+        rel_index = [
+            i for i, s_ in enumerate(
+                s for s in self.node.out_streams if isinstance(s, _StreamVideoFFMPEG)
+            ) if s_ is self
+        ].pop()
+        return get_fps(self.node.filename, rel_index)
+
+    @property
+    def height(self) -> int:
+        return self.av_container.streams[self.index].height
+
+    @property
+    def key_times(self) -> np.ndarray[np.float32]:
+        """
+        ** Allows to read the file at the last moment. **
         """
         if self._key_times is None:
-            try:
-                self._key_times = np.fromiter(
-                    (
-                        frame_dates(frame)[0] for frame in _extract_key_frames(
-                            self.av_container.streams[self.index]
-                        )
-                    ),
-                    dtype=object,
-                )
-            except MissingInformation as err:
-                raise MissingInformation("the timestamp is not known for all keyframes") from err
+            self._key_times = np.fromiter(
+                (
+                    frame.time for frame in _extract_key_frames(
+                        self.av_container.streams[self.index]
+                    )
+                ),
+                dtype=np.float32,
+            )
             if len(self._key_times) == 0:
                 raise MissingStreamError(
                     f"can not decode any frames of {self.node.filename} stream {self.index}"
                 )
+            if np.any(np.isnan(self._key_times)):
+                raise MissingInformation("the timestamp is not known for all keyframes")
         return self._key_times
 
-    def get_current_range(self) -> tuple[fractions.Fraction, fractions.Fraction]:
+    @property
+    def nb_frames(self) -> int:
         """
-        ** Returns the time interval cover by the current frame. **
+        ** The exact number of frames present in this stream. **
         """
-        start_time = frame_dates(self.prec_frame)[0]
-        if (next_frame := self.next_frame) is None:
-            return start_time, start_time + 1/self.rate
-        return start_time, frame_dates(next_frame)[0]
+        rel_index = [
+            i for i, s_ in enumerate(
+                s for s in self.node.out_streams if isinstance(s, _StreamVideoFFMPEG)
+            ) if s_ is self
+        ].pop()
+        return get_nb_frames(self.node.filename, rel_index, accurate=True)
 
     @property
-    def height(self) -> int:
-        return self.av_container.streams[self.index].height
-
-    def seek(self, position: fractions.Fraction) -> None:
+    def time_base(self) -> fractions.Fraction:
         """
-        ** Moves into the file until reaching the frame at this position. **
-
-        If you are already well placed, this has no effect.
-        Allows backward even a little bit, but only jump forward if the jump is big enough.
-
-        Parameters
-        ----------
-        position : fraction.Fraction
-            The target position such as ``self.prec_frame.time <= position < self.next_frame.time``.
-            This position is expressed in seconds.
-
-        Raises
-        ------
-        OutOfTimeRange
-            If the required position is out of the definition range.
+        ** The unit of time (in fractional seconds) in which timestamps are expressed. **
 
         Examples
         --------
-        >>> from fractions import Fraction
         >>> from movia.core.io.read import ContainerInputFFMPEG
         >>> with ContainerInputFFMPEG("movia/examples/video.mp4") as container:
         ...     (stream,) = container.out_streams
-        ...     stream.seek(Fraction(15))
-        ...     stream.get_current_range()
-        ...     stream.seek(Fraction(5))
-        ...     stream.get_current_range()
+        ...     stream.time_base
         ...
-        (Fraction(15, 1), Fraction(376, 25))
-        (Fraction(5, 1), Fraction(126, 25))
+        Fraction(1, 12800)
         >>>
         """
-        assert isinstance(position, fractions.Fraction), position.__class__.__name__
-
-        # case need to seek
-        if position > self.get_current_range()[1] + 100/self.rate: # forward if jump more 100 frames
-            self._seek_forward(position) # very approximative
-        if position < self.get_current_range()[0]:
-            self._seek_backward(position) # guaranteed to be before
-
-        # fine adjustment
-        while self.get_current_range()[1] <= position:
-            self._prec_frame, self._next_frame = self._next_frame, None # hack for iter in stream
+        return self.av_container.streams[self.index].time_base
 
     @property
     def width(self) -> int:
         return self.av_container.streams[self.index].width
 
 
-def _convert_audio_samples(audio_samples: np.ndarray[numbers.Real]) -> torch.Tensor:
+def _born(refs, val):
+    """
+    ** Search the 2 values that encadre the number. **
+
+    The interval sought is the upper one.
+
+    Parameters
+    ----------
+    refs : np.ndarray
+        The list in ascending order of key values.
+    val : numbers.Real
+        The value to be placed among the other values.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from movia.core.io.read import _born
+    >>> _born(np.array([0, 2]), -1)
+    (None, 0)
+    >>> _born(np.array([0, 2]), 0)
+    (0, 2)
+    >>> _born(np.array([0, 2]), 1)
+    (0, 2)
+    >>> _born(np.array([0, 2]), 2)
+    (2, None)
+    >>> _born(np.array([0, 2]), 3)
+    (2, None)
+    >>> _born(np.array([0]), -1)
+    (None, 0)
+    >>> _born(np.array([0]), 0)
+    (0, None)
+    >>> _born(np.array([0]), 1)
+    (0, None)
+    >>>
+    """
+    if val < refs[0]:
+        return None, refs[0]
+    if val >= refs[-1]:
+        return refs[-1], None
+    ind_sup = np.argmin(refs <= val)
+    return refs[ind_sup-1], refs[ind_sup]
+
+
+def _clip_convert(audio_samples: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
     """
     ** Converts sound samples into float between -1 and 1. **
 
     Minimizes copying and reallocations.
-    The values are not clamped.
 
     Examples
     --------
     >>> import numpy as np
-    >>> from movia.core.io.read import _convert_audio_samples
-    >>> _convert_audio_samples(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float64))
-    tensor([-1.5000, -1.0000, -0.5000,  0.5000,  1.0000,  1.5000],
-           dtype=torch.float64)
-    >>> _convert_audio_samples(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float32))
-    tensor([-1.5000, -1.0000, -0.5000,  0.5000,  1.0000,  1.5000])
-    >>> _convert_audio_samples(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float16))
-    tensor([-1.5000, -1.0000, -0.5000,  0.5000,  1.0000,  1.5000],
-           dtype=torch.float16)
-    >>> _convert_audio_samples(
-    ...     np.array([-2147483648, -1073741824, 1073741824, 2147483647], dtype=np.int32)
-    ... )
-    tensor([-1.0000, -0.5000,  0.5000,  1.0000], dtype=torch.float64)
-    >>> _convert_audio_samples(np.array([-32768, -16384, 16384, 32767], dtype=np.int16))
-    tensor([-1.0000, -0.5000,  0.5000,  1.0000], dtype=torch.float64)
-    >>> _convert_audio_samples(np.array([0, 64, 192, 255], dtype=np.uint8))
-    tensor([-1.0000, -0.4980,  0.5059,  1.0000], dtype=torch.float64)
+    >>> from movia.core.io.read import _clip_convert
+    >>> _clip_convert(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float64))
+    array([-1. , -1. , -0.5,  0.5,  1. ,  1. ])
+    >>> _clip_convert(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float32))
+    array([-1. , -1. , -0.5,  0.5,  1. ,  1. ], dtype=float32)
+    >>> _clip_convert(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float16))
+    array([-1. , -1. , -0.5,  0.5,  1. ,  1. ], dtype=float16)
+    >>> _clip_convert(np.array([-2147483648, -1073741824, 1073741824, 2147483647], dtype=np.int32))
+    array([-1. , -0.5,  0.5,  1. ])
+    >>> _clip_convert(np.array([-32768, -16384, 16384, 32767], dtype=np.int16))
+    array([-1.        , -0.49999237,  0.50002289,  1.        ])
+    >>> _clip_convert(np.array([0, 64, 192, 255], dtype=np.uint8))
+    array([-1.        , -0.49803922,  0.50588235,  1.        ])
     >>>
     """
     assert isinstance(audio_samples, np.ndarray), audio_samples.__class__.__name__
-    audio_samples = torch.from_numpy(audio_samples)
-    if not audio_samples.dtype.is_floating_point:
-        iinfo = torch.iinfo(audio_samples.dtype)
-        audio_samples = audio_samples.to(dtype=torch.float64)
-        audio_samples -= .5*float(iinfo.min + iinfo.max)
-        audio_samples /= .5*float(iinfo.max - iinfo.min)
+    if issubclass(audio_samples.dtype.type, numbers.Integral):
+        iinfo = np.iinfo(audio_samples.dtype)
+        audio_samples = audio_samples.astype(np.float64)
+        audio_samples -= .5*np.float64(iinfo.min + iinfo.max)
+        audio_samples /= .5*np.float64(iinfo.max - iinfo.min)
+    else:
+        np.clip(audio_samples, -1, 1, out=audio_samples)
     return audio_samples
 
 
-def _extract_key_frames(av_stream: av.video.stream.VideoStream):
+def _extract_key_frames(av_stream):
     """
     ** Extract the list of key frames. **
 
     Examples
     --------
     >>> import av
     >>> from movia.core.io.read import _extract_key_frames
@@ -698,61 +803,37 @@
     av_stream.container.seek(0, backward=True, any_frame=False, stream=av_stream)
     av_stream.codec_context.skip_frame = "NONKEY"
     yield from av_stream.container.decode(av_stream)
     av_stream.container.seek(0, backward=True, any_frame=False, stream=av_stream)
     av_stream.codec_context.skip_frame = "DEFAULT"
 
 
-def frame_dates(frame: av.frame.Frame) -> tuple[fractions.Fraction, fractions.Fraction]:
+def _frame_dates(frame: av.frame.Frame) -> tuple[numbers.Real, numbers.Real]:
     """
     ** Returns the accurate time interval of the given frame. **
 
-    Parameters
-    ----------
-    frame : av.frame.Frame
-        The audio or video frame witch we extract the timing information.
-
-    Returns
-    -------
-    t_start : fractions.Fraction
-        The display time of the frame. for audio frame, it corressponds to
-        the time of the first sample.
-    t_end : fractions.Fraction or None
-        For audio frame only, the time to switch off the last sample.
-
     Examples
     --------
     >>> import av
-    >>> from movia.core.io.read import frame_dates
+    >>> from movia.core.io.read import _frame_dates
     >>> with av.open("movia/examples/video.mp4") as av_container:
-    ...     frame_dates(next(av_container.decode(av_container.streams.video[0])))
-    ...     frame_dates(next(av_container.decode(av_container.streams.video[0])))
+    ...     frame = next(av_container.decode(av_container.streams.video[0]))
+    ...     _frame_dates(frame)
     ...
-    (Fraction(0, 1), None)
-    (Fraction(1, 25), None)
+    (Fraction(0, 1), Fraction(0, 1))
     >>> with av.open("movia/examples/audio.ogg") as av_container:
-    ...     frame_dates(next(av_container.decode(av_container.streams.audio[0])))
-    ...     frame_dates(next(av_container.decode(av_container.streams.audio[0])))
+    ...     frame = next(av_container.decode(av_container.streams.audio[0]))
+    ...     _frame_dates(frame)
     ...
     (Fraction(0, 1), Fraction(4, 125))
-    (Fraction(4, 125), Fraction(8, 125))
     >>>
-
-    Notes
-    -----
-    For audio frame, include the duration of the last sample.
-    For video frame, the duration of the frame is unmknonw.
     """
     assert isinstance(frame, av.frame.Frame), frame.__class__.__name__
 
-    if (time_base := frame.time_base) is None:
-        start_time = fractions.Fraction(frame.time)
-    elif (pts := frame.pts) is not None:
-        start_time = pts * time_base
-    elif (dts := frame.dts) is not None:
-        start_time = dts * time_base
+    if (pts := frame.pts) is None or (time_base := frame.time_base) is None:
+        start_time = frame.time
     else:
-        raise MissingInformation(f"unable to catch the time of the frame {frame}")
+        start_time = pts * time_base
     if isinstance(frame, av.audio.frame.AudioFrame):
         stop_time = start_time + fractions.Fraction(frame.samples, frame.rate)
         return start_time, stop_time
-    return start_time, None
+    return start_time, start_time
```

### Comparing `movia-1.0.0b3/movia/gui/base.py` & `movia-1.0a1/movia/gui/base.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/gui/edition_tabs.py` & `movia-1.0a1/movia/gui/edition_tabs.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/gui/entry/base.py` & `movia-1.0a1/movia/gui/entry/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 """
 ** Defines the global style and behavior of the tabs of the entries table. **
 -----------------------------------------------------------------------------
 """
 
-import importlib
+import importlib.machinery
+import importlib.util
 import inspect
 import logging
 import re
 import typing
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 import numpy as np
@@ -65,17 +66,20 @@
         if len(self.selectedItems()) != 1:
             logging.error("can drag and drop only one item, not %d", len(self.selectedItems()))
             self.app.global_vars["drag_an_drop"] = None
             event.ignore()
             return
 
         classname, path = [i.data(3) for i in self.selectedItems()].pop()
-        mod = importlib.import_module(
-            ".".join(("movia" / path.relative_to(get_project_root()).with_suffix("")).parts)
+        mod_name = ".".join(("movia" / path.relative_to(get_project_root()).with_suffix("")).parts)
+        spec = importlib.util.spec_from_loader(
+            mod_name, importlib.machinery.SourceFileLoader(mod_name, str(path))
         )
+        mod = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(mod)
 
         generator_cls = dict(inspect.getmembers(mod))[classname]
         node_name, attrs = new_node(self.app.graph, generator_cls.default())
         self.app.global_vars["drag_an_drop"] = (node_name, attrs)
         event.accept()
 
     def refresh(self):
@@ -84,19 +88,19 @@
         """
         self.clear()
 
         # complete the elements
         elements = {}
         for filepath in (
             file for sub_dir in self.sub_dirs
-            for file in (get_project_root() / "core" / sub_dir).rglob("*.py")
+            for file in (get_project_root()/"core"/sub_dir).rglob("*.py")
         ):
-            mod = importlib.import_module(
-                ".".join(("movia" / filepath.relative_to(get_project_root()).with_suffix("")).parts)
-            )
+            spec = importlib.util.spec_from_file_location("foo", filepath)
+            mod = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(mod)
             for classname, node_cls in inspect.getmembers(mod):
                 if (
                     inspect.isclass(node_cls)
                     and issubclass(node_cls, Node)
                     and issubclass(node_cls, self.classnames)
                     and classname not in self.excluded_clsn
                 ):
```

### Comparing `movia-1.0.0b3/movia/gui/entry/generators.py` & `movia-1.0a1/movia/gui/entry/generators.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/gui/entry/project_files.py` & `movia-1.0a1/movia/gui/entry/project_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import inspect
 import logging
 import pathlib
 
 import numpy as np
 from PyQt6 import QtCore, QtGui, QtWidgets
 
-from movia.core.analysis.stream import get_streams_type
+from movia.core.analysis.streams import get_streams_type
 from movia.core.io.read import ContainerInputFFMPEG
 from movia.gui.entry.base import Entry
 
 
 
 class ProjectFiles(Entry):
     """
@@ -110,16 +110,12 @@
             img = np.zeros((128, 128, 3), dtype=np.uint8)
             icon = QtGui.QIcon(QtGui.QPixmap(QtGui.QImage(
                 img.data, img.shape[1], img.shape[0], 3*img.shape[1],
                 QtGui.QImage.Format.Format_BGR888
             )))
             item = QtWidgets.QListWidgetItem(icon, pathlib.Path(file).name, parent=self)
             item.setData(
-                3,
-                (
-                    ContainerInputFFMPEG.__name__,
-                    pathlib.Path(inspect.getsourcefile(ContainerInputFFMPEG)).resolve(),
-                ),
+                3, (ContainerInputFFMPEG.__name__, inspect.getsourcefile(ContainerInputFFMPEG))
             ) # 0 for text, 1 for icon, 2 for text, 3 is free!
             item.setData(4, file)
             self.addItem(item)
             self._item2index[item.text()] = index
```

### Comparing `movia-1.0.0b3/movia/gui/entry_tabs.py` & `movia-1.0a1/movia/gui/entry_tabs.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/gui/graph/edge_properties.py` & `movia-1.0a1/movia/gui/graph/edge_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import math
 
 from PyQt6 import QtCore, QtWidgets
 
 from movia.core.classes.stream_audio import StreamAudio
 from movia.core.classes.stream_video import StreamVideo
 from movia.gui.base import MoviaWidget
-from movia.gui.edit_node_state.main import EditNodeWindow
+from movia.gui.node_properties.node_properties import WindowNodeProperties
 
 
 
 class WindowEdgeProperties(MoviaWidget, QtWidgets.QDialog):
     """
     ** Show the edge properties. **
     """
@@ -124,9 +124,9 @@
 
         return ref_span
 
     def open_procreator(self):
         """
         ** Created and opens the property window for the parent node. **
         """
-        node_win = EditNodeWindow(self, self.edge_name[0])
+        node_win = WindowNodeProperties(self, self.edge_name[0])
         node_win.exec()
```

### Comparing `movia-1.0.0b3/movia/gui/graph/graph_editor.py` & `movia-1.0a1/movia/gui/graph/graph_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from movia.core.edit.operation.add import add_edge, add_node
 from movia.core.edit.operation.remove import remove_element
 from movia.gui.base import MoviaWidget
 from movia.gui.graph.edge_properties import WindowEdgeProperties
 from movia.gui.graph.layout import (compute_positions, clear_positions, create_and_init_agraph,
     draw, has_positions, same_structure)
-from movia.gui.edit_node_state.main import EditNodeWindow
+from movia.gui.node_properties.node_properties import WindowNodeProperties
 
 
 
 class GraphEditor(MoviaWidget, QtWidgets.QWidget):
     """
     ** Viewing and editing the assembly graph. **
     """
@@ -523,15 +523,15 @@
         """
         name, dist = self.select(event)
         if dist <= 20:
             old_state, self.state = self.state, "loading"
             if isinstance(name, tuple): # element is edge
                 graph_win = WindowEdgeProperties(self, name)
             else: # element is node
-                graph_win = EditNodeWindow(self, name)
+                graph_win = WindowNodeProperties(self, name)
             graph_win.exec()
             self.state = old_state
 
     @property
     def state(self) -> str:
         """
         ** Returns the graph viewer state. **
```

### Comparing `movia-1.0.0b3/movia/gui/graph/layout.py` & `movia-1.0a1/movia/gui/graph/layout.py`

 * *Files identical despite different names*

### Comparing `movia-1.0.0b3/movia/gui/menu.py` & `movia-1.0a1/movia/gui/menu.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 
 def fill_menu(menu, actions):
     """
     ** Adds fields to the empty menu. **
     """
 
     file_menu = menu.addMenu("File")
-    file_menu.addAction(actions["open"])
-    file_menu.addAction(actions["save"])
-    file_menu.addAction(actions["save_as"])
-    file_menu.addSeparator()
     file_menu.addAction(actions["import"])
     file_menu.addAction(actions["export"])
+    file_menu.addSeparator()
 
     edit_menu = menu.addMenu("Edit")
     edit_menu.addAction(actions["refresh"])
     edit_menu.addAction(actions["undo"])
     edit_menu.addAction(actions["redo"])
```

### Comparing `movia-1.0.0b3/movia/gui/toolbar.py` & `movia-1.0a1/movia/gui/toolbar.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,15 @@
     ** Main window menu bar. **
     """
 
     def __init__(self, parent, actions):
         super().__init__(parent)
         self._parent = parent
 
-        self.addAction(actions["import"])
-        self.addAction(actions["open"])
-        self.addAction(actions["save"])
-
-        self.addSeparator()
-
+        # location
         self.addAction(actions["refresh"])
         self.addAction(actions["undo"])
         self.addAction(actions["redo"])
 
         self.addSeparator()
 
         self.addAction(actions["export"])
```

### Comparing `movia-1.0.0b3/movia/gui/video_viewer.py` & `movia-1.0a1/movia/gui/video_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 #!/usr/bin/env python3
 
 """
 ** Definition of the toolbar. **
 --------------------------------
 """
 
-import fractions
 import numbers
 import queue
 import subprocess
 import sys
 import time
 
+import av
 import numpy as np
 from PyQt6 import QtCore, QtGui, QtWidgets
 
-from movia.core.classes.frame_audio import FrameAudio
-from movia.core.classes.frame_video import FrameVideo
 from movia.core.classes.stream_audio import StreamAudio
 from movia.core.classes.stream_video import StreamVideo
 from movia.core.compilation.export.rate_audio import find_optimal_audio_rate
 from movia.core.compilation.export.rate_video import find_optimal_video_rate
 from movia.core.exceptions import OutOfTimeRange
-from movia.core.io.write import frame_audio_to_av, scheduler
+from movia.core.io.write import global_scheduler
 from movia.gui.base import MoviaWidget
 
 
 
 class AudioPlayer(QtCore.QThread):
     """
     ** Allows to play sound buffers in the background, without blocking. **
@@ -193,16 +191,16 @@
             signature = hash((tuple(id(s) for s in streams), tuple(rates), position))
             if signature != self._frame_iter_signature:
                 self._frame_iter_signature = signature
                 recreate = True
 
         # creation of the new iterator
         if recreate:
-            self._frame_iter = iter(scheduler(
-                streams, rates, start_time=fractions.Fraction(position), samples=8192
+            self._frame_iter = iter(global_scheduler(
+                streams, rates, start_time=position, duration=0.2
             ))
 
     def get_index_audio(self):
         """
         ** Retrive the index of the audio stream. **
         """
         if any(isinstance(s, StreamAudio) for s in self.app.tree().in_streams):
@@ -248,16 +246,17 @@
             cv_img = np.array([[[]]], dtype=np.uint8)
             if (index := self.get_index_video()) != -1:
                 container_out = self.app.tree()
                 stream = [s for s in container_out.in_streams if isinstance(s, StreamVideo)][index]
                 try:
                     frame = stream.snapshot(self.get_position())
                 except OutOfTimeRange:
-                    frame = stream.snapshot(np.nan) # default frame
-                cv_img = frame.to_numpy_bgr(contiguous=True)
+                    pass
+                else:
+                    cv_img = frame.to_ndarray(format="bgr24")
             self.change_video_frame.emit(cv_img)
 
     def run(self):
         """
         ** Sends the frames of the video at the right time. **
         """
         while self._is_alive:
@@ -272,24 +271,23 @@
                 self.get_frame_iter() # relatively slow function
             try:
                 _, frame = next(self._frame_iter)
             except StopIteration:
                 self.set_pause()
                 self.set_position(0)
                 continue
-            if isinstance(frame, FrameVideo):
+            if isinstance(frame, av.video.frame.VideoFrame):
                 emit_func = self.change_video_frame.emit
-                data = (frame.to_numpy_bgr(contiguous=True),)
-            elif isinstance(frame, FrameAudio):
+                data = (frame.to_ndarray(format="bgr24"),)
+            elif isinstance(frame, av.audio.frame.AudioFrame):
                 emit_func = self.change_audio_frame.emit
                 data = (
-                    frame.channels,
+                    len(frame.layout.channels),
                     frame.rate,
-                    b"".join(bytes(p) for p in frame_audio_to_av(frame).planes),
-                    # bytes(frame.numpy(force=True).astype(np.float32).ravel(order="F"))
+                    b"".join(bytes(p) for p in frame.planes),
                 )
             else:
                 raise NotImplementedError(f"{frame.__class__.__name__} is not yet supported")
 
             # real time delivery
             timestamp = self.get_position() + (time.time() - self._start_date) # real time position
             wait = frame.time - timestamp
```

### Comparing `movia-1.0.0b3/movia/utils.py` & `movia-1.0a1/movia/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,11 +18,11 @@
     >>> from movia.utils import get_project_root
     >>> root = get_project_root()
     >>> root.is_dir()
     True
     >>> root.name
     'movia'
     >>> sorted(p.name for p in root.iterdir())
-    ['__init__.py', '__main__.py', '__pycache__', 'core', 'examples', 'gui', 'testing', 'utils.py']
+    ['__init__.py', '__main__.py', '__pycache__', 'core', 'examples', 'gui', 'tests', 'utils.py']
     >>>
     """
     return pathlib.Path(__file__).parent
```

### Comparing `movia-1.0.0b3/setup.py` & `movia-1.0a1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,98 +1,72 @@
 #!/usr/bin/env python3
 
 """
 ** Configuration file for pip. **
 ---------------------------------
 """
 
-import sys
-
-from setuptools import find_packages, setup
+import setuptools
 
 import movia
 
 
-if sys.version_info < (3, 9):
-    print(
-        "Movia requires Python 3.9 or newer. "
-        f"Python {sys.version_info[0]}.{sys.version_info[1]} detected"
-    )
-    sys.exit(-1)
-
-
 with open("README.rst", "r", encoding="utf-8") as file:
     long_description = file.read()
 
-setup(
+setuptools.setup(
     name="movia",
     version=movia.__version__,
     author="Robin RICHARD (robinechuca)",
     author_email="serveurpython.oz@gmail.com",
     description="video editing softwear",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://framagit.org/robinechuca/movia/-/blob/main/README.md",
-    data_files=[
-        ("movia/", ["README.rst", ".pylintrc"]),
-    ],
-    packages=find_packages(),
-    install_requires=[ # dependences: apt install graphviz-dev ffmpeg
+    packages=setuptools.find_packages(),
+    install_requires=[
         "av", # apt install ffmpeg python3-av
+        "black",
         "click", # apt install python3-click
         "networkx", # apt install python3-networkx
         "numpy >= 1.22", # apt install python3-numpy
         "opencv-contrib-python-headless", # apt install python3-opencv
+        "pdoc3",
+        "pygraphviz", # apt install graphviz graphviz-dev pygraphviz https://pygraphviz.github.io/documentation/stable/install.html
+        "pyqt6", # apt install python3-pyqt6[.sip]
         "sympy", # apt install python3-sympy
-        "torch >= 1.8",
-        "tqdm", # apt install python3-tqdm
         "unidecode", # apt install python3-unidecode
     ],
     extras_require={
-        "gui": [
-            "black", # apt install black python3-pyls-black
-            "pdoc3",
-            "pygraphviz", # https://pygraphviz.github.io/documentation/stable/install.html
-            "pyqt6", # apt install python3-pyqt6[.sip]
-        ], # apt install pylint, python3-pylint-common, python3-pytest
-        "optional": [
-            "black",
-            "pdoc3",
-            "pygraphviz",
-            "pylint",
-            "pyqt6",
-            "pytest",
-        ],
+        "dev": ["pylint", "pytest"] # apt install pylint, python3-pylint-common, python3-pytest
     },
     entry_points={
         "console_scripts": [
             "movia=movia.__main__:main",
-            "movia-test=movia.testing.runtests:test",
-        ],
-        "gui_scripts": [
-            "movia-qt=movia.gui.__main__:main",
         ]
     },
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Environment :: X11 Applications :: Qt",
         "Intended Audience :: Customer Service",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
         "Topic :: Multimedia",
+        "Topic :: Multimedia :: Graphics :: Capture",
         "Topic :: Multimedia :: Graphics :: Editors",
         "Topic :: Multimedia :: Graphics :: Graphics Conversion",
         "Topic :: Multimedia :: Sound/Audio",
         "Topic :: Multimedia :: Sound/Audio :: Analysis",
         "Topic :: Multimedia :: Sound/Audio :: Conversion",
         "Topic :: Multimedia :: Sound/Audio :: Mixers",
         "Topic :: Multimedia :: Sound/Audio :: Players",
         "Topic :: Multimedia :: Video",
+        "Topic :: Multimedia :: Video :: Capture",
         "Topic :: Multimedia :: Video :: Conversion",
         "Topic :: Multimedia :: Video :: Display",
         "Topic :: Multimedia :: Video :: Non-Linear Editor",
         "Topic :: Scientific/Engineering :: Image Processing",
     ],
     keywords=[
         "video",
```

