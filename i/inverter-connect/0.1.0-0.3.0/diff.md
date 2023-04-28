# Comparing `tmp/inverter-connect-0.1.0.tar.gz` & `tmp/inverter-connect-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.1.0.tar", last modified: Thu Apr 27 17:09:26 2023, max compression
+gzip compressed data, was "inverter-connect-0.3.0.tar", last modified: Fri Apr 28 07:06:43 2023, max compression
```

## Comparing `inverter-connect-0.1.0.tar` & `inverter-connect-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.1.0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.1.0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.377880 inverter-connect-0.1.0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-19 06:56:31.000000 inverter-connect-0.1.0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.1.0/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     9457 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     9043 2023-04-27 16:51:26.000000 inverter-connect-0.1.0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-04-20 19:23:05.000000 inverter-connect-0.1.0/cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.377880 inverter-connect-0.1.0/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      148 2023-04-27 16:57:57.000000 inverter-connect-0.1.0/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.1.0/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3753 2023-04-27 16:10:03.000000 inverter-connect-0.1.0/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    17570 2023-04-27 17:05:44.000000 inverter-connect-0.1.0/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)      276 2023-04-23 15:55:16.000000 inverter-connect-0.1.0/inverter/config.py
--rw-rw-r--   0 jens      (1000) users      (100)     8893 2023-04-27 16:18:50.000000 inverter-connect-0.1.0/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      261 2023-04-27 15:55:08.000000 inverter-connect-0.1.0/inverter/constants.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.1.0/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2784 2023-04-23 17:17:07.000000 inverter-connect-0.1.0/inverter/definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      429 2023-04-27 16:18:39.000000 inverter-connect-0.1.0/inverter/exceptions.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/test_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/test_doctests.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/utilities/string_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     2460 2023-04-24 09:00:54.000000 inverter-connect-0.1.0/inverter/publish_loop.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.1.0/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3262 2023-04-24 15:18:26.000000 inverter-connect-0.1.0/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-27 15:42:06.000000 inverter-connect-0.1.0/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     1452 2023-04-23 17:17:07.000000 inverter-connect-0.1.0/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2314 2023-04-20 19:36:47.000000 inverter-connect-0.1.0/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2135 2023-04-21 06:50:23.000000 inverter-connect-0.1.0/inverter/tests/test_readme.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.1.0/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      458 2023-04-27 17:06:47.000000 inverter-connect-0.1.0/inverter/utilities/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.1.0/inverter/utilities/credentials.py
--rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.1.0/inverter/utilities/log_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.1.0/inverter/utilities/modbus_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     9457 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1544 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       52 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      259 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4731 2023-04-27 15:42:09.000000 inverter-connect-0.1.0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    50591 2023-04-27 17:07:50.000000 inverter-connect-0.1.0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     5305 2023-04-27 17:07:31.000000 inverter-connect-0.1.0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.3.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.3.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.902163 inverter-connect-0.3.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.902163 inverter-connect-0.3.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-19 06:56:31.000000 inverter-connect-0.3.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.3.0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)    11263 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    10849 2023-04-28 07:05:23.000000 inverter-connect-0.3.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-04-20 19:23:05.000000 inverter-connect-0.3.0/cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.902163 inverter-connect-0.3.0/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.3.0/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.3.0/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.902163 inverter-connect-0.3.0/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.902163 inverter-connect-0.3.0/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.3.0/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.3.0/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      148 2023-04-28 06:50:48.000000 inverter-connect-0.3.0/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.3.0/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3753 2023-04-27 16:10:03.000000 inverter-connect-0.3.0/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.902163 inverter-connect-0.3.0/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.3.0/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    18250 2023-04-28 06:48:54.000000 inverter-connect-0.3.0/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)      276 2023-04-23 15:55:16.000000 inverter-connect-0.3.0/inverter/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)     9131 2023-04-28 05:57:27.000000 inverter-connect-0.3.0/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      261 2023-04-27 15:55:08.000000 inverter-connect-0.3.0/inverter/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.3.0/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2784 2023-04-23 17:17:07.000000 inverter-connect-0.3.0/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      429 2023-04-27 16:18:39.000000 inverter-connect-0.3.0/inverter/exceptions.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/inverter/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/inverter/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/tests/test_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/tests/test_doctests.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/inverter/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.3.0/inverter/mqtt4homeassistant/utilities/string_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2460 2023-04-24 09:00:54.000000 inverter-connect-0.3.0/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.3.0/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3262 2023-04-24 15:18:26.000000 inverter-connect-0.3.0/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-27 15:42:06.000000 inverter-connect-0.3.0/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1452 2023-04-23 17:17:07.000000 inverter-connect-0.3.0/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.3.0/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2314 2023-04-20 19:36:47.000000 inverter-connect-0.3.0/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2557 2023-04-28 07:02:52.000000 inverter-connect-0.3.0/inverter/tests/test_readme.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.3.0/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1459 2023-04-28 06:47:09.000000 inverter-connect-0.3.0/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.3.0/inverter/utilities/credentials.py
+-rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.3.0/inverter/utilities/log_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.3.0/inverter/utilities/modbus_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    11263 2023-04-28 07:06:43.000000 inverter-connect-0.3.0/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1544 2023-04-28 07:06:43.000000 inverter-connect-0.3.0/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-04-28 07:06:43.000000 inverter-connect-0.3.0/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       52 2023-04-28 07:06:43.000000 inverter-connect-0.3.0/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      259 2023-04-28 07:06:43.000000 inverter-connect-0.3.0/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-04-28 07:06:43.000000 inverter-connect-0.3.0/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4731 2023-04-27 15:42:09.000000 inverter-connect-0.3.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    50591 2023-04-27 17:07:50.000000 inverter-connect-0.3.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     5305 2023-04-27 17:07:31.000000 inverter-connect-0.3.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-04-28 07:06:43.906163 inverter-connect-0.3.0/setup.cfg
```

### Comparing `inverter-connect-0.1.0/.github/workflows/tests.yml` & `inverter-connect-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/PKG-INFO` & `inverter-connect-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,21 @@
-Metadata-Version: 2.1
-Name: inverter-connect
-Version: 0.1.0
-Summary: Get information from Deye Microinverter
-Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
-License: GPL-3.0-or-later
-Project-URL: Documentation, https://github.com/jedie/inverter-connect
-Project-URL: Source, https://github.com/jedie/inverter-connect
-Requires-Python: <4,>=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
-## screenshots
-
-Example output of `print-values` call:
-
-![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-21_08-53.png "2023-04-21_08-53.png")
-
-----
-
-Example output of `print-at-commands` call:
-
-![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-21_08-52.png "2023-04-21_08-52.png")
-
-----
-
 
