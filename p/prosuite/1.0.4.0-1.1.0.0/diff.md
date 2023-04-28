# Comparing `tmp/prosuite-1.0.4.0.tar.gz` & `tmp/prosuite-1.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosuite-1.0.4.0.tar", last modified: Fri Mar 24 16:02:05 2023, max compression
+gzip compressed data, was "prosuite-1.1.0.0.tar", last modified: Fri Apr 28 13:38:51 2023, max compression
```

## Comparing `prosuite-1.0.4.0.tar` & `prosuite-1.1.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 16:02:05.870046 prosuite-1.0.4.0/
--rw-rw-rw-   0        0        0     1103 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1701 2023-03-24 16:02:05.871055 prosuite-1.0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2023-02-24 14:29:45.000000 prosuite-1.0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 16:02:05.835047 prosuite-1.0.4.0/prosuite/
--rw-rw-rw-   0        0        0      959 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/__init__.py
--rw-rw-rw-   0        0        0      984 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/advanced_parameters.py
--rw-rw-rw-   0        0        0     4269 2023-03-24 06:45:02.000000 prosuite-1.0.4.0/prosuite/condition.py
--rw-rw-rw-   0        0        0     1109 2023-03-23 07:51:35.000000 prosuite-1.0.4.0/prosuite/dataset.py
-drwxrwxrwx   0        0        0        0 2023-03-24 16:02:05.852049 prosuite-1.0.4.0/prosuite/datatypes/
--rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/datatypes/__init__.py
--rw-rw-rw-   0        0        0      160 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/datatypes/esri_geometry_type.py
--rw-rw-rw-   0        0        0      127 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/datatypes/expected_case.py
--rw-rw-rw-   0        0        0      117 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/datatypes/expected_string_difference.py
--rw-rw-rw-   0        0        0      208 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/datatypes/non_linear_segment_type.py
--rw-rw-rw-   0        0        0       98 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/datatypes/unique_strings_constraint.py
-drwxrwxrwx   0        0        0        0 2023-03-24 16:02:05.860047 prosuite-1.0.4.0/prosuite/factories/
--rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/factories/__init__.py
--rw-rw-rw-   0        0        0     3540 2023-03-24 16:01:51.000000 prosuite-1.0.4.0/prosuite/factories/enums.py
--rw-rw-rw-   0        0        0      768 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/factories/issue_filters.py
--rw-rw-rw-   0        0        0   441304 2023-03-24 16:01:51.000000 prosuite-1.0.4.0/prosuite/factories/quality_conditions.py
--rw-rw-rw-   0        0        0      771 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/factories/transformers.py
-drwxrwxrwx   0        0        0        0 2023-03-24 16:02:05.869047 prosuite-1.0.4.0/prosuite/generated/
--rw-rw-rw-   0        0        0      454 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/generated/__init__.py
--rw-rw-rw-   0        0        0    21058 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/generated/quality_test_pb2.py
--rw-rw-rw-   0        0        0     2705 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/generated/quality_test_pb2_grpc.py
--rw-rw-rw-   0        0        0     7878 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/generated/quality_verification_service_pb2.py
--rw-rw-rw-   0        0        0     6983 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/generated/quality_verification_service_pb2_grpc.py
--rw-rw-rw-   0        0        0    21382 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/generated/shared_qa_pb2.py
--rw-rw-rw-   0        0        0    10649 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/generated/shared_types_pb2.py
--rw-rw-rw-   0        0        0      252 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/issue_filter.py
--rw-rw-rw-   0        0        0      496 2023-03-23 07:20:12.000000 prosuite-1.0.4.0/prosuite/model.py
--rw-rw-rw-   0        0        0     2146 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/parameter.py
--rw-rw-rw-   0        0        0      984 2023-03-24 06:49:44.000000 prosuite-1.0.4.0/prosuite/perimeter.py
--rw-rw-rw-   0        0        0    12515 2023-03-24 07:15:01.000000 prosuite-1.0.4.0/prosuite/service.py
--rw-rw-rw-   0        0        0      843 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/specification.py
--rw-rw-rw-   0        0        0      364 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/transformed_dataset.py
--rw-rw-rw-   0        0        0       92 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/transformer.py
--rw-rw-rw-   0        0        0     5142 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/utils.py
--rw-rw-rw-   0        0        0      489 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/verification_parameters.py
--rw-rw-rw-   0        0        0     2581 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/verification_response.py
--rw-rw-rw-   0        0        0     2543 2023-01-20 23:17:38.000000 prosuite-1.0.4.0/prosuite/xml_specification.py
-drwxrwxrwx   0        0        0        0 2023-03-24 16:02:05.846048 prosuite-1.0.4.0/prosuite.egg-info/
--rw-rw-rw-   0        0        0     1701 2023-03-24 16:02:05.000000 prosuite-1.0.4.0/prosuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-03-24 16:02:05.000000 prosuite-1.0.4.0/prosuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 16:02:05.000000 prosuite-1.0.4.0/prosuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-03-24 16:02:05.000000 prosuite-1.0.4.0/prosuite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-24 16:02:05.000000 prosuite-1.0.4.0/prosuite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-02-24 14:29:45.000000 prosuite-1.0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      925 2023-03-24 16:02:05.873048 prosuite-1.0.4.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-02-24 14:29:45.000000 prosuite-1.0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.542591 prosuite-1.1.0.0/
+-rw-rw-rw-   0        0        0     1103 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1701 2023-04-28 13:38:51.542591 prosuite-1.1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2023-02-24 14:29:45.000000 prosuite-1.1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.514593 prosuite-1.1.0.0/prosuite/
+-rw-rw-rw-   0        0        0      959 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/__init__.py
+-rw-rw-rw-   0        0        0      984 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/advanced_parameters.py
+-rw-rw-rw-   0        0        0     4269 2023-04-12 17:32:29.000000 prosuite-1.1.0.0/prosuite/condition.py
+-rw-rw-rw-   0        0        0     1109 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.526591 prosuite-1.1.0.0/prosuite/datatypes/
+-rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/esri_geometry_type.py
+-rw-rw-rw-   0        0        0      127 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/expected_case.py
+-rw-rw-rw-   0        0        0      117 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/expected_string_difference.py
+-rw-rw-rw-   0        0        0      208 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/non_linear_segment_type.py
+-rw-rw-rw-   0        0        0       98 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/unique_strings_constraint.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.531592 prosuite-1.1.0.0/prosuite/factories/
+-rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/factories/__init__.py
+-rw-rw-rw-   0        0        0     3540 2023-04-28 13:38:33.000000 prosuite-1.1.0.0/prosuite/factories/enums.py
+-rw-rw-rw-   0        0        0      768 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/factories/issue_filters.py
+-rw-rw-rw-   0        0        0   441467 2023-04-28 13:38:33.000000 prosuite-1.1.0.0/prosuite/factories/quality_conditions.py
+-rw-rw-rw-   0        0        0      771 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/factories/transformers.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.541592 prosuite-1.1.0.0/prosuite/generated/
+-rw-rw-rw-   0        0        0      454 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/__init__.py
+-rw-rw-rw-   0        0        0    21058 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/quality_test_pb2.py
+-rw-rw-rw-   0        0        0     2705 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/quality_test_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7878 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/quality_verification_service_pb2.py
+-rw-rw-rw-   0        0        0     6983 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/quality_verification_service_pb2_grpc.py
+-rw-rw-rw-   0        0        0    21382 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/shared_qa_pb2.py
+-rw-rw-rw-   0        0        0    10649 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/shared_types_pb2.py
+-rw-rw-rw-   0        0        0      252 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/issue_filter.py
+-rw-rw-rw-   0        0        0      496 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/model.py
+-rw-rw-rw-   0        0        0     2146 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/parameter.py
+-rw-rw-rw-   0        0        0      984 2023-04-12 17:32:29.000000 prosuite-1.1.0.0/prosuite/perimeter.py
+-rw-rw-rw-   0        0        0    14618 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/service.py
+-rw-rw-rw-   0        0        0      843 2023-04-28 12:31:16.000000 prosuite-1.1.0.0/prosuite/specification.py
+-rw-rw-rw-   0        0        0      364 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/transformed_dataset.py
+-rw-rw-rw-   0        0        0       92 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/transformer.py
+-rw-rw-rw-   0        0        0     5321 2023-04-24 10:20:56.000000 prosuite-1.1.0.0/prosuite/utils.py
+-rw-rw-rw-   0        0        0      489 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/verification_parameters.py
+-rw-rw-rw-   0        0        0     2581 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/verification_response.py
+-rw-rw-rw-   0        0        0     2543 2023-04-28 13:17:28.000000 prosuite-1.1.0.0/prosuite/xml_specification.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.519592 prosuite-1.1.0.0/prosuite.egg-info/
+-rw-rw-rw-   0        0        0     1701 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-02-24 14:29:45.000000 prosuite-1.1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      925 2023-04-28 13:38:51.543592 prosuite-1.1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-02-24 14:29:45.000000 prosuite-1.1.0.0/setup.py
```

### Comparing `prosuite-1.0.4.0/LICENSE` & `prosuite-1.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/PKG-INFO` & `prosuite-1.1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosuite
-Version: 1.0.4.0
+Version: 1.1.0.0
 Summary: An API to configure quality assurance tests for geodata and execute quality verifications on a ProSuite Server
 Home-page: https://dirageosystems.ch/prosuite/doc/api
 Author: Dira GeoSystems
 Author-email: programmers@dirageosystems.ch
 License: MIT
 Keywords: prosuite,gis,arcgis,geodata,spatial-data,quality,quality-assurance,qa,test
 Classifier: Operating System :: OS Independent
