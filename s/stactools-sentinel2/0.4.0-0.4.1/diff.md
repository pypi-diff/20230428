# Comparing `tmp/stactools-sentinel2-0.4.0.tar.gz` & `tmp/stactools-sentinel2-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-sentinel2-0.4.0.tar", last modified: Tue Jan 31 17:33:39 2023, max compression
+gzip compressed data, was "stactools-sentinel2-0.4.1.tar", last modified: Fri Apr 28 11:34:52 2023, max compression
```

## Comparing `stactools-sentinel2-0.4.0.tar` & `stactools-sentinel2-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:33:39.342742 stactools-sentinel2-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-01-31 17:33:39.342742 stactools-sentinel2-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-31 17:33:39.342742 stactools-sentinel2-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:33:39.338742 stactools-sentinel2-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:33:39.338742 stactools-sentinel2-0.4.0/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:33:39.342742 stactools-sentinel2-0.4.0/src/stactools/sentinel2/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/granule_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/mgrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/product_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/safe_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/tileinfo_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-01-31 17:33:27.000000 stactools-sentinel2-0.4.0/src/stactools/sentinel2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:33:39.342742 stactools-sentinel2-0.4.0/src/stactools_sentinel2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-01-31 17:33:39.000000 stactools-sentinel2-0.4.0/src/stactools_sentinel2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-01-31 17:33:39.000000 stactools-sentinel2-0.4.0/src/stactools_sentinel2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 17:33:39.000000 stactools-sentinel2-0.4.0/src/stactools_sentinel2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-31 17:33:39.000000 stactools-sentinel2-0.4.0/src/stactools_sentinel2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-31 17:33:39.000000 stactools-sentinel2-0.4.0/src/stactools_sentinel2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.754932 stactools-sentinel2-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.754932 stactools-sentinel2-0.4.1/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/src/stactools/sentinel2/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/granule_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/mgrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/product_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/safe_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22081 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/tileinfo_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/top_level.txt
```

### Comparing `stactools-sentinel2-0.4.0/LICENSE` & `stactools-sentinel2-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.0/PKG-INFO` & `stactools-sentinel2-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel2
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create STAC Items from Sentinel-2 metadata
 Home-page: https://github.com/stactools-sentinel2/stactools-sentinel2
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Issues, https://github.com/stactools-sentinel2s/stactools-sentinel2/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # stactools-sentinel2
 
 stactools package for Sentinel-2 data.
@@ -71,7 +72,13 @@
 ```
 
 Run the tests with:
 
 ```commandline
 pytest -vvv
 ```
+
+If you change the STAC metadata output, you will need to re-create the test files with the following command:
+
+```shell
+python scripts/create_expected.py
+```
```

### Comparing `stactools-sentinel2-0.4.0/README.md` & `stactools-sentinel2-0.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -52,8 +52,14 @@
 pip install -e .
 ```
 
 Run the tests with:
 
 ```commandline
 pytest -vvv
-```
+```
+
+If you change the STAC metadata output, you will need to re-create the test files with the following command:
+
+```shell
+python scripts/create_expected.py
+```
```

### Comparing `stactools-sentinel2-0.4.0/setup.cfg` & `stactools-sentinel2-0.4.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 	STAC
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 python_requires = >=3.8
 package_dir = 
 	= src
 packages = find_namespace:
 install_requires = 
 	stactools >= 0.4.2
+	pystac >= 1.7.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/cog.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/cog.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/commands.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/constants.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/granule_metadata.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/granule_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 import re
+from dataclasses import dataclass
 from typing import Dict, Final, List, Optional, Pattern, Tuple
 
 import pystac
+from pystac.utils import map_opt
 from stactools.core.io import ReadHrefModifier
 from stactools.core.io.xml import XmlElement
