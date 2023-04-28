# Comparing `tmp/encoded_core-0.0.0.1b0.tar.gz` & `tmp/encoded_core-0.0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoded_core-0.0.0.1b0.tar", max compression
+gzip compressed data, was "encoded_core-0.0.0.1b1.tar", max compression
```

## Comparing `encoded_core-0.0.0.1b0.tar` & `encoded_core-0.0.0.1b1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.0.1b0/LICENSE
--rw-r--r--   0        0        0      174 2023-04-28 13:50:12.674541 encoded_core-0.0.0.1b0/README.rst
--rw-r--r--   0        0        0     3091 2023-04-28 15:28:22.722166 encoded_core-0.0.0.1b0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-28 13:50:12.698338 encoded_core-0.0.0.1b0/src/encoded-core/__init__.py
--rw-r--r--   0        0        0     1915 2023-04-28 13:50:12.708994 encoded_core-0.0.0.1b0/src/encoded-core/schemas/document.json
--rw-r--r--   0        0        0    18553 2023-04-28 13:50:12.704726 encoded_core-0.0.0.1b0/src/encoded-core/schemas/file.json
--rw-r--r--   0        0        0     5070 2023-04-28 13:50:12.701442 encoded_core-0.0.0.1b0/src/encoded-core/schemas/file_format.json
--rw-r--r--   0        0        0     6170 2023-04-28 13:50:12.706416 encoded_core-0.0.0.1b0/src/encoded-core/schemas/file_processed.json
--rw-r--r--   0        0        0     2336 2023-04-28 13:50:12.710774 encoded_core-0.0.0.1b0/src/encoded-core/schemas/file_reference.json
--rw-r--r--   0        0        0     1331 2023-04-28 13:50:12.712368 encoded_core-0.0.0.1b0/src/encoded-core/schemas/file_submitted.json
--rw-r--r--   0        0        0     1831 2023-04-28 13:50:12.715563 encoded_core-0.0.0.1b0/src/encoded-core/schemas/higlass_view_config.json
--rw-r--r--   0        0        0     1528 2023-04-28 13:50:12.714806 encoded_core-0.0.0.1b0/src/encoded-core/schemas/image.json
--rw-r--r--   0        0        0    18352 2023-04-28 13:50:12.707283 encoded_core-0.0.0.1b0/src/encoded-core/schemas/meta_workflow.json
--rw-r--r--   0        0        0    14409 2023-04-28 13:50:12.713194 encoded_core-0.0.0.1b0/src/encoded-core/schemas/meta_workflow_run.json
--rw-r--r--   0        0        0    17295 2023-04-28 13:50:12.702288 encoded_core-0.0.0.1b0/src/encoded-core/schemas/mixins.json
--rw-r--r--   0        0        0     4581 2023-04-28 13:50:12.716243 encoded_core-0.0.0.1b0/src/encoded-core/schemas/page.json
--rw-r--r--   0        0        0     1457 2023-04-28 13:50:12.709844 encoded_core-0.0.0.1b0/src/encoded-core/schemas/quality_metric.json
--rw-r--r--   0        0        0     5715 2023-04-28 13:50:12.713992 encoded_core-0.0.0.1b0/src/encoded-core/schemas/software.json
--rw-r--r--   0        0        0     5010 2023-04-28 13:50:12.708092 encoded_core-0.0.0.1b0/src/encoded-core/schemas/static_section.json
--rw-r--r--   0        0        0    20411 2023-04-28 13:50:12.700669 encoded_core-0.0.0.1b0/src/encoded-core/schemas/tracking_item.json
--rw-r--r--   0        0        0     3749 2023-04-28 13:50:12.703052 encoded_core-0.0.0.1b0/src/encoded-core/schemas/user_content.json
--rw-r--r--   0        0        0    28267 2023-04-28 13:50:12.699926 encoded_core-0.0.0.1b0/src/encoded-core/schemas/workflow.json
--rw-r--r--   0        0        0    10502 2023-04-28 13:50:12.711544 encoded_core-0.0.0.1b0/src/encoded-core/schemas/workflow_run.json
--rw-r--r--   0        0        0     1908 2023-04-28 13:50:12.703919 encoded_core-0.0.0.1b0/src/encoded-core/schemas/workflow_run_awsem.json
--rw-r--r--   0        0        0       70 2023-04-28 13:50:12.688855 encoded_core-0.0.0.1b0/src/encoded-core/types/__init__.py
--rw-r--r--   0        0        0     1290 2023-04-28 13:50:12.692749 encoded_core-0.0.0.1b0/src/encoded-core/types/document.py
--rw-r--r--   0        0        0    41353 2023-04-28 13:50:12.690559 encoded_core-0.0.0.1b0/src/encoded-core/types/file.py
--rw-r--r--   0        0        0      870 2023-04-28 13:50:12.692030 encoded_core-0.0.0.1b0/src/encoded-core/types/file_format.py
--rw-r--r--   0        0        0     2352 2023-04-28 13:50:12.696184 encoded_core-0.0.0.1b0/src/encoded-core/types/file_processed.py
--rw-r--r--   0        0        0      517 2023-04-28 13:50:12.693465 encoded_core-0.0.0.1b0/src/encoded-core/types/file_reference.py
--rw-r--r--   0        0        0     2025 2023-04-28 13:50:12.691291 encoded_core-0.0.0.1b0/src/encoded-core/types/file_submitted.py
--rw-r--r--   0        0        0      607 2023-04-28 13:50:12.697483 encoded_core-0.0.0.1b0/src/encoded-core/types/higlass_view_config.py
--rw-r--r--   0        0        0     1046 2023-04-28 13:50:12.695219 encoded_core-0.0.0.1b0/src/encoded-core/types/image.py
--rw-r--r--   0        0        0     3191 2023-04-28 13:50:12.689732 encoded_core-0.0.0.1b0/src/encoded-core/types/meta_workflow.py
--rw-r--r--   0        0        0     5428 2023-04-28 13:50:12.687023 encoded_core-0.0.0.1b0/src/encoded-core/types/quality_metric.py
--rw-r--r--   0        0        0     2745 2023-04-28 13:50:12.696837 encoded_core-0.0.0.1b0/src/encoded-core/types/software.py
--rw-r--r--   0        0        0     3895 2023-04-28 13:50:12.687755 encoded_core-0.0.0.1b0/src/encoded-core/types/tracking_item.py
--rw-r--r--   0        0        0     5458 2023-04-28 13:50:12.686230 encoded_core-0.0.0.1b0/src/encoded-core/types/user_content.py
--rw-r--r--   0        0        0    12871 2023-04-28 13:50:12.694432 encoded_core-0.0.0.1b0/src/encoded-core/types/workflow.py
--rw-r--r--   0        0        0     1948 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b0/setup.py
--rw-r--r--   0        0        0     2576 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.0.1b1/LICENSE
+-rw-r--r--   0        0        0      174 2023-04-28 13:50:12.674541 encoded_core-0.0.0.1b1/README.rst
+-rw-r--r--   0        0        0     3092 2023-04-28 15:30:08.225982 encoded_core-0.0.0.1b1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-28 13:50:12.698338 encoded_core-0.0.0.1b1/src/encoded-core/__init__.py
+-rw-r--r--   0        0        0     1915 2023-04-28 13:50:12.708994 encoded_core-0.0.0.1b1/src/encoded-core/schemas/document.json
+-rw-r--r--   0        0        0    18553 2023-04-28 13:50:12.704726 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file.json
+-rw-r--r--   0        0        0     5070 2023-04-28 13:50:12.701442 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_format.json
+-rw-r--r--   0        0        0     6170 2023-04-28 13:50:12.706416 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_processed.json
+-rw-r--r--   0        0        0     2336 2023-04-28 13:50:12.710774 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_reference.json
+-rw-r--r--   0        0        0     1331 2023-04-28 13:50:12.712368 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_submitted.json
+-rw-r--r--   0        0        0     1831 2023-04-28 13:50:12.715563 encoded_core-0.0.0.1b1/src/encoded-core/schemas/higlass_view_config.json
+-rw-r--r--   0        0        0     1528 2023-04-28 13:50:12.714806 encoded_core-0.0.0.1b1/src/encoded-core/schemas/image.json
+-rw-r--r--   0        0        0    18352 2023-04-28 13:50:12.707283 encoded_core-0.0.0.1b1/src/encoded-core/schemas/meta_workflow.json
+-rw-r--r--   0        0        0    14409 2023-04-28 13:50:12.713194 encoded_core-0.0.0.1b1/src/encoded-core/schemas/meta_workflow_run.json
+-rw-r--r--   0        0        0    17295 2023-04-28 13:50:12.702288 encoded_core-0.0.0.1b1/src/encoded-core/schemas/mixins.json
+-rw-r--r--   0        0        0     4581 2023-04-28 13:50:12.716243 encoded_core-0.0.0.1b1/src/encoded-core/schemas/page.json
+-rw-r--r--   0        0        0     1457 2023-04-28 13:50:12.709844 encoded_core-0.0.0.1b1/src/encoded-core/schemas/quality_metric.json
+-rw-r--r--   0        0        0     5715 2023-04-28 13:50:12.713992 encoded_core-0.0.0.1b1/src/encoded-core/schemas/software.json
+-rw-r--r--   0        0        0     5010 2023-04-28 13:50:12.708092 encoded_core-0.0.0.1b1/src/encoded-core/schemas/static_section.json
+-rw-r--r--   0        0        0    20411 2023-04-28 13:50:12.700669 encoded_core-0.0.0.1b1/src/encoded-core/schemas/tracking_item.json
+-rw-r--r--   0        0        0     3749 2023-04-28 13:50:12.703052 encoded_core-0.0.0.1b1/src/encoded-core/schemas/user_content.json
+-rw-r--r--   0        0        0    28267 2023-04-28 13:50:12.699926 encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow.json
+-rw-r--r--   0        0        0    10502 2023-04-28 13:50:12.711544 encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow_run.json
+-rw-r--r--   0        0        0     1908 2023-04-28 13:50:12.703919 encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow_run_awsem.json
+-rw-r--r--   0        0        0       70 2023-04-28 13:50:12.688855 encoded_core-0.0.0.1b1/src/encoded-core/types/__init__.py
+-rw-r--r--   0        0        0     1290 2023-04-28 13:50:12.692749 encoded_core-0.0.0.1b1/src/encoded-core/types/document.py
+-rw-r--r--   0        0        0    41353 2023-04-28 13:50:12.690559 encoded_core-0.0.0.1b1/src/encoded-core/types/file.py
+-rw-r--r--   0        0        0      870 2023-04-28 13:50:12.692030 encoded_core-0.0.0.1b1/src/encoded-core/types/file_format.py
+-rw-r--r--   0        0        0     2352 2023-04-28 13:50:12.696184 encoded_core-0.0.0.1b1/src/encoded-core/types/file_processed.py
+-rw-r--r--   0        0        0      517 2023-04-28 13:50:12.693465 encoded_core-0.0.0.1b1/src/encoded-core/types/file_reference.py
+-rw-r--r--   0        0        0     2025 2023-04-28 13:50:12.691291 encoded_core-0.0.0.1b1/src/encoded-core/types/file_submitted.py
+-rw-r--r--   0        0        0      607 2023-04-28 13:50:12.697483 encoded_core-0.0.0.1b1/src/encoded-core/types/higlass_view_config.py
+-rw-r--r--   0        0        0     1046 2023-04-28 13:50:12.695219 encoded_core-0.0.0.1b1/src/encoded-core/types/image.py
+-rw-r--r--   0        0        0     3191 2023-04-28 13:50:12.689732 encoded_core-0.0.0.1b1/src/encoded-core/types/meta_workflow.py
+-rw-r--r--   0        0        0     5428 2023-04-28 13:50:12.687023 encoded_core-0.0.0.1b1/src/encoded-core/types/quality_metric.py
+-rw-r--r--   0        0        0     2745 2023-04-28 13:50:12.696837 encoded_core-0.0.0.1b1/src/encoded-core/types/software.py
+-rw-r--r--   0        0        0     3895 2023-04-28 13:50:12.687755 encoded_core-0.0.0.1b1/src/encoded-core/types/tracking_item.py
+-rw-r--r--   0        0        0     5458 2023-04-28 13:50:12.686230 encoded_core-0.0.0.1b1/src/encoded-core/types/user_content.py
+-rw-r--r--   0        0        0    12871 2023-04-28 13:50:12.694432 encoded_core-0.0.0.1b1/src/encoded-core/types/workflow.py
+-rw-r--r--   0        0        0     1957 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b1/setup.py
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b1/PKG-INFO
```

### Comparing `encoded_core-0.0.0.1b0/LICENSE` & `encoded_core-0.0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/pyproject.toml` & `encoded_core-0.0.0.1b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encoded-core"
-version = "0.0.0.1b0"  # to become 0.0.1
+version = "0.0.0.1b1"  # to become 0.0.1
 description = "Core data models for Park Lab ENCODE based projects"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/smaht-dac/encoded-core"
 repository = "https://github.com/smaht-dac/encoded-core"
 documentation = "https://github.com/smaht-dac/encoded-core"
