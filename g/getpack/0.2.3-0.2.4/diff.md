# Comparing `tmp/getpack-0.2.3.tar.gz` & `tmp/getpack-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpack-0.2.3.tar", last modified: Mon Apr  3 00:23:08 2023, max compression
+gzip compressed data, was "getpack-0.2.4.tar", last modified: Fri Apr 28 00:04:39 2023, max compression
```

## Comparing `getpack-0.2.3.tar` & `getpack-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 00:23:08.326466 getpack-0.2.3/
--rw-rw-rw-   0        0        0       37 2023-02-16 21:01:44.000000 getpack-0.2.3/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-03 00:23:08.263014 getpack-0.2.3/.vscode/
--rw-rw-rw-   0        0        0      186 2022-11-26 18:28:38.000000 getpack-0.2.3/.vscode/cspell.json
--rw-rw-rw-   0        0        0      494 2022-11-26 18:28:38.000000 getpack-0.2.3/.vscode/launch.json
--rw-rw-rw-   0        0        0      500 2022-11-26 18:28:38.000000 getpack-0.2.3/.vscode/settings.json
--rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     2504 2023-04-03 00:23:08.327464 getpack-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1535 2023-02-17 09:18:11.000000 getpack-0.2.3/README.md
--rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      951 2023-04-03 00:23:08.330271 getpack-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 00:23:08.237165 getpack-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-03 00:23:08.268013 getpack-0.2.3/src/getpack/
--rw-rw-rw-   0        0        0      403 2023-04-03 00:19:17.000000 getpack-0.2.3/src/getpack/__init__.py
--rw-rw-rw-   0        0        0     1867 2023-03-31 19:09:34.000000 getpack-0.2.3/src/getpack/executable.py
-drwxrwxrwx   0        0        0        0 2023-04-03 00:23:08.322456 getpack-0.2.3/src/getpack/library/
--rw-rw-rw-   0        0        0     2486 2023-04-03 00:18:28.000000 getpack-0.2.3/src/getpack/library/__init__.py
--rw-rw-rw-   0        0        0      449 2023-04-03 00:13:44.000000 getpack-0.2.3/src/getpack/library/ffmpeg.py
--rw-rw-rw-   0        0        0    10634 2023-03-21 16:49:59.000000 getpack-0.2.3/src/getpack/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-03 00:23:08.318690 getpack-0.2.3/src/getpack.egg-info/
--rw-rw-rw-   0        0        0     2504 2023-04-03 00:23:08.000000 getpack-0.2.3/src/getpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-04-03 00:23:08.000000 getpack-0.2.3/src/getpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 00:23:08.000000 getpack-0.2.3/src/getpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-04-03 00:23:08.000000 getpack-0.2.3/src/getpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-03 00:23:08.000000 getpack-0.2.3/src/getpack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 00:23:08.325465 getpack-0.2.3/tests/
--rw-rw-rw-   0        0        0     1219 2023-04-03 00:18:56.000000 getpack-0.2.3/tests/test_common.py
--rw-rw-rw-   0        0        0      426 2023-03-31 19:43:17.000000 getpack-0.2.3/tests/test_executable.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.436935 getpack-0.2.4/
+-rw-rw-rw-   0        0        0       37 2023-02-16 21:01:44.000000 getpack-0.2.4/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.360936 getpack-0.2.4/.vscode/
+-rw-rw-rw-   0        0        0      186 2022-11-26 18:28:38.000000 getpack-0.2.4/.vscode/cspell.json
+-rw-rw-rw-   0        0        0      534 2023-04-27 21:31:59.000000 getpack-0.2.4/.vscode/launch.json
+-rw-rw-rw-   0        0        0      500 2022-11-26 18:28:38.000000 getpack-0.2.4/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2504 2023-04-28 00:04:39.437935 getpack-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1535 2023-02-17 09:18:11.000000 getpack-0.2.4/README.md
+-rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0      967 2023-04-28 00:04:39.447938 getpack-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.339940 getpack-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.379936 getpack-0.2.4/src/getpack/
+-rw-rw-rw-   0        0        0      403 2023-04-27 21:46:03.000000 getpack-0.2.4/src/getpack/__init__.py
+-rw-rw-rw-   0        0        0     2492 2023-04-27 23:53:20.000000 getpack-0.2.4/src/getpack/executable.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.427935 getpack-0.2.4/src/getpack/library/
+-rw-rw-rw-   0        0        0     2486 2023-04-03 00:18:28.000000 getpack-0.2.4/src/getpack/library/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-04-03 00:13:44.000000 getpack-0.2.4/src/getpack/library/ffmpeg.py
+-rw-rw-rw-   0        0        0    11596 2023-04-27 23:46:55.000000 getpack-0.2.4/src/getpack/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.423936 getpack-0.2.4/src/getpack.egg-info/
+-rw-rw-rw-   0        0        0     2504 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.435937 getpack-0.2.4/tests/
+-rw-rw-rw-   0        0        0     1219 2023-04-28 00:04:00.000000 getpack-0.2.4/tests/test_common.py
+-rw-rw-rw-   0        0        0      954 2023-04-27 22:47:06.000000 getpack-0.2.4/tests/test_concurrency.py
+-rw-rw-rw-   0        0        0      426 2023-03-31 19:43:17.000000 getpack-0.2.4/tests/test_executable.py
+-rw-rw-rw-   0        0        0      496 2023-04-03 00:10:25.000000 getpack-0.2.4/tests/test_unicode.py
```

### Comparing `getpack-0.2.3/LICENSE` & `getpack-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getpack-0.2.3/PKG-INFO` & `getpack-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpack
-Version: 0.2.3
+Version: 0.2.4
 Summary: Declarative external resources with implicit deployment
 Home-page: https://github.com/kalemas/getpack
 Author: Konstantin Maslyuk
 Author-email: Kostya.Maslyuk@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
 Description: ### Declarative external resources any with implicit deployment