```

### Comparing `prosuite-1.0.4.0/README.md` & `prosuite-1.1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/__init__.py` & `prosuite-1.1.0.0/prosuite/__init__.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/advanced_parameters.py` & `prosuite-1.1.0.0/prosuite/advanced_parameters.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/condition.py` & `prosuite-1.1.0.0/prosuite/condition.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/dataset.py` & `prosuite-1.1.0.0/prosuite/dataset.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/factories/enums.py` & `prosuite-1.1.0.0/prosuite/factories/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿__author__ = "The ProSuite Authors"
 __copyright__ = "Copyright 2021-2023, The ProSuite Authors"
 __license__ = "MIT"
-__version__ = "1.0.4.0"
+__version__ = "1.1.0.0"
 __maintainer__ = "Dira GeoSystems"
 __email__ = "programmers@dirageosystems.ch"
-__date__  = "24.03.2023"
+__date__  = "28.04.2023"
 __status__ = "Production"
 
 
 from datetime import datetime
 from typing import List
```

### Comparing `prosuite-1.0.4.0/prosuite/factories/issue_filters.py` & `prosuite-1.1.0.0/prosuite/factories/issue_filters.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/factories/quality_conditions.py` & `prosuite-1.1.0.0/prosuite/factories/quality_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿__author__ = "The ProSuite Authors"
 __copyright__ = "Copyright 2021-2023, The ProSuite Authors"
 __license__ = "MIT"
