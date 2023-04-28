# Comparing `tmp/estimenergy-1.9.1.tar.gz` & `tmp/estimenergy-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimenergy-1.9.1.tar", max compression
+gzip compressed data, was "estimenergy-1.9.2.tar", max compression
```

## Comparing `estimenergy-1.9.1.tar` & `estimenergy-1.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1089 2023-03-10 12:19:14.715407 estimenergy-1.9.1/LICENSE
--rw-r--r--   0        0        0     2705 2023-03-10 12:19:14.715407 estimenergy-1.9.1/README.md
--rw-r--r--   0        0        0        0 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/__init__.py
--rw-r--r--   0        0        0       37 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/client/__init__.py
--rw-r--r--   0        0        0      972 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/client/client.py
--rw-r--r--   0        0        0       74 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/collectors/__init__.py
--rw-r--r--   0        0        0      238 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/collectors/collector.py
--rw-r--r--   0        0        0     4431 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/collectors/glow_collector.py
--rw-r--r--   0        0        0      598 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/common.py
--rw-r--r--   0        0        0     4896 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/const.py
--rw-r--r--   0        0        0      582 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/helpers.py
--rw-r--r--   0        0        0     2468 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/main.py
--rw-r--r--   0        0        0       47 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/metrics/__init__.py
--rw-r--r--   0        0        0      873 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/metrics/collector_metrics.py
--rw-r--r--   0        0        0      110 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/models/__init__.py
--rw-r--r--   0        0        0     6861 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/models/collector_data.py
--rw-r--r--   0        0        0      711 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/models/energy_data.py
--rw-r--r--   0        0        0      381 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/models/settings.py
--rw-r--r--   0        0        0        0 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/routers/__init__.py
--rw-r--r--   0        0        0      270 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/routers/collector_router.py
--rw-r--r--   0        0        0      255 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/routers/energy_router.py
--rw-r--r--   0        0        0       85 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/schemas/__init__.py
--rw-r--r--   0        0        0      184 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/schemas/collector_schema.py
--rw-r--r--   0        0        0      172 2023-03-10 12:19:14.715407 estimenergy-1.9.1/estimenergy/schemas/energy_schema.py
--rw-r--r--   0        0        0     1173 2023-03-10 12:19:38.303381 estimenergy-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 estimenergy-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-03-10 13:35:51.710370 estimenergy-1.9.2/LICENSE
+-rw-r--r--   0        0        0     2705 2023-03-10 13:35:51.710370 estimenergy-1.9.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/__init__.py
+-rw-r--r--   0        0        0       37 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/client/__init__.py
+-rw-r--r--   0        0        0      972 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/client/client.py
+-rw-r--r--   0        0        0       74 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/collectors/__init__.py
+-rw-r--r--   0        0        0      238 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/collectors/collector.py
+-rw-r--r--   0        0        0     4461 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/collectors/glow_collector.py
+-rw-r--r--   0        0        0      598 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/common.py
+-rw-r--r--   0        0        0     4896 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/const.py
+-rw-r--r--   0        0        0      582 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/helpers.py
+-rw-r--r--   0        0        0     2468 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/main.py
+-rw-r--r--   0        0        0       47 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/metrics/__init__.py
+-rw-r--r--   0        0        0      873 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/metrics/collector_metrics.py
+-rw-r--r--   0        0        0      110 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/models/__init__.py
+-rw-r--r--   0        0        0     6861 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/models/collector_data.py
+-rw-r--r--   0        0        0      711 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/models/energy_data.py
+-rw-r--r--   0        0        0      381 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/models/settings.py
+-rw-r--r--   0        0        0        0 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/routers/__init__.py
+-rw-r--r--   0        0        0      270 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/routers/collector_router.py
+-rw-r--r--   0        0        0      255 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/routers/energy_router.py
+-rw-r--r--   0        0        0       85 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/schemas/__init__.py
+-rw-r--r--   0        0        0      184 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/schemas/collector_schema.py
+-rw-r--r--   0        0        0      172 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/schemas/energy_schema.py
+-rw-r--r--   0        0        0     1173 2023-03-10 13:36:19.246579 estimenergy-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 estimenergy-1.9.2/PKG-INFO
```

### Comparing `estimenergy-1.9.1/LICENSE` & `estimenergy-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/README.md` & `estimenergy-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/estimenergy/client/client.py` & `estimenergy-1.9.2/estimenergy/client/client.py`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/estimenergy/collectors/glow_collector.py` & `estimenergy-1.9.2/estimenergy/collectors/glow_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,18 @@
 
         try:
             await self.api.subscribe_states(self.__state_changed)
         except APIConnectionError as err:
             await self.api.disconnect()
     
     async def __on_disconnect(self):
-        self.logger.warn(f"Disconnected from ESPHome Device {self.name}")
+        self.logger.warn(f"Disconnected from ESPHome Device {self.collector_data.name}")
 
     async def __on_connect_error(self, exception: Exception):
-        self.logger.error(f"Error connecting to ESPHome Device {self.name}")
+        self.logger.error(f"Error connecting to ESPHome Device {self.collector_data.name}")
         self.logger.error(exception)
 
     def __state_changed(self, state: EntityState):
         if not state.key == 3673186328:
             return
         
         current_kwh: float = state.state
```

### Comparing `estimenergy-1.9.1/estimenergy/common.py` & `estimenergy-1.9.2/estimenergy/common.py`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/estimenergy/const.py` & `estimenergy-1.9.2/estimenergy/const.py`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/estimenergy/helpers.py` & `estimenergy-1.9.2/estimenergy/helpers.py`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/estimenergy/main.py` & `estimenergy-1.9.2/estimenergy/main.py`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/estimenergy/metrics/collector_metrics.py` & `estimenergy-1.9.2/estimenergy/metrics/collector_metrics.py`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/estimenergy/models/collector_data.py` & `estimenergy-1.9.2/estimenergy/models/collector_data.py`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/estimenergy/models/energy_data.py` & `estimenergy-1.9.2/estimenergy/models/energy_data.py`

 * *Files identical despite different names*

### Comparing `estimenergy-1.9.1/pyproject.toml` & `estimenergy-1.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = "estimenergy"
 description = "Estimate Energy Consumption"
 authors = ["Lennard Beers <l.beers@outlook.de>"]
 repository = "https://github.com/EuleMitKeule/EstimEnergy"
 readme = "README.md"
 packages = [{include = "estimenergy"}]
 license = "MIT"
-version = "1.9.1"
+version = "1.9.2"
 
 [tool.poetry.scripts]
 api = "estimenergy.main:start"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `estimenergy-1.9.1/PKG-INFO` & `estimenergy-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimenergy
-Version: 1.9.1
+Version: 1.9.2
 Summary: Estimate Energy Consumption
 Home-page: https://github.com/EuleMitKeule/EstimEnergy
 License: MIT
 Author: Lennard Beers
 Author-email: l.beers@outlook.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

