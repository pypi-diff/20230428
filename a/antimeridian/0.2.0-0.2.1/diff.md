# Comparing `tmp/antimeridian-0.2.0.tar.gz` & `tmp/antimeridian-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.2.0.tar", last modified: Wed Apr 26 19:57:55 2023, max compression
+gzip compressed data, was "antimeridian-0.2.1.tar", last modified: Fri Apr 28 13:54:19 2023, max compression
```

## Comparing `antimeridian-0.2.0.tar` & `antimeridian-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.125674 antimeridian-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-26 19:57:41.000000 antimeridian-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-26 19:57:55.125674 antimeridian-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-26 19:57:41.000000 antimeridian-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-26 19:57:41.000000 antimeridian-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:57:55.125674 antimeridian-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.121674 antimeridian-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.125674 antimeridian-0.2.0/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-26 19:57:41.000000 antimeridian-0.2.0/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-26 19:57:41.000000 antimeridian-0.2.0/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-04-26 19:57:41.000000 antimeridian-0.2.0/src/antimeridian/_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.125674 antimeridian-0.2.0/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.125674 antimeridian-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:19.793020 antimeridian-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-28 13:54:11.000000 antimeridian-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-28 13:54:19.793020 antimeridian-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-28 13:54:11.000000 antimeridian-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-28 13:54:11.000000 antimeridian-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:54:19.793020 antimeridian-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:19.789020 antimeridian-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:19.793020 antimeridian-0.2.1/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-28 13:54:11.000000 antimeridian-0.2.1/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-28 13:54:11.000000 antimeridian-0.2.1/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-28 13:54:11.000000 antimeridian-0.2.1/src/antimeridian/_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:19.793020 antimeridian-0.2.1/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-28 13:54:19.000000 antimeridian-0.2.1/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 13:54:19.000000 antimeridian-0.2.1/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:54:19.000000 antimeridian-0.2.1/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 13:54:19.000000 antimeridian-0.2.1/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 13:54:19.000000 antimeridian-0.2.1/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 13:54:19.000000 antimeridian-0.2.1/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:19.793020 antimeridian-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 13:54:11.000000 antimeridian-0.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-28 13:54:11.000000 antimeridian-0.2.1/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 13:54:11.000000 antimeridian-0.2.1/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-28 13:54:11.000000 antimeridian-0.2.1/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-28 13:54:11.000000 antimeridian-0.2.1/tests/test_segment.py
```

### Comparing `antimeridian-0.2.0/LICENSE` & `antimeridian-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.0/pyproject.toml` & `antimeridian-0.2.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 64"]
 
 [project]
 name = "antimeridian"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
@@ -34,16 +34,22 @@
     "mypy~=1.2",
     "pre-commit~=3.2",
     "pytest~=7.3",
     "pytest-console-scripts~=1.3",
     "ruff==0.0.262",
 ]
 docs = [
+    "cartopy~=0.21",
+    "ipykernel~=6.22",
+    "jupytext~=1.14",
+    "nbsphinx~=0.9",
     "pydata-sphinx-theme~=0.13",
+    "scipy~=1.10",
     "sphinx~=6.1",
+    "sphinx-click~=4.4",
 ]
 
 [project.scripts]
 antimeridian = "antimeridian._cli:cli"
 
 [tool.mypy]
 strict = true
```

### Comparing `antimeridian-0.2.0/src/antimeridian/_cli.py` & `antimeridian-0.2.1/src/antimeridian/_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.0/src/antimeridian/_implementation.py` & `antimeridian-0.2.1/src/antimeridian/_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 module can change at any time without warning.
 """
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Protocol, Tuple, Union, cast
 
+import shapely
 import shapely.geometry
 from shapely.geometry import MultiLineString, MultiPolygon, Polygon
 
 Point = Tuple[float, float]
 
 
 class GeoInterface(Protocol):
@@ -140,24 +141,35 @@
         polygons += fix_polygon_to_list(polygon)
     return MultiPolygon(polygons)
 
 
 def fix_polygon(polygon: Polygon) -> Union[Polygon, MultiPolygon]:
     """Fixes a :py:class:`shapely.geometry.Polygon`.
 
+    If the input polygon is a single polygon that is wound clockwise and doesn't
+    cross the antimeridian, it will be corrected by adding a counter-clockwise
+    polygon from (-180, -90) to (180, 90) as its exterior.
+
     Args:
         polygon: The input polygon
 
     Returns:
         The fixed polygon, either as a single polygon or a multi-polygon (if it
         was split)
     """
     polygons = fix_polygon_to_list(polygon)
     if len(polygons) == 1:
-        return polygons[0]
+        polygon = polygons[0]
+        if shapely.is_ccw(polygon.exterior):
+            return polygon
+        else:
+            return Polygon(
+                [(-180, 90), (-180, -90), (180, -90), (180, 90)],
+                [polygon.exterior.coords],
+            )
     else:
         return MultiPolygon(polygons)
 
 
 def segment_polygon(polygon: Polygon) -> List[List[Point]]:
     segments = segment(list(polygon.exterior.coords))
     if not segments:
```

### Comparing `antimeridian-0.2.0/tests/test_cli.py` & `antimeridian-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.0/tests/test_geojson.py` & `antimeridian-0.2.1/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.0/tests/test_multi_polygon.py` & `antimeridian-0.2.1/tests/test_multi_polygon.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.0/tests/test_polygon.py` & `antimeridian-0.2.1/tests/test_polygon.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 @pytest.mark.parametrize(
     ("name"),
     [
         "both-poles",
         "complex-split",
         "crossing-latitude",
+        "cw-only",
         "extra-crossing",
         "latitude-band",
         "north-pole",
         "one-hole",
         "over-180",
         "overlap",
         "simple",
```