-__version__ = "1.0.4.0"
+__version__ = "1.1.0.0"
 __maintainer__ = "Dira GeoSystems"
 __email__ = "programmers@dirageosystems.ch"
-__date__  = "24.03.2023"
+__date__  = "28.04.2023"
 __status__ = "Production"
 
 
 from datetime import datetime
 from typing import List
 from prosuite.condition import Condition
 from prosuite.parameter import Parameter
@@ -4207,15 +4207,15 @@
         result.parameters.append(Parameter("featureClass", feature_class))
         result.generate_name()
         return result
 
     @classmethod
     def qa_orphan_node_0(cls, point_classes: List[BaseDataset], polyline_classes: List[BaseDataset]) -> Condition:
         """
-        Finds all points in 'pointClasses' that are neither from nor to point of any feature in 'polylineClasses'
+        Finds all points in 'pointClasses' that are neither From- nor To-point of any feature in 'polylineClasses' and line end points without any point
         
         Remark: All feature classes in 'pointClasses' and 'polylineClasses' must have the same spatial reference.
         """
         
         result = Condition("QaOrphanNode(0)")
         if type(point_classes) == list:
             for element in point_classes:
@@ -4229,29 +4229,29 @@
             result.parameters.append(Parameter("polylineClasses", polyline_classes))
         result.generate_name()
         return result
 
     @classmethod
     def qa_orphan_node_1(cls, point_class: BaseDataset, polyline_class: BaseDataset) -> Condition:
         """
-        Finds all points in 'pointClass' that are neither from nor to point of any feature in 'polylineClass'
+        Finds all points in 'pointClass' that are neither From- nor To-point of any feature in 'polylineClass' and line end points without any point
         
         Remark: The feature classes in 'pointClass' and 'polylineClass' must have the same spatial reference.
         """
         
         result = Condition("QaOrphanNode(1)")
         result.parameters.append(Parameter("pointClass", point_class))
         result.parameters.append(Parameter("polylineClass", polyline_class))
         result.generate_name()
         return result
 
     @classmethod
     def qa_orphan_node_2(cls, point_classes: List[BaseDataset], polyline_classes: List[BaseDataset], error_type: OrphanErrorType) -> Condition:
         """
-        Finds all points in 'pointClasses' that are neither from nor to point of any feature in 'polylineClasses'.
+        Finds all points in 'pointClasses' that are neither From- nor To-point of any feature in 'polylineClasses' and\/or line end points without any point
         Performs the tests defined in 'errorType'.
         
         Remark: All feature classes in 'pointClasses' and 'polylineClasses' must have the same spatial reference.
         """
         
         result = Condition("QaOrphanNode(2)")
         if type(point_classes) == list:
