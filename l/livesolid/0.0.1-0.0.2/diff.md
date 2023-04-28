# Comparing `tmp/livesolid-0.0.1.tar.gz` & `tmp/livesolid-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livesolid-0.0.1.tar", last modified: Fri Apr 28 14:32:41 2023, max compression
+gzip compressed data, was "livesolid-0.0.2.tar", last modified: Fri Apr 28 15:16:28 2023, max compression
```

## Comparing `livesolid-0.0.1.tar` & `livesolid-0.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 14:32:41.360590 livesolid-0.0.1/
--rw-r--r--   0 mtm        (501) staff       (20)      592 2023-04-28 13:28:55.000000 livesolid-0.0.1/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      566 2023-04-28 13:28:55.000000 livesolid-0.0.1/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       57 2023-04-28 13:28:55.000000 livesolid-0.0.1/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-04-28 14:23:15.000000 livesolid-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      530 2023-04-28 13:28:55.000000 livesolid-0.0.1/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2023-04-28 13:28:55.000000 livesolid-0.0.1/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2023-04-28 13:28:55.000000 livesolid-0.0.1/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13840 2023-04-28 13:28:55.000000 livesolid-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-04-28 13:28:55.000000 livesolid-0.0.1/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-04-28 14:32:41.360906 livesolid-0.0.1/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2084 2023-04-28 13:28:55.000000 livesolid-0.0.1/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 14:32:41.350107 livesolid-0.0.1/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 14:32:41.350790 livesolid-0.0.1/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9742 2023-04-28 13:36:58.000000 livesolid-0.0.1/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2321 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2023-04-28 13:28:55.000000 livesolid-0.0.1/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      346 2023-04-28 13:28:55.000000 livesolid-0.0.1/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1253 2023-04-28 14:32:41.362188 livesolid-0.0.1/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      704 2023-04-28 13:28:55.000000 livesolid-0.0.1/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 14:32:41.335245 livesolid-0.0.1/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 14:32:41.352938 livesolid-0.0.1/src/livesolid/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2023-04-28 13:28:55.000000 livesolid-0.0.1/src/livesolid/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)      779 2023-04-28 14:23:22.000000 livesolid-0.0.1/src/livesolid/lib.py
--rw-r--r--   0 mtm        (501) staff       (20)     2881 2023-04-28 14:28:31.000000 livesolid-0.0.1/src/livesolid/main.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 14:32:41.358514 livesolid-0.0.1/src/livesolid/templates/
--rw-r--r--   0 mtm        (501) staff       (20)      332 2023-04-28 14:23:22.000000 livesolid-0.0.1/src/livesolid/templates/Makefile.j2
--rw-r--r--   0 mtm        (501) staff       (20)     1184 2023-04-28 14:17:25.000000 livesolid-0.0.1/src/livesolid/templates/goreleaser.yaml.j2
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 14:32:41.357414 livesolid-0.0.1/src/livesolid.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-04-28 14:32:41.000000 livesolid-0.0.1/src/livesolid.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      810 2023-04-28 14:32:41.000000 livesolid-0.0.1/src/livesolid.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-28 14:32:41.000000 livesolid-0.0.1/src/livesolid.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       49 2023-04-28 14:32:41.000000 livesolid-0.0.1/src/livesolid.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-28 14:32:40.000000 livesolid-0.0.1/src/livesolid.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)       93 2023-04-28 14:32:41.000000 livesolid-0.0.1/src/livesolid.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       10 2023-04-28 14:32:41.000000 livesolid-0.0.1/src/livesolid.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 14:32:41.360032 livesolid-0.0.1/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      277 2023-04-28 13:28:55.000000 livesolid-0.0.1/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)      594 2023-04-28 13:28:55.000000 livesolid-0.0.1/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-04-28 13:28:55.000000 livesolid-0.0.1/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 15:16:28.615685 livesolid-0.0.2/
+-rw-r--r--   0 mtm        (501) staff       (20)      592 2023-04-28 13:28:55.000000 livesolid-0.0.2/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      566 2023-04-28 13:28:55.000000 livesolid-0.0.2/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       57 2023-04-28 13:28:55.000000 livesolid-0.0.2/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-04-28 14:23:15.000000 livesolid-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      530 2023-04-28 13:28:55.000000 livesolid-0.0.2/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2023-04-28 13:28:55.000000 livesolid-0.0.2/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2023-04-28 13:28:55.000000 livesolid-0.0.2/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13840 2023-04-28 13:28:55.000000 livesolid-0.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-04-28 13:28:55.000000 livesolid-0.0.2/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-04-28 15:16:28.616010 livesolid-0.0.2/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2084 2023-04-28 13:28:55.000000 livesolid-0.0.2/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 15:16:28.606274 livesolid-0.0.2/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 15:16:28.606769 livesolid-0.0.2/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9742 2023-04-28 13:36:58.000000 livesolid-0.0.2/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2321 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2023-04-28 13:28:55.000000 livesolid-0.0.2/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      346 2023-04-28 13:28:55.000000 livesolid-0.0.2/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1253 2023-04-28 15:16:28.617758 livesolid-0.0.2/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      704 2023-04-28 13:28:55.000000 livesolid-0.0.2/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 15:16:28.593634 livesolid-0.0.2/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 15:16:28.608745 livesolid-0.0.2/src/livesolid/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2023-04-28 13:28:55.000000 livesolid-0.0.2/src/livesolid/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)      779 2023-04-28 14:23:22.000000 livesolid-0.0.2/src/livesolid/lib.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2881 2023-04-28 14:28:31.000000 livesolid-0.0.2/src/livesolid/main.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 15:16:28.613602 livesolid-0.0.2/src/livesolid/templates/
+-rw-r--r--   0 mtm        (501) staff       (20)      485 2023-04-28 15:13:58.000000 livesolid-0.0.2/src/livesolid/templates/Makefile.j2
+-rw-r--r--   0 mtm        (501) staff       (20)     1184 2023-04-28 14:17:25.000000 livesolid-0.0.2/src/livesolid/templates/goreleaser.yaml.j2
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 15:16:28.612399 livesolid-0.0.2/src/livesolid.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-04-28 15:16:28.000000 livesolid-0.0.2/src/livesolid.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      810 2023-04-28 15:16:28.000000 livesolid-0.0.2/src/livesolid.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-28 15:16:28.000000 livesolid-0.0.2/src/livesolid.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       49 2023-04-28 15:16:28.000000 livesolid-0.0.2/src/livesolid.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-28 15:16:28.000000 livesolid-0.0.2/src/livesolid.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)       93 2023-04-28 15:16:28.000000 livesolid-0.0.2/src/livesolid.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       10 2023-04-28 15:16:28.000000 livesolid-0.0.2/src/livesolid.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-28 15:16:28.615079 livesolid-0.0.2/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      277 2023-04-28 13:28:55.000000 livesolid-0.0.2/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)      594 2023-04-28 13:28:55.000000 livesolid-0.0.2/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-04-28 13:28:55.000000 livesolid-0.0.2/tox.ini
```

### Comparing `livesolid-0.0.1/.coveragerc` & `livesolid-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/.gitignore` & `livesolid-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/.pre-commit-config.yaml` & `livesolid-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/.readthedocs.yml` & `livesolid-0.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/CONTRIBUTING.rst` & `livesolid-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/LICENSE.txt` & `livesolid-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/PKG-INFO` & `livesolid-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livesolid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `livesolid-0.0.1/README.rst` & `livesolid-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/docs/Makefile` & `livesolid-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/docs/conf.py` & `livesolid-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/docs/index.rst` & `livesolid-0.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/setup.cfg` & `livesolid-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/setup.py` & `livesolid-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/src/livesolid/__init__.py` & `livesolid-0.0.2/src/livesolid/__init__.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/src/livesolid/lib.py` & `livesolid-0.0.2/src/livesolid/lib.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/src/livesolid/main.py` & `livesolid-0.0.2/src/livesolid/main.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/src/livesolid/templates/goreleaser.yaml.j2` & `livesolid-0.0.2/src/livesolid/templates/goreleaser.yaml.j2`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/src/livesolid.egg-info/PKG-INFO` & `livesolid-0.0.2/src/livesolid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livesolid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `livesolid-0.0.1/src/livesolid.egg-info/SOURCES.txt` & `livesolid-0.0.2/src/livesolid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/tests/test_skeleton.py` & `livesolid-0.0.2/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.1/tox.ini` & `livesolid-0.0.2/tox.ini`

 * *Files identical despite different names*

