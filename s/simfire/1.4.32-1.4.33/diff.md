# Comparing `tmp/simfire-1.4.32.tar.gz` & `tmp/simfire-1.4.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfire-1.4.32.tar", max compression
+gzip compressed data, was "simfire-1.4.33.tar", max compression
```

## Comparing `simfire-1.4.32.tar` & `simfire-1.4.33.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    10789 2023-04-06 02:10:59.176490 simfire-1.4.32/LICENSE
--rw-r--r--   0        0        0     2688 2023-04-06 02:10:59.176490 simfire-1.4.32/README.md
--rw-r--r--   0        0        0     1824 2023-04-06 02:10:59.372492 simfire-1.4.32/pyproject.toml
--rw-r--r--   0        0        0     1111 2023-04-06 02:10:59.372492 simfire-1.4.32/simfire/__init__.py
--rw-r--r--   0        0        0    10646 2023-04-06 02:10:59.372492 simfire-1.4.32/simfire/enums.py
--rw-r--r--   0        0        0       37 2023-04-06 02:10:59.372492 simfire-1.4.32/simfire/game/__init__.py
--rw-r--r--   0        0        0      874 2023-04-06 02:10:59.372492 simfire-1.4.32/simfire/game/_tests/__init__.py
--rw-r--r--   0        0        0    15523 2023-04-06 02:10:59.372492 simfire-1.4.32/simfire/game/_tests/test_game.py
--rw-r--r--   0        0        0     9928 2023-04-06 02:10:59.372492 simfire-1.4.32/simfire/game/_tests/test_sprites.py
--rw-r--r--   0        0        0    14937 2023-04-06 02:10:59.372492 simfire-1.4.32/simfire/game/game.py
--rw-r--r--   0        0        0     1318 2023-04-06 02:10:59.372492 simfire-1.4.32/simfire/game/image.py
--rw-r--r--   0        0        0      379 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/game/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/game/managers/_tests/__init__.py
--rw-r--r--   0        0        0    18385 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/game/managers/_tests/test_fire.py
--rw-r--r--   0        0        0     8301 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/game/managers/_tests/test_mitigation.py
--rw-r--r--   0        0        0    29762 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/game/managers/fire.py
--rw-r--r--   0        0        0     7321 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/game/managers/mitigation.py
--rw-r--r--   0        0        0    15972 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/game/sprites.py
--rw-r--r--   0        0        0       49 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/sim/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/sim/_tests/__init__.py
--rw-r--r--   0        0        0    14392 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/sim/_tests/test_simulation.py
--rw-r--r--   0        0        0    37791 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/sim/simulation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/__init__.py
--rw-r--r--   0        0        0     2378 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_config.py
--rw-r--r--   0        0        0     1875 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_configs/test_config.yml
--rw-r--r--   0        0        0       47 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_configs/test_config_bad.yml
--rw-r--r--   0        0        0     1824 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
--rw-r--r--   0        0        0     1826 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_configs/test_config_gaussian.yml
--rw-r--r--   0        0        0     1801 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
--rw-r--r--   0        0        0     4693 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_graph.py
--rw-r--r--   0        0        0    16597 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_layers.py
--rw-r--r--   0        0        0      622 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_log.py
--rw-r--r--   0        0        0     2537 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_terrain.py
--rw-r--r--   0        0        0     1472 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/_tests/test_units.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/assets/__init__.py
--rw-r--r--   0        0        0     1854 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/assets/fireline_logo.png
--rw-r--r--   0        0        0    37679 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/config.py
--rw-r--r--   0        0        0      499 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/decorators.py
--rw-r--r--   0        0        0     4153 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/generate_cfd_wind_layer.py
--rw-r--r--   0        0        0    10189 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/graph.py
--rw-r--r--   0        0        0    50730 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/layers.py
--rw-r--r--   0        0        0     2030 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/log.py
--rw-r--r--   0        0        0   143776 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
--rw-r--r--   0        0        0   143776 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
--rw-r--r--   0        0        0     2248 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/terrain.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/textures/__init__.py
--rw-r--r--   0        0        0   204702 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/textures/terrain.jpg
--rw-r--r--   0        0        0     2555 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/utils/units.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/world/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/world/_tests/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/world/_tests/test_cfd_wind.py
--rw-r--r--   0        0        0     2423 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/world/_tests/test_elevation_functions.py
--rw-r--r--   0        0        0     2821 2023-04-06 02:10:59.376492 simfire-1.4.32/simfire/world/_tests/test_rothermel.py
--rw-r--r--   0        0        0     1466 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/_tests/test_wind.py
--rw-r--r--   0        0        0     3703 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/elevation_functions.py
--rw-r--r--   0        0        0     1054 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/fuel_array_functions.py
--rw-r--r--   0        0        0     2306 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/parameters.py
--rw-r--r--   0        0        0     2083 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/presets.py
--rw-r--r--   0        0        0     4306 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/rothermel.py
--rw-r--r--   0        0        0        0 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/wind_mechanics/__init__.py
--rw-r--r--   0        0        0     8781 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/wind_mechanics/cfd_wind.py
--rw-r--r--   0        0        0     3132 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/wind_mechanics/perlin_wind.py
--rw-r--r--   0        0        0     6578 2023-04-06 02:10:59.380492 simfire-1.4.32/simfire/world/wind_mechanics/wind_controller.py
--rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 simfire-1.4.32/PKG-INFO
+-rw-r--r--   0        0        0    10789 2023-04-28 04:45:12.821836 simfire-1.4.33/LICENSE
+-rw-r--r--   0        0        0     2688 2023-04-28 04:45:12.821836 simfire-1.4.33/README.md
+-rw-r--r--   0        0        0     1852 2023-04-28 04:45:13.021838 simfire-1.4.33/pyproject.toml
+-rw-r--r--   0        0        0     1111 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/__init__.py
+-rw-r--r--   0        0        0    10646 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/enums.py
+-rw-r--r--   0        0        0       37 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/_tests/__init__.py
+-rw-r--r--   0        0        0    15523 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/_tests/test_game.py
+-rw-r--r--   0        0        0     9928 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/_tests/test_sprites.py
+-rw-r--r--   0        0        0    14937 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/game.py
+-rw-r--r--   0        0        0     1318 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/image.py
+-rw-r--r--   0        0        0      379 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/_tests/__init__.py
+-rw-r--r--   0        0        0    18385 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/_tests/test_fire.py
+-rw-r--r--   0        0        0     8301 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/_tests/test_mitigation.py
+-rw-r--r--   0        0        0    29762 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/fire.py
+-rw-r--r--   0        0        0     7321 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/mitigation.py
+-rw-r--r--   0        0        0    15972 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/sprites.py
+-rw-r--r--   0        0        0       49 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/sim/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/sim/_tests/__init__.py
+-rw-r--r--   0        0        0    14392 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/sim/_tests/test_simulation.py
+-rw-r--r--   0        0        0    37791 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/sim/simulation.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/__init__.py
+-rw-r--r--   0        0        0     2378 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_config.py
+-rw-r--r--   0        0        0     1925 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config.yml
+-rw-r--r--   0        0        0       47 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_bad.yml
+-rw-r--r--   0        0        0     1874 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
+-rw-r--r--   0        0        0     1876 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_gaussian.yml
+-rw-r--r--   0        0        0     1851 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
+-rw-r--r--   0        0        0     4693 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_graph.py
+-rw-r--r--   0        0        0    17172 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_layers.py
+-rw-r--r--   0        0        0      622 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_log.py
+-rw-r--r--   0        0        0     2537 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_terrain.py
+-rw-r--r--   0        0        0     1472 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_units.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/assets/__init__.py
+-rw-r--r--   0        0        0     1854 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/assets/fireline_logo.png
+-rw-r--r--   0        0        0    38450 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/config.py
+-rw-r--r--   0        0        0      499 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/decorators.py
+-rw-r--r--   0        0        0     4153 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/generate_cfd_wind_layer.py
+-rw-r--r--   0        0        0    10189 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/graph.py
+-rw-r--r--   0        0        0    51105 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/layers.py
+-rw-r--r--   0        0        0     2030 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/log.py
+-rw-r--r--   0        0        0   143776 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
+-rw-r--r--   0        0        0   143776 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
+-rw-r--r--   0        0        0     2248 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/terrain.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/textures/__init__.py
+-rw-r--r--   0        0        0   204702 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/textures/terrain.jpg
+-rw-r--r--   0        0        0     2555 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/units.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/test_cfd_wind.py
+-rw-r--r--   0        0        0     2423 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/test_elevation_functions.py
+-rw-r--r--   0        0        0     2821 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/test_rothermel.py
+-rw-r--r--   0        0        0     1466 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/test_wind.py
+-rw-r--r--   0        0        0     3703 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/elevation_functions.py
+-rw-r--r--   0        0        0     1054 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/fuel_array_functions.py
+-rw-r--r--   0        0        0     2306 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/parameters.py
+-rw-r--r--   0        0        0     2083 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/presets.py
+-rw-r--r--   0        0        0     4306 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/rothermel.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/wind_mechanics/__init__.py
+-rw-r--r--   0        0        0     8781 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/wind_mechanics/cfd_wind.py
+-rw-r--r--   0        0        0     3132 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/wind_mechanics/perlin_wind.py
+-rw-r--r--   0        0        0     6578 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/wind_mechanics/wind_controller.py
+-rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 simfire-1.4.33/PKG-INFO
```

### Comparing `simfire-1.4.32/LICENSE` & `simfire-1.4.33/LICENSE`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/README.md` & `simfire-1.4.33/README.md`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/pyproject.toml` & `simfire-1.4.33/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simfire"
-version = "1.4.32"
+version = "1.4.33"
 description = "Fire simulator built in Python"
 authors = ["Tim Welsh <twelsh@mitre.org>", "Marissa Dotter <mdotter@mitre.org>",
            "Michael Doyle <mdoyle@mitre.org>", "Dhanuj Gandikota <dgandikota@mitre.org>",
            "Chris Kempis <ckempis@mitre.org>", "Lauren Schambach <lschambach@mitre.org>",
            "Alex Tapley <atapley@mitre.org>", "Michael Threet <mthreet@mitre.org>"]
 readme = "README.md"
 include = ["simfire/utils/textures/terrain.jpg", "simfire/utils/assets/fireline_logo.png"]
