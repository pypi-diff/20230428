# Comparing `tmp/pqam_dparamhu2021-0.1.1.tar.gz` & `tmp/pqam_dparamhu2021-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqam_dparamhu2021-0.1.1.tar", last modified: Fri Apr 28 20:33:05 2023, max compression
+gzip compressed data, was "pqam_dparamhu2021-0.1.2.tar", last modified: Fri Apr 28 21:01:30 2023, max compression
```

## Comparing `pqam_dparamhu2021-0.1.1.tar` & `pqam_dparamhu2021-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-28 20:33:05.679526 pqam_dparamhu2021-0.1.1/
--rw-r--r--   0 adam       (501) staff       (20)       37 2023-04-28 20:32:16.000000 pqam_dparamhu2021-0.1.1/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     3871 2023-04-28 20:33:05.679388 pqam_dparamhu2021-0.1.1/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     3005 2023-04-28 20:32:16.000000 pqam_dparamhu2021-0.1.1/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-28 20:33:05.673267 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/
--rw-r--r--   0 adam       (501) staff       (20)      919 2023-04-28 20:32:16.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/HEA_pred.R
--rw-r--r--   0 adam       (501) staff       (20)     1710 2023-04-28 19:43:08.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)       50 2023-04-28 20:30:30.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-28 20:33:05.679022 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/__pycache__/
--rw-r--r--   0 adam       (501) staff       (20)      221 2023-04-28 20:04:50.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 adam       (501) staff       (20)     2281 2023-04-28 20:11:42.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/__pycache__/compositionalModel.cpython-39.pyc
--rw-r--r--   0 adam       (501) staff       (20)     1868 2023-04-28 20:30:30.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/compositionalModel.py
--rw-r--r--   0 adam       (501) staff       (20)     1677 2023-04-28 20:30:30.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R
--rw-r--r--   0 adam       (501) staff       (20)     1688 2023-04-28 20:30:30.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R
--rw-r--r--   0 adam       (501) staff       (20)      158 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/elemental_features.csv
--rw-r--r--   0 adam       (501) staff       (20)    12504 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/features_gsf.Rdata
--rw-r--r--   0 adam       (501) staff       (20)    12683 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/features_surf.Rdata
--rw-r--r--   0 adam       (501) staff       (20)    16646 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/gbm-locfit.R
--rw-r--r--   0 adam       (501) staff       (20)  5181124 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/locfit_3_var_all.Rdata
--rw-r--r--   0 adam       (501) staff       (20)  1855653 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/locfit_surf_2_var_all.Rdata
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-28 20:33:05.678585 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3871 2023-04-28 20:33:05.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      822 2023-04-28 20:33:05.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-04-28 20:33:05.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)       30 2023-04-28 20:33:05.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       18 2023-04-28 20:33:05.000000 pqam_dparamhu2021-0.1.1/pqam_dparamhu2021.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)     1013 2023-04-28 20:32:24.000000 pqam_dparamhu2021-0.1.1/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-04-28 20:33:05.679567 pqam_dparamhu2021-0.1.1/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-28 21:01:30.066252 pqam_dparamhu2021-0.1.2/
+-rw-r--r--   0 adam       (501) staff       (20)       37 2023-04-28 20:32:16.000000 pqam_dparamhu2021-0.1.2/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     3871 2023-04-28 21:01:30.066113 pqam_dparamhu2021-0.1.2/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     3005 2023-04-28 20:32:16.000000 pqam_dparamhu2021-0.1.2/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-28 21:01:30.065057 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/
+-rw-r--r--   0 adam       (501) staff       (20)      976 2023-04-28 20:56:11.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/HEA_pred.R
+-rw-r--r--   0 adam       (501) staff       (20)     1710 2023-04-28 19:43:08.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)       37 2023-04-28 20:51:33.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-28 21:01:30.065895 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/__pycache__/
+-rw-r--r--   0 adam       (501) staff       (20)      206 2023-04-28 20:53:13.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 adam       (501) staff       (20)     2364 2023-04-28 20:53:13.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0 adam       (501) staff       (20)     1693 2023-04-28 20:56:11.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R
+-rw-r--r--   0 adam       (501) staff       (20)     1704 2023-04-28 20:56:11.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R
+-rw-r--r--   0 adam       (501) staff       (20)      158 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/elemental_features.csv
+-rw-r--r--   0 adam       (501) staff       (20)    12504 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/features_gsf.Rdata
+-rw-r--r--   0 adam       (501) staff       (20)    12683 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/features_surf.Rdata
+-rw-r--r--   0 adam       (501) staff       (20)    16646 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/gbm-locfit.R
+-rw-r--r--   0 adam       (501) staff       (20)  5181124 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/locfit_3_var_all.Rdata
+-rw-r--r--   0 adam       (501) staff       (20)  1855653 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/locfit_surf_2_var_all.Rdata
+-rw-r--r--   0 adam       (501) staff       (20)     1957 2023-04-28 20:50:00.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/model.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-28 21:01:30.065638 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3871 2023-04-28 21:01:29.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      796 2023-04-28 21:01:30.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-04-28 21:01:29.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)       30 2023-04-28 21:01:29.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       18 2023-04-28 21:01:29.000000 pqam_dparamhu2021-0.1.2/pqam_dparamhu2021.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)     1013 2023-04-28 21:01:23.000000 pqam_dparamhu2021-0.1.2/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-04-28 21:01:30.066291 pqam_dparamhu2021-0.1.2/setup.cfg
```

### Comparing `pqam_dparamhu2021-0.1.1/PKG-INFO` & `pqam_dparamhu2021-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqam_dparamhu2021
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyQAlloy-compatible Model for D Parameter prediction based on Hu2021
 Author-email: Adam Krajewski <ak@psu.edu>
 Project-URL: Homepage, https://github.com/amkrajewski/pqam-dparamhu2021
 Project-URL: Bug Tracker, https://github.com/amkrajewski/pqam-dparamhu2021/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pqam_dparamhu2021-0.1.1/README.md` & `pqam_dparamhu2021-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/HEA_pred.R` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/HEA_pred.R`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-HEA_pred <- function(composition = composition) {
