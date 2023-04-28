# Comparing `tmp/webexbotsdk-0.2.1.tar.gz` & `tmp/webexbotsdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexbotsdk-0.2.1.tar", last modified: Fri Apr 28 20:10:37 2023, max compression
+gzip compressed data, was "webexbotsdk-0.2.2.tar", last modified: Fri Apr 28 20:56:38 2023, max compression
```

## Comparing `webexbotsdk-0.2.1.tar` & `webexbotsdk-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:10:37.364929 webexbotsdk-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-28 20:10:37.364929 webexbotsdk-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:10:37.364929 webexbotsdk-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:10:37.360929 webexbotsdk-0.2.1/webexbotsdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/webexbotsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:10:37.364929 webexbotsdk-0.2.1/webexbotsdk/teams/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/webexbotsdk/teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/webexbotsdk/teams/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/webexbotsdk/teams/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/webexbotsdk/teams/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 20:10:22.000000 webexbotsdk-0.2.1/webexbotsdk/tinydb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:10:37.360929 webexbotsdk-0.2.1/webexbotsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-28 20:10:37.000000 webexbotsdk-0.2.1/webexbotsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 20:10:37.000000 webexbotsdk-0.2.1/webexbotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:10:37.000000 webexbotsdk-0.2.1/webexbotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 20:10:37.000000 webexbotsdk-0.2.1/webexbotsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 20:10:37.000000 webexbotsdk-0.2.1/webexbotsdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/webexbotsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/webexbotsdk/teams/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/teams/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/teams/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/teams/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/tinydb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/webexbotsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/top_level.txt
```

### Comparing `webexbotsdk-0.2.1/LICENSE` & `webexbotsdk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webexbotsdk-0.2.1/PKG-INFO` & `webexbotsdk-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webexbotsdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Webex bot creation framework and tools
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2020 Cisco and/or its affiliates.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,25 +20,27 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: repository, https://github.com/xharriscisco/WebexPythonBotSDK
 Keywords: cisco,webex,teams,bot,python,framework,enterprise,messaging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Communications :: Chat
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 webex bot creation framework and tools via `pip install webexbotsdk`
 
-![PyPI](https://img.shields.io/pypi/v/webexbotsdk) ![PyPI - License](https://img.shields.io/pypi/l/webexbotsdk)
+[![PyPI](https://img.shields.io/pypi/v/webexbotsdk)](https://pypi.org/project/webexbotsdk/)
+[![PyPI - License](https://img.shields.io/pypi/l/webexbotsdk)](https://github.com/xharriscisco/WebexPythonBotSDK/blob/main/LICENSE)
 
 ##### <a id='toc'></a> [webexbotsdk](https://pypi.org/project/webexteamssdk/)
 
 - [teams](#teams)
 - [util](#util)
 - [tinydb](#tinydb)
 
@@ -274,17 +276,15 @@
 ###### [^TOC](#toc) | [@DOCS](https://tinydb.readthedocs.io/en/latest/) | TinyDB library
 
 <br/>
 <br/>
 
 ## <a id='contributing'></a> Contributing
 
-Create an Issue to:
+Create an [Issue](https://github.com/xharriscisco/WebexPythonBotSDK/issues) to:
 
 1. Ask a question
 2. Request a feature
 3. Report a bug
 4. ~~File a complaint~~
 
 Pull requests from branches/forks are also welcome! I will try to respond to them ASAP.
-
-
```

### Comparing `webexbotsdk-0.2.1/README.md` & `webexbotsdk-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 webex bot creation framework and tools via `pip install webexbotsdk`
 
-![PyPI](https://img.shields.io/pypi/v/webexbotsdk) ![PyPI - License](https://img.shields.io/pypi/l/webexbotsdk)
+[![PyPI](https://img.shields.io/pypi/v/webexbotsdk)](https://pypi.org/project/webexbotsdk/)
+[![PyPI - License](https://img.shields.io/pypi/l/webexbotsdk)](https://github.com/xharriscisco/WebexPythonBotSDK/blob/main/LICENSE)
 
 ##### <a id='toc'></a> [webexbotsdk](https://pypi.org/project/webexteamssdk/)
 
 - [teams](#teams)
 - [util](#util)
 - [tinydb](#tinydb)
 
@@ -240,17 +241,15 @@
 ###### [^TOC](#toc) | [@DOCS](https://tinydb.readthedocs.io/en/latest/) | TinyDB library
 
 <br/>
 <br/>
 
 ## <a id='contributing'></a> Contributing
 
-Create an Issue to:
+Create an [Issue](https://github.com/xharriscisco/WebexPythonBotSDK/issues) to:
 
 1. Ask a question
 2. Request a feature
 3. Report a bug
 4. ~~File a complaint~~
 
 Pull requests from branches/forks are also welcome! I will try to respond to them ASAP.
-
-
```

### Comparing `webexbotsdk-0.2.1/webexbotsdk/teams/bot.py` & `webexbotsdk-0.2.2/webexbotsdk/teams/bot.py`

 * *Files identical despite different names*

### Comparing `webexbotsdk-0.2.1/webexbotsdk/teams/hook.py` & `webexbotsdk-0.2.2/webexbotsdk/teams/hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from typing import Callable
 from bottle import request
 from webexteamssdk import WebexTeamsAPI, Message, Person, AttachmentAction, ApiError
-from re import Pattern, search, match
+from re import Pattern, search, match, compile
 from logging import Logger, getLogger, INFO
 
 from .util import is_bot
 
 __all__ = []
 
 class WebhookEvent(Enum):
```

### Comparing `webexbotsdk-0.2.1/webexbotsdk.egg-info/PKG-INFO` & `webexbotsdk-0.2.2/webexbotsdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webexbotsdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Webex bot creation framework and tools
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2020 Cisco and/or its affiliates.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,25 +20,27 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: repository, https://github.com/xharriscisco/WebexPythonBotSDK
 Keywords: cisco,webex,teams,bot,python,framework,enterprise,messaging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Communications :: Chat
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 webex bot creation framework and tools via `pip install webexbotsdk`
 
-![PyPI](https://img.shields.io/pypi/v/webexbotsdk) ![PyPI - License](https://img.shields.io/pypi/l/webexbotsdk)
+[![PyPI](https://img.shields.io/pypi/v/webexbotsdk)](https://pypi.org/project/webexbotsdk/)
+[![PyPI - License](https://img.shields.io/pypi/l/webexbotsdk)](https://github.com/xharriscisco/WebexPythonBotSDK/blob/main/LICENSE)
 
 ##### <a id='toc'></a> [webexbotsdk](https://pypi.org/project/webexteamssdk/)
 
 - [teams](#teams)
 - [util](#util)
 - [tinydb](#tinydb)
 
@@ -274,17 +276,15 @@
 ###### [^TOC](#toc) | [@DOCS](https://tinydb.readthedocs.io/en/latest/) | TinyDB library
 
 <br/>
 <br/>
 
 ## <a id='contributing'></a> Contributing
 
-Create an Issue to:
+Create an [Issue](https://github.com/xharriscisco/WebexPythonBotSDK/issues) to:
 
 1. Ask a question
 2. Request a feature
 3. Report a bug
 4. ~~File a complaint~~
 
 Pull requests from branches/forks are also welcome! I will try to respond to them ASAP.
-
-
```

