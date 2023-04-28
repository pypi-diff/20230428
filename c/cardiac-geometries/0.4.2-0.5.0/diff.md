# Comparing `tmp/cardiac_geometries-0.4.2.tar.gz` & `tmp/cardiac_geometries-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardiac_geometries-0.4.2.tar", last modified: Mon Mar 20 13:09:50 2023, max compression
+gzip compressed data, was "cardiac_geometries-0.5.0.tar", last modified: Fri Apr 28 11:20:48 2023, max compression
```

## Comparing `cardiac_geometries-0.4.2.tar` & `cardiac_geometries-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:09:50.637890 cardiac_geometries-0.4.2/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1082 2023-03-20 13:09:50.637890 cardiac_geometries-0.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1599 2023-03-20 13:09:50.637890 cardiac_geometries-0.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:09:50.617890 cardiac_geometries-0.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:09:50.625890 cardiac_geometries-0.4.2/src/cardiac_geometries/
--rw-r--r--   0 root         (0) root         (0)     1355 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:09:50.629890 cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     9594 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/_slab.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/utils.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_import_checks.py
--rw-r--r--   0 root         (0) root         (0)    14594 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:09:50.633890 cardiac_geometries-0.4.2/src/cardiac_geometries/_mshr/
--rw-r--r--   0 root         (0) root         (0)      260 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_mshr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_mshr/_biv.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_mshr/_lv.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/_mshr/_utils.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/calculus.py
--rw-r--r--   0 root         (0) root         (0)    13971 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/cli.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:09:50.633890 cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/
--rw-r--r--   0 root         (0) root         (0)      133 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     5490 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     4187 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/_slab.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/_utils.py
--rw-r--r--   0 root         (0) root         (0)    14224 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/geometry.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/utils.py
--rw-r--r--   0 root         (0) root         (0)     9972 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/src/cardiac_geometries/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:09:50.629890 cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-03-20 13:09:50.000000 cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2023-03-20 13:09:50.000000 cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 13:09:50.000000 cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-03-20 13:09:50.000000 cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 13:09:36.000000 cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      236 2023-03-20 13:09:50.000000 cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-20 13:09:50.000000 cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:09:50.633890 cardiac_geometries-0.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)     1510 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4372 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/tests/test_gmsh.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-03-20 13:09:34.000000 cardiac_geometries-0.4.2/tests/test_mshr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.743077 cardiac_geometries-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-28 11:20:48.743077 cardiac_geometries-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-28 11:20:48.743077 cardiac_geometries-0.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.731077 cardiac_geometries-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.735077 cardiac_geometries-0.5.0/src/cardiac_geometries/
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.739076 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/
+-rw-r--r--   0 root         (0) root         (0)      602 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10271 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/utils.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_import_checks.py
+-rw-r--r--   0 root         (0) root         (0)    21055 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.739076 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_biv.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_lv.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/calculus.py
+-rw-r--r--   0 root         (0) root         (0)    19505 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/dolfin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.739076 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     4187 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_utils.py
+-rw-r--r--   0 root         (0) root         (0)    14224 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9972 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.735077 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:20:36.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.743077 cardiac_geometries-0.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/tests/test_gmsh.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/tests/test_mshr.py
```

### Comparing `cardiac_geometries-0.4.2/LICENSE` & `cardiac_geometries-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/PKG-INFO` & `cardiac_geometries-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac_geometries
-Version: 0.4.2
+Version: 0.5.0
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.4.2/setup.cfg` & `cardiac_geometries-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardiac_geometries
-version = 0.4.2
+version = 0.5.0
 description = A python library for cardiac geometries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ComputationalPhysiology/cardiac_geometries
 author = Henrik Finsberg
 author_email = henriknf@simula.no
 license = MIT
