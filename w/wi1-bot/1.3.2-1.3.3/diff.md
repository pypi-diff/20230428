# Comparing `tmp/wi1-bot-1.3.2.tar.gz` & `tmp/wi1-bot-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.3.2.tar", last modified: Sun Apr 23 07:42:26 2023, max compression
+gzip compressed data, was "wi1-bot-1.3.3.tar", last modified: Fri Apr 28 06:44:47 2023, max compression
```

## Comparing `wi1-bot-1.3.2.tar` & `wi1-bot-1.3.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.135047 wi1-bot-1.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 07:42:26.143047 wi1-bot-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-23 07:42:26.000000 wi1-bot-1.3.2/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 07:42:26.000000 wi1-bot-1.3.2/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 06:44:47.000000 wi1-bot-1.3.3/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 06:44:47.000000 wi1-bot-1.3.3/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.3.2/.github/workflows/pypi-publish.yml` & `wi1-bot-1.3.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/.pre-commit-config.yaml` & `wi1-bot-1.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/LICENSE` & `wi1-bot-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/PKG-INFO` & `wi1-bot-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.2
+Version: 1.3.3
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.3.2/README.md` & `wi1-bot-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/config.yaml.template` & `wi1-bot-1.3.3/config.yaml.template`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/pyproject.toml` & `wi1-bot-1.3.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -16,27 +16,26 @@
 dynamic = ["version"]
 requires-python = ">=3.10"
 dependencies = [
     "discord.py==2.2.2",
     "Flask==2.2.3",
     "mongoengine==0.27.0",
     "pyarr==3.1.3",
-    "python-pushover==0.4",
-    "PyYAML==6.0"
+    "PyYAML==6.0",
+    "requests==2.28.2"
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==23.3.0",
     "flake8==6.0.0",
     "isort==5.12.0",
     "mongo-types==0.15.1",
     "mypy==1.2.0",
     "pre-commit==3.2.2",
-    "requests==2.28.2",
     "types-PyYAML==6.0.12.9",
 ]
 
 [project.urls]
 Homepage = "https://github.com/wthueb/wi1-bot"
 
 [project.scripts]
```

### Comparing `wi1-bot-1.3.2/wi1_bot/arr/download.py` & `wi1-bot-1.3.3/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/arr/episode.py` & `wi1-bot-1.3.3/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/arr/movie.py` & `wi1-bot-1.3.3/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/arr/radarr.py` & `wi1-bot-1.3.3/wi1_bot/arr/radarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/arr/sonarr.py` & `wi1-bot-1.3.3/wi1_bot/arr/sonarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/config.py` & `wi1-bot-1.3.3/wi1_bot/config.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/discord/bot.py` & `wi1-bot-1.3.3/wi1_bot/discord/bot.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.3.3/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.3.3/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/discord/helpers.py` & `wi1-bot-1.3.3/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/scripts/start.py` & `wi1-bot-1.3.3/wi1_bot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.3.3/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.3.3/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.3.3/wi1_bot/transcoder/transcoder.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot/webhook.py` & `wi1-bot-1.3.3/wi1_bot/webhook.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.2/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.3.3/wi1_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.2
+Version: 1.3.3
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.3.2/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.3.3/wi1_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