@@ -25,14 +25,15 @@
 scikit-image = "^0.19.3"
 svglib = "^1.3.0"
 rich = "^12.5.1"
 geopandas = "^0.11.1"
 wurlitzer = "^3.0.2"
 h5py = "^3.7.0"
 jsonlines = "^3.1.0"
+opencv-python = "^4.7.0.72"
 
 [tool.poetry.group.coverage.dependencies]
 pytest-cov = "^3.0.0"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.0.2"
 sphinx-autoapi = "^1.8.4"
```

### Comparing `simfire-1.4.32/simfire/__init__.py` & `simfire-1.4.33/simfire/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/enums.py` & `simfire-1.4.33/simfire/enums.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/_tests/__init__.py` & `simfire-1.4.33/simfire/game/_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/_tests/test_game.py` & `simfire-1.4.33/simfire/game/_tests/test_game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/_tests/test_sprites.py` & `simfire-1.4.33/simfire/game/_tests/test_sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/game.py` & `simfire-1.4.33/simfire/game/game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/image.py` & `simfire-1.4.33/simfire/game/image.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/managers/_tests/test_fire.py` & `simfire-1.4.33/simfire/game/managers/_tests/test_fire.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/managers/_tests/test_mitigation.py` & `simfire-1.4.33/simfire/game/managers/_tests/test_mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/managers/fire.py` & `simfire-1.4.33/simfire/game/managers/fire.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/managers/mitigation.py` & `simfire-1.4.33/simfire/game/managers/mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/game/sprites.py` & `simfire-1.4.33/simfire/game/sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/sim/_tests/test_simulation.py` & `simfire-1.4.33/simfire/sim/_tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/sim/simulation.py` & `simfire-1.4.33/simfire/sim/simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_config.py` & `simfire-1.4.33/simfire/utils/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_configs/test_config.yml` & `simfire-1.4.33/simfire/utils/_tests/test_configs/test_config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 operational:
   seed:
   latitude: 39.67
   longitude: 119.8
   height: 400
   width: 400
