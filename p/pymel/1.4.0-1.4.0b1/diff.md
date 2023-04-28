# Comparing `tmp/pymel-1.4.0-py2.py3-none-any.whl.zip` & `tmp/pymel-1.4.0b1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9855601 bytes, number of entries: 158
--rw-r--r--  2.0 unx     1327 b- defN 80-Jan-01 00:00 pymel/__init__.py
+Zip file size: 9855622 bytes, number of entries: 158
+-rw-r--r--  2.0 unx     1329 b- defN 80-Jan-01 00:00 pymel/__init__.py
 -rw-r--r--  2.0 unx     1584 b- defN 80-Jan-01 00:00 pymel/all.py
 -rw-r--r--  2.0 unx      451 b- defN 80-Jan-01 00:00 pymel/all.pyi
 -rw-r--r--  2.0 unx      232 b- defN 80-Jan-01 00:00 pymel/api/__init__.py
 -rw-r--r--  2.0 unx    35358 b- defN 80-Jan-01 00:00 pymel/api/allapi.py
 -rw-r--r--  2.0 unx    48028 b- defN 80-Jan-01 00:00 pymel/api/plugins.py
 -rw-r--r--  2.0 unx  6515586 b- defN 80-Jan-01 00:00 pymel/cache/mayaApi2020.py
 -rw-r--r--  2.0 unx  6486201 b- defN 80-Jan-01 00:00 pymel/cache/mayaApi2022.py
@@ -148,13 +148,13 @@
 -rw-r--r--  2.0 unx     1769 b- defN 80-Jan-01 00:00 pymel/util/testing.pyi
 -rw-r--r--  2.0 unx    71741 b- defN 80-Jan-01 00:00 pymel/util/trees.py
 -rw-r--r--  2.0 unx     3266 b- defN 80-Jan-01 00:00 pymel/util/trees.pyi
 -rw-r--r--  2.0 unx    45914 b- defN 80-Jan-01 00:00 pymel/util/utilitytypes.py
 -rw-r--r--  2.0 unx     5153 b- defN 80-Jan-01 00:00 pymel/util/utilitytypes.pyi
 -rw-r--r--  2.0 unx     6606 b- defN 80-Jan-01 00:00 pymel/versions.py
 -rw-r--r--  2.0 unx     1629 b- defN 80-Jan-01 00:00 pymel/versions.pyi
--rw-r--r--  2.0 unx     1392 b- defN 80-Jan-01 00:00 pymel-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13552 b- defN 80-Jan-01 00:00 pymel-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 pymel-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 pymel-1.4.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    13114 b- defN 16-Jan-01 00:00 pymel-1.4.0.dist-info/RECORD
-158 files, 98345522 bytes uncompressed, 9835421 bytes compressed:  90.0%
+-rw-r--r--  2.0 unx     1392 b- defN 80-Jan-01 00:00 pymel-1.4.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13554 b- defN 80-Jan-01 00:00 pymel-1.4.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 pymel-1.4.0b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 pymel-1.4.0b1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    13124 b- defN 16-Jan-01 00:00 pymel-1.4.0b1.dist-info/RECORD
+158 files, 98345536 bytes uncompressed, 9835422 bytes compressed:  90.0%
```

## zipnote {}

```diff
@@ -453,23 +453,23 @@
 
 Filename: pymel/versions.py
 Comment: 
 
 Filename: pymel/versions.pyi
 Comment: 
 
-Filename: pymel-1.4.0.dist-info/LICENSE
+Filename: pymel-1.4.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: pymel-1.4.0.dist-info/METADATA
+Filename: pymel-1.4.0b1.dist-info/METADATA
 Comment: 
 
-Filename: pymel-1.4.0.dist-info/WHEEL
+Filename: pymel-1.4.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: pymel-1.4.0.dist-info/entry_points.txt
+Filename: pymel-1.4.0b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pymel-1.4.0.dist-info/RECORD
+Filename: pymel-1.4.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymel/__init__.py

```diff
@@ -26,9 +26,9 @@
 from __future__ import absolute_import
 
 from future import standard_library
 standard_library.install_aliases()
 
 __versiontuple__ = (1, 4, 0)
 __version_suffix__ = 'b1'
-__version__ = '1.4.0'.join(str(x) for x in __versiontuple__) + __version_suffix__
+__version__ = '1.4.0b1'.join(str(x) for x in __versiontuple__) + __version_suffix__
 __authors__ = ['Chad Dombrova', 'Paul Molodowitch', 'Olivier Renouard', 'Ofer Koren']
```