-  source("pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R")
-  source("pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R")
-  source("pqam_dparamhu2021/gbm-locfit.R")
+HEA_pred <- function(composition = composition, path) {
+  source(paste(path,"/descriptors_gen_dev_predict_surf.R", sep = ""))
+  source(paste(path,"/descriptors_gen_dev_predict_gsf.R", sep = ""))
+  source(paste(path,"/gbm-locfit.R", sep = ""))
 
-  load("pqam_dparamhu2021/locfit_3_var_all.Rdata")
+  load(paste(path,"/locfit_3_var_all.Rdata", sep = ""))
   model_gsf <- model
-  load("pqam_dparamhu2021/locfit_surf_2_var_all.Rdata")
+  load(paste(path,"/locfit_surf_2_var_all.Rdata", sep = ""))
   model_surf <- model
 
-  descriptors.gsf <- des_gsf(comp = composition)
-  descriptors.surf <- des_surf(comp = composition)
+  descriptors.gsf <- des_gsf(comp = composition, path = path)
+  descriptors.surf <- des_surf(comp = composition, path = path)
   sel <- c(1:26, 35:38)
   descriptors.gsf <- as.matrix(descriptors.gsf[, sel])
   descriptors.surf <- as.matrix(descriptors.surf[, sel])
   pre.gsf <- predict.gbm.locfit(model_gsf, descriptors.gsf)
   pre.surf <- predict.gbm.locfit(model_surf, descriptors.surf)
   D <- pre.surf[2] / pre.gsf[2]
   result <- t(as.matrix(c(pre.gsf[2], pre.surf[2], D)))
```

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/LICENSE` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/LICENSE`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/__pycache__/compositionalModel.cpython-39.pyc` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/__pycache__/model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 28 20:11:40 2023 UTC, .py size: 1869 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,148 @@
-00000000: 610d 0d0a 0000 0000 7c28 4c64 4d07 0000  a.......|(LdM...
+00000000: 610d 0d0a 0000 0000 7831 4c64 a507 0000  a.......x1Ld....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
-00000060: 0100 6501 6405 8301 5a09 6503 6a0a 5a0a  ..e.d...Z.e.j.Z.
-00000070: 650a 6406 1900 6407 8301 0100 6503 6a0b  e.d...d.....e.j.
-00000080: 6408 1900 5a0c 6700 6409 a201 5a0d 6507  d...Z.g.d...Z.e.
-00000090: 650e 6505 6602 1900 650f 640a 9c02 640b  e.e.f...e.d...d.
-000000a0: 640c 8404 5a10 6508 650e 1900 640d 9c01  d...Z.e.e...d...
-000000b0: 640e 640f 8404 5a11 6402 5300 2910 e900  d.d...Z.d.S.)...
-000000c0: 0000 0029 01da 0769 6d70 6f72 7472 4e29  ...)...importrN)
-000000d0: 01da 0b43 6f6d 706f 7369 7469 6f6e 2902  ...Composition).
-000000e0: da05 556e 696f 6eda 044c 6973 74da 066c  ..Union..List..l
-000000f0: 6f63 6669 74da 0673 6f75 7263 657a 1d70  ocfit..sourcez.p
-00000100: 7971 616d 5f64 7061 7261 6d68 7532 3032  yqam_dparamhu202
-00000110: 312f 4845 415f 7072 6564 2e52 5a08 4845  1/HEA_pred.RZ.HE
-00000120: 415f 7072 6564 290a 5a02 5469 5a02 5a72  A_pred).Z.TiZ.Zr
-00000130: 5a02 4866 da01 565a 024e 625a 0254 615a  Z.Hf..VZ.NbZ.TaZ
-00000140: 024d 6fda 0157 5a02 5265 5a02 5275 2902  .Mo..WZ.ReZ.Ru).
-00000150: da04 636f 6d70 da06 7265 7475 726e 6301  ..comp..returnc.
-00000160: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000170: 0000 0003 0000 0073 6c00 0000 7400 8800  .......sl...t...
-00000180: 7401 7402 6602 8302 7316 4a00 6401 8301  t.t.f...s.J.d...
-00000190: 8201 7400 8800 7401 8302 7228 7402 8800  ..t...t...r(t...
-000001a0: 8301 8900 7403 6402 6403 8400 8800 6a04  ....t.d.d.....j.
-000001b0: 4400 8301 8301 7344 4a00 6404 8301 8201  D.....sDJ.d.....
-000001c0: 8700 6601 6405 6403 8408 7405 4400 8301  ..f.d.d...t.D...
-000001d0: 7d01 7406 7407 a008 7c01 a101 8301 7d02  }.t.t...|.....}.
-000001e0: 7409 7c02 8301 5300 2906 61a8 0100 000a  t.|...S.).a.....
-000001f0: 2020 2020 5072 6564 6963 7473 2074 6865      Predicts the
-00000200: 2047 5346 2c20 5375 7264 2c20 616e 6420   GSF, Surd, and 
-00000210: 7265 7375 6c74 696e 6720 4420 7061 7261  resulting D para
-00000220: 6d65 7465 7220 666f 7220 6120 6769 7665  meter for a give
-00000230: 6e20 4845 4120 636f 6d70 6f73 6974 696f  n HEA compositio
-00000240: 6e20 696e 2074 6865 0a20 2020 2063 6f6d  n in the.    com
-00000250: 706f 7369 7469 6f6e 2073 7061 6365 206f  position space o
-00000260: 6620 2854 692c 5a72 2c48 662c 562c 4e62  f (Ti,Zr,Hf,V,Nb
-00000270: 2c54 612c 4d6f 2c57 2c52 652c 5275 2920  ,Ta,Mo,W,Re,Ru) 
-00000280: 6261 7365 6420 6f6e 2048 7527 7320 3230  based on Hu's 20
-00000290: 3231 206d 6f64 656c 2028 3130 2e31 3031  21 model (10.101
-000002a0: 362f 6a2e 6163 7461 6d61 742e 3230 3231  6/j.actamat.2021
-000002b0: 2e31 3136 3830 3029 2e0a 0a20 2020 2041  .116800)...    A
-000002c0: 7267 733a 0a20 2020 2020 2020 2063 6f6d  rgs:.        com
-000002d0: 703a 2041 2063 6f6d 706f 7369 7469 6f6e  p: A composition
-000002e0: 2073 7472 696e 6720 7768 6963 6820 7769   string which wi
-000002f0: 6c6c 2062 6520 6361 7374 2069 6e74 6f20  ll be cast into 
-00000300: 7079 6d61 7467 656e 2043 6f6d 706f 7369  pymatgen Composi
-00000310: 7469 6f6e 206f 626a 6563 7420 6f72 2072  tion object or r
-00000320: 6561 6479 2043 6f6d 706f 7369 7469 6f6e  eady Composition
-00000330: 206f 626a 6563 742e 0a0a 2020 2020 5265   object...    Re
-00000340: 7475 726e 733a 0a20 2020 2020 2020 2041  turns:.        A
-00000350: 2066 6c6f 6174 206c 6973 7420 7265 7072   float list repr
-00000360: 6573 656e 7469 6e67 2074 6865 2070 7265  esenting the pre
-00000370: 6469 6374 6564 2047 5346 2c20 5375 7264  dicted GSF, Surd
-00000380: 2c20 616e 6420 4420 7061 7261 6d65 7465  , and D paramete
-00000390: 722e 0a20 2020 207a 3763 6f6d 7020 6d75  r..    z7comp mu
-000003a0: 7374 2062 6520 6120 7374 7269 6e67 206f  st be a string o
-000003b0: 7220 6120 7079 6d61 7467 656e 2043 6f6d  r a pymatgen Com
-000003c0: 706f 7369 7469 6f6e 206f 626a 6563 742e  position object.
-000003d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000003e0: 0004 0000 0053 0000 0073 1600 0000 6700  .....S...s....g.
-000003f0: 7c00 5d0e 7d01 7c01 6a00 7401 7600 9102  |.].}.|.j.t.v...
-00000400: 7104 5300 a900 2902 da06 7379 6d62 6f6c  q.S...)...symbol
-00000410: da0d 656c 656d 656e 7473 5370 6163 65a9  ..elementsSpace.
-00000420: 02da 022e 30da 0165 720c 0000 0072 0c00  ....0..er....r..
-00000430: 0000 fa56 2f55 7365 7273 2f61 6461 6d2f  ...V/Users/adam/
-00000440: 5079 6368 6172 6d50 726f 6a65 6374 732f  PycharmProjects/
-00000450: 7071 616d 5f64 7061 7261 6d68 7532 3032  pqam_dparamhu202
-00000460: 312f 7079 7161 6d5f 6470 6172 616d 6875  1/pyqam_dparamhu
-00000470: 3230 3231 2f63 6f6d 706f 7369 7469 6f6e  2021/composition
-00000480: 616c 4d6f 6465 6c2e 7079 da0a 3c6c 6973  alModel.py..<lis
-00000490: 7463 6f6d 703e 2100 0000 f300 0000 007a  tcomp>!........z
-000004a0: 1b70 7265 6469 6374 2e3c 6c6f 6361 6c73  .predict.<locals
-000004b0: 3e2e 3c6c 6973 7463 6f6d 703e 7a52 5468  >.<listcomp>zRTh
-000004c0: 6520 636f 6d70 6f73 6974 696f 6e20 6d75  e composition mu
-000004d0: 7374 2062 6520 696e 2074 6865 2063 6f6d  st be in the com
-000004e0: 706f 7369 7469 6f6e 2073 7061 6365 206f  position space o
-000004f0: 6620 2854 692c 5a72 2c48 662c 562c 4e62  f (Ti,Zr,Hf,V,Nb
-00000500: 2c54 612c 4d6f 2c57 2c52 652c 5275 292e  ,Ta,Mo,W,Re,Ru).
-00000510: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000520: 0005 0000 0013 0000 0073 1600 0000 6700  .........s....g.
-00000530: 7c00 5d0e 7d01 8800 a000 7c01 a101 9102  |.].}.....|.....
-00000540: 7104 5300 720c 0000 0029 015a 1367 6574  q.S.r....).Z.get
-00000550: 5f61 746f 6d69 635f 6672 6163 7469 6f6e  _atomic_fraction
-00000560: 720f 0000 00a9 0172 0a00 0000 720c 0000  r......r....r...
-00000570: 0072 1200 0000 7213 0000 0024 0000 0072  .r....r....$...r
-00000580: 1400 0000 290a da0a 6973 696e 7374 616e  ....)...isinstan
-00000590: 6365 da03 7374 7272 0300 0000 da03 616c  ce..strr......al
-000005a0: 6cda 0865 6c65 6d65 6e74 7372 0e00 0000  l..elementsr....
-000005b0: da0b 6865 6150 7265 6446 756e 63da 0872  ..heaPredFunc..r
-000005c0: 6f62 6a65 6374 735a 0b46 6c6f 6174 5665  objectsZ.FloatVe
-000005d0: 6374 6f72 da04 6c69 7374 2903 720a 0000  ctor..list).r...
-000005e0: 005a 0863 6f6d 704c 6973 74da 0672 6573  .Z.compList..res
-000005f0: 756c 7472 0c00 0000 7215 0000 0072 1200  ultr....r....r..
-00000600: 0000 da07 7072 6564 6963 7410 0000 0073  ....predict....s
-00000610: 1600 0000 000c 1001 02ff 0402 0a01 0802  ................
-00000620: 1601 02ff 0403 1201 0e01 721e 0000 0029  ..........r....)
-00000630: 0172 0b00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000640: 0000 0000 0000 0001 0000 0043 0000 0073  ...........C...s
-00000650: 0600 0000 6401 6701 5300 2902 7a7c 0a20  ....d.g.S.).z|. 
-00000660: 2020 2052 6574 7572 6e73 2074 6865 2063     Returns the c
-00000670: 6974 6174 696f 6e20 6f66 2074 6865 206d  itation of the m
-00000680: 6f64 656c 2e0a 0a20 2020 2052 6574 7572  odel...    Retur
-00000690: 6e73 3a0a 2020 2020 2020 2020 4120 6c69  ns:.        A li
-000006a0: 7374 206f 6620 7374 7269 6e67 7320 7265  st of strings re
-000006b0: 7072 6573 656e 7469 6e67 2074 6865 2063  presenting the c
-000006c0: 6974 6174 696f 6e20 6f66 2074 6865 206d  itation of the m
-000006d0: 6f64 656c 2e0a 2020 2020 6116 0100 0059  odel..    a....Y
-000006e0: 6f6e 672d 4a69 6520 4875 2c20 4164 6974  ong-Jie Hu, Adit
-000006f0: 7961 2053 756e 6461 722c 2053 6869 6765  ya Sundar, Shige
-00000700: 6e6f 6275 204f 6761 7461 2c20 4c69 616e  nobu Ogata, Lian
-00000710: 6720 5169 2c20 5363 7265 656e 696e 6720  g Qi, Screening 
-00000720: 6f66 2067 656e 6572 616c 697a 6564 2073  of generalized s
-00000730: 7461 636b 696e 6720 6661 756c 7420 656e  tacking fault en
-00000740: 6572 6769 6573 2c20 7375 7266 6163 6520  ergies, surface 
-00000750: 656e 6572 6769 6573 2061 6e64 2069 6e74  energies and int
-00000760: 7269 6e73 6963 2064 7563 7469 6c65 2070  rinsic ductile p
-00000770: 6f74 656e 6379 206f 6620 7265 6672 6163  otency of refrac
-00000780: 746f 7279 206d 756c 7469 636f 6d70 6f6e  tory multicompon
-00000790: 656e 7420 616c 6c6f 7973 2c20 4163 7461  ent alloys, Acta
-000007a0: 204d 6174 6572 6961 6c69 612c 2056 6f6c   Materialia, Vol
-000007b0: 756d 6520 3231 302c 2032 3032 312c 2031  ume 210, 2021, 1
-000007c0: 3136 3830 302c 2068 7474 7073 3a2f 2f64  16800, https://d
-000007d0: 6f69 2e6f 7267 2f31 302e 3130 3136 2f6a  oi.org/10.1016/j
-000007e0: 2e61 6374 616d 6174 2e32 3032 312e 3131  .actamat.2021.11
-000007f0: 3638 3030 2e72 0c00 0000 720c 0000 0072  6800.r....r....r
-00000800: 0c00 0000 720c 0000 0072 1200 0000 da04  ....r....r......
-00000810: 6369 7465 2800 0000 7302 0000 0000 0772  cite(...s......r
-00000820: 1f00 0000 2912 5a16 7270 7932 2e72 6f62  ....).Z.rpy2.rob
-00000830: 6a65 6374 732e 7061 636b 6167 6573 7202  jects.packagesr.
-00000840: 0000 005a 0d72 7079 322e 726f 626a 6563  ...Z.rpy2.robjec
-00000850: 7473 721b 0000 005a 0d70 796d 6174 6765  tsr....Z.pymatge
-00000860: 6e2e 636f 7265 7203 0000 00da 0674 7970  n.corer......typ
-00000870: 696e 6772 0400 0000 7205 0000 0072 0600  ingr....r....r..
-00000880: 0000 da01 725a 0967 6c6f 6261 6c65 6e76  ....rZ.globalenv
-00000890: 721a 0000 0072 0e00 0000 7217 0000 0072  r....r....r....r
-000008a0: 1c00 0000 721e 0000 0072 1f00 0000 720c  ....r....r....r.
-000008b0: 0000 0072 0c00 0000 720c 0000 0072 1200  ...r....r....r..
-000008c0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000008d0: 7314 0000 000c 010c 010c 0110 0208 0206  s...............
-000008e0: 010c 010a 0308 0318 18                   .........
+00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6501  ..d.d.l.m.Z...e.
+00000070: 6406 8301 5a0b 6503 6a0c 5a0c 650c 6407  d...Z.e.j.Z.e.d.
+00000080: 1900 6408 8301 0100 6503 6a0d 6409 1900  ..d.....e.j.d...
+00000090: 5a0e 6700 640a a201 5a0f 6510 650a a011  Z.g.d...Z.e.e...
+000000a0: 640b a101 8301 5a12 6507 6510 6505 6602  d.....Z.e.e.e.f.
+000000b0: 1900 6513 640c 9c02 640d 640e 8404 5a14  ..e.d...d.d...Z.
+000000c0: 6508 6510 1900 640f 9c01 6410 6411 8404  e.e...d...d.d...
+000000d0: 5a15 6402 5300 2912 e900 0000 0029 01da  Z.d.S.)......)..
+000000e0: 0769 6d70 6f72 7472 4e29 01da 0b43 6f6d  .importrN)...Com
+000000f0: 706f 7369 7469 6f6e 2902 da05 556e 696f  position)...Unio
+00000100: 6eda 044c 6973 7429 01da 0972 6573 6f75  n..List)...resou
+00000110: 7263 6573 da06 6c6f 6366 6974 da06 736f  rces..locfit..so
+00000120: 7572 6365 7a1c 7071 616d 5f64 7061 7261  urcez.pqam_dpara
+00000130: 6d68 7532 3032 312f 4845 415f 7072 6564  mhu2021/HEA_pred
+00000140: 2e52 5a08 4845 415f 7072 6564 290a 5a02  .RZ.HEA_pred).Z.
+00000150: 5469 5a02 5a72 5a02 4866 da01 565a 024e  TiZ.ZrZ.Hf..VZ.N
+00000160: 625a 0254 615a 024d 6fda 0157 5a02 5265  bZ.TaZ.Mo..WZ.Re
+00000170: 5a02 5275 da11 7071 616d 5f64 7061 7261  Z.Ru..pqam_dpara
+00000180: 6d68 7532 3032 3129 02da 0463 6f6d 70da  mhu2021)...comp.
+00000190: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
+000001a0: 0000 0000 0300 0000 0400 0000 0300 0000  ................
+000001b0: 736e 0000 0074 0088 0074 0174 0266 0283  sn...t...t.t.f..
+000001c0: 0273 164a 0064 0183 0182 0174 0088 0074  .s.J.d.....t...t
+000001d0: 0183 0272 2874 0288 0083 0189 0074 0364  ...r(t.......t.d
+000001e0: 0264 0384 0088 006a 0444 0083 0183 0173  .d.....j.D.....s
+000001f0: 444a 0064 0483 0182 0187 0066 0164 0564  DJ.d.......f.d.d
+00000200: 0384 0874 0544 0083 017d 0174 0674 07a0  ...t.D...}.t.t..
+00000210: 087c 01a1 0174 0983 027d 0274 0a7c 0283  .|...t...}.t.|..
+00000220: 0153 0029 0661 a801 0000 0a20 2020 2050  .S.).a.....    P
+00000230: 7265 6469 6374 7320 7468 6520 4753 462c  redicts the GSF,
+00000240: 2053 7572 642c 2061 6e64 2072 6573 756c   Surd, and resul
+00000250: 7469 6e67 2044 2070 6172 616d 6574 6572  ting D parameter
+00000260: 2066 6f72 2061 2067 6976 656e 2048 4541   for a given HEA
+00000270: 2063 6f6d 706f 7369 7469 6f6e 2069 6e20   composition in 
+00000280: 7468 650a 2020 2020 636f 6d70 6f73 6974  the.    composit
+00000290: 696f 6e20 7370 6163 6520 6f66 2028 5469  ion space of (Ti
+000002a0: 2c5a 722c 4866 2c56 2c4e 622c 5461 2c4d  ,Zr,Hf,V,Nb,Ta,M
+000002b0: 6f2c 572c 5265 2c52 7529 2062 6173 6564  o,W,Re,Ru) based
+000002c0: 206f 6e20 4875 2773 2032 3032 3120 6d6f   on Hu's 2021 mo
+000002d0: 6465 6c20 2831 302e 3130 3136 2f6a 2e61  del (10.1016/j.a
+000002e0: 6374 616d 6174 2e32 3032 312e 3131 3638  ctamat.2021.1168
+000002f0: 3030 292e 0a0a 2020 2020 4172 6773 3a0a  00)...    Args:.
+00000300: 2020 2020 2020 2020 636f 6d70 3a20 4120          comp: A 
+00000310: 636f 6d70 6f73 6974 696f 6e20 7374 7269  composition stri
+00000320: 6e67 2077 6869 6368 2077 696c 6c20 6265  ng which will be
+00000330: 2063 6173 7420 696e 746f 2070 796d 6174   cast into pymat
+00000340: 6765 6e20 436f 6d70 6f73 6974 696f 6e20  gen Composition 
+00000350: 6f62 6a65 6374 206f 7220 7265 6164 7920  object or ready 
+00000360: 436f 6d70 6f73 6974 696f 6e20 6f62 6a65  Composition obje
+00000370: 6374 2e0a 0a20 2020 2052 6574 7572 6e73  ct...    Returns
+00000380: 3a0a 2020 2020 2020 2020 4120 666c 6f61  :.        A floa
+00000390: 7420 6c69 7374 2072 6570 7265 7365 6e74  t list represent
+000003a0: 696e 6720 7468 6520 7072 6564 6963 7465  ing the predicte
+000003b0: 6420 4753 462c 2053 7572 642c 2061 6e64  d GSF, Surd, and
+000003c0: 2044 2070 6172 616d 6574 6572 2e0a 2020   D parameter..  
+000003d0: 2020 7a37 636f 6d70 206d 7573 7420 6265    z7comp must be
+000003e0: 2061 2073 7472 696e 6720 6f72 2061 2070   a string or a p
+000003f0: 796d 6174 6765 6e20 436f 6d70 6f73 6974  ymatgen Composit
+00000400: 696f 6e20 6f62 6a65 6374 2e63 0100 0000  ion object.c....
+00000410: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000420: 5300 0000 7316 0000 0067 007c 005d 0e7d  S...s....g.|.].}
+00000430: 017c 016a 0074 0176 0091 0271 0453 00a9  .|.j.t.v...q.S..
+00000440: 0029 02da 0673 796d 626f 6cda 0d65 6c65  .)...symbol..ele
+00000450: 6d65 6e74 7353 7061 6365 a902 da02 2e30  mentsSpace.....0
+00000460: da01 6572 0e00 0000 720e 0000 00fa 482f  ..er....r.....H/
+00000470: 5573 6572 732f 6164 616d 2f50 7963 6861  Users/adam/Pycha
+00000480: 726d 5072 6f6a 6563 7473 2f70 7161 6d5f  rmProjects/pqam_
+00000490: 6470 6172 616d 6875 3230 3231 2f70 7161  dparamhu2021/pqa
+000004a0: 6d5f 6470 6172 616d 6875 3230 3231 2f6d  m_dparamhu2021/m
+000004b0: 6f64 656c 2e70 79da 0a3c 6c69 7374 636f  odel.py..<listco
+000004c0: 6d70 3e24 0000 00f3 0000 0000 7a1b 7072  mp>$........z.pr
+000004d0: 6564 6963 742e 3c6c 6f63 616c 733e 2e3c  edict.<locals>.<
+000004e0: 6c69 7374 636f 6d70 3e7a 5254 6865 2063  listcomp>zRThe c
+000004f0: 6f6d 706f 7369 7469 6f6e 206d 7573 7420  omposition must 
+00000500: 6265 2069 6e20 7468 6520 636f 6d70 6f73  be in the compos
+00000510: 6974 696f 6e20 7370 6163 6520 6f66 2028  ition space of (
+00000520: 5469 2c5a 722c 4866 2c56 2c4e 622c 5461  Ti,Zr,Hf,V,Nb,Ta
+00000530: 2c4d 6f2c 572c 5265 2c52 7529 2e63 0100  ,Mo,W,Re,Ru).c..
+00000540: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00000550: 0000 1300 0000 7316 0000 0067 007c 005d  ......s....g.|.]
+00000560: 0e7d 0188 00a0 007c 01a1 0191 0271 0453  .}.....|.....q.S
+00000570: 0072 0e00 0000 2901 5a13 6765 745f 6174  .r....).Z.get_at
+00000580: 6f6d 6963 5f66 7261 6374 696f 6e72 1100  omic_fractionr..
+00000590: 0000 a901 720c 0000 0072 0e00 0000 7214  ....r....r....r.
+000005a0: 0000 0072 1500 0000 2700 0000 7216 0000  ...r....'...r...
+000005b0: 0029 0bda 0a69 7369 6e73 7461 6e63 65da  .)...isinstance.
+000005c0: 0373 7472 7203 0000 00da 0361 6c6c da08  .strr......all..
+000005d0: 656c 656d 656e 7473 7210 0000 00da 0b68  elementsr......h
+000005e0: 6561 5072 6564 4675 6e63 da08 726f 626a  eaPredFunc..robj
+000005f0: 6563 7473 5a0b 466c 6f61 7456 6563 746f  ectsZ.FloatVecto
+00000600: 72da 0470 6174 68da 046c 6973 7429 0372  r..path..list).r
+00000610: 0c00 0000 5a08 636f 6d70 4c69 7374 da06  ....Z.compList..
+00000620: 7265 7375 6c74 720e 0000 0072 1700 0000  resultr....r....
+00000630: 7214 0000 00da 0770 7265 6469 6374 1300  r......predict..
+00000640: 0000 7316 0000 0000 0c10 0102 ff04 020a  ..s.............
+00000650: 0108 0216 0102 ff04 0312 0110 0172 2100  .............r!.
+00000660: 0000 2901 720d 0000 0063 0000 0000 0000  ..).r....c......
+00000670: 0000 0000 0000 0000 0000 0100 0000 4300  ..............C.
+00000680: 0000 7306 0000 0064 0167 0153 0029 027a  ..s....d.g.S.).z
+00000690: 7c0a 2020 2020 5265 7475 726e 7320 7468  |.    Returns th
+000006a0: 6520 6369 7461 7469 6f6e 206f 6620 7468  e citation of th
+000006b0: 6520 6d6f 6465 6c2e 0a0a 2020 2020 5265  e model...    Re
+000006c0: 7475 726e 733a 0a20 2020 2020 2020 2041  turns:.        A
+000006d0: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
+000006e0: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+000006f0: 6520 6369 7461 7469 6f6e 206f 6620 7468  e citation of th
+00000700: 6520 6d6f 6465 6c2e 0a20 2020 2061 1601  e model..    a..
+00000710: 0000 596f 6e67 2d4a 6965 2048 752c 2041  ..Yong-Jie Hu, A
+00000720: 6469 7479 6120 5375 6e64 6172 2c20 5368  ditya Sundar, Sh
+00000730: 6967 656e 6f62 7520 4f67 6174 612c 204c  igenobu Ogata, L
+00000740: 6961 6e67 2051 692c 2053 6372 6565 6e69  iang Qi, Screeni
+00000750: 6e67 206f 6620 6765 6e65 7261 6c69 7a65  ng of generalize
+00000760: 6420 7374 6163 6b69 6e67 2066 6175 6c74  d stacking fault
+00000770: 2065 6e65 7267 6965 732c 2073 7572 6661   energies, surfa
+00000780: 6365 2065 6e65 7267 6965 7320 616e 6420  ce energies and 
+00000790: 696e 7472 696e 7369 6320 6475 6374 696c  intrinsic ductil
+000007a0: 6520 706f 7465 6e63 7920 6f66 2072 6566  e potency of ref
+000007b0: 7261 6374 6f72 7920 6d75 6c74 6963 6f6d  ractory multicom
+000007c0: 706f 6e65 6e74 2061 6c6c 6f79 732c 2041  ponent alloys, A
+000007d0: 6374 6120 4d61 7465 7269 616c 6961 2c20  cta Materialia, 
+000007e0: 566f 6c75 6d65 2032 3130 2c20 3230 3231  Volume 210, 2021
+000007f0: 2c20 3131 3638 3030 2c20 6874 7470 733a  , 116800, https:
+00000800: 2f2f 646f 692e 6f72 672f 3130 2e31 3031  //doi.org/10.101
+00000810: 362f 6a2e 6163 7461 6d61 742e 3230 3231  6/j.actamat.2021
+00000820: 2e31 3136 3830 302e 720e 0000 0072 0e00  .116800.r....r..
+00000830: 0000 720e 0000 0072 0e00 0000 7214 0000  ..r....r....r...
+00000840: 00da 0463 6974 652c 0000 0073 0200 0000  ...cite,...s....
+00000850: 0007 7222 0000 0029 165a 1672 7079 322e  ..r"...).Z.rpy2.
+00000860: 726f 626a 6563 7473 2e70 6163 6b61 6765  robjects.package
+00000870: 7372 0200 0000 5a0d 7270 7932 2e72 6f62  sr....Z.rpy2.rob
+00000880: 6a65 6374 7372 1d00 0000 5a0d 7079 6d61  jectsr....Z.pyma
+00000890: 7467 656e 2e63 6f72 6572 0300 0000 da06  tgen.corer......
+000008a0: 7479 7069 6e67 7204 0000 0072 0500 0000  typingr....r....
+000008b0: da09 696d 706f 7274 6c69 6272 0600 0000  ..importlibr....
+000008c0: 7207 0000 00da 0172 5a09 676c 6f62 616c  r......rZ.global
+000008d0: 656e 7672 1c00 0000 7210 0000 0072 1900  envr....r....r..
+000008e0: 0000 da05 6669 6c65 7372 1e00 0000 721f  ....filesr....r.
+000008f0: 0000 0072 2100 0000 7222 0000 0072 0e00  ...r!...r"...r..
+00000900: 0000 720e 0000 0072 0e00 0000 7214 0000  ..r....r....r...
+00000910: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000920: 1800 0000 0c01 0c01 0c01 1001 0c03 0802  ................
+00000930: 0601 0c01 0a03 0802 0e02 1819            ............
```

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/compositionalModel.py` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from rpy2.robjects.packages import importr
 import rpy2.robjects as robjects
 from pymatgen.core import Composition
 from typing import Union, List