+  path: "/nfs/lslab2/fireline/data/"
   resolution: 30
+  year: 2020
 
 historical:
   use: false
   fire_init_pos_lat: 36.095
   fire_init_pos_long: -120.522
   name: Mineral
   year: '2020'
```

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_configs/test_config_flat_simple.yml` & `simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_flat_simple.yml`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 operational:
   seed:
   latitude: 39.67
   longitude: 119.8
   height: 4000
   width: 4000
+  path: "/nfs/lslab2/fireline/data/"
   resolution: 30
+  year: 2020
 
 historical:
   use: false
   fire_init_pos_lat: 36.095
   fire_init_pos_long: -120.522
   name: Mineral
   year: '2020'
```

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_configs/test_config_gaussian.yml` & `simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_gaussian.yml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 operational:
   seed:
   latitude: 39.67
   longitude: 119.8
   height: 4000
   width: 4000
+  path: "/nfs/lslab2/fireline/data/"
   resolution: 30
+  year: 2020
 
 historical:
   use: false
   fire_init_pos_lat: 36.095
   fire_init_pos_long: -120.522
   name: Mineral
   year: '2020'
```

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml` & `simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 operational:
   seed:
   latitude: 39.67
   longitude: 119.8
   height: 4000
   width: 4000
