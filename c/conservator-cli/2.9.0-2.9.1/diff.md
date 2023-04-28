# Comparing `tmp/conservator-cli-2.9.0.tar.gz` & `tmp/conservator-cli-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conservator-cli-2.9.0.tar", last modified: Mon Mar  6 23:42:15 2023, max compression
+gzip compressed data, was "conservator-cli-2.9.1.tar", last modified: Fri Mar 10 22:06:43 2023, max compression
```

## Comparing `conservator-cli-2.9.0.tar` & `conservator-cli-2.9.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.366573 conservator-cli-2.9.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.338573 conservator-cli-2.9.0/FLIR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.346573 conservator-cli-2.9.0/FLIR/conservator/
--rw-r--r--   0 root         (0) root         (0)       82 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.350573 conservator-cli-2.9.0/FLIR/conservator/cli/
--rw-r--r--   0 root         (0) root         (0)     2322 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/cli/config.py
--rw-r--r--   0 root         (0) root         (0)    16123 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/cli/cvc.py
--rw-r--r--   0 root         (0) root         (0)    12922 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/cli/interactive.py
--rw-r--r--   0 root         (0) root         (0)    17131 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/cli/managers.py
--rw-r--r--   0 root         (0) root         (0)    11384 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.350573 conservator-cli-2.9.0/FLIR/conservator/configs/
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/configs/download.json
--rw-r--r--   0 root         (0) root         (0)      592 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/configs/upload.json
--rw-r--r--   0 root         (0) root         (0)     7059 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/connection.py
--rw-r--r--   0 root         (0) root         (0)     4719 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/conservator.py
--rw-r--r--   0 root         (0) root         (0)     7082 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/fields_manager.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/fields_request.py
--rw-r--r--   0 root         (0) root         (0)     9209 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/file_transfers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.350573 conservator-cli-2.9.0/FLIR/conservator/generated/
--rw-r--r--   0 root         (0) root         (0)      235 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/generated/date.py
--rw-r--r--   0 root         (0) root         (0)   352004 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/generated/schema.py
--rw-r--r--   0 root         (0) root         (0)    41082 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/local_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.354573 conservator-cli-2.9.0/FLIR/conservator/managers/
--rw-r--r--   0 root         (0) root         (0)    14451 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/managers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11244 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/managers/media.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/managers/searchable.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/managers/type_manager.py
--rw-r--r--   0 root         (0) root         (0)     8948 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/paginated_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.354573 conservator-cli-2.9.0/FLIR/conservator/run_tasks_plugins/
--rw-r--r--   0 root         (0) root         (0)      296 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/run_tasks_plugins/conservator_cli.py
--rw-r--r--   0 root         (0) root         (0)     3872 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/util.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-06 23:42:15.000000 conservator-cli-2.9.0/FLIR/conservator/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.362573 conservator-cli-2.9.0/FLIR/conservator/wrappers/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14670 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/collection.py
--rw-r--r--   0 root         (0) root         (0)    15918 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/dataset.py
--rw-r--r--   0 root         (0) root         (0)     6314 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/dataset_frame.py
--rw-r--r--   0 root         (0) root         (0)     3420 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/file_locker.py
--rw-r--r--   0 root         (0) root         (0)     2896 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/frame.py
--rw-r--r--   0 root         (0) root         (0)      675 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/image.py
--rw-r--r--   0 root         (0) root         (0)    10682 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/media.py
--rw-r--r--   0 root         (0) root         (0)     3158 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/metadata.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/project.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/queryable.py
--rw-r--r--   0 root         (0) root         (0)     8577 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/type_proxy.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/FLIR/conservator/wrappers/video.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1035 2023-03-06 23:42:15.366573 conservator-cli-2.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 23:42:15.366573 conservator-cli-2.9.0/conservator_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1035 2023-03-06 23:42:15.000000 conservator-cli-2.9.0/conservator_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1697 2023-03-06 23:42:15.000000 conservator-cli-2.9.0/conservator_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-06 23:42:15.000000 conservator-cli-2.9.0/conservator_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2023-03-06 23:42:15.000000 conservator-cli-2.9.0/conservator_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-06 23:28:29.000000 conservator-cli-2.9.0/conservator_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      209 2023-03-06 23:42:15.000000 conservator-cli-2.9.0/conservator_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-06 23:42:15.000000 conservator-cli-2.9.0/conservator_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-06 23:42:15.366573 conservator-cli-2.9.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2848 2023-03-06 23:28:03.000000 conservator-cli-2.9.0/setup.py
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.730650 conservator-cli-2.9.1/
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.706650 conservator-cli-2.9.1/FLIR/
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.714650 conservator-cli-2.9.1/FLIR/conservator/
+-rw-r--r--   0 tester    (1000) docker     (999)       82 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/__init__.py
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.714650 conservator-cli-2.9.1/FLIR/conservator/cli/
+-rw-r--r--   0 tester    (1000) docker     (999)     2322 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/cli/__init__.py
+-rw-r--r--   0 tester    (1000) docker     (999)     2020 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/cli/config.py
+-rw-r--r--   0 tester    (1000) docker     (999)    18242 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/cli/cvc.py
+-rw-r--r--   0 tester    (1000) docker     (999)    12922 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/cli/interactive.py
+-rw-r--r--   0 tester    (1000) docker     (999)    17131 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/cli/managers.py
+-rw-r--r--   0 tester    (1000) docker     (999)    12109 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/config.py
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.714650 conservator-cli-2.9.1/FLIR/conservator/configs/
+-rw-r--r--   0 tester    (1000) docker     (999)      588 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/configs/download.json
+-rw-r--r--   0 tester    (1000) docker     (999)      592 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/configs/upload.json
+-rw-r--r--   0 tester    (1000) docker     (999)     7478 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/connection.py
+-rw-r--r--   0 tester    (1000) docker     (999)     5374 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/conservator.py
+-rw-r--r--   0 tester    (1000) docker     (999)     7082 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/fields_manager.py
+-rw-r--r--   0 tester    (1000) docker     (999)     6564 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/fields_request.py
+-rw-r--r--   0 tester    (1000) docker     (999)     9209 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/file_transfers.py
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.718650 conservator-cli-2.9.1/FLIR/conservator/generated/
+-rw-r--r--   0 tester    (1000) docker     (999)      235 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/generated/__init__.py
+-rw-r--r--   0 tester    (1000) docker     (999)      398 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/generated/date.py
+-rw-r--r--   0 tester    (1000) docker     (999)   352004 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/generated/schema.py
+-rw-r--r--   0 tester    (1000) docker     (999)    41171 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/local_dataset.py
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.722650 conservator-cli-2.9.1/FLIR/conservator/managers/
+-rw-r--r--   0 tester    (1000) docker     (999)    14451 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/managers/__init__.py
+-rw-r--r--   0 tester    (1000) docker     (999)    11244 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/managers/media.py
+-rw-r--r--   0 tester    (1000) docker     (999)     1456 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/managers/searchable.py
+-rw-r--r--   0 tester    (1000) docker     (999)     2536 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/managers/type_manager.py
+-rw-r--r--   0 tester    (1000) docker     (999)     8948 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/paginated_query.py
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.722650 conservator-cli-2.9.1/FLIR/conservator/run_tasks_plugins/
+-rw-r--r--   0 tester    (1000) docker     (999)      296 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/run_tasks_plugins/conservator_cli.py
+-rw-r--r--   0 tester    (1000) docker     (999)     4181 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/util.py
+-rw-r--r--   0 tester    (1000) docker     (999)       18 2023-03-10 22:06:43.000000 conservator-cli-2.9.1/FLIR/conservator/version.py
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.726650 conservator-cli-2.9.1/FLIR/conservator/wrappers/
+-rw-r--r--   0 tester    (1000) docker     (999)     1124 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/__init__.py
+-rw-r--r--   0 tester    (1000) docker     (999)    14670 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/collection.py
+-rw-r--r--   0 tester    (1000) docker     (999)    15918 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/dataset.py
+-rw-r--r--   0 tester    (1000) docker     (999)     6314 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/dataset_frame.py
+-rw-r--r--   0 tester    (1000) docker     (999)     3420 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/file_locker.py
+-rw-r--r--   0 tester    (1000) docker     (999)     2896 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/frame.py
+-rw-r--r--   0 tester    (1000) docker     (999)      675 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/image.py
+-rw-r--r--   0 tester    (1000) docker     (999)    10682 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/media.py
+-rw-r--r--   0 tester    (1000) docker     (999)     3158 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/metadata.py
+-rw-r--r--   0 tester    (1000) docker     (999)     1052 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/project.py
+-rw-r--r--   0 tester    (1000) docker     (999)     1819 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/queryable.py
+-rw-r--r--   0 tester    (1000) docker     (999)     8577 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/type_proxy.py
+-rw-r--r--   0 tester    (1000) docker     (999)      752 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/FLIR/conservator/wrappers/video.py
+-rw-r--r--   0 tester    (1000) docker     (999)     1070 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/LICENSE
+-rw-r--r--   0 tester    (1000) docker     (999)     1035 2023-03-10 22:06:43.730650 conservator-cli-2.9.1/PKG-INFO
+-rw-r--r--   0 tester    (1000) docker     (999)      567 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/README.md
+drwxr-xr-x   0 tester    (1000) docker     (999)        0 2023-03-10 22:06:43.730650 conservator-cli-2.9.1/conservator_cli.egg-info/
+-rw-r--r--   0 tester    (1000) docker     (999)     1035 2023-03-10 22:06:43.000000 conservator-cli-2.9.1/conservator_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tester    (1000) docker     (999)     1697 2023-03-10 22:06:43.000000 conservator-cli-2.9.1/conservator_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tester    (1000) docker     (999)        1 2023-03-10 22:06:43.000000 conservator-cli-2.9.1/conservator_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tester    (1000) docker     (999)       94 2023-03-10 22:06:43.000000 conservator-cli-2.9.1/conservator_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tester    (1000) docker     (999)        1 2023-03-10 21:52:43.000000 conservator-cli-2.9.1/conservator_cli.egg-info/not-zip-safe
+-rw-r--r--   0 tester    (1000) docker     (999)      209 2023-03-10 22:06:43.000000 conservator-cli-2.9.1/conservator_cli.egg-info/requires.txt
+-rw-r--r--   0 tester    (1000) docker     (999)        5 2023-03-10 22:06:43.000000 conservator-cli-2.9.1/conservator_cli.egg-info/top_level.txt
+-rw-r--r--   0 tester    (1000) docker     (999)       38 2023-03-10 22:06:43.730650 conservator-cli-2.9.1/setup.cfg
+-rwxr-xr-x   0 tester    (1000) docker     (999)     2848 2023-03-10 21:52:15.000000 conservator-cli-2.9.1/setup.py
```

### Comparing `conservator-cli-2.9.0/FLIR/conservator/cli/__init__.py` & `conservator-cli-2.9.1/FLIR/conservator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/cli/config.py` & `conservator-cli-2.9.1/FLIR/conservator/cli/config.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/cli/cvc.py` & `conservator-cli-2.9.1/FLIR/conservator/cli/cvc.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,32 @@
 
 import click
 
 from click import get_current_context
 
 from FLIR.conservator.conservator import Conservator
 from FLIR.conservator.local_dataset import LocalDataset
