# Comparing `tmp/runfalcon-build-tools-1.2.0.tar.gz` & `tmp/runfalcon-build-tools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runfalcon-build-tools-1.2.0.tar", last modified: Wed Apr 26 21:49:10 2023, max compression
+gzip compressed data, was "runfalcon-build-tools-1.3.1.tar", last modified: Thu Apr 27 23:17:38 2023, max compression
```

## Comparing `runfalcon-build-tools-1.2.0.tar` & `runfalcon-build-tools-1.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-26 21:49:10.226674 runfalcon-build-tools-1.2.0/
--rw-r--r--   0 raul.devilla   (501) staff       (20)      553 2022-08-19 17:01:36.000000 runfalcon-build-tools-1.2.0/LICENCE
--rw-r--r--   0 raul.devilla   (501) staff       (20)     3405 2023-04-26 21:49:10.226804 runfalcon-build-tools-1.2.0/PKG-INFO
--rw-r--r--   0 raul.devilla   (501) staff       (20)     2895 2022-12-20 13:30:47.000000 runfalcon-build-tools-1.2.0/README.md
--rw-r--r--   0 raul.devilla   (501) staff       (20)      155 2022-09-13 19:21:44.000000 runfalcon-build-tools-1.2.0/pyproject.toml
--rw-r--r--   0 raul.devilla   (501) staff       (20)      712 2023-04-26 21:49:10.227170 runfalcon-build-tools-1.2.0/setup.cfg
-drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-26 21:49:10.212264 runfalcon-build-tools-1.2.0/src/
-drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-26 21:49:10.214087 runfalcon-build-tools-1.2.0/src/runfalcon_build_tools.egg-info/
--rw-r--r--   0 raul.devilla   (501) staff       (20)     3405 2023-04-26 21:49:10.000000 runfalcon-build-tools-1.2.0/src/runfalcon_build_tools.egg-info/PKG-INFO
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1623 2023-04-26 21:49:10.000000 runfalcon-build-tools-1.2.0/src/runfalcon_build_tools.egg-info/SOURCES.txt
--rw-r--r--   0 raul.devilla   (501) staff       (20)        1 2023-04-26 21:49:10.000000 runfalcon-build-tools-1.2.0/src/runfalcon_build_tools.egg-info/dependency_links.txt
--rw-r--r--   0 raul.devilla   (501) staff       (20)       20 2023-04-26 21:49:10.000000 runfalcon-build-tools-1.2.0/src/runfalcon_build_tools.egg-info/top_level.txt
-drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-26 21:49:10.221973 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/
--rw-r--r--   0 raul.devilla   (501) staff       (20)     2371 2022-12-20 15:41:47.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/__init__.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      173 2022-09-05 16:52:57.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/__main__.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1013 2022-09-15 02:18:53.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/app_builder.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     5959 2022-10-19 19:59:16.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/artifacts.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     8782 2022-10-20 18:00:41.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/aws_client.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     3283 2022-09-28 22:45:40.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/base_builder.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1843 2022-09-28 14:02:40.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/command_line_executor.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     3393 2022-12-07 15:03:47.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/config_files_helper.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1539 2022-09-02 20:01:50.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_base.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1582 2022-09-28 15:33:24.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_image_builder.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     2218 2022-09-20 15:10:22.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_image_tagger.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      451 2022-08-23 22:53:15.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_options.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1130 2022-09-20 15:10:26.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_tagger.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      176 2022-08-19 21:50:31.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/env_utils.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      420 2022-08-24 22:31:32.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/environment_helper.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     2453 2023-04-26 21:45:22.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/file_utils.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      570 2022-09-21 02:22:13.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/keys_helper.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1082 2022-10-19 21:26:22.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/logger.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)    10863 2022-12-20 16:30:13.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/main_module.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      873 2022-09-20 15:10:30.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/nodejs_typescript_builder.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     3329 2022-09-13 19:22:27.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/properties.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1978 2022-10-19 21:26:59.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/repository_helper.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      550 2022-12-20 16:29:56.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/ssl_certificate_manager.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      197 2022-09-14 16:58:21.000000 runfalcon-build-tools-1.2.0/src/runfalconbuildtools/string_util.py
-drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-26 21:49:10.226343 runfalcon-build-tools-1.2.0/tests/
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1547 2022-09-21 03:09:22.000000 runfalcon-build-tools-1.2.0/tests/test_functional_main.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      847 2022-10-19 20:00:25.000000 runfalcon-build-tools-1.2.0/tests/test_integration_artifacts.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1659 2022-10-19 19:58:30.000000 runfalcon-build-tools-1.2.0/tests/test_integration_aws_client.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      451 2022-08-31 15:52:15.000000 runfalcon-build-tools-1.2.0/tests/test_integration_builder.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1275 2022-09-14 17:01:53.000000 runfalcon-build-tools-1.2.0/tests/test_integration_config_file_helper.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1077 2022-08-31 15:52:40.000000 runfalcon-build-tools-1.2.0/tests/test_integration_docker_image_builder.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      689 2022-12-20 16:32:23.000000 runfalcon-build-tools-1.2.0/tests/test_integration_ssl_certificate_manager.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1134 2022-09-28 13:55:11.000000 runfalcon-build-tools-1.2.0/tests/test_unit_command_line_executor.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      922 2022-08-31 15:52:49.000000 runfalcon-build-tools-1.2.0/tests/test_unit_evironment_helper.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      857 2022-09-22 00:13:03.000000 runfalcon-build-tools-1.2.0/tests/test_unit_file_utils.py
+drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-27 23:17:38.014511 runfalcon-build-tools-1.3.1/
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      553 2022-08-19 17:01:36.000000 runfalcon-build-tools-1.3.1/LICENCE
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     3405 2023-04-27 23:17:38.014599 runfalcon-build-tools-1.3.1/PKG-INFO
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     2895 2022-12-20 13:30:47.000000 runfalcon-build-tools-1.3.1/README.md
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      155 2022-09-13 19:21:44.000000 runfalcon-build-tools-1.3.1/pyproject.toml
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      712 2023-04-27 23:17:38.014907 runfalcon-build-tools-1.3.1/setup.cfg
+drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-27 23:17:38.004080 runfalcon-build-tools-1.3.1/src/
+drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-27 23:17:38.005665 runfalcon-build-tools-1.3.1/src/runfalcon_build_tools.egg-info/
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     3405 2023-04-27 23:17:37.000000 runfalcon-build-tools-1.3.1/src/runfalcon_build_tools.egg-info/PKG-INFO
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1623 2023-04-27 23:17:38.000000 runfalcon-build-tools-1.3.1/src/runfalcon_build_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 raul.devilla   (501) staff       (20)        1 2023-04-27 23:17:37.000000 runfalcon-build-tools-1.3.1/src/runfalcon_build_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 raul.devilla   (501) staff       (20)       20 2023-04-27 23:17:37.000000 runfalcon-build-tools-1.3.1/src/runfalcon_build_tools.egg-info/top_level.txt
+drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-27 23:17:38.011962 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     2371 2022-12-20 15:41:47.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/__init__.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      173 2022-09-05 16:52:57.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/__main__.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1013 2022-09-15 02:18:53.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/app_builder.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     5959 2022-10-19 19:59:16.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/artifacts.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     8782 2022-10-20 18:00:41.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/aws_client.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     3283 2022-09-28 22:45:40.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/base_builder.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1843 2022-09-28 14:02:40.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/command_line_executor.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     3393 2022-12-07 15:03:47.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/config_files_helper.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1539 2022-09-02 20:01:50.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_base.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1582 2022-09-28 15:33:24.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_image_builder.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     2218 2022-09-20 15:10:22.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_image_tagger.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      451 2022-08-23 22:53:15.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_options.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1130 2022-09-20 15:10:26.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_tagger.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      176 2022-08-19 21:50:31.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/env_utils.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      420 2022-08-24 22:31:32.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/environment_helper.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     2624 2023-04-27 22:46:48.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/file_utils.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      570 2022-09-21 02:22:13.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/keys_helper.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1082 2022-10-19 21:26:22.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/logger.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)    10863 2022-12-20 16:30:13.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/main_module.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      873 2022-09-20 15:10:30.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/nodejs_typescript_builder.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     3329 2022-09-13 19:22:27.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/properties.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1978 2022-10-19 21:26:59.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/repository_helper.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      550 2022-12-20 16:29:56.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/ssl_certificate_manager.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      197 2022-09-14 16:58:21.000000 runfalcon-build-tools-1.3.1/src/runfalconbuildtools/string_util.py
+drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-04-27 23:17:38.014298 runfalcon-build-tools-1.3.1/tests/
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1547 2022-09-21 03:09:22.000000 runfalcon-build-tools-1.3.1/tests/test_functional_main.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      847 2022-10-19 20:00:25.000000 runfalcon-build-tools-1.3.1/tests/test_integration_artifacts.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1659 2022-10-19 19:58:30.000000 runfalcon-build-tools-1.3.1/tests/test_integration_aws_client.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      451 2022-08-31 15:52:15.000000 runfalcon-build-tools-1.3.1/tests/test_integration_builder.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1275 2022-09-14 17:01:53.000000 runfalcon-build-tools-1.3.1/tests/test_integration_config_file_helper.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1077 2022-08-31 15:52:40.000000 runfalcon-build-tools-1.3.1/tests/test_integration_docker_image_builder.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      689 2022-12-20 16:32:23.000000 runfalcon-build-tools-1.3.1/tests/test_integration_ssl_certificate_manager.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1134 2022-09-28 13:55:11.000000 runfalcon-build-tools-1.3.1/tests/test_unit_command_line_executor.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      922 2022-08-31 15:52:49.000000 runfalcon-build-tools-1.3.1/tests/test_unit_evironment_helper.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      857 2022-09-22 00:13:03.000000 runfalcon-build-tools-1.3.1/tests/test_unit_file_utils.py
```

### Comparing `runfalcon-build-tools-1.2.0/LICENCE` & `runfalcon-build-tools-1.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/PKG-INFO` & `runfalcon-build-tools-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runfalcon-build-tools
-Version: 1.2.0
+Version: 1.3.1
 Summary: Runfalcon tools to build process with quality and efficiency
 Home-page: https://git-codecommit.zone.amazonaws.com/v1/repos/runfalcon-build-tools-py-package
 Author: Raul A. de Villa C.
 Author-email: r@runfalcon.com
 Project-URL: Bug Tracker, https://no-yet
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `runfalcon-build-tools-1.2.0/README.md` & `runfalcon-build-tools-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/setup.cfg` & `runfalcon-build-tools-1.3.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = runfalcon-build-tools
-version = 1.2.0
+version = 1.3.1
 author = Raul A. de Villa C.
 author_email = r@runfalcon.com
 description = Runfalcon tools to build process with quality and efficiency
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://git-codecommit.zone.amazonaws.com/v1/repos/runfalcon-build-tools-py-package
 project_urls =
```

