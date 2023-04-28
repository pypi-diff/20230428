# Comparing `tmp/resotolib-3.4.0.tar.gz` & `tmp/resotolib-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.4.0.tar", last modified: Thu Apr 27 11:25:11 2023, max compression
+gzip compressed data, was "resotolib-3.4.1.tar", last modified: Fri Apr 28 15:13:59 2023, max compression
```

## Comparing `resotolib-3.4.0.tar` & `resotolib-3.4.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 11:22:59.000000 resotolib-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-27 11:25:11.410409 resotolib-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-27 11:22:59.000000 resotolib-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-27 11:22:59.000000 resotolib-3.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 11:22:59.000000 resotolib-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.370408 resotolib-3.4.0/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.374408 resotolib-3.4.0/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.378408 resotolib-3.4.0/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.382408 resotolib-3.4.0/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.386408 resotolib-3.4.0/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    25794 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.386408 resotolib-3.4.0/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/log/logstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.390408 resotolib-3.4.0/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.394408 resotolib-3.4.0/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.370408 resotolib-3.4.0/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:25:11.410409 resotolib-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-27 11:22:59.000000 resotolib-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/test/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/asynchronous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/test/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/asynchronous/web/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/test/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/custom_command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/model_check_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/model_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/progress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/tasks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/durations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/json_bender_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/parse_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 15:10:57.000000 resotolib-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-28 15:13:59.747479 resotolib-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-28 15:10:57.000000 resotolib-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-28 15:10:57.000000 resotolib-3.4.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 15:10:57.000000 resotolib-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.739479 resotolib-3.4.1/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.739479 resotolib-3.4.1/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.739479 resotolib-3.4.1/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40989 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/log/logstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22777 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.739479 resotolib-3.4.1/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 15:13:59.747479 resotolib-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-28 15:10:57.000000 resotolib-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/test/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/asynchronous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/test/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/asynchronous/web/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/custom_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/model_check_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/model_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/progress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/tasks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/durations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/json_bender_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/parse_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_x509.py
```

### Comparing `resotolib-3.4.0/PKG-INFO` & `resotolib-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -34,15 +34,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotolib-3.4.0/README.md` & `resotolib-3.4.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotolib-3.4.0/resotolib/args.py` & `resotolib-3.4.1/resotolib/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,90 @@
 import argparse
 import os
 import shutil
 import subprocess
-import sys
 from collections import defaultdict
-from typing import List, Dict, Any, Union, Callable
+from typing import List, Dict, Any, Union, Callable, Optional, Sequence, Tuple
 
 DEFAULT_ENV_ARGS_PREFIX = "RESOTO_"
 
 
 class Namespace(argparse.Namespace):
-    def __getattr__(self, item):
+    def __getattr__(self, item: str) -> Any:
         return None
 
 
 class _MachineHelpAction(argparse.Action):
     def __init__(
         self,
-        option_strings,
-        dest=argparse.SUPPRESS,
-        default=argparse.SUPPRESS,
-        help=None,
-    ):
+        option_strings: Sequence[str],
+        dest: str = argparse.SUPPRESS,
+        default: str = argparse.SUPPRESS,
+        help: Optional[str] = None,
+    ) -> None:
         super(_MachineHelpAction, self).__init__(
             option_strings=option_strings,
             dest=dest,
             default=default,
             nargs=0,
             help=help,
         )
 
-    def __call__(self, parser, namespace, values, option_string=None):
-        parser.print_machine_help()
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,
+        values: Union[str, Sequence[Any], None],
+        option_string: Optional[str] = None,
+    ) -> None:
+        parser.print_machine_help()  # type: ignore
         parser.exit()
 
 
 class ArgumentParser(argparse.ArgumentParser):
     # Class variable containing the last return value of parse_args()
     # If parse_args() hasn't been called yet will return None for any
     # attribute.
     args = Namespace()
 
     def __init__(
         self,
-        *args,
+        *args: Any,
         env_args_prefix: str = DEFAULT_ENV_ARGS_PREFIX,
         add_machine_help: bool = True,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.env_args_prefix = env_args_prefix
         self.add_machine_help = add_machine_help
         self.register("action", "machine_help", _MachineHelpAction)
 
         if self.add_machine_help:
             self.add_argument(
                 "--machine-help",
                 action="machine_help",
                 help="print machine readable help",
             )
 
-    def print_machine_help(self):
+    def print_machine_help(self) -> None:
         for action in self._actions:
             if action.default == argparse.SUPPRESS:
                 continue
             for option_string in action.option_strings:
                 print(option_string)
 
-    def parse_known_args(self, args=None, namespace=None):
+    def parse_known_args(self, args: Any = None, namespace: Any = None) -> Tuple[Namespace, List[str]]:
         for action in self._actions:
             env_name = None
             for option_string in action.option_strings:
                 if option_string.startswith("--"):
                     env_name = self.env_args_prefix + option_string[2:].replace("-", "_").upper()
                     break
             if env_name is not None and action.default != argparse.SUPPRESS:
-                new_default = None
+                new_default: Any = None
                 if action.nargs not in (0, None):
                     new_default = os.environ.get(env_name)
                     if new_default is not None:
                         new_default = new_default.split(" ")
                     else:
                         new_default = []
                         for i in range(255):
@@ -102,16 +107,16 @@
                     if isinstance(new_default, list):
                         new_default = [convert(n, type_goal) for n in new_default]
                     else:
                         new_default = convert(new_default, type_goal)
 
                     action.default = new_default
         ret_args, ret_argv = super().parse_known_args(args=args, namespace=namespace)
-        ArgumentParser.args = ret_args
-        return ret_args, ret_argv
+        ArgumentParser.args = ret_args  # type: ignore
+        return ret_args, ret_argv  # type: ignore
 
 
 def get_arg_parser(
     add_help: bool = True,
     description: str = "resoto",
     env_args_prefix: str = DEFAULT_ENV_ARGS_PREFIX,
 ) -> ArgumentParser:
@@ -119,16 +124,16 @@
     return arg_parser
 
 
 # removed from types in 3.0-3.9: introduced again in 3.10
 NoneType = type(None)
 
 
-def convert(value: Any, type_goal: Union[type, Callable]) -> Any:
-    if type_goal is NoneType:
+def convert(value: Any, type_goal: Union[type, Callable[[Any], Any]]) -> Any:
+    if type_goal is NoneType:  # type: ignore
         return value
     elif isinstance(type_goal, type):
         try:
             if type_goal in (str, int, float, complex):
                 return type_goal(value)
             elif type_goal is bool:
                 return value.lower() in ("true", "1", "yes")
@@ -138,22 +143,22 @@
         except Exception:
             # can not convert value
             return value
     elif callable(type_goal):
         return type_goal(value)
 
 
-def args_dispatcher(dispatch_to: List, use_which: bool = False, argv: List = sys.argv[1:]) -> Dict[str, List[str]]:
+def args_dispatcher(dispatch_to: List[str], use_which: bool, argv: List[str]) -> Dict[str, List[str]]:
     dispatch_args = defaultdict(list)
     prog_args = defaultdict(list)
 
     for prog in dispatch_to:
         cmd = prog
         if use_which:
-            cmd = shutil.which(prog)
+            cmd = shutil.which(prog)  # type: ignore
         result = subprocess.run([cmd, "--machine-help"], capture_output=True)
         if result.returncode != 0:
             continue
         for arg in result.stdout.decode("utf8").splitlines():
             prog_args[arg].append(prog)
 
     args = defaultdict(list)
```

### Comparing `resotolib-3.4.0/resotolib/asynchronous/periodic.py` & `resotolib-3.4.1/resotolib/asynchronous/periodic.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/asynchronous/web/auth.py` & `resotolib-3.4.1/resotolib/asynchronous/web/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     Expected message: json object with type kind="authorization" and a jwt field
     { "kind": "authorization", "jwt": "Bearer <jwt>" }
     """
     try:
         js = json.loads(msg)
         assert js.get("kind") == "authorization"
-        return js.get("jwt")
+        return js.get("jwt")  # type: ignore
     except Exception:
         return None
 
 
 @middleware
 async def no_check(request: Request, handler: RequestHandler) -> StreamResponse:
     # all requests are authorized automatically
@@ -68,15 +68,15 @@
 
     @middleware
     async def valid_jwt_handler(request: Request, handler: RequestHandler) -> StreamResponse:
         auth_header = request.headers.get("Authorization") or request.cookies.get("resoto_authorization")
         authorized = False
         if auth_header:
             # make sure origin and host match, so the request is valid
-            origin: Optional[str] = urlparse(request.headers.get("Origin")).hostname
+            origin: Optional[str] = urlparse(request.headers.get("Origin")).hostname  # type: ignore
             host: Optional[str] = request.headers.get("Host")
             if host is not None and origin is not None:
                 if ":" in host:
                     host = host.split(":")[0]
                 if origin.lower() != host.lower():
                     log.warning(f"Origin {origin} is not allowed in request from {request.remote} to {request.path}")
                     raise web.HTTPForbidden()
```

### Comparing `resotolib-3.4.0/resotolib/asynchronous/web/runner.py` & `resotolib-3.4.1/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.4.1/resotolib/asynchronous/web/ws_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             future.cancel()
             log.info(f"Cleanup ws handler: {ws_id} ({len(websocket_handler)} active)")
             if not ws.closed:
                 await ws.close()
 
 
 def js_str(a: Any) -> str:
-    return jsons.dumps(a, strip_privates=True)
+    return jsons.dumps(a, strip_privates=True)  # type: ignore
 
 
 async def accept_websocket(
     request: Request,
     *,
     handle_incoming: Callable[[str], Awaitable[None]],
     websocket_handler: WSHandler,
```

### Comparing `resotolib-3.4.0/resotolib/baseplugin.py` & `resotolib-3.4.1/resotolib/baseplugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 from abc import ABC, abstractmethod
 from enum import Enum, auto
 from threading import Thread, current_thread
-from typing import Dict, Optional, Set
+from typing import Dict, Optional, Set, Any
 
 from prometheus_client import Counter
 
 import resotolib.config
 import resotolib.proc
 from resotolib.args import ArgumentParser
 from resotolib.baseresources import BaseResource, Cloud
@@ -97,26 +97,26 @@
         self.name = self.__class__.__name__
         self.finished = False
         self.timeout = Config.resotoworker.timeout
         self.wait_for_completion = True
         self.tls_data = tls_data
 
     @abstractmethod
-    def do_action(self, data: Dict):
+    def do_action(self, data: Dict[str, Any]) -> None:
         """Perform an action"""
         pass
 
-    def action_processor(self, message: Dict) -> Optional[Json]:
+    def action_processor(self, message: Json) -> Optional[Json]:
         """Process incoming action messages"""
         if not isinstance(message, dict):
             log.error(f"Invalid message: {message}")
             return None
         kind = message.get("kind")
         message_type = message.get("message_type")
-        data = message.get("data")
+        data: Json = message.get("data", {})
         log.debug(f"Received message of kind {kind}, type {message_type}, data: {data}")
         if kind == "action":
             try:
                 if message_type == self.action:
                     start_time = time.time()
                     self.do_action(data)
                     run_time = int(time.time() - start_time)
@@ -125,20 +125,21 @@
                     raise ValueError(f"Unknown message type {message_type}")
             except Exception as e:
                 log.exception(f"Failed to {message_type}: {e}")
                 reply_kind = "action_error"
             else:
                 reply_kind = "action_done"
 
-            reply_message = {
+            return {
                 "kind": reply_kind,
                 "message_type": message_type,
                 "data": data,
             }
-            return reply_message
+        else:
+            return None
 
     def run(self) -> None:
         try:
             # ArgumentParser.args = self._args
             # resotolib.config._config = self._config
             # setup_logger("resotoworker")
             # resotolib.proc.initializer()
@@ -231,15 +232,15 @@
 
     @staticmethod
     def pre_cleanup(config: Config, resource: BaseResource, graph: Graph) -> bool:
         return resource.pre_cleanup(graph)
 
     @staticmethod
     def cleanup(config: Config, resource: BaseResource, graph: Graph) -> bool:
-        return resource.cleanup(graph)
+        return resource.cleanup(graph)  # type: ignore
 
     def go(self) -> None:
         self.collect()
 
 
 class BasePostCollectPlugin(ABC):
     """A resoto Post Collect plugin is a thread that runs after collection is done.
```

### Comparing `resotolib-3.4.0/resotolib/baseresources.py` & `resotolib-3.4.1/resotolib/baseresources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from functools import wraps, cached_property
-from datetime import datetime, timezone, timedelta
-from copy import deepcopy
 import base64
 import hashlib
 import weakref
-from resotolib.logger import log
+from abc import ABC, abstractmethod
+from copy import deepcopy
+from datetime import datetime, timezone, timedelta
 from enum import Enum
-from typing import Dict, Iterator, List, ClassVar, Optional, TypedDict, Any, TypeVar, Type
-from resotolib.utils import make_valid_timestamp, utc_str
+from functools import wraps, cached_property
+from typing import Dict, Iterator, List, ClassVar, Optional, TypedDict, Any, TypeVar, Type, Callable, Set, Tuple
+
+import jsons
+from attrs import define, field, resolve_types, Factory
+from prometheus_client import Counter, Summary
+
 from resotolib.json import from_json as _from_json, to_json as _to_json
+from resotolib.logger import log
 from resotolib.types import Json
-from prometheus_client import Counter, Summary
-from attrs import define, field, resolve_types, Factory
-import jsons
+from resotolib.utils import make_valid_timestamp, utc_str
 
 metrics_resource_pre_cleanup_exceptions = Counter(
     "resource_pre_cleanup_exceptions_total",
     "Number of resource pre_cleanup() exceptions",
     ["cloud", "account", "region", "kind"],
 )
 metrics_resource_cleanup_exceptions = Counter(
     "resource_cleanup_exceptions_total",
     "Number of resource cleanup() exceptions",
     ["cloud", "account", "region", "kind"],
 )
 metrics_resource_cleanup = Summary("resoto_resource_cleanup_seconds", "Time it took the resource cleanup() method")
 
 
-def unless_protected(f):
+def unless_protected(f: Callable[..., bool]) -> Callable[..., bool]:
     @wraps(f)
-    def wrapper(self, *args, **kwargs):
+    def wrapper(self: Any, *args: Any, **kwargs: Any) -> bool:
         if not isinstance(self, BaseResource):
             raise ValueError("unless_protected() only supports BaseResource type objects")
         if self.protected:
             log.error(f"Resource {self.rtdname} is protected - refusing modification")
             self.log(("Modification was requested even though resource is protected" " - refusing"))
             return False
         return f(self, *args, **kwargs)
@@ -61,45 +63,45 @@
 
 
 class EdgeType(Enum):
     default = "default"
     delete = "delete"
 
     @staticmethod
-    def from_value(value: Optional[str] = None) -> Enum:
+    def from_value(value: Optional[str] = None) -> EdgeType:
         try:
             return EdgeType(value)
         except ValueError:
             pass
         return EdgeType.default
 
 
 class ResourceChanges:
-    def __init__(self, node) -> None:
+    def __init__(self, node: BaseResource) -> None:
         self.node = node
-        self.reported = set()
-        self.desired = set()
-        self.metadata = set()
+        self.reported: Set[str] = set()
+        self.desired: Set[str] = set()
+        self.metadata: Set[str] = set()
         self.changed = False
 
     def add(self, property: str) -> None:
-        if property in ("tags"):
+        if property == "tags":
             self.reported.add(property)
-        elif property in ("clean"):
+        elif property == "clean":
             self.desired.add(property)
         elif property in ("cleaned", "protected"):
             self.metadata.add(property)
         elif property == "log":
             pass
         else:
             raise ValueError(f"Unknown property {property}")
         self.changed = True
 
-    def get(self) -> Dict:
-        changes = {}
+    def get(self) -> Dict[str, Any]:
+        changes: Dict[str, Any] = {}
         for section in ("reported", "desired", "metadata"):
             for attribute in getattr(self, section, []):
                 if section not in changes:
                     changes[section] = {}
                 try:
                     changes[section][attribute] = getattr(self.node, attribute)
                 except AttributeError:
@@ -144,15 +146,15 @@
     _zone: "Optional[BaseZone]" = field(default=None, repr=False)
     _resotocore_id: Optional[str] = field(default=None, repr=False)
     _resotocore_revision: Optional[str] = field(default=None, repr=False)
     _resotocore_query_tag: Optional[str] = field(default=None, repr=False)
     _clean: bool = False
     _cleaned: bool = False
     _protected: bool = False
-    _deferred_connections: List = field(factory=list)
+    _deferred_connections: List[Dict[str, Any]] = field(factory=list)
 
     ctime: Optional[datetime] = field(
         default=None,
         metadata={"synthetic": {"age": "trafo.duration_to_datetime"}},
     )
     mtime: Optional[datetime] = field(
         default=None,
@@ -164,24 +166,24 @@
     )
 
     def __attrs_post_init__(self) -> None:
         if self.name is None:
             self.name = self.id
         self._changes: ResourceChanges = ResourceChanges(self)
         self.__graph = None
-        self.__log: List = []
+        self.__log: List[Json] = []
         self._raise_tags_exceptions: bool = False
         if not hasattr(self, "_ctime"):
             self._ctime = None
         if not hasattr(self, "_atime"):
             self._atime = None
         if not hasattr(self, "_mtime"):
             self._mtime = None
 
-    def _keys(self) -> tuple:
+    def _keys(self) -> Tuple[Any, ...]:
         """Return a tuple of all keys that make this resource unique
 
         Must not be called before the resource is connected to the graph
         as the relative location within the graph is used to determine the
         tuple of unique keys.
 
         E.g. instance -> aws -> 123457 -> us-east-1 -> us-east-1b -> i-987654 -> myServer
@@ -246,15 +248,15 @@
                 "rtdname",
                 "str_event_log",
                 "usage_percentage",
                 "uuid",
             ),
         )
 
-    def log(self, msg: str, data=None, exception=None) -> None:
+    def log(self, msg: str, data: Optional[Any] = None, exception: Optional[Exception] = None) -> None:
         now = datetime.utcnow().replace(tzinfo=timezone.utc)
         log_entry = {
             "timestamp": now,
             "msg": str(msg),
             "exception": repr(exception) if exception else None,
             "data": deepcopy(data),
         }
@@ -265,19 +267,19 @@
         self._changes.add(change)
 
     @property
     def changes(self) -> ResourceChanges:
         return self._changes
 
     @property
-    def event_log(self) -> List:
+    def event_log(self) -> List[Json]:
         return self.__log
 
     @property
-    def str_event_log(self) -> List:
+    def str_event_log(self) -> List[Json]:
         return [
             {
                 "timestamp": utc_str(le["timestamp"]),
                 "msg": le["msg"],
                 "exception": le["exception"],
             }
             for le in self.__log
@@ -299,52 +301,55 @@
         )
 
     @property
     def age(self) -> Optional[timedelta]:
         now = datetime.utcnow().replace(tzinfo=timezone.utc)
         if self.ctime is not None:
             return now - self.ctime
+        else:
+            return None
 
     @property
     def last_access(self) -> Optional[timedelta]:
         now = datetime.utcnow().replace(tzinfo=timezone.utc)
         if self.atime is not None:
             return now - self.atime
+        else:
+            return None
 
     @property
     def last_update(self) -> Optional[timedelta]:
         now = datetime.utcnow().replace(tzinfo=timezone.utc)
         if self.mtime is not None:
             return now - self.mtime
+        else:
+            return None
 
     def _ctime_getter(self) -> Optional[datetime]:
-        if "resoto:ctime" in self.tags:
-            ctime = self.tags["resoto:ctime"]
+        if ctime_string := self.tags.get("resoto:ctime"):
             try:
-                ctime = make_valid_timestamp(datetime.fromisoformat(ctime))
+                return make_valid_timestamp(datetime.fromisoformat(ctime_string))
             except ValueError:
                 pass
-            else:
-                return ctime
         return self._ctime
 
     def _ctime_setter(self, value: Optional[datetime]) -> None:
-        self._ctime = make_valid_timestamp(value)
+        self._ctime = make_valid_timestamp(value) if value else None  # type: ignore
 
     def _atime_getter(self) -> Optional[datetime]:
         return self._atime
 
     def _atime_setter(self, value: Optional[datetime]) -> None:
-        self._atime = make_valid_timestamp(value)
+        self._atime = make_valid_timestamp(value) if value else None  # type: ignore
 
     def _mtime_getter(self) -> Optional[datetime]:
         return self._mtime
 
     def _mtime_setter(self, value: Optional[datetime]) -> None:
-        self._mtime = make_valid_timestamp(value)
+        self._mtime = make_valid_timestamp(value) if value else None  # type: ignore
 
     @property
     def clean(self) -> bool:
         return self._clean
 
     @clean.setter
     @unless_protected
@@ -378,17 +383,17 @@
             log.debug(f"Protecting resource {self.rtdname}")
             self.log("Protecting resource")
             self._changes.add("protected")
             self._protected = value
 
     # deprecated. future collectors plugins should be responsible for running pre_cleanup
     # and calling delete_resource on resources
-    @metrics_resource_cleanup.time()
+    @metrics_resource_cleanup.time()  # type: ignore
     @unless_protected
-    def cleanup(self, graph=None) -> bool:
+    def cleanup(self, graph: Optional[Any] = None) -> bool:
         if self.phantom:
             raise RuntimeError(f"Can't cleanup phantom resource {self.rtdname}")
 
         if self.cleaned:
             log.debug(f"Resource {self.rtdname} has already been cleaned up")
             return True
 
@@ -423,15 +428,15 @@
         if not deleted:
             raise RuntimeError(f"Failed to clean up {self.rtdname}{log_suffix}")
         return True
 
     # deprecated. future collectors plugins should be responsible for running pre_cleanup
     # and calling pre_delete_resource on resources
     @unless_protected
-    def pre_cleanup(self, graph=None) -> bool:
+    def pre_cleanup(self, graph: Optional[Any] = None) -> bool:
         if not hasattr(self, "pre_delete"):
             return True
 
         if graph is None:
             graph = self._graph
 
         if self.phantom:
@@ -468,66 +473,66 @@
                 kind=self.kind,
             ).inc()
             raise
         return True
 
     @unless_protected
     @abstractmethod
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         raise NotImplementedError
 
-    def account(self, graph=None) -> "BaseAccount":
-        account = None
+    def account(self, graph: Optional[Any] = None) -> "BaseAccount":
+        account: Optional[BaseAccount] = None
         if graph is None:
             graph = self._graph
         if self._account:
             account = self._account
         elif graph:
             account = graph.search_first_parent_class(self, BaseAccount)
         if account is None:
             account = UnknownAccount(id="undefined", tags={})
         return account
 
-    def cloud(self, graph=None) -> "BaseCloud":
-        cloud = None
+    def cloud(self, graph: Optional[Any] = None) -> "BaseCloud":
+        cloud: Optional[BaseCloud] = None
         if graph is None:
             graph = self._graph
         if self._cloud:
             cloud = self._cloud
         elif graph:
             cloud = graph.search_first_parent_class(self, BaseCloud)
         if cloud is None:
             cloud = UnknownCloud(id="undefined", tags={})
         return cloud
 
-    def region(self, graph=None) -> "BaseRegion":
-        region = None
+    def region(self, graph: Optional[Any] = None) -> "BaseRegion":
+        region: Optional[BaseRegion] = None
         if graph is None:
             graph = self._graph
         if self._region:
             region = self._region
         elif graph:
             region = graph.search_first_parent_class(self, BaseRegion)
         if region is None:
             region = UnknownRegion(id="undefined", tags={})
         return region
 
-    def zone(self, graph=None) -> "BaseZone":
-        zone = None
+    def zone(self, graph: Optional[Any] = None) -> "BaseZone":
+        zone: Optional[BaseZone] = None
         if graph is None:
             graph = self._graph
         if self._zone:
             zone = self._zone
         elif graph:
             zone = graph.search_first_parent_class(self, BaseZone)
         if zone is None:
             zone = UnknownZone(id="undefined", tags={})
         return zone
 
-    def location(self, graph=None):
+    def resource_location(self, graph: Optional[Any] = None) -> "BaseResource":
         if graph is None:
             graph = self._graph
         zone = self.zone(graph)
         if zone.name != "undefined":
             return zone
         region = self.region(graph)
         if region.name != "undefined":
@@ -537,19 +542,19 @@
             return account
         cloud = self.cloud(graph)
         if cloud.name != "undefined":
             return cloud
         return UnknownLocation(id="undefined", tags={})
 
     def add_deferred_connection(
-        self, search: Dict, parent: bool = True, edge_type: EdgeType = EdgeType.default
+        self, search: Dict[str, Any], parent: bool = True, edge_type: EdgeType = EdgeType.default
     ) -> None:
         self._deferred_connections.append({"search": search, "parent": parent, "edge_type": edge_type})
 
-    def resolve_deferred_connections(self, graph) -> None:
+    def resolve_deferred_connections(self, graph: Any) -> None:
         if graph is None:
             graph = self._graph
         while self._deferred_connections:
             dc = self._deferred_connections.pop(0)
             node = graph.search_first_all(dc["search"])
             edge_type = dc["edge_type"]
             if node:
@@ -557,98 +562,100 @@
                     src = node
                     dst = self
                 else:
                     src = self
                     dst = node
                 graph.add_edge(src, dst, edge_type=edge_type)
 
-    def predecessors(self, graph=None, edge_type=None) -> Iterator:
+    def predecessors(self, graph: Optional[Any] = None, edge_type: Optional[EdgeType] = None) -> Iterator[BaseResource]:
         """Returns an iterator of the node's parent nodes"""
         if graph is None:
             graph = self._graph
         if graph is None:
-            return ()
-        return graph.predecessors(self, edge_type=edge_type)
+            return iter(())
+        return graph.predecessors(self, edge_type=edge_type)  # type: ignore
 
-    def successors(self, graph=None, edge_type=None) -> Iterator:
+    def successors(self, graph: Optional[Any] = None, edge_type: Optional[EdgeType] = None) -> Iterator[BaseResource]:
         """Returns an iterator of the node's child nodes"""
         if graph is None:
             graph = self._graph
         if graph is None:
-            return ()
-        return graph.successors(self, edge_type=edge_type)
+            return iter(())
+        return graph.successors(self, edge_type=edge_type)  # type: ignore
 
-    def predecessor_added(self, resource, graph) -> None:
+    def predecessor_added(self, resource: BaseResource, graph: Any) -> None:
         """Called when a predecessor is added to this node"""
         pass
 
-    def successor_added(self, resource, graph) -> None:
+    def successor_added(self, resource: BaseResource, graph: Any) -> None:
         """Called when a successor is added to this node"""
         pass
 
-    def ancestors(self, graph, edge_type=None) -> Iterator:
+    def ancestors(self, graph: Any, edge_type: Optional[EdgeType] = None) -> Iterator[BaseResource]:
         """Returns an iterator of the node's ancestors"""
         if graph is None:
             graph = self._graph
         if graph is None:
-            return ()
-        return graph.ancestors(self, edge_type=edge_type)
+            return iter(())
+        return graph.ancestors(self, edge_type=edge_type)  # type: ignore
 
-    def descendants(self, graph, edge_type=None) -> Iterator:
+    def descendants(self, graph: Any, edge_type: Optional[EdgeType] = None) -> Iterator[BaseResource]:
         """Returns an iterator of the node's descendants"""
         if graph is None:
             graph = self._graph
         if graph is None:
-            return ()
-        return graph.descendants(self, edge_type=edge_type)
+            return iter(())
+        return graph.descendants(self, edge_type=edge_type)  # type: ignore
 
     @property
-    def _graph(self):
+    def _graph(self) -> Optional[Any]:
         if self.__graph is not None:
             return self.__graph()
+        else:
+            return None
 
     @_graph.setter
-    def _graph(self, value) -> None:
-        self.__graph = weakref.ref(value)
+    def _graph(self, value: Any) -> None:
+        self.__graph = weakref.ref(value)  # type: ignore
 
-    def __getstate__(self):
+    def __getstate__(self) -> Dict[str, Any]:
         ret = self.__dict__.copy()
         ret["_BaseResource__graph"] = None
         return ret
 
-    def __setstate__(self, state):
+    def __setstate__(self, state: Dict[str, Any]) -> None:
         self.__dict__.update(state)
 
 
-BaseResource.ctime = property(BaseResource._ctime_getter, BaseResource._ctime_setter)
-BaseResource.mtime = property(BaseResource._mtime_getter, BaseResource._mtime_setter)
-BaseResource.atime = property(BaseResource._atime_getter, BaseResource._atime_setter)
+BaseResource.ctime = property(BaseResource._ctime_getter, BaseResource._ctime_setter)  # type: ignore
+BaseResource.mtime = property(BaseResource._mtime_getter, BaseResource._mtime_setter)  # type: ignore
+BaseResource.atime = property(BaseResource._atime_getter, BaseResource._atime_setter)  # type: ignore
 
 
 BaseResourceType = TypeVar("BaseResourceType", bound=BaseResource)
 
 
 @define(eq=False, slots=False)
 class PhantomBaseResource(BaseResource):
     kind: ClassVar[str] = "phantom_resource"
     phantom: ClassVar[bool] = True
 
-    def update_tag(self, key, value) -> bool:
+    def update_tag(self, key: str, value: str) -> bool:
         log.error(f"Resource {self.rtdname} is a phantom resource and does not maintain tags")
         return False
 
-    def delete_tag(self, key) -> bool:
+    def delete_tag(self, key: str) -> bool:
         log.error(f"Resource {self.rtdname} is a phantom resource and does not maintain tags")
         return False
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         log.error(f"Resource {self.rtdname} is a phantom resource and can't be deleted")
         return False
 
-    def cleanup(self, graph=None) -> bool:
+    def cleanup(self, graph: Optional[Any] = None) -> bool:
         log.error(f"Resource {self.rtdname} is a phantom resource and can't be cleaned up")
         return False
 
 
 @define(eq=False, slots=False)
 class BaseQuota(PhantomBaseResource):
     metadata: ClassVar[Dict[str, Any]] = {"icon": "quota", "group": "control"}
@@ -712,54 +719,54 @@
 
 
 @define(eq=False, slots=False)
 class BaseCloud(BaseResource):
     kind: ClassVar[str] = "base_cloud"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "cloud", "group": "control"}
 