```

### Comparing `getpack-0.2.3/README.md` & `getpack-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `getpack-0.2.3/setup.cfg` & `getpack-0.2.4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -40,21 +40,22 @@
 00000270: 0a09 3d73 7263 0d0a 7061 636b 6167 6573  ..=src..packages
 00000280: 203d 2066 696e 643a 0d0a 696e 7374 616c   = find:..instal
 00000290: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
 000002a0: 7061 7468 6c69 623b 2070 7974 686f 6e5f  pathlib; python_
 000002b0: 7665 7273 696f 6e3c 2233 220d 0a09 7369  version<"3"...si
 000002c0: 780d 0a09 7479 7069 6e67 3b20 7079 7468  x...typing; pyth
 000002d0: 6f6e 5f76 6572 7369 6f6e 3c22 3322 0d0a  on_version<"3"..
-000002e0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000002f0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000300: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-00000310: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
-00000320: 655d 0d0a 6465 7620 3d20 0d0a 0966 6c61  e]..dev = ...fla
-00000330: 6b65 380d 0a09 666c 616b 6538 2d69 6d70  ke8...flake8-imp
-00000340: 6f72 742d 6f72 6465 720d 0a09 6d79 7079  ort-order...mypy
-00000350: 0d0a 0970 7974 6573 740d 0a09 7961 7066  ...pytest...yapf
-00000360: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 696d  ....[flake8]..im
-00000370: 706f 7274 2d6f 7264 6572 2d73 7479 6c65  port-order-style
-00000380: 203d 2067 6f6f 676c 650d 0a0d 0a5b 6567   = google....[eg
-00000390: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000003a0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000003b0: 3d20 300d 0a0d 0a                        = 0....
+000002e0: 0970 6f72 7461 6c6f 636b 6572 3c32 0d0a  .portalocker<2..
+000002f0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000300: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+00000310: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
+00000320: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
+00000330: 655d 0d0a 6465 7620 3d20 0d0a 0966 6c61  e]..dev = ...fla
+00000340: 6b65 380d 0a09 666c 616b 6538 2d69 6d70  ke8...flake8-imp
+00000350: 6f72 742d 6f72 6465 720d 0a09 6d79 7079  ort-order...mypy
+00000360: 0d0a 0970 7974 6573 740d 0a09 7961 7066  ...pytest...yapf
+00000370: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 696d  ....[flake8]..im
+00000380: 706f 7274 2d6f 7264 6572 2d73 7479 6c65  port-order-style
+00000390: 203d 2067 6f6f 676c 650d 0a0d 0a5b 6567   = google....[eg
+000003a0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000003b0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000003c0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `getpack-0.2.3/src/getpack/library/__init__.py` & `getpack-0.2.4/src/getpack/library/__init__.py`

 * *Files identical despite different names*

### Comparing `getpack-0.2.3/src/getpack/resource.py` & `getpack-0.2.4/src/getpack/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,55 @@
 import os
 from pathlib import Path
 import random
 import re
 import shutil
 import sys
 import tarfile
