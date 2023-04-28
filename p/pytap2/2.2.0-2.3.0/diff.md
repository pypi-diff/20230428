# Comparing `tmp/pytap2-2.2.0.tar.gz` & `tmp/pytap2-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytap2-2.2.0.tar", last modified: Sat Nov  6 18:31:00 2021, max compression
+gzip compressed data, was "pytap2-2.3.0.tar", last modified: Fri Apr 28 12:43:06 2023, max compression
```

## Comparing `pytap2-2.2.0.tar` & `pytap2-2.3.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-11-06 18:31:00.421185 pytap2-2.2.0/
--rw-rw-rw-   0        0        0     1070 2019-12-15 18:16:51.000000 pytap2-2.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       41 2019-12-15 18:16:51.000000 pytap2-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4431 2021-11-06 18:31:00.421185 pytap2-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3444 2021-11-06 18:23:26.000000 pytap2-2.2.0/README.rst
--rw-rw-rw-   0        0        0      491 2020-09-27 18:42:43.000000 pytap2-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      140 2021-11-06 18:31:00.431184 pytap2-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1238 2021-11-06 18:22:02.000000 pytap2-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-06 18:31:00.375184 pytap2-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2021-11-06 18:31:00.394183 pytap2-2.2.0/src/pytap2/
--rw-rw-rw-   0        0        0     7467 2020-09-27 18:52:10.000000 pytap2-2.2.0/src/pytap2/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-06 18:31:00.419184 pytap2-2.2.0/src/pytap2.egg-info/
--rw-rw-rw-   0        0        0     4431 2021-11-06 18:31:00.000000 pytap2-2.2.0/src/pytap2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2021-11-06 18:31:00.000000 pytap2-2.2.0/src/pytap2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-06 18:31:00.000000 pytap2-2.2.0/src/pytap2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-12-30 18:25:23.000000 pytap2-2.2.0/src/pytap2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2021-11-06 18:31:00.000000 pytap2-2.2.0/src/pytap2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 12:43:06.918309 pytap2-2.3.0/
+-rw-rw-rw-   0        0        0     1075 2023-04-28 12:40:08.000000 pytap2-2.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       41 2023-04-27 23:11:00.000000 pytap2-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4517 2023-04-28 12:43:06.918309 pytap2-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3571 2023-04-28 12:42:42.000000 pytap2-2.3.0/README.rst
+-rw-rw-rw-   0        0        0      573 2023-04-28 12:40:08.000000 pytap2-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 12:43:06.918309 pytap2-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-04-28 12:42:42.000000 pytap2-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:43:06.893308 pytap2-2.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 12:43:06.900308 pytap2-2.3.0/src/pytap2/
+-rw-rw-rw-   0        0        0     7490 2023-04-28 12:40:08.000000 pytap2-2.3.0/src/pytap2/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-28 12:40:08.000000 pytap2-2.3.0/src/pytap2/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-28 12:43:06.916307 pytap2-2.3.0/src/pytap2.egg-info/
+-rw-rw-rw-   0        0        0     4517 2023-04-28 12:43:06.000000 pytap2-2.3.0/src/pytap2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-04-28 12:43:06.000000 pytap2-2.3.0/src/pytap2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 12:43:06.000000 pytap2-2.3.0/src/pytap2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-28 12:33:11.000000 pytap2-2.3.0/src/pytap2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-04-28 12:43:06.000000 pytap2-2.3.0/src/pytap2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 12:43:06.917308 pytap2-2.3.0/tests/
+-rw-rw-rw-   0        0        0      146 2023-04-28 12:40:08.000000 pytap2-2.3.0/tests/test_pytap2.py
```

### Comparing `pytap2-2.2.0/LICENSE.txt` & `pytap2-2.3.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2019 John Hagen
+Copyright (c) 2019-2023 John Hagen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytap2-2.2.0/PKG-INFO` & `pytap2-2.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pytap2
-Version: 2.2.0
-Summary: Object-oriented wrapper around the Linux Tun/Tap device for Python 2 and 3
+Version: 2.3.0
+Summary: Object-oriented wrapper around the Linux Tun/Tap device
 Home-page: https://github.com/johnthagen/pytap2
 Author: John Hagen
 Author-email: johnthagen@gmail.com
 License: MIT
 Keywords: pytap,tun,tap,networking
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 ``pytap2`` - Object oriented interface to Linux Tun/Tap devices
 ===============================================================
 
 .. image:: https://github.com/johnthagen/pytap2/workflows/python/badge.svg
     :target: https://github.com/johnthagen/pytap2/actions
