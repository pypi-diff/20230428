# Comparing `tmp/varvault-6.0.0.tar.gz` & `tmp/varvault-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvault-6.0.0.tar", last modified: Wed Apr 26 14:12:48 2023, max compression
+gzip compressed data, was "varvault-6.0.1.tar", last modified: Fri Apr 28 12:36:00 2023, max compression
```

## Comparing `varvault-6.0.0.tar` & `varvault-6.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-26 14:12:48.849854 varvault-6.0.0/
--rw-r--r--   0 chloe      (501) staff       (20)    11357 2021-11-12 15:14:41.000000 varvault-6.0.0/LICENSE
--rw-r--r--   0 chloe      (501) staff       (20)    10885 2023-04-26 14:12:48.849532 varvault-6.0.0/PKG-INFO
--rw-r--r--   0 chloe      (501) staff       (20)    10377 2023-04-24 18:48:06.000000 varvault-6.0.0/README.md
--rw-r--r--   0 chloe      (501) staff       (20)       38 2023-04-26 14:12:48.849942 varvault-6.0.0/setup.cfg
--rw-r--r--   0 chloe      (501) staff       (20)     2868 2023-04-24 06:37:05.000000 varvault-6.0.0/setup.py
-drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-26 14:12:48.843066 varvault-6.0.0/tests/
--rw-r--r--   0 chloe      (501) staff       (20)    15646 2023-04-24 18:16:29.000000 varvault-6.0.0/tests/test_automatic.py
--rw-r--r--   0 chloe      (501) staff       (20)    18858 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_large_scale_vault.py
--rw-r--r--   0 chloe      (501) staff       (20)     4944 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_live_update.py
--rw-r--r--   0 chloe      (501) staff       (20)    11049 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_logging.py
--rw-r--r--   0 chloe      (501) staff       (20)    12664 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_structs.py
--rw-r--r--   0 chloe      (501) staff       (20)    51616 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_vault.py
--rw-r--r--   0 chloe      (501) staff       (20)     4427 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_xml_vault.py
-drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-26 14:12:48.847468 varvault-6.0.0/varvault/
--rw-r--r--   0 chloe      (501) staff       (20)     4983 2023-04-24 06:37:05.000000 varvault-6.0.0/varvault/__init__.py
--rw-r--r--   0 chloe      (501) staff       (20)     3547 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/factory.py
--rw-r--r--   0 chloe      (501) staff       (20)     5609 2023-04-24 18:16:29.000000 varvault-6.0.0/varvault/flags.py
--rw-r--r--   0 chloe      (501) staff       (20)     7154 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/keyring.py
--rw-r--r--   0 chloe      (501) staff       (20)     2604 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/logger.py
--rw-r--r--   0 chloe      (501) staff       (20)     1627 2023-01-13 12:55:44.000000 varvault-6.0.0/varvault/minivault.py
--rw-r--r--   0 chloe      (501) staff       (20)    11207 2023-04-24 06:37:05.000000 varvault-6.0.0/varvault/resource.py
--rw-r--r--   0 chloe      (501) staff       (20)      520 2023-04-24 06:37:06.000000 varvault-6.0.0/varvault/subscriber_thread.py
--rw-r--r--   0 chloe      (501) staff       (20)     2155 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/utils.py
--rw-r--r--   0 chloe      (501) staff       (20)     5385 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/validator.py
--rw-r--r--   0 chloe      (501) staff       (20)    40136 2023-04-24 18:53:37.000000 varvault-6.0.0/varvault/vault.py
--rw-r--r--   0 chloe      (501) staff       (20)      930 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/vaultstructs.py
-drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-26 14:12:48.849195 varvault-6.0.0/varvault.egg-info/
--rw-r--r--   0 chloe      (501) staff       (20)    10885 2023-04-26 14:12:48.000000 varvault-6.0.0/varvault.egg-info/PKG-INFO
--rw-r--r--   0 chloe      (501) staff       (20)      578 2023-04-26 14:12:48.000000 varvault-6.0.0/varvault.egg-info/SOURCES.txt
--rw-r--r--   0 chloe      (501) staff       (20)        1 2023-04-26 14:12:48.000000 varvault-6.0.0/varvault.egg-info/dependency_links.txt
--rw-r--r--   0 chloe      (501) staff       (20)        9 2023-04-26 14:12:48.000000 varvault-6.0.0/varvault.egg-info/top_level.txt
+drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-28 12:36:00.929476 varvault-6.0.1/
+-rw-r--r--   0 chloe      (501) staff       (20)    11357 2021-11-12 15:14:41.000000 varvault-6.0.1/LICENSE
+-rw-r--r--   0 chloe      (501) staff       (20)    10885 2023-04-28 12:36:00.928975 varvault-6.0.1/PKG-INFO
+-rw-r--r--   0 chloe      (501) staff       (20)    10377 2023-04-24 18:48:06.000000 varvault-6.0.1/README.md
+-rw-r--r--   0 chloe      (501) staff       (20)       38 2023-04-28 12:36:00.929613 varvault-6.0.1/setup.cfg
+-rw-r--r--   0 chloe      (501) staff       (20)     2868 2023-04-28 12:30:49.000000 varvault-6.0.1/setup.py
+drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-28 12:36:00.918785 varvault-6.0.1/tests/
+-rw-r--r--   0 chloe      (501) staff       (20)    19401 2023-04-28 12:26:33.000000 varvault-6.0.1/tests/test_automatic.py
+-rw-r--r--   0 chloe      (501) staff       (20)    18858 2023-04-24 06:37:05.000000 varvault-6.0.1/tests/test_large_scale_vault.py
+-rw-r--r--   0 chloe      (501) staff       (20)     4944 2023-04-24 06:37:05.000000 varvault-6.0.1/tests/test_live_update.py
+-rw-r--r--   0 chloe      (501) staff       (20)    11049 2023-04-24 06:37:05.000000 varvault-6.0.1/tests/test_logging.py
+-rw-r--r--   0 chloe      (501) staff       (20)    12664 2023-04-24 06:37:05.000000 varvault-6.0.1/tests/test_structs.py
+-rw-r--r--   0 chloe      (501) staff       (20)    51616 2023-04-24 06:37:05.000000 varvault-6.0.1/tests/test_vault.py
+-rw-r--r--   0 chloe      (501) staff       (20)     4427 2023-04-24 06:37:05.000000 varvault-6.0.1/tests/test_xml_vault.py
+drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-28 12:36:00.925582 varvault-6.0.1/varvault/
+-rw-r--r--   0 chloe      (501) staff       (20)     4983 2023-04-28 12:30:49.000000 varvault-6.0.1/varvault/__init__.py
+-rw-r--r--   0 chloe      (501) staff       (20)     3547 2022-12-05 20:24:44.000000 varvault-6.0.1/varvault/factory.py
+-rw-r--r--   0 chloe      (501) staff       (20)     5609 2023-04-24 18:16:29.000000 varvault-6.0.1/varvault/flags.py
+-rw-r--r--   0 chloe      (501) staff       (20)     7154 2022-12-05 20:24:44.000000 varvault-6.0.1/varvault/keyring.py
+-rw-r--r--   0 chloe      (501) staff       (20)     2604 2022-12-05 20:24:44.000000 varvault-6.0.1/varvault/logger.py
+-rw-r--r--   0 chloe      (501) staff       (20)     1627 2023-01-13 12:55:44.000000 varvault-6.0.1/varvault/minivault.py
+-rw-r--r--   0 chloe      (501) staff       (20)    11207 2023-04-24 06:37:05.000000 varvault-6.0.1/varvault/resource.py
+-rw-r--r--   0 chloe      (501) staff       (20)      521 2023-04-28 12:29:41.000000 varvault-6.0.1/varvault/subscriber_thread.py
+-rw-r--r--   0 chloe      (501) staff       (20)     2155 2022-12-05 20:24:44.000000 varvault-6.0.1/varvault/utils.py
+-rw-r--r--   0 chloe      (501) staff       (20)     5385 2022-12-05 20:24:44.000000 varvault-6.0.1/varvault/validator.py
+-rw-r--r--   0 chloe      (501) staff       (20)    40745 2023-04-28 12:29:41.000000 varvault-6.0.1/varvault/vault.py
+-rw-r--r--   0 chloe      (501) staff       (20)      930 2022-12-05 20:24:44.000000 varvault-6.0.1/varvault/vaultstructs.py
+drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-28 12:36:00.928350 varvault-6.0.1/varvault.egg-info/
+-rw-r--r--   0 chloe      (501) staff       (20)    10885 2023-04-28 12:36:00.000000 varvault-6.0.1/varvault.egg-info/PKG-INFO
+-rw-r--r--   0 chloe      (501) staff       (20)      578 2023-04-28 12:36:00.000000 varvault-6.0.1/varvault.egg-info/SOURCES.txt
+-rw-r--r--   0 chloe      (501) staff       (20)        1 2023-04-28 12:36:00.000000 varvault-6.0.1/varvault.egg-info/dependency_links.txt
+-rw-r--r--   0 chloe      (501) staff       (20)        9 2023-04-28 12:36:00.000000 varvault-6.0.1/varvault.egg-info/top_level.txt
```

### Comparing `varvault-6.0.0/LICENSE` & `varvault-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/PKG-INFO` & `varvault-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvault
-Version: 6.0.0
+Version: 6.0.1
 Summary: A package that sets up a key-value vault to store and access variables in a global context.
 Home-page: https://github.com/data-ductus/varvault
 Author: Chloe Holst
 Author-email: chloe.holst@dataductus.se
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `varvault-6.0.0/README.md` & `varvault-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/setup.py` & `varvault-6.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # The text of the README file
 README = pathlib.Path(f"{HERE}/README.md").read_text()
 
 # Version handling
 # A good way to tell if we are backwards compatible is to run the test suite and if the tests pass without requiring any changes, we can pretty safely assume we are backwards compatible.
 MAJOR = 6  # Change this if the previous MAJOR is incompatible with this build. Set MINOR and PATCH to 0
 MINOR = 0  # Change this if the functionality has changed, but we are still backwards compatible with previous MINOR versions. Set PATCH to 0
-PATCH = 0  # Change this is if we are fixing a bug that doesn't change the functionality. If a bug-fix has caused functionality to be changed, see MINOR instead
+PATCH = 1  # Change this is if we are fixing a bug that doesn't change the functionality. If a bug-fix has caused functionality to be changed, see MINOR instead
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 
 assert varvault.__version__ == VERSION, f"Version mismatch: {varvault.__version__} != {VERSION}"
 
 
 def find_todos_for_version_in_code():
```

