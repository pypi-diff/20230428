# Comparing `tmp/VMedNLP-0.0.1-py310-none-any.whl.zip` & `tmp/vMedNLP-1.0.0-py310-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11202 bytes, number of entries: 7
--rw-------  2.0 unx      141 b- defN 23-Apr-27 09:02 vMedNLP/__init__.pyc
--rw-------  2.0 unx    19162 b- defN 23-Apr-27 09:02 vMedNLP/medToolkit.pyc
--rw-------  2.0 unx     8743 b- defN 23-Apr-27 09:02 VMedNLP-0.0.1.dist-info/METADATA
--rw-------  2.0 unx       83 b- defN 23-Apr-27 09:02 VMedNLP-0.0.1.dist-info/WHEEL
--rw-------  2.0 unx        8 b- defN 23-Apr-27 09:02 VMedNLP-0.0.1.dist-info/top_level.txt
--rw-------  2.0 unx        1 b- defN 23-Apr-27 09:02 VMedNLP-0.0.1.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      539 b- defN 23-Apr-27 09:02 VMedNLP-0.0.1.dist-info/RECORD
-7 files, 28677 bytes uncompressed, 10244 bytes compressed:  64.3%
+Zip file size: 11206 bytes, number of entries: 7
+-rw-------  2.0 unx      141 b- defN 23-Apr-28 05:38 vMedNLP/__init__.pyc
+-rw-------  2.0 unx    19162 b- defN 23-Apr-28 05:38 vMedNLP/medToolkit.pyc
+-rw-------  2.0 unx     8756 b- defN 23-Apr-28 05:38 vMedNLP-1.0.0.dist-info/METADATA
+-rw-------  2.0 unx       83 b- defN 23-Apr-28 05:38 vMedNLP-1.0.0.dist-info/WHEEL
+-rw-------  2.0 unx        8 b- defN 23-Apr-28 05:38 vMedNLP-1.0.0.dist-info/top_level.txt
+-rw-------  2.0 unx        1 b- defN 23-Apr-28 05:38 vMedNLP-1.0.0.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      539 b- defN 23-Apr-28 05:38 vMedNLP-1.0.0.dist-info/RECORD
+7 files, 28690 bytes uncompressed, 10248 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: vMedNLP/__init__.pyc
 Comment: 
 
 Filename: vMedNLP/medToolkit.pyc
 Comment: 
 
-Filename: VMedNLP-0.0.1.dist-info/METADATA
+Filename: vMedNLP-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: VMedNLP-0.0.1.dist-info/WHEEL
+Filename: vMedNLP-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: VMedNLP-0.0.1.dist-info/top_level.txt
+Filename: vMedNLP-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: VMedNLP-0.0.1.dist-info/zip-safe
+Filename: vMedNLP-1.0.0.dist-info/zip-safe
 Comment: 
 
-Filename: VMedNLP-0.0.1.dist-info/RECORD
+Filename: vMedNLP-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vMedNLP/medToolkit.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 24 05:51:22 2023 UTC, .py size: 27067 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 da18 4664 bb69 0000  o.........Fd.i..
+00000000: 6f0d 0d0a 0000 0000 6455 4a64 ba69 0000  o.......dUJd.i..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c00 6d04 5a04 6d01 5a01  ..d.d.l.m.Z.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 5a06 6400  m.Z...d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6400 6402 6c00 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000070: 6d01 5a01 6d05 5a05 0100 6400 6403 6c08  m.Z.m.Z...d.d.l.
@@ -1135,15 +1135,15 @@
 000046e0: 7287 0000 0072 9400 0000 725a 0000 005a  r....r....rZ...Z
 000046f0: 0470 6167 655a 0973 656e 7369 7469 7665  .pageZ.sensitive
 00004700: 7228 0000 0072 3c00 0000 da04 6461 7461  r(...r<.....data
 00004710: 5a05 6172 6561 735a 0461 7265 6172 1700  Z.areasZ.arear..
 00004720: 0000 7299 0000 0072 1800 0000 7292 0000  ..r....r....r...
 00004730: 0064 0200 0073 2000 0000 0802 0601 0801  .d...s .........
 00004740: 1801 1602 0c01 0e01 0802 0a01 0801 1001  ................
-00004750: 02ff 0a02 0a03 0801 0401 7a1b 4465 6964  ..........z.Deid
+00004750: 02ff 0a02 0a02 0801 0401 7a1b 4465 6964  ..........z.Deid
 00004760: 656e 7469 6669 6361 7469 6f6e 2e72 6564  entification.red
 00004770: 6163 745f 7064 6663 0300 0000 0000 0000  act_pdfc........
 00004780: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
 00004790: 7316 0000 0064 017c 025f 0064 017c 025f  s....d.|._.d.|._
 000047a0: 0164 017c 025f 027c 0253 0029 027a a672  .d.|._.|.S.).z.r
 000047b0: 6574 7572 6e73 2061 2072 6564 6163 7465  eturns a redacte
 000047c0: 6420 6469 636f 6d20 696d 6167 6520 7769  d dicom image wi