+  path: "/nfs/lslab2/fireline/data/"
   resolution: 30
+  year: 2020
 
 historical:
   use: false
   fire_init_pos_lat: 36.095
   fire_init_pos_long: -120.522
   name: Mineral
   year: '2020'
```

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_graph.py` & `simfire-1.4.33/simfire/utils/_tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_layers.py` & `simfire-1.4.33/simfire/utils/_tests/test_layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import shutil
 import unittest
+from pathlib import Path
 
 import matplotlib as mpl
 import numpy as np
 
 from ...world.fuel_array_functions import chaparral_fn
 from ..layers import (
     DataLayer,
@@ -120,15 +121,16 @@
         Test that the call to _save_contour_map() runs propoerly.
         """
         resolution = 30
         # Single Tile
         center = (33.5, 116.8)
         height, width = 1600, 1600
         lat_long_box = LatLongBox(center, height, width, resolution)
-        topo_layer = OperationalTopographyLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        topo_layer = OperationalTopographyLayer(lat_long_box, path)
         rmtree = False
         if not os.path.isdir("images/"):
             os.makedirs("images/")
             rmtree = True
         # Make sure that the function runs successfully
         try:
             lat_long_box._save_contour_map(topo_layer.data, "topo")
@@ -193,42 +195,46 @@
         NOTE: This method should always return a square
         """
         resolution = 30
         # 2 Tiles (easternly)
         center = (33.4, 115.04)
         height, width = 3200, 3200
         lat_long_box = LatLongBox(center, height, width, resolution)
-        topographyGen = OperationalTopographyLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        topographyGen = OperationalTopographyLayer(lat_long_box, path)
         self.assertEqual(topographyGen.data.shape[0], topographyGen.data.shape[1])
 
     def test__get_dems(self) -> None:
         """
         Test that the call to _get_dems() runs properly.
         This method will generate a list of the DEMs in the fireline /nfs/
         """
         resolution = 30
         # Single Tile
         center = (35.2, 119.6)
         height, width = 1600, 1600
         lat_long_box = LatLongBox(center, height, width, resolution)
-        topographyGen = OperationalTopographyLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        topographyGen = OperationalTopographyLayer(lat_long_box, path)
         self.assertEqual(1, len(topographyGen.tif_filenames))
 
         # 2 Tiles
         center = (37.4, 115.0)
         height, width = 1600, 1600
         lat_long_box = LatLongBox(center, height, width, resolution)
-        topographyGen = OperationalTopographyLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        topographyGen = OperationalTopographyLayer(lat_long_box, path)
         self.assertEqual(2, len(topographyGen.tif_filenames))
 
         # 4 Tiles
         center = (34.001, 116.008)
         height, width = 3200, 3200
         lat_long_box = LatLongBox(center, height, width, resolution)
-        topographyGen = OperationalTopographyLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        topographyGen = OperationalTopographyLayer(lat_long_box, path)
         self.assertEqual(4, len(topographyGen.tif_filenames))
 
 
 class TestFunctionalTopograpyLayer(unittest.TestCase):
     def setUp(self) -> None:
         # Create arbitrary function to test
         self.fn = lambda x, y: x + y
@@ -272,55 +278,60 @@
         NOTE: This method should always return a square
         """
         resolution = 30
         # 2 Tiles (easternly)
         center = (33.4, 116.04)
         height, width = 3200, 3200
         lat_long_box = LatLongBox(center, height, width, resolution)
-        FuelGen = OperationalFuelLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        FuelGen = OperationalFuelLayer(lat_long_box, path)
         self.assertEqual(FuelGen.data.shape[0], FuelGen.data.shape[1])
 
     def test_get_fuel_dems(self) -> None:
         """
         Test that the call to _get_dems() runs properly.
         This method will generate a list of the DEMs in the fireline /nfs/
         """
         resolution = 30
         # Single Tile
         center = (35.2, 117.6)
         height, width = 1600, 1600
         lat_long_box = LatLongBox(center, height, width, resolution)
-        FuelGen = OperationalFuelLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        FuelGen = OperationalFuelLayer(lat_long_box, path)
         self.assertEqual(1, len(FuelGen.fuel_model_filenames))
 
         # 2 Tiles
         center = (37.4, 118.0)
         height, width = 1600, 1600
         lat_long_box = LatLongBox(center, height, width, resolution)
-        FuelGen = OperationalFuelLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        FuelGen = OperationalFuelLayer(lat_long_box, path)
         self.assertEqual(2, len(FuelGen.fuel_model_filenames))
 
         # 4 Tiles
-        center = (33.001, 116.008)
+        center = (33.001, 113.008)
         height, width = 3200, 3200
         lat_long_box = LatLongBox(center, height, width, resolution)
-        FuelGen = OperationalFuelLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        FuelGen = OperationalFuelLayer(lat_long_box, path)
         self.assertEqual(4, len(FuelGen.fuel_model_filenames))
 
     def test_image(self) -> None:
         """
         Test that the internal call to _make_image() runs properly and
         returns a numpy array.
         """
         resolution = 30
         # Single Tile
         center = (35.2, 117.6)
         height, width = 1600, 1600
         lat_long_box = LatLongBox(center, height, width, resolution)
-        FuelGen = OperationalFuelLayer(lat_long_box)
+        path = Path("/nfs/lslab2/fireline/data")
+        FuelGen = OperationalFuelLayer(lat_long_box, path)
 
         self.assertIsInstance(
             FuelGen.image,
             np.ndarray,
             msg="The created image should be a numpy.ndarray, "
             f"but is of type {type(FuelGen.image)}",
         )
```

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_log.py` & `simfire-1.4.33/simfire/utils/_tests/test_log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_terrain.py` & `simfire-1.4.33/simfire/utils/_tests/test_terrain.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/_tests/test_units.py` & `simfire-1.4.33/simfire/utils/_tests/test_units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/assets/fireline_logo.png` & `simfire-1.4.33/simfire/utils/assets/fireline_logo.png`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/config.py` & `simfire-1.4.33/simfire/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,22 +129,26 @@
 @dataclasses.dataclass
 class OperationalConfig:
     seed: Optional[int]
     latitude: float
     longitude: float
     height: float
     width: float
+    path: Union[Path, str]
     resolution: float  # TODO: Make enum for resolution?
+    year: int  # TODO: Make enum for year?
 
     def __post_init__(self) -> None:
         self.latitude = float(self.latitude)
         self.longitude = float(self.longitude)
         self.height = float(self.height)
         self.width = float(self.width)
+        self.path = Path(self.path)
         self.resolution = float(self.resolution)
+        self.year = int(self.year)
 
 
 @dataclasses.dataclass
 class HistoricalConfig:
     """
     Class that tracks historical layer.
     """
@@ -334,17 +338,27 @@
         return True
 
     def _set_all_combos(self) -> None:
         """
         Get all possible combinations of latitude and longitude for the
         data layers.
         """
-        data_path = Path("/nfs/lslab2/fireline/data/fuel/")
+        path = self.yaml_data["operational"]["path"]
+        data_path = Path(f"{path}/fuel/")
         res = str(self.yaml_data["operational"]["resolution"]) + "m"
-        data_path = data_path / res / "old_2020"
+        year = str(self.yaml_data["operational"]["year"])
+        if res not in ["30m"]:
+            message = "Resolution must be 30m"
+            log.error(message)
+            raise ConfigError(message)
+        if year not in ["2019", "2020", "2022"]:
+            message = "Year must be 2019, 2020, or 2022"
+            log.error(message)
+            raise ConfigError(message)
+        data_path = data_path / res / year
         all_files = [
             f.stem
             for f in data_path.iterdir()
             if f.is_dir() and "n" in f.stem and "w" in f.stem
         ]
         self._all_combos = [
             (
@@ -487,15 +501,16 @@
                 The keyword arguments for the function if a functinoal layer is used.
                     Otherwise None
         """
         topo_layer: TopographyLayer
         topo_type = self.yaml_data["terrain"]["topography"]["type"]
         if topo_type == "operational":
             if self.lat_long_box is not None:
-                topo_layer = OperationalTopographyLayer(self.lat_long_box)
+                path = Path(self.yaml_data["operational"]["path"])
+                topo_layer = OperationalTopographyLayer(self.lat_long_box, path)
             else:
                 raise ConfigError(
                     "The topography layer type is `operational`, "
                     "but self.lat_long_box is None"
                 )
             fn_name = None
             kwargs = None
@@ -552,15 +567,16 @@
                 The keyword arguments for the function if a functinoal layer is used.
                     Otherwise None
         """
         burn_prob_layer: BurnProbabilityLayer
         bp_type = self.yaml_data["terrain"]["burn_probability"]["type"]
         if bp_type == "operational":
             if self.lat_long_box is not None:
-                burn_prob_layer = OperationalBurnProbabilityLayer(self.lat_long_box)
+                path = Path(self.yaml_data["operational"]["path"])
+                burn_prob_layer = OperationalBurnProbabilityLayer(self.lat_long_box, path)
             else:
                 raise ConfigError(
                     "The burn probability layer type is `operational`, "
                     "but self.lat_long_box is None"
                 )
             fn_name = None
             kwargs = None
@@ -612,15 +628,16 @@
             A FunctionalFuelLayer that utilizes the fuction specified by
             fn_name and the keyword arguments in kwargs
         """
         fuel_layer: FuelLayer
         fuel_type = self.yaml_data["terrain"]["fuel"]["type"]
         if fuel_type == "operational":
             if self.lat_long_box is not None:
-                fuel_layer = OperationalFuelLayer(self.lat_long_box)
+                path = Path(self.yaml_data["operational"]["path"])
+                fuel_layer = OperationalFuelLayer(self.lat_long_box, path)
             else:
                 raise ConfigError(
                     "The topography layer type is `operational`, "
                     "but self.lat_long_box is None"
                 )
             fn_name = None
             kwargs = None
```