+import threading
 import typing
 import zipfile
 
+import portalocker
 from six.moves import urllib
 
 
+__FILE_LOCK_TIMEOUT__ = 15 * 60
+
+
+class HybridLock:
+    def __init__(self, key):
+        self.key = key.as_posix() + '.portalock'
+        self.file_lock = portalocker.RLock(
+                self.key,
+                timeout=__FILE_LOCK_TIMEOUT__,
+                mode='w',
+            )
+        self.lock = threading.RLock()
+
+    def __enter__(self):
+        self.lock.acquire()
+        self.file_lock.acquire()
+
+    def __exit__(self, *_):
+        self.file_lock.release()
+        self.lock.release()
+        try:
+            os.unlink(self.key)
+        except Exception:
+            pass
+
+
+def lock(key, _locks={None: threading.Lock()}):
+    with _locks[None]:
+        if key not in _locks:
+            _locks[key] = HybridLock(key)
+    return _locks[key]
+
+
 def _logging(*args):
     print(args[0] % args[1:])
 
 
 def _logging_off(*args):
     pass
 
@@ -69,19 +104,20 @@
 
     def provide(self):
         """Make resource available so it would be immediately used."""
         if self._available:
             return
         assert self.name, 'Resource should be named'
         assert self.version, 'Resource should be versioned'
-        if self.version in self.get_available_versions():
+        with lock(self.path):
+            if self.version in self.get_available_versions():
+                self._available = True
+                return
+            self.deploy()
             self._available = True
-            return
-        self.deploy()
-        self._available = True
 
     def __call__(self):
         self.provide()
         return self
 
     def cleanup(self):
         raise NotImplementedError
@@ -133,17 +169,19 @@
             temp_path.rename(self.path)
         except Exception:
             if temp_path and temp_path.is_dir():
                 shutil.rmtree(str(temp_path))
             raise
 
     def cleanup(self):
-        if self.path.is_dir():
-            info('Cleanup %s', self.path)
-            shutil.rmtree(str(self.path))
+        with lock(self.path):
+            if self.path.is_dir():
+                info('Cleanup %s', self.path)
+                shutil.rmtree(str(self.path))
+            self._available = False
 
 
 class ArchiveExtractor:
     def __init__(self, stream):
         self.stream = stream
 
     def __enter__(self):
```

### Comparing `getpack-0.2.3/src/getpack.egg-info/PKG-INFO` & `getpack-0.2.4/src/getpack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpack
-Version: 0.2.3
+Version: 0.2.4
 Summary: Declarative external resources with implicit deployment
 Home-page: https://github.com/kalemas/getpack
 Author: Konstantin Maslyuk
 Author-email: Kostya.Maslyuk@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
 Description: ### Declarative external resources any with implicit deployment
```

### Comparing `getpack-0.2.3/tests/test_common.py` & `getpack-0.2.4/tests/test_common.py`

 * *Files identical despite different names*