-    def cloud(self, graph=None):
+    def cloud(self, graph: Optional[Any] = None) -> BaseCloud:
         return self
 
 
 @define(eq=False, slots=False)
 class BaseAccount(BaseResource):
     kind: ClassVar[str] = "account"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "account", "group": "control"}
 
-    def account(self, graph=None):
+    def account(self, graph: Optional[Any] = None) -> BaseAccount:
         return self
 
 
 @define(eq=False, slots=False)
 class BaseRegion(BaseResource):
     kind: ClassVar[str] = "region"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "region", "group": "control"}
 
-    def region(self, graph=None):
+    def region(self, graph: Optional[Any] = None) -> BaseRegion:
         return self
 
 
 @define(eq=False, slots=False)
 class BaseZone(BaseResource):
     kind: ClassVar[str] = "zone"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "zone", "group": "control"}
 
-    def zone(self, graph=None):
+    def zone(self, graph: Optional[Any] = None) -> BaseZone:
         return self
 
 
 class InstanceStatus(Enum):
     RUNNING = "running"
     STOPPED = "stopped"
     TERMINATED = "terminated"
     BUSY = "busy"
     UNKNOWN = "unknown"
 
 
-def serialize_enum(obj, **kwargs):
+def serialize_enum(obj: Enum, **kwargs: Any) -> Any:
     return obj.value
 
 
 jsons.set_serializer(serialize_enum, InstanceStatus)
 
 
 @define(eq=False, slots=False)
@@ -767,17 +774,14 @@
     kind: ClassVar[str] = "instance"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "instance", "group": "compute"}
     instance_cores: float = 0.0
     instance_memory: float = 0.0
     instance_type: Optional[str] = ""
     instance_status: Optional[InstanceStatus] = None
 
-    def instance_type_info(self, graph) -> BaseInstanceType:
-        return graph.search_first_parent_class(self, BaseInstanceType)
-
 
 @define(eq=False, slots=False)
 class BaseVolumeType(BaseType):
     kind: ClassVar[str] = "volume_type"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "volume_type", "group": "storage"}
     volume_type: str = ""
     ondemand_cost: float = 0.0
@@ -819,17 +823,14 @@
     volume_type: str = ""
     volume_status: Optional[VolumeStatus] = None
     volume_iops: Optional[int] = None
     volume_throughput: Optional[int] = None
     volume_encrypted: Optional[bool] = None
     snapshot_before_delete: bool = False
 
-    def volume_type_info(self, graph) -> BaseVolumeType:
-        return graph.search_first_parent_class(self, BaseVolumeType)
-
 
 @define(eq=False, slots=False)
 class BaseSnapshot(BaseResource):
     kind: ClassVar[str] = "snapshot"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "snapshot", "group": "storage"}
     snapshot_status: str = ""
     description: Optional[str] = None
@@ -841,24 +842,24 @@
 
 
 @define(eq=False, slots=False)
 class Cloud(BaseCloud):
     kind: ClassVar[str] = "cloud"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "cloud", "group": "control"}
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         return False
 
 
 @define(eq=False, slots=False)
 class GraphRoot(PhantomBaseResource):
     kind: ClassVar[str] = "graph_root"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "graph_root", "group": "control"}
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         return False
 
 
 @define(eq=False, slots=False)
 class BaseBucket(BaseResource):
     kind: ClassVar[str] = "bucket"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "bucket", "group": "storage"}
@@ -1046,15 +1047,15 @@
 
 @define(eq=False, slots=False)
 class BaseStack(BaseResource):
     kind: ClassVar[str] = "stack"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "stack", "group": "control"}
     stack_status: str = ""
     stack_status_reason: str = ""
-    stack_parameters: Dict = field(factory=dict)
+    stack_parameters: Dict[str, str] = field(factory=dict)
 
 
 @define(eq=False, slots=False)
 class BaseAutoScalingGroup(BaseResource):
     kind: ClassVar[str] = "autoscaling_group"
     metadata: ClassVar[Dict[str, Any]] = {"icon": "autoscaling_group", "group": "compute"}
     min_size: int = -1
@@ -1095,23 +1096,21 @@
     record_type: str = ""
     record_values: List[str] = field(factory=list)
 
     def __attrs_post_init__(self) -> None:
         super().__attrs_post_init__()
         self.record_type = self.record_type.upper()
 
-    def dns_zone(self, graph=None) -> "BaseDNSZone":
+    def dns_zone(self, graph: Optional[Any] = None) -> "BaseDNSZone":
         if graph is None:
             graph = self._graph
-        dns_zone = graph.search_first_parent_class(self, BaseDNSZone)
-        if dns_zone is None:
-            dns_zone = UnknownDNSZone(id="undefined", tags={})
-        return dns_zone
+        dns_zone = graph.search_first_parent_class(self, BaseDNSZone) if graph else None
+        return dns_zone or UnknownDNSZone(id="undefined", tags={})
 
-    def _keys(self) -> tuple:
+    def _keys(self) -> tuple[Any, ...]:
         if self._graph is None:
             raise RuntimeError(f"_keys() called on {self.rtdname} before resource was added to graph")
         return (
             self.kind,
             self.cloud().id,
             self.account().id,
             self.region().id,
@@ -1145,23 +1144,21 @@
     record_expire: Optional[int] = None
     record_minimum: Optional[int] = None
 
     def __attrs_post_init__(self) -> None:
         super().__attrs_post_init__()
         self.record_type = self.record_type.upper()
 
-    def dns_zone(self, graph=None) -> "BaseDNSZone":
+    def dns_zone(self, graph: Optional[Any] = None) -> "BaseDNSZone":
         if graph is None:
             graph = self._graph
-        dns_zone = graph.search_first_parent_class(self, BaseDNSZone)
-        if dns_zone is None:
-            dns_zone = UnknownDNSZone(id="undefined", tags={})
-        return dns_zone
+        dns_zone = graph.search_first_parent_class(self, BaseDNSZone) if graph else None
+        return dns_zone or UnknownDNSZone(id="undefined", tags={})
 
-    def _keys(self) -> tuple:
+    def _keys(self) -> tuple[Any, ...]:
         if self._graph is None:
             raise RuntimeError(f"_keys() called on {self.rtdname} before resource was added to graph")
         return (
             self.kind,
             self.cloud().id,
             self.account().id,
             self.region().id,
@@ -1174,52 +1171,52 @@
         )
 
 
 @define(eq=False, slots=False)
 class UnknownCloud(BaseCloud):
     kind: ClassVar[str] = "unknown_cloud"
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         return False
 
 
 @define(eq=False, slots=False)
 class UnknownAccount(BaseAccount):
     kind: ClassVar[str] = "unknown_account"
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         return False
 
 
 @define(eq=False, slots=False)
 class UnknownRegion(BaseRegion):
     kind: ClassVar[str] = "unknown_region"
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         return False
 
 
 @define(eq=False, slots=False)
 class UnknownDNSZone(BaseDNSZone):
     kind: ClassVar[str] = "unknown_dns_zone"
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         return False
 
 
 @define(eq=False, slots=False)
 class UnknownZone(BaseZone):
     kind: ClassVar[str] = "unknown_zone"
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         return False
 
 
 @define(eq=False, slots=False)
 class UnknownLocation(BaseResource):
     kind: ClassVar[str] = "unknown_location"
 
-    def delete(self, graph) -> bool:
+    def delete(self, graph: Any) -> bool:
         return False
 
 
 resolve_types(BaseResource)
```

### Comparing `resotolib-3.4.0/resotolib/config.py` & `resotolib-3.4.1/resotolib/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,28 @@
             raise TypeError(f"Cannot apply {type(other)} to RunningConfig")
 
 
 _config = RunningConfig()
 
 
 class MetaConfig(type):
-    def __getattr__(cls, name):
+    def __getattr__(cls, name: str) -> Any:
         if name in _config.data:
             return _config.data[name]
         else:
             raise ConfigNotFoundError(f"No such config {name}")
 
 
 class Config(metaclass=MetaConfig):
     running_config: RunningConfig = _config
 
     def __init__(
         self,
         config_name: str,
-        resotocore_uri: str = None,
+        resotocore_uri: Optional[str] = None,
         tls_data: Optional[TLSData] = None,
     ) -> None:
         self._config_lock = threading.Lock()
         self.config_name = config_name
         self._initial_load = True
         resotocore = ResotocoreURI(resotocore_uri)
         self.resotocore_uri = resotocore.http_uri
@@ -75,22 +75,22 @@
         self._ce = CoreEvents(
             resotocore.ws_uri,
             events={"config-updated"},
             message_processor=self.on_config_event,
             tls_data=tls_data,
         )
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> Any:
         if name in self.running_config.data:
             return self.running_config.data[name]
         else:
             raise ConfigNotFoundError(f"No such config {name}")
 
     def shutdown(self) -> None:
-        self._ce.stop()
+        self._ce.shutdown()
 
     @staticmethod
     def init_default_config() -> None:
         for config_id, config_data in Config.running_config.classes.items():
             if config_id not in Config.running_config.data:
                 log.debug(f"Initializing defaults for config section {config_id}")
                 Config.running_config.data[config_id] = config_data()
@@ -99,17 +99,17 @@
     def add_config(config: object) -> None:
         """Add a config to the config manager.
 
         Takes a dataclass as input and adds its fields to the config store.
         Dataclass must have a kind ClassVar which specifies the top level config name.
         """
         if hasattr(config, "kind"):
-            Config.running_config.classes[config.kind] = config
+            Config.running_config.classes[config.kind] = config  # type: ignore
             Config.running_config.types[config.kind] = {}
-            for field in fields(config):
+            for field in fields(config):  # type: ignore
                 if hasattr(field, "type"):
                     Config.running_config.types[config.kind][field.name] = optional_origin(field.type)
         else:
             raise RuntimeError("Config must have a 'kind' attribute")
 
     def load_config(self, reload: bool = False) -> None:
         if len(Config.running_config.classes) == 0:
@@ -124,15 +124,15 @@
             # Load the config from the core, populate it with defaults
             # and send it back to resotocore
             ############################################################
             try:
                 # We need two configs here: one with env_vars resolved and overrides applied
                 # and one with the raw config as it was stored in the database
                 config_response, new_config_revision = get_config(
-                    self.config_name, self.resotocore_uri, verify=self.verify
+                    self.config_name, self.resotocore_uri, verify=self.verify  # type: ignore
                 )
                 # config with env_vars resolved and overrides applied
                 config_json = config_response["config"]
                 config_json = {
                     k: replace_env_vars(v, os.environ, keep_unresolved=False) for k, v in config_json.items()
                 }
                 # raw config as it was stored in the database, to be sent to the core
@@ -228,26 +228,26 @@
         new_config = {}
         for config_id, config_data in config.items():
             if config_data is None:
                 config_data = {}
             if config_id in Config.running_config.classes:
                 message = f" reason: {reason}" if reason else ""
                 log.debug(f"Loading config section {config_id}" + message)
-                clazz: Type[Any] = Config.running_config.classes.get(config_id, Any) if not read_as_json else Any
+                clazz: Type[Any] = Config.running_config.classes.get(config_id, Any) if not read_as_json else Any  # type: ignore # noqa: E501
                 # use the from_json class from config, if available
                 if loader := getattr(clazz, "from_json", None):
                     new_config[config_id] = loader(config_data)
                 else:
                     new_config[config_id] = from_json(config_data, clazz)
             else:
                 log.warning(f"Unknown config section {config_id}")
         return new_config
 
     @staticmethod
-    def restart_required(new_config: Dict) -> bool:
+    def restart_required(new_config: Json) -> bool:
         for config_id, config_data in new_config.items():
             if config_id in Config.running_config.data:
                 for field in fields(type(config_data)):
                     if field.metadata.get("restart_required", False):
                         old_value = getattr(Config.running_config.data[config_id], field.name, None)
                         new_value = getattr(config_data, field.name, None)
                         if new_value != old_value:
@@ -328,28 +328,28 @@
                     config_value = target_type(config_value.split(","))
                 config_value = convert(config_value, target_type)
 
             except Exception:
                 log.exception(f"Failed to override config {override}")
 
     @staticmethod
-    def cast_target_type(config_value: Any, current_value: Any, fallback_target_type: type) -> object:
+    def cast_target_type(config_value: Any, current_value: Any, fallback_target_type: Optional[type]) -> object:
         if current_value is None and fallback_target_type is not None:
             target_type = fallback_target_type
         else:
             target_type = type(current_value)
         if target_type in (list, tuple, set):
             config_value = target_type(config_value.split(","))
         else:
             config_value = convert(config_value, target_type)
         return config_value
 
     @staticmethod
-    def dict() -> Dict:
-        return jsons.dump(Config.running_config.data, strip_attr="kind", strip_properties=True, strip_privates=True)
+    def dict() -> Json:
+        return jsons.dump(Config.running_config.data, strip_attr="kind", strip_properties=True, strip_privates=True)  # type: ignore # noqa: E501
 
     def save_config(self) -> None:
         update_config_model(self.model, resotocore_uri=self.resotocore_uri, verify=self.verify)
         stored_config_revision = set_config(self.config_name, self.dict(), self.resotocore_uri, verify=self.verify)
         if stored_config_revision != Config.running_config.revision:
             Config.running_config.revision = stored_config_revision
             log.debug(f"Saved config {self.config_name} revision {Config.running_config.revision}")
@@ -375,15 +375,15 @@
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Config):
             return self.running_config.__dict__ == other.running_config.__dict__
         return False
 
     @property
