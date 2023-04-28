# Comparing `tmp/pyvizio-0.1.8.tar.gz` & `tmp/pyvizio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyvizio-0.1.8.tar", last modified: Wed Jan 29 01:57:22 2020, max compression
+gzip compressed data, was "dist/pyvizio-0.1.9.tar", last modified: Wed Jan 29 02:13:05 2020, max compression
```

## Comparing `pyvizio-0.1.8.tar` & `pyvizio-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-29 01:57:22.000000 pyvizio-0.1.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5675 2020-01-29 01:57:22.000000 pyvizio-0.1.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4074 2020-01-29 01:57:04.000000 pyvizio-0.1.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-29 01:57:22.000000 pyvizio-0.1.8/pyvizio/
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8239 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3014 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/cmd_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/cmd_pair.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      633 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/cmd_power.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      905 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/cmd_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2516 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/cmd_settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/const.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1491 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8273 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/protocol.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22327 2020-01-29 01:57:04.000000 pyvizio-0.1.8/pyvizio/vizio.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-29 01:57:22.000000 pyvizio-0.1.8/pyvizio.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5675 2020-01-29 01:57:22.000000 pyvizio-0.1.8/pyvizio.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      453 2020-01-29 01:57:22.000000 pyvizio-0.1.8/pyvizio.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-29 01:57:22.000000 pyvizio-0.1.8/pyvizio.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2020-01-29 01:57:22.000000 pyvizio-0.1.8/pyvizio.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-01-29 01:57:22.000000 pyvizio-0.1.8/pyvizio.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-01-29 01:57:22.000000 pyvizio-0.1.8/pyvizio.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      754 2020-01-29 01:57:22.000000 pyvizio-0.1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1038 2020-01-29 01:57:04.000000 pyvizio-0.1.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-29 02:13:05.000000 pyvizio-0.1.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5675 2020-01-29 02:13:05.000000 pyvizio-0.1.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4074 2020-01-29 02:12:45.000000 pyvizio-0.1.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-29 02:13:05.000000 pyvizio-0.1.9/pyvizio/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      116 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7913 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3014 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/cmd_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/cmd_pair.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      633 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/cmd_power.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      905 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/cmd_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2516 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/cmd_settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/const.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1491 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8273 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/protocol.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22327 2020-01-29 02:12:45.000000 pyvizio-0.1.9/pyvizio/vizio.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-29 02:13:05.000000 pyvizio-0.1.9/pyvizio.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5675 2020-01-29 02:13:04.000000 pyvizio-0.1.9/pyvizio.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      453 2020-01-29 02:13:04.000000 pyvizio-0.1.9/pyvizio.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-29 02:13:04.000000 pyvizio-0.1.9/pyvizio.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2020-01-29 02:13:04.000000 pyvizio-0.1.9/pyvizio.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-01-29 02:13:04.000000 pyvizio-0.1.9/pyvizio.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-01-29 02:13:04.000000 pyvizio-0.1.9/pyvizio.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      754 2020-01-29 02:13:05.000000 pyvizio-0.1.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1038 2020-01-29 02:12:45.000000 pyvizio-0.1.9/setup.py
```

### Comparing `pyvizio-0.1.8/PKG-INFO` & `pyvizio-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvizio
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library for interfacing with Vizio SmartCast TVs and Sound Bars (2016+ models)
 Home-page: https://github.com/vkorn/pyvizio
 Author: Vlad Korniev
 Author-email: vladimir.kornev@gmail.com
 License: GPLv3
 Description: | NOTE: The device type `soundbar` has been deprecated in favor of `speaker`. Support will be removed soon.
```

### Comparing `pyvizio-0.1.8/README.md` & `pyvizio-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio/cli.py` & `pyvizio-0.1.9/pyvizio/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,15 +163,14 @@
 
 @cli.command()
 @click.argument(
     "state",
     required=False,
     default="toggle",
     type=click.Choice(["toggle", "on", "off"]),
-    help="Type of power action",
 )
 @coro
 @pass_vizio
 async def power(vizio: VizioAsync, state: str) -> None:
     if "on" == state:
         txt = "Turning ON"
         result = await vizio.pow_on()
