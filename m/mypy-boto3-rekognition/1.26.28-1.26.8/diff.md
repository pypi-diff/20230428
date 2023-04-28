# Comparing `tmp/mypy-boto3-rekognition-1.26.28.tar.gz` & `tmp/mypy-boto3-rekognition-1.26.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rekognition-1.26.28.tar", last modified: Mon Dec 12 20:27:27 2022, max compression
+gzip compressed data, was "mypy-boto3-rekognition-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
```

## Comparing `mypy-boto3-rekognition-1.26.28.tar` & `mypy-boto3-rekognition-1.26.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.871752 mypy-boto3-rekognition-1.26.28/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24730 2022-12-12 20:27:27.871752 mypy-boto3-rekognition-1.26.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23227 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.867752 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51097 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51017 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2022-12-12 20:27:08.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    83699 2022-12-12 20:27:10.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83598 2022-12-12 20:27:09.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.871752 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24730 2022-12-12 20:27:27.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2022-12-12 20:27:27.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:27:27.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:27:27.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-12 20:27:27.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-12 20:27:27.000000 mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 20:27:27.871752 mypy-boto3-rekognition-1.26.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2022-12-12 20:27:07.000000 mypy-boto3-rekognition-1.26.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.082122 mypy-boto3-rekognition-1.26.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    24573 2022-11-11 21:07:54.078122 mypy-boto3-rekognition-1.26.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    23122 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.070122 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50861 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50781 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    12528 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12526 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     9820 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9810 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    83084 2022-11-11 21:07:34.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    82983 2022-11-11 21:07:33.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-11-11 21:07:32.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.078122 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    24573 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-11 21:07:53.000000 mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.082122 mypy-boto3-rekognition-1.26.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-11-11 21:07:31.000000 mypy-boto3-rekognition-1.26.8/setup.py
```

### Comparing `mypy-boto3-rekognition-1.26.28/LICENSE` & `mypy-boto3-rekognition-1.26.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.28/PKG-INFO` & `mypy-boto3-rekognition-1.26.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.26.28
-Summary: Type annotations for boto3.Rekognition 1.26.28 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.8
+Summary: Type annotations for boto3.Rekognition 1.26.8 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,16 +366,14 @@
     DescribeProjectsPaginatorName,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
-    LabelDetectionAggregateByType,
-    LabelDetectionFeatureNameType,
     LabelDetectionSortByType,
     LandmarkTypeType,
     ListCollectionsPaginatorName,
     ListDatasetEntriesPaginatorName,
     ListDatasetLabelsPaginatorName,
     ListFacesPaginatorName,
     ListProjectPoliciesPaginatorName,
@@ -565,15 +562,14 @@
     ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
-    LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestTypeDef,
     GroundTruthManifestTypeDef,
```

### Comparing `mypy-boto3-rekognition-1.26.28/README.md` & `mypy-boto3-rekognition-1.26.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,16 +335,14 @@
     DescribeProjectsPaginatorName,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
-    LabelDetectionAggregateByType,
-    LabelDetectionFeatureNameType,
     LabelDetectionSortByType,
     LandmarkTypeType,
     ListCollectionsPaginatorName,
     ListDatasetEntriesPaginatorName,
     ListDatasetLabelsPaginatorName,
     ListFacesPaginatorName,
     ListProjectPoliciesPaginatorName,
@@ -533,15 +531,14 @@
     ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
-    LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestTypeDef,
     GroundTruthManifestTypeDef,
```

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/__init__.py` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/__init__.pyi` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/client.py` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     AttributeType,
     CelebrityRecognitionSortByType,
     ContentModerationSortByType,
     DatasetTypeType,
     DetectLabelsFeatureNameType,
     FaceAttributesType,
     FaceSearchSortByType,
-    LabelDetectionAggregateByType,
     LabelDetectionSortByType,
     PersonTrackingSortByType,
     QualityFilterType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
 )
 from .paginator import (
@@ -79,15 +78,14 @@
     GetLabelDetectionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     HumanLoopConfigTypeDef,
     ImageTypeDef,
     IndexFacesResponseTypeDef,
-    LabelDetectionSettingsTypeDef,
     ListCollectionsResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     ListFacesResponseTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -539,15 +537,15 @@
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: CelebrityRecognitionSortByType = ...
     ) -> GetCelebrityRecognitionResponseTypeDef:
         """
         Gets the celebrity recognition results for a Amazon Rekognition Video analysis
-        started by  StartCelebrityRecognition.
+        started by  StartCelebrityRecognition .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_recognition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_celebrity_recognition)
         """
 
     def get_content_moderation(
         self,
@@ -566,15 +564,15 @@
         """
 
     def get_face_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetFaceDetectionResponseTypeDef:
         """
         Gets face detection results for a Amazon Rekognition Video analysis started by
-        StartFaceDetection.
+        StartFaceDetection .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_face_detection)
         """
 
     def get_face_search(
         self,
@@ -594,20 +592,19 @@
 
     def get_label_detection(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: LabelDetectionSortByType = ...,
-        AggregateBy: LabelDetectionAggregateByType = ...
+        SortBy: LabelDetectionSortByType = ...
     ) -> GetLabelDetectionResponseTypeDef:
         """
         Gets the label detection results of a Amazon Rekognition Video analysis started
