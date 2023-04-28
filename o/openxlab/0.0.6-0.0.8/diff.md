# Comparing `tmp/openxlab-0.0.6.tar.gz` & `tmp/openxlab-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-0.0.6.tar", last modified: Tue Apr 25 10:30:41 2023, max compression
+gzip compressed data, was "openxlab-0.0.8.tar", last modified: Fri Apr 28 10:26:52 2023, max compression
```

## Comparing `openxlab-0.0.6.tar` & `openxlab-0.0.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.292377 openxlab-0.0.6/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:30:41.292100 openxlab-0.0.6/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.6/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.279630 openxlab-0.0.6/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.6/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.6/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.282048 openxlab-0.0.6/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.6/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-25 10:30:31.000000 openxlab-0.0.6/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.282350 openxlab-0.0.6/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.282729 openxlab-0.0.6/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      337 2023-04-24 11:33:14.000000 openxlab-0.0.6/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.283517 openxlab-0.0.6/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.6/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.6/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     5233 2023-04-25 09:47:26.000000 openxlab-0.0.6/openxlab/model/clients/openapi_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.286242 openxlab-0.0.6/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.6/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-04-24 10:01:11.000000 openxlab-0.0.6/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      861 2023-04-25 10:15:10.000000 openxlab-0.0.6/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.6/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-04-24 09:23:06.000000 openxlab-0.0.6/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-04-24 11:39:15.000000 openxlab-0.0.6/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      702 2023-04-24 11:39:15.000000 openxlab-0.0.6/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.6/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      752 2023-04-24 11:11:49.000000 openxlab-0.0.6/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.287330 openxlab-0.0.6/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.6/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1229 2023-04-25 09:26:21.000000 openxlab-0.0.6/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-04-24 09:23:06.000000 openxlab-0.0.6/openxlab/model/common/meta_file_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.6/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.290242 openxlab-0.0.6/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-04-24 09:23:06.000000 openxlab-0.0.6/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.6/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1285 2023-04-24 09:23:06.000000 openxlab-0.0.6/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2550 2023-04-25 10:29:48.000000 openxlab-0.0.6/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.6/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-04-24 11:33:14.000000 openxlab-0.0.6/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-04-24 11:39:15.000000 openxlab-0.0.6/openxlab/model/handler/query_repo_model.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1044 2023-04-24 11:28:18.000000 openxlab-0.0.6/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 openxlab-0.0.6/openxlab/model/handler/update_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1095 2023-04-24 11:05:26.000000 openxlab-0.0.6/openxlab/model/handler/update_repository.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.290726 openxlab-0.0.6/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.6/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.291400 openxlab-0.0.6/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/utils/file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.291707 openxlab-0.0.6/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.281462 openxlab-0.0.6/openxlab.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1487 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      107 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.6/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-25 10:30:41.292469 openxlab-0.0.6/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.6/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.226486 openxlab-0.0.8/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-28 10:26:52.226177 openxlab-0.0.8/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.8/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.200958 openxlab-0.0.8/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.8/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.8/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.204253 openxlab-0.0.8/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.8/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-28 10:26:12.000000 openxlab-0.0.8/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.204694 openxlab-0.0.8/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.205692 openxlab-0.0.8/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      391 2023-04-27 05:13:40.000000 openxlab-0.0.8/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.206914 openxlab-0.0.8/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.8/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.8/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     5272 2023-04-28 09:49:50.000000 openxlab-0.0.8/openxlab/model/clients/openapi_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.213664 openxlab-0.0.8/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.8/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-04-24 10:01:11.000000 openxlab-0.0.8/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      861 2023-04-25 10:15:10.000000 openxlab-0.0.8/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.8/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-04-24 09:23:06.000000 openxlab-0.0.8/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-04-24 11:39:15.000000 openxlab-0.0.8/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      702 2023-04-24 11:39:15.000000 openxlab-0.0.8/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1085 2023-04-27 05:56:30.000000 openxlab-0.0.8/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      752 2023-04-24 11:11:49.000000 openxlab-0.0.8/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.215809 openxlab-0.0.8/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.8/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1230 2023-04-28 09:57:07.000000 openxlab-0.0.8/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-04-24 09:23:06.000000 openxlab-0.0.8/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.8/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.222566 openxlab-0.0.8/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-04-24 09:23:06.000000 openxlab-0.0.8/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.8/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1285 2023-04-24 09:23:06.000000 openxlab-0.0.8/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2474 2023-04-28 09:56:29.000000 openxlab-0.0.8/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.8/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-04-24 11:33:14.000000 openxlab-0.0.8/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-04-24 11:39:15.000000 openxlab-0.0.8/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1044 2023-04-24 11:28:18.000000 openxlab-0.0.8/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1131 2023-04-27 06:01:17.000000 openxlab-0.0.8/openxlab/model/handler/update_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1095 2023-04-24 11:05:26.000000 openxlab-0.0.8/openxlab/model/handler/update_repository.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.223702 openxlab-0.0.8/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.8/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.224860 openxlab-0.0.8/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.225379 openxlab-0.0.8/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.203624 openxlab-0.0.8/openxlab.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1487 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       88 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.8/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-28 10:26:52.226591 openxlab-0.0.8/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.8/setup.py
```

### Comparing `openxlab-0.0.6/PKG-INFO` & `openxlab-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab
-Version: 0.0.6
+Version: 0.0.8
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-0.0.6/README.md` & `openxlab-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/cli.py` & `openxlab-0.0.8/openxlab/cli.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/demo_cmd/__init__.py` & `openxlab-0.0.8/openxlab/demo_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/clients/openapi_client.py` & `openxlab-0.0.8/openxlab/model/clients/openapi_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         path = paths['file_download_path']
         response_dto = self.http_post_response_dto(path, payload)
         if response_dto.msg_code != '10000':
             raise ValueError(f"Get download url error:{response_dto.msg}, traceId:{response_dto.trace_id}")
         if response_dto.data['msgCode'] != '10000':
             raise ValueError(f"Get download url error:{response_dto.data['msg']}, "
                              f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data['data']['url']
+        return response_dto.data['data']['url'], response_dto.data['data']['fileName']
 
     def get_metafile_template_download_url(self, file=None):
         """
         get metafile template download url
         """
         payload = {}
         path = paths['meta_file_template_download_path']
```

### Comparing `openxlab-0.0.6/openxlab/model/commands/__init__.py` & `openxlab-0.0.8/openxlab/model/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/commands/create.py` & `openxlab-0.0.8/openxlab/model/commands/create.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/commands/download.py` & `openxlab-0.0.8/openxlab/model/commands/download.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/commands/init.py` & `openxlab-0.0.8/openxlab/model/commands/init.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/commands/list.py` & `openxlab-0.0.8/openxlab/model/commands/list.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/commands/remove.py` & `openxlab-0.0.8/openxlab/model/commands/remove.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/commands/visibility.py` & `openxlab-0.0.8/openxlab/model/commands/visibility.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/common/constants.py` & `openxlab-0.0.8/openxlab/model/common/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
     'file_download_path': '/model-center/api/v1/cli/repository/getFileDownloadUrl',
     'meta_file_template_download_path': '/model-center/api/v1/cli/repository/getMetafileTemplateUrl',
     'create_repository_path': '/model-center/api/v1/cli/repository/createModelRepository',
     'update_repository_path': '/model-center/api/v1/cli/repository/updateRepositoryBaseInfo',
     'delete_repository_path': '/model-center/api/v1/cli/repository/deleteRepository',
     'query_models_path': '/model-center/api/v1/cli/repository/queryModels',
 }
