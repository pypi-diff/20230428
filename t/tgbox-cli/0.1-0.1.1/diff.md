# Comparing `tmp/tgbox-cli-0.1.tar.gz` & `tmp/tgbox-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgbox-cli-0.1.tar", last modified: Fri Apr 21 01:30:00 2023, max compression
+gzip compressed data, was "tgbox-cli-0.1.1.tar", last modified: Fri Apr 28 21:09:14 2023, max compression
```

## Comparing `tgbox-cli-0.1.tar` & `tgbox-cli-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-04-21 01:30:00.949699 tgbox-cli-0.1/
--rw-r--r--   0 non       (1000) non       (1000)      256 2023-04-21 01:30:00.949699 tgbox-cli-0.1/PKG-INFO
--rw-r--r--   0 non       (1000) non       (1000)        0 2023-04-21 01:29:02.000000 tgbox-cli-0.1/README
--rw-r--r--   0 non       (1000) non       (1000)       38 2023-04-21 01:30:00.949699 tgbox-cli-0.1/setup.cfg
--rw-r--r--   0 non       (1000) non       (1000)      467 2023-04-21 01:28:40.000000 tgbox-cli-0.1/setup.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-04-21 01:30:00.949699 tgbox-cli-0.1/tgbox_cli.egg-info/
--rw-r--r--   0 non       (1000) non       (1000)      256 2023-04-21 01:30:00.000000 tgbox-cli-0.1/tgbox_cli.egg-info/PKG-INFO
--rw-r--r--   0 non       (1000) non       (1000)      247 2023-04-21 01:30:00.000000 tgbox-cli-0.1/tgbox_cli.egg-info/SOURCES.txt
--rw-r--r--   0 non       (1000) non       (1000)        1 2023-04-21 01:30:00.000000 tgbox-cli-0.1/tgbox_cli.egg-info/dependency_links.txt
--rw-r--r--   0 non       (1000) non       (1000)       68 2023-04-21 01:30:00.000000 tgbox-cli-0.1/tgbox_cli.egg-info/entry_points.txt
--rw-r--r--   0 non       (1000) non       (1000)       21 2023-04-21 01:30:00.000000 tgbox-cli-0.1/tgbox_cli.egg-info/requires.txt
--rw-r--r--   0 non       (1000) non       (1000)       26 2023-04-21 01:30:00.000000 tgbox-cli-0.1/tgbox_cli.egg-info/top_level.txt
--rwxr-xr-x   0 non       (1000) non       (1000)    41117 2023-04-21 01:22:07.000000 tgbox-cli-0.1/tgbox_cli.py
--rw-r--r--   0 non       (1000) non       (1000)     3677 2023-04-21 01:15:50.000000 tgbox-cli-0.1/tgbox_cli_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:09:14.032647 tgbox-cli-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 21:09:14.028647 tgbox-cli-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 21:09:14.032647 tgbox-cli-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-04-28 21:08:38.000000 tgbox-cli-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:09:14.024647 tgbox-cli-0.1.1/tgbox_cli/
+-rwxr-xr-x   0 root         (0) root         (0)    41172 2023-04-28 21:08:38.000000 tgbox-cli-0.1.1/tgbox_cli/tgbox_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2023-04-28 21:08:38.000000 tgbox-cli-0.1.1/tgbox_cli/tools.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 21:08:38.000000 tgbox-cli-0.1.1/tgbox_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:09:14.028647 tgbox-cli-0.1.1/tgbox_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      271 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/top_level.txt
```

### Comparing `tgbox-cli-0.1/tgbox_cli.py` & `tgbox-cli-0.1.1/tgbox_cli/tgbox_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 from hashlib import sha256
 from asyncio import gather
 
 from ast import literal_eval
 from pickle import loads, dumps
 from sys import platform, stdout
 
+from os import (
+    getenv, _exit,
+    system as os_system,
+)
 from base64 import urlsafe_b64encode
 from traceback import format_exception
 from typing import Union, AsyncGenerator
 from datetime import datetime, timedelta
 from subprocess import run as subprocess_run, PIPE
 
-from os import (
-    getenv, _exit,
-    system as os_system,
-)
-from tgbox_cli_tools import (
+from enlighten import get_manager
+
+from .tools import (
     Progress, format_bytes, sync_async_gen,
     filters_to_searchfilter, clear_console,
     exit_program
 )
-from enlighten import get_manager
+from .version import VERSION
 
 
-__version__ = '0.1_' + tgbox.constants.VERSION
+__version__ = f'{VERSION}_{tgbox.constants.VERSION}'
 tgbox.constants.VERSION = __version__
 
 # Please DO NOT use this parameters in your projects.
 # You can get your own at my.telegram.org. Thanks.
 API_ID = 2210681
 API_HASH = '33755adb5ba3c296ccf0dd5220143841'
 
@@ -163,15 +165,15 @@
         )
         exit_program()
 
 @click.group()
 def cli():
    pass
 
-def safe_cli():
+def safe_tgbox_cli_startup():
     try:
         cli()
     except Exception as e:
         if getenv('TGBOX_DEBUG'):
             e = ''.join(format_exception(
                 etype = None,
                 value = e,
@@ -1342,8 +1344,8 @@
         f'''TGBOX Version: {magenta(ver[1])}\n\n'''
         f'''FFMPEG: {ffmpeg_version}\n'''
         f'''FAST_ENCRYPTION: {green('YES') if tgbox.crypto.FAST_ENCRYPTION else red('NO')}\n'''
         f'''FAST_TELETHON: {green('YES') if tgbox.crypto.FAST_TELETHON else red('NO')}\n'''
     )
 
 if __name__ == '__main__':
-    safe_cli()
+    safe_tgbox_cli_startup()
```

### Comparing `tgbox-cli-0.1/tgbox_cli_tools.py` & `tgbox-cli-0.1.1/tgbox_cli/tools.py`

 * *Files identical despite different names*

