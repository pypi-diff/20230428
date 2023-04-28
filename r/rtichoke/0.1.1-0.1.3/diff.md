# Comparing `tmp/rtichoke-0.1.1-py3-none-any.whl.zip` & `tmp/rtichoke-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14878 bytes, number of entries: 23
+Zip file size: 14880 bytes, number of entries: 23
 -rw-r--r--  2.0 fat     1045 b- defN 80-Jan-01 00:00 rtichoke/__init__.py
 -rw-r--r--  2.0 fat       38 b- defN 80-Jan-01 00:00 rtichoke/calibration/__init__.py
 -rw-r--r--  2.0 fat    10705 b- defN 80-Jan-01 00:00 rtichoke/calibration/calibration.py
 -rw-r--r--  2.0 fat       41 b- defN 80-Jan-01 00:00 rtichoke/discrimination/__init__.py
 -rw-r--r--  2.0 fat     2253 b- defN 80-Jan-01 00:00 rtichoke/discrimination/gains.py
 -rw-r--r--  2.0 fat     2246 b- defN 80-Jan-01 00:00 rtichoke/discrimination/lift.py
 -rw-r--r--  2.0 fat     2330 b- defN 80-Jan-01 00:00 rtichoke/discrimination/precision_recall.py
@@ -14,12 +14,12 @@
 -rw-r--r--  2.0 fat       43 b- defN 80-Jan-01 00:00 rtichoke/performance_data/__init__.py
 -rw-r--r--  2.0 fat     1323 b- defN 80-Jan-01 00:00 rtichoke/performance_data/performance_data.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 rtichoke/rtichoke.py
 -rw-r--r--  2.0 fat       41 b- defN 80-Jan-01 00:00 rtichoke/summary_report/__init__.py
 -rw-r--r--  2.0 fat      676 b- defN 80-Jan-01 00:00 rtichoke/summary_report/summary_report.py
 -rw-r--r--  2.0 fat       42 b- defN 80-Jan-01 00:00 rtichoke/utility/__init__.py
 -rw-r--r--  2.0 fat     3293 b- defN 80-Jan-01 00:00 rtichoke/utility/decision.py
--rw-r--r--  2.0 fat     1093 b- defN 80-Jan-01 00:00 rtichoke-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 fat      755 b- defN 80-Jan-01 00:00 rtichoke-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 rtichoke-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat     2017 b- defN 16-Jan-01 00:00 rtichoke-0.1.1.dist-info/RECORD
-23 files, 46908 bytes uncompressed, 11552 bytes compressed:  75.4%
+-rw-r--r--  2.0 fat     1093 b- defN 80-Jan-01 00:00 rtichoke-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 fat      755 b- defN 80-Jan-01 00:00 rtichoke-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 rtichoke-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 fat     2017 b- defN 16-Jan-01 00:00 rtichoke-0.1.3.dist-info/RECORD
+23 files, 46908 bytes uncompressed, 11554 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: rtichoke/utility/__init__.py
 Comment: 
 
 Filename: rtichoke/utility/decision.py
 Comment: 
 
-Filename: rtichoke-0.1.1.dist-info/LICENSE
+Filename: rtichoke-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: rtichoke-0.1.1.dist-info/METADATA
+Filename: rtichoke-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: rtichoke-0.1.1.dist-info/WHEEL
+Filename: rtichoke-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: rtichoke-0.1.1.dist-info/RECORD
+Filename: rtichoke-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rtichoke-0.1.1.dist-info/LICENSE` & `rtichoke-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rtichoke-0.1.1.dist-info/METADATA` & `rtichoke-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtichoke
-Version: 0.1.1
+Version: 0.1.3
 Summary: interactive visualizations for performance of predictive models
 License: MIT
 Author: Uriah Finkel
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `rtichoke-0.1.1.dist-info/RECORD` & `rtichoke-0.1.3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 rtichoke/performance_data/__init__.py,sha256=oOA9dNxjTNCe6Rlo2HUOvSkLBLv492CjmE_98fH6yv0,43
 rtichoke/performance_data/performance_data.py,sha256=BYlv4Puercqa8Zu5MoNTNSRCPj8BJ1azNhUg9Scr4Nk,1323
 rtichoke/rtichoke.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rtichoke/summary_report/__init__.py,sha256=5_xw5Oib70-sgCNaom0i6XPlQVjUDRH8WJNUVepTMtI,41
 rtichoke/summary_report/summary_report.py,sha256=JNp4hdHjloFCmTViHXxD3c9RgzxMidjo18TNRdvkQsM,676
 rtichoke/utility/__init__.py,sha256=-s9MCY2QVeLXRgmLXhVNEassbfQDs7j5FkfHm5JWRMo,42
 rtichoke/utility/decision.py,sha256=4vqFSzjCf4iRXH2TnYzkXJXy-76wNeg2zpRv0JNlBdk,3293
-rtichoke-0.1.1.dist-info/LICENSE,sha256=0uNjYeBvVUt69zJb5Ft2d0dbx8sB5-Bqg7fkfpynQtU,1093
-rtichoke-0.1.1.dist-info/METADATA,sha256=UAZoDr93f9BgmNgVIjXA2lh2V0wbtEIHoPno_nxZ1nk,755
-rtichoke-0.1.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-rtichoke-0.1.1.dist-info/RECORD,,
+rtichoke-0.1.3.dist-info/LICENSE,sha256=0uNjYeBvVUt69zJb5Ft2d0dbx8sB5-Bqg7fkfpynQtU,1093
+rtichoke-0.1.3.dist-info/METADATA,sha256=MEScUiHExXHy9LUNLFGMQ-p-Utd2o1wob91AxoEkV4g,755
+rtichoke-0.1.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+rtichoke-0.1.3.dist-info/RECORD,,
```