### Comparing `simfire-1.4.32/simfire/utils/generate_cfd_wind_layer.py` & `simfire-1.4.33/simfire/utils/generate_cfd_wind_layer.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/graph.py` & `simfire-1.4.33/simfire/utils/graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/layers.py` & `simfire-1.4.33/simfire/utils/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import math
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
+import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.contour import QuadContourSet
 from PIL import Image
 from scipy import ndimage
 
 from ..enums import (
@@ -543,28 +544,28 @@
         """
         contours = plt.contour(self.data.squeeze(), origin="upper")
         plt.close()
         return contours
 
 
 class OperationalBurnProbabilityLayer(BurnProbabilityLayer):
-    def __init__(self, lat_long_box: LatLongBox) -> None:
+    def __init__(self, lat_long_box: LatLongBox, path: Path) -> None:
         """
         Initialize the elevation layer by retrieving the correct topograpchic data
         and computing the area
 
         Arguments:
             center: The lat/long coordinates of the center point of the screen.
             height: The height of the screen size (meters).
             width: The width of the screen size (meters).
             resolution: The resolution to get data (meters).
         """
         super().__init__()
         self.lat_long_box = lat_long_box
-        self.path = Path("/nfs/lslab2/fireline/data/risk/")
+        self.path = Path(path) / "risk"
         res = str(self.lat_long_box.resolution) + "m"
         self.datapath = self.path / res
 
         # TODO: Add check here if resolution isnt available
 
         self.data = self._make_data()
         self.contours = self._make_contours()
@@ -705,38 +706,39 @@
         """
         contours = plt.contour(self.data.squeeze(), origin="upper")
         plt.close()
         return contours
 
 
 class OperationalTopographyLayer(TopographyLayer):
-    def __init__(self, lat_long_box: LatLongBox) -> None:
+    def __init__(self, lat_long_box: LatLongBox, path: Path) -> None:
         """
         Initialize the elevation layer by retrieving the correct topograpchic data
         and computing the area
 
         Arguments:
             center: The lat/long coordinates of the center point of the screen.
             height: The height of the screen size (meters).
             width: The width of the screen size (meters).
             resolution: The resolution to get data (meters).
         """
         super().__init__()
         self.lat_long_box = lat_long_box
-        self.path = Path("/nfs/lslab2/fireline/data/topographic/")
+        self.path = Path(path) / "topographic"
         res = str(self.lat_long_box.resolution) + "m"
         self.datapath = self.path / res
 
         self.data = self._make_data()
         self.contours = self._make_contours()
 
     def _make_data(self) -> np.ndarray:
         self._get_dems()
         data = Image.open(self.tif_filenames[0])
         data = np.array(data, dtype=np.float32)
+        data = cv2.resize(data, (3612, 3612), interpolation=cv2.INTER_NEAREST)
         # flip axis because latitude goes up but numpy will read it down
         data = np.flip(data, 0)
         data = np.expand_dims(data, axis=-1)
 
         for key, _ in self.lat_long_box.tiles.items():
 
             if key == "single":
@@ -744,14 +746,17 @@
                 tr = (self.lat_long_box.bl[0][0], self.lat_long_box.tr[1][0])
                 bl = (self.lat_long_box.tr[0][0], self.lat_long_box.bl[1][0])
                 return data[tr[0] : bl[0], tr[1] : bl[1]]
             tmp_array = data
             for idx, dem in enumerate(self.tif_filenames[1:]):
                 tif_data = Image.open(dem)
                 tif_data = np.array(tif_data, dtype=np.float32)
+                tif_data = cv2.resize(
+                    tif_data, (3612, 3612), interpolation=cv2.INTER_NEAREST
+                )
                 # flip axis because latitude goes up but numpy will read it down
                 tif_data = np.flip(tif_data, 0)
                 tif_data = np.expand_dims(tif_data, axis=-1)
 
                 if key == "north":
                     # stack tiles along axis = 0 -> leftmost: bottom, rightmost: top
                     data = np.concatenate((data, tif_data), axis=0)
@@ -865,15 +870,15 @@
 
         """
         return np.array([])
         pass
 
 
 class OperationalFuelLayer(FuelLayer):
-    def __init__(self, lat_long_box: LatLongBox, type: str = "13") -> None:
+    def __init__(self, lat_long_box: LatLongBox, path: Path, type: str = "13") -> None:
         """
         Initialize the elevation layer by retrieving the correct topograpchic data
         and computing the area.
 
         Arguments:
             center: The lat/long coordinates of the center point of the screen
             height: The height of the screen size (meters)
@@ -882,53 +887,57 @@
             type: The type of data you wnt to load: 'display' or 'simulation'
                   display: rgb data for simulator
                   simulation: fuel model values for RL Harness/Simulation
         """
         self.lat_long_box = lat_long_box
         self.type = type
         # Temporary until we get real fuel data
-        self.path = Path("/nfs/lslab2/fireline/data/fuel/")
+        self.path = Path(path) / "fuel"
         res = str(self.lat_long_box.resolution) + "m"
 
-        self.datapath = self.path / res / "old_2020"
+        self.datapath = self.path / res / "2020"
 
         self._get_fuel_dems()
         fm_int_data = self._make_data(self.fuel_model_filenames)
         self.data = self._make_fuel_data(fm_int_data)
         self.image = self._make_data(self.rgb_filenames)
         self.image = self.image * 255.0
         self.image = self.image.astype(np.uint8)
 
     def _make_image(self) -> np.ndarray:
         """
         Use the fuel data in self.data to make an RGB background image.
         """
         return np.array([])
-        pass
 
     def _make_data(self, filename: List) -> np.ndarray:
 
         data = np.load(filename[0])
         # Flip the data over a horizontal axis
         data = np.flip(data, axis=0)
         data = np.array(data, dtype=np.float32)
+        data = cv2.resize(data, (3612, 3612), interpolation=cv2.INTER_NEAREST)
         data = np.expand_dims(data, axis=-1)
 
         for key, _ in self.lat_long_box.tiles.items():
 
             if key == "single":
                 # simple case
                 tr = (self.lat_long_box.bl[0][0], self.lat_long_box.tr[1][0])
                 bl = (self.lat_long_box.tr[0][0], self.lat_long_box.bl[1][0])
                 return data[tr[0] : bl[0], tr[1] : bl[1]]
             tmp_array = data
             for idx, dem in enumerate(filename[1:]):
                 tif_data = np.load(dem)
                 tif_data = np.array(tif_data, dtype=np.float32)
+                tif_data = cv2.resize(
+                    tif_data, (3612, 3612), interpolation=cv2.INTER_NEAREST
+                )
                 tif_data = np.expand_dims(tif_data, axis=-1)
+
                 # Flip the tif data over a horizontal axis
                 tif_data = np.flip(tif_data, axis=0)
 
                 if key == "north":
                     # stack tiles along axis = 0 -> leftmost: bottom, rightmost: top
                     data = np.concatenate((data, tif_data), axis=0)
                 elif key == "east":
@@ -952,16 +961,16 @@
         """
         This method will use the outputed tiles and return the correct dem files
         for both the RGB fuel model data and the fuel model data.
         """
         self.rgb_filenames = []
         self.fuel_model_filenames = []
         fuel_model = f"LF2020_FBFM{self.type}_200_CONUS"
-        fuel_data_fm = f"LC20_F{self.type}_200_projected_no_whitespace.npy"
-        fuel_data_rgb = f"LC20_F{self.type}_200_projected_rgb.npy"
+        fuel_data_fm = f"LC20_F{self.type}_200_no_whitespace.npy"
+        fuel_data_rgb = f"LC20_F{self.type}_200_rgb.npy"
         for _, ranges in self.lat_long_box.tiles.items():
             for range in ranges:
                 (five_deg_n, five_deg_w) = range
 
                 int_data_region = Path(
                     f"n{five_deg_n}w{five_deg_w}/{fuel_model}/{fuel_data_fm}"
                 )
```

### Comparing `simfire-1.4.32/simfire/utils/log.py` & `simfire-1.4.33/simfire/utils/log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy` & `simfire-1.4.33/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy` & `simfire-1.4.33/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/terrain.py` & `simfire-1.4.33/simfire/utils/terrain.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/textures/terrain.jpg` & `simfire-1.4.33/simfire/utils/textures/terrain.jpg`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/utils/units.py` & `simfire-1.4.33/simfire/utils/units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/_tests/test_cfd_wind.py` & `simfire-1.4.33/simfire/world/_tests/test_cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/_tests/test_elevation_functions.py` & `simfire-1.4.33/simfire/world/_tests/test_elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/_tests/test_rothermel.py` & `simfire-1.4.33/simfire/world/_tests/test_rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/_tests/test_wind.py` & `simfire-1.4.33/simfire/world/_tests/test_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/elevation_functions.py` & `simfire-1.4.33/simfire/world/elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/fuel_array_functions.py` & `simfire-1.4.33/simfire/world/fuel_array_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/parameters.py` & `simfire-1.4.33/simfire/world/parameters.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/presets.py` & `simfire-1.4.33/simfire/world/presets.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/rothermel.py` & `simfire-1.4.33/simfire/world/rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/wind_mechanics/cfd_wind.py` & `simfire-1.4.33/simfire/world/wind_mechanics/cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/wind_mechanics/perlin_wind.py` & `simfire-1.4.33/simfire/world/wind_mechanics/perlin_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/simfire/world/wind_mechanics/wind_controller.py` & `simfire-1.4.33/simfire/world/wind_mechanics/wind_controller.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.32/PKG-INFO` & `simfire-1.4.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfire
-Version: 1.4.32
+Version: 1.4.33
 Summary: Fire simulator built in Python
 Home-page: https://gitlab.mitre.org/fireline/simfire
 Keywords: python,reinforcement learning,simulation,fire
 Author: Tim Welsh
 Author-email: twelsh@mitre.org
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: geopandas (>=0.11.1,<0.12.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: noise (>=1.2.2,<2.0.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
+Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pygame (>=2.1.2,<3.0.0)
 Requires-Dist: reportlab (>=3.6.10,<4.0.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: svglib (>=1.3.0,<2.0.0)
 Requires-Dist: wurlitzer (>=3.0.2,<4.0.0)
 Project-URL: Documentation, https://fireline.pages.mitre.org/simfire/
```