-from stactools.core.utils import map_opt
 
 from stactools.sentinel2.constants import GRANULE_METADATA_ASSET_KEY
 from stactools.sentinel2.constants import SENTINEL2_PROPERTY_PREFIX as s2_prefix
 
 BASELINE_PROCESSING: Final[Pattern[str]] = re.compile(r"_N(\d\d\.\d\d)")
 
 
@@ -35,16 +38,18 @@
         self._geocoding_node = geocoding_node
 
         tile_angles_node = self._root.find("n1:Geometric_Info/Tile_Angles")
         if tile_angles_node is None:
             raise GranuleMetadataError(f"Cannot find tile angles node in {self.href}")
         self._tile_angles_node = tile_angles_node
 
-        self._viewing_angle_nodes = self._tile_angles_node.findall(
-            "Mean_Viewing_Incidence_Angle_List/Mean_Viewing_Incidence_Angle"
+        self.viewing_angles = ViewingAngle.from_nodes(
+            self._tile_angles_node.findall(
+                "Mean_Viewing_Incidence_Angle_List/Mean_Viewing_Incidence_Angle"
+            )
         )
 
         self._image_content_node = self._root.find(
             "n1:Quality_Indicators_Info/Image_Content_QI"
         )
 
         self.resolution_to_shape: Dict[int, Tuple[int, int]] = {}
@@ -218,12 +223,50 @@
         https://sentinel.esa.int/web/sentinel/user-guides/sentinel-2-msi/naming-convention
         """
         mgrs_match = BASELINE_PROCESSING.search(self.product_id)
         if mgrs_match:
             return mgrs_match.group(1)
         return None
 
+    @property
+    def pvi_filename(self) -> Optional[str]:
+        return self._root.find_text("n1:Quality_Indicators_Info/PVI_FILENAME")
+
     def create_asset(self):
         asset = pystac.Asset(
             href=self.href, media_type=pystac.MediaType.XML, roles=["metadata"]
         )
         return GRANULE_METADATA_ASSET_KEY, asset
+
+
+@dataclass
+class ViewingAngle:
+    azimuth: float
+    zenith: float
+
+    @classmethod
+    def from_nodes(cls, nodes: List[XmlElement]) -> Dict[str, ViewingAngle]:
+        angles = dict()
+        for node in nodes:
+            band_id_str = node.get_attr("bandId")
+            if band_id_str is None:
+                raise ValueError("expected band id on viewing angle node")
+            else:
+                band_id = int(band_id_str)
+            if band_id < 8:
+                band = f"B0{band_id + 1}"
+            elif band_id == 8:
+                band = "B8A"
+            else:
+                band = f"B{band_id:02}"
+            zenith = float(
+                node.find_text_or_throw(
+                    "ZENITH_ANGLE", lambda s: ValueError(f"missing ZENITH_ANGLE: {s}")
+                )
+            )
+            azimuth = float(
+                node.find_text_or_throw(
+                    "AZIMUTH_ANGLE", lambda s: ValueError(f"missing AZIMUTH_ANGLE: {s}")
+                )
+            )
+            angles[band] = cls(azimuth=azimuth, zenith=zenith)
+        return angles
```

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/mgrs.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/mgrs.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/product_metadata.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/product_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import pystac
-from pystac.utils import str_to_datetime
+from pystac.utils import map_opt, str_to_datetime
 from shapely.geometry import Polygon, mapping
 from stactools.core.io import ReadHrefModifier
 from stactools.core.io.xml import XmlElement
-from stactools.core.utils import map_opt
 
 from stactools.sentinel2.constants import COORD_ROUNDING, PRODUCT_METADATA_ASSET_KEY
 from stactools.sentinel2.constants import SENTINEL2_PROPERTY_PREFIX as s2_prefix
 from stactools.sentinel2.utils import fix_z_values
 
 
 class ProductMetadataError(Exception):
@@ -94,15 +93,14 @@
                         * 2
                     )
                 )
             ]
             footprint_polygon = Polygon(footprint_points)
             geometry = mapping(footprint_polygon)
             bbox = footprint_polygon.bounds
-            print(geometry)
             return bbox, geometry
 
         self.bbox, self.geometry = _get_geometries()
 
     @property
     def scene_id(self) -> str:
         """Returns the string to be used for a STAC Item id.
```

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/safe_manifest.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/safe_manifest.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,14 @@
             return None
         else:
             # Remove relative prefix that some paths have
             file_path = file_path.strip("./")
             return os.path.join(self.granule_href, file_path)
 
     @property
-    def thumbnail_href(self) -> Optional[str]:
-        return self._find_href(
-            [
-                'dataObject[@ID="S2_Level-1C_Preview_Tile1_Data"]/byteStream/fileLocation',
-                'dataObject[@ID="Preview_4_Tile1_Data"]/byteStream/fileLocation',
-            ]
-        )
-
-    @property
     def product_metadata_href(self) -> Optional[str]:
         return self._find_href(
             [
                 'dataObject[@ID="S2_Level-1C_Product_Metadata"]/byteStream/fileLocation',
                 'dataObject[@ID="S2_Level-2A_Product_Metadata"]/byteStream/fileLocation',
             ]
         )
```

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/stac.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/stac.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import re
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import chain
 from typing import Any, Dict, Final, List, Optional, Pattern, Tuple
 
 import pystac
+import shapely
 from pystac.extensions.eo import Band, EOExtension
+from pystac.extensions.grid import GridExtension
 from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.raster import DataType, RasterBand, RasterExtension
 from pystac.extensions.sat import OrbitState, SatExtension
 from pystac.extensions.view import ViewExtension
-from shapely.geometry import mapping
-from shapely.geometry import shape as make_shape
 from stactools.core.io import ReadHrefModifier
 from stactools.core.projection import reproject_geom, transform_from_bbox
 from stactools.core.utils import antimeridian
 from stactools.core.utils.antimeridian import Strategy
 
 from stactools.sentinel2.constants import (
     BANDS_TO_ASSET_NAME,
@@ -33,16 +33,15 @@
     SENTINEL_BANDS,
     SENTINEL_CONSTELLATION,
     SENTINEL_INSTRUMENTS,
     SENTINEL_LICENSE,
     SENTINEL_PROVIDER,
     UNSUFFIXED_BAND_RESOLUTION,
 )
-from stactools.sentinel2.granule_metadata import GranuleMetadata
-from stactools.sentinel2.grid import GridExtension
+from stactools.sentinel2.granule_metadata import GranuleMetadata, ViewingAngle
 from stactools.sentinel2.mgrs import MgrsExtension
 from stactools.sentinel2.product_metadata import ProductMetadata
 from stactools.sentinel2.safe_manifest import SafeManifest
 from stactools.sentinel2.tileinfo_metadata import TileInfoMetadata
 from stactools.sentinel2.utils import extract_gsd
 
 logger = logging.getLogger(__name__)
@@ -83,14 +82,15 @@
     metadata_dict: Dict[str, Any]
     image_media_type: str
     image_paths: List[str]
     epsg: int
     proj_bbox: List[float]
     resolution_to_shape: Dict[int, Tuple[int, int]]
     processing_baseline: str
+    viewing_angles: Dict[str, ViewingAngle]
     orbit_state: Optional[str] = None
     relative_orbit: Optional[int] = None
     sun_azimuth: Optional[float] = None
     sun_zenith: Optional[float] = None
     boa_add_offsets: Optional[Dict[str, int]] = None
 
 
@@ -163,21 +163,23 @@
     if metadata.orbit_state or metadata.relative_orbit:
         sat = SatExtension.ext(item, add_if_missing=True)
         sat.orbit_state = (
             OrbitState(metadata.orbit_state.lower()) if metadata.orbit_state else None
         )
         sat.relative_orbit = metadata.relative_orbit
 
-    # proj
+    # Projection Extension
     projection = ProjectionExtension.ext(item, add_if_missing=True)
     projection.epsg = metadata.epsg
     if projection.epsg is None:
         raise ValueError(
             f"Could not determine EPSG code for {granule_href}; which is required."
         )
+    centroid = shapely.geometry.shape(item.geometry).centroid
+    projection.centroid = {"lat": round(centroid.y, 5), "lon": round(centroid.x, 5)}
 
     # MGRS and Grid Extension
     mgrs_match = MGRS_PATTERN.search(metadata.scene_id)
     if mgrs_match and len(mgrs_groups := mgrs_match.groups()) == 3:
         mgrs = MgrsExtension.ext(item, add_if_missing=True)
         mgrs.utm_zone = int(mgrs_groups[0])
         mgrs.latitude_band = mgrs_groups[1]
@@ -204,14 +206,15 @@
         [
             image_asset_from_href(
                 asset_href=os.path.join(asset_href_prefix or granule_href, image_path),
                 resolution_to_shape=metadata.resolution_to_shape,
                 proj_bbox=metadata.proj_bbox,
                 media_type=metadata.image_media_type,
                 processing_baseline=metadata.processing_baseline,
+                viewing_angles=metadata.viewing_angles,
                 boa_add_offsets=metadata.boa_add_offsets,
             )
             for image_path in metadata.image_paths
         ]
     )
 
     for key, asset in chain(image_assets.items(), metadata.extra_assets.items()):