```

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/__init__.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,29 @@
 
 if has_dolfin():
     from .dolfin_utils import gmsh2dolfin
     from .fibers import _slab as slab_fibers
     from .fibers import _lv_ellipsoid as lv_ellipsoid_fibers
     from .fibers import _biv_ellipsoid as biv_ellipsoid_fibers
     from . import _mesh as mesh
-    from ._mesh import create_biv_ellipsoid, create_lv_ellipsoid, create_slab
+    from ._mesh import (
+        create_biv_ellipsoid,
+        create_lv_ellipsoid,
+        create_slab,
+        create_biv_ellipsoid_torso,
+    )
 else:
     gmsh2dolfin = None  # type: ignore
     slab_fibers = None  # type: ignore
     lv_ellipsoid_fibers = None  # type:ignore
     biv_ellipsoid_fibers = None  # type: ignore
     create_biv_ellipsoid = None  # type: ignore
     create_lv_ellipsoid = None  # type: ignore
     create_slab = None  # type: ignore
+    create_biv_ellipsoid_torso = None  # type: ignore
 
 if has_mshr():
     from . import _mshr as mshr
 else:
     mshr = None  # type: ignore
 
 __all__ = [
@@ -43,11 +49,12 @@
     "mshr",
     "gmsh",
     "gmsh2dolfin",
     "slab_fibers",
     "lv_ellipsoid_fibers",
     "biv_ellipsoid_fibers",
     "create_biv_ellipsoid",
+    "create_biv_ellipsoid_torso",
     "create_lv_ellipsoid",
     "create_slab",
     "mesh",
 ]
```

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/__init__.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ._biv_ellipsoid import biv_ellipsoid
+from ._biv_ellipsoid import biv_ellipsoid_torso
 from ._lv_ellipsoid import create_benchmark_geometry_land15
 from ._lv_ellipsoid import lv_ellipsoid
 from ._lv_ellipsoid import lv_ellipsoid_flat_base
 from ._lv_ellipsoid import prolate_lv_ellipsoid
 from ._lv_ellipsoid import prolate_lv_ellipsoid_flat_base
 from ._slab import slab
 
@@ -11,8 +12,9 @@
     "lv_ellipsoid",
     "lv_ellipsoid_flat_base",
     "prolate_lv_ellipsoid_flat_base",
     "prolate_lv_ellipsoid",
     "create_benchmark_geometry_land15",
     "slab",
     "biv_ellipsoid",
+    "biv_ellipsoid_torso",
 ]
```

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/_gmsh/_slab.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/_import_checks.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/_import_checks.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/_mesh.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/_mesh.py`

 * *Files 12% similar despite different names*