-    def model(self) -> List:
+    def model(self) -> List[Json]:
         """Return the config dataclass model in resotocore format"""
         classes = set(_config.classes.values())
         return dataclasses_to_resotocore_model(classes)
 
     @staticmethod
     def add_args(arg_parser: ArgumentParser) -> None:
         arg_parser.add_argument(
```

### Comparing `resotolib-3.4.0/resotolib/core/__init__.py` & `resotolib-3.4.1/resotolib/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         pass
     return False
 
 
 def wait_for_resotocore(resotocore_uri: str, timeout: int = 300) -> None:
     start_time = time.time()
     core_up = False
-    wait_time = -1
-    remaining_wait = timeout
+    wait_time: float = -1
+    remaining_wait: float = timeout
     waitlog = log.info
     while wait_time < timeout:
         if resotocore_is_up(resotocore_uri):
             core_up = True
             break
         else:
             waitlog(f"Waiting up to {remaining_wait:.2f}s for resotocore" f" to come online at {resotocore_uri}")
@@ -61,15 +61,15 @@
                 resotocore_uri = str(resotocore_uri).rstrip("/")
             else:
                 resotocore_uri = "https://localhost:8900"
         else:
             resotocore_uri = self.resotocore_uri
         if resotocore_uri is None:
             raise AttributeError("resotocore_uri is not set")
-        return urlparse(resotocore_uri)
+        return urlparse(resotocore_uri)  # type: ignore
 
     @property
     def http_uri(self) -> str:
         return f"{self.uri.scheme}://{self.uri.netloc}{self.uri.path}"
 
     @property
     def ws_uri(self) -> str:
```

### Comparing `resotolib-3.4.0/resotolib/core/actions.py` & `resotolib-3.4.1/resotolib/core/actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 import websocket
 import requests
 import json
 from concurrent.futures import ThreadPoolExecutor
 
 from attr import define, evolve, field
+from requests import Response
 
 from resotolib.core.progress import Progress, ProgressDone
 from resotolib.logger import log
 from resotolib.event import EventType, remove_event_listener, add_event_listener, Event
 from resotolib.args import ArgumentParser
 from resotolib.jwt import encode_jwt_to_headers
 from resotolib.core.ca import TLSData
-from typing import Callable, Dict, Optional, List
+from typing import Callable, Dict, Optional, List, Any
 
 from resotolib.types import Json
 from resotolib.utils import utc_str
 
 
 @define(frozen=True)
 class CoreFeedback:
@@ -52,15 +53,15 @@
         if logger:
             logger.warning(self.context_str + message)
         self._info_message("info", message)
 
     def error(self, message: str, logger: Optional[Logger] = None) -> None:
         if logger:
             logger.error(self.context_str + message)
-        self._info_message("error", message)
+        self._info_message("error", message[0:250])  # truncate message to 250 characters
 
     @property
     def context_str(self) -> str:
         return "[" + (":".join(self.context)) + "] " if self.context else ""
 
     def _info_message(self, level: str, message: str) -> None:
         self.core_messages.put(
@@ -85,40 +86,41 @@
 
 class CoreActions(threading.Thread):
     def __init__(
         self,
         identifier: str,
         resotocore_uri: str,
         resotocore_ws_uri: str,
-        actions: Dict,
+        actions: Dict[str, Json],
         incoming_messages: Optional[Queue[Json]] = None,
-        message_processor: Optional[Callable] = None,
+        message_processor: Optional[Callable[[Json], Any]] = None,
         tls_data: Optional[TLSData] = None,
         max_concurrent_actions: int = 5,
     ) -> None:
         super().__init__()
         self.identifier = identifier
         self.resotocore_uri = resotocore_uri
         self.resotocore_ws_uri = resotocore_ws_uri
         self.actions = actions
         self.message_processor = message_processor
-        self.ws = None
+        self.ws: Optional[websocket.WebSocketApp] = None
         self.incoming_messages = incoming_messages
         self.tls_data = tls_data
         self.shutdown_event = threading.Event()
         # one thread is taken by the queue listener
         self.executor = ThreadPoolExecutor(max_workers=max_concurrent_actions + 1, thread_name_prefix=self.identifier)
 
     def run(self) -> None:
-        def listen_on_queue(in_messages: Queue) -> None:
+        def listen_on_queue(in_messages: Queue[Json]) -> None:
             while not self.shutdown_event.is_set():
                 with suppress(Exception):
                     message = in_messages.get(timeout=1)
                     log.debug("Got feedback message. Send it to core", message)
-                    self.ws.send(json.dumps(message))
+                    if self.ws:
+                        self.ws.send(json.dumps(message))
 
         self.name = self.identifier
         add_event_listener(EventType.SHUTDOWN, self.shutdown)
         if self.incoming_messages:
             self.executor.submit(listen_on_queue, self.incoming_messages)
         while not self.shutdown_event.is_set():
             log.debug("Connecting to resotocore message bus")
@@ -138,15 +140,15 @@
         for event, data in self.actions.items():
             if not isinstance(data, dict):
                 data = None
             self.register(event, data)
 
         ws_uri = f"{self.resotocore_ws_uri}/subscriber/{self.identifier}/handle"
         log.debug(f"{self.identifier} connecting to {ws_uri}")
-        headers = {}
+        headers: Dict[str, str] = {}
         if getattr(ArgumentParser.args, "psk", None):
             encode_jwt_to_headers(headers, {}, ArgumentParser.args.psk)
         try:
             self.ws = websocket.WebSocketApp(
                 ws_uri,
                 header=headers,
                 on_open=self.on_open,
@@ -159,31 +161,36 @@
             sslopt = None
             if self.tls_data:
                 sslopt = {"ca_certs": self.tls_data.ca_cert_path}
             self.ws.run_forever(sslopt=sslopt, ping_interval=20, ping_timeout=10, ping_payload="ping")
         finally:
             self.ws = None
 
-    def shutdown(self, event: Event = None) -> None:
+    def shutdown(self, event: Optional[Event] = None) -> None:
         remove_event_listener(EventType.SHUTDOWN, self.shutdown)
         log.debug("Received shutdown event - shutting down resotocore message bus listener")
         self.shutdown_event.set()
         self.executor.shutdown(wait=False, cancel_futures=True)
         if self.ws:
             self.ws.close()
 
-    def register(self, action: str, data: Optional[Dict] = None) -> bool:
+    def register(self, action: str, data: Optional[Dict[str, str]] = None) -> bool:
         log.debug(f"{self.identifier} registering for {action} actions ({data})")
         return self.registration(action, requests.post, data)
 
-    def unregister(self, action: str, data: Optional[Dict] = None) -> bool:
+    def unregister(self, action: str, data: Optional[Dict[str, str]] = None) -> bool:
         log.debug(f"{self.identifier} unregistering from {action} actions ({data})")
         return self.registration(action, requests.delete, data)
 
-    def registration(self, action: str, client: Callable, data: Optional[Dict] = None) -> bool:
+    def registration(
+        self,
+        action: str,
+        client: Callable[..., Response],
+        data: Optional[Dict[str, str]] = None,
+    ) -> bool:
         url = f"{self.resotocore_uri}/subscriber/{self.identifier}/{action}"
         headers = {"accept": "application/json"}
 
         if getattr(ArgumentParser.args, "psk", None):
             encode_jwt_to_headers(headers, {}, ArgumentParser.args.psk)
 
         verify = None
@@ -196,36 +203,36 @@
         return True
 
     def on_message(self, _: websocket.WebSocketApp, message: str) -> None:
         self.executor.submit(self.process_message, message)
 
     def process_message(self, message: str) -> None:
         try:
-            message: Json = json.loads(message)
+            json_message: Json = json.loads(message)
         except json.JSONDecodeError:
             log.exception(f"Unable to decode received message {message}")
             return
         log.debug(f"{self.identifier} received: {message}")
         if self.message_processor is not None and callable(self.message_processor):
             try:
-                result = self.message_processor(message)
+                result: Json = self.message_processor(json_message)
                 if result is None:
                     return
-                if self.wait_for_ws():
+                if self.wait_for_ws() and self.ws:
                     log.debug(f"Sending reply {result}")
                     self.ws.send(json.dumps(result))
                 else:
                     log.error(f"Unable to send reply {result}")
             except Exception:
                 log.exception(f"Something went wrong while processing {message}")
 
     def on_error(self, _: websocket.WebSocketApp, e: Exception) -> None:
         log.debug(f"{self.identifier} message bus error: {e!r}")
 
-    def on_close(self, _: websocket.WebSocketApp, close_status_code: int, close_msg: str):
+    def on_close(self, _: websocket.WebSocketApp, close_status_code: int, close_msg: str) -> None:
         log.debug(f"{self.identifier} disconnected from resotocore message bus: {close_status_code}: {close_msg}")
 
     def on_open(self, _: websocket.WebSocketApp) -> None:
         log.debug(f"{self.identifier} connected to resotocore message bus")
 
     def on_ping(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug(f"{self.identifier} actions ping from resotocore message bus")
```

### Comparing `resotolib-3.4.0/resotolib/core/ca.py` & `resotolib-3.4.1/resotolib/core/ca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import time
 import warnings
 import requests
 from ssl import create_default_context, SSLContext
-from typing import Tuple, Optional, List, Dict, Union
+from typing import Tuple, Optional, List, Dict, Union, Any
 from resotolib.args import ArgumentParser
 from resotolib.core import resotocore
 from resotolib.x509 import (
     csr_to_bytes,
     load_cert_from_bytes,
     cert_fingerprint,
     gen_rsa_key,
@@ -60,17 +60,17 @@
         return ca_cert
 
 
 def get_signed_cert(
     common_name: str,
     san_dns_names: Optional[List[str]] = None,
     san_ip_addresses: Optional[List[str]] = None,
-    resotocore_uri: str = None,
-    psk: str = None,
-    ca_cert_path: str = None,
+    resotocore_uri: Optional[str] = None,
+    psk: Optional[str] = None,
+    ca_cert_path: Optional[str] = None,
     connect_to_ips: Optional[List[str]] = None,
 ) -> Tuple[RSAPrivateKey, Certificate]:
     if resotocore_uri is None:
         resotocore_uri = getattr(ArgumentParser.args, "resotocore_uri", None)
     if psk is None:
         psk = getattr(ArgumentParser.args, "psk", None)
 
@@ -79,66 +79,66 @@
         cert_key,
         common_name=common_name,
         connect_to_ips=connect_to_ips,
         san_dns_names=san_dns_names,
         san_ip_addresses=san_ip_addresses,
     )
     cert_csr_bytes = csr_to_bytes(cert_csr)
-    headers = {}
+    headers: Dict[str, str] = {}
     if psk is not None:
         encode_jwt_to_headers(headers, {}, psk)
-    request_kwargs = {}
+    request_kwargs: Dict[str, str] = {}
     if ca_cert_path is not None:
         request_kwargs["verify"] = ca_cert_path
-    r = requests.post(f"{resotocore_uri}/ca/sign", cert_csr_bytes, headers=headers, **request_kwargs)
+    r = requests.post(f"{resotocore_uri}/ca/sign", cert_csr_bytes, headers=headers, **request_kwargs)  # type: ignore
     if r.status_code != 200:
         raise ValueError(f"Failed to get signed certificate: {r.text}")
     cert_bytes = r.content
     cert_crt = load_cert_from_bytes(cert_bytes)
     return cert_key, cert_crt
 
 
 class TLSData:
     def __init__(
         self,
         common_name: str,
         san_dns_names: Optional[List[str]] = None,
         san_ip_addresses: Optional[List[str]] = None,
-        tempdir: str = None,
-        resotocore_uri: str = None,
-        psk: str = None,
+        tempdir: Optional[str] = None,
+        resotocore_uri: Optional[str] = None,
+        psk: Optional[str] = None,
         ca_only: bool = False,
         renew_before: timedelta = timedelta(days=1),
     ) -> None:
         self.common_name = common_name
         self.san_dns_names = san_dns_names
         self.san_ip_addresses = san_ip_addresses
         self.__ca_only = ca_only
         self.renew_before = renew_before
         self.__tempdir = TemporaryDirectory(prefix="resoto-cert-", dir=tempdir)
         if resotocore_uri is None:
             resotocore_uri = resotocore.http_uri
         self.__resotocore_uri = resotocore_uri
         self.__psk = psk
-        self.__ca_cert = None
-        self.__cert = None
-        self.__key = None
+        self.__ca_cert: Optional[Certificate] = None
+        self.__cert: Optional[Certificate] = None
+        self.__key: Optional[RSAPrivateKey] = None
         self.__ca_cert_path = f"{self.__tempdir.name}/ca.crt"
         self.__cert_path = f"{self.__tempdir.name}/cert.crt"
         self.__key_path = f"{self.__tempdir.name}/cert.key"
         self.__load_lock = Lock()
         self.__loaded = Event()
         self.__exit = Condition()
         self.__watcher: Optional[Thread] = None
 
     def __enter__(self) -> "TLSData":
         self.start()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.shutdown()
 
     def start(self) -> None:
         if self.__watcher is None:
             self.load()
             self.__watcher = Thread(target=self.__certificates_watcher, name="certificates_watcher")
             self.__watcher.start()
@@ -147,31 +147,31 @@
     def shutdown(self, event: Optional[ResotoEvent] = None) -> None:
         if self.__watcher is not None:
             with self.__exit:
                 self.__exit.notify()
             self.__watcher.join()
             self.__watcher = None
 
-    def __getstate__(self):
+    def __getstate__(self) -> Dict[str, Any]:
         d = self.__dict__.copy()
         del d["_TLSData__load_lock"]
         del d["_TLSData__loaded"]
         del d["_TLSData__exit"]
         del d["_TLSData__ca_cert"]
         del d["_TLSData__cert"]
         del d["_TLSData__key"]
         del d["_TLSData__watcher"]
         d["__is_loaded"] = self.__loaded.is_set()
         if self.__loaded.is_set():
-            d["__ca_cert_bytes"] = cert_to_bytes(self.__ca_cert)
-            d["__cert_bytes"] = cert_to_bytes(self.__cert)
-            d["__key_bytes"] = key_to_bytes(self.__key)
+            d["__ca_cert_bytes"] = cert_to_bytes(self.__ca_cert)  # type: ignore
+            d["__cert_bytes"] = cert_to_bytes(self.__cert)  # type: ignore
+            d["__key_bytes"] = key_to_bytes(self.__key)  # type: ignore
         return d
 
-    def __setstate__(self, d):
+    def __setstate__(self, d: Dict[str, Any]) -> None:
         d["_TLSData__load_lock"] = Lock()
         d["_TLSData__loaded"] = Event()
         d["_TLSData__exit"] = Condition()
         d["_TLSData__ca_cert"] = None
         d["_TLSData__cert"] = None
         d["_TLSData__key"] = None
         if d["__is_loaded"]:
@@ -209,17 +209,17 @@
         if not self.__loaded.is_set():
             return
         try:
             last_ca_cert_update = time.time() - os.path.getmtime(self.__ca_cert_path)
             last_cert_update = time.time() - os.path.getmtime(self.__cert_path)
             if last_ca_cert_update > refresh_every_sec or last_cert_update > refresh_every_sec:
                 log.debug("Refreshing cert/key files on disk")
-                write_ca_bundle(self.__ca_cert, self.__ca_cert_path, include_certifi=True)
-                write_cert_to_file(self.__cert, self.__cert_path)
-                write_key_to_file(self.__key, self.__key_path)
+                write_ca_bundle(self.__ca_cert, self.__ca_cert_path, include_certifi=True)  # type: ignore
+                write_cert_to_file(self.__cert, self.__cert_path)  # type: ignore
+                write_key_to_file(self.__key, self.__key_path)  # type: ignore
         except FileNotFoundError:
             pass
 
     def load(self) -> None:
         with self.__load_lock:
             if getattr(ArgumentParser.args, "ca_cert", None) is not None:
                 log.debug(f"Loading CA certificate from {ArgumentParser.args.ca_cert}")
@@ -266,29 +266,32 @@
                     )
                 log.debug(f"Writing signed cert/key {self.__cert_path}")
                 write_cert_to_file(self.__cert, self.__cert_path)
                 write_key_to_file(self.__key, self.__key_path)
             self.__loaded.set()
 
     @property
-    def ca_cert(self) -> str:
+    def ca_cert(self) -> Certificate:
         if not os.path.isfile(self.__ca_cert_path):
             self.load()
+        assert self.__ca_cert is not None, "CA cert is None"
         return self.__ca_cert
 
     @property
-    def cert(self) -> str:
+    def cert(self) -> Certificate:
         if not self.__loaded.is_set():
             self.load()
+        assert self.__cert is not None, "Cert is None"
         return self.__cert
 
     @property
-    def key(self) -> str:
+    def key(self) -> RSAPrivateKey:
         if not self.__loaded.is_set():
             self.load()
+        assert self.__key is not None, "Key is None"
         return self.__key
 
     @property
     def ca_cert_path(self) -> str:
         if not os.path.isfile(self.__ca_cert_path):
             self.load()
         return self.__ca_cert_path
```

### Comparing `resotolib-3.4.0/resotolib/core/config.py` & `resotolib-3.4.1/resotolib/core/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import requests
 import json
-from typing import Dict, Tuple, List, Optional
+from typing import Dict, Tuple, List, Optional, cast, Union
 from resotolib.core import resotocore
 from resotolib.args import ArgumentParser
 from resotolib.jwt import encode_jwt_to_headers
 from resotolib.logger import log
+from resotolib.types import Json
 
 
-def default_args(resotocore_uri: str = None, psk: str = None, headers=None) -> Tuple[str, str, Dict[str, str]]:
+def default_args(
+    resotocore_uri: Optional[str] = None, psk: Optional[str] = None, headers: Optional[Dict[str, str]] = None
+) -> Tuple[str, Optional[str], Dict[str, str]]:
     if resotocore_uri is None:
         resotocore_uri = resotocore.http_uri
     if psk is None:
         psk = getattr(ArgumentParser.args, "psk", None)
     if headers is None:
         headers = {}
     if psk is not None:
@@ -19,30 +22,32 @@
     return resotocore_uri, psk, headers
 
 
 class ConfigNotFoundError(AttributeError):
     pass
 
 
-def get_configs(resotocore_uri: str = None, psk: str = None, verify: Optional[str] = None) -> List:
+def get_configs(
+    resotocore_uri: Optional[str] = None, psk: Optional[str] = None, verify: Optional[str] = None
+) -> List[Json]:
     resotocore_uri, psk, headers = default_args(resotocore_uri, psk)
 
     log.debug("Getting configs")
     r = requests.get(f"{resotocore_uri}/configs", headers=headers, verify=verify)
     if r.status_code == 200:
-        return r.json()
+        return cast(List[Json], r.json())
     raise RuntimeError(f"Error getting configs: {r.content.decode('utf-8')}")
 
 
 def get_config(
     config_id: str,
-    resotocore_uri: str = None,
-    psk: str = None,
+    resotocore_uri: Optional[str] = None,
+    psk: Optional[str] = None,
     verify: Optional[str] = None,
-) -> Tuple[Dict, str]:
+) -> Tuple[Json, str]:
     resotocore_uri, psk, headers = default_args(resotocore_uri, psk)
 
     log.debug(f"Getting config {config_id}")
 
     params = {
         "separate_overrides": "true",  # we don not to have a single config with everything merged into it
         "apply_overrides": "true",  # apply the overrides to the config
@@ -62,18 +67,18 @@
     elif r.status_code == 404:
         raise ConfigNotFoundError(f"Config {config_id} does not exist")
     raise RuntimeError(f"Error getting config {config_id}: {r.content.decode('utf-8')}")
 
 
 def set_config(
     config_id: str,
-    config: Dict,
-    resotocore_uri: str = None,
-    psk: str = None,
-    verify: Optional[str] = None,
+    config: Json,
+    resotocore_uri: Optional[str] = None,
+    psk: Optional[str] = None,
+    verify: Union[str, bool, None] = None,
 ) -> str:
     resotocore_uri, psk, headers = default_args(resotocore_uri, psk)
 
     log.debug(f"Storing config {config_id}")
     r = requests.put(
         f"{resotocore_uri}/config/{config_id}",
         json=config,
@@ -84,36 +89,37 @@
         revision = r.headers.get("Resoto-Config-Revision", "unknown")
         return revision
     raise RuntimeError(f"Error storing config {config_id}: {r.content.decode('utf-8')}")
 
 
 def delete_config(
     config_id: str,
-    resotocore_uri: str = None,
-    psk: str = None,
-    verify: Optional[str] = None,
+    resotocore_uri: Optional[str] = None,
+    psk: Optional[str] = None,
+    verify: Union[str, bool, None] = None,
 ) -> bool:
     resotocore_uri, psk, headers = default_args(resotocore_uri, psk)
 
     log.debug(f"Deleting config {config_id}")
     r = requests.delete(f"{resotocore_uri}/config/{config_id}", headers=headers, verify=verify)
     if r.status_code == 204:
         return True
     raise RuntimeError(f"Error deleting config {config_id}: {r.content.decode('utf-8')}")
 
 
 def update_config_model(
-    model: List,
-    resotocore_uri: str = None,
-    psk: str = None,
-    verify: Optional[str] = None,
+    model: List[Json],
+    resotocore_uri: Optional[str] = None,
+    psk: Optional[str] = None,
+    verify: Union[str, bool, None] = None,
 ) -> bool:
     headers = {"Content-Type": "application/json"}
     resotocore_uri, psk, headers = default_args(resotocore_uri, psk, headers=headers)
     model_uri = f"{resotocore_uri}/configs/model"
     model_json = json.dumps(model, indent=4)
 
     log.debug("Updating config model")
     r = requests.patch(model_uri, data=model_json, headers=headers, verify=verify)
     if r.status_code != 200:
         log.error(r.content)
-        raise RuntimeError(f"Failed to update model: {r.content}")
+        raise RuntimeError(f"Failed to update model: {r.content.decode('utf-8')}")
+    return True
```

### Comparing `resotolib-3.4.0/resotolib/core/custom_command.py` & `resotolib-3.4.1/resotolib/core/custom_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Type, Optional
+from typing import Any, Dict, List, Type, Optional, Callable
 
 from resotolib.types import DecoratedFn
 
 definitions = "__task_definitions"
 
 
 class CommandDefinition:
@@ -29,25 +29,25 @@
         self.name = name
         self.info = info
         self.args_description = args_description
         self.description = description
         self.expect_resource = expect_resource
         self.expect_node_result = expect_node_result
         self.allowed_on_kind = allowed_on_kind
-        self.filter = filter
+        self.filter = filter or {}
 
-    def __set_name__(self, owner, name):
+    def __set_name__(self, owner: str, name: str) -> None:
         # store this definition on the owners side (class)
         if getattr(owner, definitions, None) is None:
             setattr(owner, definitions, [])
         getattr(owner, definitions).append(self)
         # make the function available at the call side (class)
         setattr(owner, name, self.fn)
 
-    def __call__(self) -> DecoratedFn:
+    def __call__(self) -> Callable[..., Any]:
         return self.fn
 
 
 # noinspection PyPep8Naming
 class execute_command:  # noqa: N801
     """
     In case you want to expose a method as worker task to the core, you can use this decorator.
@@ -90,15 +90,15 @@
         self.info = info
         self.args_description = args_description
         self.description = description
         self.expect_node_result = expect_node_result
         self.allowed_on_kind = allowed_on_kind
         self.filter = filter or {}
 
-    def __call__(self, fn: DecoratedFn) -> DecoratedFn:
+    def __call__(self, fn: DecoratedFn) -> CommandDefinition:
         return CommandDefinition(
             fn,
             name=self.name,
             info=self.info,
             args_description=self.args_description,
             description=self.description,
             expect_node_result=self.expect_node_result,
@@ -153,15 +153,15 @@
         self.info = info
         self.args_description = args_description
         self.description = description
         self.expect_node_result = expect_node_result
         self.allowed_on_kind = allowed_on_kind
         self.filter = filter or {}
 
-    def __call__(self, fn: DecoratedFn) -> DecoratedFn:
+    def __call__(self, fn: DecoratedFn) -> CommandDefinition:
         return CommandDefinition(
             fn,
             name=self.name,
             info=self.info,
             args_description=self.args_description,
             description=self.description,
             expect_node_result=self.expect_node_result,
```

### Comparing `resotolib-3.4.0/resotolib/core/events.py` & `resotolib-3.4.1/resotolib/core/events.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,36 @@
 from resotolib.logger import log
 from resotolib.event import EventType, remove_event_listener, add_event_listener, Event
 from resotolib.args import ArgumentParser
 from resotolib.jwt import encode_jwt_to_headers
 from resotolib.core.ca import TLSData
 from typing import Callable, Dict, Optional, Set
 
+from resotolib.types import Json
+
 
 class CoreEvents(threading.Thread):
     def __init__(
         self,
         resotocore_ws_uri: str,
-        events: Optional[Set] = None,
-        message_processor: Optional[Callable] = None,
+        events: Optional[Set[str]] = None,
+        message_processor: Optional[Callable[[Json], None]] = None,
         tls_data: Optional[TLSData] = None,
     ) -> None:
         super().__init__()
         self.ws_uri = f"{resotocore_ws_uri}/events"
         if events:
             query_string = urlencode({"show": ",".join(events)})
             self.ws_uri += f"?{query_string}"
         self.message_processor = message_processor
         self.tls_data = tls_data
-        self.ws = None
+        self.ws: Optional[websocket.WebSocketApp] = None
         self.shutdown_event = threading.Event()
 
-    def __del__(self):
+    def __del__(self) -> None:
         remove_event_listener(EventType.SHUTDOWN, self.shutdown)
 
     def run(self) -> None:
         self.name = "eventbus-listener"
         add_event_listener(EventType.SHUTDOWN, self.shutdown)
         while not self.shutdown_event.is_set():
             log.debug("Connecting to resotocore event bus")
@@ -41,15 +43,15 @@
                 self.connect()
             except Exception as e:
                 log.error(e)
             time.sleep(1)
 
     def connect(self) -> None:
         log.debug(f"Connecting to {self.ws_uri}")
-        headers = {}
+        headers: Dict[str, str] = {}
         if getattr(ArgumentParser.args, "psk", None):
             encode_jwt_to_headers(headers, {}, ArgumentParser.args.psk)
         self.ws = websocket.WebSocketApp(
             self.ws_uri,
             header=headers,
             on_open=self.on_open,
             on_message=self.on_message,
@@ -59,40 +61,40 @@
             on_pong=self.on_pong,
         )
         sslopt = None
         if self.tls_data:
             sslopt = {"ca_certs": self.tls_data.ca_cert_path}
         self.ws.run_forever(sslopt=sslopt, ping_interval=20, ping_timeout=10, ping_payload="ping")
 
-    def shutdown(self, event: Event = None) -> None:
+    def shutdown(self, event: Optional[Event] = None) -> None:
         log.debug("Received shutdown event - shutting down resotocore event bus listener")
         self.shutdown_event.set()
         if self.ws:
             self.ws.close()
 
-    def on_message(self, ws, message):
+    def on_message(self, _: websocket.WebSocketApp, message: str) -> None:
         try:
-            message: Dict = json.loads(message)
+            json_message: Json = json.loads(message)
         except json.JSONDecodeError:
             log.exception(f"Unable to decode received message {message}")
             return
-        log.debug(f"Received event: {message}")
+        log.debug(f"Received event: {json_message}")
         if self.message_processor is not None and callable(self.message_processor):
             try:
-                self.message_processor(message)
+                self.message_processor(json_message)
             except Exception:
                 log.exception(f"Something went wrong while processing {message}")
 
-    def on_error(self, ws, e):
+    def on_error(self, _: websocket.WebSocketApp, e: Exception) -> None:
         log.debug(f"Event bus error: {e!r}")
 
-    def on_close(self, ws, close_status_code, close_msg):
+    def on_close(self, _: websocket.WebSocketApp, close_status_code: int, close_msg: str) -> None:
         log.debug("Disconnected from resotocore event bus")
 
-    def on_open(self, ws):
+    def on_open(self, _: websocket.WebSocketApp) -> None:
         log.debug("Connected to resotocore event bus")
 
-    def on_ping(self, ws, message):
+    def on_ping(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug("Ping from resotocore event bus")
 
-    def on_pong(self, ws, message):
+    def on_pong(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug("Pong from resotocore event bus")
```

### Comparing `resotolib-3.4.0/resotolib/core/model_check.py` & `resotolib-3.4.1/resotolib/core/model_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from attrs import define
-from typing import List, Dict, Tuple, Type, Optional
+from typing import List, Dict, Tuple, Type, Optional, Any
 
 from resotolib.baseresources import BaseResource
 from resotolib.core.model_export import dataclasses_to_resotocore_model
 from resotolib.json import from_json
 from resotolib.types import Json
 
 
@@ -101,15 +101,15 @@
     This will try to load all models from all known plugins.
     The call will fail if the imports are not working - make sure the calling side has all those plugins installed.
 
     @param base: additional base classes to check for overlapping properties. All existing known plugins are added.
     :raise Exception: if there is an overlap
     """
 
-    def dynamic_import(name) -> List[type]:
+    def dynamic_import(name: str) -> List[Type[Any]]:
         components = name.split(".")
         mod = __import__(components[0])
         for comp in components[1:]:
             mod = getattr(mod, comp)
         if isinstance(mod, type):
             return [mod]
         elif isinstance(mod, list):
```

### Comparing `resotolib-3.4.0/resotolib/core/model_export.py` & `resotolib-3.4.1/resotolib/core/model_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,35 @@
 
 import attrs
 import cattrs
 from attr import resolve_types
 from attrs import Attribute
 
 from resotolib.baseresources import BaseResource
-from resotolib.durations import duration_str
 from resotolib.types import Json
-from resotolib.utils import type_str, str2timedelta, str2timezone, utc_str
+from resotolib.utils import type_str, str2timedelta, str2timezone
 
 if sys.version_info >= (3, 10):
     from types import UnionType, NoneType
 else:
     UnionType = Union
     NoneType = type(None)
 
 property_metadata_to_strip = ["restart_required", "description", "required", "kind"]
 
 
 # List[X] -> list, list -> list
-def optional_origin(clazz: type) -> type:
+def optional_origin(clazz: Type[Any]) -> Type[Any]:
     maybe_optional = get_args(clazz)[0] if is_optional(clazz) else clazz
     origin = get_origin(maybe_optional)
-    return origin if origin else maybe_optional
+    return origin if origin else maybe_optional  # type: ignore
 
 
 # Optional[x] -> true
-def is_optional(clazz: type) -> bool:
+def is_optional(clazz: Union[type, Tuple[Any]]) -> bool:
     args = get_args(clazz)
     return get_origin(clazz) is Union and type(None) in args and len(args) == 2
 
 
 # List[x] -> true, list -> true
 def is_collection(clazz: type) -> bool:
     return optional_origin(clazz) in [list, set, tuple]
@@ -56,15 +55,15 @@
     return isinstance(origin, type) and issubclass(origin, Enum)
 
 
 # List[X] -> X, list -> object
 def type_arg(clazz: type) -> type:
     maybe_optional = get_args(clazz)[0] if is_optional(clazz) else clazz
     args = get_args(maybe_optional)
-    return args[0] if args and len(args) == 1 else object
+    return args[0] if args and len(args) == 1 else object  # type: ignore
 
 
 # Dict[X,Y] -> (X,Y), dict -> (object, object)
 def dict_types(clazz: type) -> Tuple[type, type]:
     maybe_optional = get_args(clazz)[0] if is_optional(clazz) else clazz
     args = get_args(maybe_optional)
     return (args[0], args[1]) if args and len(args) == 2 else (object, object)
@@ -112,51 +111,53 @@
     date: "date",
     timedelta: "duration",
 }
 simple_type = tuple(lookup.keys())
 
 
 # Model name from the internal python class name
-def model_name(clazz: Union[type, Tuple[Any]]) -> str:
+def model_name(clazz: Union[type, Tuple[Any], None]) -> str:
+    if clazz is None:
+        return "any"
     to_check = get_args(clazz)[0] if is_optional(clazz) else clazz
     if is_collection(to_check):
         return f"{model_name(type_arg(to_check))}[]"
     elif is_dict(to_check):
         key_type, value_type = dict_types(to_check)
         return f"dictionary[{model_name(key_type)}, {model_name(value_type)}]"
     elif is_enum(to_check):
         # camel case to snake case
         return re.sub(r"(?<!^)(?=[A-Z])", "_", to_check.__name__).lower()
     elif get_origin(to_check) == Union:
         # this is a union of different types other than none.
         # since union types are not supported, we fallback to any here
         return "any"
     elif isinstance(to_check, TypeVar):
-        return model_name(get_args(to_check))
+        return model_name(get_args(to_check))  # type: ignore
     elif isinstance(to_check, type) and issubclass(to_check, simple_type):
         return lookup[to_check]
     elif attrs.has(to_check):
         name = getattr(to_check, "kind", None)
         if not name:
             raise AttributeError(f"dataclass {to_check} need to define a ClassVar kind!")
-        return name
+        return name  # type: ignore
     else:
         return "any"
 
 
 # define if a field should be exported or not.
 # Use python default: hide props starting with underscore.
-def should_export(field: Attribute) -> bool:
+def should_export(field: Attribute) -> bool:  # type: ignore
     return not field.name.startswith("_")
 
 
 def dataclasses_to_resotocore_model(
-    classes: Set[type],
+    classes: Set[Type[Any]],
     allow_unknown_props: bool = False,
-    aggregate_root: Optional[type] = None,
+    aggregate_root: Optional[Type[Any]] = None,
     walk_subclasses: bool = True,
 ) -> List[Json]:
     """
     Analyze all transitive dataclasses and create the model
     definition as understood by resotocore.
     A plain python dataclass defines the model structure and
     should be used to create json in the same format.
@@ -164,15 +165,15 @@
     :param classes: all dataclasses to analyze.
     :param allow_unknown_props: allow properties in json that are not defined in the model.
     :param aggregate_root: if a type is a subtype of this type, it will be considered an aggregate root.
     :param walk_subclasses: if true, all subclasses of the given classes will be analyzed as well.
     :return: the model definition in the resotocore json format.
     """
 
-    def prop(field: Attribute) -> List[Json]:
+    def prop(field: Attribute) -> List[Json]:  # type: ignore
         # the field itself can define the type via a type hint
         # this is useful for int and float in python where the representation can not be
         # detected by the type itself. Example: int32/int64 or float/double
         # If not defined, we fallback to the largest container: int64 and double
         name = field.name
         meta = field.metadata.copy()
         kind = meta.pop("type_hint", model_name(field.type))
@@ -230,15 +231,15 @@
                         for value in values:
                             successors[value][edge_type].append(name)
     successors = {k: {ik: list(set(iv)) for ik, iv in v.items()} for k, v in successors.items()}
 
     def export_data_class(clazz: type) -> None:
         bases = [base for base in clazz.__bases__ if attrs.has(base)]
         base_names = [model_name(base) for base in bases]
-        base_props: Set[Attribute] = reduce(lambda result, base: result | set(attrs.fields(base)), bases, set())
+        base_props: Set[Attribute] = reduce(lambda result, base: result | set(attrs.fields(base)), bases, set())  # type: ignore # noqa: E501
         props = [
             p for field in attrs.fields(clazz) if field not in base_props and should_export(field) for p in prop(field)
         ]
         root = any(sup == aggregate_root for sup in clazz.mro()) if aggregate_root else True
         kind = model_name(clazz)
         metadata: Optional[Json] = None
         if (m := getattr(clazz, "metadata", None)) and isinstance(m, dict):
@@ -268,15 +269,15 @@
         model.append({"fqn": model_name(clazz), "runtime_kind": "string", "enum": enum_values})
 
     for cls in all_classes:
         if attrs.has(cls):
             resolve_types(cls)  # make sure all string based types are resolved correctly
             export_data_class(cls)
         elif is_enum(cls):
-            export_enum(cls)  # type: ignore
+            export_enum(cls)
         else:
             raise AttributeError(f"Don't know how to handle: {cls}")
     return model
 
 
 # Use this model exporter, if a dynamic object is exported
 # with given name and properties.
@@ -292,34 +293,24 @@
                 for prop_name, prop_type in properties.items()
             ],
         }
     )
     return dependant
 
 
