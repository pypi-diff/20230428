# Comparing `tmp/dgg-bot-0.9.0.tar.gz` & `tmp/dgg-bot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgg-bot-0.9.0.tar", last modified: Sat Feb 11 13:03:15 2023, max compression
+gzip compressed data, was "dgg-bot-0.9.1.tar", last modified: Wed Feb 15 11:08:53 2023, max compression
```

## Comparing `dgg-bot-0.9.0.tar` & `dgg-bot-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-11 13:03:15.032088 dgg-bot-0.9.0/
--rw-rw-rw-   0        0        0     1081 2022-09-09 16:56:19.000000 dgg-bot-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     3551 2023-02-11 13:03:15.031089 dgg-bot-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2811 2023-02-10 14:04:45.000000 dgg-bot-0.9.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-11 13:03:15.007089 dgg-bot-0.9.0/dgg_bot.egg-info/
--rw-rw-rw-   0        0        0     3551 2023-02-11 13:03:14.000000 dgg-bot-0.9.0/dgg_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-02-11 13:03:14.000000 dgg-bot-0.9.0/dgg_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-11 13:03:14.000000 dgg-bot-0.9.0/dgg_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-11 13:03:14.000000 dgg-bot-0.9.0/dgg_bot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-11 13:03:15.026088 dgg-bot-0.9.0/dggbot/
--rw-rw-rw-   0        0        0      206 2023-01-11 16:43:22.000000 dgg-bot-0.9.0/dggbot/__init__.py
--rw-rw-rw-   0        0        0      504 2022-09-11 20:38:19.000000 dgg-bot-0.9.0/dggbot/_logging.py
--rw-rw-rw-   0        0        0     3208 2023-02-10 14:04:45.000000 dgg-bot-0.9.0/dggbot/bot.py
--rw-rw-rw-   0        0        0    13851 2023-02-10 14:06:34.000000 dgg-bot-0.9.0/dggbot/chat.py
--rw-rw-rw-   0        0        0      497 2023-01-15 02:17:22.000000 dgg-bot-0.9.0/dggbot/errors.py
--rw-rw-rw-   0        0        0      607 2023-02-08 17:15:19.000000 dgg-bot-0.9.0/dggbot/event.py
--rw-rw-rw-   0        0        0      339 2023-01-11 16:43:22.000000 dgg-bot-0.9.0/dggbot/funcs.py
-drwxrwxrwx   0        0        0        0 2023-02-11 13:03:15.030089 dgg-bot-0.9.0/dggbot/live/
--rw-rw-rw-   0        0        0     3551 2023-01-11 16:43:22.000000 dgg-bot-0.9.0/dggbot/live/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-01-11 16:43:22.000000 dgg-bot-0.9.0/dggbot/live/message.py
--rw-rw-rw-   0        0        0     1569 2023-02-10 14:03:33.000000 dgg-bot-0.9.0/dggbot/message.py
--rw-rw-rw-   0        0        0      197 2023-01-11 16:43:21.000000 dgg-bot-0.9.0/dggbot/user.py
--rw-rw-rw-   0        0        0      756 2023-02-10 14:08:10.000000 dgg-bot-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-11 13:03:15.032088 dgg-bot-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-02-10 14:08:10.000000 dgg-bot-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-15 11:08:53.812425 dgg-bot-0.9.1/
+-rw-rw-rw-   0        0        0     1081 2022-09-09 16:56:19.000000 dgg-bot-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     3565 2023-02-15 11:08:53.812425 dgg-bot-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2811 2023-02-10 14:04:45.000000 dgg-bot-0.9.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-02-15 11:08:53.789426 dgg-bot-0.9.1/dgg_bot.egg-info/
+-rw-rw-rw-   0        0        0     3565 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-15 11:08:53.807428 dgg-bot-0.9.1/dggbot/
+-rw-rw-rw-   0        0        0      206 2023-01-11 16:43:22.000000 dgg-bot-0.9.1/dggbot/__init__.py
+-rw-rw-rw-   0        0        0      504 2022-09-11 20:38:19.000000 dgg-bot-0.9.1/dggbot/_logging.py
+-rw-rw-rw-   0        0        0     3208 2023-02-10 14:04:45.000000 dgg-bot-0.9.1/dggbot/bot.py
+-rw-rw-rw-   0        0        0    13851 2023-02-14 14:09:09.000000 dgg-bot-0.9.1/dggbot/chat.py
+-rw-rw-rw-   0        0        0      497 2023-01-15 02:17:22.000000 dgg-bot-0.9.1/dggbot/errors.py
+-rw-rw-rw-   0        0        0      607 2023-02-08 17:15:19.000000 dgg-bot-0.9.1/dggbot/event.py
+-rw-rw-rw-   0        0        0      339 2023-01-11 16:43:22.000000 dgg-bot-0.9.1/dggbot/funcs.py
+drwxrwxrwx   0        0        0        0 2023-02-15 11:08:53.811425 dgg-bot-0.9.1/dggbot/live/
+-rw-rw-rw-   0        0        0     3551 2023-01-11 16:43:22.000000 dgg-bot-0.9.1/dggbot/live/__init__.py
+-rw-rw-rw-   0        0        0     1270 2023-01-11 16:43:22.000000 dgg-bot-0.9.1/dggbot/live/message.py
+-rw-rw-rw-   0        0        0     1569 2023-02-10 14:03:33.000000 dgg-bot-0.9.1/dggbot/message.py
+-rw-rw-rw-   0        0        0      197 2023-01-11 16:43:21.000000 dgg-bot-0.9.1/dggbot/user.py
+-rw-rw-rw-   0        0        0     1017 2023-02-15 10:52:35.000000 dgg-bot-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       26 2023-02-10 14:04:45.000000 dgg-bot-0.9.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-02-15 11:08:53.813425 dgg-bot-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2023-02-15 10:38:12.000000 dgg-bot-0.9.1/setup.py
```

### Comparing `dgg-bot-0.9.0/LICENSE` & `dgg-bot-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dgg-bot-0.9.0/PKG-INFO` & `dgg-bot-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: dgg-bot
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for making a bot in Destiny.gg chat.
 Home-page: https://github.com/Fritz-02/dgg-bot/
 Author: Fritz-02
+License: MIT
 Project-URL: Homepage, https://github.com/Fritz-02/dgg-bot/
 Project-URL: Bug Tracker, https://github.com/Fritz-02/dgg-bot/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dgg-bot-0.9.0/README.rst` & `dgg-bot-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `dgg-bot-0.9.0/dgg_bot.egg-info/PKG-INFO` & `dgg-bot-0.9.1/dgg_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: dgg-bot
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for making a bot in Destiny.gg chat.
 Home-page: https://github.com/Fritz-02/dgg-bot/
 Author: Fritz-02
+License: MIT
 Project-URL: Homepage, https://github.com/Fritz-02/dgg-bot/
 Project-URL: Bug Tracker, https://github.com/Fritz-02/dgg-bot/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dgg-bot-0.9.0/dggbot/bot.py` & `dgg-bot-0.9.1/dggbot/bot.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-0.9.0/dggbot/chat.py` & `dgg-bot-0.9.1/dggbot/chat.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-0.9.0/dggbot/event.py` & `dgg-bot-0.9.1/dggbot/event.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-0.9.0/dggbot/live/__init__.py` & `dgg-bot-0.9.1/dggbot/live/__init__.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-0.9.0/dggbot/live/message.py` & `dgg-bot-0.9.1/dggbot/live/message.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-0.9.0/dggbot/message.py` & `dgg-bot-0.9.1/dggbot/message.py`

 * *Files identical despite different names*