```diff
@@ -188,14 +188,197 @@
 
     if _tmpfile is not None:
         _tmpfile.__exit__(None, None, None)
 
     return geo
 
 
+def create_biv_ellipsoid_torso(
+    outdir: Union[str, Path, None] = None,
+    char_length: float = 0.5,
+    torso_length: float = 20.0,
+    torso_width: float = 20.0,
+    torso_height: float = 20.0,
+    rotation_angle: float = math.pi / 6,
+    center_lv_y: float = 0.0,
+    a_endo_lv: float = 2.5,
+    b_endo_lv: float = 1.0,
+    c_endo_lv: float = 1.0,
+    a_epi_lv: float = 3.0,
+    b_epi_lv: float = 1.5,
+    c_epi_lv: float = 1.5,
+    center_rv_y: float = 0.5,
+    a_endo_rv: float = 3.0,
+    b_endo_rv: float = 1.5,
+    c_endo_rv: float = 1.5,
+    a_epi_rv: float = 4.0,
+    b_epi_rv: float = 2.5,
+    c_epi_rv: float = 2.0,
+    create_fibers: bool = False,
+    fiber_angle_endo: float = -60,
+    fiber_angle_epi: float = +60,
+    fiber_space: str = "P_1",
+) -> Optional[Geometry]:
+    """Create BiV ellipsoidal geometry
+
+    Parameters
+    ----------
+    outdir : Union[str, Path, None], optional
+        Directory where to save the results. If not provided a temporary
+        directory will be created, by default None, by default None
+    char_length : float, optional
+        Characteristic length of mesh, by default 0.5
+    torso_length : float, optional
+        Length of torso in the x-direction, by default 20.0
+    torso_width : float, optional
+        Length of torso in the y-direction, by default 20.0
+    torso_height : float, optional
+        Length of torso in the z-direction, by default 20.0
+    rotation_angle: float, optional
+        Angle to rotate the torso in order to object realistic position of
+        the heart in a torso, by default pi / 6
+    center_lv_y : float, optional
+        Y-coordinate for the center of the lv, by default 0.0
+    a_endo_lv : float, optional
+        Dilation of lv endo ellipsoid in the x-direction, by default 2.5
+    b_endo_lv : float, optional
+       Dilation of lv endo ellipsoid in the y-direction, by default 1.0
+    c_endo_lv : float, optional
+       Dilation of lv endo ellipsoid in the z-direction, by default 1.0
+    a_epi_lv : float, optional
+        Dilation of lv epi ellipsoid in the x-direction, by default 3.0
+    b_epi_lv : float, optional
+        Dilation of lv epi ellipsoid in the y-direction, by default 1.5
+    c_epi_lv : float, optional
+        Dilation of lv epi ellipsoid in the z-direction, by default 1.5
+    center_rv_y : float, optional
+        Y-coordinate for the center of the rv, by default 0.5
+    a_endo_rv : float, optional
+       Dilation of rv endo ellipsoid in the x-direction, by default 3.0
+    b_endo_rv : float, optional
+       Dilation of rv endo ellipsoid in the y-direction, by default 1.5
+    c_endo_rv : float, optional
+       Dilation of rv endo ellipsoid in the z-direction, by default 1.5
+    a_epi_rv : float, optional
+        Dilation of rv epi ellipsoid in the x-direction, by default 4.0
+    b_epi_rv : float, optional
+        Dilation of rv epi ellipsoid in the y-direction, by default 2.5
+    c_epi_rv : float, optional
+        Dilation of rv epi ellipsoid in the z-direction, by default 2.0
+    create_fibers : bool, optional
+        If True create analytic fibers, by default False
+    fiber_angle_endo : float, optional
+        Angle for the endocardium, by default -60
+    fiber_angle_epi : float, optional
+        Angle for the epicardium, by default +60
+    fiber_space : str, optional
+        Function space for fibers of the form family_degree, by default "P_1"
+
+    Returns
+    -------
+    Optional[Geometry]
+        A Geometry with the mesh, markers, markers functions and fibers.
+        Returns None if dolfin is not installed.
+
+    Raises
+    ------
+    ImportError
+        If gmsh is not installed
+    """
+    if not has_gmsh():
+        raise ImportError("Cannot create BiV ellipsoid. Gmsh is not installed")
+
+    _tmpfile = None
+    if outdir is None:
+        _tmpfile = tempfile.TemporaryDirectory()
+        outdir = _tmpfile.__enter__()
+
+    from ._gmsh import biv_ellipsoid_torso
+
+    outdir = Path(outdir)
+    outdir.mkdir(exist_ok=True, parents=True)
+
+    with open(outdir / "info.json", "w") as f:
+        json.dump(
+            {
+                "char_length": char_length,
+                "torso_length": torso_length,
+                "torso_width": torso_width,
+                "torso_height": torso_height,
+                "rotation_angle": rotation_angle,
+                "center_lv": (0.0, center_lv_y, 0.0),
+                "a_endo_lv": a_endo_lv,
+                "b_endo_lv": b_endo_lv,
+                "c_endo_lv": c_endo_lv,
+                "a_epi_lv": a_epi_lv,
+                "b_epi_lv": b_epi_lv,
+                "c_epi_lv": c_epi_lv,
+                "center_rv": (0.0, center_rv_y, 0.0),
+                "a_endo_rv": a_endo_rv,
+                "b_endo_rv": b_endo_rv,
+                "c_endo_rv": c_endo_rv,
+                "a_epi_rv": a_epi_rv,
+                "b_epi_rv": b_epi_rv,
+                "c_epi_rv": c_epi_rv,
+                "create_fibers": create_fibers,
+                "fibers_angle_endo": fiber_angle_endo,
+                "fibers_angle_epi": fiber_angle_epi,
+                "fiber_space": fiber_space,
+                "mesh_type": MeshTypes.biv_ellipsoid.value,
+                "cardiac_geometry_version": __version__,
+                "timestamp": datetime.datetime.now().isoformat(),
+            },
+            f,
+            indent=2,
+            default=json_serial,
+        )
+
+    mesh_name = outdir / "biv_ellipsoid_torso.msh"
+
+    biv_ellipsoid_torso(
+        mesh_name=mesh_name.as_posix(),
+        char_length=char_length,
+        torso_length=torso_length,
+        torso_height=torso_height,
+        torso_width=torso_width,
+        rotation_angle=rotation_angle,
+        center_lv=(0.0, center_lv_y, 0.0),
+        a_endo_lv=a_endo_lv,
+        b_endo_lv=b_endo_lv,
+        c_endo_lv=c_endo_lv,
+        a_epi_lv=a_epi_lv,
+        b_epi_lv=b_epi_lv,
+        c_epi_lv=c_epi_lv,
+        center_rv=(0.0, center_rv_y, 0.0),
+        a_endo_rv=a_endo_rv,
+        b_endo_rv=b_endo_rv,
+        c_endo_rv=c_endo_rv,
+        a_epi_rv=a_epi_rv,
+        b_epi_rv=b_epi_rv,
+        c_epi_rv=c_epi_rv,
+    )
+
+    if not has_dolfin():
+        return None
+
+    from .dolfin_utils import gmsh2dolfin
+
+    geometry = gmsh2dolfin(mesh_name, unlink=False)
+
+    with open(outdir / "markers.json", "w") as f:
+        json.dump(geometry.markers, f, default=json_serial)
+
+    geo = Geometry.from_folder(outdir)
+
+    if _tmpfile is not None:
+        _tmpfile.__exit__(None, None, None)
+
+    return geo
+
+
 def create_lv_ellipsoid(
     outdir: Optional[Union[Path, str]] = None,
     r_short_endo: float = 7.0,
     r_short_epi: float = 10.0,
     r_long_endo: float = 17.0,
     r_long_epi: float = 20.0,
     psize_ref: float = 3,
```

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/_mshr/_biv.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_biv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/_mshr/_lv.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_lv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/calculus.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/calculus.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/cli.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -365,14 +365,252 @@
         fiber_angle_epi=fiber_angle_epi,
         fiber_space=fiber_space,
     )
     if geo is not None:
         geo.save(outdir / "biv_ellipsoid.h5")
 
 