-        by  StartLabelDetection.
+        by  StartLabelDetection .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_label_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_label_detection)
         """
 
     def get_person_tracking(
         self,
@@ -615,37 +612,37 @@
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: PersonTrackingSortByType = ...
     ) -> GetPersonTrackingResponseTypeDef:
         """
         Gets the path tracking results of a Amazon Rekognition Video analysis started by
-        StartPersonTracking.
+        StartPersonTracking .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_person_tracking)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_person_tracking)
         """
 
     def get_segment_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetSegmentDetectionResponseTypeDef:
         """
         Gets the segment detection results of a Amazon Rekognition Video analysis
-        started by  StartSegmentDetection.
+        started by  StartSegmentDetection .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_segment_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_segment_detection)
         """
 
     def get_text_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetTextDetectionResponseTypeDef:
         """
         Gets the text detection results of a Amazon Rekognition Video analysis started
-        by  StartTextDetection.
+        by  StartTextDetection .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_text_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_text_detection)
         """
 
     def index_faces(
         self,
@@ -723,15 +720,15 @@
         """
 
     def list_stream_processors(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListStreamProcessorsResponseTypeDef:
         """
         Gets a list of stream processors that you have created with
-        CreateStreamProcessor.
+        CreateStreamProcessor .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_stream_processors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_stream_processors)
         """
 
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -863,17 +860,15 @@
     def start_label_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         MinConfidence: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...,
-        Features: Sequence[Literal["GENERAL_LABELS"]] = ...,
-        Settings: LabelDetectionSettingsTypeDef = ...
+        JobTag: str = ...
     ) -> StartLabelDetectionResponseTypeDef:
         """
         Starts asynchronous detection of labels in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_label_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#start_label_detection)
         """
