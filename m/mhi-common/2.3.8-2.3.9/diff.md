# Comparing `tmp/mhi_common-2.3.8-py3-none-any.whl.zip` & `tmp/mhi_common-2.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 39508 bytes, number of entries: 19
--rw-rw-rw-  2.0 fat      538 b- defN 23-Feb-16 21:09 mhi/common/__init__.py
+Zip file size: 40585 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat      538 b- defN 23-Mar-24 19:27 mhi/common/__init__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 21-Aug-20 15:09 mhi/common/__main__.py
 -rw-rw-rw-  2.0 fat     3681 b- defN 22-Oct-06 21:42 mhi/common/_script.py
 -rw-rw-rw-  2.0 fat     2943 b- defN 21-Aug-20 15:09 mhi/common/arrow.py
 -rw-rw-rw-  2.0 fat      903 b- defN 21-Aug-20 15:09 mhi/common/cdata.py
 -rw-rw-rw-  2.0 fat    10743 b- defN 21-Aug-20 15:09 mhi/common/codec.py
 -rw-rw-rw-  2.0 fat     2211 b- defN 21-Oct-27 19:00 mhi/common/collection.py
 -rw-rw-rw-  2.0 fat    32864 b- defN 21-Aug-20 15:09 mhi/common/colour.py
 -rw-rw-rw-  2.0 fat     2208 b- defN 21-Aug-20 15:09 mhi/common/config.py
 -rw-rw-rw-  2.0 fat     6859 b- defN 23-Jan-04 21:52 mhi/common/path.py
--rw-rw-rw-  2.0 fat    19369 b- defN 23-Jan-19 15:51 mhi/common/process.py
--rw-rw-rw-  2.0 fat    26252 b- defN 23-Feb-16 21:08 mhi/common/remote.py
+-rw-rw-rw-  2.0 fat    19492 b- defN 23-Mar-24 19:27 mhi/common/process.py
+-rw-rw-rw-  2.0 fat    26602 b- defN 23-Mar-24 19:27 mhi/common/remote.py
 -rw-rw-rw-  2.0 fat    22352 b- defN 22-Oct-06 21:44 mhi/common/server.py
+-rw-rw-rw-  2.0 fat     2790 b- defN 23-Mar-24 19:27 mhi/common/version.py
 -rw-rw-rw-  2.0 fat    11270 b- defN 22-Oct-06 21:44 mhi/common/zipper.py
--rw-rw-rw-  2.0 fat     1731 b- defN 23-Feb-16 21:25 mhi_common-2.3.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1315 b- defN 23-Feb-16 21:25 mhi_common-2.3.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-16 21:25 mhi_common-2.3.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Feb-16 21:25 mhi_common-2.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1486 b- defN 23-Feb-16 21:25 mhi_common-2.3.8.dist-info/RECORD
-19 files, 146986 bytes uncompressed, 37124 bytes compressed:  74.7%
+-rw-rw-rw-  2.0 fat     1731 b- defN 23-Mar-24 19:31 mhi_common-2.3.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1315 b- defN 23-Mar-24 19:31 mhi_common-2.3.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-24 19:31 mhi_common-2.3.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-24 19:31 mhi_common-2.3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1564 b- defN 23-Mar-24 19:31 mhi_common-2.3.9.dist-info/RECORD
+20 files, 150327 bytes uncompressed, 38083 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -33,26 +33,29 @@
 
 Filename: mhi/common/remote.py
 Comment: 
 
 Filename: mhi/common/server.py
 Comment: 
 
+Filename: mhi/common/version.py
+Comment: 
+
 Filename: mhi/common/zipper.py
 Comment: 
 
-Filename: mhi_common-2.3.8.dist-info/LICENSE
+Filename: mhi_common-2.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: mhi_common-2.3.8.dist-info/METADATA
+Filename: mhi_common-2.3.9.dist-info/METADATA
 Comment: 
 
-Filename: mhi_common-2.3.8.dist-info/WHEEL
+Filename: mhi_common-2.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: mhi_common-2.3.8.dist-info/top_level.txt
+Filename: mhi_common-2.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mhi_common-2.3.8.dist-info/RECORD
+Filename: mhi_common-2.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mhi/common/__init__.py

```diff
@@ -2,16 +2,16 @@
 The `mhi.common` library is a package of common functions, which facilitate
 the automation of various MHI applications from Python scripts.
 
 This package is not intended to be used directly.  It will be used
 internally by the application specific packages.
 """
 
-VERSION = '2.3.8'
-VERSION_HEX = 0x020308f0
+VERSION = '2.3.9'
+VERSION_HEX = 0x020309f0
 
 __all__ = [] # type: ignore
 
 def version_msg():
     """
     Common Library Version Message
     """
```

## mhi/common/process.py

