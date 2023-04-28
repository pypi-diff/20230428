# Comparing `tmp/mo_json-6.370.23104-py2.py3-none-any.whl.zip` & `tmp/mo_json-6.371.23118-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 30545 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat    13208 b- defN 23-Apr-14 10:26 mo_json/__init__.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-14 10:26 mo_json/decoder.py
 -rw-rw-rw-  2.0 fat    15429 b- defN 23-Apr-14 10:26 mo_json/encoder.py
 -rw-rw-rw-  2.0 fat    16185 b- defN 23-Apr-14 10:26 mo_json/stream.py
 -rw-rw-rw-  2.0 fat    17916 b- defN 23-Apr-14 10:26 mo_json/typed_encoder.py
 -rw-rw-rw-  2.0 fat     9865 b- defN 23-Apr-14 10:26 mo_json/types.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11641 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      875 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11641 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      875 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/RECORD
 11 files, 102275 bytes uncompressed, 29085 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mo_json/typed_encoder.py
 Comment: 
 
 Filename: mo_json/types.py
 Comment: 
 
-Filename: mo_json-6.370.23104.dist-info/LICENSE
+Filename: mo_json-6.371.23118.dist-info/LICENSE
 Comment: 
 
-Filename: mo_json-6.370.23104.dist-info/METADATA
+Filename: mo_json-6.371.23118.dist-info/METADATA
 Comment: 
 
-Filename: mo_json-6.370.23104.dist-info/WHEEL
+Filename: mo_json-6.371.23118.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json-6.370.23104.dist-info/top_level.txt
+Filename: mo_json-6.371.23118.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json-6.370.23104.dist-info/RECORD
+Filename: mo_json-6.371.23118.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mo_json-6.370.23104.dist-info/LICENSE` & `mo_json-6.371.23118.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_json-6.370.23104.dist-info/METADATA` & `mo_json-6.371.23118.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.370.23104
+Version: 6.371.23118
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -15,16 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
 Requires-Dist: mo-dots (==9.368.23092)
 Requires-Dist: mo-future (==7.340.23006)
-Requires-Dist: mo-logs (==7.368.23092)
-Requires-Dist: mo-times (==5.368.23092)
+Requires-Dist: mo-logs (==7.371.23118)
+Requires-Dist: mo-times (==5.371.23118)
 Provides-Extra: tests
 Requires-Dist: pyLibrary ; extra == 'tests'
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 
 # More JSON Tools
```

