# Comparing `tmp/coppyr-0.9.1.tar.gz` & `tmp/coppyr-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coppyr-0.9.1.tar", last modified: Tue Apr 25 15:37:40 2023, max compression
+gzip compressed data, was "coppyr-0.9.2.tar", last modified: Fri Apr 28 16:52:27 2023, max compression
```

## Comparing `coppyr-0.9.1.tar` & `coppyr-0.9.2.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.898836 coppyr-0.9.1/
--rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-24 19:48:14.000000 coppyr-0.9.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       83 2023-04-24 21:42:08.000000 coppyr-0.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4983 2023-04-25 15:37:40.898836 coppyr-0.9.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4266 2023-04-24 21:55:15.000000 coppyr-0.9.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.894836 coppyr-0.9.1/coppyr/
--rw-rw-r--   0 root         (0) root         (0)      476 2023-04-25 15:37:32.000000 coppyr-0.9.1/coppyr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.898836 coppyr-0.9.1/coppyr/collections/
--rw-rw-r--   0 root         (0) root         (0)       78 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/collections/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1091 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/collections/cycle.py
--rw-rw-r--   0 root         (0) root         (0)      705 2023-04-24 20:00:23.000000 coppyr-0.9.1/coppyr/collections/dotdict.py
--rw-rw-r--   0 root         (0) root         (0)     1431 2023-04-24 19:55:39.000000 coppyr-0.9.1/coppyr/concurrent.py
--rw-rw-r--   0 root         (0) root         (0)     1164 2023-04-25 02:55:52.000000 coppyr-0.9.1/coppyr/config.py
--rw-rw-r--   0 root         (0) root         (0)     4059 2023-04-24 19:54:46.000000 coppyr-0.9.1/coppyr/context.py
--rw-rw-r--   0 root         (0) root         (0)     2316 2023-04-24 19:56:41.000000 coppyr-0.9.1/coppyr/daemon.py
--rw-rw-r--   0 root         (0) root         (0)     1645 2023-04-24 19:57:04.000000 coppyr-0.9.1/coppyr/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.898836 coppyr-0.9.1/coppyr/extensions/
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/extensions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3152 2023-04-24 20:41:07.000000 coppyr-0.9.1/coppyr/extensions/load.py
--rw-rw-r--   0 root         (0) root         (0)      351 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/lazyproperty.py
--rw-rw-r--   0 root         (0) root         (0)     4735 2023-04-24 19:57:57.000000 coppyr-0.9.1/coppyr/logger.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2023-04-25 15:19:57.000000 coppyr-0.9.1/coppyr/package.py
--rw-rw-r--   0 root         (0) root         (0)    10912 2023-04-24 19:58:31.000000 coppyr-0.9.1/coppyr/parallel.py
--rw-rw-r--   0 root         (0) root         (0)     1163 2023-04-24 19:54:28.000000 coppyr-0.9.1/coppyr/singleton.py
--rw-rw-r--   0 root         (0) root         (0)     3482 2023-04-24 19:59:29.000000 coppyr-0.9.1/coppyr/subp.py
--rw-rw-r--   0 root         (0) root         (0)      389 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/testing.py
--rw-rw-r--   0 root         (0) root         (0)     1028 2023-04-24 20:44:01.000000 coppyr-0.9.1/coppyr/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.898836 coppyr-0.9.1/coppyr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4983 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-25 15:25:17.000000 coppyr-0.9.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 15:37:40.898836 coppyr-0.9.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1285 2023-04-25 15:26:56.000000 coppyr-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.066432 coppyr-0.9.2/
+-rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-24 19:48:14.000000 coppyr-0.9.2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       83 2023-04-24 21:42:08.000000 coppyr-0.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-04-28 16:52:27.066432 coppyr-0.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4266 2023-04-24 21:55:15.000000 coppyr-0.9.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.062432 coppyr-0.9.2/coppyr/
+-rw-rw-r--   0 root         (0) root         (0)      437 2023-04-28 16:48:36.000000 coppyr-0.9.2/coppyr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.062432 coppyr-0.9.2/coppyr/collections/
+-rw-rw-r--   0 root         (0) root         (0)       78 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/collections/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1091 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/collections/cycle.py
+-rw-rw-r--   0 root         (0) root         (0)      856 2023-04-28 16:36:15.000000 coppyr-0.9.2/coppyr/collections/dotdict.py
+-rw-rw-r--   0 root         (0) root         (0)     1871 2023-04-28 16:28:29.000000 coppyr-0.9.2/coppyr/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4319 2023-04-28 16:07:28.000000 coppyr-0.9.2/coppyr/context.py
+-rw-rw-r--   0 root         (0) root         (0)     2316 2023-04-24 19:56:41.000000 coppyr-0.9.2/coppyr/daemon.py
+-rw-rw-r--   0 root         (0) root         (0)     1645 2023-04-24 19:57:04.000000 coppyr-0.9.2/coppyr/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.062432 coppyr-0.9.2/coppyr/extensions/
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/extensions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3152 2023-04-24 20:41:07.000000 coppyr-0.9.2/coppyr/extensions/load.py
+-rw-rw-r--   0 root         (0) root         (0)     4735 2023-04-24 19:57:57.000000 coppyr-0.9.2/coppyr/logger.py
+-rw-rw-r--   0 root         (0) root         (0)     2428 2023-04-25 15:19:57.000000 coppyr-0.9.2/coppyr/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.066432 coppyr-0.9.2/coppyr/process/
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-04-27 19:30:48.000000 coppyr-0.9.2/coppyr/process/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1431 2023-04-24 19:55:39.000000 coppyr-0.9.2/coppyr/process/concurrent.py
+-rw-rw-r--   0 root         (0) root         (0)    10912 2023-04-24 19:58:31.000000 coppyr-0.9.2/coppyr/process/parallel.py
+-rw-rw-r--   0 root         (0) root         (0)     3482 2023-04-24 19:59:29.000000 coppyr-0.9.2/coppyr/process/subp.py
+-rw-rw-r--   0 root         (0) root         (0)      389 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.066432 coppyr-0.9.2/coppyr/types/
+-rw-rw-r--   0 root         (0) root         (0)      179 2023-04-27 21:29:25.000000 coppyr-0.9.2/coppyr/types/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3569 2023-04-27 23:05:32.000000 coppyr-0.9.2/coppyr/types/differ.py
+-rw-rw-r--   0 root         (0) root         (0)      351 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/types/lazyproperty.py
+-rw-rw-r--   0 root         (0) root         (0)     1187 2023-04-27 19:30:58.000000 coppyr-0.9.2/coppyr/types/singleton.py
+-rw-rw-r--   0 root         (0) root         (0)      763 2023-04-27 19:56:36.000000 coppyr-0.9.2/coppyr/types/slot.py
+-rw-rw-r--   0 root         (0) root         (0)     1028 2023-04-24 20:44:01.000000 coppyr-0.9.2/coppyr/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.062432 coppyr-0.9.2/coppyr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      732 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-25 15:25:17.000000 coppyr-0.9.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 16:52:27.066432 coppyr-0.9.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1285 2023-04-25 15:26:56.000000 coppyr-0.9.2/setup.py
```

### Comparing `coppyr-0.9.1/LICENSE` & `coppyr-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/PKG-INFO` & `coppyr-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coppyr
-Version: 0.9.1
+Version: 0.9.2
 Summary: A collection of boilerplate for Python applications.
 Home-page: https://github.com/gshulegaard/coppyr
 Author: Grant Hulegaard
 Author-email: loki.labrys@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `coppyr-0.9.1/README.rst` & `coppyr-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/collections/cycle.py` & `coppyr-0.9.2/coppyr/collections/cycle.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/collections/dotdict.py` & `coppyr-0.9.2/coppyr/collections/dotdict.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,23 @@
 
         # recursively cast dicts to DotDicts that may have been set by init
         for k, v in self.items():
             if isinstance(v, dict):
                 self[k] = DotDict(**v)
 
     def __getattr__(self, k):
+        if k.startswith("__"):
+            return super().__getattr__(k)
+
         return super().get(k)
 
     def __setattr__(self, k, v):
+        if k.startswith("__"):
+            return super().__setattr__(k, v)
+
         super().__setitem__(k, v)
 
     def __delattr__(self, k):
         super().__delitem__(k)
 
     def __setitem__(self, k, v):
         # support recursive dot spec
```

