# Comparing `tmp/sdss_cherno-0.6.1.tar.gz` & `tmp/sdss_cherno-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_cherno-0.6.1.tar", max compression
+gzip compressed data, was "sdss_cherno-0.6.2.tar", max compression
```

## Comparing `sdss_cherno-0.6.1.tar` & `sdss_cherno-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1504 2023-04-27 15:49:06.932924 sdss_cherno-0.6.1/LICENSE.md
--rw-r--r--   0        0        0     2723 2023-04-27 15:49:06.933270 sdss_cherno-0.6.1/README.md
--rw-r--r--   0        0        0     1251 2023-04-27 15:49:06.933672 sdss_cherno-0.6.1/cherno/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-27 15:49:06.934006 sdss_cherno-0.6.1/cherno/__main__.py
--rw-r--r--   0        0        0      747 2023-04-27 15:49:06.934389 sdss_cherno-0.6.1/cherno/actor/__init__.py
--rw-r--r--   0        0        0     4493 2023-04-27 15:49:06.934860 sdss_cherno-0.6.1/cherno/actor/actor.py
--rw-r--r--   0        0        0        0 2023-04-27 15:49:06.935084 sdss_cherno-0.6.1/cherno/actor/commands/__init__.py
--rw-r--r--   0        0        0     1746 2023-04-27 15:49:06.935760 sdss_cherno-0.6.1/cherno/actor/commands/acquire.py
--rw-r--r--   0        0        0     4938 2023-04-27 15:49:06.936996 sdss_cherno-0.6.1/cherno/actor/commands/config.py
--rw-r--r--   0        0        0     8213 2023-04-27 15:49:06.937407 sdss_cherno-0.6.1/cherno/actor/commands/guide.py
--rw-r--r--   0        0        0     1273 2023-04-27 15:49:06.937813 sdss_cherno-0.6.1/cherno/actor/commands/offset.py
--rw-r--r--   0        0        0     1007 2023-04-27 15:49:06.938943 sdss_cherno-0.6.1/cherno/actor/commands/reprocess.py
--rw-r--r--   0        0        0     2298 2023-04-27 15:49:06.939411 sdss_cherno-0.6.1/cherno/actor/commands/scale.py
--rw-r--r--   0        0        0     3119 2023-04-27 15:49:06.939872 sdss_cherno-0.6.1/cherno/actor/commands/set.py
--rw-r--r--   0        0        0     1049 2023-04-27 15:49:06.940241 sdss_cherno-0.6.1/cherno/actor/commands/show.py
--rw-r--r--   0        0        0     1964 2023-04-27 15:49:06.940894 sdss_cherno-0.6.1/cherno/actor/commands/status.py
--rw-r--r--   0        0        0      778 2023-04-27 15:49:06.941407 sdss_cherno-0.6.1/cherno/actor/commands/stop.py
--rw-r--r--   0        0        0     1148 2023-04-27 15:49:06.941771 sdss_cherno-0.6.1/cherno/actor/commands/version.py
--rw-r--r--   0        0        0    10857 2023-04-27 15:49:06.942168 sdss_cherno-0.6.1/cherno/actor/exposer.py
--rw-r--r--   0        0        0       73 2023-04-27 15:49:06.942579 sdss_cherno-0.6.1/cherno/etc/astrometrynet_APO.cfg
--rw-r--r--   0        0        0       73 2023-04-27 15:49:06.942896 sdss_cherno-0.6.1/cherno/etc/astrometrynet_LCO.cfg
--rw-r--r--   0        0        0     1994 2023-04-27 15:49:06.943266 sdss_cherno-0.6.1/cherno/etc/cherno_APO.yml
--rw-r--r--   0        0        0     1958 2023-04-27 15:49:06.943603 sdss_cherno-0.6.1/cherno/etc/cherno_LCO.yml
--rw-r--r--   0        0        0     5688 2023-04-27 15:49:06.943938 sdss_cherno-0.6.1/cherno/etc/schema.json
--rw-r--r--   0        0        0     1233 2023-04-27 15:49:06.944428 sdss_cherno-0.6.1/cherno/exceptions.py
--rw-r--r--   0        0        0    14028 2023-04-27 15:49:06.945028 sdss_cherno-0.6.1/cherno/extraction.py
--rw-r--r--   0        0        0    40346 2023-04-27 15:49:06.945681 sdss_cherno-0.6.1/cherno/guider.py
--rw-r--r--   0        0        0     4175 2023-04-27 15:49:06.946143 sdss_cherno-0.6.1/cherno/lcotcc.py
--rw-r--r--   0        0        0     1394 2023-04-27 15:49:06.946554 sdss_cherno-0.6.1/cherno/maskbits.py
--rw-r--r--   0        0        0     4738 2023-04-27 15:49:06.946970 sdss_cherno-0.6.1/cherno/tcc.py
--rw-r--r--   0        0        0     6237 2023-04-27 15:49:06.947512 sdss_cherno-0.6.1/cherno/utils.py
--rw-r--r--   0        0        0     2314 2023-04-27 15:49:06.957729 sdss_cherno-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 sdss_cherno-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-28 18:04:40.338639 sdss_cherno-0.6.2/LICENSE.md
+-rw-r--r--   0        0        0     2723 2023-04-28 18:04:40.339034 sdss_cherno-0.6.2/README.md
+-rw-r--r--   0        0        0     1251 2023-04-28 18:04:40.339429 sdss_cherno-0.6.2/cherno/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-28 18:04:40.339759 sdss_cherno-0.6.2/cherno/__main__.py
+-rw-r--r--   0        0        0      747 2023-04-28 18:04:40.340146 sdss_cherno-0.6.2/cherno/actor/__init__.py
+-rw-r--r--   0        0        0     4493 2023-04-28 18:04:40.340499 sdss_cherno-0.6.2/cherno/actor/actor.py
+-rw-r--r--   0        0        0        0 2023-04-28 18:04:40.340708 sdss_cherno-0.6.2/cherno/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1746 2023-04-28 18:04:40.341112 sdss_cherno-0.6.2/cherno/actor/commands/acquire.py
+-rw-r--r--   0        0        0     4938 2023-04-28 18:04:40.341605 sdss_cherno-0.6.2/cherno/actor/commands/config.py
+-rw-r--r--   0        0        0     8213 2023-04-28 18:04:40.342068 sdss_cherno-0.6.2/cherno/actor/commands/guide.py
+-rw-r--r--   0        0        0     1273 2023-04-28 18:04:40.342558 sdss_cherno-0.6.2/cherno/actor/commands/offset.py
+-rw-r--r--   0        0        0     1007 2023-04-28 18:04:40.343170 sdss_cherno-0.6.2/cherno/actor/commands/reprocess.py
+-rw-r--r--   0        0        0     2298 2023-04-28 18:04:40.343621 sdss_cherno-0.6.2/cherno/actor/commands/scale.py
+-rw-r--r--   0        0        0     3119 2023-04-28 18:04:40.344119 sdss_cherno-0.6.2/cherno/actor/commands/set.py
+-rw-r--r--   0        0        0     1049 2023-04-28 18:04:40.344473 sdss_cherno-0.6.2/cherno/actor/commands/show.py
+-rw-r--r--   0        0        0     1964 2023-04-28 18:04:40.344830 sdss_cherno-0.6.2/cherno/actor/commands/status.py
+-rw-r--r--   0        0        0      778 2023-04-28 18:04:40.345393 sdss_cherno-0.6.2/cherno/actor/commands/stop.py
+-rw-r--r--   0        0        0     1148 2023-04-28 18:04:40.345836 sdss_cherno-0.6.2/cherno/actor/commands/version.py
+-rw-r--r--   0        0        0    10857 2023-04-28 18:04:40.346392 sdss_cherno-0.6.2/cherno/actor/exposer.py
+-rw-r--r--   0        0        0       73 2023-04-28 18:04:40.346871 sdss_cherno-0.6.2/cherno/etc/astrometrynet_APO.cfg
+-rw-r--r--   0        0        0       73 2023-04-28 18:04:40.347215 sdss_cherno-0.6.2/cherno/etc/astrometrynet_LCO.cfg
+-rw-r--r--   0        0        0     1994 2023-04-28 18:04:40.347555 sdss_cherno-0.6.2/cherno/etc/cherno_APO.yml
+-rw-r--r--   0        0        0     1958 2023-04-28 18:04:40.347909 sdss_cherno-0.6.2/cherno/etc/cherno_LCO.yml
+-rw-r--r--   0        0        0     5688 2023-04-28 18:04:40.348383 sdss_cherno-0.6.2/cherno/etc/schema.json
+-rw-r--r--   0        0        0     1233 2023-04-28 18:04:40.348845 sdss_cherno-0.6.2/cherno/exceptions.py
+-rw-r--r--   0        0        0    14028 2023-04-28 18:04:40.349269 sdss_cherno-0.6.2/cherno/extraction.py
+-rw-r--r--   0        0        0    40346 2023-04-28 18:04:40.349909 sdss_cherno-0.6.2/cherno/guider.py
+-rw-r--r--   0        0        0     4175 2023-04-28 18:04:40.350366 sdss_cherno-0.6.2/cherno/lcotcc.py
+-rw-r--r--   0        0        0     1394 2023-04-28 18:04:40.350707 sdss_cherno-0.6.2/cherno/maskbits.py
+-rw-r--r--   0        0        0     4738 2023-04-28 18:04:40.351065 sdss_cherno-0.6.2/cherno/tcc.py
+-rw-r--r--   0        0        0     6237 2023-04-28 18:04:40.351435 sdss_cherno-0.6.2/cherno/utils.py
+-rw-r--r--   0        0        0     2314 2023-04-28 18:04:40.360969 sdss_cherno-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 sdss_cherno-0.6.2/PKG-INFO
```

### Comparing `sdss_cherno-0.6.1/LICENSE.md` & `sdss_cherno-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/README.md` & `sdss_cherno-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/__init__.py` & `sdss_cherno-0.6.2/cherno/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/__main__.py` & `sdss_cherno-0.6.2/cherno/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/__init__.py` & `sdss_cherno-0.6.2/cherno/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/actor.py` & `sdss_cherno-0.6.2/cherno/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/acquire.py` & `sdss_cherno-0.6.2/cherno/actor/commands/acquire.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/config.py` & `sdss_cherno-0.6.2/cherno/actor/commands/config.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/guide.py` & `sdss_cherno-0.6.2/cherno/actor/commands/guide.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/offset.py` & `sdss_cherno-0.6.2/cherno/actor/commands/offset.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/reprocess.py` & `sdss_cherno-0.6.2/cherno/actor/commands/reprocess.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/scale.py` & `sdss_cherno-0.6.2/cherno/actor/commands/scale.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/set.py` & `sdss_cherno-0.6.2/cherno/actor/commands/set.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/show.py` & `sdss_cherno-0.6.2/cherno/actor/commands/show.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/status.py` & `sdss_cherno-0.6.2/cherno/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/stop.py` & `sdss_cherno-0.6.2/cherno/actor/commands/stop.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/commands/version.py` & `sdss_cherno-0.6.2/cherno/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/actor/exposer.py` & `sdss_cherno-0.6.2/cherno/actor/exposer.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/etc/cherno_APO.yml` & `sdss_cherno-0.6.2/cherno/etc/cherno_APO.yml`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/etc/cherno_LCO.yml` & `sdss_cherno-0.6.2/cherno/etc/cherno_LCO.yml`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/etc/schema.json` & `sdss_cherno-0.6.2/cherno/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/exceptions.py` & `sdss_cherno-0.6.2/cherno/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/extraction.py` & `sdss_cherno-0.6.2/cherno/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/guider.py` & `sdss_cherno-0.6.2/cherno/guider.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/lcotcc.py` & `sdss_cherno-0.6.2/cherno/lcotcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/maskbits.py` & `sdss_cherno-0.6.2/cherno/maskbits.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/tcc.py` & `sdss_cherno-0.6.2/cherno/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/cherno/utils.py` & `sdss_cherno-0.6.2/cherno/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.1/pyproject.toml` & `sdss_cherno-0.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-cherno"
-version = "0.6.1"
+version = "0.6.2"
 description = "SDSS guider actor"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/cherno"
 repository = "https://github.com/sdss/cherno"
 documentation = "https://sdss-cherno.readthedocs.org"