@@ -183,26 +182,18 @@
         result = await vizio.pow_toggle()
     _LOGGER.info(txt)
     _LOGGER.info("OK" if result else "ERROR")
 
 
 @cli.command()
 @click.argument(
-    "state",
-    required=False,
-    default="up",
-    type=click.Choice(["up", "down"]),
-    help="Direction to change the volume",
+    "state", required=False, default="up", type=click.Choice(["up", "down"])
 )
 @click.argument(
-    "amount",
-    required=False,
-    default=1,
-    type=click.IntRange(1, 100, clamp=True),
-    help="Number of steps to change the volume by",
+    "amount", required=False, default=1, type=click.IntRange(1, 100, clamp=True)
 )
 @coro
 @pass_vizio
 async def volume(vizio: VizioAsync, state: str, amount: int) -> None:
     if "up" == state:
         txt = "Increasing volume"
         result = await vizio.vol_up(amount)
@@ -229,22 +220,17 @@
 
 @cli.command()
 @click.argument(
     "state",
     required=False,
     default="previous",
     type=click.Choice(["up", "down", "previous"]),
-    help="Type of channel action",
 )
 @click.argument(
-    "amount",
-    required=False,
-    default=1,
-    type=click.IntRange(1, 100, clamp=True),
-    help="Number of steps to change the channel by",
+    "amount", required=False, default=1, type=click.IntRange(1, 100, clamp=True)
 )
 @coro
 @pass_vizio
 async def channel(vizio: VizioAsync, state: str, amount: str) -> None:
     amount = int(amount)
     if "up" == state:
         txt = "Channel up"
@@ -261,15 +247,14 @@
 
 @cli.command()
 @click.argument(
     "state",
     required=False,
     default="toggle",
     type=click.Choice(["toggle", "on", "off"]),
-    help="Type of mute action",
 )
 @coro
 @pass_vizio
 async def mute(vizio: VizioAsync, state: str) -> None:
     if "on" == state:
         txt = "Muting"
         result = await vizio.mute_on()
@@ -317,17 +302,15 @@
 @pass_vizio
 async def pause(vizio: VizioAsync) -> None:
     result = await vizio.pause()
     _LOGGER.info("OK" if result else "ERROR")
 
 
 @cli.command()
-@click.argument(
-    "key", required=True, type=click.STRING, help="Name of the key to press"
-)
+@click.argument("key", required=True, type=click.STRING)
 @coro
 @pass_vizio
 async def key_press(vizio: VizioAsync, key: str) -> None:
     _LOGGER.info("Emulating pressing of '%s' key", key)
     result = await vizio.remote(key.upper())
     _LOGGER.info("OK" if result else "ERROR")
```

### Comparing `pyvizio-0.1.8/pyvizio/cmd_input.py` & `pyvizio-0.1.9/pyvizio/cmd_input.py`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio/cmd_pair.py` & `pyvizio-0.1.9/pyvizio/cmd_pair.py`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio/cmd_power.py` & `pyvizio-0.1.9/pyvizio/cmd_power.py`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio/cmd_remote.py` & `pyvizio-0.1.9/pyvizio/cmd_remote.py`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio/cmd_settings.py` & `pyvizio-0.1.9/pyvizio/cmd_settings.py`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio/discovery.py` & `pyvizio-0.1.9/pyvizio/discovery.py`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio/protocol.py` & `pyvizio-0.1.9/pyvizio/protocol.py`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio/vizio.py` & `pyvizio-0.1.9/pyvizio/vizio.py`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/pyvizio.egg-info/PKG-INFO` & `pyvizio-0.1.9/pyvizio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvizio
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library for interfacing with Vizio SmartCast TVs and Sound Bars (2016+ models)
 Home-page: https://github.com/vkorn/pyvizio
 Author: Vlad Korniev
 Author-email: vladimir.kornev@gmail.com
 License: GPLv3
 Description: | NOTE: The device type `soundbar` has been deprecated in favor of `speaker`. Support will be removed soon.
```

### Comparing `pyvizio-0.1.8/setup.cfg` & `pyvizio-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvizio-0.1.8/setup.py` & `pyvizio-0.1.9/setup.py`

 * *Files identical despite different names*