### Comparing `coppyr-0.9.1/coppyr/concurrent.py` & `coppyr-0.9.2/coppyr/process/concurrent.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/context.py` & `coppyr-0.9.2/coppyr/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
-import binascii
 import os
 import sys
 import time
 
 from typing import Optional
 
-from coppyr.lazyproperty import lazyproperty
+from coppyr.types import lazyproperty, Singleton, Namespace
 from coppyr.collections import cycle, DotDict
-from coppyr.singleton import Singleton, Namespace
 
 
 # TODO: These sys variables should really be applied elsewhere.
 sys.tracebacklimit = 10000
 sys.setrecursionlimit(2048)
 
 
@@ -86,23 +84,38 @@
     def app_name_env(self):
         return self.app_name.replace("-", "_")\
                             .replace(".", "__")\
                             .upper()
 
     @lazyproperty
     def ident(self):
+        import binascii
         random_hex = binascii.b2a_hex(os.urandom(4)).decode()
         return random_hex
 
     @lazyproperty
+    def uuid(self):
+        import uuid
+        return uuid.uuid4()
+
+    @lazyproperty
+    def host_id(self):
+        import uuid
+        import platform
+
+        return uuid.uuid5(
+            uuid.NAMESPACE_DNS, platform.node() + str(uuid.getnode())
+        ).hex
+
+    @lazyproperty
     def cwd(self):
         return os.getcwd()
 
     def inc_action_id(self):