### Comparing `varvault-6.0.0/tests/test_automatic.py` & `varvault-6.0.1/tests/test_automatic.py`

 * *Files 12% similar despite different names*

```diff
@@ -111,38 +111,47 @@
 
         # All functions should have been called
         assert called
 
     def test_subscriber_threaded(self):
         vault = varvault.create(keyring=KeyringSubscriber, resource=varvault.JsonResource(vault_file_new, mode="w"))
         called_first = False
+        num_calls_first = 0
         called_second = False
+        num_calls_second = 0
         called_third = False
+        num_calls_third = 0
         sleep_dur = 2
 
         @vault.automatic(threaded=True, input=KeyringSubscriber.trigger, output=KeyringSubscriber.first)
         def one(**kwargs):
             logger.info("one")
             nonlocal called_first
+            nonlocal num_calls_first
+            num_calls_first += 1
             called_first = True
             time.sleep(sleep_dur)
             return "first"
 
         @vault.automatic(threaded=True, input=KeyringSubscriber.trigger, output=KeyringSubscriber.second)
         def two(**kwargs):
             logger.info("two")
             nonlocal called_second
+            nonlocal num_calls_second
+            num_calls_second += 1
             called_second = True
             time.sleep(sleep_dur)
             return "second"
 
         @vault.automatic(threaded=True, input=KeyringSubscriber.trigger, output=KeyringSubscriber.third)
         def three(**kwargs):
             logger.info("three")
             nonlocal called_third
+            nonlocal num_calls_third
+            num_calls_third += 1
             called_third = True
             time.sleep(sleep_dur)
             return "third"
 
         @vault.manual(output=KeyringSubscriber.trigger)
         def start():
             return "go"
@@ -162,20 +171,96 @@
 
         assert len(vault.running_tasks) == 0, "All tasks should have completed and not be listed as running"
         # All functions should have been called
         assert called_first and vault.get(KeyringSubscriber.first) == "first"
         assert called_second and vault.get(KeyringSubscriber.second) == "second"
         assert called_third and vault.get(KeyringSubscriber.third) == "third"
 
+        assert num_calls_first == 1
+        assert num_calls_second == 1
+        assert num_calls_third == 1
+
         with pytest.raises(ValueError) as e:
             @vault.automatic()
             async def async_func():
                 pass
         assert f"Async subscriber functions do not work because async functions cannot truly run in the background. Use {vault.automatic.__name__} with 'threaded=True' instead." in str(e.value)
 
+    def test_subscriber_threaded_existing_vault(self):
+        vault = varvault.create(keyring=KeyringSubscriber, resource=varvault.JsonResource(vault_file_new, mode="w"))
+        vault.insert(KeyringSubscriber.trigger, "go")
+
+        called_first = False
+        num_calls_first = 0
+        called_second = False
+        num_calls_second = 0
+        called_third = False
+        num_calls_third = 0
+        sleep_dur = 2
+
+        vault_recreated = varvault.create(keyring=KeyringSubscriber, resource=varvault.JsonResource(vault_file_new, mode="a"))
+
+        @vault_recreated.automatic(threaded=True, input=KeyringSubscriber.trigger, output=KeyringSubscriber.first)
+        def one(**kwargs):
+            logger.info("one")
+            nonlocal called_first
+            nonlocal num_calls_first
+            num_calls_first += 1
+            called_first = True
+            time.sleep(sleep_dur)
+            return "first"
+
+        @vault_recreated.automatic(threaded=True, input=KeyringSubscriber.trigger, output=KeyringSubscriber.second)
+        def two(**kwargs):
+            logger.info("two")
+            nonlocal called_second
+            nonlocal num_calls_second
+            num_calls_second += 1
+            called_second = True
+            time.sleep(sleep_dur)
+            return "second"
+
+        @vault_recreated.automatic(threaded=True, input=KeyringSubscriber.trigger, output=KeyringSubscriber.third)
+        def three(**kwargs):
+            logger.info("three")
+            nonlocal called_third
+            nonlocal num_calls_third
+            num_calls_third += 1
+            called_third = True
+            time.sleep(sleep_dur)
+            logger.info("three done")
+            return "third"
+
+        @vault_recreated.automatic(input=(KeyringSubscriber.first, KeyringSubscriber.second, KeyringSubscriber.third),
+                                   output=KeyringSubscriber.final)
+        def final(first, second, third):
+            return first + second + third
+
+        # If this fails, it's probably due to I/O contention. Try increasing the sleep duration.
+        # KeyringSubscriber.final will be written to the vault sooner than it seems, but the different automatic functions
+        # will lock the vault when they write, so a short sleep will mean the effect of I/O has a larger impact on the result.
+        # Try increasing and lowering the sleep duration to see how it affects the duration of the test.
+
+        logger.info("Waiting for final...")
+        while KeyringSubscriber.final not in vault_recreated:
+            pass
+        logger.info("Final value found in vault")
+
+        vault_recreated.await_running_tasks(timeout=sleep_dur * 3, exception=TimeoutError(f"All tasks should have completed within {sleep_dur * 3} seconds. Methods appear to run in sequence"))
+
+        assert len(vault_recreated.running_tasks) == 0, "All tasks should have completed and not be listed as running"
+        # All functions should have been called
+        assert called_first and vault_recreated.get(KeyringSubscriber.first) == "first"
+        assert called_second and vault_recreated.get(KeyringSubscriber.second) == "second"
+        assert called_third and vault_recreated.get(KeyringSubscriber.third) == "third"
+
+        assert num_calls_first == 1
+        assert num_calls_second == 1
+        assert num_calls_third == 1
+
     def test_subscriber_with_existing_vault(self):
         vault = varvault.create(keyring=KeyringSubscriber, resource=varvault.JsonResource(vault_file_new, mode="w"))
         vault.insert(KeyringSubscriber.trigger, "go")
 
         vault_recreated = varvault.create(keyring=KeyringSubscriber, resource=varvault.JsonResource(vault_file_new, mode="a"))
 
         # Registering this subscriber will not trigger the function since the vault does not have the relevant keys yet, but will receive them
```