@@ -956,15 +951,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_project_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#stop_project_version)
         """
 
     def stop_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
-        Stops a running stream processor that was created by  CreateStreamProcessor.
+        Stops a running stream processor that was created by  CreateStreamProcessor .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_stream_processor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#stop_stream_processor)
         """
 
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/client.pyi` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     AttributeType,
     CelebrityRecognitionSortByType,
     ContentModerationSortByType,
     DatasetTypeType,
     DetectLabelsFeatureNameType,
     FaceAttributesType,
     FaceSearchSortByType,
-    LabelDetectionAggregateByType,
     LabelDetectionSortByType,
     PersonTrackingSortByType,
     QualityFilterType,
     SegmentTypeType,
     StreamProcessorParameterToDeleteType,
 )
 from .paginator import (
@@ -79,15 +78,14 @@
     GetLabelDetectionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     GetTextDetectionResponseTypeDef,
     HumanLoopConfigTypeDef,
     ImageTypeDef,
     IndexFacesResponseTypeDef,
-    LabelDetectionSettingsTypeDef,
     ListCollectionsResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     ListFacesResponseTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -504,15 +502,15 @@
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: CelebrityRecognitionSortByType = ...
     ) -> GetCelebrityRecognitionResponseTypeDef:
         """
         Gets the celebrity recognition results for a Amazon Rekognition Video analysis
-        started by  StartCelebrityRecognition.
+        started by  StartCelebrityRecognition .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_recognition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_celebrity_recognition)
         """
     def get_content_moderation(
         self,
         *,
@@ -529,15 +527,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_content_moderation)
         """
     def get_face_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetFaceDetectionResponseTypeDef:
         """
         Gets face detection results for a Amazon Rekognition Video analysis started by
-        StartFaceDetection.
+        StartFaceDetection .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_face_detection)
         """
     def get_face_search(
         self,
         *,
@@ -555,55 +553,54 @@
         """
     def get_label_detection(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: LabelDetectionSortByType = ...,
-        AggregateBy: LabelDetectionAggregateByType = ...
+        SortBy: LabelDetectionSortByType = ...
     ) -> GetLabelDetectionResponseTypeDef:
         """
         Gets the label detection results of a Amazon Rekognition Video analysis started
-        by  StartLabelDetection.
+        by  StartLabelDetection .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_label_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_label_detection)
         """
     def get_person_tracking(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: PersonTrackingSortByType = ...
     ) -> GetPersonTrackingResponseTypeDef:
         """
         Gets the path tracking results of a Amazon Rekognition Video analysis started by
-        StartPersonTracking.
+        StartPersonTracking .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_person_tracking)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_person_tracking)
         """
     def get_segment_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetSegmentDetectionResponseTypeDef:
         """
         Gets the segment detection results of a Amazon Rekognition Video analysis
-        started by  StartSegmentDetection.
+        started by  StartSegmentDetection .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_segment_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_segment_detection)
         """
     def get_text_detection(
         self, *, JobId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetTextDetectionResponseTypeDef:
         """
         Gets the text detection results of a Amazon Rekognition Video analysis started
-        by  StartTextDetection.
+        by  StartTextDetection .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_text_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#get_text_detection)
         """
     def index_faces(
         self,
         *,
@@ -674,15 +671,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_project_policies)
         """
     def list_stream_processors(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListStreamProcessorsResponseTypeDef:
         """
         Gets a list of stream processors that you have created with
-        CreateStreamProcessor.
+        CreateStreamProcessor .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_stream_processors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#list_stream_processors)
         """
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags in an Amazon Rekognition collection, stream processor, or
@@ -804,17 +801,15 @@
     def start_label_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         MinConfidence: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...,
-        Features: Sequence[Literal["GENERAL_LABELS"]] = ...,
-        Settings: LabelDetectionSettingsTypeDef = ...
+        JobTag: str = ...
     ) -> StartLabelDetectionResponseTypeDef:
         """
         Starts asynchronous detection of labels in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_label_detection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#start_label_detection)
         """
@@ -890,15 +885,15 @@
         Stops a running model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_project_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#stop_project_version)
         """
     def stop_stream_processor(self, *, Name: str) -> Dict[str, Any]:
         """
-        Stops a running stream processor that was created by  CreateStreamProcessor.
+        Stops a running stream processor that was created by  CreateStreamProcessor .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.stop_stream_processor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#stop_stream_processor)
         """
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more key-value tags to an Amazon Rekognition collection, stream
```

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/literals.py` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     "DescribeProjectsPaginatorName",
     "DetectLabelsFeatureNameType",
     "EmotionNameType",
     "FaceAttributesType",
     "FaceSearchSortByType",
     "GenderTypeType",
     "KnownGenderTypeType",
-    "LabelDetectionAggregateByType",
-    "LabelDetectionFeatureNameType",
     "LabelDetectionSortByType",
     "LandmarkTypeType",
     "ListCollectionsPaginatorName",
     "ListDatasetEntriesPaginatorName",
     "ListDatasetLabelsPaginatorName",
     "ListFacesPaginatorName",
     "ListProjectPoliciesPaginatorName",
@@ -93,16 +91,14 @@
 EmotionNameType = Literal[
     "ANGRY", "CALM", "CONFUSED", "DISGUSTED", "FEAR", "HAPPY", "SAD", "SURPRISED", "UNKNOWN"
 ]
 FaceAttributesType = Literal["ALL", "DEFAULT"]
 FaceSearchSortByType = Literal["INDEX", "TIMESTAMP"]
 GenderTypeType = Literal["Female", "Male"]
 KnownGenderTypeType = Literal["Female", "Male", "Nonbinary", "Unlisted"]
-LabelDetectionAggregateByType = Literal["SEGMENTS", "TIMESTAMPS"]
-LabelDetectionFeatureNameType = Literal["GENERAL_LABELS"]
 LabelDetectionSortByType = Literal["NAME", "TIMESTAMP"]
 LandmarkTypeType = Literal[
     "chinBottom",
     "eyeLeft",
     "eyeRight",
     "leftEyeBrowLeft",
     "leftEyeBrowRight",
@@ -200,15 +196,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -218,29 +213,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -269,15 +262,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -325,15 +317,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -399,32 +390,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -452,44 +439,39 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/literals.pyi` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,14 @@
     "DescribeProjectsPaginatorName",
     "DetectLabelsFeatureNameType",
     "EmotionNameType",
     "FaceAttributesType",
     "FaceSearchSortByType",
     "GenderTypeType",
     "KnownGenderTypeType",
