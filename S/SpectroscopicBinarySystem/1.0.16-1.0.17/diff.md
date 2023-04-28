# Comparing `tmp/SpectroscopicBinarySystem-1.0.16.tar.gz` & `tmp/SpectroscopicBinarySystem-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.0.16.tar", last modified: Fri Apr 28 12:14:31 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.0.17.tar", last modified: Fri Apr 28 12:33:43 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.0.16.tar` & `SpectroscopicBinarySystem-1.0.17.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 12:14:31.946306 SpectroscopicBinarySystem-1.0.16/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.16/LICENSE
--rw-rw-rw-   0        0        0     2127 2023-04-28 12:14:31.946306 SpectroscopicBinarySystem-1.0.16/PKG-INFO
--rw-rw-rw-   0        0        0     1736 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.16/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 12:14:31.942301 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     2127 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.0.16/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-04-28 12:14:31.950312 SpectroscopicBinarySystem-1.0.16/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 12:14:31.946306 SpectroscopicBinarySystem-1.0.16/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    26258 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.16/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:33:43.513624 SpectroscopicBinarySystem-1.0.17/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.17/LICENSE
+-rw-rw-rw-   0        0        0     2128 2023-04-28 12:33:43.513624 SpectroscopicBinarySystem-1.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1736 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.17/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 12:33:43.509614 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     2128 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.0.17/pyproject.toml
+-rw-rw-rw-   0        0        0      725 2023-04-28 12:33:43.516632 SpectroscopicBinarySystem-1.0.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 12:33:43.510616 SpectroscopicBinarySystem-1.0.17/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    26258 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.17/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.0.16/LICENSE` & `SpectroscopicBinarySystem-1.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.16/PKG-INFO` & `SpectroscopicBinarySystem-1.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.16
+Version: 1.0.17
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
```

### Comparing `SpectroscopicBinarySystem-1.0.16/README.md` & `SpectroscopicBinarySystem-1.0.17/README.md`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.16
+Version: 1.0.17
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
```

### Comparing `SpectroscopicBinarySystem-1.0.16/setup.cfg` & `SpectroscopicBinarySystem-1.0.17/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 302e 3136 0d0a  rsion = 1.0.16..
+00000030: 7273 696f 6e20 3d20 312e 302e 3137 0d0a  rsion = 1.0.17..
 00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
 00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
 00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
 00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
 00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
 000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
@@ -22,25 +22,25 @@
 00000150: 7374 726f 6e6f 6d79 2c61 7374 726f 7068  stronomy,astroph
 00000160: 7973 6963 732c 7363 6965 6e63 652c 6669  ysics,science,fi
 00000170: 7473 2c6d 6f64 656c 732c 6669 7474 696e  ts,models,fittin
 00000180: 672c 7370 6563 7472 6f73 636f 7079 2c73  g,spectroscopy,s
 00000190: 7065 6374 7275 6d0d 0a0d 0a5b 6f70 7469  pectrum....[opti
 000001a0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
 000001b0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-000001c0: 6571 7569 7265 7320 3d20 3e3d 332e 390d  equires = >=3.9.
-000001d0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-000001e0: 7320 3d20 0d0a 0961 7374 726f 7079 3e3d  s = ...astropy>=
-000001f0: 352e 322e 320d 0a09 6173 7472 6f71 7565  5.2.2...astroque
-00000200: 7279 3e3d 302e 342e 360d 0a09 4269 6e61  ry>=0.4.6...Bina
-00000210: 7279 5374 6172 536f 6c76 6572 3e3d 312e  ryStarSolver>=1.
-00000220: 322e 300d 0a09 6d61 7470 6c6f 746c 6962  2.0...matplotlib
-00000230: 3e3d 332e 372e 310d 0a09 6e75 6d70 793e  >=3.7.1...numpy>
-00000240: 3d31 2e32 342e 320d 0a09 4f72 6269 7461  =1.24.2...Orbita
-00000250: 6c50 793e 3d30 2e37 2e30 0d0a 0950 7959  lPy>=0.7.0...PyY
-00000260: 414d 4c3e 3d36 2e30 0d0a 0973 7065 6375  AML>=6.0...specu
-00000270: 7469 6c73 3e3d 312e 392e 310d 0a09 4269  tils>=1.9.1...Bi
-00000280: 6e61 7279 5374 6172 536f 6c76 6572 3e3d  naryStarSolver>=
-00000290: 312e 322e 300d 0a09 706c 6f74 6c79 3e3d  1.2.0...plotly>=
-000002a0: 352e 3134 2e31 0d0a 0d0a 5b65 6767 5f69  5.14.1....[egg_i
-000002b0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000002c0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000002d0: 0d0a 0d0a                                ....
+000001c0: 6571 7569 7265 7320 3d20 3e3d 332e 3130  equires = >=3.10
+000001d0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+000001e0: 6573 203d 200d 0a09 6173 7472 6f70 793e  es = ...astropy>
+000001f0: 3d35 2e32 2e32 0d0a 0961 7374 726f 7175  =5.2.2...astroqu
+00000200: 6572 793e 3d30 2e34 2e36 0d0a 0942 696e  ery>=0.4.6...Bin
+00000210: 6172 7953 7461 7253 6f6c 7665 723e 3d31  aryStarSolver>=1
+00000220: 2e32 2e30 0d0a 096d 6174 706c 6f74 6c69  .2.0...matplotli
+00000230: 623e 3d33 2e37 2e31 0d0a 096e 756d 7079  b>=3.7.1...numpy
+00000240: 3e3d 312e 3234 2e32 0d0a 094f 7262 6974  >=1.24.2...Orbit
+00000250: 616c 5079 3e3d 302e 372e 300d 0a09 5079  alPy>=0.7.0...Py
+00000260: 5941 4d4c 3e3d 362e 300d 0a09 7370 6563  YAML>=6.0...spec
+00000270: 7574 696c 733e 3d31 2e39 2e31 0d0a 0942  utils>=1.9.1...B
+00000280: 696e 6172 7953 7461 7253 6f6c 7665 723e  inaryStarSolver>
+00000290: 3d31 2e32 2e30 0d0a 0970 6c6f 746c 793e  =1.2.0...plotly>
+000002a0: 3d35 2e31 342e 310d 0a0d 0a5b 6567 675f  =5.14.1....[egg_
+000002b0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+000002c0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000002d0: 300d 0a0d 0a                             0....
```

### Comparing `SpectroscopicBinarySystem-1.0.16/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.0.17/spectroscopicbinarysystem/__init__.py`

 * *Files identical despite different names*

