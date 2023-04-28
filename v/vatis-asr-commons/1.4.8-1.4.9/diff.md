# Comparing `tmp/vatis_asr_commons-1.4.8.tar.gz` & `tmp/vatis_asr_commons-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vatis_asr_commons-1.4.8.tar", last modified: Sat Feb  4 10:24:01 2023, max compression
+gzip compressed data, was "dist/vatis_asr_commons-1.4.9.tar", last modified: Tue Feb 21 19:18:41 2023, max compression
```

## Comparing `vatis_asr_commons-1.4.8.tar` & `vatis_asr_commons-1.4.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/
--rw-r--r--   0 mac        (501) staff       (20)      601 2021-09-17 07:50:18.000000 vatis_asr_commons-1.4.8/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)       72 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      931 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      845 2023-01-21 11:08:04.000000 vatis_asr_commons-1.4.8/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/requirements/
--rw-r--r--   0 mac        (501) staff       (20)       25 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/requirements/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       79 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1906 2023-01-23 16:42:26.000000 vatis_asr_commons-1.4.8/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/
--rw-r--r--   0 mac        (501) staff       (20)        0 2021-11-19 07:42:07.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/config/
--rw-r--r--   0 mac        (501) staff       (20)      540 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/config/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     6120 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/config/audio.py
--rw-r--r--   0 mac        (501) staff       (20)      740 2022-08-01 15:26:57.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/config/headers.py
--rw-r--r--   0 mac        (501) staff       (20)     1950 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/config/logging.py
--rw-r--r--   0 mac        (501) staff       (20)     6417 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/config/parse.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/constants/
--rw-r--r--   0 mac        (501) staff       (20)       89 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/constants/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       21 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/constants/custom_models.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/custom_models/
--rw-r--r--   0 mac        (501) staff       (20)     1014 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/custom_models/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/custom_models/en_GB.py
--rw-r--r--   0 mac        (501) staff       (20)     1112 2023-01-21 11:08:04.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/custom_models/model.py
--rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/custom_models/ro_RO.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/domain/
--rw-r--r--   0 mac        (501) staff       (20)      922 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/domain/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      717 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/domain/exception.py
--rw-r--r--   0 mac        (501) staff       (20)     2245 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/domain/expression.py
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/domain/find_replace.py
--rw-r--r--   0 mac        (501) staff       (20)      131 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/domain/speaker.py
--rw-r--r--   0 mac        (501) staff       (20)     1703 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/domain/spoken_commands.py
--rw-r--r--   0 mac        (501) staff       (20)    10313 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/domain/transcriber.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/
--rw-r--r--   0 mac        (501) staff       (20)       87 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      212 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/i18n_keys.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/en/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/
--rw-r--r--   0 mac        (501) staff       (20)      178 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.mo
--rw-r--r--   0 mac        (501) staff       (20)      132 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.po
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/ro/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/
--rw-r--r--   0 mac        (501) staff       (20)      179 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.mo
--rw-r--r--   0 mac        (501) staff       (20)      133 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.po
--rw-r--r--   0 mac        (501) staff       (20)      114 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/locale/speakers_service.pot
--rw-r--r--   0 mac        (501) staff       (20)     2822 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/translate.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/json/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-01-22 13:07:30.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/json/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      139 2023-01-22 13:21:45.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/json/deserialization.py
--rw-r--r--   0 mac        (501) staff       (20)      106 2023-01-22 13:11:37.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/json/serialization.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/live/
--rw-r--r--   0 mac        (501) staff       (20)      333 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/live/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1325 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/live/event.py
--rw-r--r--   0 mac        (501) staff       (20)     1562 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/live/headers.py
--rw-r--r--   0 mac        (501) staff       (20)      127 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/live/response.py
--rw-r--r--   0 mac        (501) staff       (20)       98 2021-09-17 07:02:12.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/live/sio_topics.py
--rw-r--r--   0 mac        (501) staff       (20)     1268 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/live/utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/scaler/
--rw-r--r--   0 mac        (501) staff       (20)       71 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/scaler/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      155 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/scaler/response.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/security/
--rw-r--r--   0 mac        (501) staff       (20)       75 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/security/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      138 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/security/jwt.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/static/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-01-23 09:41:24.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/static/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      457 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/static/exceptions.py
--rw-r--r--   0 mac        (501) staff       (20)       62 2022-04-14 11:35:28.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/static/headers.py
--rw-r--r--   0 mac        (501) staff       (20)     4532 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.8/vatis/asr_commons/static/request.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      931 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2145 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2021-09-17 07:17:20.000000 vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)       25 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-02-04 10:24:01.000000 vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/
+-rw-r--r--   0 mac        (501) staff       (20)      601 2021-09-17 07:50:18.000000 vatis_asr_commons-1.4.9/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)       72 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      931 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      845 2023-01-21 11:08:04.000000 vatis_asr_commons-1.4.9/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/requirements/
+-rw-r--r--   0 mac        (501) staff       (20)       25 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/requirements/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       79 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1906 2023-02-04 10:25:09.000000 vatis_asr_commons-1.4.9/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2021-11-19 07:42:07.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/
+-rw-r--r--   0 mac        (501) staff       (20)      540 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     6120 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/audio.py
+-rw-r--r--   0 mac        (501) staff       (20)      740 2022-08-01 15:26:57.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)     1950 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/logging.py
+-rw-r--r--   0 mac        (501) staff       (20)     6417 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/parse.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/constants/
+-rw-r--r--   0 mac        (501) staff       (20)       89 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/constants/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       21 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/constants/custom_models.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/
+-rw-r--r--   0 mac        (501) staff       (20)     1014 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/en_GB.py
+-rw-r--r--   0 mac        (501) staff       (20)     1112 2023-01-21 11:08:04.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/model.py
+-rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/ro_RO.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/
+-rw-r--r--   0 mac        (501) staff       (20)      922 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      717 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/exception.py
+-rw-r--r--   0 mac        (501) staff       (20)     2245 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/expression.py
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/find_replace.py
+-rw-r--r--   0 mac        (501) staff       (20)      131 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/speaker.py
+-rw-r--r--   0 mac        (501) staff       (20)     1703 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/spoken_commands.py
+-rw-r--r--   0 mac        (501) staff       (20)    10416 2023-02-21 19:15:38.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/transcriber.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/
+-rw-r--r--   0 mac        (501) staff       (20)       87 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      212 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/i18n_keys.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/en/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/
+-rw-r--r--   0 mac        (501) staff       (20)      178 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.mo
+-rw-r--r--   0 mac        (501) staff       (20)      132 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.po
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/ro/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 mac        (501) staff       (20)      179 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.mo
+-rw-r--r--   0 mac        (501) staff       (20)      133 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.po
+-rw-r--r--   0 mac        (501) staff       (20)      114 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/speakers_service.pot
+-rw-r--r--   0 mac        (501) staff       (20)     2822 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/translate.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/json/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-01-22 13:07:30.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/json/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      139 2023-01-22 13:21:45.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/json/deserialization.py
+-rw-r--r--   0 mac        (501) staff       (20)      106 2023-01-22 13:11:37.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/json/serialization.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/
+-rw-r--r--   0 mac        (501) staff       (20)      333 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1325 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/event.py
+-rw-r--r--   0 mac        (501) staff       (20)     1562 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)      127 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/response.py
+-rw-r--r--   0 mac        (501) staff       (20)       98 2021-09-17 07:02:12.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/sio_topics.py
+-rw-r--r--   0 mac        (501) staff       (20)     1268 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/scaler/
+-rw-r--r--   0 mac        (501) staff       (20)       71 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/scaler/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      155 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/scaler/response.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/security/
+-rw-r--r--   0 mac        (501) staff       (20)       75 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/security/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      138 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/security/jwt.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2022-01-23 09:41:24.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      457 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/exceptions.py
+-rw-r--r--   0 mac        (501) staff       (20)       62 2022-04-14 11:35:28.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)     4532 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/request.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      931 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2145 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2021-09-17 07:17:20.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (501) staff       (20)       25 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/top_level.txt
```

### Comparing `vatis_asr_commons-1.4.8/LICENSE.txt` & `vatis_asr_commons-1.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/PKG-INFO` & `vatis_asr_commons-1.4.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vatis_asr_commons
-Version: 1.4.8
+Version: 1.4.9
 Summary: Common objects for Vatis ASR clients
 Home-page: https://gitlab.com/vatistech/asr-commons
 Maintainer: VATIS TECH
 Maintainer-email: support@vatis.tech
 License: UNKNOWN
-Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/1.4.8/asr_commons-1.4.8.zip
+Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/1.4.9/asr_commons-1.4.9.zip
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `vatis_asr_commons-1.4.8/README.md` & `vatis_asr_commons-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/setup.py` & `vatis_asr_commons-1.4.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import find_namespace_packages, setup
 
 __name__ = 'vatis_asr_commons'
-__tag__ = '1.4.8'
+__tag__ = '1.4.9'
 __short_description__ = 'Common objects for Vatis ASR clients'
 __download_url__ = 'https://gitlab.com/vatistech/asr-commons/-/archive/{__tag__}/asr_commons-{__tag__}.zip'\
     .format(__tag__=__tag__)
 
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
```

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/config/__init__.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/config/__init__.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/config/audio.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/config/audio.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/config/headers.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/config/headers.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/config/logging.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/config/logging.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/config/parse.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/config/parse.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/custom_models/__init__.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/__init__.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/custom_models/model.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/model.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/domain/__init__.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/domain/exception.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/exception.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/domain/expression.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/expression.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/domain/find_replace.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/find_replace.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/domain/spoken_commands.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/spoken_commands.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/domain/transcriber.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/transcriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,24 +176,25 @@
         QUANTITY: ClassVar[str] = 'QUANTITY'
         MONEY: ClassVar[str] = 'MONEY'
         NUMERIC: ClassVar[str] = 'NUMERIC'
         ORDINAL: ClassVar[str] = 'ORDINAL'
         FACILITY: ClassVar[str] = 'FACILITY'
         WORK_OF_ART: ClassVar[str] = 'WORK_OF_ART'
         EVENT: ClassVar[str] = 'EVENT'