@@ -4267,15 +4267,15 @@
         result.parameters.append(Parameter("errorType", error_type))
         result.generate_name()
         return result
 
     @classmethod
     def qa_orphan_node_3(cls, point_class: BaseDataset, polyline_class: BaseDataset, error_type: OrphanErrorType) -> Condition:
         """
-        Finds all points in 'pointClass' that are neither from nor to point of any feature in 'polylineClass'
+        Finds all points in 'pointClass' that are neither From- nor To-point of any feature in 'polylineClass' and\/or line end points without any point
         Performs the tests defined in 'errorType'.
         
         Remark: The feature classes in 'pointClass' and 'polylineClass' must have the same spatial reference.
         """
         
         result = Condition("QaOrphanNode(3)")
         result.parameters.append(Parameter("pointClass", point_class))
```

### Comparing `prosuite-1.0.4.0/prosuite/factories/transformers.py` & `prosuite-1.1.0.0/prosuite/factories/transformers.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/generated/quality_test_pb2.py` & `prosuite-1.1.0.0/prosuite/generated/quality_test_pb2.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/generated/quality_test_pb2_grpc.py` & `prosuite-1.1.0.0/prosuite/generated/quality_test_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/generated/quality_verification_service_pb2.py` & `prosuite-1.1.0.0/prosuite/generated/quality_verification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/generated/quality_verification_service_pb2_grpc.py` & `prosuite-1.1.0.0/prosuite/generated/quality_verification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/generated/shared_qa_pb2.py` & `prosuite-1.1.0.0/prosuite/generated/shared_qa_pb2.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/generated/shared_types_pb2.py` & `prosuite-1.1.0.0/prosuite/generated/shared_types_pb2.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/parameter.py` & `prosuite-1.1.0.0/prosuite/parameter.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/perimeter.py` & `prosuite-1.1.0.0/prosuite/perimeter.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/service.py` & `prosuite-1.1.0.0/prosuite/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,48 +19,93 @@
 
 from prosuite.dataset import Dataset
 
 MAX_MESSAGE_LENGTH_MB = 1024
 
 class Service:
     """
-    The service class communicates on the http/2 channel and executes server functions.
+    The service class communicates on the http/2 channel with the server and initiates the 
+    quality verifications.
 
-    :param host_name: The host running the quality verification service
+    :param host_name: The name or IP address of the host running the quality verification service.
     :type host_name: str
-    :param port_nr: The port used by the quality verification service
+    :param port_nr: The port used by the quality verification service.
     :type port_nr: int
-    :param channel_credentials: The ssl credentials and authentication between client and server. 
+    :param channel_credentials: The channel credentials to be used for TLS/SSL server 
+        authentication, if required by the server (Default: None -> No TLS/SSL).
+
         Use :py:meth:`prosuite.utils.get_ssl_channel_credentials` to create the basic https 
-        if the required root certificates are in the windows certificate store.
+        credentials if the appropria root certificates are in the windows certificate store.
         For advanced scenarios or credentials on a non-windows platform, see the gRPC Python docs
         (https://grpc.github.io/grpc/python/grpc.html).
     :type channel_credentials: grpc.ChannelCredentials  
     """
 
     ISSUE_GDB = "Issues.gdb"
