# Comparing `tmp/unipolator-0.2.7.tar.gz` & `tmp/unipolator-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipolator-0.2.7.tar", last modified: Wed Apr 26 14:13:47 2023, max compression
+gzip compressed data, was "unipolator-0.2.8.tar", last modified: Fri Apr 28 09:19:28 2023, max compression
```

## Comparing `unipolator-0.2.7.tar` & `unipolator-0.2.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 14:13:47.782727 unipolator-0.2.7/
--rw-rw-rw-   0        0        0     1096 2023-04-26 14:12:56.000000 unipolator-0.2.7/LICENSE
--rw-rw-rw-   0        0        0       86 2023-04-26 14:12:56.000000 unipolator-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1791 2023-04-26 14:13:47.783726 unipolator-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-04-26 14:12:56.000000 unipolator-0.2.7/README.md
--rw-rw-rw-   0        0        0       30 2023-04-26 14:12:56.000000 unipolator-0.2.7/requirements-dev.txt
--rw-rw-rw-   0        0        0       27 2023-04-26 14:12:56.000000 unipolator-0.2.7/requirements.txt
--rw-rw-rw-   0        0        0      976 2023-04-26 14:13:47.816600 unipolator-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     3298 2023-04-26 14:12:56.000000 unipolator-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:13:47.346764 unipolator-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 14:13:47.666504 unipolator-0.2.7/src/unipolator/
--rw-rw-rw-   0        0        0      408 2023-03-30 16:40:02.000000 unipolator-0.2.7/src/unipolator/__init__.py
--rw-rw-rw-   0        0        0  1031537 2023-04-26 14:13:07.000000 unipolator-0.2.7/src/unipolator/blas_functions.c
--rw-rw-rw-   0        0        0     3446 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/blas_functions.pxd
--rw-rw-rw-   0        0        0    12512 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/blas_functions.pyx
--rw-rw-rw-   0        0        0  1168547 2023-04-26 14:13:10.000000 unipolator-0.2.7/src/unipolator/caching.c
--rw-rw-rw-   0        0        0      327 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/caching.pxd
--rw-rw-rw-   0        0        0    16121 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/caching.pyx
--rw-rw-rw-   0        0        0  1116857 2023-04-26 14:13:15.000000 unipolator-0.2.7/src/unipolator/exp_and_log.c
--rw-rw-rw-   0        0        0     4322 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/exp_and_log.pxd
--rw-rw-rw-   0        0        0    16417 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/exp_and_log.pyx
--rw-rw-rw-   0        0        0  1054030 2023-04-26 14:13:22.000000 unipolator-0.2.7/src/unipolator/hamiltonian_system.c
--rw-rw-rw-   0        0        0    11198 2023-04-26 14:07:05.000000 unipolator-0.2.7/src/unipolator/hamiltonian_system.pyx
--rw-rw-rw-   0        0        0  1174002 2023-04-26 14:13:25.000000 unipolator-0.2.7/src/unipolator/indexing.c
--rw-rw-rw-   0        0        0     1918 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/indexing.pxd
--rw-rw-rw-   0        0        0    11597 2023-03-14 14:26:21.000000 unipolator-0.2.7/src/unipolator/indexing.pyx
--rw-rw-rw-   0        0        0   996531 2023-04-26 14:13:31.000000 unipolator-0.2.7/src/unipolator/sym_trotter_system.c
--rw-rw-rw-   0        0        0    13737 2023-04-26 08:32:03.000000 unipolator-0.2.7/src/unipolator/sym_trotter_system.pyx
--rw-rw-rw-   0        0        0  1087291 2023-04-26 14:13:35.000000 unipolator-0.2.7/src/unipolator/symmetric_unitary_interpolation.c
--rw-rw-rw-   0        0        0    11305 2023-04-24 12:15:16.000000 unipolator-0.2.7/src/unipolator/symmetric_unitary_interpolation.pyx
--rw-rw-rw-   0        0        0   986270 2023-04-26 14:13:41.000000 unipolator-0.2.7/src/unipolator/trotter_system.c
--rw-rw-rw-   0        0        0    13643 2023-04-24 12:19:37.000000 unipolator-0.2.7/src/unipolator/trotter_system.pyx
--rw-rw-rw-   0        0        0      220 2023-04-24 11:56:46.000000 unipolator-0.2.7/src/unipolator/unipolator.pyx
--rw-rw-rw-   0        0        0  1186825 2023-04-26 14:13:44.000000 unipolator-0.2.7/src/unipolator/unitary_interpolation.c
--rw-rw-rw-   0        0        0    21275 2023-04-24 12:14:55.000000 unipolator-0.2.7/src/unipolator/unitary_interpolation.pyx
-drwxrwxrwx   0        0        0        0 2023-04-26 14:13:47.779708 unipolator-0.2.7/src/unipolator.egg-info/
--rw-rw-rw-   0        0        0     1791 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2023-04-26 14:13:46.000000 unipolator-0.2.7/src/unipolator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       86 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 09:19:28.943419 unipolator-0.2.8/
+-rw-rw-rw-   0        0        0     1096 2023-04-28 09:18:47.000000 unipolator-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0       86 2023-04-28 09:18:47.000000 unipolator-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1791 2023-04-28 09:19:28.943419 unipolator-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-04-28 09:18:47.000000 unipolator-0.2.8/README.md
+-rw-rw-rw-   0        0        0       30 2023-04-28 09:18:47.000000 unipolator-0.2.8/requirements-dev.txt
+-rw-rw-rw-   0        0        0       27 2023-04-28 09:18:47.000000 unipolator-0.2.8/requirements.txt
+-rw-rw-rw-   0        0        0      976 2023-04-28 09:19:28.944415 unipolator-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     3299 2023-04-28 09:18:47.000000 unipolator-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:19:28.809271 unipolator-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 09:19:28.925378 unipolator-0.2.8/src/unipolator/
+-rw-rw-rw-   0        0        0      408 2023-03-30 16:40:02.000000 unipolator-0.2.8/src/unipolator/__init__.py
+-rw-rw-rw-   0        0        0  1031537 2023-04-28 09:18:57.000000 unipolator-0.2.8/src/unipolator/blas_functions.c
+-rw-rw-rw-   0        0        0     3446 2023-03-14 14:26:20.000000 unipolator-0.2.8/src/unipolator/blas_functions.pxd
+-rw-rw-rw-   0        0        0    12512 2023-03-14 14:26:20.000000 unipolator-0.2.8/src/unipolator/blas_functions.pyx
+-rw-rw-rw-   0        0        0  1168547 2023-04-28 09:18:59.000000 unipolator-0.2.8/src/unipolator/caching.c
+-rw-rw-rw-   0        0        0      327 2023-03-14 14:26:20.000000 unipolator-0.2.8/src/unipolator/caching.pxd
+-rw-rw-rw-   0        0        0    16121 2023-03-14 14:26:20.000000 unipolator-0.2.8/src/unipolator/caching.pyx
+-rw-rw-rw-   0        0        0  1116857 2023-04-28 09:19:04.000000 unipolator-0.2.8/src/unipolator/exp_and_log.c
+-rw-rw-rw-   0        0        0     4322 2023-03-14 14:26:20.000000 unipolator-0.2.8/src/unipolator/exp_and_log.pxd
+-rw-rw-rw-   0        0        0    16417 2023-03-14 14:26:20.000000 unipolator-0.2.8/src/unipolator/exp_and_log.pyx
+-rw-rw-rw-   0        0        0  1054030 2023-04-28 09:19:09.000000 unipolator-0.2.8/src/unipolator/hamiltonian_system.c
+-rw-rw-rw-   0        0        0    11198 2023-04-26 14:07:05.000000 unipolator-0.2.8/src/unipolator/hamiltonian_system.pyx
+-rw-rw-rw-   0        0        0  1174002 2023-04-28 09:19:11.000000 unipolator-0.2.8/src/unipolator/indexing.c
+-rw-rw-rw-   0        0        0     1918 2023-03-14 14:26:20.000000 unipolator-0.2.8/src/unipolator/indexing.pxd
+-rw-rw-rw-   0        0        0    11597 2023-03-14 14:26:21.000000 unipolator-0.2.8/src/unipolator/indexing.pyx
+-rw-rw-rw-   0        0        0   996531 2023-04-28 09:19:16.000000 unipolator-0.2.8/src/unipolator/sym_trotter_system.c
+-rw-rw-rw-   0        0        0    13737 2023-04-26 08:32:03.000000 unipolator-0.2.8/src/unipolator/sym_trotter_system.pyx
+-rw-rw-rw-   0        0        0  1087291 2023-04-28 09:19:19.000000 unipolator-0.2.8/src/unipolator/symmetric_unitary_interpolation.c
+-rw-rw-rw-   0        0        0    11305 2023-04-24 12:15:16.000000 unipolator-0.2.8/src/unipolator/symmetric_unitary_interpolation.pyx
+-rw-rw-rw-   0        0        0   986270 2023-04-28 09:19:24.000000 unipolator-0.2.8/src/unipolator/trotter_system.c
+-rw-rw-rw-   0        0        0    13643 2023-04-24 12:19:37.000000 unipolator-0.2.8/src/unipolator/trotter_system.pyx
+-rw-rw-rw-   0        0        0      220 2023-04-24 11:56:46.000000 unipolator-0.2.8/src/unipolator/unipolator.pyx
+-rw-rw-rw-   0        0        0  1186825 2023-04-28 09:19:27.000000 unipolator-0.2.8/src/unipolator/unitary_interpolation.c
+-rw-rw-rw-   0        0        0    21275 2023-04-24 12:14:55.000000 unipolator-0.2.8/src/unipolator/unitary_interpolation.pyx
+drwxrwxrwx   0        0        0        0 2023-04-28 09:19:28.942418 unipolator-0.2.8/src/unipolator.egg-info/
+-rw-rw-rw-   0        0        0     1791 2023-04-28 09:19:28.000000 unipolator-0.2.8/src/unipolator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2023-04-28 09:19:28.000000 unipolator-0.2.8/src/unipolator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:19:28.000000 unipolator-0.2.8/src/unipolator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-28 09:19:28.000000 unipolator-0.2.8/src/unipolator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       86 2023-04-28 09:19:28.000000 unipolator-0.2.8/src/unipolator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-28 09:19:28.000000 unipolator-0.2.8/src/unipolator.egg-info/top_level.txt
```

### Comparing `unipolator-0.2.7/LICENSE` & `unipolator-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/PKG-INFO` & `unipolator-0.2.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: unipolator
-Version: 0.2.7
+Version: 0.2.8
 Summary: Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.
 Home-page: https://github.com/Ntropic/unipolator
-Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.7.tar.gz
+Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.8.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `unipolator-0.2.7/README.md` & `unipolator-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/setup.cfg` & `unipolator-0.2.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 706f 6c61 746f 720d 0a76   = unipolator..v
-00000020: 6572 7369 6f6e 203d 2030 2e32 2e37 0d0a  ersion = 0.2.7..
+00000020: 6572 7369 6f6e 203d 2030 2e32 2e38 0d0a  ersion = 0.2.8..
 00000030: 6175 7468 6f72 203d 204d 6963 6861 656c  author = Michael
 00000040: 2053 6368 696c 6c69 6e67 0d0a 6175 7468   Schilling..auth
 00000050: 6f72 5f65 6d61 696c 203d 206d 6963 6861  or_email = micha
 00000060: 656c 406e 7472 6f70 6963 2e64 650d 0a64  el@ntropic.de..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2055 6e69  escription = Uni
 00000080: 706f 6c61 746f 7220 616c 6c6f 7773 2066  polator allows f
 00000090: 6f72 206e 2064 696d 656e 7369 6f6e 616c  or n dimensional
@@ -25,15 +25,15 @@
 00000180: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
 00000190: 2f67 6974 6875 622e 636f 6d2f 4e74 726f  /github.com/Ntro
 000001a0: 7069 632f 756e 6970 6f6c 6174 6f72 0d0a  pic/unipolator..
 000001b0: 646f 776e 6c6f 6164 5f75 726c 203d 2068  download_url = h
 000001c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000001d0: 6d2f 4e74 726f 7069 632f 756e 6970 6f6c  m/Ntropic/unipol
 000001e0: 6174 6f72 2f61 7263 6869 7665 2f72 6566  ator/archive/ref
-000001f0: 732f 7461 6773 2f76 302e 322e 372e 7461  s/tags/v0.2.7.ta
+000001f0: 732f 7461 6773 2f76 302e 322e 382e 7461  s/tags/v0.2.8.ta
 00000200: 722e 677a 0d0a 5072 6f67 7261 6d6d 696e  r.gz..Programmin
 00000210: 6720 4c61 6e67 7561 6765 203d 203a 2050  g Language = : P
 00000220: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
 00000230: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000240: 6520 3a3a 2050 7974 686f 6e20 3a3a 2049  e :: Python :: I
 00000250: 6d70 6c65 6d65 6e74 6174 696f 6e20 3a3a  mplementation ::
 00000260: 2043 5079 7468 6f6e 0d0a 0949 6e74 656e   CPython...Inten
```