-from FLIR.conservator.util import check_platform
+from FLIR.conservator.util import check_platform, check_dir_access
 
 
 def pass_valid_local_dataset(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         ctx_obj = get_current_context().obj
 
         if "conservator" in ctx_obj:
             conservator = ctx_obj["conservator"]
+        elif "url" in ctx_obj and "api_key" in ctx_obj:
+            path = ctx_obj["cvc_local_path"]
+            config_dict = {
+                "CONSERVATOR_URL": ctx_obj["url"],
+                "CONSERVATOR_API_KEY": ctx_obj["api_key"],
+            }
+            conservator = Conservator.from_config_dict(config_dict)
+            ctx_obj["conservator"] = conservator
         else:
             path = ctx_obj["cvc_local_path"]
             conservator = Conservator.create(ctx_obj["config_name"])
             ctx_obj["conservator"] = conservator
 
         # raises InvalidLocalDatasetPath if the path does not point to a
         # valid LocalDataset (defined as a directory containing index.json).
@@ -139,47 +147,68 @@
     "--config",
     default=None,
     help="Conservator config name, use default credentials if not specified",
 )
 @click.option(
     "-p", "--path", default=".", help="Path to dataset, defaults to current directory"
 )
+@click.option("-u", "--url", help="URL of Conservator instance to connect to")
+@click.option("-k", "--api-key", help="API Key to use when connecting to Conservator")
 @click.version_option(prog_name="conservator-cli", package_name="conservator-cli")
 @click.pass_context