@@ -28,15 +28,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 sdsstools = "^1.0.0"
 sdss-clu = "^1.8.0"
 astropy = "^5.0.0"
 click-default-group = "^1.2.2"
-sdss-coordio = "^1.7.2"
+sdss-coordio = "^1.7.3"
 pandas = "^1.3.4"
 tables = ">=3.6.1"
 simple-pid = "^1.0.1"
 sqlalchemy = "^1.4.45"
 psycopg2-binary = "^2.9.5"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `sdss_cherno-0.6.1/PKG-INFO` & `sdss_cherno-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-cherno
-Version: 0.6.1
+Version: 0.6.2
 Summary: SDSS guider actor
 Home-page: https://github.com/sdss/cherno
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.9,<3.12
@@ -21,15 +21,15 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: astropy (>=5.0.0,<6.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: sdss-clu (>=1.8.0,<2.0.0)
-Requires-Dist: sdss-coordio (>=1.7.2,<2.0.0)
+Requires-Dist: sdss-coordio (>=1.7.3,<2.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Requires-Dist: simple-pid (>=1.0.1,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.4.45,<2.0.0)
 Requires-Dist: tables (>=3.6.1)
 Project-URL: Documentation, https://sdss-cherno.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/cherno
 Description-Content-Type: text/markdown
```

