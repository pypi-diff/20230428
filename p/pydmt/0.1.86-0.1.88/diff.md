# Comparing `tmp/pydmt-0.1.86.tar.gz` & `tmp/pydmt-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmt-0.1.86.tar", last modified: Fri Apr 28 17:21:50 2023, max compression
+gzip compressed data, was "pydmt-0.1.88.tar", last modified: Fri Apr 28 20:04:10 2023, max compression
```

## Comparing `pydmt-0.1.86.tar` & `pydmt-0.1.88.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.911301 pydmt-0.1.86/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-28 17:21:12.000000 pydmt-0.1.86/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-28 17:21:50.911301 pydmt-0.1.86/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      391 2023-04-28 17:21:12.000000 pydmt-0.1.86/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.907301 pydmt-0.1.86/pydmt/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.86/pydmt/__init__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.907301 pydmt-0.1.86/pydmt/api/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.86/pydmt/api/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.1.86/pydmt/api/builder.py
--rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.1.86/pydmt/api/copy.py
--rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.1.86/pydmt/api/fail.py
--rw-r--r--   0 mark      (1000) mark      (1000)      613 2020-09-20 14:25:08.000000 pydmt-0.1.86/pydmt/api/feature.py
--rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.1.86/pydmt/api/one_source_one_target.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.908301 pydmt-0.1.86/pydmt/builders/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.86/pydmt/builders/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.1.86/pydmt/builders/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      428 2023-04-21 14:45:52.000000 pydmt-0.1.86/pydmt/builders/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.1.86/pydmt/builders/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.1.86/pydmt/builders/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1390 2022-10-15 00:29:42.000000 pydmt-0.1.86/pydmt/builders/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.1.86/pydmt/builders/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1663 2023-04-27 11:13:11.000000 pydmt-0.1.86/pydmt/builders/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1584 2023-04-21 14:45:35.000000 pydmt-0.1.86/pydmt/builders/venv_full.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.1.86/pydmt/builders/yaml.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2927 2023-04-28 17:19:24.000000 pydmt-0.1.86/pydmt/configs.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.909301 pydmt-0.1.86/pydmt/core/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.86/pydmt/core/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.1.86/pydmt/core/cache.py
--rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.1.86/pydmt/core/graph.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.1.86/pydmt/core/pydmt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.1.86/pydmt/core/tempdir.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.909301 pydmt-0.1.86/pydmt/features/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.86/pydmt/features/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.1.86/pydmt/features/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.1.86/pydmt/features/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1422 2022-05-04 08:25:10.000000 pydmt-0.1.86/pydmt/features/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.1.86/pydmt/features/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.1.86/pydmt/features/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.1.86/pydmt/features/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)      392 2022-05-09 05:06:11.000000 pydmt-0.1.86/pydmt/features/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)      325 2022-05-09 04:57:20.000000 pydmt-0.1.86/pydmt/features/venv_full.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1010 2022-05-04 08:23:35.000000 pydmt-0.1.86/pydmt/features/yaml.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.910301 pydmt-0.1.86/pydmt/helpers/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.1.86/pydmt/helpers/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.1.86/pydmt/helpers/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      129 2022-05-16 19:51:40.000000 pydmt-0.1.86/pydmt/helpers/composites.py
--rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.1.86/pydmt/helpers/deb.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.1.86/pydmt/helpers/deb_python_package.py
--rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.1.86/pydmt/helpers/files.py
--rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.1.86/pydmt/helpers/general.py
--rw-r--r--   0 mark      (1000) mark      (1000)      313 2022-06-25 06:56:24.000000 pydmt-0.1.86/pydmt/helpers/git.py
--rw-r--r--   0 mark      (1000) mark      (1000)      465 2022-05-19 21:23:46.000000 pydmt-0.1.86/pydmt/helpers/github.py
--rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.1.86/pydmt/helpers/messages.py
--rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.1.86/pydmt/helpers/misc.py
--rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.1.86/pydmt/helpers/pkgs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-28 04:28:36.000000 pydmt-0.1.86/pydmt/helpers/project.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4895 2023-03-08 23:18:25.000000 pydmt-0.1.86/pydmt/helpers/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)      775 2022-05-19 21:09:23.000000 pydmt-0.1.86/pydmt/helpers/signature.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.1.86/pydmt/helpers/snipplets.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1333 2022-10-12 19:19:30.000000 pydmt-0.1.86/pydmt/helpers/urls.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4939 2023-04-28 17:20:40.000000 pydmt-0.1.86/pydmt/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      175 2023-04-28 17:21:12.000000 pydmt-0.1.86/pydmt/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.911301 pydmt-0.1.86/pydmt/utils/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.86/pydmt/utils/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.1.86/pydmt/utils/digest.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.1.86/pydmt/utils/digester.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.1.86/pydmt/utils/filesystem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.1.86/pydmt/utils/logging.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.1.86/pydmt/utils/php.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2822 2022-10-15 00:35:27.000000 pydmt-0.1.86/pydmt/utils/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1339 2023-04-24 05:56:18.000000 pydmt-0.1.86/pydmt/utils/subprocess.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 17:21:50.907301 pydmt-0.1.86/pydmt.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-28 17:21:50.000000 pydmt-0.1.86/pydmt.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     1602 2023-04-28 17:21:50.000000 pydmt-0.1.86/pydmt.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-28 17:21:50.000000 pydmt-0.1.86/pydmt.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       42 2023-04-28 17:21:50.000000 pydmt-0.1.86/pydmt.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       77 2023-04-28 17:21:50.000000 pydmt-0.1.86/pydmt.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2023-04-28 17:21:50.000000 pydmt-0.1.86/pydmt.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-28 17:21:50.911301 pydmt-0.1.86/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-28 17:21:12.000000 pydmt-0.1.86/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.470185 pydmt-0.1.88/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-28 20:03:48.000000 pydmt-0.1.88/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-28 20:04:10.470185 pydmt-0.1.88/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      391 2023-04-28 20:03:48.000000 pydmt-0.1.88/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.465185 pydmt-0.1.88/pydmt/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.88/pydmt/__init__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.466185 pydmt-0.1.88/pydmt/api/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.88/pydmt/api/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.1.88/pydmt/api/builder.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.1.88/pydmt/api/copy.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.1.88/pydmt/api/fail.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      613 2020-09-20 14:25:08.000000 pydmt-0.1.88/pydmt/api/feature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.1.88/pydmt/api/one_source_one_target.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.467185 pydmt-0.1.88/pydmt/builders/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.88/pydmt/builders/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.1.88/pydmt/builders/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      428 2023-04-21 14:45:52.000000 pydmt-0.1.88/pydmt/builders/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.1.88/pydmt/builders/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.1.88/pydmt/builders/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1390 2022-10-15 00:29:42.000000 pydmt-0.1.88/pydmt/builders/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.1.88/pydmt/builders/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1663 2023-04-27 11:13:11.000000 pydmt-0.1.88/pydmt/builders/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1584 2023-04-21 14:45:35.000000 pydmt-0.1.88/pydmt/builders/venv_full.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.1.88/pydmt/builders/yaml.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2930 2023-04-28 19:50:08.000000 pydmt-0.1.88/pydmt/configs.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.467185 pydmt-0.1.88/pydmt/core/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.88/pydmt/core/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.1.88/pydmt/core/cache.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.1.88/pydmt/core/graph.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.1.88/pydmt/core/pydmt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.1.88/pydmt/core/tempdir.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.468185 pydmt-0.1.88/pydmt/features/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.88/pydmt/features/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.1.88/pydmt/features/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.1.88/pydmt/features/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1422 2022-05-04 08:25:10.000000 pydmt-0.1.88/pydmt/features/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.1.88/pydmt/features/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.1.88/pydmt/features/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.1.88/pydmt/features/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      392 2022-05-09 05:06:11.000000 pydmt-0.1.88/pydmt/features/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      325 2022-05-09 04:57:20.000000 pydmt-0.1.88/pydmt/features/venv_full.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1010 2022-05-04 08:23:35.000000 pydmt-0.1.88/pydmt/features/yaml.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.470185 pydmt-0.1.88/pydmt/helpers/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.1.88/pydmt/helpers/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.1.88/pydmt/helpers/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      129 2022-05-16 19:51:40.000000 pydmt-0.1.88/pydmt/helpers/composites.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.1.88/pydmt/helpers/deb.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.1.88/pydmt/helpers/deb_python_package.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.1.88/pydmt/helpers/files.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.1.88/pydmt/helpers/general.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      313 2022-06-25 06:56:24.000000 pydmt-0.1.88/pydmt/helpers/git.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      212 2023-04-28 19:49:07.000000 pydmt-0.1.88/pydmt/helpers/github.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.1.88/pydmt/helpers/messages.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.1.88/pydmt/helpers/misc.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.1.88/pydmt/helpers/pkgs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-28 04:28:36.000000 pydmt-0.1.88/pydmt/helpers/project.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4782 2023-04-28 19:46:14.000000 pydmt-0.1.88/pydmt/helpers/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      775 2022-05-19 21:09:23.000000 pydmt-0.1.88/pydmt/helpers/signature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.1.88/pydmt/helpers/snipplets.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1337 2023-04-28 19:44:33.000000 pydmt-0.1.88/pydmt/helpers/urls.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4939 2023-04-28 17:20:40.000000 pydmt-0.1.88/pydmt/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      175 2023-04-28 20:03:48.000000 pydmt-0.1.88/pydmt/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.470185 pydmt-0.1.88/pydmt/utils/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.88/pydmt/utils/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.1.88/pydmt/utils/digest.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.1.88/pydmt/utils/digester.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.1.88/pydmt/utils/filesystem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.1.88/pydmt/utils/logging.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.1.88/pydmt/utils/php.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2822 2022-10-15 00:35:27.000000 pydmt-0.1.88/pydmt/utils/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1339 2023-04-24 05:56:18.000000 pydmt-0.1.88/pydmt/utils/subprocess.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 20:04:10.466185 pydmt-0.1.88/pydmt.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-28 20:04:10.000000 pydmt-0.1.88/pydmt.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     1602 2023-04-28 20:04:10.000000 pydmt-0.1.88/pydmt.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-28 20:04:10.000000 pydmt-0.1.88/pydmt.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       42 2023-04-28 20:04:10.000000 pydmt-0.1.88/pydmt.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       77 2023-04-28 20:04:10.000000 pydmt-0.1.88/pydmt.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2023-04-28 20:04:10.000000 pydmt-0.1.88/pydmt.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-28 20:04:10.471185 pydmt-0.1.88/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-28 20:03:48.000000 pydmt-0.1.88/setup.py
```

### Comparing `pydmt-0.1.86/LICENSE` & `pydmt-0.1.88/LICENSE`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/PKG-INFO` & `pydmt-0.1.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.1.86
+Version: 0.1.88
 Summary: Python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
 Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.1.86
+version: 0.1.88
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pydmt-0.1.86/pydmt/api/builder.py` & `pydmt-0.1.88/pydmt/api/builder.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/api/feature.py` & `pydmt-0.1.88/pydmt/api/feature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/api/one_source_one_target.py` & `pydmt-0.1.88/pydmt/api/one_source_one_target.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/builders/apt.py` & `pydmt-0.1.88/pydmt/builders/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/builders/mako.py` & `pydmt-0.1.88/pydmt/builders/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/builders/reqs.py` & `pydmt-0.1.88/pydmt/builders/reqs.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/builders/sphinx.py` & `pydmt-0.1.88/pydmt/builders/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/builders/venv.py` & `pydmt-0.1.88/pydmt/builders/venv.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/builders/venv_full.py` & `pydmt-0.1.88/pydmt/builders/venv_full.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/builders/yaml.py` & `pydmt-0.1.88/pydmt/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/configs.py` & `pydmt-0.1.88/pydmt/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,17 +103,17 @@
 
 class ConfigImport(Config):
     """
     Configure how to set PYTHONPATH
     """
     import_cwd = ParamCreator.create_bool(
         help_string="Add . to PYTHONPATH",
-        default=True,
+        default=False,
     )
     import_home = ParamCreator.create_bool(
         help_string="Add ~/.config/pydmt to PYTHONPATH",
-        default=True,
+        default=False,
     )
     import_system = ParamCreator.create_bool(
         help_string="Add /etc/pydmt to PYTHONPATH",
-        default=True,
+        default=False,
     )
```