@@ -105,14 +104,20 @@
 
 The ``fileno()`` method is defined, so that the device object can be passed directly
 to `select() <https://docs.python.org/library/select.html#select.select>`_.
 
 Releases
 --------
 
+2.3.0 - 2023-04-28
+^^^^^^^^^^^^^^^^^^
+
+- Drop Python 3.7 and support Python 3.11
+- Support Mypy type checking for users
+
 2.2.0 - 2021-11-06
 ^^^^^^^^^^^^^^^^^^
 
 - Drop Python 3.6 and support Python 3.10.
 - Document dependency on ``ifconfig``
 
 2.1.0 - 2020-12-30
@@ -159,9 +164,7 @@
 Allow ``read()`` to be called with a specific number of bytes to read.
 
 
 1.0.0 - 2017-06-16
 ^^^^^^^^^^^^^^^^^^
 
 Initial release that supports Python 2 and 3.
-
-
```

### Comparing `pytap2-2.2.0/README.rst` & `pytap2-2.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -141,76 +141,84 @@
 000008c0: 6e20 6265 2070 6173 7365 6420 6469 7265  n be passed dire
 000008d0: 6374 6c79 0d0a 746f 2060 7365 6c65 6374  ctly..to `select
 000008e0: 2829 203c 6874 7470 733a 2f2f 646f 6373  () <https://docs
 000008f0: 2e70 7974 686f 6e2e 6f72 672f 6c69 6272  .python.org/libr
 00000900: 6172 792f 7365 6c65 6374 2e68 746d 6c23  ary/select.html#
 00000910: 7365 6c65 6374 2e73 656c 6563 743e 605f  select.select>`_
 00000920: 2e0d 0a0d 0a52 656c 6561 7365 730d 0a2d  .....Releases..-
-00000930: 2d2d 2d2d 2d2d 2d0d 0a0d 0a32 2e32 2e30  -------....2.2.0
-00000940: 202d 2032 3032 312d 3131 2d30 360d 0a5e   - 2021-11-06..^
+00000930: 2d2d 2d2d 2d2d 2d0d 0a0d 0a32 2e33 2e30  -------....2.3.0
+00000940: 202d 2032 3032 332d 3034 2d32 380d 0a5e   - 2023-04-28..^
 00000950: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
 00000960: 5e0d 0a0d 0a2d 2044 726f 7020 5079 7468  ^....- Drop Pyth
-00000970: 6f6e 2033 2e36 2061 6e64 2073 7570 706f  on 3.6 and suppo
-00000980: 7274 2050 7974 686f 6e20 332e 3130 2e0d  rt Python 3.10..
-00000990: 0a2d 2044 6f63 756d 656e 7420 6465 7065  .- Document depe
-000009a0: 6e64 656e 6379 206f 6e20 6060 6966 636f  ndency on ``ifco
-000009b0: 6e66 6967 6060 0d0a 0d0a 322e 312e 3020  nfig``....2.1.0 
-000009c0: 2d20 3230 3230 2d31 322d 3330 0d0a 5e5e  - 2020-12-30..^^
+00000970: 6f6e 2033 2e37 2061 6e64 2073 7570 706f  on 3.7 and suppo
+00000980: 7274 2050 7974 686f 6e20 332e 3131 0d0a  rt Python 3.11..
+00000990: 2d20 5375 7070 6f72 7420 4d79 7079 2074  - Support Mypy t
+000009a0: 7970 6520 6368 6563 6b69 6e67 2066 6f72  ype checking for
+000009b0: 2075 7365 7273 0d0a 0d0a 322e 322e 3020   users....2.2.0 
+000009c0: 2d20 3230 3231 2d31 312d 3036 0d0a 5e5e  - 2021-11-06..^^
 000009d0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
 000009e0: 0d0a 0d0a 2d20 4472 6f70 2050 7974 686f  ....- Drop Pytho