+        REPLACED: ClassVar[str] = 'REPLACED'
 
     def __init__(self, word: str, start_time_millis: float, end_time_millis: float, speaker: Optional[Union[str, int]] = None,
-                 confidence: float = 0, entity: Optional[str] = None, entity_group_id: Optional[int] = None):
+                 confidence: float = 0, entity: Optional[str] = None, entity_group_id: Optional[Union[int, str]] = None):
         self.word: str = word
         self.start_time: float = start_time_millis
         self.end_time: float = end_time_millis
         self.speaker: str = str(speaker) if speaker is not None else None
         self.confidence: float = confidence
         self.entity: Optional[str] = entity
-        self.entity_group_id: Optional[int] = entity_group_id
+        self.entity_group_id: Optional[str] = str(entity_group_id) if entity_group_id is not None else None
 
     def __str__(self):
         return f'''
         {{
             "word": "{self.word}",
             "start_time": {self.start_time},
             "end_time": {self.end_time},
```

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/i18n/translate.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/translate.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/live/event.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/live/event.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/live/headers.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/live/headers.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/live/utils.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/live/utils.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis/asr_commons/static/request.py` & `vatis_asr_commons-1.4.9/vatis/asr_commons/static/request.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/PKG-INFO` & `vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vatis-asr-commons
-Version: 1.4.8
+Version: 1.4.9
 Summary: Common objects for Vatis ASR clients
 Home-page: https://gitlab.com/vatistech/asr-commons
 Maintainer: VATIS TECH
 Maintainer-email: support@vatis.tech
 License: UNKNOWN
-Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/1.4.8/asr_commons-1.4.8.zip
+Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/1.4.9/asr_commons-1.4.9.zip
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `vatis_asr_commons-1.4.8/vatis_asr_commons.egg-info/SOURCES.txt` & `vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

