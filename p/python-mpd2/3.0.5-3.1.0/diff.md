# Comparing `tmp/python-mpd2-3.0.5.tar.gz` & `tmp/python-mpd2-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mpd2-3.0.5.tar", last modified: Mon Jan 17 17:41:12 2022, max compression
+gzip compressed data, was "python-mpd2-3.1.0.tar", last modified: Fri Apr 28 19:48:52 2023, max compression
```

## Comparing `python-mpd2-3.0.5.tar` & `python-mpd2-3.1.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 joerg     (1000) users      (100)        0 2022-01-17 17:41:12.224058 python-mpd2-3.0.5/
--rw-r--r--   0 joerg     (1000) users      (100)    35147 2014-01-23 16:36:04.000000 python-mpd2-3.0.5/GPL.txt
--rw-r--r--   0 joerg     (1000) users      (100)      855 2014-11-20 09:00:55.000000 python-mpd2-3.0.5/INSTALL.rst
--rw-r--r--   0 joerg     (1000) users      (100)     7651 2014-01-23 16:36:04.000000 python-mpd2-3.0.5/LICENSE.txt
--rw-r--r--   0 joerg     (1000) users      (100)       74 2014-01-23 16:36:04.000000 python-mpd2-3.0.5/MANIFEST.in
--rw-r--r--   0 joerg     (1000) users      (100)     4856 2022-01-17 17:41:12.224058 python-mpd2-3.0.5/PKG-INFO
--rw-r--r--   0 joerg     (1000) users      (100)     4056 2021-10-29 19:31:55.000000 python-mpd2-3.0.5/README.rst
-drwxr-xr-x   0 joerg     (1000) users      (100)        0 2022-01-17 17:41:12.210058 python-mpd2-3.0.5/doc/
--rw-r--r--   0 joerg     (1000) users      (100)     4762 2022-01-17 17:35:45.000000 python-mpd2-3.0.5/doc/changes.rst
--rw-r--r--   0 joerg     (1000) users      (100)     1719 2018-07-30 10:02:15.000000 python-mpd2-3.0.5/doc/index.rst
-drwxr-xr-x   0 joerg     (1000) users      (100)        0 2022-01-17 17:41:12.220058 python-mpd2-3.0.5/doc/topics/
--rw-r--r--   0 joerg     (1000) users      (100)     1375 2021-10-29 19:31:55.000000 python-mpd2-3.0.5/doc/topics/advanced.rst
--rw-r--r--   0 joerg     (1000) users      (100)    27223 2021-10-29 19:31:55.000000 python-mpd2-3.0.5/doc/topics/commands.rst
--rw-r--r--   0 joerg     (1000) users      (100)     2979 2021-10-29 19:31:55.000000 python-mpd2-3.0.5/doc/topics/getting-started.rst
--rw-r--r--   0 joerg     (1000) users      (100)      481 2018-02-20 07:34:15.000000 python-mpd2-3.0.5/doc/topics/logging.rst
--rw-r--r--   0 joerg     (1000) users      (100)     1434 2018-02-20 07:34:15.000000 python-mpd2-3.0.5/doc/topics/porting.rst
-drwxr-xr-x   0 joerg     (1000) users      (100)        0 2022-01-17 17:41:12.222058 python-mpd2-3.0.5/mpd/
--rw-r--r--   0 joerg     (1000) users      (100)     1398 2021-02-02 11:41:53.000000 python-mpd2-3.0.5/mpd/__init__.py
--rw-r--r--   0 joerg     (1000) users      (100)    23459 2021-10-29 19:32:26.000000 python-mpd2-3.0.5/mpd/asyncio.py
--rw-r--r--   0 joerg     (1000) users      (100)    27274 2022-01-17 17:36:19.000000 python-mpd2-3.0.5/mpd/base.py
--rwxr-xr-x   0 joerg     (1000) users      (100)    53406 2021-10-29 19:32:26.000000 python-mpd2-3.0.5/mpd/tests.py
--rw-r--r--   0 joerg     (1000) users      (100)     9177 2020-11-20 15:05:39.000000 python-mpd2-3.0.5/mpd/twisted.py
-drwxr-xr-x   0 joerg     (1000) users      (100)        0 2022-01-17 17:41:12.224058 python-mpd2-3.0.5/python_mpd2.egg-info/
--rw-r--r--   0 joerg     (1000) users      (100)     4856 2022-01-17 17:41:12.000000 python-mpd2-3.0.5/python_mpd2.egg-info/PKG-INFO
--rw-r--r--   0 joerg     (1000) users      (100)      517 2022-01-17 17:41:12.000000 python-mpd2-3.0.5/python_mpd2.egg-info/SOURCES.txt
--rw-r--r--   0 joerg     (1000) users      (100)        1 2022-01-17 17:41:12.000000 python-mpd2-3.0.5/python_mpd2.egg-info/dependency_links.txt
--rw-r--r--   0 joerg     (1000) users      (100)       19 2022-01-17 17:41:12.000000 python-mpd2-3.0.5/python_mpd2.egg-info/requires.txt
--rw-r--r--   0 joerg     (1000) users      (100)        4 2022-01-17 17:41:12.000000 python-mpd2-3.0.5/python_mpd2.egg-info/top_level.txt
--rw-r--r--   0 joerg     (1000) users      (100)        1 2016-09-10 16:06:18.000000 python-mpd2-3.0.5/python_mpd2.egg-info/zip-safe
--rw-r--r--   0 joerg     (1000) users      (100)        0 2017-03-20 12:49:07.000000 python-mpd2-3.0.5/requirements_frozen.txt
--rw-r--r--   0 joerg     (1000) users      (100)       38 2022-01-17 17:41:12.224058 python-mpd2-3.0.5/setup.cfg
--rw-r--r--   0 joerg     (1000) users      (100)     2718 2021-10-29 19:31:55.000000 python-mpd2-3.0.5/setup.py
+drwxr-xr-x   0 joerg     (1000) users      (100)        0 2023-04-28 19:48:52.978772 python-mpd2-3.1.0/
+-rw-r--r--   0 joerg     (1000) users      (100)    35147 2014-01-23 16:36:04.000000 python-mpd2-3.1.0/GPL.txt
+-rw-r--r--   0 joerg     (1000) users      (100)      855 2014-11-20 09:00:55.000000 python-mpd2-3.1.0/INSTALL.rst
+-rw-r--r--   0 joerg     (1000) users      (100)     7651 2014-01-23 16:36:04.000000 python-mpd2-3.1.0/LICENSE.txt
+-rw-r--r--   0 joerg     (1000) users      (100)       74 2014-01-23 16:36:04.000000 python-mpd2-3.1.0/MANIFEST.in
+-rw-r--r--   0 joerg     (1000) users      (100)     4836 2023-04-28 19:48:52.978772 python-mpd2-3.1.0/PKG-INFO
+-rw-r--r--   0 joerg     (1000) users      (100)     4056 2021-10-29 19:31:55.000000 python-mpd2-3.1.0/README.rst
+drwxr-xr-x   0 joerg     (1000) users      (100)        0 2023-04-28 19:48:52.976772 python-mpd2-3.1.0/doc/
+-rw-r--r--   0 joerg     (1000) users      (100)     5493 2023-02-18 05:38:28.000000 python-mpd2-3.1.0/doc/changes.rst
+-rw-r--r--   0 joerg     (1000) users      (100)     1719 2018-07-30 10:02:15.000000 python-mpd2-3.1.0/doc/index.rst
+drwxr-xr-x   0 joerg     (1000) users      (100)        0 2023-04-28 19:48:52.977772 python-mpd2-3.1.0/doc/topics/
+-rw-r--r--   0 joerg     (1000) users      (100)     1375 2021-10-29 19:31:55.000000 python-mpd2-3.1.0/doc/topics/advanced.rst
+-rw-r--r--   0 joerg     (1000) users      (100)    27223 2021-10-29 19:31:55.000000 python-mpd2-3.1.0/doc/topics/commands.rst
+-rw-r--r--   0 joerg     (1000) users      (100)     2979 2021-10-29 19:31:55.000000 python-mpd2-3.1.0/doc/topics/getting-started.rst
+-rw-r--r--   0 joerg     (1000) users      (100)      481 2018-02-20 07:34:15.000000 python-mpd2-3.1.0/doc/topics/logging.rst
+-rw-r--r--   0 joerg     (1000) users      (100)     1434 2018-02-20 07:34:15.000000 python-mpd2-3.1.0/doc/topics/porting.rst
+drwxr-xr-x   0 joerg     (1000) users      (100)        0 2023-04-28 19:48:52.977772 python-mpd2-3.1.0/mpd/
+-rw-r--r--   0 joerg     (1000) users      (100)     1398 2021-02-02 11:41:53.000000 python-mpd2-3.1.0/mpd/__init__.py
+-rw-r--r--   0 joerg     (1000) users      (100)    23949 2023-02-18 05:38:24.000000 python-mpd2-3.1.0/mpd/asyncio.py
+-rw-r--r--   0 joerg     (1000) users      (100)    27760 2023-02-18 05:38:28.000000 python-mpd2-3.1.0/mpd/base.py
+-rwxr-xr-x   0 joerg     (1000) users      (100)    54939 2023-02-18 05:38:24.000000 python-mpd2-3.1.0/mpd/tests.py
+-rw-r--r--   0 joerg     (1000) users      (100)     9177 2020-11-20 15:05:39.000000 python-mpd2-3.1.0/mpd/twisted.py
+drwxr-xr-x   0 joerg     (1000) users      (100)        0 2023-04-28 19:48:52.978772 python-mpd2-3.1.0/python_mpd2.egg-info/
+-rw-r--r--   0 joerg     (1000) users      (100)     4836 2023-04-28 19:48:52.000000 python-mpd2-3.1.0/python_mpd2.egg-info/PKG-INFO
+-rw-r--r--   0 joerg     (1000) users      (100)      493 2023-04-28 19:48:52.000000 python-mpd2-3.1.0/python_mpd2.egg-info/SOURCES.txt
+-rw-r--r--   0 joerg     (1000) users      (100)        1 2023-04-28 19:48:52.000000 python-mpd2-3.1.0/python_mpd2.egg-info/dependency_links.txt
+-rw-r--r--   0 joerg     (1000) users      (100)       19 2023-04-28 19:48:52.000000 python-mpd2-3.1.0/python_mpd2.egg-info/requires.txt
+-rw-r--r--   0 joerg     (1000) users      (100)        4 2023-04-28 19:48:52.000000 python-mpd2-3.1.0/python_mpd2.egg-info/top_level.txt
+-rw-r--r--   0 joerg     (1000) users      (100)        1 2016-09-10 16:06:18.000000 python-mpd2-3.1.0/python_mpd2.egg-info/zip-safe
+-rw-r--r--   0 joerg     (1000) users      (100)       38 2023-04-28 19:48:52.978772 python-mpd2-3.1.0/setup.cfg
+-rw-r--r--   0 joerg     (1000) users      (100)     2718 2021-10-29 19:31:55.000000 python-mpd2-3.1.0/setup.py
```

### Comparing `python-mpd2-3.0.5/GPL.txt` & `python-mpd2-3.1.0/GPL.txt`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/INSTALL.rst` & `python-mpd2-3.1.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/LICENSE.txt` & `python-mpd2-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/PKG-INFO` & `python-mpd2-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: python-mpd2
-Version: 3.0.5
+Version: 3.1.0
 Summary: A Python MPD client library
 Home-page: https://github.com/Mic92/python-mpd2
 Author: Joerg Thalheim
 Author-email: joerg@thalheim.io
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: mpd
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -149,9 +148,7 @@
 The command reference is generated from the official mpd protocol documentation.
 In order to update it, install python-lxml and run the following command::
 
     $ python ./doc/generate_command_reference.py > ./doc/topics/commands.rst
 
 
 .. _python-mpd: https://pypi.python.org/pypi/python-mpd/
-
-
```

