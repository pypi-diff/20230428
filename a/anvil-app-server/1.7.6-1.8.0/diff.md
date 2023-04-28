# Comparing `tmp/anvil-app-server-1.7.6.tar.gz` & `tmp/anvil-app-server-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\anvil-app-server-1.7.6.tar", last modified: Thu Feb 16 13:16:55 2023, max compression
+gzip compressed data, was "anvil-app-server-1.8.0.tar", last modified: Fri Apr 28 14:19:42 2023, max compression
```

## Comparing `anvil-app-server-1.7.6.tar` & `anvil-app-server-1.8.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.929036 anvil-app-server-1.7.6/
--rw-rw-rw-   0        0        0     1145 2023-02-16 13:16:55.928036 anvil-app-server-1.7.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.826020 anvil-app-server-1.7.6/anvil_app_server/
--rw-rw-rw-   0        0        0    10039 2023-02-16 13:15:28.000000 anvil-app-server-1.7.6/anvil_app_server/Blank.zip
--rw-rw-rw-   0        0        0    10262 2023-02-16 13:15:28.000000 anvil-app-server-1.7.6/anvil_app_server/Default.zip
--rw-rw-rw-   0        0        0    12594 2023-02-16 13:15:28.000000 anvil-app-server-1.7.6/anvil_app_server/TodoList.zip
--rw-rw-rw-   0        0        0     7226 2023-02-16 13:15:28.000000 anvil-app-server-1.7.6/anvil_app_server/__init__.py
--rw-rw-rw-   0        0        0      742 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_app_server/shell.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.837938 anvil-app-server-1.7.6/anvil_app_server.egg-info/
--rw-rw-rw-   0        0        0     1145 2023-02-16 13:16:55.000000 anvil-app-server-1.7.6/anvil_app_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2847 2023-02-16 13:16:55.000000 anvil-app-server-1.7.6/anvil_app_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 13:16:55.000000 anvil-app-server-1.7.6/anvil_app_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-02-16 13:16:55.000000 anvil-app-server-1.7.6/anvil_app_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-02-16 13:16:55.000000 anvil-app-server-1.7.6/anvil_app_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       79 2023-02-16 13:16:55.000000 anvil-app-server-1.7.6/anvil_app_server.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.844022 anvil-app-server-1.7.6/anvil_downlink_host/
--rw-rw-rw-   0        0        0    20028 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_host/__init__.py
--rw-rw-rw-   0        0        0    17467 2022-07-27 12:46:48.000000 anvil-app-server-1.7.6/anvil_downlink_host/full_python.py
--rw-rw-rw-   0        0        0    15364 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_host/pdf_renderer.py
--rw-rw-rw-   0        0        0      100 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_host/run.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.848036 anvil-app-server-1.7.6/anvil_downlink_util/
--rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_util/__init__.py
--rw-rw-rw-   0        0        0     1501 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_util/pipes.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.856035 anvil-app-server-1.7.6/anvil_downlink_worker/
--rw-rw-rw-   0        0        0     8804 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.884036 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/
--rw-rw-rw-   0        0        0     4684 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/__init__.py
--rw-rw-rw-   0        0        0     2951 2023-02-15 09:50:29.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_components.py
--rw-rw-rw-   0        0        0     4143 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_form_templating.py
--rw-rw-rw-   0        0        0     4111 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_serialise.py
--rw-rw-rw-   0        0        0    56000 2023-02-16 13:11:03.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_server.py
--rw-rw-rw-   0        0        0    16093 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_threaded_server.py
--rw-rw-rw-   0        0        0    10975 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/email.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.887037 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/facebook/
--rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/facebook/__init__.py
--rw-rw-rw-   0        0        0      421 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/facebook/auth.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.889035 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/files/
--rw-rw-rw-   0        0        0    12369 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.896034 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/
--rw-rw-rw-   0        0        0      181 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/__init__.py
--rw-rw-rw-   0        0        0      621 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/auth.py
--rw-rw-rw-   0        0        0    21821 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/drive.py
--rw-rw-rw-   0        0        0     1435 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/mail.py
--rw-rw-rw-   0        0        0    13576 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/sheets.py
--rw-rw-rw-   0        0        0     3631 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/http.py
--rw-rw-rw-   0        0        0      339 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/js.py
--rw-rw-rw-   0        0        0     1638 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/media.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.900036 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/microsoft/
--rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/microsoft/__init__.py
--rw-rw-rw-   0        0        0      688 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/microsoft/auth.py
--rw-rw-rw-   0        0        0      698 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/mpl_util.py
--rw-rw-rw-   0        0        0     3512 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/pdf.py
--rw-rw-rw-   0        0        0       86 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/regex.py
--rw-rw-rw-   0        0        0      944 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/secrets.py
--rw-rw-rw-   0        0        0    10549 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/server.py
--rw-rw-rw-   0        0        0     2075 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/stripe.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.908035 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/
--rw-rw-rw-   0        0        0     9740 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/__init__.py
--rw-rw-rw-   0        0        0      898 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/_base_classes.py
--rw-rw-rw-   0        0        0      308 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/_config.py
--rw-rw-rw-   0        0        0     1039 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/_errors.py
--rw-rw-rw-   0        0        0      428 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/_helpers.py
--rw-rw-rw-   0        0        0     5160 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/query.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.922037 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/
--rw-rw-rw-   0        0        0      231 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/__init__.py
--rw-rw-rw-   0        0        0     1183 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_app_tables.py
--rw-rw-rw-   0        0        0     2105 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_batcher.py
--rw-rw-rw-   0        0        0      845 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_constants.py
--rw-rw-rw-   0        0        0      284 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_load_hacks.py
--rw-rw-rw-   0        0        0     1211 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_refs.py
--rw-rw-rw-   0        0        0    20029 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_row.py
--rw-rw-rw-   0        0        0     9461 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_search.py
--rw-rw-rw-   0        0        0     4339 2022-07-26 14:31:31.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_table.py
--rw-rw-rw-   0        0        0     4668 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_utils.py
--rw-rw-rw-   0        0        0     1964 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tz.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.926036 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/
--rw-rw-rw-   0        0        0    39409 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/__init__.py
--rw-rw-rw-   0        0        0      205 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/config.py
--rw-rw-rw-   0        0        0      979 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-16 13:16:55.927035 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/mfa/
--rw-rw-rw-   0        0        0    18907 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/mfa/__init__.py
--rw-rw-rw-   0        0        0     2525 2022-07-08 11:06:55.000000 anvil-app-server-1.7.6/anvil_downlink_worker/anvil/util.py
--rw-rw-rw-   0        0        0       49 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/exec2.py
--rw-rw-rw-   0        0        0       15 2022-07-08 11:06:57.000000 anvil-app-server-1.7.6/anvil_downlink_worker/exec3.py
--rw-rw-rw-   0        0        0     3464 2023-01-26 14:34:47.000000 anvil-app-server-1.7.6/anvil_downlink_worker/full_python_worker.py
--rw-rw-rw-   0        0        0       42 2023-02-16 13:16:55.929036 anvil-app-server-1.7.6/setup.cfg
--rw-rw-rw-   0        0        0     1813 2023-02-16 13:15:28.000000 anvil-app-server-1.7.6/setup.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1121 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/PKG-INFO
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_app_server/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    10039 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/anvil_app_server/Blank.zip
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    10262 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/anvil_app_server/Default.zip
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    12594 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/anvil_app_server/TodoList.zip
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     7226 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/anvil_app_server/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      742 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_app_server/shell.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_app_server.egg-info/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1121 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/PKG-INFO
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2847 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)        1 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      155 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/entry_points.txt
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       55 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/requires.txt
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       79 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/top_level.txt
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_host/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    20028 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_host/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    17467 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_host/full_python.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    15364 2022-06-08 12:52:10.000000 anvil-app-server-1.8.0/anvil_downlink_host/pdf_renderer.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      100 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_host/run.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_util/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)        0 2021-10-08 13:19:20.000000 anvil-app-server-1.8.0/anvil_downlink_util/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1501 2021-10-08 13:19:20.000000 anvil-app-server-1.8.0/anvil_downlink_util/pipes.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     8804 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/__init__.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4684 2022-05-19 09:15:03.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2951 2023-04-26 21:52:21.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_components.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4143 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_form_templating.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4111 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_serialise.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    56083 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_server.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    16093 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_threaded_server.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    10975 2022-05-24 19:01:05.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/email.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/facebook/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)        0 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/facebook/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      421 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/facebook/auth.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/files/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    12369 2023-01-03 13:49:28.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/files/__init__.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      181 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      621 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/auth.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    21821 2023-01-03 13:49:28.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/drive.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1435 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/mail.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    13576 2022-12-19 17:36:19.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/sheets.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4137 2023-04-20 21:39:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/http.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      339 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/js.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1638 2022-12-19 17:36:19.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/media.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/microsoft/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)        0 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/microsoft/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      688 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/microsoft/auth.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      693 2023-03-03 12:04:38.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/mpl_util.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     3512 2023-01-03 13:49:28.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/pdf.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       86 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/regex.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      944 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/secrets.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    10549 2023-02-06 10:21:14.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/server.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2075 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/stripe.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     9866 2023-04-12 13:59:51.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      898 2022-05-19 09:15:03.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_base_classes.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      308 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_config.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1039 2022-12-19 17:40:31.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_errors.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      428 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_helpers.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     5160 2022-06-19 19:43:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/query.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      231 2022-05-19 09:15:03.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1183 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_app_tables.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2105 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_batcher.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      845 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_constants.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      284 2022-05-19 09:15:03.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_load_hacks.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1211 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_refs.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    20172 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_row.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     9520 2023-04-12 13:59:51.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_search.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4398 2023-04-12 13:59:51.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_table.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4668 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_utils.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1964 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tz.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    39409 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      205 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/config.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      979 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/exceptions.py
+drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/mfa/
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    18907 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/mfa/__init__.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2525 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/util.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       49 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/exec2.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       15 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/exec3.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     3464 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/full_python_worker.py
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       38 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/setup.cfg
+-rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1812 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/setup.py
```

### Comparing `anvil-app-server-1.7.6/PKG-INFO` & `anvil-app-server-1.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: anvil-app-server
-Version: 1.7.6
-Summary: A standalone server for Anvil full-stack Python web apps
-Home-page: https://anvil.works
-Author: Anvil
-Author-email: contact@anvil.works
-License: GNU Affero General Public License v3
-Project-URL: Source Code, https://github.com/anvil-works/anvil-runtime
-Description: 
-        ## A standalone server for Anvil full-stack Python web apps.
-        
-        This package includes several assets, some not in Python:
-         - The "anvil-standalone-runtime" script for launching the runtime
-         - The "downlink" Python code for the server-side parts of apps
-         - The core Anvil server (requires Java to launch)
-         - The client-side Anvil runtime (Javascript, using the Skulpt Python-to-JS compiler)
-        
-        Head over to [the Github Repository](https://github.com/anvil-works/anvil-runtime) for usage instructions, and to learn more.
-            
-Keywords: anvil web apps standalone browser Python
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: anvil-app-server
+Version: 1.8.0
+Summary: A standalone server for Anvil full-stack Python web apps
+Home-page: https://anvil.works
+Author: Anvil
+Author-email: contact@anvil.works
+License: GNU Affero General Public License v3
+Project-URL: Source Code, https://github.com/anvil-works/anvil-runtime
+Description: 
+        ## A standalone server for Anvil full-stack Python web apps.
+        
+        This package includes several assets, some not in Python:
+         - The "anvil-standalone-runtime" script for launching the runtime
+         - The "downlink" Python code for the server-side parts of apps
+         - The core Anvil server (requires Java to launch)
+         - The client-side Anvil runtime (Javascript, using the Skulpt Python-to-JS compiler)
+        
+        Head over to [the Github Repository](https://github.com/anvil-works/anvil-runtime) for usage instructions, and to learn more.
+            
+Keywords: anvil web apps standalone browser Python
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Description-Content-Type: text/markdown
```

### Comparing `anvil-app-server-1.7.6/anvil_app_server/__init__.py` & `anvil-app-server-1.8.0/anvil_app_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         print("psql 'host=localhost port={} user=postgres dbname=postgres options=--search-path=app_tables'".format(port))
         os.system("psql 'host=localhost port={} user=postgres dbname=postgres options=--search-path=app_tables'".format(port))
 
 
 def find_or_download_app_server(): # Work out whether we already have the server JAR file. It could be in the package itself, or in ~/.anvil
     package_dir = os.path.dirname(__file__)
     home_dir = os.path.expanduser("~")
-    server_jar_name = "anvil-app-server.20230216-131528.jar"
+    server_jar_name = "anvil-app-server.20230428-151654.jar"
 
     package_dir_path = os.path.join(package_dir, server_jar_name)
     home_dir_path = os.path.join(home_dir, ".anvil", server_jar_name)
 
     if os.path.isfile(package_dir_path):
         print("Found Anvil App Server JAR in package directory")
         return package_dir_path
```

### Comparing `anvil-app-server-1.7.6/anvil_app_server/shell.py` & `anvil-app-server-1.8.0/anvil_app_server/shell.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_app_server.egg-info/PKG-INFO` & `anvil-app-server-1.8.0/anvil_app_server.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: anvil-app-server
-Version: 1.7.6
-Summary: A standalone server for Anvil full-stack Python web apps
-Home-page: https://anvil.works
-Author: Anvil
-Author-email: contact@anvil.works
-License: GNU Affero General Public License v3
-Project-URL: Source Code, https://github.com/anvil-works/anvil-runtime
-Description: 
-        ## A standalone server for Anvil full-stack Python web apps.
-        
-        This package includes several assets, some not in Python:
-         - The "anvil-standalone-runtime" script for launching the runtime
-         - The "downlink" Python code for the server-side parts of apps
-         - The core Anvil server (requires Java to launch)
-         - The client-side Anvil runtime (Javascript, using the Skulpt Python-to-JS compiler)
-        
-        Head over to [the Github Repository](https://github.com/anvil-works/anvil-runtime) for usage instructions, and to learn more.
-            
-Keywords: anvil web apps standalone browser Python
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: anvil-app-server
+Version: 1.8.0
+Summary: A standalone server for Anvil full-stack Python web apps
+Home-page: https://anvil.works
+Author: Anvil
+Author-email: contact@anvil.works
+License: GNU Affero General Public License v3
+Project-URL: Source Code, https://github.com/anvil-works/anvil-runtime
+Description: 
+        ## A standalone server for Anvil full-stack Python web apps.
+        
+        This package includes several assets, some not in Python:
+         - The "anvil-standalone-runtime" script for launching the runtime
+         - The "downlink" Python code for the server-side parts of apps
+         - The core Anvil server (requires Java to launch)
+         - The client-side Anvil runtime (Javascript, using the Skulpt Python-to-JS compiler)
+        
+        Head over to [the Github Repository](https://github.com/anvil-works/anvil-runtime) for usage instructions, and to learn more.
+            
+Keywords: anvil web apps standalone browser Python
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Description-Content-Type: text/markdown
```

### Comparing `anvil-app-server-1.7.6/anvil_app_server.egg-info/SOURCES.txt` & `anvil-app-server-1.8.0/anvil_app_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_host/__init__.py` & `anvil-app-server-1.8.0/anvil_downlink_host/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_host/full_python.py` & `anvil-app-server-1.8.0/anvil_downlink_host/full_python.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_host/pdf_renderer.py` & `anvil-app-server-1.8.0/anvil_downlink_host/pdf_renderer.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_util/pipes.py` & `anvil-app-server-1.8.0/anvil_downlink_util/pipes.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/__init__.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/__init__.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_components.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_components.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_form_templating.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_form_templating.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_serialise.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_serialise.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_server.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,19 +497,23 @@
             self.error_obj = {"message": str(message), "trace": []}
             t = type(self).registered_type_name
             if t is not None:
                 self.error_obj["type"] = t
         self.message = self.error_obj.get("message", "")
         Exception.__init__(self, self.message)
 
-    def __str__(self):
+    def __repr__(self):
+        r = Exception.__repr__(self)
+        if type(self) is not AnvilWrappedError:
+            return r
         eo_type = self.error_obj.get("type")
-        if type(self) is AnvilWrappedError and eo_type is not None:
-            return str(eo_type) + ": " + repr(self.message)
-        return repr(self.message)
+        if eo_type is None:
+            return r
+
+        return "AnvilWrappedError" + "(" + eo_type + r[len("AnvilWrappedError"):] + ")"
 
 
 def augment_exception(exc_class):
     def f(error_obj):
         e = exc_class(error_obj['message'])
         e._anvil_error_obj = error_obj
         return e
```

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/_threaded_server.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_threaded_server.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/email.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/email.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/files/__init__.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/files/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/auth.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/auth.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/drive.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/drive.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/mail.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/mail.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/google/sheets.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/sheets.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/http.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,29 @@
 
 
 anvil.server._register_exception_type("anvil.http.HttpRequestFailed", HttpRequestFailed)
 
 def _has_content(method):
     return method != "GET" and method != "HEAD"
 
-#!defFunction(anvil.http,_,url,[method="GET"],[data=None],[json=False],[headers=None],[username=None],[password=None], [timeout=None])!2: "Make an HTTP request to the specified URL.\n\nIf json=True, the response is parsed into Python objects (dicts/lists/etc), and 'data' is JSON-encoded before sending.\n\n'headers' can be a dict of strings to set HTTP headers.\nIf specified, 'username' and 'password' will be used to perform HTTP Basic authentication." ["request"]
+#!defFunction(anvil.http,_,url,[method="GET"],[data=None],[json=False],[headers=None],[username=None],[password=None],[timeout=None])!2: 
+# {
+#   $doc: "Make an HTTP request to the specified URL.",
+#   anvil$helpLink: "/docs/http-apis/making-http-requests",
+#   anvil$args: {
+#     url: "The request will be made to this URL.",
+#     method: "The HTTP method. Defaults to 'GET'.",
+#     data: "The data to send in the request body",
+#     json: "If set to True, the response is parsed into Python objects (dicts/lists/etc), and ‘data’ is JSON-encoded before sending. If False, the response will be a Media object.",
+#     headers: "A dict of strings to set HTTP headers",
+#     username: "If specified, used to perform HTTP Basic authentication",
+#     password: "If specified, used to perform HTTP Basic authentication",
+#     timeout: "An int or float representing the amount of time, in seconds, to wait for a response. Default is 60 seconds.",
+#   } 
+# }["request"]
 def request(url, method='GET', data=None, headers=None, username=None, password=None, json=False, timeout=None):
     method = str(method).upper()
 
     if headers is None:
         headers = {}
     if json and data is not None and _has_content(method):
         data = json_mod.dumps(data)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/media.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/media.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/microsoft/auth.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/microsoft/auth.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/mpl_util.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/mpl_util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import anvil
 import io
 
 
 #!defFunction(anvil.mpl_util,anvil.Media instance,[dpi=],[facecolor=],[edgecolor=],[format=],[transparent=],[frameon=],[bbox_inches=],[pad_inches=],[filename=])!2: "Return the current Matplotlib figure as an PNG image. Returns an Anvil Media object that can be displayed in Image components.\n\nOptional arguments have the same meaning as for 'savefig()'" ["plot_image"]
-def plot_image(format='png', transparent=True, **kwargs):
+def plot_image(format='png', transparent=True, filename="plot.png", **kwargs):
   with io.BytesIO() as buf:
     plt.savefig(buf, format=format, transparent=transparent, **kwargs)
     buf.seek(0)    
-    return anvil.BlobMedia('image/png', buf.read(), name=kwargs.get("filename", "plot.png"))
+    return anvil.BlobMedia('image/png', buf.read(), name=filename)
```

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/pdf.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/pdf.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/secrets.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/secrets.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/server.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/server.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/stripe.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/stripe.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/__init__.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -215,18 +215,18 @@
 #!defMethod(client writable view)!2: "Return a view on this table that can be written by client code. Use keyword arguments to specify view restrictions." ["client_writable_cascade"]
 #!defMethod(_)!2: "Delete all the rows from the data table" ["delete_all_rows"]
 #!defMethod(_)!2: "Get a single matching row from the data table whose columns match the keyword arguments. Returns None if no matching row exists, and raises an exception if more than one row matches.\n\nEg: app_tables.table_1.get(name='John Smith')" ["get"]
 #!defMethod(row,id)!2: "Get the matching row from this data table, by its unique ID" ["get_by_id"]
 #!defMethod(bool,row)!2: "Returns true if the table (or view) contains the provided row." ["has_row"]
 #!defMethod(list of dicts)!2: "Get the spec for the table as a list of dicts. Each dict contains the name and type of a column." ["list_columns"]
 #!defMethod(Row or None)!2: "Get rows from a data table. If you specify keyword arguments, you will retrieve only rows whose columns match those values.\n\nEg: app_tables.table_1.search(name='John Smith')" ["search"]
-#!defMethod(Media object)!2: "Get the table in CSV format. Returns a downloadable Media object; use its url property." ["to_csv"]
+#!defMethod(Media object, [escape_for_excel=False])!2: "Get the table in CSV format, optionally escaped for use in Excel. Returns a downloadable Media object; use its url property." ["to_csv"]
 #!defClassNoConstructor(anvil.tables,#Table)!1: "A table returned from app_tables"
 
-#!defMethod(Media object)!2: "Get the results of the SearchIterator in CSV format. Returns a downloadable Media object; use its url property." ["to_csv"]
+#!defMethod(Media object, [escape_for_excel=False])!2: "Get the results of the SearchIterator in CSV format, optionally escaped for use in Excel. Returns a downloadable Media object; use its url property." ["to_csv"]
 #!defClassNoConstructor(anvil.tables,#SearchIterator)!1: "An iterator of table rows returned from a search()";
 
 
 #!defMethod(_)!2: "Delete the row from its data table" ["delete"]
 #!defMethod(id)!2: "Get the unique ID of the table row" ["get_id"]
 #!defMethod(_,**column_values)!2: "update the data for multiple columns" ["update"]
 #!defClassNoConstructor(anvil.tables,#Row)!1: "A table row";
```

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/_base_classes.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_base_classes.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/_errors.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_errors.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/query.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/query.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_app_tables.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_app_tables.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_batcher.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_batcher.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_constants.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_constants.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_refs.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_refs.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_row.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,14 +407,21 @@
     #     return self._id
 
     # TODO reinclude this api
     # @property
     # def table_id(self):
     #     return self._table_id
 
+    def get(self, key, default=None):
+        try:
+            return self[key]
+        except NoSuchColumnError:
+            return default
+
+
     def keys(self):
         if self._spec is None:
             # if we don't have a _spec we don't have any keys
             # but we don't need to blindly call _fill_uncached: UNCACHED values are fine
             self._fill_cache()
         return self._cache.keys()
```

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_search.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,16 +189,16 @@
         return True
 
     __nonzero__ = __bool__
 
     def refresh(self):
         self._clear_cache()
 
-    def to_csv(self):
-        return anvil.server.call(PREFIX + "to_csv", self._cap)
+    def to_csv(self, escape_for_excel=False):
+        return anvil.server.call(PREFIX + "to_csv", self._cap, escape_for_excel=escape_for_excel)
 
     def delete_all_rows(self):
         result = anvil.server.call(PREFIX + "delete_all", self._cap)
         self._clear_cache()
         return result
 
     def __getitem__(self, idx):
```

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_table.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,14 @@
         return anvil.server.call(PREFIX + "list_columns", self._cap)
 
     def search(self, *args, **kws):
         kws = make_refs(kws)
         row_ids, cap, cap_next, table_data = anvil.server.call(PREFIX + "search", self._cap, args, kws)
         return SearchIterator._create(self._view_key, self._id, row_ids, cap, cap_next, table_data)
 
-    def to_csv(self):
-        return anvil.server.call(PREFIX + "to_csv", self._cap)
+    def to_csv(self, escape_for_excel=False):
+        return anvil.server.call(PREFIX + "to_csv", self._cap, escape_for_excel=escape_for_excel)
 
     # TODO reinclude this API
     # @property
     # def id(self):
     #     return self._id
```

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tables/v2/_utils.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_utils.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/tz.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tz.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/__init__.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/exceptions.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/exceptions.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/users/mfa/__init__.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/mfa/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/anvil/util.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/util.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/anvil_downlink_worker/full_python_worker.py` & `anvil-app-server-1.8.0/anvil_downlink_worker/full_python_worker.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.7.6/setup.py` & `anvil-app-server-1.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_packages
 setup(
     name="anvil-app-server",
-    version="1.7.6",
+    version="1.8.0",
     packages=find_packages(),
-    install_requires=["pychrome", "anvil-uplink==0.3.42", "progressbar2", "wheel", "psutil"],
+    install_requires=["pychrome", "anvil-uplink==0.4.2", "progressbar2", "wheel", "psutil"],
 
     # Include the App Server JAR directly in this debug build of the package. That way the release version won't be downloaded on first run.
     package_data={
         "anvil_app_server": [
             "TodoList.zip",
             "Default.zip",
             "Blank.zip"
```