-def format_value_for_export(value: Any) -> Any:
-    if isinstance(value, (date, datetime)):
-        return utc_str(value)
-    elif isinstance(value, (timedelta, timezone)):
-        return duration_str(value)
-    elif isinstance(value, Enum):
-        return value.value
-    return value
-
-
-def get_node_attributes(node: BaseResource) -> Dict:
+def get_node_attributes(node: BaseResource) -> Json:
     if not hasattr(node, "to_json"):
         raise ValueError(f"Node {node} has no to_json() method!")
     result = node.to_json()
     result["kind"] = node.kind
     return result
 
 
 def node_to_dict(node: BaseResource, changes_only: bool = False, include_revision: bool = False) -> Json:
-    node_dict = {"id": node._resotocore_id if node._resotocore_id else node.chksum}
+    node_dict: Json = {"id": node._resotocore_id if node._resotocore_id else node.chksum}
     if changes_only:
         node_dict.update(node.changes.get())
     else:
         node_dict.update(
             {
                 "reported": get_node_attributes(node),
                 "metadata": {
@@ -345,15 +336,15 @@
             }
         )
     return node_dict
 
 
 @lru_cache(maxsize=None)
 def locate_python_type(python_type: str) -> Any:
-    cls = locate(python_type)
+    cls: Type[Any] = locate(python_type)  # type: ignore
     if attrs.has(cls):
         attrs.resolve_types(cls)
     return cls
 
 
 converter = cattrs.Converter()
 
@@ -379,18 +370,18 @@
 
 
 converter.register_structure_hook(datetime, lambda obj, typ: convert_datetime(obj))
 converter.register_structure_hook(date, lambda obj, typ: date.fromisoformat(obj))
 converter.register_structure_hook(timedelta, lambda obj, typ: str2timedelta(obj))
 converter.register_structure_hook(timezone, lambda obj, typ: str2timezone(obj))
 # work around until this is solved: https://github.com/python-attrs/cattrs/issues/278
-converter.register_structure_hook_func(is_primitive_or_primitive_union, lambda v, ty: v)
+converter.register_structure_hook_func(is_primitive_or_primitive_union, lambda v, ty: v)  # type: ignore
 
 
-def node_from_dict(node_data: Dict, include_select_ancestors: bool = False) -> BaseResource:
+def node_from_dict(node_data: Json, include_select_ancestors: bool = False) -> BaseResource:
     """Create a resource from resotocore graph node data
 
     If include_select_ancestors is True, the resource will be created with
     ancestors cloud, account, region and zone passed directly to the constructor.
     This is useful for when the node is being created for standalone use instead
     of in the context of a graph. E.g. during tagging of an individual resource
     where the tagger needs to know which cloud and account a resource came from.
@@ -432,22 +423,22 @@
         {
             "_resotocore_id": node_data.get("id"),
             "_resotocore_revision": node_data.get("revision"),
             "_resotocore_query_tag": node_data_metadata.get("query_tag"),
         }
     )
 
-    node = converter.structure_attrs_fromdict(new_node_data, node_type)
+    node: BaseResource = converter.structure_attrs_fromdict(new_node_data, node_type)
     for field_name, value in ancestors.items():
         setattr(node, field_name, value)
     node._raise_tags_exceptions = True
     node._protected = node_data_metadata.get("protected", False)
     node._cleaned = node_data_metadata.get("cleaned", False)
     node._clean = node_data_desired.get("clean", False)
     return node
 
 
-def cleanup_node_field_types(node_type: BaseResource, node_data_reported: Dict):
-    valid_fields = set(field.name for field in attrs.fields(node_type))
+def cleanup_node_field_types(node_type: BaseResource, node_data_reported: Json) -> None:
+    valid_fields = set(field.name for field in attrs.fields(node_type))  # type: ignore
     for field_name in list(node_data_reported.keys()):
         if field_name not in valid_fields:
             del node_data_reported[field_name]
```

### Comparing `resotolib-3.4.0/resotolib/core/progress.py` & `resotolib-3.4.1/resotolib/core/progress.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 "name": self.name,
                 **p,
                 "current": self.current,
                 "total": self.total,
             }
         elif isinstance(self, ProgressTree):
             node_iter = (part.data for part in self.sub_tree.all_nodes_itr() if part.data is not None)
-            nodes: List[Progress] = sorted(node_iter, key=key) if key else list(node_iter)  # type: ignore
+            nodes: List[Progress] = sorted(node_iter, key=key) if key else list(node_iter)
             return {"kind": "tree", "name": self.name, **p, "parts": [part.to_json() for part in nodes]}
         else:
             raise AttributeError("No handler to marshal progress")
 
     def info_json(self) -> JsonElement:
         if isinstance(self, ProgressDone):
             if self.total == self.current:
@@ -79,15 +79,15 @@
             else:
                 return f"{self.percentage}%"
         elif isinstance(self, ProgressTree):
             cloned = Tree(self.sub_tree.subtree(self.sub_tree.root), deep=True)
 
             def level_info(nd: Node) -> Json:
                 if dt := nd.data:
-                    return dt.info_json()
+                    return dt.info_json()  # type: ignore
                 else:
                     return {child.tag: level_info(child) for child in cloned.children(nd.identifier)}
 
             return {self.name: level_info(cloned.get_node(cloned.root))}
         else:
             raise AttributeError("No handler to marshal progress")
 
@@ -107,15 +107,15 @@
 
 
 @define
 class ProgressDone(Progress):
     current: int
     total: int
 
-    def __attrs_post_init__(self):
+    def __attrs_post_init__(self) -> None:
         if self.total <= 0:
             raise ValueError("total must be greater than 0")
         if self.current > self.total:
             raise ValueError(f"current ({self.current}) > total ({self.total})")
 
     def __str__(self) -> str:
         return f"{self.current}/{self.total}"
@@ -149,15 +149,15 @@
 
     def sub_progress(self, nid: str) -> Optional[Progress]:
         nid = nid if nid.startswith(_TreeRoot) else _TreeRoot + "." + nid
         node = self.sub_tree.get_node(nid)
         if node is None:
             return None
         elif node.data is not None:
-            return node.data
+            return node.data  # type: ignore
         else:
             return evolve(self, sub_tree=Tree(self.sub_tree.subtree(nid), deep=True))
 
     def has_path(self, nid: str) -> bool:
         nid = nid if nid.startswith(_TreeRoot) else _TreeRoot + "." + nid
         return nid in self.sub_tree
 
@@ -167,41 +167,41 @@
         return node.data if node and node.data else None
 
     def overall_progress(self) -> ProgressInfo:
         def sub_progress_info(nid: str) -> ProgressInfo:
             node = self.sub_tree.get_node(nid)
             # either the node is a data node or a tree node with children
             if node.data is not None:
-                return node.data.overall_progress()
+                return node.data.overall_progress()  # type: ignore
             else:
                 parts = [sub_progress_info(child.identifier) for child in self.sub_tree.children(nid)]
                 total_max = max(parts, key=lambda x: x.total).total if parts else 1
                 current = 0
                 total = 0
                 for info in parts:
                     current += int(info.current * total_max / max(1, info.total))
                     total += total_max
                 return ProgressInfo(current, total)
 
-        return sub_progress_info(self.sub_tree.root)
+        return sub_progress_info(self.sub_tree.root)  # type: ignore
 
     def mark_done(self) -> Progress:
         cloned = evolve(self, sub_tree=Tree(self.sub_tree.subtree(self.sub_tree.root), deep=True))
         for node in cloned.sub_tree.all_nodes():
             if node.data is not None:
                 node.data = node.data.mark_done()
         return cloned
 
     def update_progress(self, progress: Progress) -> Progress:
         cloned = evolve(self, sub_tree=Tree(self.sub_tree.subtree(self.sub_tree.root), deep=True))
         cloned.add_progress(progress)
         return cloned
 
     def add_progress(self, progress: Progress) -> None:
-        last = self.sub_tree.root
+        last: str = self.sub_tree.root  # type: ignore
         last_path = last
         path = last
         for part in progress.path:
             path += "." + part
             if path not in self.sub_tree:  # if the path does not exist, create it
                 self.sub_tree.create_node(part, path, parent=last_path)
             elif self.sub_tree[path].data is not None:  # if the path contains a value: remove it
```

### Comparing `resotolib-3.4.0/resotolib/core/search.py` & `resotolib-3.4.1/resotolib/core/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-import requests
 import json
+from typing import Optional, Iterator, Dict, Any
 from urllib.parse import urlencode
+
+import requests
+
+from resotolib.args import ArgumentParser
+from resotolib.baseresources import EdgeType
 from resotolib.config import Config
 from resotolib.core import resotocore
-from resotolib.graph import Graph, sanitize
-from resotolib.core.model_export import node_from_dict, node_to_dict
 from resotolib.core.ca import TLSData
-from resotolib.baseresources import EdgeType
-from resotolib.args import ArgumentParser
-from resotolib.logger import log
+from resotolib.core.model_export import node_from_dict, node_to_dict
+from resotolib.graph import Graph, sanitize
 from resotolib.jwt import encode_jwt_to_headers
-from typing import Optional
+from resotolib.logger import log
+from resotolib.types import Json
 
 
 class CoreGraph:
     def __init__(
         self,
-        base_uri: str = None,
-        graph: str = None,
+        base_uri: Optional[str] = None,
+        graph: Optional[str] = None,
         tls_data: Optional[TLSData] = None,
     ) -> None:
         if base_uri is None:
             self.base_uri = resotocore.http_uri
         else:
             self.base_uri = base_uri.strip("/")
         if graph is None:
@@ -30,52 +33,52 @@
             self.graph_name = graph
         self.verify = None
         if tls_data:
             self.verify = tls_data.ca_cert_path
         self.graph_uri = f"{self.base_uri}/graph/{self.graph_name}"
         self.search_uri = f"{self.graph_uri}/search/graph"
 
-    def execute(self, command: str):
+    def execute(self, command: str) -> Iterator[Json]:
         log.debug(f"Executing command: {command}")
         headers = {"Accept": "application/x-ndjson", "Content-Type": "text/plain"}
         execute_endpoint = f"{self.base_uri}/cli/execute"
         if self.graph_name:
             query_string = urlencode({"graph": self.graph_name})
             execute_endpoint += f"?{query_string}"
         return self.post(execute_endpoint, command, headers, verify=self.verify)
 
-    def search(self, search: str, edge_type: Optional[EdgeType] = None):
+    def search(self, search: str, edge_type: Optional[EdgeType] = None) -> Iterator[Json]:
         log.debug(f"Sending search {search}")
         headers = {"Accept": "application/x-ndjson"}
         search_endpoint = self.search_uri
         if edge_type is not None:
             query_string = urlencode({"edge_type": edge_type.value})
             search_endpoint += f"?{query_string}"
         return self.post(search_endpoint, search, headers, verify=self.verify)
 
     @staticmethod
-    def post(uri, data, headers, verify: Optional[str] = None):
+    def post(uri: str, data: str, headers: Dict[str, str], verify: Optional[str] = None) -> Iterator[Json]:
         if getattr(ArgumentParser.args, "psk", None):
             encode_jwt_to_headers(headers, {}, ArgumentParser.args.psk)
         r = requests.post(uri, data=data, headers=headers, stream=True, verify=verify)
         if r.status_code != 200:
             log.error(r.content.decode())
             raise RuntimeError(f"Failed to search graph: {r.content.decode()}")
         for line in r.iter_lines():
             if not line:
                 continue
             try:
-                data = json.loads(line.decode("utf-8"))
-                yield data
+                response: Json = json.loads(line.decode("utf-8"))
+                yield response
             except TypeError as e:
                 log.error(e)
                 continue
 
     def graph(self, search: str) -> Graph:
-        def process_data_line(data: dict, graph: Graph):
+        def process_data_line(data: Json, graph: Graph) -> None:
             """Process a single line of resotocore graph data"""
 
             if data.get("type") == "node":
                 node_id = data.get("id")
                 node = node_from_dict(data)
                 node_mapping[node_id] = node
                 log.debug(f"Adding node {node} to the graph")
@@ -88,25 +91,25 @@
                 node_to = data.get("to")
                 edge_type = EdgeType.from_value(data.get("edge_type"))
                 if node_from not in node_mapping or node_to not in node_mapping:
                     raise ValueError(f"One of {node_from} -> {node_to} unknown")
                 graph.add_edge(node_mapping[node_from], node_mapping[node_to], edge_type=edge_type)
 
         graph = Graph()
-        node_mapping = {}
+        node_mapping: Dict[Any, Any] = {}
         for data in self.search(search):
             try:
                 process_data_line(data, graph)
             except ValueError as e:
                 log.error(e)
                 continue
         sanitize(graph)
         return graph
 
-    def patch_nodes(self, graph: Graph):
+    def patch_nodes(self, graph: Graph) -> None:
         headers = {"Content-Type": "application/x-ndjson"}
         if getattr(ArgumentParser.args, "psk", None):
             encode_jwt_to_headers(headers, {}, ArgumentParser.args.psk)
 
         r = requests.patch(
             f"{self.graph_uri}/nodes",
             data=GraphChangeIterator(graph),
@@ -116,18 +119,18 @@
         if r.status_code != 200:
             err = r.content.decode("utf-8")
             log.error(err)
             raise RuntimeError(f"Failed to patch nodes: {err}")
 
 
 class GraphChangeIterator:
-    def __init__(self, graph: Graph):
+    def __init__(self, graph: Graph) -> None:
         self.graph = graph
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[bytes]:
         for node in self.graph.nodes:
             if not node.changes.changed:
                 continue
             node_dict = node_to_dict(node, changes_only=True)
             node_json = json.dumps(node_dict) + "\n"
             log.debug(f"Updating node {node_dict}")
             yield node_json.encode()
```

### Comparing `resotolib-3.4.0/resotolib/core/tasks.py` & `resotolib-3.4.1/resotolib/core/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             result = self.handler(task_data)
             return CoreTaskResult(task_id=task_id, data=result)
         except Exception as e:
             log.debug(f"Error while executing task {self.name}: {e}", exc_info=True)
             return CoreTaskResult(task_id=task_id, error=str(e))
 
     def matches(self, js: Json) -> bool:
-        attrs: Json = js.get("attrs")
+        attrs: Json = js.get("attrs", {})
         if js.get("task_name") != self.name or not isinstance(attrs, dict):
             return False
         return all((attrs.get(n) in f) for n, f in self.filter.items())
 
     def core_json(self) -> Json:
         return {
             "name": self.name,
@@ -73,26 +73,26 @@
         }
 
     @staticmethod
     def from_definition(target: Any, wtd: CommandDefinition) -> CoreTaskHandler:
         def handle_message(message: Json) -> JsonElement:
             node_data = message.get("node", {})
             args = message.get("args", [])
-            return wtd.fn(target, current_config(), node_data, args)
+            return wtd.fn(target, current_config(), node_data, args)  # type: ignore
 
         def handle_resource(message: Json) -> JsonElement:
             node_data = message.get("node", {})
             node = node_from_dict(node_data, include_select_ancestors=True) if node_data else None
             args = message.get("args", [])
             result = wtd.fn(target, current_config(), node, args)
             # expect either a base resource or json element as result
             if isinstance(result, BaseResource):
                 return node_to_dict(result)
             else:
-                return result
+                return result  # type: ignore
 
         to_call = handle_resource if wtd.expect_resource else handle_message
         return CoreTaskHandler(
             name=wtd.name,
             info=wtd.info,
             args_description=wtd.args_description,
             description=wtd.description,
@@ -114,19 +114,19 @@
     ) -> None:
         super().__init__()
         self.identifier = identifier
         self.resotocore_ws_uri = resotocore_ws_uri
         self.task_handler = task_handler
         self.max_workers = max_workers
         self.tls_data = tls_data
-        self.ws = None
+        self.ws: Optional[websocket.WebSocketApp] = None
         self.shutdown_event = threading.Event()
         self.queue: queue.Queue[Json] = queue.Queue()
 
-    def __del__(self):
+    def __del__(self) -> None:
         remove_event_listener(EventType.SHUTDOWN, self.shutdown)
 
     def run(self) -> None:
         self.name = self.identifier
         add_event_listener(EventType.SHUTDOWN, self.shutdown)
 
         for i in range(self.max_workers):
@@ -144,32 +144,33 @@
         while not self.shutdown_event.is_set():
             message = self.queue.get()
             log.debug(f"{self.identifier} received: {message}")
             for handler in self.task_handler:
                 if handler.matches(message):
                     try:
                         result = handler.execute(message)
-                        log.debug(f"Sending reply {result.to_json()}")
-                        self.ws.send(json.dumps(result.to_json()))
+                        if self.ws:
+                            log.debug(f"Sending reply {result.to_json()}")
+                            self.ws.send(json.dumps(result.to_json()))
                     except Exception as ex:
                         log.exception(f"Something went wrong while processing {message}")
-                        if task_id := message.get("task_id"):
+                        if task_id := message.get("task_id") and self.ws:
                             self.ws.send(jsons.dumps(CoreTaskResult(task_id, error=str(ex)).to_json()))
                     break
             self.queue.task_done()
 
     def connect(self) -> None:
         resotocore_ws_uri_split = urlsplit(self.resotocore_ws_uri)
         scheme = resotocore_ws_uri_split.scheme
         netloc = resotocore_ws_uri_split.netloc
         path = resotocore_ws_uri_split.path + "/work/queue"
         ws_uri = urlunsplit((scheme, netloc, path, "", ""))
 
         log.debug(f"{self.identifier} connecting to {ws_uri}")
-        headers = {}
+        headers: Dict[str, str] = {}
         if getattr(ArgumentParser.args, "psk", None):
             encode_jwt_to_headers(headers, {}, ArgumentParser.args.psk)
         self.ws = websocket.WebSocketApp(
             ws_uri,
             header=headers,
             on_open=self.on_open,
             on_message=self.on_message,
@@ -179,38 +180,38 @@
             on_pong=self.on_pong,
         )
         sslopt = None
         if self.tls_data:
             sslopt = {"ca_certs": self.tls_data.ca_cert_path}
         self.ws.run_forever(sslopt=sslopt, ping_interval=20, ping_timeout=10, ping_payload="ping")
 
-    def shutdown(self, event: Event = None) -> None:
+    def shutdown(self, event: Optional[Event] = None) -> None:
         log.debug("Received shutdown event - shutting down resotocore task queue listener")
         self.shutdown_event.set()
         if self.ws:
             self.ws.close()
 
-    def on_message(self, ws, message):
+    def on_message(self, _: websocket.WebSocketApp, message: str) -> None:
         try:
-            message: Json = json.loads(message)
+            jsom_message: Json = json.loads(message)
         except json.JSONDecodeError:
             log.exception(f"Unable to decode received message {message}")
             return
-        self.queue.put(message)
+        self.queue.put(jsom_message)
 
-    def on_error(self, ws, e):
+    def on_error(self, _: websocket.WebSocketApp, e: Exception) -> None:
         log.debug(f"{self.identifier} event bus error: {e!r}")
 
-    def on_close(self, ws, close_status_code, close_msg):
+    def on_close(self, _: websocket.WebSocketApp, close_status_code: int, close_msg: str) -> None:
         log.debug(f"{self.identifier} disconnected from resotocore task queue")
 
-    def on_open(self, ws):
+    def on_open(self, ws: websocket.WebSocketApp) -> None:
         log.debug(f"{self.identifier} connected to resotocore, register at task queue")
         # when we are connected, we register at the task queue
         # by sending all task handler definitions
         ws.send(json.dumps([handler.core_json() for handler in self.task_handler]))
 
-    def on_ping(self, ws, message):
+    def on_ping(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug(f"{self.identifier} tasks ping from resotocore message bus")
 
-    def on_pong(self, ws, message):
+    def on_pong(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug(f"{self.identifier} tasks pong from resotocore message bus")
```

### Comparing `resotolib-3.4.0/resotolib/durations.py` & `resotolib-3.4.1/resotolib/durations.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/event.py` & `resotolib-3.4.1/resotolib/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import time
-from resotolib.logger import log
-from resotolib.lock import RWLock
 from collections import defaultdict
-from threading import Thread, Lock
-from typing import Callable, Iterable
 from enum import Enum
+from threading import Thread, Lock
+from typing import Callable, Iterable, Any, Dict
+
+from resotolib.lock import RWLock
+from resotolib.logger import log
+from resotolib.types import Json
 
 
 class EventType(Enum):
     """Defines Event Types
 
     Event().data definitions for EventType:
     STARTUP: None
@@ -37,24 +39,24 @@
     PROCESS_FINISH = "process_finish"
     GENERATE_METRICS = "generate_metrics"
 
 
 class Event:
     """An Event"""
 
-    def __init__(self, event_type: EventType, data=None) -> None:
+    def __init__(self, event_type: EventType, data: Json) -> None:
         self.event_type = event_type
         self.data = data
 
 
-_events = defaultdict(dict)
+_events: Dict[EventType, Dict[Callable[[Event], None], Any]] = defaultdict(dict)
 _events_lock = RWLock()
 
 
-def event_listener_registered(event_type: EventType, listener: Callable) -> bool:
+def event_listener_registered(event_type: EventType, listener: Callable[[Event], None]) -> bool:
     """Return whether listener is registered to event"""
     if _events is None:
         return False
     return event_type in _events.keys() and listener in _events[event_type].keys()
 
 
 def dispatch_event(event: Event, blocking: bool = False) -> None:
@@ -107,15 +109,15 @@
         log.debug(f"Waiting up to {timeout:.2f}s for event listener {thread.name} to finish")
         thread.join(timeout)
         log.debug(f"Event listener {thread.name} finished (timeout: {thread.is_alive()})")
 
 
 def add_event_listener(
     event_type: EventType,
-    listener: Callable,
+    listener: Callable[[Event], None],
     blocking: bool = False,
     timeout: int = 900,
     one_shot: bool = False,
 ) -> bool:
     """Add an Event Listener"""
     if not callable(listener):
         log.error(f"Error registering {listener} of type {type(listener)} with event" f" {event_type.name}")
@@ -131,27 +133,27 @@
                 "lock": Lock(),
                 "pid": os.getpid(),
             }
             return True
         return False
 
 
