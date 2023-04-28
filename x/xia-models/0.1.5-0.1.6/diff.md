# Comparing `tmp/xia_models-0.1.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_models-0.1.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 335180 bytes, number of entries: 8
--rw-r--r--  2.0 unx      239 b- defN 23-Apr-01 09:57 xia_models/__init__.py
--rw-r--r--  2.0 unx   421376 b- defN 23-Apr-01 12:30 xia_models/address.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   442368 b- defN 23-Apr-01 12:29 xia_models/model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-01 12:30 xia_models-0.1.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      638 b- defN 23-Apr-01 12:30 xia_models-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-01 12:30 xia_models-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-01 12:30 xia_models-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      671 b- defN 23-Apr-01 12:30 xia_models-0.1.5.dist-info/RECORD
-8 files, 865554 bytes uncompressed, 334006 bytes compressed:  61.4%
+Zip file size: 335251 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      239 b- defN 23-Apr-28 10:45 xia_models/__init__.py
+-rw-r--r--  2.0 unx   421376 b- defN 23-Apr-28 10:49 xia_models/address.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   442368 b- defN 23-Apr-28 10:48 xia_models/model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-28 10:49 xia_models-0.1.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      638 b- defN 23-Apr-28 10:49 xia_models-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-28 10:49 xia_models-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-28 10:49 xia_models-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      671 b- defN 23-Apr-28 10:49 xia_models-0.1.6.dist-info/RECORD
+8 files, 865554 bytes uncompressed, 334077 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: xia_models/address.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_models/model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_models-0.1.5.dist-info/LICENSE.txt
+Filename: xia_models-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_models-0.1.5.dist-info/METADATA
+Filename: xia_models-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_models-0.1.5.dist-info/WHEEL
+Filename: xia_models-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_models-0.1.5.dist-info/top_level.txt
+Filename: xia_models-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_models-0.1.5.dist-info/RECORD
+Filename: xia_models-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_models/__init__.py

```diff
@@ -2,8 +2,8 @@
 from xia_models.address import DataAddress, TableAddress, TableCatalog
 
 __all__ = [
     "DataModel", "DataField",
     "DataAddress", "TableAddress", "TableCatalog"
 ]
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

## Comparing `xia_models-0.1.5.dist-info/METADATA` & `xia_models-0.1.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-models
-Version: 0.1.5
+Version: 0.1.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-models/0.1.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-models/0.1.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