@@ -1156,24 +1156,24 @@
 00004830: 756e 6374 696f 6e20 6163 6365 7074 7320  unction accepts 
 00004840: 6120 7369 6e67 6c65 2070 7964 6963 6f6d  a single pydicom
 00004850: 2066 696c 65da 0029 035a 0a50 6174 6965   file..).Z.Patie
 00004860: 6e74 4167 655a 0950 6174 6965 6e74 4964  ntAgeZ.PatientId
 00004870: 5a10 5061 7469 656e 7442 6972 7468 4461  Z.PatientBirthDa
 00004880: 7465 2903 7287 0000 0072 9400 0000 725a  te).r....r....rZ
 00004890: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-000048a0: 0000 7293 0000 007a 0200 0073 0800 0000  ..r....z...s....
+000048a0: 0000 7293 0000 0079 0200 0073 0800 0000  ..r....y...s....
 000048b0: 0605 0601 0601 0403 7a21 4465 6964 656e  ........z!Deiden
 000048c0: 7469 6669 6361 7469 6f6e 2e64 6569 6465  tification.deide
 000048d0: 6e74 6966 795f 6469 636f 6d4e 290a 7246  ntify_dicomN).rF
 000048e0: 0000 0072 4700 0000 7248 0000 0072 8800  ...rG...rH...r..
 000048f0: 0000 727d 0000 0072 9100 0000 7219 0000  ..r}...r....r...
 00004900: 0072 4300 0000 7292 0000 0072 9300 0000  .rC...r....r....
 00004910: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
 00004920: 1800 0000 7286 0000 0034 0200 0073 0e00  ....r....4...s..
-00004930: 0000 0800 0802 0e0a 0814 0809 0807 0c16  ................
+00004930: 0000 0800 0802 0e0a 0814 0809 0807 0c15  ................
 00004940: 7286 0000 0029 27da 0c74 7261 6e73 666f  r....)'..transfo
 00004950: 726d 6572 7372 0200 0000 7203 0000 0072  rmersr....r....r
 00004960: 0400 0000 7205 0000 0072 0600 0000 726b  ....r....r....rk
 00004970: 0000 0072 5600 0000 7268 0000 005a 0670  ...rV...rh...Z.p
 00004980: 616e 6461 73da 0270 6472 0700 0000 da08  andas..pdr......
 00004990: 7363 6973 7061 6379 5a15 7363 6973 7061  scispacyZ.scispa
 000049a0: 6379 2e61 6262 7265 7669 6174 696f 6e72  cy.abbreviationr
```

## Comparing `VMedNLP-0.0.1.dist-info/METADATA` & `vMedNLP-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: VMedNLP
-Version: 0.0.1
+Name: vMedNLP
+Version: 1.0.0
 Summary: Medical NLP Toolkit
 Author: vLife|Virtusa
 Author-email: vlife@virtusa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -23,15 +23,15 @@
 
 # vLife | Virtusa
 
 
 ## Usage
 
 ```
-import medToolkit
+from vMedNLP import medToolKit
 from medToolkit import *
 
 ```
 
 
 
 # Section 1. Diagnosis and Procedure
```