### Comparing `python-mpd2-3.0.5/README.rst` & `python-mpd2-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/doc/changes.rst` & `python-mpd2-3.1.0/doc/changes.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 python-mpd2 Changes List
 ========================
 
+Changes in v3.1.0
+-----------------
+
+* fixed multiple use of "group" in list command by @SoongNoonien in https://github.com/Mic92/python-mpd2/pull/187
+* fix unmount command not working by @burrocargado in https://github.com/Mic92/python-mpd2/pull/188
+* added binarylimit command by @SoongNoonien in https://github.com/Mic92/python-mpd2/pull/191
+* Implement abstract socket support by @aurieh in https://github.com/Mic92/python-mpd2/pull/193
+* missing import / wrong variable by @mk-81 in https://github.com/Mic92/python-mpd2/pull/196
+* also test python3.12 by @Mic92 in https://github.com/Mic92/python-mpd2/pull/200
+* asyncio: fix race condition in command queue by @yakshaver2000 in https://github.com/Mic92/python-mpd2/pull/199
+
 Changes in v3.0.5
 -----------------
 
 * python 3.10 compatibility
 * fixes for using idle in async
 * use python's internal mock library instead of external mock
 * expose connection status in async (connected property)
```

### Comparing `python-mpd2-3.0.5/doc/index.rst` & `python-mpd2-3.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/doc/topics/advanced.rst` & `python-mpd2-3.1.0/doc/topics/advanced.rst`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/doc/topics/commands.rst` & `python-mpd2-3.1.0/doc/topics/commands.rst`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/doc/topics/getting-started.rst` & `python-mpd2-3.1.0/doc/topics/getting-started.rst`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/doc/topics/porting.rst` & `python-mpd2-3.1.0/doc/topics/porting.rst`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/mpd/__init__.py` & `python-mpd2-3.1.0/mpd/__init__.py`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/mpd/asyncio.py` & `python-mpd2-3.1.0/mpd/asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import asyncio
 from functools import partial
 from typing import Optional, List, Tuple, Iterable, Callable, Union
 
 from mpd.base import HELLO_PREFIX, ERROR_PREFIX, SUCCESS
 from mpd.base import MPDClientBase
 from mpd.base import MPDClient as SyncMPDClient
-from mpd.base import ProtocolError, ConnectionError, CommandError
+from mpd.base import ProtocolError, ConnectionError, CommandError, CommandListError
 from mpd.base import mpd_command_provider
 
 
 class BaseCommandResult(asyncio.Future):
     """A future that carries its command/args/callback with it for the
     convenience of passing it around to the command queue."""
 
@@ -198,15 +198,17 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__rfile = self.__wfile = None
 
     async def connect(self, host, port=6600, loop=None):
         if loop is not None:
             warnings.warn("loop passed into MPDClient.connect is ignored, this will become an error", DeprecationWarning)
-        if "/" in host:
+        if host.startswith("@"):
+            host = "\0" + host[1:]
+        if host.startswith("\0") or "/" in host:
             r, w = await asyncio.open_unix_connection(host)
         else:
             r, w = await asyncio.open_connection(host, port)
         self.__rfile, self.__wfile = r, w
 
         self.__command_queue = asyncio.Queue(maxsize=self.COMMAND_QUEUE_LENGTH)
         self.__idle_consumers = []  #: list of (subsystem-list, callbacks) tuples
@@ -274,14 +276,21 @@
                         timeout=self.IMMEDIATE_COMMAND_TIMEOUT,
                     )
                 except asyncio.TimeoutError:
                     # The cancellation of the __command_queue.get() that happens
                     # in this case is intended, and is just what asyncio.Queue
                     # suggests for "get with timeout".
 
+                    if not self.__command_queue.empty():
+                        # A __command_queue.put() has happened after the
+                        # asyncio.wait_for() timeout but before execution of
+                        # this coroutine resumed. Looping around again will
+                        # fetch the new entry from the queue.
+                        continue
+
                     if self.__idle_failed:
                         # We could try for a more elaborate path where we now
                         # await the command queue indefinitely, but as we're
                         # already in an error case, this whole situation only
                         # persists until the error is processed somewhere else,
                         # so ticking once per idle timeout is OK to keep things
                         # simple.
```

