# Comparing `tmp/xia_engine_rest-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_rest-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 142455 bytes, number of entries: 7
--rw-r--r--  2.0 unx      140 b- defN 23-Mar-25 13:47 xia_engine_rest/__init__.py
--rw-r--r--  2.0 unx   347648 b- defN 23-Mar-25 13:50 xia_engine_rest/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-25 13:50 xia_engine_rest-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      682 b- defN 23-Mar-25 13:50 xia_engine_rest-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-25 13:50 xia_engine_rest-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-25 13:50 xia_engine_rest-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      611 b- defN 23-Mar-25 13:50 xia_engine_rest-0.1.8.dist-info/RECORD
-7 files, 349348 bytes uncompressed, 141359 bytes compressed:  59.5%
+Zip file size: 142572 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      140 b- defN 23-Apr-02 11:29 xia_engine_rest/__init__.py
+-rw-r--r--  2.0 unx   348160 b- defN 23-Apr-02 11:32 xia_engine_rest/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-02 11:32 xia_engine_rest-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      682 b- defN 23-Apr-02 11:32 xia_engine_rest-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-02 11:32 xia_engine_rest-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-02 11:32 xia_engine_rest-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      611 b- defN 23-Apr-02 11:32 xia_engine_rest-0.1.9.dist-info/RECORD
+7 files, 349860 bytes uncompressed, 141476 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_rest/__init__.py
 Comment: 
 
 Filename: xia_engine_rest/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_rest-0.1.8.dist-info/LICENSE.txt
+Filename: xia_engine_rest-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_rest-0.1.8.dist-info/METADATA
+Filename: xia_engine_rest-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_rest-0.1.8.dist-info/WHEEL
+Filename: xia_engine_rest-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_rest-0.1.8.dist-info/top_level.txt
+Filename: xia_engine_rest-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_rest-0.1.8.dist-info/RECORD
+Filename: xia_engine_rest-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_rest/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_rest.engine import RestEngine, RestConnectParam
 
 
 __all__ = [
     "RestEngine", "RestConnectParam"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_engine_rest-0.1.8.dist-info/METADATA` & `xia_engine_rest-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-rest
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-rest/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-rest/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