-def remove_event_listener(event_type: EventType, listener: Callable) -> bool:
+def remove_event_listener(event_type: EventType, listener: Callable[[Event], None]) -> bool:
     """Remove an Event Listener"""
     with _events_lock.write_access:
         if event_listener_registered(event_type, listener):
             log.debug(f"Removing {listener} from event {event_type.name}")
             del _events[event_type][listener]
             if len(_events[event_type]) == 0:
                 del _events[event_type]
             return True
         return False
 
 
-def list_event_listeners() -> Iterable:
+def list_event_listeners() -> Iterable[str]:
     with _events_lock.read_access:
         for event_type, listeners in _events.items():
             for listener, listener_data in listeners.items():
                 yield (
                     f"{event_type.name}: {listener}, "
                     f"blocking: {listener_data['blocking']}, "
                     f"one-shot: {listener_data['one-shot']}"
```

### Comparing `resotolib-3.4.0/resotolib/graph/__init__.py` & `resotolib-3.4.1/resotolib/graph/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tempfile
 import threading
 from collections import defaultdict, namedtuple, deque
 from datetime import datetime
 from enum import Enum
 from functools import lru_cache
 from time import time
-from typing import Dict, Iterator, List, Tuple, Optional, Union, Any, Type
+from typing import Dict, Iterator, List, Tuple, Optional, Union, Any, Type, TypeVar
 
 import jsons
 import networkx
 from attr import resolve_types
 from attrs import define, fields
 from networkx.algorithms.dag import is_directed_acyclic_graph
 from prometheus_client import Summary
@@ -31,14 +31,16 @@
     dataclasses_to_resotocore_model,
     node_to_dict,
 )
 from resotolib.logger import log
 from resotolib.types import Json
 from resotolib.utils import get_resource_attributes, unset_cached_properties, utc_str
 