### Comparing `python-mpd2-3.0.5/mpd/base.py` & `python-mpd2-3.1.0/mpd/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import socket
 import sys
 import warnings
 
 from enum import Enum
 
 
-VERSION = (3, 0, 5)
+VERSION = (3, 1, 0)
 HELLO_PREFIX = "OK MPD "
 ERROR_PREFIX = "ACK "
 ERROR_PATTERN = re.compile(r"\[(?P<errno>\d+)@(?P<offset>\d+)\]\s+{(?P<command>\w+)}\s+(?P<msg>.*)")
 SUCCESS = "OK"
 NEXT = "list_OK"
 
 
@@ -235,20 +235,28 @@
         for line in lines:
             yield self._parse_pair(line, separator)
 
     def _parse_objects(self, lines, delimiters=[], lookup_delimiter=False):
         obj = {}
         for key, value in self._parse_pairs(lines):
             key = key.lower()
-            if lookup_delimiter and not delimiters:
-                delimiters = [key]
+            if lookup_delimiter and key not in delimiters:
+                delimiters = delimiters + [key]
             if obj:
                 if key in delimiters:
-                    yield obj
-                    obj = {}
+                    if lookup_delimiter:
+                        if key in obj:
+                            yield obj
+                            obj = obj.copy()
+                            while delimiters[-1] != key:
+                                obj.pop(delimiters[-1], None)
+                                delimiters.pop()
+                    else:
+                        yield obj
+                        obj = {}
                 elif key in obj:
                     if not isinstance(obj[key], list):
                         obj[key] = [obj[key], value]
                     else:
                         obj[key].append(value)
                     continue
             obj[key] = value