-## quickstart
+# quickstart
 
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
 ~$ cd inverter-connect
@@ -80,18 +54,18 @@
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
-### most important commands
+# most important commands
 
 
-#### print-values
+## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
 
@@ -103,16 +77,22 @@
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
+Example output of `print-values` call:
+
+![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
+
+----
+
 
-#### print-at-commands
+## print-at-commands
 
 Help from `./cli.py print-at-commands --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
 
@@ -129,24 +109,61 @@
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
+Example output of `print-at-commands` call:
+
+![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
+
+----
+
+
+## read-register
+
+Help from `./cli.py read-register --help` Looks like:
+
+[comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
+```
+Usage: ./cli.py read-register [OPTIONS] IP REGISTER LENGTH
+
+ Read register(s) from the inverter
+ e.g.: read 3 registers starting from 0x16:
+ .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
+ e.g.: read the first 32 registers:
+ .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
+ The start address can be pass as decimal number or as hex string, e.g.: 0x123
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
+│                                                       [default: 48899; 1000<=x<=65535]           │
+│ --debug/--no-debug                                    [default: debug]                           │
+│ --help                                                Show this message and exit.                │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
+
+Example output of `read-register` call:
+
+![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
+
+----
+
 
-## credits
+# credits
 
 Others before me have done good work. In particular, I have learned a lot from the following projects:
 
 * https://github.com/s10l/deye-logger-at-cmd
 * https://github.com/kbialek/deye-inverter-mqtt
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
-## various links
+# various links
 
 * Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.1.0/README.md` & `inverter-connect-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
+Metadata-Version: 2.1
+Name: inverter-connect
+Version: 0.3.0
+Summary: Get information from Deye Microinverter
+Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://github.com/jedie/inverter-connect
+Project-URL: Source, https://github.com/jedie/inverter-connect
+Requires-Python: <4,>=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
-## screenshots
-
-Example output of `print-values` call:
-
-![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-21_08-53.png "2023-04-21_08-53.png")
-
-----
-
-Example output of `print-at-commands` call:
-
-![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-21_08-52.png "2023-04-21_08-52.png")
-
-----
-
 
-## quickstart
+# quickstart
 
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
 ~$ cd inverter-connect
@@ -68,18 +66,18 @@
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
-### most important commands
+# most important commands
 
 
-#### print-values
+## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
 
@@ -91,16 +89,22 @@
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
+Example output of `print-values` call:
+
+![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
+
+----
+
 
-#### print-at-commands
+## print-at-commands
 
 Help from `./cli.py print-at-commands --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
 
@@ -117,24 +121,61 @@
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
+Example output of `print-at-commands` call:
+
+![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
+
+----
+
+
+## read-register
+
+Help from `./cli.py read-register --help` Looks like:
+
+[comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
+```
+Usage: ./cli.py read-register [OPTIONS] IP REGISTER LENGTH
+
+ Read register(s) from the inverter
+ e.g.: read 3 registers starting from 0x16:
+ .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
+ e.g.: read the first 32 registers:
+ .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
+ The start address can be pass as decimal number or as hex string, e.g.: 0x123
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
+│                                                       [default: 48899; 1000<=x<=65535]           │
+│ --debug/--no-debug                                    [default: debug]                           │
+│ --help                                                Show this message and exit.                │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
+
+Example output of `read-register` call:
+
+![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
+
+----
+
 
-## credits
+# credits
 
 Others before me have done good work. In particular, I have learned a lot from the following projects:
 
 * https://github.com/s10l/deye-logger-at-cmd
 * https://github.com/kbialek/deye-inverter-mqtt
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
-## various links
+# various links
 
 * Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.1.0/cli.py` & `inverter-connect-0.3.0/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/.github/workflows/tests.yml` & `inverter-connect-0.3.0/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/api.py` & `inverter-connect-0.3.0/inverter/api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/cli/cli_app.py` & `inverter-connect-0.3.0/inverter/cli/cli_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import getpass
 import logging
 import sys
+import time
 from pathlib import Path
 
 import rich_click as click
 from bx_py_utils.path import assert_is_file
 from manageprojects.utilities import code_style
 from manageprojects.utilities.publish import publish_package
 from manageprojects.utilities.subprocess_utils import verbose_check_call
@@ -21,15 +22,15 @@
 from inverter.connection import InverterInfo, InverterSock, ModbusResponse
 from inverter.constants import ERROR_STR_NO_DATA
 from inverter.definitions import Parameter
 from inverter.exceptions import ModbusNoData, ModbusNoHexData
 from inverter.mqtt4homeassistant.data_classes import MqttSettings
 from inverter.mqtt4homeassistant.mqtt import get_connected_client
 from inverter.publish_loop import publish_forever
-from inverter.utilities.cli import convert_address_option
+from inverter.utilities.cli import convert_address_option, print_hex_table
 from inverter.utilities.credentials import get_mqtt_settings, store_mqtt_settings
 from inverter.utilities.log_setup import basic_log_setup
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -420,19 +421,24 @@
 
 
 @click.command()
 @click.argument('ip')
 @click.option(
     '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
 )
-@click.option('--register', default="0x22", help='Start address', show_default=True)
+@click.option('--register', default="0x16", help='Start address', show_default=True)
 @click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
 def set_time(ip, port, register, debug):
     """
     Set current date time in the inverter device.
+
+    Default start address is 0x16, so that this will be filled:
+        0x16 - year + month
+        0x17 - day + hour
+        0x18 - minute + second
     """
     address = convert_address_option(raw_address=register, debug=debug)
 
     config = Config(yaml_filename=None, host=ip, port=port, debug=debug)
     if debug:
         print(config)
 
@@ -447,14 +453,19 @@
             256 * (now.year % 100) + now.month,
             256 * now.day + now.hour,
             256 * now.minute + now.second,
         ]
         data = inv_sock.write(address=address, values=values)
         print(f'Response: {data!r}')
 
+        print('\nCheck time by request "AT+NTPTM"', end='...')
+        time.sleep(1)
+        result: str = inv_sock.cleaned_at_command(command='NTPTM')
+        print(f'[green]{result}')
+
 
 cli.add_command(set_time)
 
 
 @click.command()
 @click.argument('ip')
 @click.option(
@@ -463,21 +474,25 @@
 @click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
 @click.argument('register')
 @click.argument('length', type=click.IntRange(1, 100))
 def read_register(ip, port, register, length, debug):
     """
     Read register(s) from the inverter
 
-    e.g.: read the first 32 bytes:
+    e.g.: read 3 registers starting from 0x16:
+
+        .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
+
+    e.g.: read the first 32 registers:
 
     .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
 
     The start address can be pass as decimal number or as hex string, e.g.: 0x123
     """
-    print(f'Read {length} value(s) from {register=!r} ({ip}:{port})')
+    print(f'Read {length} register(s) from {register=!r} ({ip}:{port})')
     address = convert_address_option(raw_address=register, debug=debug)
 
     config = Config(yaml_filename=None, host=ip, port=port, debug=debug)
     if debug:
         print(config)
 
     with InverterSock(config) as inv_sock:
@@ -489,16 +504,21 @@
             response: ModbusResponse = inv_sock.read(start_register=address, length=length)
         except ModbusNoHexData as err:
             print(f'[yellow]Non hex response: [magenta]{err.data!r}')
         except ModbusNoData:
             print('[yellow]no data')
         else:
             print(response)
-            print()
-            print(f'Result (in hex): [cyan]{response.data_hex}')
+            print(f'\nResult (in hex): [cyan]{response.data_hex}\n')
+
+            print_hex_table(
+                address=address,
+                data_hex=response.data_hex,
+                title=f'[green][bold]{length} value(s) from {hex(address)}',
+            )
 
 
 cli.add_command(read_register)
 
 
 ######################################################################################################
 # MQTT
```

### Comparing `inverter-connect-0.1.0/inverter/connection.py` & `inverter-connect-0.3.0/inverter/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import dataclasses
 import logging
 import socket
 import time
 
+from rich import print  # noqa
+
 from inverter.config import Config
 from inverter.constants import AT_READ_FUNC_NUMBER, AT_WRITE_FUNC_NUMBER, ERROR_STR_NO_DATA
 from inverter.definitions import Parameter
 from inverter.exceptions import CrcError, ModbusNoData, ModbusNoHexData, ParseModbusValueError, ReadTimeout
 
 
 logger = logging.getLogger(__name__)
@@ -185,22 +187,29 @@
 
     def recv_command(self, *, command: bytes, buffer_size=1024):
         self.send(command=command)
 
         if self.config.debug:
             print('recv', end='...', flush=True)
 
-        try:
-            data = self.sock.recv(buffer_size)
-        except TimeoutError as err:
-            raise ReadTimeout(f'Get no response from {self.config.host}: {err}')
-        if self.config.debug:
-            print(f'{data}', flush=True)
+        for try_count in range(3):
+            try:
+                data = self.sock.recv(buffer_size)
+            except TimeoutError as err:
+                print(err)
+                print('[yellow]retry...')
+                time.sleep(0.25)
+                continue
+            else:
+                if self.config.debug:
+                    print(f'{data}', flush=True)
+
+                return data
 
-        return data
+        raise ReadTimeout(f'Get no response from {self.config.host}')
 
     def at_command(self, command: str, buffer_size=1024):
         assert not command.startswith('AT+'), f'Remove "AT+" prefix from: {command=}'
         assert not command.endswith('\n'), f'Line ending found in: {command=}'
         command = f'AT+{command}\n'.encode()
         return self.recv_command(command=command, buffer_size=buffer_size)
```

### Comparing `inverter-connect-0.1.0/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.3.0/inverter/definitions/deye_2mppt.yaml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/definitions.py` & `inverter-connect-0.3.0/inverter/definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/mqtt4homeassistant/converter.py` & `inverter-connect-0.3.0/inverter/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/mqtt4homeassistant/data_classes.py` & `inverter-connect-0.3.0/inverter/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/mqtt4homeassistant/mqtt.py` & `inverter-connect-0.3.0/inverter/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/test_converter.py` & `inverter-connect-0.3.0/inverter/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/publish_loop.py` & `inverter-connect-0.3.0/inverter/publish_loop.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/tests/test_api.py` & `inverter-connect-0.3.0/inverter/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/tests/test_connect.py` & `inverter-connect-0.3.0/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/tests/test_definitions.py` & `inverter-connect-0.3.0/inverter/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/tests/test_project_setup.py` & `inverter-connect-0.3.0/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/tests/test_readme.py` & `inverter-connect-0.3.0/inverter/tests/test_readme.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,7 +54,19 @@
             parts=(
                 'Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...',
                 '--port',
                 '--debug/--no-debug',
             ),
         )
         assert_cli_help_in_readme(text_block=stdout, marker='print-at-commands help')
+
+    def test_read_register(self):
+        stdout = invoke_click(cli, 'read-register', '--help')
+        self.assert_in_content(
+            got=stdout,
+            parts=(
+                'Usage: ./cli.py read-register [OPTIONS] IP REGISTER LENGTH',
+                '--port',
+                '--debug/--no-debug',
+            ),
+        )
+        assert_cli_help_in_readme(text_block=stdout, marker='read-register help')
```

### Comparing `inverter-connect-0.1.0/inverter/utilities/credentials.py` & `inverter-connect-0.3.0/inverter/utilities/credentials.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter/utilities/modbus_converter.py` & `inverter-connect-0.3.0/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.3.0/inverter_connect.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.1.0
+Version: 0.3.0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -18,30 +18,16 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
-## screenshots
-
-Example output of `print-values` call:
-
-![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-21_08-53.png "2023-04-21_08-53.png")
-
-----
-
-Example output of `print-at-commands` call:
-
-![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-21_08-52.png "2023-04-21_08-52.png")
-
-----
 
-
-## quickstart
+# quickstart
 
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
 ~$ cd inverter-connect
@@ -80,18 +66,18 @@
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
-### most important commands
+# most important commands
 
 
-#### print-values
+## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
 
@@ -103,16 +89,22 @@
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
+Example output of `print-values` call:
+
+![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
+
+----
 
-#### print-at-commands
+
+## print-at-commands
 
 Help from `./cli.py print-at-commands --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
 
@@ -129,24 +121,61 @@
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
+Example output of `print-at-commands` call:
+
+![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
+
+----
+
+
+## read-register
+
+Help from `./cli.py read-register --help` Looks like:
+
+[comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
+```
+Usage: ./cli.py read-register [OPTIONS] IP REGISTER LENGTH
+
+ Read register(s) from the inverter
+ e.g.: read 3 registers starting from 0x16:
+ .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
+ e.g.: read the first 32 registers:
+ .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
+ The start address can be pass as decimal number or as hex string, e.g.: 0x123
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
+│                                                       [default: 48899; 1000<=x<=65535]           │
+│ --debug/--no-debug                                    [default: debug]                           │
+│ --help                                                Show this message and exit.                │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
+
+Example output of `read-register` call:
+
+![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
+
+----
+
 
-## credits
+# credits
 
 Others before me have done good work. In particular, I have learned a lot from the following projects:
 
 * https://github.com/s10l/deye-logger-at-cmd
 * https://github.com/kbialek/deye-inverter-mqtt
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
-## various links
+# various links
 
 * Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.1.0/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.3.0/inverter_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/pyproject.toml` & `inverter-connect-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/requirements.dev.txt` & `inverter-connect-0.3.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.1.0/requirements.txt` & `inverter-connect-0.3.0/requirements.txt`

 * *Files identical despite different names*