-def main(ctx, log, path, config):
+def main(ctx, log, path, config, url, api_key):
     check_platform()
     levels = {
         "DEBUG": logging.DEBUG,
         "INFO": logging.INFO,
         "WARNING": logging.WARNING,
         "ERROR": logging.ERROR,
         "CRITICAL": logging.CRITICAL,
     }
     logging.basicConfig(level=levels[log])
 
     ctx.ensure_object(dict)
     ctx.obj["config_name"] = config
     ctx.obj["cvc_local_path"] = path
+    if url is None and api_key is not None:
+        click.secho("Must provide either both url and api_key, or neither!", fg="red")
+        sys.exit(1)
+    if url is not None and api_key is None:
+        click.secho("Must provide either both url and api_key, or neither!", fg="red")
+        sys.exit(1)
+    if url is not None:
+        ctx.obj["url"] = url
+    if api_key is not None:
+        ctx.obj["api_key"] = api_key
 
 
 @main.command(help="Clone a dataset by id, path, or name (if unique)")
 @click.argument("identifier")
 @click.option(
     "-p",
     "--path",
     default=None,
     help="An empty directory to clone the dataset to. Defaults to a new "
     "directory with the name of the dataset",
 )
 @click.option(
     "-c", "--checkout", help="If specified, a commit hash to checkout after cloning"
 )