### Comparing `pydmt-0.1.86/pydmt/core/cache.py` & `pydmt-0.1.88/pydmt/core/cache.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/core/pydmt.py` & `pydmt-0.1.88/pydmt/core/pydmt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/features/apt.py` & `pydmt-0.1.88/pydmt/features/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/features/mako.py` & `pydmt-0.1.88/pydmt/features/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/features/yaml.py` & `pydmt-0.1.88/pydmt/features/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/helpers/apt.py` & `pydmt-0.1.88/pydmt/helpers/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/helpers/deb.py` & `pydmt-0.1.88/pydmt/helpers/deb.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/helpers/deb_python_package.py` & `pydmt-0.1.88/pydmt/helpers/deb_python_package.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/helpers/python.py` & `pydmt-0.1.88/pydmt/helpers/python.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,17 +103,14 @@
     return os.path.basename(os.getcwd())
 
 
 def get_attr(attr: str):
     mod = importlib.import_module("config.python")
     if hasattr(mod, attr):
         return getattr(mod, attr)
-    mod = importlib.import_module("default.python")
-    if hasattr(mod, attr):
-        return getattr(mod, attr)
     # TODO: need a better exception type (make my own)
     raise ValueError(f"cannot find {attr}")
 
 
 def get_license_type():
     return get_attr("license_type")