```diff
@@ -5,15 +5,15 @@
 """
 
 #===============================================================================
 # Imports
 #===============================================================================
 
 import logging, os, subprocess, random
-from packaging.version import Version
+from .version import Version, InvalidVersion
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple
 
 # Pywin32
 from winreg import EnumKey as _EnumKey
 from winreg import OpenKey as _OpenKey, CloseKey as _CloseKey
 from winreg import QueryValueEx as _QueryValueEx
 from winreg import HKEY_LOCAL_MACHINE as _HKLM, KEY_READ as _KEY_READ
@@ -437,48 +437,46 @@
 
     # Select the 32 or 64 bit dictionaries, or merge the two dictionaries
     if x64 is not None:
         filtered = versions64 if x64 else versions32
     else:
         filtered = dict(versions32, **versions64)
 
-    # Filter
-    if not allow_alpha:
-        filtered = {ver:filtered[ver] for ver in filtered if ver != 'Alpha'}
+    # If Alpha and/or Beta versions are allowed and are present, use them.
+    if allow_alpha and 'Alpha' in filtered:
+        return filtered['Alpha']
 
-    if not allow_beta:
-        filtered = {ver:filtered[ver] for ver in filtered if ver != 'Beta'}
+    if allow_beta and 'Beta' in filtered:
+        return filtered['Beta']
 
+    # Filter out any non-standard versions (Alpha, Beta, Free, ...)
+    filtered = {ver: filtered[ver] for ver in filtered if Version.valid(ver)}
+
+    # Filter any versions outside minimum/maximum limits
     if minimum:
         limit = Version(minimum)
-        filtered = {ver:filtered[ver] for ver in filtered
-                    if ver.isalpha() or Version(ver) >= limit}
+        filtered = {ver: filtered[ver] for ver in filtered
+                    if Version(ver) >= limit}
 
     if maximum:
         limit = Version(maximum)
-        filtered = {ver:filtered[ver] for ver in filtered
-                    if ver.isalpha() or Version(ver) <= limit}
+        filtered = {ver: filtered[ver] for ver in filtered
+                    if Version(ver) <= limit}
 
 
     # If an explicit version is not given, select the latest version
     # (starting with Alpha)
     if version is None:
-        if 'Alpha' in filtered:
-            version = 'Alpha'
-        elif 'Beta' in filtered:
-            version = 'Beta'
-        else:
-            version = max(filtered, default=None, key=Version)
-            if version is None:
-                return None
+        version = max(filtered, default=None, key=Version)
+        if version is None:
+            return None
 
     return filtered.get(version, None)
 
 
-
 def launch(*args: str, options: Dict[str, Any] = None, **kwargs):
 
     """
     Launch an application process.
 
     All ``{keyword}`` format codes in the list of ``args`` strings are
     replaced by the value in the corresponding ``options`` dictionary and/or
@@ -563,9 +561,10 @@
 #===============================================================================
 
 if __name__ == '__main__':
 
     # Show executables for known apps, but it is ok if they aren't installed.
     for app in ('PSCAD', 'Enerplot'):
         print(app, "=", find_exe(app))
-    for app in ('PSCAD', 'Enerplot'):
-        print(app, "=", find_exe(app, allow_alpha=False, allow_beta=False))
+    for app, minimum in {'PSCAD': '5.0', 'Enerplot': '1.1.0'}.items():
+        print(app, "=", find_exe(app, minimum=minimum,
+                                 allow_alpha=False, allow_beta=False))
```

## mhi/common/remote.py

```diff
@@ -2,15 +2,15 @@
 """
 Remote method invocation from Python scripts to MHI application entities.
 """
 
 import sys, queue, pickle, io, importlib, time, warnings, socket, threading
 from typing import Any, Dict, Optional, Union, Tuple, TYPE_CHECKING
 from functools import wraps
-from packaging.version import Version
+from .version import Version
 
 
 #===============================================================================
 # Window constants
 #===============================================================================
 
 _WSAEOPNOTSUPP = 10045
@@ -290,28 +290,28 @@
                 #
                 # application.close_connection() is automatically called
                 # when the `with` statement block exits.
         """
 
 
     def close_connection(self) -> None:
-
         """
         Terminate connection to remote application.
 
         Note: The remote application will not be terminated.
         The "silence all dialog and message boxes" flag is cleared.
         """
 
         self.silence = False
         self._context.close()
 
     #-----------------------------------------------------------------------
     # Version Attribute
     #-----------------------------------------------------------------------
+
     @property
     def version(self) -> str:
         """Application Version"""
         raise NotImplementedError()
 
 
     #-----------------------------------------------------------------------
@@ -358,14 +358,25 @@
 
         if not self.minimum_version(version):
             msg = "{} requires application version >= {}".format(msg, version)
             raise NotImplementedError(msg)
 
 
     #-----------------------------------------------------------------------
+    # Embedded
+    #-----------------------------------------------------------------------
+
+    @property
+    def is_embedded(self) -> bool:
+        """Return whether an internal Python environment is being used"""
+
+        return Context._EMBEDDED_SERVER is not None
+
+
+    #-----------------------------------------------------------------------
     # Server Address
     #-----------------------------------------------------------------------
 
     def server_address(self) -> Tuple[str, int]:
         """
         Return the host/port address for the application server, which
         may be used to open additional connections to the application.
```