@@ -34,15 +34,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 awscli = ">=1.25.36"
 boto3 = "^1.24.36"
 botocore = "^1.27.36"
-dcicsnovault = "8.0.1.0b0"
+dcicsnovault = "^8.0.1.0b1"
 dcicutils = "^7.0.0"
 elasticsearch = "7.13.4"
 jsonschema_serialize_fork = "^2.1.1"
 plaster-pastedeploy = "0.6"
 psycopg2-binary = "^2.9.3"
 PyJWT = "^2.6.0"
 pyramid = "1.10.4"
```

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/document.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/document.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/file.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/file_format.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_format.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/file_processed.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_processed.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/file_reference.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_reference.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/file_submitted.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_submitted.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/higlass_view_config.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/higlass_view_config.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/image.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/image.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/meta_workflow.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/meta_workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/meta_workflow_run.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/meta_workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/mixins.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/page.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/page.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/quality_metric.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/quality_metric.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/software.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/software.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/static_section.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/static_section.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/tracking_item.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/tracking_item.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/user_content.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/user_content.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/workflow.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/workflow_run.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/schemas/workflow_run_awsem.json` & `encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow_run_awsem.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/document.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/document.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/file.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/file.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/file_format.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/file_format.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/file_processed.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/file_processed.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/file_reference.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/file_reference.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/file_submitted.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/file_submitted.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/higlass_view_config.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/higlass_view_config.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/image.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/image.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/meta_workflow.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/meta_workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/quality_metric.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/quality_metric.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/software.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/software.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/tracking_item.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/tracking_item.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/user_content.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/user_content.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/src/encoded-core/types/workflow.py` & `encoded_core-0.0.0.1b1/src/encoded-core/types/workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b0/setup.py` & `encoded_core-0.0.0.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'SQLAlchemy==1.4.41',
  'WSGIProxy2==0.4.2',
  'WebOb>=1.8.7,<2.0.0',
  'WebTest>=2.0.35,<3.0.0',
  'awscli>=1.25.36',
  'boto3>=1.24.36,<2.0.0',
  'botocore>=1.27.36,<2.0.0',
- 'dcicsnovault==8.0.1.0b0',
+ 'dcicsnovault>=8.0.1.0b1,<9.0.0.0',
  'dcicutils>=7.0.0,<8.0.0',
  'elasticsearch==7.13.4',
  'jsonschema_serialize_fork>=2.1.1,<3.0.0',
  'plaster-pastedeploy==0.6',
  'psycopg2-binary>=2.9.3,<3.0.0',
  'pyramid-multiauth>=0.9.0,<1',
  'pyramid-retry>=1.0,<2.0',
@@ -45,15 +45,15 @@
  'waitress>=2.1.1,<3.0.0',
  'zope.deprecation>=4.4.0,<5.0.0',
  'zope.interface>=4.7.2,<5.0.0',
  'zope.sqlalchemy==1.6']
 
 setup_kwargs = {
     'name': 'encoded-core',
-    'version': '0.0.0.1b0',
+    'version': '0.0.0.1b1',
     'description': 'Core data models for Park Lab ENCODE based projects',
     'long_description': '============\nencoded-core\n============\n\n\nWelcome to ``encoded-core``!\n\nThis library contains common data models used across ENCODE style projects\nimplemented by the Park Lab.',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smaht-dac/encoded-core',
```