-    "LabelDetectionAggregateByType",
-    "LabelDetectionFeatureNameType",
     "LabelDetectionSortByType",
     "LandmarkTypeType",
     "ListCollectionsPaginatorName",
     "ListDatasetEntriesPaginatorName",
     "ListDatasetLabelsPaginatorName",
     "ListFacesPaginatorName",
     "ListProjectPoliciesPaginatorName",
@@ -91,16 +89,14 @@
 EmotionNameType = Literal[
     "ANGRY", "CALM", "CONFUSED", "DISGUSTED", "FEAR", "HAPPY", "SAD", "SURPRISED", "UNKNOWN"
 ]
 FaceAttributesType = Literal["ALL", "DEFAULT"]
 FaceSearchSortByType = Literal["INDEX", "TIMESTAMP"]
 GenderTypeType = Literal["Female", "Male"]
 KnownGenderTypeType = Literal["Female", "Male", "Nonbinary", "Unlisted"]
-LabelDetectionAggregateByType = Literal["SEGMENTS", "TIMESTAMPS"]
-LabelDetectionFeatureNameType = Literal["GENERAL_LABELS"]
 LabelDetectionSortByType = Literal["NAME", "TIMESTAMP"]
 LandmarkTypeType = Literal[
     "chinBottom",
     "eyeLeft",
     "eyeRight",
     "leftEyeBrowLeft",
     "leftEyeBrowRight",
@@ -198,15 +194,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -216,29 +211,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -267,15 +260,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -323,15 +315,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -397,32 +388,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -450,44 +437,39 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/paginator.py` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/paginator.pyi` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/type_defs.py` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     DatasetTypeType,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
-    LabelDetectionAggregateByType,
     LabelDetectionSortByType,
     LandmarkTypeType,
     OrientationCorrectionType,
     PersonTrackingSortByType,
     ProjectStatusType,
     ProjectVersionStatusType,
     ProtectiveEquipmentTypeType,
@@ -48,18 +47,14 @@
     TechnicalCueTypeType,
     TextTypesType,
     VideoColorRangeType,
     VideoJobStatusType,
 )
 
 if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AgeRangeTypeDef",
@@ -208,15 +203,14 @@
     "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     "DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     "DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     "DetectLabelsImageBackgroundTypeDef",
     "DetectLabelsImageForegroundTypeDef",
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
-    "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
     "RegionOfInterestTypeDef",
     "GroundTruthManifestTypeDef",
@@ -987,15 +981,14 @@
 )
 _OptionalGetLabelDetectionRequestRequestTypeDef = TypedDict(
     "_OptionalGetLabelDetectionRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": LabelDetectionSortByType,
-        "AggregateBy": LabelDetectionAggregateByType,
     },
     total=False,
 )
 
 
 class GetLabelDetectionRequestRequestTypeDef(
     _RequiredGetLabelDetectionRequestRequestTypeDef, _OptionalGetLabelDetectionRequestRequestTypeDef
@@ -2028,22 +2021,14 @@
     {
         "GeneralLabels": GeneralLabelsSettingsTypeDef,
         "ImageProperties": DetectLabelsImagePropertiesSettingsTypeDef,
     },
     total=False,
 )
 
-LabelDetectionSettingsTypeDef = TypedDict(
-    "LabelDetectionSettingsTypeDef",
-    {
-        "GeneralLabels": GeneralLabelsSettingsTypeDef,
-    },
-    total=False,
-)
-
 DetectModerationLabelsResponseTypeDef = TypedDict(
     "DetectModerationLabelsResponseTypeDef",
     {
         "ModerationLabels": List[ModerationLabelTypeDef],
         "ModerationModelVersion": str,
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2775,16 +2760,14 @@
 _OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_OptionalStartLabelDetectionRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "MinConfidence": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
-        "Features": Sequence[Literal["GENERAL_LABELS"]],
-        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
 
 class StartLabelDetectionRequestRequestTypeDef(
     _RequiredStartLabelDetectionRequestRequestTypeDef,
@@ -3020,17 +3003,14 @@
 )
 
 LabelDetectionTypeDef = TypedDict(
     "LabelDetectionTypeDef",
     {
         "Timestamp": int,
         "Label": LabelTypeDef,
-        "StartTimestampMillis": int,
-        "EndTimestampMillis": int,
-        "DurationMillis": int,
     },
     total=False,
 )
 
 CelebrityRecognitionTypeDef = TypedDict(
     "CelebrityRecognitionTypeDef",
     {
```

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/type_defs.pyi` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     DatasetTypeType,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
-    LabelDetectionAggregateByType,
     LabelDetectionSortByType,
     LandmarkTypeType,
     OrientationCorrectionType,
     PersonTrackingSortByType,
     ProjectStatusType,
     ProjectVersionStatusType,
     ProtectiveEquipmentTypeType,
@@ -48,18 +47,14 @@
     TechnicalCueTypeType,
     TextTypesType,
     VideoColorRangeType,
     VideoJobStatusType,
 )
 
 if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AgeRangeTypeDef",
     "AudioMetadataTypeDef",
@@ -207,15 +202,14 @@
     "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     "DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     "DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     "DetectLabelsImageBackgroundTypeDef",
     "DetectLabelsImageForegroundTypeDef",
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
-    "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
     "RegionOfInterestTypeDef",
     "GroundTruthManifestTypeDef",
@@ -970,15 +964,14 @@
 )
 _OptionalGetLabelDetectionRequestRequestTypeDef = TypedDict(
     "_OptionalGetLabelDetectionRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": LabelDetectionSortByType,
-        "AggregateBy": LabelDetectionAggregateByType,
     },
     total=False,
 )
 
 class GetLabelDetectionRequestRequestTypeDef(
     _RequiredGetLabelDetectionRequestRequestTypeDef, _OptionalGetLabelDetectionRequestRequestTypeDef
 ):
@@ -1973,22 +1966,14 @@
     {
         "GeneralLabels": GeneralLabelsSettingsTypeDef,
         "ImageProperties": DetectLabelsImagePropertiesSettingsTypeDef,
     },
     total=False,
 )
 
-LabelDetectionSettingsTypeDef = TypedDict(
-    "LabelDetectionSettingsTypeDef",
-    {
-        "GeneralLabels": GeneralLabelsSettingsTypeDef,
-    },
-    total=False,
-)
-
 DetectModerationLabelsResponseTypeDef = TypedDict(
     "DetectModerationLabelsResponseTypeDef",
     {
         "ModerationLabels": List[ModerationLabelTypeDef],
         "ModerationModelVersion": str,
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2694,16 +2679,14 @@
 _OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_OptionalStartLabelDetectionRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "MinConfidence": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
-        "Features": Sequence[Literal["GENERAL_LABELS"]],
-        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
 class StartLabelDetectionRequestRequestTypeDef(
     _RequiredStartLabelDetectionRequestRequestTypeDef,
     _OptionalStartLabelDetectionRequestRequestTypeDef,
@@ -2927,17 +2910,14 @@
 )
 
 LabelDetectionTypeDef = TypedDict(
     "LabelDetectionTypeDef",
     {
         "Timestamp": int,
         "Label": LabelTypeDef,
-        "StartTimestampMillis": int,
-        "EndTimestampMillis": int,
-        "DurationMillis": int,
     },
     total=False,
 )
 
 CelebrityRecognitionTypeDef = TypedDict(
     "CelebrityRecognitionTypeDef",
     {
```

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/waiter.py` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition/waiter.pyi` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/PKG-INFO` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.26.28
-Summary: Type annotations for boto3.Rekognition 1.26.28 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.8
+Summary: Type annotations for boto3.Rekognition 1.26.8 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,16 +366,14 @@
     DescribeProjectsPaginatorName,
     DetectLabelsFeatureNameType,
     EmotionNameType,
     FaceAttributesType,
     FaceSearchSortByType,
     GenderTypeType,
     KnownGenderTypeType,
-    LabelDetectionAggregateByType,
-    LabelDetectionFeatureNameType,
     LabelDetectionSortByType,
     LandmarkTypeType,
     ListCollectionsPaginatorName,
     ListDatasetEntriesPaginatorName,
     ListDatasetLabelsPaginatorName,
     ListFacesPaginatorName,
     ListProjectPoliciesPaginatorName,
@@ -565,15 +562,14 @@
     ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
-    LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
     RegionOfInterestTypeDef,
     GroundTruthManifestTypeDef,
```

### Comparing `mypy-boto3-rekognition-1.26.28/mypy_boto3_rekognition.egg-info/SOURCES.txt` & `mypy-boto3-rekognition-1.26.8/mypy_boto3_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.26.28/setup.py` & `mypy-boto3-rekognition-1.26.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,46 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-rekognition",
-    version="1.26.28",
+    version="1.26.8",
     packages=["mypy_boto3_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Rekognition 1.26.28 service generated with mypy-boto3-builder"
-        " 7.12.0"
+        "Type annotations for boto3.Rekognition 1.26.8 service generated with mypy-boto3-builder"
+        " 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 rekognition type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_rekognition": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_rekognition": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