@@ -318,14 +326,15 @@
     @mpd_commands("listpartitions", is_direct=True)
     def _parse_partitions(self, lines):
         return self._parse_objects_direct(lines, ["partition"])
 
     @mpd_commands(
         "add",
         "addtagid",
+        "binarylimit",
         "clear",
         "clearerror",
         "cleartagid",
         "consume",
         "crossfade",
         "delete",
         "deleteid",
@@ -375,15 +384,15 @@
         "sticker delete",
         "sticker set",
         "stop",
         "subscribe",
         "swap",
         "swapid",
         "toggleoutput",
-        "umount",
+        "unmount",
         "unsubscribe",
         "volume",
     )
     def _parse_nothing(self, lines):
         for line in lines:
             raise ProtocolError(
                 "Got unexpected return value: '{}'".format(", ".join(lines))
@@ -620,15 +629,15 @@
                 chunk_size = int(value)
                 value = self._read_chunk(chunk_size)
 
                 if len(value) != chunk_size:
                     self.disconnect()
                     raise ConnectionError(
                         "Connection lost while reading binary data: "
-                        "expected %d bytes, got %d" % (chunk_size, len(data))
+                        "expected %d bytes, got %d" % (chunk_size, len(value))
                     )
 
                 if self._rbfile.read(1) != b"\n":
                     # newline after binary content
                     self.disconnect()
                     raise ConnectionError("Connection lost while reading line")
 
@@ -775,15 +784,17 @@
         if timeout is not None:
             warnings.warn(
                 "The timeout parameter in connect() is deprecated! "
                 "Use MPDClient.timeout = yourtimeout instead.",
                 DeprecationWarning,
             )
             self.timeout = timeout
-        if host.startswith("/"):
+        if host.startswith("@"):
+            host = "\0" + host[1:]
+        if host.startswith(("/", "\0")):
             self._sock = self._connect_unix(host)
         else:
             if port is None:
                 raise ValueError(
                     "port argument must be specified when connecting via tcp"
                 )
             self._sock = self._connect_tcp(host, port)
```

### Comparing `python-mpd2-3.0.5/mpd/tests.py` & `python-mpd2-3.1.0/mpd/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,39 @@
         self.assertIsNone(self.client.delpartition("Another Partition"))
         self.assertMPDReceived('delpartition "Another Partition"\n')
 
         self.MPDWillReturn("OK\n")
         self.assertIsNone(self.client.moveoutput("My ALSA Device"))
         self.assertMPDReceived('moveoutput "My ALSA Device"\n')
 
+    def test_list_group(self):
+        self.MPDWillReturn(
+            "AlbumArtist: Kraftwerk\n",
+            "Date: 1970\n",
+            "Album: Tone Float (Unofficial)\n",
+            "Date: 1974\n",
+            "Album: Autobahn\n",
+            "Album: Autobahn (2009 Der Katalog)\n",
+            "OK\n"
+        )
+        grouped_list = self.client.list(
+            "album", "albumartist", "Kraftwerk", "group", "date", "group", "albumartist"
+        )
+        self.assertMPDReceived(
+            'list "album" "albumartist" "Kraftwerk" "group" "date" "group" "albumartist"\n'
+        )
+        self.assertEqual(
+            [
+                {'albumartist': 'Kraftwerk', 'date': '1970', 'album': 'Tone Float (Unofficial)'},
+                {'albumartist': 'Kraftwerk', 'date': '1974', 'album': 'Autobahn'},
+                {'albumartist': 'Kraftwerk', 'date': '1974', 'album': 'Autobahn (2009 Der Katalog)'}
+            ],
+            grouped_list
+        )
+
     def test_client_to_client(self):
         # client to client is at this time in beta!
 
         self.MPDWillReturn("OK\n")
         self.assertIsNone(self.client.subscribe("monty"))
         self.assertMPDReceived('subscribe "monty"\n')
 
@@ -1547,10 +1572,22 @@
 
         self.client.disconnect()
 
     def test_idle(self):
         self.init_client()
         self._await(self._test_idle())
 
+    async def _test_idle_timeout(self):
+        self.mockserver.expect_exchange([b'currentsong\n'], [b"OK\n"])
+        self.mockserver.expect_exchange([b'currentsong\n'], [b"OK\n"])
+        await self.client.currentsong()
+        # pausing for exactly this duration triggers a special case in mpd.asyncio.MPDClient.__run
+        await asyncio.sleep(self.client.IMMEDIATE_COMMAND_TIMEOUT)
+        await self.client.currentsong()
+        self.client.disconnect()
+
+    def test_idle_timeout(self):
+        self.init_client()
+        self._await(self._test_idle_timeout())
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `python-mpd2-3.0.5/mpd/twisted.py` & `python-mpd2-3.1.0/mpd/twisted.py`

 * *Files identical despite different names*

### Comparing `python-mpd2-3.0.5/python_mpd2.egg-info/PKG-INFO` & `python-mpd2-3.1.0/python_mpd2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: python-mpd2
-Version: 3.0.5
+Version: 3.1.0
 Summary: A Python MPD client library
 Home-page: https://github.com/Mic92/python-mpd2
 Author: Joerg Thalheim
 Author-email: joerg@thalheim.io
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: mpd
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -149,9 +148,7 @@
 The command reference is generated from the official mpd protocol documentation.
 In order to update it, install python-lxml and run the following command::
 
     $ python ./doc/generate_command_reference.py > ./doc/topics/commands.rst
 
 
 .. _python-mpd: https://pypi.python.org/pypi/python-mpd/
-
-
```

### Comparing `python-mpd2-3.0.5/setup.py` & `python-mpd2-3.1.0/setup.py`

 * *Files identical despite different names*

