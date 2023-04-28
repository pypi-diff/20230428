# Comparing `tmp/vbdataset_test-0.0.0.1-py3-none-any.whl.zip` & `tmp/vbdataset_test-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,8 @@
-Zip file size: 1157 bytes, number of entries: 4
--rw-rw-rw-  2.0 fat      275 b- defN 23-Apr-28 06:19 vbdataset_test-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 06:19 vbdataset_test-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-28 06:19 vbdataset_test-0.0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      333 b- defN 23-Apr-28 06:19 vbdataset_test-0.0.0.1.dist-info/RECORD
-4 files, 710 bytes uncompressed, 503 bytes compressed:  29.2%
+Zip file size: 2333 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-28 05:36 vbdataset/__init__.py
+-rw-rw-rw-  2.0 fat     1848 b- defN 23-Apr-28 05:19 vbdataset/fetch.py
+-rw-rw-rw-  2.0 fat      275 b- defN 23-Apr-28 06:33 vbdataset_test-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 06:33 vbdataset_test-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-28 06:33 vbdataset_test-0.0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      485 b- defN 23-Apr-28 06:33 vbdataset_test-0.0.0.2.dist-info/RECORD
+6 files, 2833 bytes uncompressed, 1449 bytes compressed:  48.9%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
-Filename: vbdataset_test-0.0.0.1.dist-info/METADATA
+Filename: vbdataset/__init__.py
 Comment: 
 
-Filename: vbdataset_test-0.0.0.1.dist-info/WHEEL
+Filename: vbdataset/fetch.py
 Comment: 
 
-Filename: vbdataset_test-0.0.0.1.dist-info/top_level.txt
+Filename: vbdataset_test-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: vbdataset_test-0.0.0.1.dist-info/RECORD
+Filename: vbdataset_test-0.0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: vbdataset_test-0.0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: vbdataset_test-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

