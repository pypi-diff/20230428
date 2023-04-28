# Comparing `tmp/pyfreefem-1.0.2-py3-none-any.whl.zip` & `tmp/pyfreefem-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 27977 bytes, number of entries: 9
+Zip file size: 27975 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      800 b- defN 23-Jan-30 15:19 pyfreefem/__init__.py
 -rw-r--r--  2.0 unx    13599 b- defN 23-Apr-28 07:23 pyfreefem/freefemrunner.py
 -rw-r--r--  2.0 unx     8245 b- defN 23-Apr-28 07:23 pyfreefem/io.py
 -rw-r--r--  2.0 unx    21163 b- defN 23-Apr-28 07:23 pyfreefem/preprocessor.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Apr-28 11:33 pyfreefem-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4178 b- defN 23-Apr-28 11:33 pyfreefem-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 11:33 pyfreefem-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 11:33 pyfreefem-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      713 b- defN 23-Apr-28 11:33 pyfreefem-1.0.2.dist-info/RECORD
-9 files, 83949 bytes uncompressed, 26759 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4178 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      713 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/RECORD
+9 files, 83949 bytes uncompressed, 26757 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: pyfreefem/io.py
 Comment: 
 
 Filename: pyfreefem/preprocessor.py
 Comment: 
 
-Filename: pyfreefem-1.0.2.dist-info/LICENSE
+Filename: pyfreefem-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyfreefem-1.0.2.dist-info/METADATA
+Filename: pyfreefem-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pyfreefem-1.0.2.dist-info/WHEEL
+Filename: pyfreefem-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyfreefem-1.0.2.dist-info/top_level.txt
+Filename: pyfreefem-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyfreefem-1.0.2.dist-info/RECORD
+Filename: pyfreefem-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyfreefem-1.0.2.dist-info/LICENSE` & `pyfreefem-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyfreefem-1.0.2.dist-info/METADATA` & `pyfreefem-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfreefem
-Version: 1.0.2
+Version: 1.1.0
 Summary: Package PyFreeFEM for interfacing Python and FreeFEM.
 Home-page: https://pyfreefem.readthedocs.io/en/latest/
 Author: Florian Feppon
 Author-email: florian.feppon@kuleuven.be
 License: GNU GPL version 3
 Keywords: FreeFEM
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyfreefem-1.0.2.dist-info/RECORD` & `pyfreefem-1.1.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pyfreefem/__init__.py,sha256=qa8aAf6J_dHWHIKm2PnWpdLzuRYxypArNv8S2Yi4xJM,800
 pyfreefem/freefemrunner.py,sha256=oHCUUHXg-Oxv9kF1gqXhJUhALT-71L9wJhfk2fi-HvA,13599
 pyfreefem/io.py,sha256=zk2TdeU34fzvgup8CgOU3BuNCXfBqOHio9dsdD8wl8E,8245
 pyfreefem/preprocessor.py,sha256=f-0JqpqbSXyekc9FnwZyb67DYz0VPhqngjx9XYvuICI,21163
-pyfreefem-1.0.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pyfreefem-1.0.2.dist-info/METADATA,sha256=nRcFok8EqhAOsrK54a9AwOwfrQgE85nBC0h_ROtb670,4178
-pyfreefem-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pyfreefem-1.0.2.dist-info/top_level.txt,sha256=z1tUMsoAVRLY34PxrqfcgahYpPcvJdL1f59U6L_m-6w,10
-pyfreefem-1.0.2.dist-info/RECORD,,
+pyfreefem-1.1.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pyfreefem-1.1.0.dist-info/METADATA,sha256=CTGwhm2w_-gCRXoZJix5rIviqUCYNEQpjK5qyIwStxQ,4178
+pyfreefem-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pyfreefem-1.1.0.dist-info/top_level.txt,sha256=z1tUMsoAVRLY34PxrqfcgahYpPcvJdL1f59U6L_m-6w,10
+pyfreefem-1.1.0.dist-info/RECORD,,
```

