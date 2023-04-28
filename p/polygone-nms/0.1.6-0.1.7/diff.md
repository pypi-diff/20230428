# Comparing `tmp/polygone-nms-0.1.6.tar.gz` & `tmp/polygone-nms-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygone-nms-0.1.6.tar", last modified: Fri Apr 28 10:52:31 2023, max compression
+gzip compressed data, was "polygone-nms-0.1.7.tar", last modified: Fri Apr 28 12:10:28 2023, max compression
```

## Comparing `polygone-nms-0.1.6.tar` & `polygone-nms-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:52:31.089029 polygone-nms-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-28 10:52:31.089029 polygone-nms-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:52:31.085029 polygone-nms-0.1.6/polygone_nms/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/polygone_nms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/polygone_nms/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/polygone_nms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:52:31.089029 polygone-nms-0.1.6/polygone_nms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-28 10:52:31.000000 polygone-nms-0.1.6/polygone_nms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 10:52:31.000000 polygone-nms-0.1.6/polygone_nms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:52:31.000000 polygone-nms-0.1.6/polygone_nms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 10:52:31.000000 polygone-nms-0.1.6/polygone_nms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 10:52:31.000000 polygone-nms-0.1.6/polygone_nms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-28 10:52:31.089029 polygone-nms-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:52:31.089029 polygone-nms-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/tests/test_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/tests/test_polygone_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-28 10:52:09.000000 polygone-nms-0.1.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:10:28.987722 polygone-nms-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-28 12:10:28.987722 polygone-nms-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:10:28.987722 polygone-nms-0.1.7/polygone_nms/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/polygone_nms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/polygone_nms/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/polygone_nms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:10:28.987722 polygone-nms-0.1.7/polygone_nms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-28 12:10:28.000000 polygone-nms-0.1.7/polygone_nms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 12:10:28.000000 polygone-nms-0.1.7/polygone_nms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:10:28.000000 polygone-nms-0.1.7/polygone_nms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 12:10:28.000000 polygone-nms-0.1.7/polygone_nms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 12:10:28.000000 polygone-nms-0.1.7/polygone_nms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-28 12:10:28.987722 polygone-nms-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:10:28.987722 polygone-nms-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/tests/test_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/tests/test_polygone_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-28 12:10:06.000000 polygone-nms-0.1.7/tests/test_utils.py
```

### Comparing `polygone-nms-0.1.6/LICENSE` & `polygone-nms-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polygone-nms-0.1.6/PKG-INFO` & `polygone-nms-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygone-nms
-Version: 0.1.6
+Version: 0.1.7
 Summary: Efficient and distributed polygon Non-Maximum Suppression (NMS) library
 Home-page: https://github.com/WolodjaZ/polygone-nms
 Author: Vladimir Zaigrajew
 Author-email: vladimirzaigrajew@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -58,20 +58,24 @@
 # Example input data
 data = np.array([
     [0, 0, 1, 1, 0, 1, 0, 0, 1, 0.9],
     [0.5, 0.5, 1.5, 1.5, 0.5, 1.5, 0, 0, 1, 0.8],
 ])
 
 # Apply NMS
-results = polygone_nms(data, distributed=None, nms_method="Default", intersection_method="IOU")
+results = nms(data, distributed=None, nms_method="Default", intersection_method="IOU")
 
-print(results)
+print("Filtered indices:", results)
+
+# Filtered data
+print("Filtered data:")
+print(data[results])
 ```
 
-For a more detailed guide on using PolyGoneNMS, please see the [Quickstart](https://www.example.com/) in the documentation.
+For a more detailed guide on using PolyGoneNMS, please see the [Quickstart](https://wolodjaz.github.io/PolyGoneNMS/0.1.6/quickstart/) in the documentation.
 
 ## Documentation
 
 Detailed documentation is available at:
 [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=flat)](https://wolodjaz.github.io/PolyGoneNMS)
```

### Comparing `polygone-nms-0.1.6/README.md` & `polygone-nms-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,20 +32,24 @@
 # Example input data
 data = np.array([
     [0, 0, 1, 1, 0, 1, 0, 0, 1, 0.9],
     [0.5, 0.5, 1.5, 1.5, 0.5, 1.5, 0, 0, 1, 0.8],
 ])
 
 # Apply NMS
-results = polygone_nms(data, distributed=None, nms_method="Default", intersection_method="IOU")
+results = nms(data, distributed=None, nms_method="Default", intersection_method="IOU")
 
