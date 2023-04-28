# Comparing `tmp/resotoworker-3.4.0.tar.gz` & `tmp/resotoworker-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.4.0.tar", last modified: Thu Apr 27 11:24:42 2023, max compression
+gzip compressed data, was "resotoworker-3.4.1.tar", last modified: Fri Apr 28 15:17:01 2023, max compression
```

## Comparing `resotoworker-3.4.0.tar` & `resotoworker-3.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:42.280683 resotoworker-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:22:30.000000 resotoworker-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-27 11:24:42.280683 resotoworker-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-27 11:22:30.000000 resotoworker-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-27 11:22:30.000000 resotoworker-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:42.272683 resotoworker-3.4.0/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:42.276683 resotoworker-3.4.0/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:24:42.280683 resotoworker-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-27 11:22:30.000000 resotoworker-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:42.280683 resotoworker-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:01.656600 resotoworker-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:14:50.000000 resotoworker-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-28 15:17:01.656600 resotoworker-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-28 15:14:50.000000 resotoworker-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 15:14:50.000000 resotoworker-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:01.656600 resotoworker-3.4.1/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:01.656600 resotoworker-3.4.1/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:17:01.656600 resotoworker-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-28 15:14:50.000000 resotoworker-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:01.656600 resotoworker-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/test_utils.py
```

### Comparing `resotoworker-3.4.0/PKG-INFO` & `resotoworker-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.4.0
+Version: 3.4.1
 Summary: Runs collector plugins and sends the result to resotocore.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoworker
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -95,15 +95,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotoworker-3.4.0/README.md` & `resotoworker-3.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotoworker-3.4.0/resotoworker/__main__.py` & `resotoworker-3.4.1/resotoworker/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             plugin.start()
         except Exception as e:
             log.exception(f"Caught unhandled persistent Plugin exception {e}")
 
     # We wait for the shutdown Event to be set() and then end the program
     # While doing so we print the list of active threads once per 15 minutes
     shutdown_event.wait()
-    web_server.shutdown()  # type: ignore
+    web_server.shutdown()
     time.sleep(1)  # everything gets 1000ms to shutdown gracefully before we force it
     resotolib.proc.kill_children(SIGTERM, ensure_death=True)
     log.info("Shutdown complete")
     os._exit(0)
 
 
 def core_actions_processor(
@@ -267,15 +267,15 @@
             "data": data,
         }
         return reply_message
     return None
 
 
 def shutdown(event: Event) -> None:
-    reason = event.data.get("reason")
+    reason = str(event.data.get("reason"))
     emergency = event.data.get("emergency")
 
     if emergency:
         resotolib.proc.emergency_shutdown(reason)
 
     current_pid = os.getpid()
     if current_pid != resotolib.proc.parent_pid:
```

### Comparing `resotoworker-3.4.0/resotoworker/cleanup.py` & `resotoworker-3.4.1/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/resotoworker/collect.py` & `resotoworker-3.4.1/resotoworker/collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/resotoworker/config.py` & `resotoworker-3.4.1/resotoworker/config.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/resotoworker/pluginloader.py` & `resotoworker-3.4.1/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/resotoworker/resotocore.py` & `resotoworker-3.4.1/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/resotoworker/tag.py` & `resotoworker-3.4.1/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/resotoworker/utils.py` & `resotoworker-3.4.1/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.4.1/resotoworker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.4.0
+Version: 3.4.1
 Summary: Runs collector plugins and sends the result to resotocore.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoworker
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -95,15 +95,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotoworker-3.4.0/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.4.1/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/setup.py` & `resotoworker-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/test/test_collect.py` & `resotoworker-3.4.1/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/test/test_resotocore.py` & `resotoworker-3.4.1/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.0/test/test_utils.py` & `resotoworker-3.4.1/test/test_utils.py`

 * *Files identical despite different names*