+@click.option("-u", "--url", help="URL of Conservator instance to connect to")
+@click.option("-k", "--api-key", help="API Key to use when connecting to Conservator")
 @click.pass_context
-def clone(ctx, identifier, path, checkout):
-    conservator = Conservator.create(ctx.obj["config_name"])
+def clone(ctx, identifier, path, checkout, url, api_key):
+    if not check_dir_access(os.getcwd()):
+        click.secho(f"Cannot clone to directory {os.getcwd()}!", fg="red", bold=True)
+        sys.exit(1)
+    if url is not None and api_key is not None:
+        config_dict = {"CONSERVATOR_URL": url, "CONSERVATOR_API_KEY": api_key}
+        conservator = Conservator.from_config_dict(config_dict)
+    else:
+        conservator = Conservator.create(ctx.obj["config_name"])
     dataset = conservator.datasets.from_string(identifier)
     cloned = LocalDataset.clone(dataset, path)
     if checkout is not None:
         cloned.checkout(checkout)
 
 
 @main.command("checkout", help="Checkout a commit hash")
@@ -329,14 +358,30 @@
     default=5,
     show_default=True,
     help="Number of tries to recover from spurious server errors.",
 )
 @pass_valid_local_dataset
 @check_git_config
 def download(local_dataset, include_raw, include_analytics, pool_size, symlink, tries):
+    if include_raw and not check_dir_access(local_dataset.data_path):
+        click.secho(f"Cannot write to {local_dataset.data_path}!", fg="red", bold=True)
+        sys.exit(1)
+
+    if include_analytics and not check_dir_access(local_dataset.raw_data_path):
+        click.secho(f"Cannot write to {local_dataset.data_path}!", fg="red", bold=True)
+        sys.exit(1)
+
+    if not check_dir_access(local_dataset.cache_path):
+        click.secho(
+            f"Cannot write to cache directory ({local_dataset.cache_path})!",
+            fg="red",
+            bold=True,
+        )
+        sys.exit(1)
+
     if pool_size == 10:  # default
         yellow = "\x1b[33;21m"
         cyan = "\x1b[36;21m"
         reset = "\x1b[0m"
         click.echo(
             f"{yellow}If you have a fast connection, you might be able to speed "
             f"this up by rerunning with the -p (--process_count) option. "
```

### Comparing `conservator-cli-2.9.0/FLIR/conservator/cli/interactive.py` & `conservator-cli-2.9.1/FLIR/conservator/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/cli/managers.py` & `conservator-cli-2.9.1/FLIR/conservator/cli/managers.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/config.py` & `conservator-cli-2.9.1/FLIR/conservator/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,67 +27,72 @@
         self.internal_name = internal_name
         self.friendly_name = friendly_name
         self.default = default
         self.type_ = type_
         self.validator = validator
 
 
-"""
-validators for config fields
-
-input argument 'd' is dict of config data containing the field of interest
-"""
-
-
-def validate_max_retries(d):
+def validate_max_retries(config_dict):
+    """
+    Validates max retries value in a config
+    """
     retries_ok = False
     try:
-        max_retries = int(d["CONSERVATOR_MAX_RETRIES"])
+        max_retries = int(config_dict["CONSERVATOR_MAX_RETRIES"])
         if max_retries > 0:
             retries_ok = True
         else:
             print("Error: invalid retries count, please try again")
     except Exception:
         print("Error: invalid retries count, please try again")
     return retries_ok
 
 
-def validate_cache_path(d):
-    cache_path = d["CONSERVATOR_CVC_CACHE_PATH"]
+def validate_cache_path(config_dict):
+    """
+    Validates cache path value in a config
+    """
+    cache_path = config_dict["CONSERVATOR_CVC_CACHE_PATH"]
     dir_ok = False
     try:
         os.makedirs(cache_path, exist_ok=True)
         os.chmod(cache_path, 0o755)
         dir_ok = True
     except Exception:
         print("Error: invalid cache path, please try again")
     return dir_ok
 
 
-def validate_url(d):
+def validate_url(config_dict):
+    """
+    Validates URL value in a config
+    """
     url_ok = False
     try:
         # does url have graphql endpoint?
-        check_url = ConservatorConnection.to_graphql_url(d["CONSERVATOR_URL"])
-        r = requests.head(check_url)
-        if r.status_code == 405:
+        check_url = ConservatorConnection.to_graphql_url(config_dict["CONSERVATOR_URL"])
+        response = requests.head(check_url, timeout=10)
+        if response.status_code == 405:
             url_ok = True
     except Exception:
         pass
 
     if not url_ok:
         print("Error: invalid url, please try again")
     return url_ok
 
 
-def validate_key(d):
+def validate_key(config_dict):
+    """
+    Validates API Key value in a config
+    """
     key_ok = False
 
     # check whether this is a valid config
-    config = Config.from_dict(d)
+    config = Config.from_dict(config_dict)
 
     # is API key accepted by server?
     connection = ConservatorConnection(config)
     try:
         connection.get_email()
         key_ok = True
     except Exception:
@@ -138,26 +143,29 @@
                 "CONSERVATOR_API_KEY", "Conservator API Key", validator=validate_key
             ),
         }
     )
 
     def __init__(self, **kwargs):
         for name, attr in Config.ATTRIBUTES.items():