+    """The name of the issue File Geodatabase. 
+        It will be written to the output_dir specified in the :py:meth:`prosuite.service.Service.verify` 
+        method. This File Geodatabase contains the issues found during the verification and could 
+        be used as the source for the Issue Worklist in the ProSuite QA Add-In for ArcGIS Pro.
+    """
+
     XML_REPORT = "verification.xml"
+    """The name of the xml verification report.
+        It will be written to the output_dir specified in the :py:meth:`prosuite.service.Service.verify` 
+        method.
+    """
+
     HTML_REPORT = "verification.html"
+    """The name of the html verification report.
+        It will be written to the output_dir specified in the :py:meth:`prosuite.service.Service.verify` 
+        method.
+    """
 
     def __init__(self, host_name: str, port_nr: int, channel_credentials: grpc.ssl_channel_credentials = None):
         #:
         self.host_name = host_name
+        """The host name.
+
+        :meta private:
+        """
         #:
         self.port_nr = port_nr
+        """The port.
+
+        :meta private:
+        """
         #:
         self.ssl_channel_credentials: grpc.ssl_channel_credentials = channel_credentials
+        """The TLS/SSL credentials.
 
-    def verify(self, specification: Union[Specification, XmlSpecification], perimeter: Union[EnvelopePerimeter,
-                                                                                             EsriShapePerimeter, WkbPerimeter] = None, output_dir: str = None, parameters: VerificationParameters = None) -> Iterable[VerificationResponse]:
+        :meta private:
         """
-        executes a verification. Runs all tests that are defined in the specification.
+
+    def verify(self, specification: Union[Specification, XmlSpecification],
+               perimeter: Union[EnvelopePerimeter, EsriShapePerimeter, WkbPerimeter] = None, 
+               output_dir: str = None, 
+               parameters: VerificationParameters = None) -> Iterable[VerificationResponse]:
+        """
+        Executes a quality verification by running all the quality conditions defined in the 
+        provided quality specification.
         Returns a collection of VerificationResponse objects, containing the verification
         messages.
 
-        :return: Iterator for looping over VerificationResponse objects
+        Please refer to the :ref:`samples <samples-link>` for more details.
+
+        :param specification: The quality specification containing the conditions to be verified.
+            It can be either a :py:class:`prosuite.specification.Specification` directly defined in 
+            python code or a :py:class:`prosuite.xml_specification.XmlSpecification` from an XML 
+            file, for example created by the XML export in the ProSuite Data Dictionary Editor.
+        :param perimeter: The perimeter that defines the polygon or extent of the verification.
+            Default: None -> Full extent of the verified datasets.
+        :param output_dir: The output directory (must be writable / creatable by the service process).
+            Default: No output is written by the server process.
+        :param parameters: Additional optional verification parameters.
+        :return: Iterator for looping over VerificationResponse objects. The verification response
+            contains progress information, found issues and, in the final message, the verification results.
         :rtype: Iterator[VerificationResponse]
         """
 
         advanced_parameters = AdvancedParameters(
             specification, output_dir, perimeter, parameters)
 
         self._validate_params(advanced_parameters)