@@ -227,14 +230,15 @@
 
 def image_asset_from_href(
     asset_href: str,
     resolution_to_shape: Dict[int, Tuple[int, int]],
     proj_bbox: List[float],
     media_type: Optional[str],
     processing_baseline: str,
+    viewing_angles: Dict[str, ViewingAngle],
     boa_add_offsets: Optional[Dict[str, int]] = None,
 ) -> Tuple[str, pystac.Asset]:
     logger.debug(f"Creating asset for image {asset_href}")
 
     _, ext = os.path.splitext(asset_href)
     if media_type is not None:
         asset_media_type = media_type
@@ -324,14 +328,19 @@
 
         asset = pystac.Asset(
             href=asset_href,
             media_type=asset_media_type,
             title=f"{band.description} - {asset_res}m",
             roles=["data", "reflectance"],
         )
+        viewing_angle = viewing_angles[band_id]
+        # We can't use the ViewExtension here until
+        # https://github.com/stac-utils/pystac/issues/793 is fixed
+        asset.extra_fields["view:azimuth"] = viewing_angle.azimuth
+        asset.extra_fields["view:incidence_angle"] = viewing_angle.zenith
 
         asset_eo = EOExtension.ext(asset)
         asset_eo.bands = [band_from_band_id(band_id)]
         set_asset_properties(asset, band_gsd)
 
         RasterExtension.ext(asset).bands = raster_bands(
             boa_add_offsets, processing_baseline, band_id, resolution
@@ -468,18 +477,18 @@
                     media_type=pystac.MediaType.XML,
                     roles=["metadata"],
                 ),
             ),
         ]
     )
 