### Comparing `varvault-6.0.0/tests/test_large_scale_vault.py` & `varvault-6.0.1/tests/test_large_scale_vault.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/tests/test_live_update.py` & `varvault-6.0.1/tests/test_live_update.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/tests/test_logging.py` & `varvault-6.0.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/tests/test_structs.py` & `varvault-6.0.1/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/tests/test_vault.py` & `varvault-6.0.1/tests/test_vault.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/tests/test_xml_vault.py` & `varvault-6.0.1/tests/test_xml_vault.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/__init__.py` & `varvault-6.0.1/varvault/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "6.0.0"
+__version__ = "6.0.1"
 
 import os
 import json
 
 from typing import Dict, TextIO, AnyStr, Literal, Union
 
 from .resource import ResourceModes
```

### Comparing `varvault-6.0.0/varvault/factory.py` & `varvault-6.0.1/varvault/factory.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/flags.py` & `varvault-6.0.1/varvault/flags.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/keyring.py` & `varvault-6.0.1/varvault/keyring.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/logger.py` & `varvault-6.0.1/varvault/logger.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/minivault.py` & `varvault-6.0.1/varvault/minivault.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/resource.py` & `varvault-6.0.1/varvault/resource.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/subscriber_thread.py` & `varvault-6.0.1/varvault/subscriber_thread.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,11 +5,11 @@
     def __init__(self, subscriber, varvault, *args, **kwargs):
         super(SubscriberThread, self).__init__(*args, **kwargs)
         self.subscriber = subscriber
         self.varvault = varvault
 
     def run(self):
         from .vault import VarVault