## Comparing `mhi_common-2.3.8.dist-info/LICENSE` & `mhi_common-2.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mhi_common-2.3.8.dist-info/METADATA` & `mhi_common-2.3.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhi-common
-Version: 2.3.8
+Version: 2.3.9
 Summary: Manitoba Hydro International: Common library
 Home-page: https://www.pscad.com/support/support-resources
 Author: Manitoba Hydro International Ltd.
 Author-email: pscad@mhi.ca
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mhi_common-2.3.8.dist-info/RECORD` & `mhi_common-2.3.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-mhi/common/__init__.py,sha256=P-ifwKaWeYQJ82gATLzPWPA8wyGCbDkmCKv2LMEnRRo,538
+mhi/common/__init__.py,sha256=CZO1JVVAQymldEvHfrBd9VfudE_onXl9PNyjm7Mit4M,538
 mhi/common/__main__.py,sha256=rImejOfTZ6c3usWV0LXoTLLmQATa2Fy9NqDaf0Er1vY,165
 mhi/common/_script.py,sha256=xXYQW9dL_ogGx5SZUWP_ZGQrP3eJgLyk82AKcYxqaGU,3681
 mhi/common/arrow.py,sha256=JEQQbF22ftye3Z7pryW6TpggUg1JCGgZw0BUgrhDCp8,2943
 mhi/common/cdata.py,sha256=l9oilnooVO2Kos5tF467cWMLgMy9BJ1Z9CBLyhYK90U,903
 mhi/common/codec.py,sha256=-6oYaHKIQKJBs-N6ctzjKFqMGntIuVBoCnY62dW4Fyg,10743
 mhi/common/collection.py,sha256=LFpBnqe2kftTUGZhrIcsu78vDRchY3flE-VO5abse10,2211
 mhi/common/colour.py,sha256=O6BrPNPQ1VDx3SuLntA1py5cQNEHeNj1ns7GELYyq_g,32864
 mhi/common/config.py,sha256=zmn-Yx0r9jgGuOc5-t3ZvmmWq8AaEWpDhHMwAoOyMy4,2208
 mhi/common/path.py,sha256=EKvRkmvctdJFqPY0leuXeNLthe8NRt_PKlA61R7GKuU,6859
-mhi/common/process.py,sha256=G8G_MA1F_RpdD6EooLnd1crvFPEscz0wNpZqV7Bhuhs,19369
-mhi/common/remote.py,sha256=SOdAeGxwW-WDXXoEP5whxO6cOIkYr1K2zRDtQif6Qf4,26252
+mhi/common/process.py,sha256=_xIVeKuXheCi9Unp3Rcf68mUGO2reY7EPMf2u4wOYlg,19492
+mhi/common/remote.py,sha256=YqCk6ITLk-bI8gU-vDC6rwmO0yRtu_NMqLJ83btGGIU,26602
 mhi/common/server.py,sha256=YE7xhxyjMREOApiN5aERkFKVlEYMhJpnVzb5H2K9FD0,22352
+mhi/common/version.py,sha256=l8k0XPpSdxUv0VwW1U8KDVfCSMMf0_PWmFM31sqmlHY,2790
 mhi/common/zipper.py,sha256=01o6O-J9dB9gfNJPnumxPfJBiYWLvLP7ZWz2kauGyPc,11270
-mhi_common-2.3.8.dist-info/LICENSE,sha256=yBd9wB7h5dagNwtLo1wdlPsEbb1CN90p3ONFg8g4Q3U,1731
-mhi_common-2.3.8.dist-info/METADATA,sha256=9-2byqxhk1fYj_zvr_APmBeGJVnlLsEaJZd9Wf0VUvk,1315
-mhi_common-2.3.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mhi_common-2.3.8.dist-info/top_level.txt,sha256=K3uum2bvGx0puBc2JFddiJZoY9hBCdmM9bCy5Qg9-aw,4
-mhi_common-2.3.8.dist-info/RECORD,,
+mhi_common-2.3.9.dist-info/LICENSE,sha256=yBd9wB7h5dagNwtLo1wdlPsEbb1CN90p3ONFg8g4Q3U,1731
+mhi_common-2.3.9.dist-info/METADATA,sha256=DaX0pMXlm7vQRJcMDJQRe3RsXL5_CtSUnDOKke1b8OA,1315
+mhi_common-2.3.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mhi_common-2.3.9.dist-info/top_level.txt,sha256=K3uum2bvGx0puBc2JFddiJZoY9hBCdmM9bCy5Qg9-aw,4
+mhi_common-2.3.9.dist-info/RECORD,,
```