-000009f0: 6e20 332e 3520 616e 6420 7375 7070 6f72  n 3.5 and suppor
-00000a00: 7420 5079 7468 6f6e 2033 2e39 2e0d 0a2d  t Python 3.9...-
-00000a10: 2053 7769 7463 6820 746f 2047 6974 4875   Switch to GitHu
-00000a20: 6220 4163 7469 6f6e 7320 666f 7220 4349  b Actions for CI
-00000a30: 2e0d 0a0d 0a32 2e30 2e30 202d 2032 3032  .....2.0.0 - 202
-00000a40: 302d 3033 2d32 390d 0a5e 5e5e 5e5e 5e5e  0-03-29..^^^^^^^
-00000a50: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d 0a0d 0a2d  ^^^^^^^^^^^....-
-00000a60: 2044 726f 7020 5079 7468 6f6e 2032 2e37   Drop Python 2.7
-00000a70: 2e0d 0a0d 0a31 2e36 2e30 202d 2032 3031  .....1.6.0 - 201
-00000a80: 392d 3132 2d31 350d 0a5e 5e5e 5e5e 5e5e  9-12-15..^^^^^^^
-00000a90: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d 0a0d 0a2d  ^^^^^^^^^^^....-
-00000aa0: 2044 726f 7020 5079 7468 6f6e 2033 2e34   Drop Python 3.4
-00000ab0: 2061 6e64 2073 7570 706f 7274 2050 7974   and support Pyt
-00000ac0: 686f 6e20 332e 382e 0d0a 2d20 496e 636c  hon 3.8...- Incl
-00000ad0: 7564 6520 6c69 6365 6e73 6520 6669 6c65  ude license file
-00000ae0: 2e0d 0a0d 0a31 2e35 2e30 202d 2032 3031  .....1.5.0 - 201
-00000af0: 382d 3037 2d30 390d 0a5e 5e5e 5e5e 5e5e  8-07-09..^^^^^^^
-00000b00: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d 0a0d 0a53  ^^^^^^^^^^^....S
-00000b10: 7570 706f 7274 2050 7974 686f 6e20 332e  upport Python 3.
-00000b20: 372e 0d0a 0d0a 312e 342e 3020 2d20 3230  7.....1.4.0 - 20
-00000b30: 3137 2d31 302d 3234 0d0a 5e5e 5e5e 5e5e  17-10-24..^^^^^^
-00000b40: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a  ^^^^^^^^^^^^....
-00000b50: 416c 6c6f 7720 6469 7361 626c 696e 6720  Allow disabling 
-00000b60: 7061 636b 6574 2069 6e66 6f72 6d61 7469  packet informati
-00000b70: 6f6e 2068 6561 6465 7220 2860 6049 4646  on header (``IFF
-00000b80: 5f4e 4f5f 5049 6060 2920 616e 6420 6465  _NO_PI``) and de
-00000b90: 6661 756c 7420 6060 7265 6164 2829 6060  fault ``read()``
-00000ba0: 2074 6f20 7265 6164 2065 6e74 6972 650d   to read entire.
-00000bb0: 0a4d 5455 2077 6f72 7468 206f 6620 6461  .MTU worth of da
-00000bc0: 7461 2070 6c75 7320 7468 6520 7061 636b  ta plus the pack
-00000bd0: 6574 2069 6e66 6f72 6d61 7469 6f6e 2068  et information h
-00000be0: 6561 6465 7220 6966 2070 7265 7365 6e74  eader if present
-00000bf0: 2e0d 0a0d 0a31 2e33 2e30 202d 2032 3031  .....1.3.0 - 201
-00000c00: 372d 3037 2d33 310d 0a5e 5e5e 5e5e 5e5e  7-07-31..^^^^^^^
-00000c10: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d 0a0d 0a41  ^^^^^^^^^^^....A
-00000c20: 6464 2060 6066 696c 656e 6f28 2960 6020  dd ``fileno()`` 
-00000c30: 6d65 7468 6f64 2074 6f20 7375 7070 6f72  method to suppor
-00000c40: 7420 6060 7365 6c65 6374 2829 6060 2063  t ``select()`` c
-00000c50: 616c 6c73 2e0d 0a0d 0a31 2e32 2e30 202d  alls.....1.2.0 -
-00000c60: 2032 3031 372d 3036 2d31 390d 0a5e 5e5e   2017-06-19..^^^
-00000c70: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d  ^^^^^^^^^^^^^^^.
-00000c80: 0a0d 0a43 6f6e 7465 7874 206d 616e 6167  ...Context manag
-00000c90: 6572 2073 7570 706f 7274 2061 6464 6564  er support added
-00000ca0: 2e0d 0a0d 0a31 2e31 2e30 202d 2032 3031  .....1.1.0 - 201
-00000cb0: 372d 3036 2d31 370d 0a5e 5e5e 5e5e 5e5e  7-06-17..^^^^^^^
-00000cc0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d 0a0d 0a41  ^^^^^^^^^^^....A
-00000cd0: 6c6c 6f77 2060 6072 6561 6428 2960 6020  llow ``read()`` 
-00000ce0: 746f 2062 6520 6361 6c6c 6564 2077 6974  to be called wit
-00000cf0: 6820 6120 7370 6563 6966 6963 206e 756d  h a specific num
-00000d00: 6265 7220 6f66 2062 7974 6573 2074 6f20  ber of bytes to 
-00000d10: 7265 6164 2e0d 0a0d 0a0d 0a31 2e30 2e30  read.......1.0.0
-00000d20: 202d 2032 3031 372d 3036 2d31 360d 0a5e   - 2017-06-16..^
-00000d30: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-00000d40: 5e0d 0a0d 0a49 6e69 7469 616c 2072 656c  ^....Initial rel
-00000d50: 6561 7365 2074 6861 7420 7375 7070 6f72  ease that suppor
-00000d60: 7473 2050 7974 686f 6e20 3220 616e 6420  ts Python 2 and 
-00000d70: 332e 0d0a                                3...
+000009f0: 6e20 332e 3620 616e 6420 7375 7070 6f72  n 3.6 and suppor
+00000a00: 7420 5079 7468 6f6e 2033 2e31 302e 0d0a  t Python 3.10...
+00000a10: 2d20 446f 6375 6d65 6e74 2064 6570 656e  - Document depen
+00000a20: 6465 6e63 7920 6f6e 2060 6069 6663 6f6e  dency on ``ifcon
+00000a30: 6669 6760 600d 0a0d 0a32 2e31 2e30 202d  fig``....2.1.0 -
+00000a40: 2032 3032 302d 3132 2d33 300d 0a5e 5e5e   2020-12-30..^^^
+00000a50: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d  ^^^^^^^^^^^^^^^.
+00000a60: 0a0d 0a2d 2044 726f 7020 5079 7468 6f6e  ...- Drop Python
+00000a70: 2033 2e35 2061 6e64 2073 7570 706f 7274   3.5 and support
+00000a80: 2050 7974 686f 6e20 332e 392e 0d0a 2d20   Python 3.9...- 
+00000a90: 5377 6974 6368 2074 6f20 4769 7448 7562  Switch to GitHub
+00000aa0: 2041 6374 696f 6e73 2066 6f72 2043 492e   Actions for CI.
+00000ab0: 0d0a 0d0a 322e 302e 3020 2d20 3230 3230  ....2.0.0 - 2020
+00000ac0: 2d30 332d 3239 0d0a 5e5e 5e5e 5e5e 5e5e  -03-29..^^^^^^^^
+00000ad0: 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a 2d20  ^^^^^^^^^^....- 
+00000ae0: 4472 6f70 2050 7974 686f 6e20 322e 372e  Drop Python 2.7.
+00000af0: 0d0a 0d0a 312e 362e 3020 2d20 3230 3139  ....1.6.0 - 2019
+00000b00: 2d31 322d 3135 0d0a 5e5e 5e5e 5e5e 5e5e  -12-15..^^^^^^^^
+00000b10: 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a 2d20  ^^^^^^^^^^....- 
+00000b20: 4472 6f70 2050 7974 686f 6e20 332e 3420  Drop Python 3.4 
+00000b30: 616e 6420 7375 7070 6f72 7420 5079 7468  and support Pyth
+00000b40: 6f6e 2033 2e38 2e0d 0a2d 2049 6e63 6c75  on 3.8...- Inclu
+00000b50: 6465 206c 6963 656e 7365 2066 696c 652e  de license file.
+00000b60: 0d0a 0d0a 312e 352e 3020 2d20 3230 3138  ....1.5.0 - 2018
+00000b70: 2d30 372d 3039 0d0a 5e5e 5e5e 5e5e 5e5e  -07-09..^^^^^^^^
+00000b80: 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a 5375  ^^^^^^^^^^....Su
+00000b90: 7070 6f72 7420 5079 7468 6f6e 2033 2e37  pport Python 3.7
+00000ba0: 2e0d 0a0d 0a31 2e34 2e30 202d 2032 3031  .....1.4.0 - 201
+00000bb0: 372d 3130 2d32 340d 0a5e 5e5e 5e5e 5e5e  7-10-24..^^^^^^^
+00000bc0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d 0a0d 0a41  ^^^^^^^^^^^....A
+00000bd0: 6c6c 6f77 2064 6973 6162 6c69 6e67 2070  llow disabling p
+00000be0: 6163 6b65 7420 696e 666f 726d 6174 696f  acket informatio
+00000bf0: 6e20 6865 6164 6572 2028 6060 4946 465f  n header (``IFF_
+00000c00: 4e4f 5f50 4960 6029 2061 6e64 2064 6566  NO_PI``) and def
+00000c10: 6175 6c74 2060 6072 6561 6428 2960 6020  ault ``read()`` 
+00000c20: 746f 2072 6561 6420 656e 7469 7265 0d0a  to read entire..
+00000c30: 4d54 5520 776f 7274 6820 6f66 2064 6174  MTU worth of dat
+00000c40: 6120 706c 7573 2074 6865 2070 6163 6b65  a plus the packe
+00000c50: 7420 696e 666f 726d 6174 696f 6e20 6865  t information he
+00000c60: 6164 6572 2069 6620 7072 6573 656e 742e  ader if present.
+00000c70: 0d0a 0d0a 312e 332e 3020 2d20 3230 3137  ....1.3.0 - 2017
+00000c80: 2d30 372d 3331 0d0a 5e5e 5e5e 5e5e 5e5e  -07-31..^^^^^^^^
+00000c90: 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a 4164  ^^^^^^^^^^....Ad
+00000ca0: 6420 6060 6669 6c65 6e6f 2829 6060 206d  d ``fileno()`` m
+00000cb0: 6574 686f 6420 746f 2073 7570 706f 7274  ethod to support
+00000cc0: 2060 6073 656c 6563 7428 2960 6020 6361   ``select()`` ca
+00000cd0: 6c6c 732e 0d0a 0d0a 312e 322e 3020 2d20  lls.....1.2.0 - 
+00000ce0: 3230 3137 2d30 362d 3139 0d0a 5e5e 5e5e  2017-06-19..^^^^
+00000cf0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a  ^^^^^^^^^^^^^^..
+00000d00: 0d0a 436f 6e74 6578 7420 6d61 6e61 6765  ..Context manage
+00000d10: 7220 7375 7070 6f72 7420 6164 6465 642e  r support added.
+00000d20: 0d0a 0d0a 312e 312e 3020 2d20 3230 3137  ....1.1.0 - 2017
+00000d30: 2d30 362d 3137 0d0a 5e5e 5e5e 5e5e 5e5e  -06-17..^^^^^^^^
+00000d40: 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a 416c  ^^^^^^^^^^....Al
+00000d50: 6c6f 7720 6060 7265 6164 2829 6060 2074  low ``read()`` t
+00000d60: 6f20 6265 2063 616c 6c65 6420 7769 7468  o be called with
+00000d70: 2061 2073 7065 6369 6669 6320 6e75 6d62   a specific numb
+00000d80: 6572 206f 6620 6279 7465 7320 746f 2072  er of bytes to r
+00000d90: 6561 642e 0d0a 0d0a 0d0a 312e 302e 3020  ead.......1.0.0 
+00000da0: 2d20 3230 3137 2d30 362d 3136 0d0a 5e5e  - 2017-06-16..^^
+00000db0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+00000dc0: 0d0a 0d0a 496e 6974 6961 6c20 7265 6c65  ....Initial rele
+00000dd0: 6173 6520 7468 6174 2073 7570 706f 7274  ase that support
+00000de0: 7320 5079 7468 6f6e 2032 2061 6e64 2033  s Python 2 and 3
+00000df0: 2e0d 0a                                  ...
```

### Comparing `pytap2-2.2.0/setup.py` & `pytap2-2.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env python3
 
 import setuptools
 
 setuptools.setup(
     name="pytap2",
-    version="2.2.0",
-    description="Object-oriented wrapper around the Linux Tun/Tap device for Python 2 and 3",
+    version="2.3.0",
+    description="Object-oriented wrapper around the Linux Tun/Tap device",
     long_description=open("README.rst").read(),
-    keywords=("pytap", "tun", "tap", "networking"),
+    keywords=["pytap", "tun", "tap", "networking"],
     author="John Hagen",
     author_email="johnthagen@gmail.com",
     url="https://github.com/johnthagen/pytap2",
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
+    package_data={"pytap2": ["py.typed"]},
     include_package_data=True,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `pytap2-2.2.0/src/pytap2/__init__.py` & `pytap2-2.3.0/src/pytap2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module that wraps the Linux Tun/Tap device."""
 
 import atexit
 import enum
 import fcntl
 import os
 import struct
-from typing import Optional
+from typing import Any, Optional
 
 TUNSETIFF = 0x400454CA
 
 IFF_NO_PI = 0x1000
 """Mask to disable packet information from being prepended to packets sent through TUN/TAP."""
 
 PACKET_INFO_SIZE = 4
@@ -70,15 +70,15 @@
         self._enable_packet_info = enable_packet_info
         mode_value = self._mode.value
         if not self._enable_packet_info:
             mode_value |= IFF_NO_PI
 
         ifs = fcntl.ioctl(
             self._fd,
-            TUNSETIFF,  # type: ignore
+            TUNSETIFF,
             struct.pack("16sH", self._name.encode(), mode_value),
         )
 
         # Retrieve real interface name from control device.
         self._name = ifs[:16].strip(b"\x00").decode()
 
         self._mtu = mtu
@@ -86,15 +86,15 @@
         # Properly close device on exit.
         atexit.register(self.close)
 
     def __enter__(self) -> "TapDevice":
         self.up()
         return self
 
-    def __exit__(self, exc_type, exc_value, exc_tb):
+    def __exit__(self, exc_type: Any, exc_value: Any, exc_tb: Any) -> None:
         self.close()
 
     @property
     def name(self) -> str:
         """The device name."""
         return self._name
 
@@ -127,15 +127,15 @@
         return self._fd
 
     def read(self, num_bytes: Optional[int] = None) -> bytes:
         """Read data from the device.
 
         Args:
             num_bytes: The number of bytes to read. If not specified, the MTU size is used,
-                including the optional packet information header if enabled on a the device.
+                including the optional packet information header if enabled on the device.
         """
         if num_bytes is None:
             num_bytes = self._mtu
             # If packet information is enabled, 4 extra bytes will be appended to a packet
             # that is potentially already the maximum MTU size, so ensure that by
             # default we can read one entire MTU-sized packet and this header.
             if self._enable_packet_info:
@@ -143,15 +143,15 @@
 
         return os.read(self._fd, num_bytes)
 
     def write(self, data: bytes) -> None:
         """Write data to the device. No care is taken for MTU limitations or similar."""
         os.write(self._fd, data)
 
-    def ifconfig(self, **args):
+    def ifconfig(self, **args: Any) -> None:
         """Issue ifconfig command on the device.
 
         Keyword Args:
             address: IP address of the device, can be in CIDR notation (see man ifconfig).
             netmask: Network mask.
             network: Network base address, normally set automatically.
             broadcast: Broadcast address, normally set automatically.
```

### Comparing `pytap2-2.2.0/src/pytap2.egg-info/PKG-INFO` & `pytap2-2.3.0/src/pytap2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pytap2
-Version: 2.2.0
-Summary: Object-oriented wrapper around the Linux Tun/Tap device for Python 2 and 3
+Version: 2.3.0
+Summary: Object-oriented wrapper around the Linux Tun/Tap device
 Home-page: https://github.com/johnthagen/pytap2
 Author: John Hagen
 Author-email: johnthagen@gmail.com
 License: MIT
 Keywords: pytap,tun,tap,networking
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 ``pytap2`` - Object oriented interface to Linux Tun/Tap devices
 ===============================================================
 
 .. image:: https://github.com/johnthagen/pytap2/workflows/python/badge.svg
     :target: https://github.com/johnthagen/pytap2/actions
@@ -105,14 +104,20 @@
 
 The ``fileno()`` method is defined, so that the device object can be passed directly
 to `select() <https://docs.python.org/library/select.html#select.select>`_.
 
 Releases
 --------
 
+2.3.0 - 2023-04-28
+^^^^^^^^^^^^^^^^^^
+
+- Drop Python 3.7 and support Python 3.11
+- Support Mypy type checking for users
+
 2.2.0 - 2021-11-06
 ^^^^^^^^^^^^^^^^^^
 
 - Drop Python 3.6 and support Python 3.10.
 - Document dependency on ``ifconfig``
 
 2.1.0 - 2020-12-30
@@ -159,9 +164,7 @@
 Allow ``read()`` to be called with a specific number of bytes to read.
 
 
 1.0.0 - 2017-06-16
 ^^^^^^^^^^^^^^^^^^
 
 Initial release that supports Python 2 and 3.
-
-
```