+T = TypeVar("T")
+
 
 @define
 class BySearchCriteria:
     query: str
 
 
 @define
@@ -78,35 +80,35 @@
 metrics_graph2pickle = Summary("resoto_graph2pickle_seconds", "Time it took the graph2pickle() method")
 metrics_graph2gexf = Summary("resoto_graph2gexf_seconds", "Time it took the graph2gexf() method")
 metrics_graph2pajek = Summary("resoto_graph2pajek_seconds", "Time it took the graph2pajek() method")
 
 EdgeKey = namedtuple("EdgeKey", ["src", "dst", "edge_type"])
 
 
-class Graph(networkx.MultiDiGraph):
+class Graph(networkx.MultiDiGraph):  # type: ignore
     """A directed Graph"""
 
-    def __init__(self, *args, root: BaseResource = None, **kwargs) -> None:
+    def __init__(self, *args: Any, root: Optional[BaseResource] = None, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.root = None
         self._log_edge_creation = True
         if isinstance(root, BaseResource):
             self.root = root
             self.add_node(self.root, label=self.root.name, **get_resource_attributes(self.root))
         self.deferred_edges: List[Tuple[NodeSelector, NodeSelector, EdgeType]] = []
 
-    def merge(self, graph: Graph, skip_deferred_edges: bool = False):
+    def merge(self, graph: Graph, skip_deferred_edges: bool = False) -> None:
         """Merge another graph into ourselves
 
         If the other graph has a graph.root an edge will be created between
         it and our own graph root.
         """
         if isinstance(self.root, BaseResource) and isinstance(getattr(graph, "root", None), BaseResource):
-            log.debug(f"Merging graph of {graph.root.rtdname} into graph of {self.root.rtdname}")
-            self.add_edge(self.root, graph.root)
+            log.debug(f"Merging graph of {graph.root.rtdname} into graph of {self.root.rtdname}")  # type: ignore
+            self.add_edge(self.root, graph.root)  # type: ignore
         else:
             log.warning("Merging graphs with no valid roots")
 
         try:
             self._log_edge_creation = False
             self.update(edges=graph.edges, nodes=graph.nodes)
             self.deferred_edges.extend(graph.deferred_edges)
@@ -115,17 +117,17 @@
         if not skip_deferred_edges:
             self.resolve_deferred_connections()
 
     def add_resource(
         self,
         parent: BaseResource,
         node_for_adding: BaseResource,
-        edge_type: EdgeType = None,
-        **attr,
-    ):
+        edge_type: Optional[EdgeType] = None,
+        **attr: Any,
+    ) -> None:
         """Add a resource node to the graph
 
         When adding resource nodes to the graph there's always a label and a
         kind as well as an edge connecting the new resource with its parent
         resource. This way we should never have disconnected nodes within the graph.
 
         The graph_attributes are a Dict of key=value pairs that contain all the
@@ -140,48 +142,48 @@
         attributes.
         """
         resource_attr = get_resource_attributes(node_for_adding)
 
         self.add_node(node_for_adding, label=node_for_adding.name, **resource_attr, **attr)
         self.add_edge(src=parent, dst=node_for_adding, edge_type=edge_type)
 
-    def add_node(self, node_for_adding: BaseResource, **attr):
+    def add_node(self, node_for_adding: BaseResource, **attr: Any) -> None:
         super().add_node(node_for_adding, **attr)
         if isinstance(node_for_adding, BaseResource):
             # We hand a reference to ourselves to the added BaseResource
             # which stores it as a weakref.
             node_for_adding._graph = self
 
     def has_edge(
-        self, src: BaseResource, dst: BaseResource, key: Optional[EdgeKey] = None, edge_type: Optional[str] = None
+        self, src: BaseResource, dst: BaseResource, key: Optional[EdgeKey] = None, edge_type: Optional[EdgeType] = None
     ) -> bool:
         edge_type = edge_type or EdgeType.default
         key = key or EdgeKey(src=src, dst=dst, edge_type=edge_type)
-        return super().has_edge(src, dst, key=key)
+        return super().has_edge(src, dst, key=key)  # type: ignore
 
     def add_edge(
         self,
         src: BaseResource,
         dst: BaseResource,
-        key: EdgeKey = None,
-        edge_type: EdgeType = None,
-        **attr,
-    ):
+        key: Optional[EdgeKey] = None,
+        edge_type: Optional[EdgeType] = None,
+        **attr: Any,
+    ) -> Optional[EdgeKey]:
         if src is None or dst is None:
             log.error(f"Not creating edge from or to NoneType: {src} to {dst}")
-            return
+            return None
 
         if edge_type is None:
             edge_type = EdgeType.default
         if key is None:
             key = EdgeKey(src=src, dst=dst, edge_type=edge_type)
 
         if self.has_edge(src, dst, key=key):
             log.debug(f"Edge from {src} to {dst} already exists in graph")
-            return
+            return None
         return_key = super().add_edge(src, dst, key=key, **attr)
         if self._log_edge_creation and isinstance(src, BaseResource) and isinstance(dst, BaseResource):
             log.debug(f"Added edge from {src.rtdname} to {dst.rtdname} (type: {edge_type.value})")
             try:
                 src.successor_added(dst, self)
             except Exception:
                 log.exception(
@@ -192,58 +194,58 @@
             except Exception:
                 log.exception(
                     (
                         f"Unhandled exception while telling {dst.rtdname}"
                         f" that {src.rtdname} was added as a predecessor"
                     )
                 )
-        return return_key
+        return return_key  # type: ignore
 
     def add_deferred_edge(self, src: NodeSelector, dst: NodeSelector, edge_type: EdgeType = EdgeType.default) -> None:
         self.deferred_edges.append((src, dst, edge_type))
 
-    def remove_node(self, node: BaseResource):
+    def remove_node(self, node: BaseResource) -> None:
         super().remove_node(node)
 
     def remove_edge(
         self,
         src: BaseResource,
         dst: BaseResource,
-        key: EdgeKey = None,
-        edge_type: EdgeType = None,
-    ):
+        key: Optional[EdgeKey] = None,
+        edge_type: Optional[EdgeType] = None,
+    ) -> None:
         if edge_type is None:
             edge_type = EdgeType.default
         if key is None:
             key = EdgeKey(src=src, dst=dst, edge_type=edge_type)
         super().remove_edge(src, dst, key=key)
 
-    def predecessors(self, node: BaseResource, edge_type: EdgeType = None):
+    def predecessors(self, node: BaseResource, edge_type: Optional[EdgeType] = None) -> Iterator[BaseResource]:
         if edge_type is None:
             edge_type = EdgeType.default
         for predecessor in super().predecessors(node):
-            key = (predecessor, node, edge_type)
+            key = EdgeKey(predecessor, node, edge_type)
             if self.has_edge(predecessor, node, key=key):
                 yield predecessor
 
-    def successors(self, node: BaseResource, edge_type: EdgeType = None):
+    def successors(self, node: BaseResource, edge_type: Optional[EdgeType] = None) -> Iterator[BaseResource]:
         if edge_type is None:
             edge_type = EdgeType.default
         for successor in super().successors(node):
-            key = (node, successor, edge_type)
+            key = EdgeKey(node, successor, edge_type)
             if self.has_edge(node, successor, key=key):
                 yield successor
 
-    def ancestors(self, node: BaseResource, edge_type: EdgeType = None):
-        return networkx.algorithms.dag.ancestors(self.edge_type_subgraph(edge_type), node)
+    def ancestors(self, node: BaseResource, edge_type: Optional[EdgeType] = None) -> Iterator[BaseResource]:
+        return networkx.algorithms.dag.ancestors(self.edge_type_subgraph(edge_type), node)  # type: ignore
 
-    def descendants(self, node: BaseResource, edge_type: EdgeType = None):
-        return networkx.algorithms.dag.descendants(self.edge_type_subgraph(edge_type), node)
+    def descendants(self, node: BaseResource, edge_type: Optional[EdgeType] = None) -> Iterator[BaseResource]:
+        return networkx.algorithms.dag.descendants(self.edge_type_subgraph(edge_type), node)  # type: ignore
 
-    def edge_type_subgraph(self, edge_type: EdgeType = None):
+    def edge_type_subgraph(self, edge_type: Optional[EdgeType] = None) -> networkx.Graph:
         if edge_type is None:
             edge_type = EdgeType.default
         edges = []
         for edge in self.edges(keys=True):
             if len(edge) == 3:
                 key: EdgeKey = edge[2]
                 if key.edge_type == edge_type:
@@ -271,16 +273,16 @@
                 edges_per_type[key.edge_type].append(edge)
         for edges in edges_per_type.values():
             typed_graph = self.edge_subgraph(edges)
             if not is_directed_acyclic_graph(typed_graph):
                 return [edge[2] for edge in networkx.algorithms.cycles.find_cycle(typed_graph)]
         return None
 
-    @metrics_graph_search.time()
-    def search(self, attr, value, regex_search=False):
+    @metrics_graph_search.time()  # type: ignore
+    def search(self, attr: str, value: Any, regex_search: bool = False) -> Iterator[BaseResource]:
         """Search for graph nodes by their attribute value"""
         if value is None:
             log.debug(f"Not searching graph for nodes with attribute values {attr}: {value}")
             return ()
         log.debug((f"Searching graph for nodes with attribute values {attr}: {value}" f" (regex: {regex_search})"))
         for node in self.nodes():
             node_attr = getattr(node, attr, None)
@@ -290,49 +292,49 @@
                 and (
                     (regex_search is False and node_attr == value)
                     or (regex_search is True and re.search(value, str(node_attr)))
                 )
             ):
                 yield node
 
-    @metrics_graph_searchre.time()
-    def searchre(self, attr, regex):
+    @metrics_graph_searchre.time()  # type: ignore
+    def searchre(self, attr: str, regex: str) -> Iterator[BaseResource]:
         """Regex search for graph nodes by their attribute value"""
         log.debug(f"Regex searching graph for nodes with attribute values {attr}: {regex}")
-        return self.search(attr, regex, regex_search=True)
+        yield from self.search(attr, regex, regex_search=True)
 
-    @metrics_graph_searchall.time()
-    def searchall(self, match: Dict):
+    @metrics_graph_searchall.time()  # type: ignore
+    def searchall(self, match: Dict[str, Any]) -> Iterator[BaseResource]:
         """Search for graph nodes by multiple attributes and values"""
-        return (
-            node for node in self.nodes() if all(getattr(node, attr, None) == value for attr, value in match.items())
-        )
+        for node in self.nodes():
+            if all(getattr(node, attr, None) == value for attr, value in match.items()):
+                yield node
 
-    @metrics_graph_search_first.time()
-    def search_first(self, attr, value):
+    @metrics_graph_search_first.time()  # type: ignore
+    def search_first(self, attr: str, value: Any) -> Optional[BaseResource]:
         """Return the first graph node that matches a certain attribute value"""
         node = next(iter(self.search(attr, value)), None)
         if node:
             log.debug(f"Found node {node} with {attr}: {value}")
         else:
             log.debug(f"Found no node with {attr}: {value}")
-        return node
+        return node  # type: ignore
 
-    @metrics_graph_search_first_all.time()
-    def search_first_all(self, match: Dict):
+    @metrics_graph_search_first_all.time()  # type: ignore
+    def search_first_all(self, match: Dict[str, Any]) -> Optional[BaseResource]:
         """Return the first graph node that matches multiple attributes and values"""
         node = next(iter(self.searchall(match)), None)
         if node:
             log.debug(f"Found node {node} with {match}")
         else:
             log.debug(f"Found no node with {match}")
-        return node
+        return node  # type: ignore
 
-    @metrics_graph_search_first_parent_class.time()
-    def search_first_parent_class(self, node, cls):
+    @metrics_graph_search_first_parent_class.time()  # type: ignore
+    def search_first_parent_class(self, node: BaseResource, cls: Type[T]) -> Optional[T]:
         """Return the first parent node matching a certain class
 
         This is being used to search up the graph and e.g. find the account that the
         graph node is a member of.
         """
         queue = deque(self.predecessors(node))
         already_checked = set(self.predecessors(node))
@@ -342,16 +344,16 @@
                 return current
             for n in self.predecessors(current):
                 if n not in already_checked:
                     already_checked.add(n)
                     queue.append(n)
         return None
 
-    @metrics_graph_resolve_deferred_connections.time()
-    def resolve_deferred_connections(self):
+    @metrics_graph_resolve_deferred_connections.time()  # type: ignore
+    def resolve_deferred_connections(self) -> None:
         log.debug("Resolving deferred graph connections")
         for node in self.nodes:
             if isinstance(node, BaseResource):
                 node.resolve_deferred_connections(self)
 
     def export_model(self, **kwargs: Any) -> List[Json]:
         """Return the graph node dataclass model in resotocore format"""
@@ -378,15 +380,15 @@
 
 
 @lru_cache(maxsize=4096)  # Only resolve types once per type
 def resolve_type(clazz: Type[Any]) -> None:
     resolve_types(clazz)
 
 