### Comparing `unipolator-0.2.7/setup.py` & `unipolator-0.2.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 
 with open("requirements-dev.txt") as fp:
     dev_requires = fp.read().strip().split("\n")
 
 setup(   
     name = "unipolator",
     #zip_safe = False,
-    version          = "0.2.7",
+    version           = "0.2.8",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Ntropic/unipolator",
-    download_url = "https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.7.tar.gz",
+    download_url = "https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.8.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     ext_modules = extensions,
     install_requires = install_requires,
```

### Comparing `unipolator-0.2.7/src/unipolator/blas_functions.c` & `unipolator-0.2.8/src/unipolator/blas_functions.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/blas_functions.pxd` & `unipolator-0.2.8/src/unipolator/blas_functions.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/blas_functions.pyx` & `unipolator-0.2.8/src/unipolator/blas_functions.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/caching.c` & `unipolator-0.2.8/src/unipolator/caching.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/caching.pyx` & `unipolator-0.2.8/src/unipolator/caching.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/exp_and_log.c` & `unipolator-0.2.8/src/unipolator/exp_and_log.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/exp_and_log.pxd` & `unipolator-0.2.8/src/unipolator/exp_and_log.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/exp_and_log.pyx` & `unipolator-0.2.8/src/unipolator/exp_and_log.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/hamiltonian_system.c` & `unipolator-0.2.8/src/unipolator/hamiltonian_system.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/hamiltonian_system.pyx` & `unipolator-0.2.8/src/unipolator/hamiltonian_system.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/indexing.c` & `unipolator-0.2.8/src/unipolator/indexing.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/indexing.pxd` & `unipolator-0.2.8/src/unipolator/indexing.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/indexing.pyx` & `unipolator-0.2.8/src/unipolator/indexing.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/sym_trotter_system.c` & `unipolator-0.2.8/src/unipolator/sym_trotter_system.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/sym_trotter_system.pyx` & `unipolator-0.2.8/src/unipolator/sym_trotter_system.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/symmetric_unitary_interpolation.c` & `unipolator-0.2.8/src/unipolator/symmetric_unitary_interpolation.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/symmetric_unitary_interpolation.pyx` & `unipolator-0.2.8/src/unipolator/symmetric_unitary_interpolation.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/trotter_system.c` & `unipolator-0.2.8/src/unipolator/trotter_system.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/trotter_system.pyx` & `unipolator-0.2.8/src/unipolator/trotter_system.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/unitary_interpolation.c` & `unipolator-0.2.8/src/unipolator/unitary_interpolation.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator/unitary_interpolation.pyx` & `unipolator-0.2.8/src/unipolator/unitary_interpolation.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.7/src/unipolator.egg-info/PKG-INFO` & `unipolator-0.2.8/src/unipolator.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: unipolator
-Version: 0.2.7
+Version: 0.2.8
 Summary: Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.
 Home-page: https://github.com/Ntropic/unipolator
-Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.7.tar.gz
+Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.8.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `unipolator-0.2.7/src/unipolator.egg-info/SOURCES.txt` & `unipolator-0.2.8/src/unipolator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

