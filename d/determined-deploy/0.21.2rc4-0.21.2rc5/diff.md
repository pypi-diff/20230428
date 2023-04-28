# Comparing `tmp/determined_deploy-0.21.2rc4-py3-none-any.whl.zip` & `tmp/determined_deploy-0.21.2rc5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1814 bytes, number of entries: 6
--rw-r--r--  2.0 unx      235 b- defN 23-Apr-26 23:08 determined_deploy/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-26 23:08 determined_deploy/__version__.py
--rw-r--r--  2.0 unx      417 b- defN 23-Apr-26 23:08 determined_deploy-0.21.2rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 23:08 determined_deploy-0.21.2rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-26 23:08 determined_deploy-0.21.2rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-26 23:08 determined_deploy-0.21.2rc4.dist-info/RECORD
-6 files, 1314 bytes uncompressed, 846 bytes compressed:  35.6%
+Zip file size: 1818 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      235 b- defN 23-Apr-28 15:46 determined_deploy/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-28 15:46 determined_deploy/__version__.py
+-rw-r--r--  2.0 unx      417 b- defN 23-Apr-28 15:46 determined_deploy-0.21.2rc5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 15:46 determined_deploy-0.21.2rc5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-28 15:46 determined_deploy-0.21.2rc5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-28 15:46 determined_deploy-0.21.2rc5.dist-info/RECORD
+6 files, 1314 bytes uncompressed, 850 bytes compressed:  35.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_deploy/__init__.py
 Comment: 
 
 Filename: determined_deploy/__version__.py
 Comment: 
 
-Filename: determined_deploy-0.21.2rc4.dist-info/METADATA
+Filename: determined_deploy-0.21.2rc5.dist-info/METADATA
 Comment: 
 
-Filename: determined_deploy-0.21.2rc4.dist-info/WHEEL
+Filename: determined_deploy-0.21.2rc5.dist-info/WHEEL
 Comment: 
 
-Filename: determined_deploy-0.21.2rc4.dist-info/top_level.txt
+Filename: determined_deploy-0.21.2rc5.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_deploy-0.21.2rc4.dist-info/RECORD
+Filename: determined_deploy-0.21.2rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_deploy/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.21.2-rc4"
+__version__ = "0.21.2-rc5"
```

## Comparing `determined_deploy-0.21.2rc4.dist-info/RECORD` & `determined_deploy-0.21.2rc5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 determined_deploy/__init__.py,sha256=e4caLmyNqYzmNjIyNmPBCVCCmZ0BPYY6K_M279HBLeA,235
-determined_deploy/__version__.py,sha256=WfvuqcX_vCTMrWPk7RT2S0LUypp1WlvQXRikTFAO8Vw,27
-determined_deploy-0.21.2rc4.dist-info/METADATA,sha256=0ksWM4XH4-Qwhq7pt7zqqsp0Rpy-IBOZ5R3YTpVHf3w,417
-determined_deploy-0.21.2rc4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-determined_deploy-0.21.2rc4.dist-info/top_level.txt,sha256=cP5FE7UPh3f1fj49mbwhot5Rs5UcGIZpFFy-tZeaPhg,18
-determined_deploy-0.21.2rc4.dist-info/RECORD,,
+determined_deploy/__version__.py,sha256=2mA1rpBqVN_PNNg9JEyGVTQSrGLSziiA6qrd0nniigo,27
+determined_deploy-0.21.2rc5.dist-info/METADATA,sha256=7qW_UkXKFvX3MyHhX7dQUiSb8lVPjruEHnL3voT93Ss,417
+determined_deploy-0.21.2rc5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+determined_deploy-0.21.2rc5.dist-info/top_level.txt,sha256=cP5FE7UPh3f1fj49mbwhot5Rs5UcGIZpFFy-tZeaPhg,18
+determined_deploy-0.21.2rc5.dist-info/RECORD,,
```