-def validate_dataclass(node: BaseResource):
+def validate_dataclass(node: BaseResource) -> None:
     resolve_type(type(node))  # make sure all type annotations are resolved
     for field in fields(type(node)):
         value = getattr(node, field.name)
         try:
             check_type(value, field.type)
         except TypeError:
             log.exception(
@@ -418,19 +420,21 @@
 
 def update_graph_ref(graph: Graph) -> None:
     for node in graph.nodes:
         if isinstance(node, BaseResource):
             node._graph = graph
 
 
-def sanitize(graph: Graph, root: GraphRoot = None) -> None:
+def sanitize(graph: Graph, maybe_root: Optional[GraphRoot] = None) -> None:
     log.debug("Sanitizing Graph")
     plugin_roots = {}
     graph_roots = []
 
+    root: Optional[BaseResource] = maybe_root
+
     if root is None and isinstance(getattr(graph, "root", None), BaseResource):
         root = graph.root
 
     if root is None:
         log.debug("No graph root found - unable to sanitize")
         return
 
@@ -502,30 +506,30 @@
             log.info(f"Writing graph json to file {self.tempfile.name}")
 
         if not isinstance(graph_merge_kind, GraphMergeKind):
             log.error(f"Graph merge kind is wrong type {type(graph_merge_kind)}")
             graph_merge_kind = GraphMergeKind.cloud
 
         if graph_merge_kind == GraphMergeKind.cloud:
-            self.graph_merge_kind = BaseCloud
+            self.graph_merge_kind: Type[Any] = BaseCloud
         elif graph_merge_kind == GraphMergeKind.account:
             self.graph_merge_kind = BaseAccount
         else:
             log.error(f"Graph merge kind has unknown value {graph_merge_kind} - defaulting to 'cloud'")
             self.graph_merge_kind = BaseCloud
 
         self.graph_exported = False
         self.found_replace_node = False
         self.export_lock = threading.Lock()
         self.total_lines = 0
         self.number_of_nodes = int(graph.number_of_nodes())
         self.number_of_edges = int(graph.number_of_edges())
         self.number_of_deferred_edges = len(graph.deferred_edges)
 
-    def __del__(self):
+    def __del__(self) -> None:
         try:
             self.tempfile.close()
         except Exception:
             pass
 
     def __iter__(self) -> Iterator[bytes]:
         if not self.graph_exported:
```

### Comparing `resotolib-3.4.0/resotolib/graph/graph_extensions.py` & `resotolib-3.4.1/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/json.py` & `resotolib-3.4.1/resotolib/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 del unstructured[strip_attr]
         elif isinstance(strip_attr, (list, tuple)):
             for field in strip_attr:
                 if unstructured.get(field):
                     del unstructured[field]
         else:
             raise ValueError(f"Don't know how to handle type of strip_attr: {strip_attr}")
-    result: Json = jsons.dump(  # type: ignore
+    result: Json = jsons.dump(
         unstructured,
         strip_microseconds=True,
         strip_nulls=True,
         # class variables have to stripped manually via strip_attr=
         # see: https://github.com/ramonhagenaars/jsons/issues/177
         # strip_class_variables=True,
         **kwargs,
@@ -53,15 +53,15 @@
     return result
 
 
 def to_json_str(node: Any, json_kwargs: Optional[Dict[str, object]] = None, **kwargs: Any) -> str:
     """
     Json string representation of the given object.
     """
-    return json.dumps(to_json(node, **kwargs), **(json_kwargs or {}))
+    return json.dumps(to_json(node, **kwargs), **(json_kwargs or {}))  # type: ignore
 
 
 def from_json(json: JsonElement, clazz: Type[AnyT], **kwargs: Any) -> AnyT:
     """
     Loads a json object into a python object.
     :param json: the json object to load.
     :param clazz: the type of the python object.
```

### Comparing `resotolib-3.4.0/resotolib/json_bender.py` & `resotolib-3.4.1/resotolib/json_bender.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     Example:
     ```
     f = F(sorted, key=lambda d: d['id'])
     K([{'id': 3}, {'id': 1}]) >> f  #  -> [{'id': 1}, {'id': 3}]
     ```
     """
 
-    def __init__(self, func: Callable[[Any], Any], *args: Any, **kwargs: Any):  # type: ignore
+    def __init__(self, func: Callable[[Any], Any], *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self._func = func
         self._args = args
         self._kwargs = kwargs
 
     def execute(self, value: Any) -> Any:
         # noinspection PyArgumentList
@@ -325,15 +325,15 @@
 
     def __init__(self, extractor: Bender, **kwargs: Any):
         super().__init__(**kwargs)
         self._extractor = extractor
 
     def execute(self, source: Any) -> Any:
         if isinstance(source, list):
-            return sorted(source, key=lambda x: bend(self._extractor, x))
+            return sorted(source, key=lambda x: bend(self._extractor, x))  # type: ignore
         else:
             return source
 
 
 class AsInt(Bender):
     def execute(self, source: Any) -> Any:
         if isinstance(source, int):
```

### Comparing `resotolib-3.4.0/resotolib/jwt.py` & `resotolib-3.4.1/resotolib/jwt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 import jwt
 import base64
 import hashlib
 import time
 from resotolib.args import ArgumentParser
-from typing import Any, Optional, Tuple, Dict
+from typing import Any, Optional, Tuple, Dict, Mapping
 
+from resotolib.types import Json
 
-def key_from_psk(psk: str, salt: bytes = None) -> Tuple[bytes, bytes]:
+
+def key_from_psk(psk: str, salt: Optional[bytes] = None) -> Tuple[bytes, bytes]:
     """Derive a 256 bit key from a passphrase/pre-shared-key.
     A salt can be optionally provided. If not one will be generated.
     Returns both the key and the salt.
     """
     if salt is None:
         salt = os.urandom(16)
     key = hashlib.pbkdf2_hmac("sha256", psk.encode(), salt, 100000)
@@ -31,25 +33,25 @@
     if headers is None:
         headers = {}
     if expire_in > 0 and "exp" not in payload:
         payload.update({"exp": int(time.time()) + expire_in})
     key, salt = key_from_psk(psk)
     salt_encoded = base64.standard_b64encode(salt).decode("utf-8")
     headers.update({"salt": salt_encoded})
-    return jwt.encode(payload, key, algorithm="HS256", headers=headers)
+    return jwt.encode(payload, key, algorithm="HS256", headers=headers)  # type: ignore
 
 
-def decode_jwt(encoded_jwt: str, psk: str, options: Optional[Dict[str, Any]] = None) -> dict:
+def decode_jwt(encoded_jwt: str, psk: str, options: Optional[Dict[str, Any]] = None) -> Json:
     """Decode a JWT using a key derived from a pre-shared-key and a salt stored
     in the JWT headers.
     """
     salt_encoded = jwt.get_unverified_header(encoded_jwt).get("salt")
-    salt = base64.standard_b64decode(salt_encoded)
+    salt = base64.standard_b64decode(salt_encoded) if salt_encoded else None
     key, _ = key_from_psk(psk, salt)
-    return jwt.decode(encoded_jwt, key, algorithms=["HS256"], options=options)
+    return jwt.decode(encoded_jwt, key, algorithms=["HS256"], options=options)  # type: ignore
 
 
 def encode_jwt_to_headers(
     http_headers: Dict[str, str],
     payload: Dict[str, Any],
     psk: str,
     scheme: str = "Bearer",
@@ -60,15 +62,15 @@
     dictionary. Also returns that dict.
     """
     http_headers.update({"Authorization": f"{scheme} {encode_jwt(payload, psk, headers, expire_in)}"})
     return http_headers
 
 
 def decode_jwt_from_headers(
-    http_headers: Dict[str, str],
+    http_headers: Mapping[str, str],
     psk: str,
     scheme: str = "Bearer",
     options: Optional[Dict[str, Any]] = None,
 ) -> Optional[Dict[str, str]]:
     """Retrieves the Authorization header from a http headers dictionary and
     passes it to `decode_jwt_from_header_value()` to return the decoded payload.
     """
```

### Comparing `resotolib-3.4.0/resotolib/lock.py` & `resotolib-3.4.1/resotolib/lock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import threading
+from typing import Any
 
 
 class RWLock:
     """Synchronization object used in a solution of so-called second
     readers-writers problem. In this problem, many readers can simultaneously
     access a share, and a writer has an exclusive access to this share.
     Additionally, the following constraints should be met:
@@ -40,28 +41,28 @@
             def __init__(self, rwlock: RWLock) -> None:
                 self.rwlock = rwlock
 
             def __enter__(self) -> RWLock:
                 self.rwlock.reader_acquire()
                 return self.rwlock
 
-            def __exit__(self, typ, value, tb) -> None:
+            def __exit__(self, typ: Any, value: Any, tb: Any) -> None:
                 self.rwlock.reader_release()
 
         self.read_access = _ReadAccess(self)
 
         class _WriteAccess:
             def __init__(self, rwlock: RWLock) -> None:
                 self.rwlock = rwlock
 
             def __enter__(self) -> RWLock:
                 self.rwlock.writer_acquire()
                 return self.rwlock
 
-            def __exit__(self, typ, value, tb) -> None:
+            def __exit__(self, typ: Any, value: Any, tb: Any) -> None:
                 self.rwlock.writer_release()
 
         self.write_access = _WriteAccess(self)
 
     def reader_acquire(self) -> None:
         self.__readers_queue.acquire()
         self.__no_readers.acquire()
@@ -85,20 +86,20 @@
     """An auxiliary "light switch"-like object. The first thread turns on the
     "switch", the last one turns it off (see [1, sec. 4.2.2] for details)."""
 
     def __init__(self) -> None:
         self.__counter = 0
         self.__mutex = threading.Lock()
 
-    def acquire(self, lock) -> None:
+    def acquire(self, lock: threading.Lock) -> None:
         self.__mutex.acquire()
         self.__counter += 1
         if self.__counter == 1:
             lock.acquire()
         self.__mutex.release()
 
-    def release(self, lock) -> None:
+    def release(self, lock: threading.Lock) -> None:
         self.__mutex.acquire()
         self.__counter -= 1
         if self.__counter == 0:
             lock.release()
         self.__mutex.release()
```

### Comparing `resotolib-3.4.0/resotolib/log/logstream.py` & `resotolib-3.4.1/resotolib/log/logstream.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from abc import ABC
 from asyncio import Task, Future
 from collections import deque
 from datetime import timedelta
 from logging import StreamHandler, LogRecord
 from ssl import SSLContext
-from typing import Optional, TypeVar, Mapping, Union
+from typing import Optional, TypeVar, Mapping, Union, Any
 
 import jsons
 from aiohttp import ClientSession, ClientWebSocketResponse, Fingerprint
 from aiohttp.typedefs import LooseHeaders
 
 from resotolib.asynchronous.periodic import Periodic
 from resotolib.log import Event, Severity
@@ -29,43 +29,44 @@
         params: Optional[Mapping[str, str]] = None,
         headers: Optional[LooseHeaders] = None,
         ssl: Union[SSLContext, bool, None, Fingerprint] = None,
     ) -> None:
         self.url = url
         self.connection_args = dict(params=params, headers=headers, ssl=ssl)
         self.buffer: deque[str] = deque(maxlen=max_outstanding)
-        self.queue = asyncio.Queue()
+        self.queue: asyncio.Queue[str] = asyncio.Queue()
         self.periodic = Periodic("flush log messages", self.__shuffle_messages, frequency)
-        self.task: Optional[Task] = None
+        self.task: Optional[Task[Any]] = None
 
     async def start(self) -> None:
         log.info("Start log streamer")
         await self.periodic.start()
         self.task = asyncio.create_task(self.__send_log_messages())
 
     async def stop(self) -> None:
         log.info("Stopping log streamer")
         await self.periodic.stop()
-        self.task.cancel()
-        await self.task
+        if self.task:
+            self.task.cancel()
+            await self.task
 
-    def send_event(self, event: Event):
+    def send_event(self, event: Event) -> None:
         self.buffer.append(jsons.dumps(event))
 
     async def __shuffle_messages(self) -> None:
         while self.buffer:
             msg = self.buffer.popleft()
             await self.queue.put(msg)
 
     async def __send_log_messages(self) -> None:
         async with ClientSession() as session:
             while True:
                 try:
                     log.debug("Try to connect to log streamer")
-                    async with session.ws_connect(self.url, **self.connection_args) as ws:
+                    async with session.ws_connect(self.url, **self.connection_args) as ws:  # type: ignore
                         await self.__send_with_connection(ws)
                 except Exception as e:
                     await asyncio.sleep(3)
                     log.warning(f"Could not send log messages to resotoeventlog. Retry. {e}")
 
     async def __send_with_connection(self, ws: ClientWebSocketResponse) -> None:
         while True:
@@ -81,15 +82,15 @@
     "INFO": Severity.info,
     "DEBUG": Severity.debug,
 }
 
 default_log_props = {"message": "message", "pid": "process", "thread": "threadName"}
 
 
-class LogStreamHandler(StreamHandler):
+class LogStreamHandler(StreamHandler):  # type: ignore
     def __init__(
         self,
         process: str,
         streamer: EventStreamer,
         fmt_dict: Optional[Mapping[str, str]] = None,
         attach: bool = True,
     ) -> None:
@@ -132,29 +133,29 @@
         pass
 
 
 class EventStreamSync(EventStream):
     def __enter__(self) -> None:
         self.start()
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.stop()
 
     def start(self) -> None:
         pass
 
     def stop(self) -> None:
         pass
 
 
 class EventStreamAsync(EventStream):
-    async def __aenter__(self):
+    async def __aenter__(self) -> None:
         await self.start()
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
+    async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         await self.stop()
 
     async def start(self) -> None:
         pass
 
     async def stop(self) -> None:
         pass
@@ -175,20 +176,20 @@
         # only here to get the result of the start task (will yield a warning otherwise)
         self.start_future: Optional[Future[None]] = None
         self.stop_future: Optional[Future[None]] = None
 
     def start(self) -> None:
         if self.start_future is None:
             loop = asyncio.get_event_loop()
-            self.start_future = asyncio.run_coroutine_threadsafe(self.streamer.start(), loop)
+            self.start_future = asyncio.run_coroutine_threadsafe(self.streamer.start(), loop)  # type: ignore
 
     def stop(self) -> None:
         if self.start_future is not None:
             loop = asyncio.get_event_loop()
-            self.stop_future = asyncio.run_coroutine_threadsafe(self.streamer.stop(), loop)
+            self.stop_future = asyncio.run_coroutine_threadsafe(self.streamer.stop(), loop)  # type: ignore
             self.start_future = None
 
 
 class EventStreamAsyncService(EventStreamBase, EventStreamAsync):
     async def start(self) -> None:
         await self.streamer.start()
```

### Comparing `resotolib-3.4.0/resotolib/logger.py` & `resotolib-3.4.1/resotolib/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 import json
 from attrs import define, field
-from typing import ClassVar, Optional, Dict, Mapping
+from typing import ClassVar, Optional, Dict, Mapping, Any
 import sys
 import os
 import logging
-from logging import (
-    basicConfig,
-    getLogger,
-    DEBUG,
-    INFO,
-    WARNING,
-    ERROR,
-    CRITICAL,
-    StreamHandler,
-    Formatter,
-)
+from logging import basicConfig, getLogger, DEBUG, INFO, WARNING, ERROR, CRITICAL, StreamHandler, Formatter, LogRecord
 
 
 from resotolib.args import ArgumentParser
 from resotolib.types import Json
 
 DEBUG2 = DEBUG - 1
 DEBUG3 = DEBUG - 2
@@ -52,18 +42,14 @@
         help="Only log errors",
         dest="quiet",
         action="store_true",
         default=False,
     )
 
 
-def add_config(config) -> None:
-    config.add_config(LoggingConfig)
-
-
 @define
 class LoggingConfig:
     kind: ClassVar[str] = "logging"
     verbose: Optional[bool] = field(default=False, metadata={"description": "Verbose logging"})
     quiet: Optional[bool] = field(default=False, metadata={"description": "Only log errors"})
 
 
@@ -74,28 +60,28 @@
     """
 
     def __init__(
         self,
         fmt_dict: Mapping[str, str],
         time_format: str = "%Y-%m-%dT%H:%M:%S",
         static_values: Optional[Dict[str, str]] = None,
-    ):
+    ) -> None:
         super().__init__()
         self.fmt_dict = fmt_dict
         self.time_format = time_format
         self.static_values = static_values or {}
         self.__use_time = "asctime" in self.fmt_dict.values()
 
     def usesTime(self) -> bool:  # noqa: N802
         return self.__use_time
 
-    def formatMessage(self, record) -> dict:  # noqa: N802
+    def formatMessage(self, record: LogRecord) -> dict:  # type: ignore # noqa: N802
         return {fmt_key: record.__dict__[fmt_val] for fmt_key, fmt_val in self.fmt_dict.items()}
 
-    def formatJsonMessage(self, record) -> Json:  # noqa: N802
+    def formatJsonMessage(self, record) -> Json:  # type: ignore # noqa: N802
         record.message = record.getMessage()
 
         if self.__use_time:
             record.asctime = self.formatTime(record, self.time_format)
 
         message_dict = self.formatMessage(record)
         message_dict.update(self.static_values)
@@ -107,15 +93,15 @@
         if record.exc_text:
             message_dict["exception"] = record.exc_text
 
         if record.stack_info:
             message_dict["stack_info"] = self.formatStack(record.stack_info)
         return message_dict
 
-    def format(self, record) -> str:
+    def format(self, record: LogRecord) -> str:
         message_dict = self.formatJsonMessage(record)
         return json.dumps(message_dict, default=str)
 
 
 def setup_logger(
     proc: str,
     *,
@@ -155,15 +141,15 @@
         getLogger("resoto").setLevel(DEBUG)
     elif quiet or "--quiet" in argv or os.environ.get("RESOTO_QUIET", "false").lower() == "true":
         getLogger().setLevel(WARNING)
         getLogger("resoto").setLevel(CRITICAL)
 
 
 # via https://stackoverflow.com/a/35804945/92184
-def add_logging_level(level_name: str, level_num: int, method_name: Optional[str] = None):
+def add_logging_level(level_name: str, level_num: int, method_name: Optional[str] = None) -> None:
     """
     Comprehensively adds a new logging level to the `logging` module and the
     currently configured logging class.
 
     `levelName` becomes an attribute of the `logging` module with the value
     `levelNum`. `methodName` becomes a convenience method for both `logging`
     itself and the class returned by `logging.getLoggerClass()` (usually just
@@ -190,19 +176,19 @@
     if hasattr(logging, level_name):
         raise AttributeError("{} already defined in logging module".format(level_name))
     if hasattr(logging, method_name):
         raise AttributeError("{} already defined in logging module".format(method_name))
     if hasattr(logging.getLoggerClass(), method_name):
         raise AttributeError("{} already defined in logger class".format(method_name))
 
-    def log_for_level(self, message, *args, **kwargs):
+    def log_for_level(self: logging.Logger, message: str, *args: Any, **kwargs: Any) -> None:
         if self.isEnabledFor(level_num):
             self._log(level_num, message, args, **kwargs)
 
-    def log_to_root(message, *args, **kwargs):
+    def log_to_root(message: str, *args: Any, **kwargs: Any) -> None:
         logging.log(level_num, message, *args, **kwargs)
 
     logging.addLevelName(level_num, level_name)
     setattr(logging, level_name, level_num)
     setattr(logging.getLoggerClass(), method_name, log_for_level)
     setattr(logging, method_name, log_to_root)
```

### Comparing `resotolib-3.4.0/resotolib/parse_util.py` & `resotolib-3.4.1/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/proc.py` & `resotolib-3.4.1/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/tree.py` & `resotolib-3.4.1/resotolib/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
 import json
 import uuid
 from collections import defaultdict
 from copy import deepcopy
+from typing import Iterable, Optional, List
 
 from resotolib.logger import log
 
 """
 NOTE:
 This module is copied and ported to proper Python 3.0 from https://github.com/caesar0301/treelib
 Since this library has outdated vulnerable dependencies, we decided to copy it here directly.
@@ -194,15 +196,15 @@
     #: ROOT, DEPTH, WIDTH, ZIGZAG constants :
     (ROOT, DEPTH, WIDTH, ZIGZAG) = list(range(4))
     node_class = Node
 
     def __contains__(self, identifier):
         return identifier in self.nodes.keys()
 
-    def __init__(self, tree=None, deep=False, node_class=None, identifier=None):
+    def __init__(self, tree=None, deep=False, node_class=None, identifier=None) -> None:
         """Initiate a new tree or copy another tree with a shallow or
         deep copy.
         """
         self._identifier = None
         self._set_identifier(identifier)
 
         if node_class:
@@ -210,15 +212,15 @@
             self.node_class = node_class
 
         #: dictionary, identifier: Node object
         self._nodes = {}
 
         #: Get or set the identifier of the root. This attribute can be accessed and modified
         #: with ``.`` and ``=`` operator respectively.
-        self.root = None
+        self.root: Optional[str] = None
 
         if tree is not None:
             self.root = tree.root
             for nid, node in tree.nodes.items():
                 new_node = deepcopy(node) if deep else node
                 self._nodes[nid] = new_node
                 if tree.identifier != self._identifier:
@@ -312,19 +314,19 @@
             raise NodeIDAbsentError("Parent node '%s' " "is not in the tree" % pid)
 
         self._nodes.update({node.identifier: node})
         self.__update_succ_pointer(pid, node.identifier, self.node_class.ADD)
         self.__update_pred_pointer(node.identifier, pid)
         node.set_initial_tree_id(self._identifier)
 
-    def all_nodes(self):
+    def all_nodes(self) -> List[Node]:
         """Return all nodes in a list"""
         return list(self._nodes.values())
 
-    def all_nodes_itr(self):
+    def all_nodes_itr(self) -> Iterable[Node]:
         """
         Returns all nodes in an iterator.
         Added by William Rusnack
         """
         return self._nodes.values()
 
     def ancestor(self, nid, level=None):
@@ -355,26 +357,26 @@
                 return self[ascendant]
             else:
                 descendant = ascendant
                 ascendant = self[descendant].bpointer
                 ascendant_level = self.level(ascendant)
         return None
 
-    def children(self, nid):
+    def children(self, nid) -> List[Node]:
         """
         Return the children (Node) list of nid.
         Empty list is returned if nid does not exist
         """
         return [self[i] for i in self.is_branch(nid)]
 
     def contains(self, nid):
         """Check if the tree contains node of given id"""
         return True if nid in self._nodes else False
 
-    def create_node(self, tag=None, identifier=None, parent=None, data=None):
+    def create_node(self, tag=None, identifier=None, parent=None, data=None) -> Node:
         """
         Create a child node for given @parent node. If ``identifier`` is absent,
         a UUID will be generated automatically.
         """
         node = self.node_class(tag=tag, identifier=identifier, data=data)
         self.add_node(node, parent)
         return node
@@ -477,15 +479,15 @@
         :param func: is passed one node as an argument and that node is included if function returns true,
         :return: a filter iterator of the node in python 3 or a list of the nodes in python 2.
 
         Added by William Rusnack.
         """
         return filter(func, self.all_nodes_itr())
 
-    def get_node(self, nid):
+    def get_node(self, nid) -> Node:
         """
         Get the object of the node with ID of ``nid``.
 
         An alternative way is using '[]' operation on the tree. But small difference exists between them:
         ``get_node()`` will return None if ``nid`` is absent, whereas '[]' will raise ``KeyError``.
         """
         if nid is None or not self.contains(nid):
@@ -504,15 +506,15 @@
 
         try:
             fpointer = self[nid].successors(self._identifier)
         except KeyError:
             fpointer = []
         return fpointer
 
-    def leaves(self, nid=None):
+    def leaves(self, nid=None) -> List[Node]:
         """Get leaves of the whole tree or a subtree."""
         leaves = []
         if nid is None:
             for node in self._nodes.values():
                 if node.is_leaf(self._identifier):
                     leaves.append(node)
         else:
@@ -706,15 +708,15 @@
         res = []
 
         for leaf in self.leaves():
             res.append([nid for nid in self.rsearch(leaf.identifier)][::-1])
 
         return res
 
-    def remove_node(self, identifier):
+    def remove_node(self, identifier) -> int:
         """Remove a node indicated by 'identifier' with all its successors.
         Return the number of removed nodes.
         """
         if not self.contains(identifier):
             raise NodeIDAbsentError("Node '%s' " "is not in the tree" % identifier)
 
         parent = self[identifier].predecessor(self._identifier)
@@ -830,15 +832,15 @@
         else:
             try:
                 level = int(level)
                 return len([node for node in self.all_nodes_itr() if self.level(node.identifier) == level])
             except Exception:
                 raise TypeError("level should be an integer instead of '%s'" % type(level))
 
-    def subtree(self, nid, identifier=None):
+    def subtree(self, nid: Optional[str], identifier: Optional[str] = None) -> Tree:
         """
         Return a shallow COPY of subtree with nid being the new root.
         If nid is None, return an empty tree.
         If you are looking for a deepcopy, please create a new tree
         with this shallow copy, e.g.,
 
         .. code-block:: python
```

### Comparing `resotolib-3.4.0/resotolib/utils.py` & `resotolib-3.4.1/resotolib/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,41 +2,36 @@
 import os
 import random
 import re
 import socket
 import string
 import time
 from argparse import ArgumentParser
-from datetime import date, datetime, timezone, timedelta
 from copy import deepcopy
-
-try:
-    from zoneinfo import ZoneInfo
-except ImportError:
-    from backports.zoneinfo import ZoneInfo
-from tzlocal import get_localzone_name
+from datetime import date, datetime, timezone, timedelta
 from functools import wraps, cached_property
-from pprint import pformat
 from tarfile import TarFile, TarInfo
-from typing import Dict, List, Tuple, Optional, NoReturn, Any, Mapping, Union, Callable, cast
-from resotolib.types import DecoratedFn, JsonElement
+from typing import Dict, List, Tuple, Optional, NoReturn, Any, Mapping, Union, Callable, cast, Iterator, TypeVar
+from zoneinfo import ZoneInfo
 
 import pkg_resources
 import requests
+from tzlocal import get_localzone_name
 
 from resotolib.logger import log
+from resotolib.types import DecoratedFn, JsonElement
+
+T = TypeVar("T")
+UTC_Date_Format = "%Y-%m-%dT%H:%M:%SZ"
 
 
 def rnd_str(str_len: int = 10) -> str:
     return "".join(random.choice(string.ascii_uppercase + string.digits) for _ in range(str_len))
 
 
-UTC_Date_Format = "%Y-%m-%dT%H:%M:%SZ"
-
-
 def utc() -> datetime:
     return datetime.now(timezone.utc)
 
 
 def utc_str(dt: datetime = utc()) -> str:
     if dt.tzinfo is not None and dt.tzname() != "UTC":
         offset = dt.tzinfo.utcoffset(dt)
@@ -72,15 +67,15 @@
     if "day" in td:
         m = re.match(
             r"(?P<days>[-\d]+) day[s]*, (?P<hours>\d+):(?P<minutes>\d+):(?P<seconds>\d[\.\d+]*)",
             td,
         )
     else:
         m = re.match(r"(?P<hours>\d+):(?P<minutes>\d+):(?P<seconds>\d[\.\d+]*)", td)
-    args = {key: float(val) for key, val in m.groupdict().items()}
+    args = {key: float(val) for key, val in m.groupdict().items()}  # type: ignore
     return timedelta(**args)
 
 
 def str2timezone(tz: str) -> timezone:
     mult = 1
     if not tz.startswith("UTC") or len(tz) != 9:
         raise ValueError(f"Invalid timezone string {tz}")
@@ -94,15 +89,15 @@
 def get_local_tzinfo() -> ZoneInfo:
     zone_name = get_localzone_name()
     if zone_name is None:
         zone_name = "Etc/UTC"
     return ZoneInfo(zone_name)
 
 
-def chunks(items: List, n: int) -> List:
+def chunks(items: List[T], n: int) -> Iterator[List[T]]:
     """Split a list of items into multiple lists of size n and yield each chunk"""
     for s in range(0, len(items), n):
         e = s + n
         yield items[s:e]
 
 
 def unset_cached_properties(obj: Any) -> None:
@@ -114,37 +109,16 @@
     cls = obj.__class__
     for a in dir(obj):
         attr_a = getattr(cls, a, cls)
         if isinstance(attr_a, cached_property):
             obj.__dict__.pop(attr_a.attrname, None)
 
 
-def split_esc(s, delim):
-    """Split with support for delimiter escaping
-
-    Via: https://stackoverflow.com/a/29107566
-    """
-    i, res, buf = 0, [], ""
-    while True:
-        j, e = s.find(delim, i), 0
-        if j < 0:  # end reached
-            return res + [buf + s[i:]]  # add remainder
-        while j - e and s[j - e - 1] == "\\":
-            e += 1  # number of escapes
-        d = e // 2  # number of double escapes
-        if e != d * 2:  # odd number of escapes
-            buf += s[i : j - d - 1] + s[j]  # add the escaped char
-            i = j + 1  # and skip it
-            continue  # add more to buf
-        res.append(buf + s[i : j - d])
-        i, buf = j + len(delim), ""  # start after delim
-
-
 # via https://stackoverflow.com/a/1094933
-def iec_size_format(byte_size: int) -> str:
+def iec_size_format(byte_size: float) -> str:
     for unit in ["B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB"]:
         if abs(byte_size) < 1024.0:
             return f"{byte_size:.2f} {unit}"
         byte_size /= 1024.0
     return f"{byte_size:.2f} YiB"
 
 
@@ -158,50 +132,39 @@
             n = f.readinto(buffer_view)
             if not n:
                 break
             h.update(buffer_view[:n])
     return h.hexdigest()
 
 
-def json_default(o):
-    if hasattr(o, "to_json"):
-        return o.to_json()
-    elif isinstance(o, (date, datetime)):
-        return utc_str(o)
-    elif isinstance(o, Exception):
-        return pformat(o)
-    raise TypeError(f"Object of type {o.__class__.__name__} is not JSON serializable")
-
-
 def log_runtime(f: DecoratedFn) -> DecoratedFn:
     @wraps(f)
-    def timer(*args, **kwargs):
+    def timer(*args: Any, **kwargs: Any) -> Any:
         start = time.time()
         ret = f(*args, **kwargs)
         runtime = time.time() - start
         args_str = ", ".join([repr(arg) for arg in args])
         kwargs_str = ", ".join([f"{k}={repr(v)}" for k, v in kwargs.items()])
         if len(args) > 0 and len(kwargs) > 0:
             args_str += ", "
         log.debug(f"Runtime of {f.__name__}({args_str}{kwargs_str}): {runtime:.3f} seconds")
         return ret
 
-    return timer
+    return timer  # type: ignore
 
 
-def except_log_and_pass(do_raise: Optional[Tuple] = None):
-    if do_raise is None:
-        do_raise = ()
+def except_log_and_pass(do_raise: Optional[Tuple[Any]] = None) -> Callable[..., Any]:
+    do_raise_tuple = do_raise if do_raise is not None else ()
 
-    def acallable(f):
+    def acallable(f: Callable[..., Any]) -> Callable[..., Any]:
         @wraps(f)
-        def catch_and_log(*args, **kwargs):
+        def catch_and_log(*args: Any, **kwargs: Any) -> Any:
             try:
                 return f(*args, **kwargs)
-            except do_raise:
+            except do_raise_tuple:
                 raise
             except Exception:
                 args_str = ", ".join([repr(arg) for arg in args])
                 kwargs_str = ", ".join([f"{k}={repr(v)}" for k, v in kwargs.items()])
                 if len(args) > 0 and len(kwargs) > 0:
                     args_str += ", "
                 log.exception(f"Caught exception in {f.__name__}({args_str}{kwargs_str})")
@@ -210,15 +173,17 @@
 
     return acallable
 
 
 resource_attributes_blacklist = ["event_log"]
 
 
-def get_resource_attributes(resource, exclude_private: bool = True, keep_data_structures: bool = False) -> Dict:
+def get_resource_attributes(
+    resource: Any, exclude_private: bool = True, keep_data_structures: bool = False
+) -> Dict[str, Any]:
     attributes = dict(resource.__dict__)
     attributes["kind"] = resource.kind
 
     for attr_name in dir(resource):
         if exclude_private and attr_name.startswith("_"):
             continue
         attr_type = getattr(type(resource), attr_name, None)
@@ -269,20 +234,20 @@
     for key in remove_keys:
         attributes.pop(key)
     attributes.update(add_keys)
 
     return attributes
 
 
-def type_str(o):
+def type_str(o: Any) -> str:
     cls = o.__class__
-    module = cls.__module__
+    module = str(cls.__module__)
     if module == "builtins":
-        return cls.__qualname__
-    return module + "." + cls.__qualname__
+        return str(cls.__qualname__)
+    return module + "." + str(cls.__qualname__)
 
 
 def get_local_ip_addresses(
     *,
     include_loopback: bool = True,
     san_ip_addresses: Optional[List[str]] = None,
     connect_to_ips: Optional[List[str]] = None,
@@ -407,52 +372,52 @@
 
     current_release_uri = f"https://api.github.com/repos/someengineering/resoto/releases/tags/{current_version}"
     current_release_response = requests.get(current_release_uri, headers=headers)
     if current_release_response.status_code == 200:
         current_version_ctime = make_valid_timestamp(
             datetime.strptime(current_release_response.json()["published_at"], "%Y-%m-%dT%H:%M:%SZ")
         )
-        current_version_age = latest_version_ctime - current_version_ctime
+        current_version_age = latest_version_ctime - current_version_ctime  # type: ignore
         msg = (
             f"Current version {current_version} is {current_version_age.days} days out of date."
             f" Latest version is {latest_version}!"
         )
 
     return msg
 
 
-def safe_members_in_tarfile(tarfile: TarFile) -> List:
+def safe_members_in_tarfile(tarfile: TarFile) -> List[Any]:
     # via vmware/pyvcloud/vcd/utils.py
     def badpath(path: str, base: str) -> bool:
         # joinpath will ignore base if path is absolute
         return not os.path.realpath(os.path.abspath(os.path.join(base, path))).startswith(base)
 
     def badlink(info: TarInfo, base: str) -> bool:
         # Links are interpreted relative to the directory containing the link
         tip = os.path.realpath(os.path.abspath(os.path.join(base, os.path.dirname(info.name))))
         return badpath(info.linkname, base=tip)
 
     base = os.path.realpath(os.path.abspath((".")))
-    basename = os.path.basename(tarfile.name)
+    basename = os.path.basename(tarfile.name)  # type: ignore
     result = []
     for tar_info in tarfile.getmembers():
         if badpath(tar_info.name, base):
             log.error(f"Error in {basename}, {tar_info.name} is blocked: illegal path")
         elif tar_info.issym() and badlink(tar_info, base):
             log.error(f"Error in {basename}, {tar_info.name} is blocked:" f" symlink to {tar_info.linkname}")
         elif tar_info.islnk() and badlink(tar_info, base):
             log.error(f"Error in {basename}, {tar_info.name} is blocked:" f" hard link to {tar_info.linkname}")
         else:
             result.append(tar_info)
     return result
 
 
-def rrdata_as_dict(record_type: str, record_data: str) -> Dict:
+def rrdata_as_dict(record_type: str, record_data: str) -> Dict[str, Any]:
     record_type = record_type.upper()
-    rrdata = {}
+    rrdata: Dict[str, Any] = {}
     record_elements = []
     if record_type not in ("TXT"):
         record_data = " ".join(
             "".join([line.split(";")[0] for line in record_data.splitlines()]).replace("(", "").replace(")", "").split()
         )
     if record_type in ("SOA", "MX", "SRV", "CAA"):
         record_elements = record_data.split(" ")
@@ -536,25 +501,25 @@
     # no need to have many instances of this
     Unresolved = UnresolvedEnvVar()
 
     def replace_env_vars_helper(
         elem: JsonElement, environment: Mapping[str, str], keep_unresolved: bool, path: List[Union[str, int]]
     ) -> Union[JsonElement, UnresolvedEnvVar]:
         if isinstance(elem, dict):
-            replaced = {
+            replaced_dict = {
                 k: replace_env_vars_helper(v, environment, keep_unresolved, path + [k]) for k, v in elem.items()
             }
-            without_unresolved = {k: v for k, v in replaced.items() if v is not Unresolved}
-            return without_unresolved
+            without_unresolved_dict = {k: v for k, v in replaced_dict.items() if v is not Unresolved}
+            return without_unresolved_dict
         elif isinstance(elem, list):
-            replaced = [
+            replaced_list = [
                 replace_env_vars_helper(v, environment, keep_unresolved, path + [i]) for i, v, in enumerate(elem)
             ]
-            without_unresolved = [v for v in replaced if v is not Unresolved]
-            return without_unresolved
+            without_unresolved_list = [v for v in replaced_list if v is not Unresolved]
+            return without_unresolved_list
         elif isinstance(elem, str):
             str_value = elem
             for match in re.finditer(env_var_substitution_pattern, elem):
                 env_var_name = match.group(1)
                 if env_var_found := environment.get(env_var_name):
                     str_value = str_value.replace(match.group(0), env_var_found)
                 elif keep_unresolved:
```

### Comparing `resotolib-3.4.0/resotolib/web/__init__.py` & `resotolib-3.4.1/resotolib/web/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import threading
 import cherrypy
 from resotolib.logger import log
-from typing import Optional
+from typing import Optional, Any
 
 
 class WebServer(threading.Thread):
     def __init__(
         self,
-        web_app,
+        web_app: Any,
         web_host: str = "::",
         web_port: int = 9955,
         ssl_cert: Optional[str] = None,
         ssl_key: Optional[str] = None,
     ) -> None:
         super().__init__()
         self.name = "webserver"
         self.web_app = web_app
         self.web_host = web_host
         self.web_port = web_port
         self.ssl_cert = ssl_cert
         self.ssl_key = ssl_key
 
     @property
-    def serving(self):
-        return cherrypy.engine.state == cherrypy.engine.states.STARTED
+    def serving(self) -> bool:
+        return bool(cherrypy.engine.state == cherrypy.engine.states.STARTED)
 
     def run(self) -> None:
         # CherryPy always prefixes its log messages with a timestamp.
         # The next line monkey patches that time method to return a
         # fixed string. So instead of having duplicate timestamps in
         # each web server related log message they are now prefixed
         # with the string 'CherryPy'.
@@ -71,10 +71,10 @@
                     **ssl_args,
                 }
             }
         )
         cherrypy.engine.start()
         cherrypy.engine.block()
 
-    def shutdown(self):
+    def shutdown(self) -> None:
         log.debug("Received request to shutdown http server threads")
         cherrypy.engine.exit()
```

### Comparing `resotolib-3.4.0/resotolib/web/metrics.py` & `resotolib-3.4.1/resotolib/web/metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         }
         self.config = {"/": config}
         if self.mountpoint not in ("/", ""):
             self.config[self.mountpoint] = config
 
     @cherrypy.expose
     @cherrypy.tools.allow(methods=["GET"])
-    def health(self):
+    def health(self) -> str:
         cherrypy.response.headers["Content-Type"] = "text/plain"
         return "ok\r\n"
 
     @cherrypy.expose
     @cherrypy.tools.allow(methods=["GET"])
-    def metrics(self):
+    def metrics(self) -> bytes:
         cherrypy.response.headers["Content-Type"] = CONTENT_TYPE_LATEST
         return generate_latest()
```

### Comparing `resotolib-3.4.0/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.4.1/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.4.1/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.4.1/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/web/static/favicon-16x16.png` & `resotolib-3.4.1/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/web/static/favicon-32x32.png` & `resotolib-3.4.1/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/web/static/index.html` & `resotolib-3.4.1/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/web/static/mstile-150x150.png` & `resotolib-3.4.1/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/web/static/picnic.min.css` & `resotolib-3.4.1/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/resotolib/x509.py` & `resotolib-3.4.1/resotolib/x509.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,30 @@
     ip_address,
     ip_network,
     IPv4Address,
     IPv6Address,
     IPv4Network,
     IPv6Network,
 )
+
+from cryptography.hazmat._oid import ExtendedKeyUsageOID
+
 from resotolib.utils import get_local_hostnames, get_local_ip_addresses
 from datetime import datetime, timedelta, timezone
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric.rsa import (
     RSAPrivateKey,
     generate_private_key,
 )
 from cryptography.x509.base import Certificate, CertificateSigningRequest
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union, Dict, Any
 
 
 def gen_rsa_key(key_size: int = 2048) -> RSAPrivateKey:
     return generate_private_key(public_exponent=65537, key_size=key_size, backend=default_backend())
 
 
 def bootstrap_ca(
@@ -146,17 +149,17 @@
             ),
             critical=True,
         )
     )
     if server_auth or client_auth:
         key_usage = []
         if server_auth:
-            key_usage.append(x509.ExtendedKeyUsageOID.SERVER_AUTH)
+            key_usage.append(ExtendedKeyUsageOID.SERVER_AUTH)
         if client_auth:
-            key_usage.append(x509.ExtendedKeyUsageOID.CLIENT_AUTH)
+            key_usage.append(ExtendedKeyUsageOID.CLIENT_AUTH)
         crt_build = crt_build.add_extension(x509.ExtendedKeyUsage(key_usage), critical=False)
     for extension in csr.extensions:
         if not isinstance(extension.value, x509.SubjectAlternativeName):
             continue
         crt_build = crt_build.add_extension(extension.value, critical=extension.critical)
     return crt_build.sign(ca_key, hashes.SHA256(), default_backend())
 
@@ -181,15 +184,15 @@
     tmp_cert_path = f"{cert_path}.tmp" if rename else cert_path
     with open(tmp_cert_path, "wb") as f:
         if include_certifi:
             f.write(certifi.contents().encode())
         f.write("\n".encode())
         f.write(f"# Issuer: {cert.issuer.rfc4514_string()}\n".encode())
         f.write(f"# Subject: {cert.subject.rfc4514_string()}\n".encode())
-        label = cert.issuer.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value
+        label: str = cert.issuer.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value  # type: ignore
         f.write(f"# Label: {label}\n".encode())
         f.write(f"# Serial: {cert.serial_number}\n".encode())
         md5 = cert_fingerprint(cert, "MD5")
         sha1 = cert_fingerprint(cert, "SHA1")
         sha256 = cert_fingerprint(cert, "SHA256")
         f.write(f"# MD5 Fingerprint: {md5}\n".encode())
         f.write(f"# SHA1 Fingerprint: {sha1}\n".encode())
@@ -211,16 +214,16 @@
     if rename:
         os.rename(tmp_key_path, key_path)
 
 
 def key_to_bytes(
     key: RSAPrivateKey,
     passphrase: Optional[str] = None,
-):
-    kwargs = {"encryption_algorithm": serialization.NoEncryption()}
+) -> bytes:
+    kwargs: Dict[str, Any] = {"encryption_algorithm": serialization.NoEncryption()}
     if passphrase is not None:
         kwargs["encryption_algorithm"] = serialization.BestAvailableEncryption(passphrase.encode())
     return key.private_bytes(
         encoding=serialization.Encoding.PEM,
         format=serialization.PrivateFormat.TraditionalOpenSSL,
         **kwargs,
     )
@@ -261,16 +264,16 @@
 
 
 def load_key_from_bytes(
     key: bytes, passphrase: Optional[str] = None, skip_rsa_key_validation: bool = False
 ) -> RSAPrivateKey:
     backend = default_backend()
     if passphrase is not None:
-        passphrase = passphrase.encode()
-    return backend.load_pem_private_key(key, passphrase, skip_rsa_key_validation)
+        passphrase = passphrase.encode()  # type: ignore
+    return backend.load_pem_private_key(key, passphrase, skip_rsa_key_validation)  # type: ignore
 
 
 def make_ip(ip: str) -> Union[IPv4Address, IPv6Address, IPv4Network, IPv6Network]:
     if "/" in ip:
         return ip_network(ip)
     else:
         return ip_address(ip)
```

### Comparing `resotolib-3.4.0/resotolib.egg-info/PKG-INFO` & `resotolib-3.4.1/resotolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -34,15 +34,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotolib-3.4.0/resotolib.egg-info/SOURCES.txt` & `resotolib-3.4.1/resotolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/setup.py` & `resotolib-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/asynchronous/web/test_auth.py` & `resotolib-3.4.1/test/asynchronous/web/test_auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/core/custom_command_test.py` & `resotolib-3.4.1/test/core/custom_command_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/core/model_check_test.py` & `resotolib-3.4.1/test/core/model_check_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/core/model_export_test.py` & `resotolib-3.4.1/test/core/model_export_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/core/progress_test.py` & `resotolib-3.4.1/test/core/progress_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/core/tasks_test.py` & `resotolib-3.4.1/test/core/tasks_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/durations_test.py` & `resotolib-3.4.1/test/durations_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/json_bender_test.py` & `resotolib-3.4.1/test/json_bender_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/parse_util_test.py` & `resotolib-3.4.1/test/parse_util_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_args.py` & `resotolib-3.4.1/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_baseresources.py` & `resotolib-3.4.1/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_config.py` & `resotolib-3.4.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_graph.py` & `resotolib-3.4.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_graph_extensions.py` & `resotolib-3.4.1/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_json.py` & `resotolib-3.4.1/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_jwt.py` & `resotolib-3.4.1/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_plugin.py` & `resotolib-3.4.1/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_tree.py` & `resotolib-3.4.1/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_utils.py` & `resotolib-3.4.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_web.py` & `resotolib-3.4.1/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.0/test/test_x509.py` & `resotolib-3.4.1/test/test_x509.py`

 * *Files identical despite different names*