+@click.command(help="Create BiV ellipsoidal geometry embedded in a torso")
+@click.argument(
+    "outdir",
+    required=True,
+    type=click.Path(
+        file_okay=False,
+        dir_okay=True,
+        writable=True,
+        readable=True,
+        resolve_path=True,
+    ),
+)
+@click.option(
+    "--char-length",
+    default=0.5,
+    type=float,
+    help="Characteristic length of mesh",
+    show_default=True,
+)
+@click.option(
+    "--torso-length",
+    default=20,
+    type=float,
+    help="Length of torso in the x-direction",
+    show_default=True,
+)
+@click.option(
+    "--torso-width",
+    default=20,
+    type=float,
+    help="Length of torso in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--torso-height",
+    default=20,
+    type=float,
+    help="Length of torso in the z-direction",
+    show_default=True,
+)
+@click.option(
+    "--rotation-angle",
+    default=math.pi / 6,
+    type=float,
+    help=(
+        "Angle to rotate the torso in order to object realistic"
+        " position of the heart in a torso"
+    ),
+    show_default=True,
+)
+@click.option(
+    "--center-lv-y",
+    default=0.0,
+    type=float,
+    help="Y-coordinate for the center of the lv",
+    show_default=True,
+)
+@click.option(
+    "--a-endo-lv",
+    default=2.5,
+    type=float,
+    help="Dilation of lv endo ellipsoid in the x-direction",
+    show_default=True,
+)
+@click.option(
+    "--b-endo-lv",
+    default=1.0,
+    type=float,
+    help="Dilation of lv endo ellipsoid in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--c-endo-lv",
+    default=1.0,
+    type=float,
+    help="Dilation of lv endo ellipsoid in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--a-epi-lv",
+    default=3.0,
+    type=float,
+    help="Dilation of lv epi ellipsoid in the x-direction",
+    show_default=True,
+)
+@click.option(
+    "--b-epi-lv",
+    default=1.5,
+    type=float,
+    help="Dilation of lv epi ellipsoid in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--c-epi-lv",
+    default=1.5,
+    type=float,
+    help="Dilation of lv epi ellipsoid in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--center-rv-y",
+    default=0.5,
+    type=float,
+    help="Y-coordinate for the center of the rv",
+    show_default=True,
+)
+@click.option(
+    "--a-endo-rv",
+    default=3.0,
+    type=float,
+    help="Dilation of rv endo ellipsoid in the x-direction",
+    show_default=True,
+)
+@click.option(
+    "--b-endo-rv",
+    default=1.5,
+    type=float,
+    help="Dilation of rv endo ellipsoid in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--c-endo-rv",
+    default=1.5,
+    type=float,
+    help="Dilation of rv endo ellipsoid in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--a-epi-rv",
+    default=4.0,
+    type=float,
+    help="Dilation of rv epi ellipsoid in the x-direction",
+    show_default=True,
+)
+@click.option(
+    "--b-epi-rv",
+    default=2.5,
+    type=float,
+    help="Dilation of rv epi ellipsoid in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--c-epi-rv",
+    default=2.0,
+    type=float,
+    help="Dilation of rv epi ellipsoid in the z-direction",
+    show_default=True,
+)
+@click.option(
+    "--create-fibers",
+    default=False,
+    is_flag=True,
+    type=bool,
+    help="If True create analytic fibers",
+    show_default=True,
+)
+@click.option(
+    "--fiber-angle-endo",
+    default=-60,
+    type=float,
+    help="Angle for the endocardium",
+    show_default=True,
+)
+@click.option(
+    "--fiber-angle-epi",
+    default=+60,
+    type=float,
+    help="Angle for the epicardium",
+    show_default=True,
+)
+@click.option(
+    "--fiber-space",
+    default="P_1",
+    type=str,
+    help="Function space for fibers of the form family_degree",
+    show_default=True,
+)
+def create_biv_ellipsoid_torso(
+    outdir: Path,
+    char_length: float = 0.5,
+    torso_length: float = 20.0,
+    torso_width: float = 20.0,
+    torso_height: float = 20.0,
+    rotation_angle: float = math.pi / 6,
+    center_lv_y: float = 0.0,
+    a_endo_lv: float = 2.5,
+    b_endo_lv: float = 1.0,
+    c_endo_lv: float = 1.0,
+    a_epi_lv: float = 3.0,
+    b_epi_lv: float = 1.5,
+    c_epi_lv: float = 1.5,
+    center_rv_y: float = 0.5,
+    a_endo_rv: float = 3.0,
+    b_endo_rv: float = 1.5,
+    c_endo_rv: float = 1.5,
+    a_epi_rv: float = 4.0,
+    b_epi_rv: float = 2.5,
+    c_epi_rv: float = 2.0,
+    create_fibers: bool = False,
+    fiber_angle_endo: float = -60,
+    fiber_angle_epi: float = +60,
+    fiber_space: str = "P_1",
+):
+    outdir = Path(outdir)
+    outdir.mkdir(exist_ok=True)
+
+    from ._mesh import create_biv_ellipsoid_torso
+
+    geo = create_biv_ellipsoid_torso(
+        outdir=outdir,
+        char_length=char_length,
+        torso_length=torso_length,
+        torso_height=torso_height,
+        torso_width=torso_width,
+        rotation_angle=rotation_angle,
+        center_lv_y=center_lv_y,
+        a_endo_lv=a_endo_lv,
+        b_endo_lv=b_endo_lv,
+        c_endo_lv=c_endo_lv,
+        a_epi_lv=a_epi_lv,
+        b_epi_lv=b_epi_lv,
+        c_epi_lv=c_epi_lv,
+        center_rv_y=center_rv_y,
+        a_endo_rv=a_endo_rv,
+        b_endo_rv=b_endo_rv,
+        c_endo_rv=c_endo_rv,
+        a_epi_rv=a_epi_rv,
+        b_epi_rv=b_epi_rv,
+        c_epi_rv=c_epi_rv,
+        create_fibers=create_fibers,
+        fiber_angle_endo=fiber_angle_endo,
+        fiber_angle_epi=fiber_angle_epi,
+        fiber_space=fiber_space,
+    )
+    if geo is not None:
+        geo.save(outdir / "biv_ellipsoid_torso.h5")
+
+
 @click.command()
 @click.argument(
     "outdir",
     required=True,
     type=click.Path(
         file_okay=False,
         dir_okay=True,
@@ -445,15 +683,14 @@
     lz: float = 3.0,
     dx: float = 1.0,
     create_fibers: bool = True,
     fiber_angle_endo: float = -60,
     fiber_angle_epi: float = +60,
     fiber_space: str = "P_1",
 ):
-
     outdir = Path(outdir)
     outdir.mkdir(exist_ok=True)
 
     from ._mesh import create_slab
 
     geo = create_slab(
         outdir=outdir,
@@ -490,15 +727,14 @@
     "--base-direction",
     default="+z",
     type=str,
     help="Direction pointing towards the base. One of +x,-x,+y,-y,+z,-z",
     show_default=True,
 )
 def fibers_to_xdmf(folder, base_direction: str):
-
     outdir = Path(folder)
     tetra_mesh_name = outdir / "mesh.xdmf"
     microstructure_path = outdir / "microstructure.h5"
 
     import dolfin
     from dolfin import FiniteElement  # noqa: F401
     from dolfin import tetrahedron  # noqa: F401
@@ -574,15 +810,14 @@
         resolve_path=True,
     ),
 )
 def info(
     mesh_path: Union[str, Path],
     schema_path: Optional[Union[str, Path]] = None,
 ) -> None:
-
     if not has_dolfin():
         msg = "Cannot get info - dolfin is not installed"
         raise ImportError(msg)
 
     from .geometry import Geometry
 
     geo = Geometry.from_file(mesh_path, schema_path=schema_path)
@@ -600,11 +835,12 @@
 
     console = Console()
     console.print(table)
 
 
 app.add_command(create_lv_ellipsoid)
 app.add_command(create_biv_ellipsoid)
+app.add_command(create_biv_ellipsoid_torso)
 app.add_command(create_slab)
 app.add_command(fibers_to_xdmf)
 app.add_command(folder2h5)
 app.add_command(info)
```

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/dolfin_utils.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/dolfin_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 
 def gmsh2dolfin(
     msh_file: typing.Union[Path, str],
     outdir: typing.Optional[typing.Union[Path, str]] = None,
     unlink: bool = False,
 ) -> Geometry:
-
     msh = meshio.gmsh.read(msh_file)
     if outdir is None:
         outdir = Path(msh_file).absolute().parent
     else:
         outdir = Path(outdir)
 
     outdir.mkdir(exist_ok=True, parents=True)
@@ -120,15 +119,15 @@
     read_meshfunction(vertex_mesh_name, vfun_val)
     vfun = dolfin.MeshFunction("size_t", mesh, vfun_val)
     vfun.array()[vfun.array() == max(vfun.array())] = 0
     if unlink:
         vertex_mesh_name.unlink(missing_ok=True)
         vertex_mesh_name.with_suffix(".h5").unlink(missing_ok=True)
 
-    markers = {k: [int(vi) for vi in v] for k, v in msh.field_data.items()}
+    markers = {k: (int(v[0]), int(v[1])) for k, v in msh.field_data.items()}
     marker_functions = MarkerFunctions(vfun=vfun, efun=efun, ffun=ffun, cfun=cfun)
 
     geo = Geometry(
         mesh=mesh,
         markers=markers,
         marker_functions=marker_functions,
     )
@@ -141,15 +140,14 @@
     region number in a meshfunction
     """
 
     if foc is None:
         foc = calculus.estimate_focal_point(mesh)
 
     for cell in dolfin.cells(mesh):
-
         # Get coordinates to cell midpoint
         x = cell.midpoint().x()
         y = cell.midpoint().y()
         z = cell.midpoint().z()
 
         T = calculus.cartesian_to_prolate_ellipsoidal(x, y, z, foc)
```

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/_biv_ellipsoid.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/_lv_ellipsoid.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/_slab.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/fibers/_utils.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/geometry.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/geometry.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries/viz.py` & `cardiac_geometries-0.5.0/src/cardiac_geometries/viz.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/PKG-INFO` & `cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac-geometries
-Version: 0.4.2
+Version: 0.5.0
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.4.2/src/cardiac_geometries.egg-info/SOURCES.txt` & `cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/tests/test_cli.py` & `cardiac_geometries-0.5.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 
 from cardiac_geometries import cli
 from cardiac_geometries.geometry import Geometry
 from click.testing import CliRunner
 
 
 def test_create_slab(tmp_path: Path):
