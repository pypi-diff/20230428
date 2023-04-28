# Comparing `tmp/kollo-1.0.0-py3-none-any.whl.zip` & `tmp/kollo-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13003 bytes, number of entries: 12
+Zip file size: 13010 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       34 b- defN 23-Jan-11 13:59 kollo/__init__.py
 -rw-rw-r--  2.0 unx      103 b- defN 23-Jan-11 10:45 kollo/__main__.py
 -rw-rw-r--  2.0 unx     2881 b- defN 23-Feb-02 13:09 kollo/cli.py
 -rw-rw-r--  2.0 unx    13083 b- defN 23-Apr-04 11:30 kollo/kollo.py
 -rw-rw-r--  2.0 unx    11602 b- defN 23-Jan-12 16:00 kollo/kollo2.py
--rwxrwxr-x  2.0 unx      112 b- defN 23-Jan-11 10:48 kollo-1.0.0.data/scripts/kollo
--rw-rw-r--  2.0 unx     1061 b- defN 23-Apr-04 11:52 kollo-1.0.0.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     5281 b- defN 23-Apr-04 11:52 kollo-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 11:52 kollo-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-04 11:52 kollo-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jan-02 12:18 kollo-1.0.0.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      908 b- defN 23-Apr-04 11:52 kollo-1.0.0.dist-info/RECORD
-12 files, 35164 bytes uncompressed, 11493 bytes compressed:  67.3%
+-rwxrwxr-x  2.0 unx      122 b- defN 23-Apr-28 09:31 kollo-1.0.1.data/scripts/kollo
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Apr-28 09:31 kollo-1.0.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     5281 b- defN 23-Apr-28 09:31 kollo-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-28 09:31 kollo-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-28 09:31 kollo-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jan-02 12:18 kollo-1.0.1.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      908 b- defN 23-Apr-28 09:31 kollo-1.0.1.dist-info/RECORD
+12 files, 35174 bytes uncompressed, 11500 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -9,29 +9,29 @@
 
 Filename: kollo/kollo.py
 Comment: 
 
 Filename: kollo/kollo2.py
 Comment: 
 
-Filename: kollo-1.0.0.data/scripts/kollo
+Filename: kollo-1.0.1.data/scripts/kollo
 Comment: 
 
-Filename: kollo-1.0.0.dist-info/LICENSE.txt
+Filename: kollo-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: kollo-1.0.0.dist-info/METADATA
+Filename: kollo-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: kollo-1.0.0.dist-info/WHEEL
+Filename: kollo-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: kollo-1.0.0.dist-info/top_level.txt
+Filename: kollo-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: kollo-1.0.0.dist-info/zip-safe
+Filename: kollo-1.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: kollo-1.0.0.dist-info/RECORD
+Filename: kollo-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `kollo-1.0.0.dist-info/LICENSE.txt` & `kollo-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `kollo-1.0.0.dist-info/METADATA` & `kollo-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kollo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extract collocations from VERT data
 Home-page: UNKNOWN
 Author: Danny McDonald
 Author-email: daniel.mcdonald@uzh.ch
 License: MIT
 Keywords: corpus,linguistics,corpora,collocation,vert
 Platform: UNKNOWN
```