-            v = kwargs.get(attr.internal_name, None)
-            if v is not None:
-                v = attr.type_(v)
-            if v is None:
-                v = attr.default
-            if v is None:
+            value = kwargs.get(attr.internal_name, None)
+            if value is not None:
+                value = attr.type_(value)
+            if value is None:
+                value = attr.default
+            if value is None:
                 raise ConfigError(f"Missing value for '{name}'")
-            assert type(v) == attr.type_
-            setattr(self, name, v)
+            assert isinstance(value, attr.type_)
+            setattr(self, name, value)
 
     @staticmethod
     def from_dict(data):
+        """
+        Construct a Config object from a dict
+        """
         return Config(**data)
 
     @staticmethod
     def from_environ():
         """
         Creates a :class:`Config` object from environment variables.
         """
@@ -168,62 +176,68 @@
         """
         Creates a :class:`Config` object from standard input.
         """
 
         # just show prompts, not errors from functions used to validate config
         logging.disable(logging.CRITICAL)
 
-        d = {}
+        config_dict = {}
         for name, attr in Config.ATTRIBUTES.items():
             # loop until user supplies a config that actually works
             while True:
                 if attr.default is None:
-                    v = input(f"{attr.friendly_name}: ")
+                    value = input(f"{attr.friendly_name}: ")
                 else:
-                    v = input(
+                    value = input(
                         f"{attr.friendly_name} (leave empty for {attr.default}): "
                     )
-                v = v.strip()
-                if len(v) == 0:
-                    v = attr.default
-                d[attr.internal_name] = v
+                value = value.strip()
+                if len(value) == 0:
+                    value = attr.default
+                config_dict[attr.internal_name] = value
                 # move on to next field if validator passes
-                if attr.validator(d):
+                if attr.validator(config_dict):
                     break
 
         # restore logging level to normal
         logging.disable(logging.NOTSET)
 
-        return Config.from_dict(d)
+        return Config.from_dict(config_dict)
 
     @staticmethod
     def from_file(path):
         """
         Creates a :class:`Config` object from a JSON config file.
 
         .. note:: For security, this file's mode will be set to ``600``.
 
         :param path: The path to the JSON config file.
         """
         try:
-            with open(path, "r") as config:
+            with open(path, "r", encoding="utf-8") as config:
                 data = json.load(config)
             if os.stat(path).st_mode & 0o777 != 0o600:
                 logger.warning("Changing config file mode to 0600.")
                 os.chmod(path, 0o600)
             return Config.from_dict(data)
         except FileNotFoundError:
             return None
 
     @classmethod
     def from_named_config_file(cls, name):
+        """
+        Create a config object from a named config file
+        """
         return Config.from_file(Config.named_config_path(name))
 
     @staticmethod
     def from_name(name):
+        """
+        Create a config object by config name
+        """
         return Config.from_named_config_file(name)
 
     @staticmethod
     def from_default_config_file():
         """
         Creates a :class:`Config` object from the JSON config file
         at the :func:`Config.default_config_path`.
@@ -249,21 +263,24 @@
 
         .. note:: For security, this file's mode will be set to ``600``.
 
         :param path: The file path to save to.
         """
         directory = os.path.split(path)[0]
         os.makedirs(directory, exist_ok=True)
-        with open(path, "w") as f:
-            json.dump(self.to_dict(), f)
+        with open(path, "w", encoding="utf-8") as json_file:
+            json.dump(self.to_dict(), json_file)
         if os.stat(path).st_mode & 0o777 != 0o600:
             logger.warning("Changing config file mode to 600.")
             os.chmod(path, 0o600)
 
     def to_dict(self):
+        """
+        Return config object as a dict
+        """
         return {
             attr.internal_name: getattr(self, name)
             for name, attr in self.ATTRIBUTES.items()
         }
 
     def save_to_named_config(self, name):
         """
@@ -294,14 +311,17 @@
         """
         The default config is saved in ``~/.config/conservator-cli/default.json``.
         """
         return Config.named_config_path(Config.DEFAULT_NAME)
 
     @staticmethod
     def saved_config_names():
+        """
+        Returns a list of config names
+        """
         root_path = os.path.join(os.path.expanduser("~"), ".config", "conservator-cli")
         files = os.listdir(root_path)
         return [file[: -len(".json")] for file in files]
 
     @staticmethod
     def delete_saved_default_config():
         """
@@ -339,15 +359,15 @@
         ]:
             creds = None
             try:
                 creds = source()
             except Exception:
                 pass
             if creds is not None:
-                logger.debug(f"Created config from source: {source}")
+                logger.debug("Created config from source: %s", source)
                 if save and source == Config.from_input:
                     creds.save_to_default_config()
                 return creds
         raise ConfigError("Couldn't find or create a config")
 
     def __str__(self):
         return f"""Config for {self.url}:""" + "".join(
```

### Comparing `conservator-cli-2.9.0/FLIR/conservator/configs/download.json` & `conservator-cli-2.9.1/FLIR/conservator/configs/download.json`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/configs/upload.json` & `conservator-cli-2.9.1/FLIR/conservator/configs/upload.json`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/connection.py` & `conservator-cli-2.9.1/FLIR/conservator/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# pylint: disable=missing-module-docstring
+# pylint: disable=broad-except
+# pylint: disable=unnecessary-pass
 import re
 import urllib.parse
 import logging
 import platform
 import sys
 
 import requests
@@ -95,37 +98,39 @@
         key = self.config.key
         return f"{email}:{key}"
 
     def get_url(self):
         """
         Returns the base URL for Conservator.
         """
-        r = urllib.parse.urlparse(self.config.url)
-        return f"{r.scheme}://{r.netloc}"
+        parsed_url = urllib.parse.urlparse(self.config.url)
+        return f"{parsed_url.scheme}://{parsed_url.netloc}"
 
     def get_collection_url(self, collection):
         """
         Returns a URL for viewing `collection`.
         """
-        return self.get_url() + f"/projects/{collection.id}"
+        return f"{self.get_url()}/projects/{collection.id}"
 
     def get_domain(self):
         """
         Returns the domain name of the Conservator instance.
         """
         return urllib.parse.urlparse(self.config.url).netloc
 
     def get_authenticated_url(self):
         """
         Returns an authenticated URL that contains an encoded username and token.
 
         This URL is used when downloading files and repositories.
         """
-        r = urllib.parse.urlparse(self.config.url)
-        return f"{r.scheme}://{self.get_url_encoded_user()}@{r.netloc}"
+        parsed_url = urllib.parse.urlparse(self.config.url)
+        return (
+            f"{parsed_url.scheme}://{self.get_url_encoded_user()}@{parsed_url.netloc}"
+        )
 
     def get_dvc_url(self):
         """
         Returns the DVC URL used for downloading files.
         """
         return f"{self.get_authenticated_url()}/dvc"
 
@@ -137,20 +142,24 @@
 
     def dvc_hash_exists(self, md5):
         """
         Returns `True` if DVC contains the given `md5` hash, and `False` otherwise.
         """
         hash_url = self.get_dvc_hash_url(md5)
         # We only care about the status code, so we use .head
-        r = requests.head(hash_url)
+        response = requests.head(hash_url, timeout=10)
         # 302 means the file was found.
-        return r.status_code == 302
+        return response.status_code == 302
 
     @staticmethod
     def to_graphql_url(url):
+        """
+        Ensure a URL is formatted correctly
+        (i.e. ends with "/graphql")
+        """
         if url.endswith("/"):
             url = url[:-1]
         if not url.endswith("graphql"):
             url = url + "/graphql"
         return url
 
     def run(self, operation, variables=None):
@@ -161,15 +170,15 @@
         If any errors are encountered, they will be raised with a
         :class:`ConservatorGraphQLServerError`.
         """
         # The depth is completely arbitrary atm...
         gql = operation.__to_graphql__(auto_select_depth=5)
         gql = re.sub(r"\w* {\s*}\s*", "", gql)
         json_response = self.endpoint(gql, variables)
-        logger.debug("Response: " + str(json_response))
+        logger.debug("Response: %s", str(json_response))
         errors = json_response.get("errors", None)
         if errors is not None:
             raise ConservatorGraphQLServerError(gql, errors)
 
         response = operation + json_response
 
         return response
@@ -186,36 +195,38 @@
         """
 
         tries = 0
 
         while True:
             try:
                 return self._query(query, fields, **kwargs)
-            except ConservatorGraphQLServerError as e:
-                exception = e.errors[0].get("exception", None)
+            except ConservatorGraphQLServerError as graphql_error:
+                exception = graphql_error.errors[0].get("exception", None)
                 if exception is None:
                     # This is a graphql error sent by the server.
                     # The query shouldn't be retried.
                     raise
 
                 # Otherwise we had an error due to connection. We should retry.
                 # (see _log_http_error in sgqlc/endpoint/http.py)
                 tries += 1
                 if tries > self.config.max_retries:
                     raise
-                logger.warning("Retrying request after exception: " + str(e))
-                logger.warning("Retry #" + str(tries))
+                logger.warning(
+                    "Retrying request after exception: %s", str(graphql_error)
+                )
+                logger.warning("Retry #%s", str(tries))
 
     def _query(self, query, fields, **kwargs):
         type_ = query.type
-        op = Operation(query.container)
+        gql_op = Operation(query.container)
         query_name = query.name
-        query = getattr(op, query_name)
+        query = getattr(gql_op, query_name)
         query(**kwargs)
 
-        fr = FieldsRequest.create(fields)
-        fr.prepare_query(query)
+        field_req = FieldsRequest.create(fields)
+        field_req.prepare_query(query)
 
-        result = self.run(op)
+        result = self.run(gql_op)
         value = getattr(result, query_name)
 
         return TypeProxy.wrap(self, type_, value)
```

### Comparing `conservator-cli-2.9.0/FLIR/conservator/conservator.py` & `conservator-cli-2.9.1/FLIR/conservator/conservator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# pylint: disable=missing-module-docstring
+# pylint: disable=broad-except
+# pylint: disable=unnecessary-pass
 import logging
 import random
 import re
 import time
 
 from FLIR.conservator.config import Config
 from FLIR.conservator.connection import ConservatorConnection
@@ -42,15 +45,15 @@
         self.files = ConservatorFileTransfers(self)
         self.collections = CollectionManager(self)
         self.datasets = DatasetManager(self)
         self.projects = ProjectManager(self)
         self.videos = VideoManager(self)
         self.images = ImageManager(self)
         self.media = MediaTypeManager(self)
-        logger.debug(f"Created new Conservator with config '{config}'")
+        logger.debug("Created new Conservator with config '%s'", config)
 
     def __repr__(self):
         return f"<Conservator at {self.config.url}>"
 
     def get_user(self):
         """Returns the User that the provided API token authorizes"""
         return self.query(Query.user)
@@ -64,35 +67,54 @@
         """
         Generate a new ID.
 
         The ID consists of ``ID_LENGTH`` characters from the ``ID_CHARSET``.
         The beginning of the ID is based on the current time, and the remaining
         characters are random.
         """
-        t = time.time()
-        time_digits = base_convert(Conservator.ID_CHARSET_SIZE, t)[::-1]
+        now = time.time()
+        time_digits = base_convert(Conservator.ID_CHARSET_SIZE, now)[::-1]
         id_ = [Conservator.ID_CHARSET[i] for i in time_digits]
         remaining_digits = Conservator.ID_LENGTH - len(id_)
         id_ += random.sample(Conservator.ID_CHARSET, remaining_digits)
         return "".join(id_)
 
     @staticmethod
     def is_valid_id(id_):
+        """
+        Validate that the supplied ID is valid
+        """
         return re.fullmatch(
             r"^[23456789ABCDEFGHJKLMNPQRSTWXYZabcdefghijkmnopqrstuvwxyz]{17}$", id_
         )
 
     @staticmethod
     def default(save=True):
         """
         Returns a :class:`Conservator` using :meth:`Config.default() <FLIR.conservator.config.Config.default>`.
         """
         return Conservator(Config.default(save=save))
 
     @staticmethod
+    def from_config_dict(config_dict):
+        """
+        Returns a :class:`Conservator` using a config constructed from
+        the supplied dict
+        """
+        conservator = None
+        try:
+            conservator = Conservator(Config.from_dict(config_dict))
+        except AttributeError:
+            raise RuntimeError(
+                "Could not connect using the supplied parameters!"
+            ) from None
+
+        return conservator
+
+    @staticmethod
     def create(config_name=None, save=True):
         """
         Returns a :class:`Conservator` using named config if given, and otherwise
         creates a default instance via `Conservator.default()`.
         """
         conservator = None
         if config_name:
```

### Comparing `conservator-cli-2.9.0/FLIR/conservator/fields_manager.py` & `conservator-cli-2.9.1/FLIR/conservator/fields_manager.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/fields_request.py` & `conservator-cli-2.9.1/FLIR/conservator/fields_request.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/file_transfers.py` & `conservator-cli-2.9.1/FLIR/conservator/file_transfers.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/generated/schema.py` & `conservator-cli-2.9.1/FLIR/conservator/generated/schema.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/local_dataset.py` & `conservator-cli-2.9.1/FLIR/conservator/local_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         logger.debug("Using cache at %s", self.cache_path)
 
         if not os.path.exists(self.cvc_path):
             os.makedirs(self.cvc_path)
         if not os.path.exists(self.staging_path):
             with open(self.staging_path, "w+", encoding="UTF-8") as staging_file:
                 json.dump([], staging_file)
+        if not os.path.exists(self.cache_path):
+            os.makedirs(self.cache_path)
         logger.debug("Opened local dataset at %s", self.path)
 
     def pull(self, verbose=True):
         """
         Pulls the latest repository state.
 
         :param verbose: If False, run git commands with the `-q` option.
```

### Comparing `conservator-cli-2.9.0/FLIR/conservator/managers/__init__.py` & `conservator-cli-2.9.1/FLIR/conservator/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/managers/media.py` & `conservator-cli-2.9.1/FLIR/conservator/managers/media.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/managers/searchable.py` & `conservator-cli-2.9.1/FLIR/conservator/managers/searchable.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/managers/type_manager.py` & `conservator-cli-2.9.1/FLIR/conservator/managers/type_manager.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/paginated_query.py` & `conservator-cli-2.9.1/FLIR/conservator/paginated_query.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/util.py` & `conservator-cli-2.9.1/FLIR/conservator/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-function-docstring
 import hashlib
 import logging
+import os
 import platform
 import sys
 
+from pathlib import Path
 from itertools import zip_longest
 
 import semver
 import requests
 
 from FLIR.conservator.version import version as cli_ver
 
@@ -62,15 +64,15 @@
     while n:
         r = int(n % b)
         output.append(r)
         n = int(n / b)
     return output
 
 
-def chunks(list, size):
+def chunks(list_to_chunk, chunk_size):
     """
     Simple one-line function to divide a list of items into chunks
     of a specified size.
 
     Once the input list is exhausted, the last list in the output
     iterator will be padded by None's to make up the size difference.
 
@@ -81,21 +83,21 @@
     :Example:
 
     chunks(['a', 'b', 'c'], 2) will return an iterator containing
     ['a', 'b'] and ['c', None]
 
     .. note:: Adapted from  https://stackoverflow.com/a/312644
     """
-    return zip_longest(*[iter(list)] * size, fillvalue=None)
+    return zip_longest(*[iter(list_to_chunk)] * chunk_size, fillvalue=None)
 
 
 def get_conservator_cli_version():
     # Get latest version from PyPi programatically
     # See https://stackoverflow.com/a/62571316
-    response = requests.get("https://pypi.org/pypi/conservator-cli/json")
+    response = requests.get("https://pypi.org/pypi/conservator-cli/json", timeout=10)
     return response.json()["info"]["version"]
 
 
 def compare_conservator_cli_version():
     current_version = semver.VersionInfo.parse(cli_ver)
     latest_version = semver.VersionInfo.parse(get_conservator_cli_version())
 
@@ -125,7 +127,15 @@
 
     if current_platform.lower() == "windows":
         print("Conservator-CLI is currently only supported on Windows through WSL.")
         print(
             "Please see https://flir.github.io/conservator-cli/usage/installation.html#installation-on-windows for details"
         )
         sys.exit(1)
+
+
+def check_dir_access(path_to_check):
+    if os.path.exists(path_to_check):
+        return os.access(path_to_check, os.W_OK)
+    else:
+        parent_path = Path(path_to_check).parent
+        return os.access(parent_path, os.W_OK)
```

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/__init__.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/collection.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/collection.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/dataset.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/dataset.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/dataset_frame.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/dataset_frame.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/file_locker.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/file_locker.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/frame.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/frame.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/image.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/image.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/media.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/media.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/metadata.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/metadata.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/project.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/project.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/queryable.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/queryable.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/type_proxy.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/type_proxy.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/FLIR/conservator/wrappers/video.py` & `conservator-cli-2.9.1/FLIR/conservator/wrappers/video.py`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/LICENSE` & `conservator-cli-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/PKG-INFO` & `conservator-cli-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conservator-cli
-Version: 2.9.0
+Version: 2.9.1
 Summary: A library for using the Teledyne FLIR Conservator API, with a nice command line interface.
 Home-page: https://github.com/FLIR/conservator-cli
 Author: Teledyne FLIR LLC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `conservator-cli-2.9.0/README.md` & `conservator-cli-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/conservator_cli.egg-info/PKG-INFO` & `conservator-cli-2.9.1/conservator_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conservator-cli
-Version: 2.9.0
+Version: 2.9.1
 Summary: A library for using the Teledyne FLIR Conservator API, with a nice command line interface.
 Home-page: https://github.com/FLIR/conservator-cli
 Author: Teledyne FLIR LLC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `conservator-cli-2.9.0/conservator_cli.egg-info/SOURCES.txt` & `conservator-cli-2.9.1/conservator_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conservator-cli-2.9.0/setup.py` & `conservator-cli-2.9.1/setup.py`

 * *Files identical despite different names*