```

### Comparing `pydmt-0.1.86/pydmt/helpers/signature.py` & `pydmt-0.1.88/pydmt/helpers/signature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/helpers/snipplets.py` & `pydmt-0.1.88/pydmt/helpers/snipplets.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/helpers/urls.py` & `pydmt-0.1.88/pydmt/helpers/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import importlib
 
 import pydmt.helpers.project
 
 
 def get_github_username():
-    mod = importlib.import_module("user.personal")
+    mod = importlib.import_module("config.personal")
     if hasattr(mod, "github_username"):
         return getattr(mod, "github_username")
     return os.getlogin()
 
 
 def get_launchpad_username():
-    mod = importlib.import_module("user.personal")
+    mod = importlib.import_module("config.personal")
     if hasattr(mod, "launchpad_username"):
         return getattr(mod, "launchpad_username")
     return os.getlogin()
 
 
 def get_website():
     github_username = get_github_username()
```

### Comparing `pydmt-0.1.86/pydmt/main.py` & `pydmt-0.1.88/pydmt/main.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/utils/digest.py` & `pydmt-0.1.88/pydmt/utils/digest.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/utils/digester.py` & `pydmt-0.1.88/pydmt/utils/digester.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/utils/filesystem.py` & `pydmt-0.1.88/pydmt/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/utils/python.py` & `pydmt-0.1.88/pydmt/utils/python.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt/utils/subprocess.py` & `pydmt-0.1.88/pydmt/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/pydmt.egg-info/PKG-INFO` & `pydmt-0.1.88/pydmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.1.86
+Version: 0.1.88
 Summary: Python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
 Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.1.86
+version: 0.1.88
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pydmt-0.1.86/pydmt.egg-info/SOURCES.txt` & `pydmt-0.1.88/pydmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.86/setup.py` & `pydmt-0.1.88/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pydmt",
-    version="0.1.86",
+    version="0.1.88",
     packages=[
         "pydmt",
         "pydmt.api",
         "pydmt.builders",
         "pydmt.core",
         "pydmt.features",
         "pydmt.helpers",
```