```

### Comparing `prosuite-1.0.4.0/prosuite/specification.py` & `prosuite-1.1.0.0/prosuite/specification.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/utils.py` & `prosuite-1.1.0.0/prosuite/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,15 +146,17 @@
     if value:
         return value
     return default
 
 
 def get_ssl_channel_credentials() -> grpc.ssl_channel_credentials:
     """
-    create a ssl channel credentials object for use with an SSL-enabled channel.
+    Creates an ssl channel credentials object for use with an SSL-enabled channel for the 
+    authentication with a server that requires TLS/SSL. The appropriate root certificates
+    for server authentication are loaded from the windows certificate store.
 
     :return: A ChannelCredentials object
     """
     ctx = ssl.create_default_context()
     ca_certs = ctx.get_ca_certs(binary_form=True)
     ctx.load_default_certs(purpose=ssl.Purpose.SERVER_AUTH)
```

### Comparing `prosuite-1.0.4.0/prosuite/verification_response.py` & `prosuite-1.1.0.0/prosuite/verification_response.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite/xml_specification.py` & `prosuite-1.1.0.0/prosuite/xml_specification.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/prosuite.egg-info/PKG-INFO` & `prosuite-1.1.0.0/prosuite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosuite
-Version: 1.0.4.0
+Version: 1.1.0.0
 Summary: An API to configure quality assurance tests for geodata and execute quality verifications on a ProSuite Server
 Home-page: https://dirageosystems.ch/prosuite/doc/api
 Author: Dira GeoSystems
 Author-email: programmers@dirageosystems.ch
 License: MIT
 Keywords: prosuite,gis,arcgis,geodata,spatial-data,quality,quality-assurance,qa,test
 Classifier: Operating System :: OS Independent
```

### Comparing `prosuite-1.0.4.0/prosuite.egg-info/SOURCES.txt` & `prosuite-1.1.0.0/prosuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosuite-1.0.4.0/setup.cfg` & `prosuite-1.1.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 00000160: 726b 646f 776e 0d0a 6b65 7977 6f72 6473  rkdown..keywords
 00000170: 203d 2070 726f 7375 6974 652c 2067 6973   = prosuite, gis
 00000180: 2c20 6172 6367 6973 2c20 6765 6f64 6174  , arcgis, geodat
 00000190: 612c 2073 7061 7469 616c 2d64 6174 612c  a, spatial-data,
 000001a0: 2071 7561 6c69 7479 2c20 7175 616c 6974   quality, qualit
 000001b0: 792d 6173 7375 7261 6e63 652c 2071 612c  y-assurance, qa,
 000001c0: 2074 6573 740d 0a76 6572 7369 6f6e 203d   test..version =
-000001d0: 2031 2e30 2e34 2e30 0d0a 6c69 6365 6e73   1.0.4.0..licens
+000001d0: 2031 2e31 2e30 2e30 0d0a 6c69 6365 6e73   1.1.0.0..licens
 000001e0: 6520 3d20 4d49 540d 0a6c 6963 656e 7365  e = MIT..license
 000001f0: 5f66 696c 6573 203d 204c 4943 454e 5345  _files = LICENSE
 00000200: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
 00000210: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
 00000220: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
 00000230: 6e64 656e 740d 0a09 5072 6f67 7261 6d6d  ndent...Programm
 00000240: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language ::
```

