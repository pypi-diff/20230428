# Comparing `tmp/antimeridian-0.2.2.tar.gz` & `tmp/antimeridian-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.2.2.tar", last modified: Fri Apr 28 16:12:40 2023, max compression
+gzip compressed data, was "antimeridian-0.2.3.tar", last modified: Fri Apr 28 18:54:00 2023, max compression
```

## Comparing `antimeridian-0.2.2.tar` & `antimeridian-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:12:40.319676 antimeridian-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-28 16:12:31.000000 antimeridian-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-28 16:12:40.319676 antimeridian-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-28 16:12:31.000000 antimeridian-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-28 16:12:31.000000 antimeridian-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 16:12:40.319676 antimeridian-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:12:40.319676 antimeridian-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:12:40.319676 antimeridian-0.2.2/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-28 16:12:31.000000 antimeridian-0.2.2/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-28 16:12:31.000000 antimeridian-0.2.2/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-04-28 16:12:31.000000 antimeridian-0.2.2/src/antimeridian/_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:12:40.319676 antimeridian-0.2.2/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-28 16:12:40.000000 antimeridian-0.2.2/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 16:12:40.000000 antimeridian-0.2.2/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 16:12:40.000000 antimeridian-0.2.2/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 16:12:40.000000 antimeridian-0.2.2/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 16:12:40.000000 antimeridian-0.2.2/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 16:12:40.000000 antimeridian-0.2.2/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:12:40.319676 antimeridian-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 16:12:31.000000 antimeridian-0.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-28 16:12:31.000000 antimeridian-0.2.2/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 16:12:31.000000 antimeridian-0.2.2/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-28 16:12:31.000000 antimeridian-0.2.2/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-28 16:12:31.000000 antimeridian-0.2.2/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.440942 antimeridian-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-28 18:53:50.000000 antimeridian-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-28 18:54:00.440942 antimeridian-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-28 18:53:50.000000 antimeridian-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-28 18:53:50.000000 antimeridian-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:54:00.440942 antimeridian-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.436942 antimeridian-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.436942 antimeridian-0.2.3/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-28 18:53:50.000000 antimeridian-0.2.3/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-28 18:53:50.000000 antimeridian-0.2.3/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-04-28 18:53:50.000000 antimeridian-0.2.3/src/antimeridian/_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.436942 antimeridian-0.2.3/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.440942 antimeridian-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_segment.py
```

### Comparing `antimeridian-0.2.2/LICENSE` & `antimeridian-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.2/PKG-INFO` & `antimeridian-0.2.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,55 @@
-Metadata-Version: 2.1
-Name: antimeridian
-Version: 0.2.2
-Summary: Fix GeoJSON geometries that cross the antimeridian
-Author-email: Pete Gadomski <pete.gadomski@gmail.com>
-License: Apache-2.0
-Project-URL: documentation, https://antimeridian.readthedocs.io
-Project-URL: repository, https://github.com/gadomski/antimeridan
-Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
-Keywords: geojson,antimeridian,shapely
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: cli
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 # antimeridian
 
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/latest/)
 [![PyPI](https://img.shields.io/pypi/v/antimeridian?style=for-the-badge)](https://pypi.org/project/antimeridian/)
 
 [![GitHub](https://img.shields.io/github/license/gadomski/antimeridian?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/CODE_OF_CONDUCT)
 
-A Python package to correct GeoJSON shapes that cross the antimeridian.
+Fix polygons that cross the antimeridian.
 See [the documentation](https://antimeridian.readthedocs.io) for information about the underlying algorithm.
+Depends on [shapely](https://shapely.readthedocs.io).
+
+Can fix:
+
+- Shapely [`Polygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.Polygon.html#shapely.Polygon) and [`MultiPolygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.MultiPolygon.html#shapely.MultiPolygon) objects
+- GeoJSON [Polygons](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.6), [MultiPolygons](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.7), [Features](https://datatracker.ietf.org/doc/html/rfc7946#section-3.2) and [FeatureCollections](https://datatracker.ietf.org/doc/html/rfc7946#section-3.3), as dictionaries
+- Anything that has a [`__geo_interface__`](https://gist.github.com/sgillies/2217756)
 
 ## Usage
 
 ```shell
 pip install antimeridian
 ```
 
-Then, in your code:
+Then:
 
 ```python
 import antimeridian
 fixed = antimeridian.fix_geojson(geojson)
 ```
 
-If you'd like to use the command line interface:
+### Command line interface
+
+Use the `cli` optional dependency to install the `antimeridian` CLI:
 
 ```shell
 pip install 'antimeridian[cli]'
 antimeridian fix input.json > output.json
 ```
 
 ## Developing
 
 Clone and install in editable mode with the development optional dependencies:
 
 ```shell
 git clone https://github.com/gadomski/antimeridian
+cd antimeridian
 pip install -e '.[dev,docs]'
 ```
 
 We use [pytest](https://docs.pytest.org) for tests:
 
 ```shell
 pytest
```

### Comparing `antimeridian-0.2.2/pyproject.toml` & `antimeridian-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 64"]
 
 [project]
 name = "antimeridian"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
```

### Comparing `antimeridian-0.2.2/src/antimeridian/_cli.py` & `antimeridian-0.2.3/src/antimeridian/_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 @click.argument("infile", type=str)
 @click.option(
     "-i", "--index", help="Return the single LineString at this index", type=int
 )
 def segment(infile: str, index: Optional[int]) -> None:
     """Segments the exterior coordinates of a GeoJSON file
 
-    Prints the resulting MultiLineString to standard output.
+    Prints the resulting MultiLineString to standard output. Useful mostly for
+    debugging problems with `fix`.
     """
     with open(infile) as f:
         data = json.load(f)
     segments = antimeridian.segment_geojson(data)
     if index is not None:
         data = shapely.geometry.mapping(segments.geoms[index])
     else:
```

### Comparing `antimeridian-0.2.2/src/antimeridian/_implementation.py` & `antimeridian-0.2.3/src/antimeridian/_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def fix_geojson(
     geojson: Dict[str, Any],
     *,
     force_north_pole: bool = False,
     force_south_pole: bool = False,
 ) -> Dict[str, Any]:
-    """Fixes GeoJSON object that crosses the antimeridian.
+    """Fixes a GeoJSON object that crosses the antimeridian.
 
     If the object does not cross the antimeridian, it is returned unchanged.
 
     See :py:func:`fix_polygon` for a description of the ``force_north_pole`` and
     ``force_south_pole`` arguments.
 
     Args:
@@ -201,15 +201,17 @@
 
     Returns:
         The fixed multi-polygon
     """
     polygons = list()
     for polygon in multi_polygon.geoms:
         polygons += fix_polygon_to_list(
-            polygon, force_north_pole=False, force_south_pole=False
+            polygon,
+            force_north_pole=force_north_pole,
+            force_south_pole=force_south_pole,
         )
     return MultiPolygon(polygons)
 
 
 def fix_polygon(
     polygon: Polygon, *, force_north_pole: bool = False, force_south_pole: bool = False
 ) -> Union[Polygon, MultiPolygon]:
```

### Comparing `antimeridian-0.2.2/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.2.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.2
+Version: 0.2.3
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
@@ -22,43 +22,53 @@
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/latest/)
 [![PyPI](https://img.shields.io/pypi/v/antimeridian?style=for-the-badge)](https://pypi.org/project/antimeridian/)
 
 [![GitHub](https://img.shields.io/github/license/gadomski/antimeridian?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/CODE_OF_CONDUCT)
 
-A Python package to correct GeoJSON shapes that cross the antimeridian.
+Fix polygons that cross the antimeridian.
 See [the documentation](https://antimeridian.readthedocs.io) for information about the underlying algorithm.
+Depends on [shapely](https://shapely.readthedocs.io).
+
+Can fix:
+
+- Shapely [`Polygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.Polygon.html#shapely.Polygon) and [`MultiPolygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.MultiPolygon.html#shapely.MultiPolygon) objects
+- GeoJSON [Polygons](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.6), [MultiPolygons](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.7), [Features](https://datatracker.ietf.org/doc/html/rfc7946#section-3.2) and [FeatureCollections](https://datatracker.ietf.org/doc/html/rfc7946#section-3.3), as dictionaries
+- Anything that has a [`__geo_interface__`](https://gist.github.com/sgillies/2217756)
 
 ## Usage
 
 ```shell
 pip install antimeridian
 ```
 
-Then, in your code:
+Then:
 
 ```python
 import antimeridian
 fixed = antimeridian.fix_geojson(geojson)
 ```
 
-If you'd like to use the command line interface:
+### Command line interface
+
+Use the `cli` optional dependency to install the `antimeridian` CLI:
 
 ```shell
 pip install 'antimeridian[cli]'
 antimeridian fix input.json > output.json
 ```
 
 ## Developing
 
 Clone and install in editable mode with the development optional dependencies:
 
 ```shell
 git clone https://github.com/gadomski/antimeridian
+cd antimeridian
 pip install -e '.[dev,docs]'
 ```
 
 We use [pytest](https://docs.pytest.org) for tests:
 
 ```shell
 pytest
```

### Comparing `antimeridian-0.2.2/tests/test_cli.py` & `antimeridian-0.2.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.2/tests/test_geojson.py` & `antimeridian-0.2.3/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.2/tests/test_multi_polygon.py` & `antimeridian-0.2.3/tests/test_multi_polygon.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.2/tests/test_polygon.py` & `antimeridian-0.2.3/tests/test_polygon.py`

 * *Files identical despite different names*

