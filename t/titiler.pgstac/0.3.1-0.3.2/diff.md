# Comparing `tmp/titiler.pgstac-0.3.1.tar.gz` & `tmp/titiler.pgstac-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.pgstac-0.3.1.tar", last modified: Fri Dec 16 21:08:40 2022, max compression
+gzip compressed data, was "titiler.pgstac-0.3.2.tar", last modified: Tue Mar 14 13:51:44 2023, max compression
```

## Comparing `titiler.pgstac-0.3.1.tar` & `titiler.pgstac-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 21:08:40.889657 titiler.pgstac-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2022-12-16 21:08:40.889657 titiler.pgstac-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 21:08:40.889657 titiler.pgstac-0.3.1/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/benchmark/create_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      537 2022-12-16 21:08:40.893657 titiler.pgstac-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 21:08:40.889657 titiler.pgstac-0.3.1/titiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 21:08:40.889657 titiler.pgstac-0.3.1/titiler/pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    39815 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2022-12-16 21:08:32.000000 titiler.pgstac-0.3.1/titiler/pgstac/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 21:08:40.889657 titiler.pgstac-0.3.1/titiler.pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2022-12-16 21:08:40.000000 titiler.pgstac-0.3.1/titiler.pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-12-16 21:08:40.000000 titiler.pgstac-0.3.1/titiler.pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 21:08:40.000000 titiler.pgstac-0.3.1/titiler.pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 21:08:40.000000 titiler.pgstac-0.3.1/titiler.pgstac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-16 21:08:40.000000 titiler.pgstac-0.3.1/titiler.pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-16 21:08:40.000000 titiler.pgstac-0.3.1/titiler.pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:51:44.737725 titiler.pgstac-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-03-14 13:51:44.737725 titiler.pgstac-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:51:44.733725 titiler.pgstac-0.3.2/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/benchmark/create_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-14 13:51:44.737725 titiler.pgstac-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:51:44.733725 titiler.pgstac-0.3.2/titiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:51:44.737725 titiler.pgstac-0.3.2/titiler/pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39815 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-03-14 13:51:33.000000 titiler.pgstac-0.3.2/titiler/pgstac/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:51:44.733725 titiler.pgstac-0.3.2/titiler.pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-03-14 13:51:44.000000 titiler.pgstac-0.3.2/titiler.pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-14 13:51:44.000000 titiler.pgstac-0.3.2/titiler.pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 13:51:44.000000 titiler.pgstac-0.3.2/titiler.pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 13:51:44.000000 titiler.pgstac-0.3.2/titiler.pgstac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-14 13:51:44.000000 titiler.pgstac-0.3.2/titiler.pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-14 13:51:44.000000 titiler.pgstac-0.3.2/titiler.pgstac.egg-info/top_level.txt
```

### Comparing `titiler.pgstac-0.3.1/LICENSE` & `titiler.pgstac-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/PKG-INFO` & `titiler.pgstac-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.pgstac
-Version: 0.3.1
+Version: 0.3.2
 Summary: Connect PgSTAC and TiTiler
 Home-page: https://github.com/stac-utils/titiler-pgstac
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: COG STAC MosaicJSON FastAPI PgSTAC
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.3.1 Summary: Connect
+Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.3.2 Summary: Connect
 PgSTAC and TiTiler Home-page: https://github.com/stac-utils/titiler-pgstac
 Author: Vincent Sarago Author-email: vincent@developmentseed.org License: MIT
 Keywords: COG STAC MosaicJSON FastAPI PgSTAC Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `titiler.pgstac-0.3.1/README.md` & `titiler.pgstac-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/benchmark/create_urls.py` & `titiler.pgstac-0.3.2/benchmark/create_urls.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/setup.cfg` & `titiler.pgstac-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/setup.py` & `titiler.pgstac-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 inst_reqs = [
-    "titiler.core>=0.10.1,<0.11",
-    "titiler.mosaic>=0.10.1,<0.11",
+    "titiler.core>=0.10.2,<0.11",
+    "titiler.mosaic>=0.10.2,<0.11",
     "geojson-pydantic>=0.4,<0.5",
     "stac-pydantic==2.0.*",
+    "fastapi>=0.87,<0.92",
+    "starlette>=0.21.0,<0.25",
 ]
 extra_reqs = {
     "dev": ["pre-commit"],
     "test": [
         "pytest",
         "pytest-cov",
         "pytest-asyncio",
```

### Comparing `titiler.pgstac-0.3.1/titiler/pgstac/db.py` & `titiler.pgstac-0.3.2/titiler/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/titiler/pgstac/dependencies.py` & `titiler.pgstac-0.3.2/titiler/pgstac/dependencies.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/titiler/pgstac/factory.py` & `titiler.pgstac-0.3.2/titiler/pgstac/factory.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/titiler/pgstac/main.py` & `titiler.pgstac-0.3.2/titiler/pgstac/main.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/titiler/pgstac/model.py` & `titiler.pgstac-0.3.2/titiler/pgstac/model.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/titiler/pgstac/mosaic.py` & `titiler.pgstac-0.3.2/titiler/pgstac/mosaic.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/titiler/pgstac/reader.py` & `titiler.pgstac-0.3.2/titiler/pgstac/reader.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/titiler/pgstac/settings.py` & `titiler.pgstac-0.3.2/titiler/pgstac/settings.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.1/titiler.pgstac.egg-info/PKG-INFO` & `titiler.pgstac-0.3.2/titiler.pgstac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.pgstac
-Version: 0.3.1
+Version: 0.3.2
 Summary: Connect PgSTAC and TiTiler
 Home-page: https://github.com/stac-utils/titiler-pgstac
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: COG STAC MosaicJSON FastAPI PgSTAC
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.3.1 Summary: Connect
+Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.3.2 Summary: Connect
 PgSTAC and TiTiler Home-page: https://github.com/stac-utils/titiler-pgstac
 Author: Vincent Sarago Author-email: vincent@developmentseed.org License: MIT
 Keywords: COG STAC MosaicJSON FastAPI PgSTAC Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `titiler.pgstac-0.3.1/titiler.pgstac.egg-info/SOURCES.txt` & `titiler.pgstac-0.3.2/titiler.pgstac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