-
     runner = CliRunner()
     res1 = runner.invoke(cli.create_slab, ["--create-fibers", tmp_path.as_posix()])
     assert res1.exit_code == 0
     outfile = tmp_path / "geo.h5"
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
 def test_create_lv_ellipsoid(tmp_path: Path):
-
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_lv_ellipsoid,
         ["--create-fibers", tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
     outfile = tmp_path / "geo.h5"
@@ -31,20 +29,34 @@
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
 def test_create_biv_ellipsoid(tmp_path: Path):
-
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_biv_ellipsoid,
         ["--create-fibers", tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
     outfile = tmp_path / "geo.h5"
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
+
+
+def test_create_biv_ellipsoid_torso(tmp_path: Path):
+    runner = CliRunner()
+    res1 = runner.invoke(
+        cli.create_biv_ellipsoid_torso,
+        [tmp_path.as_posix()],
+    )
+    assert res1.exit_code == 0
+    outfile = tmp_path / "geo.h5"
+    res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
+    assert res2.exit_code == 0
+    assert outfile.is_file()
+    geo = Geometry.from_file(outfile)
+    assert geo.mesh is not None
```

### Comparing `cardiac_geometries-0.4.2/tests/test_geometry.py` & `cardiac_geometries-0.5.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.4.2/tests/test_gmsh.py` & `cardiac_geometries-0.5.0/tests/test_gmsh.py`

 * *Files identical despite different names*