-    if safe_manifest.thumbnail_href is not None:
+    if granule_metadata.pvi_filename is not None:
         extra_assets["preview"] = pystac.Asset(
-            href=safe_manifest.thumbnail_href,
-            media_type=pystac.MediaType.COG,
+            href=os.path.join(granule_href, granule_metadata.pvi_filename),
+            media_type=product_metadata.image_media_type,
             roles=["thumbnail"],
         )
 
     return Metadata(
         scene_id=product_metadata.scene_id,
         extra_assets=extra_assets,
         geometry=product_metadata.geometry,
@@ -498,14 +507,15 @@
         epsg=granule_metadata.epsg,
         proj_bbox=[round(v, COORD_ROUNDING) for v in granule_metadata.proj_bbox],
         resolution_to_shape=granule_metadata.resolution_to_shape,
         sun_zenith=granule_metadata.mean_solar_zenith,
         sun_azimuth=granule_metadata.mean_solar_azimuth,
         processing_baseline=granule_metadata.processing_baseline,
         boa_add_offsets=product_metadata.boa_add_offsets,
+        viewing_angles=granule_metadata.viewing_angles,
     )
 
 
 # this is used for the Sinergise S3 format,
 # e.g., s3://sentinel-s2-l1c/tiles/10/S/DG/2018/12/31/0/
 def metadata_from_granule_metadata(
     granule_metadata_href: str,
@@ -526,15 +536,15 @@
         f = (
             granule_metadata_href.split("tiles/")[0]
             + tileinfo_metadata.product_path
             + "/metadata.xml"
         )
         product_metadata = ProductMetadata(f, read_href_modifier)
 
-    geometry = make_shape(
+    geometry = shapely.geometry.shape(
         reproject_geom(
             f"epsg:{granule_metadata.epsg}", "epsg:4326", tileinfo_metadata.geometry
         )
     ).simplify(tolerance)
 
     extra_assets = dict(
         [
@@ -559,24 +569,25 @@
         scene_id=granule_metadata.scene_id,
         extra_assets=extra_assets,
         metadata_dict=metadata_dict,
         cloudiness_percentage=granule_metadata.cloudiness_percentage,
         epsg=granule_metadata.epsg,
         proj_bbox=granule_metadata.proj_bbox,
         resolution_to_shape=granule_metadata.resolution_to_shape,
-        geometry=mapping(geometry),
+        geometry=shapely.geometry.mapping(geometry),
         bbox=geometry.bounds,
         datetime=tileinfo_metadata.datetime,
         platform=granule_metadata.platform,
         image_media_type=pystac.MediaType.JPEG2000,
         image_paths=image_paths,
         sun_zenith=granule_metadata.mean_solar_zenith,
         sun_azimuth=granule_metadata.mean_solar_azimuth,
         processing_baseline=granule_metadata.processing_baseline,
         boa_add_offsets=product_metadata.boa_add_offsets if product_metadata else None,
+        viewing_angles=granule_metadata.viewing_angles,
     )
 
 
 def offset_for_pb(processing_baseline: str) -> float:
     if processing_baseline < "04.00":
         return 0
     else:
```

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/tileinfo_metadata.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/tileinfo_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.0/src/stactools/sentinel2/utils.py` & `stactools-sentinel2-0.4.1/src/stactools/sentinel2/utils.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.0/src/stactools_sentinel2.egg-info/PKG-INFO` & `stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel2
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create STAC Items from Sentinel-2 metadata
 Home-page: https://github.com/stactools-sentinel2/stactools-sentinel2
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Issues, https://github.com/stactools-sentinel2s/stactools-sentinel2/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # stactools-sentinel2
 
 stactools package for Sentinel-2 data.
@@ -71,7 +72,13 @@
 ```
 
 Run the tests with:
 
 ```commandline
 pytest -vvv
 ```
+
+If you change the STAC metadata output, you will need to re-create the test files with the following command:
+
+```shell
+python scripts/create_expected.py
+```
```

### Comparing `stactools-sentinel2-0.4.0/src/stactools_sentinel2.egg-info/SOURCES.txt` & `stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.cfg
 setup.py
 src/stactools/sentinel2/__init__.py
 src/stactools/sentinel2/cog.py
 src/stactools/sentinel2/commands.py
 src/stactools/sentinel2/constants.py
 src/stactools/sentinel2/granule_metadata.py
-src/stactools/sentinel2/grid.py
 src/stactools/sentinel2/mgrs.py
 src/stactools/sentinel2/product_metadata.py
 src/stactools/sentinel2/safe_manifest.py
 src/stactools/sentinel2/stac.py
 src/stactools/sentinel2/tileinfo_metadata.py
 src/stactools/sentinel2/utils.py
 src/stactools_sentinel2.egg-info/PKG-INFO
```

