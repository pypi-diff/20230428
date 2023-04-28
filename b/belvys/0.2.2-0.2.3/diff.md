# Comparing `tmp/belvys-0.2.2.tar.gz` & `tmp/belvys-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "belvys-0.2.2.tar", last modified: Fri Apr 28 16:39:04 2023, max compression
+gzip compressed data, was "belvys-0.2.3.tar", last modified: Fri Apr 28 17:13:04 2023, max compression
```

## Comparing `belvys-0.2.2.tar` & `belvys-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:39:04.143180 belvys-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-28 16:38:52.000000 belvys-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 16:38:52.000000 belvys-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 16:39:04.143180 belvys-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 16:38:52.000000 belvys-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:39:04.143180 belvys-0.2.2/belvys/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 16:39:04.143180 belvys-0.2.2/belvys/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/example_api_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/example_api_complex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/example_structure_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/example_structure_complex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-28 16:38:52.000000 belvys-0.2.2/belvys/tenant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:39:04.143180 belvys-0.2.2/belvys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 16:39:04.000000 belvys-0.2.2/belvys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 16:39:04.000000 belvys-0.2.2/belvys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 16:39:04.000000 belvys-0.2.2/belvys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 16:39:03.000000 belvys-0.2.2/belvys.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 16:39:04.000000 belvys-0.2.2/belvys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 16:39:04.000000 belvys-0.2.2/belvys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 16:38:52.000000 belvys-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 16:39:04.143180 belvys-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 16:38:52.000000 belvys-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:39:04.143180 belvys-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-28 16:38:52.000000 belvys-0.2.2/tests/test_liveconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-28 16:38:52.000000 belvys-0.2.2/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    81464 2023-04-28 16:38:52.000000 belvys-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:04.043545 belvys-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-28 17:12:53.000000 belvys-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 17:12:53.000000 belvys-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 17:13:04.043545 belvys-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 17:12:53.000000 belvys-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:04.043545 belvys-0.2.3/belvys/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:13:04.043545 belvys-0.2.3/belvys/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example_api_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example_api_complex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example_structure_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example_structure_complex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/tenant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:04.043545 belvys-0.2.3/belvys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:13:03.000000 belvys-0.2.3/belvys.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 17:12:53.000000 belvys-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 17:13:04.043545 belvys-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 17:12:53.000000 belvys-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:04.043545 belvys-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-28 17:12:53.000000 belvys-0.2.3/tests/test_liveconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-28 17:12:53.000000 belvys-0.2.3/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81464 2023-04-28 17:12:53.000000 belvys-0.2.3/versioneer.py
```

### Comparing `belvys-0.2.2/LICENSE` & `belvys-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/PKG-INFO` & `belvys-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvys
-Version: 0.2.2
+Version: 0.2.3
 Summary: Getting timeseries data from Belvis Rest API.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Belvys
```

### Comparing `belvys-0.2.2/README.rst` & `belvys-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/belvys/adjustment.py` & `belvys-0.2.3/belvys/adjustment.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/belvys/api.py` & `belvys-0.2.3/belvys/api.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/belvys/example.py` & `belvys-0.2.3/belvys/example.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/belvys/example_api_complex.yaml` & `belvys-0.2.3/belvys/example_api_complex.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/belvys/example_structure_basic.yaml` & `belvys-0.2.3/belvys/example_structure_basic.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/belvys/example_structure_complex.yaml` & `belvys-0.2.3/belvys/example_structure_complex.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/belvys/structure.py` & `belvys-0.2.3/belvys/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         tsname = tsname_tree
         return [Ts(pfid, tsname)]
     elif isinstance(tsname_tree, Iterable):
         tsnames = tsname_tree
         return [Ts(pfid, tsname) for tsname in tsnames]
 
 
-@dataclass
+@dataclass(frozen=True)
 class Portfolios:
     original: Iterable[str]
     synthetic: Dict[str, Union[str, Iterable[str]]] = field(default_factory=dict)
 
     def __post_init__(self):
         # Assert that the class doesn't have missing refences.
         if not isinstance(self.original, Iterable):
```

### Comparing `belvys-0.2.2/belvys/tenant.py` & `belvys-0.2.3/belvys/tenant.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/belvys.egg-info/PKG-INFO` & `belvys-0.2.3/belvys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvys
-Version: 0.2.2
+Version: 0.2.3
 Summary: Getting timeseries data from Belvis Rest API.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Belvys
```

### Comparing `belvys-0.2.2/belvys.egg-info/SOURCES.txt` & `belvys-0.2.3/belvys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/setup.py` & `belvys-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/tests/test_liveconnection.py` & `belvys-0.2.3/tests/test_liveconnection.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/tests/test_structure.py` & `belvys-0.2.3/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.2/versioneer.py` & `belvys-0.2.3/versioneer.py`

 * *Files identical despite different names*