-print(results)
+print("Filtered indices:", results)
+
+# Filtered data
+print("Filtered data:")
+print(data[results])
 ```
 
-For a more detailed guide on using PolyGoneNMS, please see the [Quickstart](https://www.example.com/) in the documentation.
+For a more detailed guide on using PolyGoneNMS, please see the [Quickstart](https://wolodjaz.github.io/PolyGoneNMS/0.1.6/quickstart/) in the documentation.
 
 ## Documentation
 
 Detailed documentation is available at:
 [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=flat)](https://wolodjaz.github.io/PolyGoneNMS)
```

### Comparing `polygone-nms-0.1.6/polygone_nms/nms.py` & `polygone-nms-0.1.7/polygone_nms/nms.py`

 * *Files identical despite different names*

### Comparing `polygone-nms-0.1.6/polygone_nms/utils.py` & `polygone-nms-0.1.7/polygone_nms/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -273,14 +273,18 @@
     # Calculate the intersection area
     intersection_area = poly1.intersection(poly2).area
 
     # Calculate the union
     union_area = poly1.area + poly2.area - intersection_area
     # union_area = poly1.union(poly2).area tested and it's slower
 
+    # If the union area is 0, return 0
+    if union_area == 0:
+        return 0
+
     # Calculate the IoU
     return intersection_area / union_area
 
 
 def ios(poly1: Polygon, poly2: Polygon) -> float:
     """
     Compute the intersection over smaller (IoS) between two Shapely Polygons.
@@ -316,14 +320,18 @@
     """
     # Calculate the intersection area
     intersection_area = poly1.intersection(poly2).area
 
     # Calculate the area of the smaller polygon
     smaller_area = min(poly1.area, poly2.area)
 
+    # If the smaller area is 0, return 0
+    if smaller_area == 0:
+        return 0
+
     # Calculate the IoS
     return intersection_area / smaller_area
 
 
 def dice(poly1: Polygon, poly2: Polygon) -> float:
     """
     Compute the dice coefficient between two Shapely Polygons.
@@ -357,16 +365,23 @@
             The second polygon represented by a shapely.geometry.Polygon object.
     Returns:
         float: The Dice value between the two Shapely Polygons.
     """
     # Calculate the intersection
     intersection = poly1.intersection(poly2)
 
+    # Calculate the sum area
+    sum_area = poly1.area + poly2.area
+
+    # If the sum area is 0, than Polygons are empty in future are information #TODO
+    if sum_area == 0:
+        return 0
+
     # Calculate the Dice coefficient
-    return 2 * intersection.area / (poly1.area + poly2.area)
+    return 2 * intersection.area / sum_area
 
 
 def iot(target: Polygon, compared: Polygon) -> float:
     """
     Compute the intersection over target (IoT) between two Shapely Polygons.
 
     IoT is another overlap metric that measures the ratio of the area of
@@ -405,9 +420,13 @@
     """
     # Calculate the intersection area
     intersection_area = target.intersection(compared).area
 
     # Calculate the area of the target polygon
     target_area = target.area
 
+    # If the target area is 0, than Polygons are empty in future are information #TODO
+    if target_area == 0:
+        return 0
+
     # Calculate the IoT
     return intersection_area / target_area
```

### Comparing `polygone-nms-0.1.6/polygone_nms.egg-info/PKG-INFO` & `polygone-nms-0.1.7/polygone_nms.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygone-nms
-Version: 0.1.6
+Version: 0.1.7
 Summary: Efficient and distributed polygon Non-Maximum Suppression (NMS) library
 Home-page: https://github.com/WolodjaZ/polygone-nms
 Author: Vladimir Zaigrajew
 Author-email: vladimirzaigrajew@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -58,20 +58,24 @@
 # Example input data
 data = np.array([
     [0, 0, 1, 1, 0, 1, 0, 0, 1, 0.9],
     [0.5, 0.5, 1.5, 1.5, 0.5, 1.5, 0, 0, 1, 0.8],
 ])
 
 # Apply NMS
-results = polygone_nms(data, distributed=None, nms_method="Default", intersection_method="IOU")
+results = nms(data, distributed=None, nms_method="Default", intersection_method="IOU")
 
-print(results)
+print("Filtered indices:", results)
+
+# Filtered data
+print("Filtered data:")
+print(data[results])
 ```
 
-For a more detailed guide on using PolyGoneNMS, please see the [Quickstart](https://www.example.com/) in the documentation.
+For a more detailed guide on using PolyGoneNMS, please see the [Quickstart](https://wolodjaz.github.io/PolyGoneNMS/0.1.6/quickstart/) in the documentation.
 
 ## Documentation
 
 Detailed documentation is available at:
 [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=flat)](https://wolodjaz.github.io/PolyGoneNMS)
```