-        self.action_id = f"{self.pid}_{next(self.ids)}"  # increment action_id
+        self.action_id = f"{self.ident}_{next(self.ids)}"  # increment action_id
         self.action_stamp = time.time()  # reset start time for new action
 
     @property
     def action_duration(self):
         return time.time() - self.action_stamp
 
     @property
```

### Comparing `coppyr-0.9.1/coppyr/daemon.py` & `coppyr-0.9.2/coppyr/daemon.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/error.py` & `coppyr-0.9.2/coppyr/error.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/extensions/load.py` & `coppyr-0.9.2/coppyr/extensions/load.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/logger.py` & `coppyr-0.9.2/coppyr/logger.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/package.py` & `coppyr-0.9.2/coppyr/package.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/parallel.py` & `coppyr-0.9.2/coppyr/process/parallel.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/singleton.py` & `coppyr-0.9.2/coppyr/types/singleton.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 from coppyr.collections import DotDict
 
 
 class Singleton(object):
     """
     This object will only ever create one instance of itself in (interpreter
     local) memory.  Future constructions will just return the previously
```

### Comparing `coppyr-0.9.1/coppyr/subp.py` & `coppyr-0.9.2/coppyr/process/subp.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr/web.py` & `coppyr-0.9.2/coppyr/web.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.1/coppyr.egg-info/PKG-INFO` & `coppyr-0.9.2/coppyr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coppyr
-Version: 0.9.1
+Version: 0.9.2
 Summary: A collection of boilerplate for Python applications.
 Home-page: https://github.com/gshulegaard/coppyr
 Author: Grant Hulegaard
 Author-email: loki.labrys@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `coppyr-0.9.1/setup.py` & `coppyr-0.9.2/setup.py`

 * *Files identical despite different names*