+from importlib import resources
+
 
 locfit = importr('locfit')
 
 r = robjects.r
 r['source']('pqam_dparamhu2021/HEA_pred.R')
 heaPredFunc = robjects.globalenv['HEA_pred']
 
 # (Ti,Zr,Hf,V,Nb,Ta,Mo,W,Re,Ru)
 elementsSpace = ['Ti', 'Zr', 'Hf', 'V', 'Nb', 'Ta', 'Mo', 'W', 'Re', 'Ru']
 
+path = str(resources.files('pqam_dparamhu2021'))
 
 def predict(comp: Union[str, Composition]) -> list:
     """
     Predicts the GSF, Surd, and resulting D parameter for a given HEA composition in the
     composition space of (Ti,Zr,Hf,V,Nb,Ta,Mo,W,Re,Ru) based on Hu's 2021 model (10.1016/j.actamat.2021.116800).
 
     Args:
@@ -30,17 +33,18 @@
     if isinstance(comp, str):
         comp = Composition(comp)
 
     assert all([e.symbol in elementsSpace for e in comp.elements]), \
         "The composition must be in the composition space of (Ti,Zr,Hf,V,Nb,Ta,Mo,W,Re,Ru)."
 
     compList = [comp.get_atomic_fraction(e) for e in elementsSpace]
-    result = heaPredFunc(robjects.FloatVector(compList))
+    result = heaPredFunc(robjects.FloatVector(compList), path)
     return list(result)
 
+
 def cite() -> List[str]:
     """
     Returns the citation of the model.
 
     Returns:
         A list of strings representing the citation of the model.
     """
```

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-des_gsf <- function(comp = comp) {
+des_gsf <- function(comp = comp, path) {
   comp_n <- comp / sum(comp)
   a <- c(1, 1, 1, 1, 1, 1, 1, 1, 1, 1)
   data.1 <- data.frame(rbind(a, comp_n))
 
-  file.3 <- "pqam_dparamhu2021/elemental_features.csv"
+  file.3 <- paste(path,"/elemental_features.csv", sep = "")
   data.3 <- read.csv(file = file.3, header = T)
   para_ele <- as.matrix(data.3[, 2:4])
 
-  load(file = "pqam_dparamhu2021/features_gsf.Rdata")
+  load(file = paste(path,"/features_gsf.Rdata", sep = ""))
 
   feature.gsf.select <- feature.gsf.all
   n.ob <- length(data.1[, 1])
   n.feature <- length(feature.gsf.select[1, 1,])
   n.feature.ele <- length(para_ele[1,])
   n.feature.all <- n.feature + n.feature.ele
```

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-des_surf <- function(comp = comp) {
+des_surf <- function(comp = comp, path) {
   comp_n <- comp / sum(comp)
   a <- c(1, 1, 1, 1, 1, 1, 1, 1, 1, 1)
   data.1 <- data.frame(rbind(a, comp_n))
 
-  file.3 <- "pqam_dparamhu2021/elemental_features.csv"
+  file.3 <- paste(path,"/elemental_features.csv", sep = "")
   data.3 <- read.csv(file = file.3, header = T)
   para_ele <- as.matrix(data.3[, 2:4])
 
-  load(file = "pqam_dparamhu2021/features_surf.Rdata")
+  load(file = paste(path,"/features_surf.Rdata", sep = ""))
 
   feature.surf.select <- feature.surf.all
   n.ob <- length(data.1[, 1])
   n.feature <- length(feature.surf.select[1, 1,])
   n.feature.ele <- length(para_ele[1,])
   n.feature.all <- n.feature + n.feature.ele
```

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/features_gsf.Rdata` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/features_gsf.Rdata`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/features_surf.Rdata` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/features_surf.Rdata`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/gbm-locfit.R` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/gbm-locfit.R`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/locfit_3_var_all.Rdata` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/locfit_3_var_all.Rdata`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021/locfit_surf_2_var_all.Rdata` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021/locfit_surf_2_var_all.Rdata`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021.egg-info/PKG-INFO` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqam-dparamhu2021
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyQAlloy-compatible Model for D Parameter prediction based on Hu2021
 Author-email: Adam Krajewski <ak@psu.edu>
 Project-URL: Homepage, https://github.com/amkrajewski/pqam-dparamhu2021
 Project-URL: Bug Tracker, https://github.com/amkrajewski/pqam-dparamhu2021/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pqam_dparamhu2021-0.1.1/pqam_dparamhu2021.egg-info/SOURCES.txt` & `pqam_dparamhu2021-0.1.2/pqam_dparamhu2021.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 MANIFEST.in
 README.md
 pyproject.toml
 pqam_dparamhu2021/HEA_pred.R
 pqam_dparamhu2021/LICENSE
 pqam_dparamhu2021/__init__.py
-pqam_dparamhu2021/compositionalModel.py
 pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R
 pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R
 pqam_dparamhu2021/elemental_features.csv
 pqam_dparamhu2021/features_gsf.Rdata
 pqam_dparamhu2021/features_surf.Rdata
 pqam_dparamhu2021/gbm-locfit.R
 pqam_dparamhu2021/locfit_3_var_all.Rdata
 pqam_dparamhu2021/locfit_surf_2_var_all.Rdata
+pqam_dparamhu2021/model.py
 pqam_dparamhu2021.egg-info/PKG-INFO
 pqam_dparamhu2021.egg-info/SOURCES.txt
 pqam_dparamhu2021.egg-info/dependency_links.txt
 pqam_dparamhu2021.egg-info/requires.txt
 pqam_dparamhu2021.egg-info/top_level.txt
 pqam_dparamhu2021/__pycache__/__init__.cpython-39.pyc
-pqam_dparamhu2021/__pycache__/compositionalModel.cpython-39.pyc
+pqam_dparamhu2021/__pycache__/model.cpython-39.pyc
```

### Comparing `pqam_dparamhu2021-0.1.1/pyproject.toml` & `pqam_dparamhu2021-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqam_dparamhu2021"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Adam Krajewski", email="ak@psu.edu" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
```