-        self.varvault.logger.info(f"Starting subscriber thread for {self.subscriber.__name__}...")
+        self.varvault.logger.debug(f"Starting subscriber thread for {self.subscriber.__name__}...")
         self.subscriber()
         self.varvault: VarVault
         self.varvault.purge_stopped_thread(self)
```

### Comparing `varvault-6.0.0/varvault/utils.py` & `varvault-6.0.1/varvault/utils.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/validator.py` & `varvault-6.0.1/varvault/validator.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault/vault.py` & `varvault-6.0.1/varvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,22 +342,22 @@
             self.keys_used_by_automatics[f] = list()
             self.automatic_conditionals[f] = condition
             for key in input:
                 if key not in self.functions_as_automatics:
                     self.functions_as_automatics[key] = list()
                 self.functions_as_automatics[key].append(f)
                 self.keys_used_by_automatics[f].append(key)
-            self._dispatch_subscribers(input)
+            self._dispatch_subscriber(f, input, threaded)
             return f
 
         return wrap_outer
 
     def purge_stopped_thread(self, subscriber_thread: SubscriberThread):
         if subscriber_thread in self.running_tasks:
-            self.logger.info(f"Removing stopped thread {subscriber_thread} from the running tasks")
+            self.logger.debug(f"Removing stopped thread for {subscriber_thread.subscriber.__name__} from the running tasks")
             self.running_tasks.remove(subscriber_thread)
 
     # ============================================================
     # insert
     # ============================================================
     def insert(self, key: Key, value: object, *flags: Flags):
         f"""
@@ -684,20 +684,35 @@
                 conditional: Callable = self.automatic_conditionals[function]
                 if conditional():
                     if function in self.threaded_automatics:
                         threaded_functions_to_dispatch.add(function)
                     else:
                         functions_to_dispatch.add(function)
         for function in threaded_functions_to_dispatch:
+            self._dispatch_subscriber(function, keys, threaded=True)
+
+        for function in functions_to_dispatch:
+            self._dispatch_subscriber(function, keys, threaded=False)
+
+    def _dispatch_subscriber(self, function: Callable, keys: List[Key], threaded: bool):
+        if not all(key in self for key in keys):
+            # May not dispatch; not all keys exist in the vault
+            return
+
+        conditional: Callable = self.automatic_conditionals[function]
+        if not conditional():
+            # May not dispatch; conditional is not met
+            return
+
+        if threaded:
             # Dispatch threaded functions.
             thread = SubscriberThread(function, self)
             self.running_tasks.add(thread)
             thread.start()
-
-        for function in functions_to_dispatch:
+        else:
             # Dispatch the function.
             function()
 
     def _get_all_flags(self, *flags):
         self._assert_flag_is_correct_type(*flags)
         all_flags = self.flags.copy()
         all_flags.update(flags)
```

### Comparing `varvault-6.0.0/varvault/vaultstructs.py` & `varvault-6.0.1/varvault/vaultstructs.py`

 * *Files identical despite different names*

### Comparing `varvault-6.0.0/varvault.egg-info/PKG-INFO` & `varvault-6.0.1/varvault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvault
-Version: 6.0.0
+Version: 6.0.1
 Summary: A package that sets up a key-value vault to store and access variables in a global context.
 Home-page: https://github.com/data-ductus/varvault
 Author: Chloe Holst
 Author-email: chloe.holst@dataductus.se
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `varvault-6.0.0/varvault.egg-info/SOURCES.txt` & `varvault-6.0.1/varvault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