-default_metafile_template_name = 'metafile.yml'
+default_metafile_template_name = 'metafile.yaml'
```

### Comparing `openxlab-0.0.6/openxlab/model/common/meta_file_util.py` & `openxlab-0.0.8/openxlab/model/common/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/common/response_dto.py` & `openxlab-0.0.8/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/handler/create_repository.py` & `openxlab-0.0.8/openxlab/model/handler/create_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/handler/download_file.py` & `openxlab-0.0.8/openxlab/model/handler/download_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,35 +18,35 @@
     download model file|meta file|log filee|readme file
     usage: cli & sdk
     """
     try:
         # split params
         username, repository = _split_repo(model_repo)
         client = OpenapiClient(endpoint, token)
-        url = client.get_download_url(repository, file)
+        url, file_name = client.get_download_url(repository, file)
     except ValueError as e:
         print(f"Error: {e}")
         return
-    path_file = _download_to_local(url, file, path)
-    print("download model repo:{}, file:{}".format(model_repo, file))
+    path_file = _download_to_local(url, file_name, path)
+    print("download model repo:{}, file_name:{}".format(model_repo, file_name))
     return path_file
 
 
 def download_metafile_template(path=None) -> None:
     """
     download metafile template file
     """
     try:
         # split params
         client = OpenapiClient(endpoint, token)
         url = client.get_metafile_template_download_url()
     except ValueError as e:
         print(f"Error: {e}")
         return
-    _download_to_local(url, file=default_metafile_template_name, path=path)
+    _download_to_local(url, file_name=default_metafile_template_name, path=path)
 
 
 def _split_repo(model_repo) -> (str, str):
     """
     Split a full repository name into two separate strings: the username and the repository name.
     """
     # username/repository format check
@@ -54,29 +54,27 @@
     if not re.match(pattern, model_repo):
         raise ValueError("The input string must be in the format 'didi12/test-d-1'")
 
     values = model_repo.split('/')
     return values[0], values[1]
 
 
-def _download_to_local(url, file, path=None) -> str:
+def _download_to_local(url, file_name, path=None) -> str:
     """
     download file to local with progress_bar
     """
-    filename = os.path.basename(url)
-    file_extension = os.path.splitext(filename)[1]
     response = requests.get(url, stream=True)
 
     total_size_in_bytes = int(response.headers.get('content-length', 0))
     block_size = 1024
     progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
-    path_file = file + file_extension
+    path_file = file_name
     if path is not None:
         if not os.path.exists(path):
             os.makedirs(path)
-        path_file = f"{path}/{file + file_extension}"
+        path_file = f"{path}/{file_name}"
     with open(path_file, 'wb') as f:
         for data in response.iter_content(block_size):
             progress_bar.update(len(data))
             f.write(data)
     progress_bar.close()
     return path_file
```

### Comparing `openxlab-0.0.6/openxlab/model/handler/query_repo_model.py` & `openxlab-0.0.8/openxlab/model/handler/query_repo_model.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/handler/remove_repo_or_file.py` & `openxlab-0.0.8/openxlab/model/handler/remove_repo_or_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/model/handler/update_repository.py` & `openxlab-0.0.8/openxlab/model/handler/update_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/types/command_type.py` & `openxlab-0.0.8/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab/utils/file.py` & `openxlab-0.0.8/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/openxlab.egg-info/PKG-INFO` & `openxlab-0.0.8/openxlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab
-Version: 0.0.6
+Version: 0.0.8
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-0.0.6/openxlab.egg-info/SOURCES.txt` & `openxlab-0.0.8/openxlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.6/setup.py` & `openxlab-0.0.8/setup.py`

 * *Files identical despite different names*