### Comparing `runfalcon-build-tools-1.2.0/src/runfalcon_build_tools.egg-info/PKG-INFO` & `runfalcon-build-tools-1.3.1/src/runfalcon_build_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runfalcon-build-tools
-Version: 1.2.0
+Version: 1.3.1
 Summary: Runfalcon tools to build process with quality and efficiency
 Home-page: https://git-codecommit.zone.amazonaws.com/v1/repos/runfalcon-build-tools-py-package
 Author: Raul A. de Villa C.
 Author-email: r@runfalcon.com
 Project-URL: Bug Tracker, https://no-yet
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `runfalcon-build-tools-1.2.0/src/runfalcon_build_tools.egg-info/SOURCES.txt` & `runfalcon-build-tools-1.3.1/src/runfalcon_build_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/__init__.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/__init__.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/app_builder.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/app_builder.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/artifacts.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/artifacts.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/aws_client.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/aws_client.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/base_builder.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/base_builder.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/command_line_executor.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/command_line_executor.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/config_files_helper.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/config_files_helper.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_base.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_base.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_image_builder.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_image_builder.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_image_tagger.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_image_tagger.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/docker_tagger.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/docker_tagger.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/file_utils.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/file_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,15 +60,20 @@
 def get_runfalcon_tmp_file(ext:str = 'tmp'):
     tmp_dir:str = get_runfalcon_tmp_dir()
     file_name:str = tmp_dir + '/' + 'rf-' + get_random_string(15) + '.' + ext
     touch(file_name)
     return file_name
 
 def copy_file(source:str, target:str):
-    shutil.copy(source, target)
+    if not os.path.samefile(source, target):
+        try:
+            shutil.copy2(source, target)
+        except Exception as e:
+            if str(e).find('SameFileError') < 0:
+                raise e
 
 def move_file(source:str, target:str):
     if file_exists(target):
         delete_file(target)
     shutil.move(source, target)
 
 def get_simple_file_name(full_file_name:str) -> str:
```

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/keys_helper.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/keys_helper.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/logger.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/logger.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/main_module.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/main_module.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/nodejs_typescript_builder.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/nodejs_typescript_builder.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/properties.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/properties.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/repository_helper.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/repository_helper.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/src/runfalconbuildtools/ssl_certificate_manager.py` & `runfalcon-build-tools-1.3.1/src/runfalconbuildtools/ssl_certificate_manager.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_functional_main.py` & `runfalcon-build-tools-1.3.1/tests/test_functional_main.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_integration_artifacts.py` & `runfalcon-build-tools-1.3.1/tests/test_integration_artifacts.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_integration_aws_client.py` & `runfalcon-build-tools-1.3.1/tests/test_integration_aws_client.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_integration_config_file_helper.py` & `runfalcon-build-tools-1.3.1/tests/test_integration_config_file_helper.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_integration_docker_image_builder.py` & `runfalcon-build-tools-1.3.1/tests/test_integration_docker_image_builder.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_integration_ssl_certificate_manager.py` & `runfalcon-build-tools-1.3.1/tests/test_integration_ssl_certificate_manager.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_unit_command_line_executor.py` & `runfalcon-build-tools-1.3.1/tests/test_unit_command_line_executor.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_unit_evironment_helper.py` & `runfalcon-build-tools-1.3.1/tests/test_unit_evironment_helper.py`

 * *Files identical despite different names*

### Comparing `runfalcon-build-tools-1.2.0/tests/test_unit_file_utils.py` & `runfalcon-build-tools-1.3.1/tests/test_unit_file_utils.py`

 * *Files identical despite different names*

