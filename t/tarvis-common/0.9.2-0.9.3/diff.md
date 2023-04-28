# Comparing `tmp/tarvis-common-0.9.2.tar.gz` & `tmp/tarvis-common-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-common-0.9.2.tar", last modified: Tue Apr 25 22:43:33 2023, max compression
+gzip compressed data, was "tarvis-common-0.9.3.tar", last modified: Fri Apr 28 07:53:28 2023, max compression
```

## Comparing `tarvis-common-0.9.2.tar` & `tarvis-common-0.9.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/common/asyncio/
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/common/cache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/common/cache/local/
--rw-r--r--   0 root         (0) root         (0)     3885 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/cache/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/config/
--rw-r--r--   0 root         (0) root         (0)     1696 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/environ/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/environ/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/logging/
--rw-r--r--   0 root         (0) root         (0)     5797 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/monitoring/
--rw-r--r--   0 root         (0) root         (0)     3789 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/secrets/
--rw-r--r--   0 root         (0) root         (0)     2551 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/secrets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/time/
--rw-r--r--   0 root         (0) root         (0)     6201 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/trading/
--rw-r--r--   0 root         (0) root         (0)     8247 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      523 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.643694 tarvis-common-0.9.3/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-28 07:53:28.643694 tarvis-common-0.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 07:53:28.643694 tarvis-common-0.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.635693 tarvis-common-0.9.3/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/asyncio/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.635693 tarvis-common-0.9.3/tarvis/common/cache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/cache/local/
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/cache/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/config/
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/environ/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/environ/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/logging/
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/monitoring/
+-rw-r--r--   0 root         (0) root         (0)     3678 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/secrets/
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/secrets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/time/
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.639694 tarvis-common-0.9.3/tarvis/common/trading/
+-rw-r--r--   0 root         (0) root         (0)     8247 2023-04-28 07:53:17.000000 tarvis-common-0.9.3/tarvis/common/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:53:28.643694 tarvis-common-0.9.3/tarvis_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-28 07:53:28.000000 tarvis-common-0.9.3/tarvis_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2023-04-28 07:53:28.000000 tarvis-common-0.9.3/tarvis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 07:53:28.000000 tarvis-common-0.9.3/tarvis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-28 07:53:28.000000 tarvis-common-0.9.3/tarvis_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 07:53:28.000000 tarvis-common-0.9.3/tarvis_common.egg-info/top_level.txt
```

### Comparing `tarvis-common-0.9.2/LICENSE.txt` & `tarvis-common-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.2/setup.py` & `tarvis-common-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-common",
-    version="0.9.2",
+    version="0.9.3",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Common Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-common-0.9.2/tarvis/common/asyncio/__init__.py` & `tarvis-common-0.9.3/tarvis/common/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.2/tarvis/common/cache/local/__init__.py` & `tarvis-common-0.9.3/tarvis/common/cache/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.2/tarvis/common/config/__init__.py` & `tarvis-common-0.9.3/tarvis/common/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dependency_injector import providers
 import logging
-import json
+import json5
 import os
 from tarvis.common import environ
 from tarvis.common.environ import PlatformType, DeploymentType
 
 
 class Configuration(providers.Configuration):
     def __init__(self, path: str = ".") -> None:
@@ -25,15 +25,15 @@
         if deployment is not None:
             file_name += "-" + DeploymentType(deployment).name.lower()
         file_name += ".json"
         file_name = os.path.join(path, file_name)
         if os.path.isfile(file_name):
             try:
                 with open(file_name, "r") as json_file:
-                    self.from_dict(json.load(json_file))
+                    self.from_dict(json5.load(json_file))
                 return True
             except:
                 logging.critical(f'Invalid configuration file "{file_name}"')
                 raise
         return False
 
     def _load_environmental_configs(self, path: str) -> bool:
```

### Comparing `tarvis-common-0.9.2/tarvis/common/environ/__init__.py` & `tarvis-common-0.9.3/tarvis/common/environ/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.2/tarvis/common/logging/__init__.py` & `tarvis-common-0.9.3/tarvis/common/logging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 _original_logger_log = _empty_function
 _gcp_extra = {}
 
 
 # Class to undo a workaround for GCP's structured logging when also logging elsewhere
 class CleanedStreamHandler(StreamHandler):
     def emit(self, record):
-        record = copy.deepcopy(record)
+        record = copy.copy(record)
         json_fields = record.__dict__.pop("json_fields", None)
         if json_fields is not None:
             for key, value in json_fields.items():
                 if key != "logging_client":
                     record.__dict__[key] = value
         super().emit(record)
```

### Comparing `tarvis-common-0.9.2/tarvis/common/monitoring/__init__.py` & `tarvis-common-0.9.3/tarvis/common/monitoring/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,34 +47,31 @@
             extra={"timeout": self._timeout, **self._extra},
         )
 
 
 class Watchdog:
 
     _POLL_INTERVAL = 0.1
-    _LIVENESS_FILE_NAME = "liveness"
 
     @inject
     def __init__(self, config: dict = Provide["config"]):
         self._running = False
         self._timers = []
         self._lock = Lock()
         watchdog_config = config.get("watchdog")
         if watchdog_config is None:
             self._enabled = True
             self._poll_interval = self._POLL_INTERVAL
-            self._liveness_file_name = self._LIVENESS_FILE_NAME
+            self._liveness_file_name = ""
         else:
             self._enabled = watchdog_config.get("enabled", True)
             self._poll_interval = watchdog_config.get(
                 "poll_interval", self._POLL_INTERVAL
             )
-            self._liveness_file_name = watchdog_config.get(
-                "liveness_file_name", self._LIVENESS_FILE_NAME
-            )
+            self._liveness_file_name = watchdog_config.get("liveness_file_name", "")
 
     def add_timer(self, timer: WatchdogTimer):
         with self._lock:
             timer._parent = self
             self._timers.append(timer)
             if self._enabled and (not self._running):
                 new_thread = Thread(target=self._run)
```

### Comparing `tarvis-common-0.9.2/tarvis/common/secrets/__init__.py` & `tarvis-common-0.9.3/tarvis/common/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.2/tarvis/common/time/__init__.py` & `tarvis-common-0.9.3/tarvis/common/time/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.2/tarvis/common/trading/__init__.py` & `tarvis-common-0.9.3/tarvis/common/trading/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.2/tarvis_common.egg-info/SOURCES.txt` & `tarvis-common-0.9.3/tarvis_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