### Comparing `polygone-nms-0.1.6/setup.cfg` & `polygone-nms-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `polygone-nms-0.1.6/setup.py` & `polygone-nms-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `polygone-nms-0.1.6/tests/test_nms.py` & `polygone-nms-0.1.7/tests/test_nms.py`

 * *Files identical despite different names*

### Comparing `polygone-nms-0.1.6/tests/test_polygone_nms.py` & `polygone-nms-0.1.7/tests/test_polygone_nms.py`

 * *Files identical despite different names*

### Comparing `polygone-nms-0.1.6/tests/test_utils.py` & `polygone-nms-0.1.7/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         (
             [(0, 0), (1, 0), (1, 1), (0, 1)],
             [(0.5, 0), (1.5, 0), (1.5, 1), (0.5, 1)],
             0.3,
         ),
         ([(0, 0), (1, 0), (1, 1), (0, 1)], [(2, 0), (3, 0), (3, 1), (2, 1)], 0.0),
         ([(0, 0), (1, 0), (1, 1), (0, 1)], [(0, 0), (1, 0), (1, 1), (0, 1)], 1.0),
+        ([(0, 0), (0, 0), (0, 0), (0, 0)], [(1, 1), (1, 1), (1, 1), (1, 1)], 0.0),
     ],
 )
 def test_iou(poly1_list, poly2_list, expected):
     poly1 = Polygon(poly1_list)
     poly2 = Polygon(poly2_list)
     assert round(iou(poly1, poly2), 1) == expected
 
@@ -155,14 +156,15 @@
         (
             [(0, 0), (1, 0), (1, 1), (0, 1)],
             [(0.5, 0), (1.5, 0), (1.5, 1), (0.5, 1)],
             0.5,
         ),
         ([(0, 0), (1, 0), (1, 1), (0, 1)], [(2, 0), (3, 0), (3, 1), (2, 1)], 0.0),
         ([(0, 0), (1, 0), (1, 1), (0, 1)], [(-1, -1), (2, -1), (2, 2), (-1, 2)], 1.0),
+        ([(0, 0), (0, 0), (0, 0), (0, 0)], [(1, 1), (1, 1), (1, 1), (1, 1)], 0.0),
     ],
 )
 def test_ios(poly1_list, poly2_list, expected):
     poly1 = Polygon(poly1_list)
     poly2 = Polygon(poly2_list)
     assert round(ios(poly1, poly2), 1) == expected
 
@@ -173,14 +175,15 @@
         (
             [(0, 0), (1, 0), (1, 1), (0, 1)],
             [(0.5, 0), (1.5, 0), (1.5, 1), (0.5, 1)],
             0.5,
         ),
         ([(0, 0), (1, 0), (1, 1), (0, 1)], [(2, 0), (3, 0), (3, 1), (2, 1)], 0.0),
         ([(0, 0), (1, 0), (1, 1), (0, 1)], [(0, 0), (1, 0), (1, 1), (0, 1)], 1.0),
+        ([(0, 0), (0, 0), (0, 0), (0, 0)], [(1, 1), (1, 1), (1, 1), (1, 1)], 0.0),
     ],
 )
 def test_dice(poly1_list, poly2_list, expected):
     poly1 = Polygon(poly1_list)
     poly2 = Polygon(poly2_list)
     assert round(dice(poly1, poly2), 1) == expected
 
@@ -196,13 +199,14 @@
         (
             [(0, 0), (1, 0), (1, 1), (0, 1)],
             [(0.5, 0), (1.5, 0), (1.5, 1), (0.5, 1)],
             0.5,
         ),
         ([(0, 0), (1, 0), (1, 1), (0, 1)], [(2, 0), (3, 0), (3, 1), (2, 1)], 0.0),
         ([(0, 0), (1, 0), (1, 1), (0, 1)], [(0, 0), (1, 0), (1, 1), (0, 1)], 1.0),
+        ([(0, 0), (0, 0), (0, 0), (0, 0)], [(1, 1), (1, 1), (1, 1), (1, 1)], 0.0),
     ],
 )
 def test_iot(poly1_list, poly2_list, expected):
     poly1 = Polygon(poly1_list)
     poly2 = Polygon(poly2_list)
     assert round(iot(poly1, poly2), 1) == expected
```

