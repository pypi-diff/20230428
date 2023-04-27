# Comparing `tmp/libwwz-1.3.0a0.tar.gz` & `tmp/libwwz-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libwwz-1.3.0a0.tar", last modified: Thu Apr 27 23:27:15 2023, max compression
+gzip compressed data, was "libwwz-1.3.0a1.tar", last modified: Thu Apr 27 23:39:03 2023, max compression
```

## Comparing `libwwz-1.3.0a0.tar` & `libwwz-1.3.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:27:15.262549 libwwz-1.3.0a0/
--rw-r--r--   0 opq       (1000) opq       (1000)    11343 2023-04-27 20:24:49.000000 libwwz-1.3.0a0/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)       25 2022-02-23 23:42:14.000000 libwwz-1.3.0a0/MANIFEST.in
--rw-r--r--   0 opq       (1000) opq       (1000)    16764 2023-04-27 23:27:15.262549 libwwz-1.3.0a0/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)     3433 2022-02-23 23:35:56.000000 libwwz-1.3.0a0/README.md
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:27:15.261549 libwwz-1.3.0a0/libwwz/
--rw-rw-r--   0 opq       (1000) opq       (1000)      164 2020-07-31 02:46:27.000000 libwwz-1.3.0a0/libwwz/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4929 2020-08-17 19:57:59.000000 libwwz-1.3.0a0/libwwz/plot_methods.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    12894 2020-09-17 01:01:10.000000 libwwz-1.3.0a0/libwwz/wwz.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:27:15.261549 libwwz-1.3.0a0/libwwz.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    16764 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)      267 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       55 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        7 2023-04-27 23:27:15.000000 libwwz-1.3.0a0/libwwz.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      767 2023-04-27 23:24:30.000000 libwwz-1.3.0a0/pyproject.toml
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:27:15.262549 libwwz-1.3.0a0/setup.cfg
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:27:15.261549 libwwz-1.3.0a0/tests/
--rw-rw-r--   0 opq       (1000) opq       (1000)      221 2020-04-09 01:05:12.000000 libwwz-1.3.0a0/tests/test_wwz.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:03.470470 libwwz-1.3.0a1/
+-rw-r--r--   0 opq       (1000) opq       (1000)    11343 2023-04-27 20:24:49.000000 libwwz-1.3.0a1/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)       25 2022-02-23 23:42:14.000000 libwwz-1.3.0a1/MANIFEST.in
+-rw-r--r--   0 opq       (1000) opq       (1000)    16764 2023-04-27 23:39:03.469470 libwwz-1.3.0a1/PKG-INFO
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3433 2022-02-23 23:35:56.000000 libwwz-1.3.0a1/README.md
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:03.468470 libwwz-1.3.0a1/libwwz/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      164 2020-07-31 02:46:27.000000 libwwz-1.3.0a1/libwwz/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4929 2020-08-17 19:57:59.000000 libwwz-1.3.0a1/libwwz/plot_methods.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    12894 2020-09-17 01:01:10.000000 libwwz-1.3.0a1/libwwz/wwz.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:03.469470 libwwz-1.3.0a1/libwwz.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    16764 2023-04-27 23:39:03.000000 libwwz-1.3.0a1/libwwz.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)      267 2023-04-27 23:39:03.000000 libwwz-1.3.0a1/libwwz.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:39:03.000000 libwwz-1.3.0a1/libwwz.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       55 2023-04-27 23:39:03.000000 libwwz-1.3.0a1/libwwz.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        7 2023-04-27 23:39:03.000000 libwwz-1.3.0a1/libwwz.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      767 2023-04-27 23:38:41.000000 libwwz-1.3.0a1/pyproject.toml
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:39:03.470470 libwwz-1.3.0a1/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:03.469470 libwwz-1.3.0a1/tests/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      221 2020-04-09 01:05:12.000000 libwwz-1.3.0a1/tests/test_wwz.py
```

### Comparing `libwwz-1.3.0a0/LICENSE` & `libwwz-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `libwwz-1.3.0a0/PKG-INFO` & `libwwz-1.3.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libwwz
-Version: 1.3.0a0
+Version: 1.3.0a1
 Summary: Library for computing the weighted wavelet Z transform.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libwwz-1.3.0a0/README.md` & `libwwz-1.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `libwwz-1.3.0a0/libwwz/plot_methods.py` & `libwwz-1.3.0a1/libwwz/plot_methods.py`

 * *Files identical despite different names*

### Comparing `libwwz-1.3.0a0/libwwz/wwz.py` & `libwwz-1.3.0a1/libwwz/wwz.py`

 * *Files identical despite different names*

### Comparing `libwwz-1.3.0a0/libwwz.egg-info/PKG-INFO` & `libwwz-1.3.0a1/libwwz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libwwz
-Version: 1.3.0a0
+Version: 1.3.0a1
 Summary: Library for computing the weighted wavelet Z transform.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libwwz-1.3.0a0/pyproject.toml` & `libwwz-1.3.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # See:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "libwwz"
-version = "1.3.0a0"
+version = "1.3.0a1"
 authors = [
     { name = "RedVox, Inc", email = "support@redvox.io" }
 ]
 description = "Library for computing the weighted wavelet Z transform."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 
 dependencies = [
     "joblib==1.2.0",
-    "redvox-base[matplotlib,numpy]==2023.4.25"
+    "redvox-base[matplotlib,numpy]==2023.4.27"
 ]
 
 [project.urls]
 homepage = "https://github.com/RedVoxInc/libwwz"
 PyPI = "https://pypi.org/project/libwwz/"
 
 [build-system]
```