### Comparing `encoded_core-0.0.0.1b0/PKG-INFO` & `encoded_core-0.0.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded-core
-Version: 0.0.0.1b0
+Version: 0.0.0.1b1
 Summary: Core data models for Park Lab ENCODE based projects
 Home-page: https://github.com/smaht-dac/encoded-core
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 3 - Alpha
@@ -22,15 +22,15 @@
 Requires-Dist: SQLAlchemy (==1.4.41)
 Requires-Dist: WSGIProxy2 (==0.4.2)
 Requires-Dist: WebOb (>=1.8.7,<2.0.0)
 Requires-Dist: WebTest (>=2.0.35,<3.0.0)
 Requires-Dist: awscli (>=1.25.36)
 Requires-Dist: boto3 (>=1.24.36,<2.0.0)
 Requires-Dist: botocore (>=1.27.36,<2.0.0)
-Requires-Dist: dcicsnovault (==8.0.1.0b0)
+Requires-Dist: dcicsnovault (>=8.0.1.0b1,<9.0.0.0)
 Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: jsonschema_serialize_fork (>=2.1.1,<3.0.0)
 Requires-Dist: plaster-pastedeploy (==0.6)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: pyramid (==1.10.4)
 Requires-Dist: pyramid-multiauth (>=0.9.0,<1)
```