## Comparing `pymel-1.4.0.dist-info/LICENSE` & `pymel-1.4.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymel-1.4.0.dist-info/METADATA` & `pymel-1.4.0b1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymel
-Version: 1.4.0
+Version: 1.4.0b1
 Summary: Python in Maya Done Right
 Home-page: https://github.com/Lumapictures/pymel
 License: BSD
 Keywords: maya,mel,3d,graphics,games,VFX,CG,animation
 Author: Chad Dombrova
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
 Classifier: License :: Other/Proprietary License
```

## Comparing `pymel-1.4.0.dist-info/RECORD` & `pymel-1.4.0b1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pymel/__init__.py,sha256=tQQFvDEF-zNzc9JclQkMFOZzRT8q5x7pj8CSc3KBJcc,1327
+pymel/__init__.py,sha256=86i8CtfrmA9yLWEPdANSVwBa_gfjnYjrhEsIdXPsn3M,1329
 pymel/all.py,sha256=EXK4xopHcUEEmlYFyNJTl3fRhboBeLe0uWx09S2l3qw,1584
 pymel/all.pyi,sha256=pJbkRmZAJzqLZpQp2SJeJ7gGAbE65-_6jWtWLYvnSrA,451
 pymel/api/__init__.py,sha256=VpqcG9We2sXAddXRSKKGeDKAmYnU4d7Ue0MLm9hQLFk,232
 pymel/api/allapi.py,sha256=2HGazwmSom_gsaaVq3cEMolpqJQYBQyL8exzgWVD2Gg,35358
 pymel/api/plugins.py,sha256=FQ2BrUiUOm4CldE32ySV-uYmwI7KzeZd2wO-ctOmPf0,48028
 pymel/cache/mayaApi2020.py,sha256=tOjolWBs1UfeImoR2DRou1EN-Oa6SEKhI4Fdfni3sWU,6515586
 pymel/cache/mayaApi2022.py,sha256=kVmwfp5YxlZhFe0hrr8M_ghIPv4Pz_SoxSPmOrpxii4,6486201
@@ -147,12 +147,12 @@
 pymel/util/testing.pyi,sha256=RSm7vv6-TcXoHLSVASARdZS7s5xyhwFSKML5uYuG0i4,1769
 pymel/util/trees.py,sha256=j8Sh6mKD7S9fcROrny6F6tZmxqstm0Qv0Xg0ohljNl8,71741
 pymel/util/trees.pyi,sha256=WJxWOg_oWWj-_TnnyiTzdC3M727risTTJnbtyNFaKe4,3266
 pymel/util/utilitytypes.py,sha256=H70bWvJUQ9B-Q2uZ7zFPYW8lFK9XZOYizZf1c8AprZ4,45914
 pymel/util/utilitytypes.pyi,sha256=LTWZC3tSZaEZAA3c3ThLEZiX3ElnVva3hYApHSACwSM,5153
 pymel/versions.py,sha256=PqSrXDHOx8v4m1taImjwDH9L0_2XILMEPTHHVJGTXVg,6606
 pymel/versions.pyi,sha256=jpa1iXLg-Z5KFGFKXQ9PYsGjMICNIMtdnryvA5kTxJI,1629
-pymel-1.4.0.dist-info/LICENSE,sha256=9U5ctJHb0Yrbm8TpubcDHUKdoHXh562hWDS1CmAZto0,1392
-pymel-1.4.0.dist-info/METADATA,sha256=Ia4lDDlrespfU_8RJfVwIC-TKCBRtgR_PLfnLmyTtJc,13552
-pymel-1.4.0.dist-info/WHEEL,sha256=HaH99ouOrPevk9rpqY57z9Q0cqbngAEEM9aoS7RPGq0,92
-pymel-1.4.0.dist-info/entry_points.txt,sha256=4cD7soNKMZ8KuXjlU2o8Ofoxlx1UuQMyYlKkLyQ6hL4,50
-pymel-1.4.0.dist-info/RECORD,,
+pymel-1.4.0b1.dist-info/LICENSE,sha256=9U5ctJHb0Yrbm8TpubcDHUKdoHXh562hWDS1CmAZto0,1392
+pymel-1.4.0b1.dist-info/METADATA,sha256=Ja0KCL5EmEC_X9hFEnCjk1hIk7SaPryThZJ90lA070Y,13554
+pymel-1.4.0b1.dist-info/WHEEL,sha256=HaH99ouOrPevk9rpqY57z9Q0cqbngAEEM9aoS7RPGq0,92
+pymel-1.4.0b1.dist-info/entry_points.txt,sha256=4cD7soNKMZ8KuXjlU2o8Ofoxlx1UuQMyYlKkLyQ6hL4,50
+pymel-1.4.0b1.dist-info/RECORD,,
```

