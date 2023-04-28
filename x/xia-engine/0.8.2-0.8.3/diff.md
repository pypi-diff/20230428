# Comparing `tmp/xia_engine-0.8.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine-0.8.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 1257899 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1417 b- defN 23-Apr-27 13:35 xia_engine/__init__.py
--rw-r--r--  2.0 unx   460800 b- defN 23-Apr-27 13:41 xia_engine/acl.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   594432 b- defN 23-Apr-27 13:39 xia_engine/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   792064 b- defN 23-Apr-27 13:45 xia_engine/document.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   749056 b- defN 23-Apr-27 13:44 xia_engine/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   262144 b- defN 23-Apr-27 13:46 xia_engine/exception.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   462848 b- defN 23-Apr-27 13:42 xia_engine/fields.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-27 13:46 xia_engine-0.8.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      745 b- defN 23-Apr-27 13:46 xia_engine-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-27 13:46 xia_engine-0.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-27 13:46 xia_engine-0.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-27 13:46 xia_engine-0.8.2.dist-info/RECORD
-12 files, 3324820 bytes uncompressed, 1256133 bytes compressed:  62.2%
+Zip file size: 1258641 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1417 b- defN 23-Apr-27 15:58 xia_engine/__init__.py
+-rw-r--r--  2.0 unx   460800 b- defN 23-Apr-27 16:03 xia_engine/acl.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   594432 b- defN 23-Apr-27 16:02 xia_engine/base.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   792576 b- defN 23-Apr-27 16:08 xia_engine/document.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   749056 b- defN 23-Apr-27 16:06 xia_engine/engine.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   262144 b- defN 23-Apr-27 16:09 xia_engine/exception.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   462848 b- defN 23-Apr-27 16:05 xia_engine/fields.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-27 16:09 xia_engine-0.8.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      745 b- defN 23-Apr-27 16:09 xia_engine-0.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-27 16:09 xia_engine-0.8.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-27 16:09 xia_engine-0.8.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-27 16:09 xia_engine-0.8.3.dist-info/RECORD
+12 files, 3325332 bytes uncompressed, 1256875 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_engine/exception.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_engine/fields.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine-0.8.2.dist-info/LICENSE.txt
+Filename: xia_engine-0.8.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine-0.8.2.dist-info/METADATA
+Filename: xia_engine-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine-0.8.2.dist-info/WHEEL
+Filename: xia_engine-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine-0.8.2.dist-info/top_level.txt
+Filename: xia_engine-0.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine-0.8.2.dist-info/RECORD
+Filename: xia_engine-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine/__init__.py

```diff
@@ -20,8 +20,8 @@
     "MetaEngine", "MetaRamEngine", "MetaCache",
     "Acl", "AclItem",
     "XiaError", 'AuthorizationError', 'AuthenticationError', "OutOfScopeError",
     'NotFoundError', 'ConflictError', 'BadRequestError', "UnprocessableError",
     "ServerError"
 ]
 
-__version__ = "0.8.2"
+__version__ = "0.8.3"
```

## Comparing `xia_engine-0.8.2.dist-info/METADATA` & `xia_engine-0.8.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine
-Version: 0.8.2
+Version: 0.8.3
 Summary: X-I-A Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine/0.8.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine/0.8.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

