# Comparing `tmp/aind-ng-link-1.0.3.tar.gz` & `tmp/aind-ng-link-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-ng-link-1.0.3.tar", last modified: Fri Apr 28 16:14:24 2023, max compression
+gzip compressed data, was "aind-ng-link-1.0.4.tar", last modified: Fri Apr 28 18:02:14 2023, max compression
```

## Comparing `aind-ng-link-1.0.3.tar` & `aind-ng-link-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.333605 aind-ng-link-1.0.3/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      170 2023-04-27 22:23:53.000000 aind-ng-link-1.0.3/.flake8
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.245501 aind-ng-link-1.0.3/.github/
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.259407 aind-ng-link-1.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      834 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      595 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      772 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.290651 aind-ng-link-1.0.3/.github/workflows/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1471 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      713 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/.github/workflows/tag.yml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2199 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/.gitignore
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1092 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/LICENSE
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-04-28 16:14:24.332860 aind-ng-link-1.0.3/PKG-INFO
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2451 2023-04-28 00:41:21.000000 aind-ng-link-1.0.3/README.md
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.294062 aind-ng-link-1.0.3/doc_template/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      638 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/doc_template/Makefile
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      769 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/doc_template/make.bat
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.301666 aind-ng-link-1.0.3/doc_template/source/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1540 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/doc_template/source/conf.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      470 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/doc_template/source/index.rst
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1578 2023-04-28 16:12:23.000000 aind-ng-link-1.0.3/pyproject.toml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       38 2023-04-28 16:14:24.333813 aind-ng-link-1.0.3/setup.cfg
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      256 2023-04-28 15:26:22.000000 aind-ng-link-1.0.3/setup.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.247767 aind-ng-link-1.0.3/src/
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.312157 aind-ng-link-1.0.3/src/aind_ng_link.egg-info/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-04-28 16:14:24.000000 aind-ng-link-1.0.3/src/aind_ng_link.egg-info/PKG-INFO
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      944 2023-04-28 16:14:24.000000 aind-ng-link-1.0.3/src/aind_ng_link.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)        1 2023-04-28 16:14:24.000000 aind-ng-link-1.0.3/src/aind_ng_link.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      135 2023-04-28 16:14:24.000000 aind-ng-link-1.0.3/src/aind_ng_link.egg-info/requires.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)        8 2023-04-28 16:14:24.000000 aind-ng-link-1.0.3/src/aind_ng_link.egg-info/top_level.txt
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.320898 aind-ng-link-1.0.3/src/ng_link/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      183 2023-04-28 16:14:10.000000 aind-ng-link-1.0.3/src/ng_link/__init__.py
--rw-------   0 jonathan.wong   (502) staff       (20)     6681 2023-04-27 22:32:39.000000 aind-ng-link-1.0.3/src/ng_link/dispim_link.py
--rw-------   0 jonathan.wong   (502) staff       (20)     3665 2023-04-27 22:17:44.000000 aind-ng-link-1.0.3/src/ng_link/exaspim_link.py
--rw-------   0 jonathan.wong   (502) staff       (20)     4361 2023-04-27 22:34:41.000000 aind-ng-link-1.0.3/src/ng_link/link_utils.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    42266 2023-04-27 22:17:45.000000 aind-ng-link-1.0.3/src/ng_link/ng_layer.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    29463 2023-04-27 22:17:45.000000 aind-ng-link-1.0.3/src/ng_link/ng_state.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.325090 aind-ng-link-1.0.3/src/ng_link/scripts/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    13902 2023-04-25 22:57:30.000000 aind-ng-link-1.0.3/src/ng_link/scripts/ccf_ref.csv
--rw-------   0 jonathan.wong   (502) staff       (20)      895 2023-04-27 22:17:44.000000 aind-ng-link-1.0.3/src/ng_link/scripts/create_links.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     6945 2023-04-27 22:24:18.000000 aind-ng-link-1.0.3/src/ng_link/scripts/generate_cff_cell_count.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.327495 aind-ng-link-1.0.3/src/ng_link/utils/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       61 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/src/ng_link/utils/__init__.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     5929 2023-04-27 22:17:44.000000 aind-ng-link-1.0.3/src/ng_link/utils/utils.py
--rw-------   0 jonathan.wong   (502) staff       (20)     2508 2023-04-27 22:17:44.000000 aind-ng-link-1.0.3/src/ng_link/xml_parsing.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 16:14:24.331666 aind-ng-link-1.0.3/tests/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       22 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/tests/__init__.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-04-28 15:42:24.000000 aind-ng-link-1.0.3/tests/test_ng_layer.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-03-20 20:38:13.000000 aind-ng-link-1.0.3/tests/test_ng_state.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.931219 aind-ng-link-1.0.4/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      170 2023-04-27 22:23:53.000000 aind-ng-link-1.0.4/.flake8
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.773700 aind-ng-link-1.0.4/.github/
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.810050 aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      834 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      595 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      772 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.823229 aind-ng-link-1.0.4/.github/workflows/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1471 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      713 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/workflows/tag.yml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2199 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.gitignore
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1092 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/LICENSE
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-04-28 18:02:14.930206 aind-ng-link-1.0.4/PKG-INFO
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2451 2023-04-28 00:41:21.000000 aind-ng-link-1.0.4/README.md
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.836497 aind-ng-link-1.0.4/doc_template/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      638 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/doc_template/Makefile
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      769 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/doc_template/make.bat
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.844325 aind-ng-link-1.0.4/doc_template/source/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1540 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/doc_template/source/conf.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      470 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/doc_template/source/index.rst
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1610 2023-04-28 17:53:08.000000 aind-ng-link-1.0.4/pyproject.toml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2269 2023-04-28 16:05:38.000000 aind-ng-link-1.0.4/requirements.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       38 2023-04-28 18:02:14.931500 aind-ng-link-1.0.4/setup.cfg
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      256 2023-04-28 15:26:22.000000 aind-ng-link-1.0.4/setup.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.775862 aind-ng-link-1.0.4/src/
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.854281 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      961 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)        1 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      137 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/requires.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)        8 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.899747 aind-ng-link-1.0.4/src/ng_link/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      183 2023-04-28 18:01:35.000000 aind-ng-link-1.0.4/src/ng_link/__init__.py
+-rw-------   0 jonathan.wong   (502) staff       (20)     6457 2023-04-28 16:50:07.000000 aind-ng-link-1.0.4/src/ng_link/dispim_link.py
+-rw-------   0 jonathan.wong   (502) staff       (20)     3704 2023-04-28 16:50:21.000000 aind-ng-link-1.0.4/src/ng_link/exaspim_link.py
+-rw-------   0 jonathan.wong   (502) staff       (20)     4403 2023-04-28 16:48:59.000000 aind-ng-link-1.0.4/src/ng_link/link_utils.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    42266 2023-04-27 22:17:45.000000 aind-ng-link-1.0.4/src/ng_link/ng_layer.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    29463 2023-04-27 22:17:45.000000 aind-ng-link-1.0.4/src/ng_link/ng_state.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.913012 aind-ng-link-1.0.4/src/ng_link/scripts/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    13902 2023-04-25 22:57:30.000000 aind-ng-link-1.0.4/src/ng_link/scripts/ccf_ref.csv
+-rw-------   0 jonathan.wong   (502) staff       (20)      894 2023-04-28 16:43:46.000000 aind-ng-link-1.0.4/src/ng_link/scripts/create_links.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     6945 2023-04-27 22:24:18.000000 aind-ng-link-1.0.4/src/ng_link/scripts/generate_cff_cell_count.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.918990 aind-ng-link-1.0.4/src/ng_link/utils/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       61 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/src/ng_link/utils/__init__.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     5929 2023-04-27 22:17:44.000000 aind-ng-link-1.0.4/src/ng_link/utils/utils.py
+-rw-------   0 jonathan.wong   (502) staff       (20)     2545 2023-04-28 16:51:41.000000 aind-ng-link-1.0.4/src/ng_link/xml_parsing.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.928197 aind-ng-link-1.0.4/tests/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       22 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/tests/__init__.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-04-28 15:42:24.000000 aind-ng-link-1.0.4/tests/test_ng_layer.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/tests/test_ng_state.py
```

### Comparing `aind-ng-link-1.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/.github/ISSUE_TEMPLATE/user-story.md` & `aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/.github/workflows/ci.yml` & `aind-ng-link-1.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/.github/workflows/tag.yml` & `aind-ng-link-1.0.4/.github/workflows/tag.yml`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/.gitignore` & `aind-ng-link-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/LICENSE` & `aind-ng-link-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/PKG-INFO` & `aind-ng-link-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-ng-link
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for the generation of neuroglancer links
 Author-email: David Feng <david.feng@alleninstitute.org>, Sharmishtaa Seshamani <sharmishtaas@alleninstitute.org>, Camilo Laiton <camilo.laiton@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `aind-ng-link-1.0.3/README.md` & `aind-ng-link-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/doc_template/Makefile` & `aind-ng-link-1.0.4/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/doc_template/make.bat` & `aind-ng-link-1.0.4/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/doc_template/source/conf.py` & `aind-ng-link-1.0.4/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/pyproject.toml` & `aind-ng-link-1.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 ]
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 dynamic = ["version", "readme"]
 
 dependencies = [
-    'pandas >= 2.0.1',
-    'sphinx >= 6.2.1',
-    'pint >= 0.20.1',
-    'numpy >= 1.24.3',
-    'neuroglancer >= 2.36'
+    'pandas',
+    'sphinx',
+    'pint >= 0.18',
+    'numpy >= 1.21.6',
+    'neuroglancer >= 2.36', 
+    'xmltodict >= 0.13.0'
 ]
 
 [project.optional-dependencies]
 dev = [
     'black',
     'coverage',
     'flake8',
@@ -72,9 +73,9 @@
 exclude_lines = ["if __name__ == .__main__.:"]
 fail_under = 0
 
 [tool.isort]
 line_length = 79
 
 [tool.interrogate]
-exclude = ["setup.py", "docs", "build"]
+exclude = ["setup.py", "docs", "build", "src/ng_link/scripts/"]
 fail-under = 100
```

### Comparing `aind-ng-link-1.0.3/src/aind_ng_link.egg-info/PKG-INFO` & `aind-ng-link-1.0.4/src/aind_ng_link.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-ng-link
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for the generation of neuroglancer links
 Author-email: David Feng <david.feng@alleninstitute.org>, Sharmishtaa Seshamani <sharmishtaas@alleninstitute.org>, Camilo Laiton <camilo.laiton@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `aind-ng-link-1.0.3/src/aind_ng_link.egg-info/SOURCES.txt` & `aind-ng-link-1.0.4/src/aind_ng_link.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .flake8
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/user-story.md
 .github/workflows/ci.yml
 .github/workflows/tag.yml
 doc_template/Makefile
```

### Comparing `aind-ng-link-1.0.3/src/ng_link/dispim_link.py` & `aind-ng-link-1.0.4/src/ng_link/dispim_link.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Library for generating dispim link.
+"""
 import numpy as np
 
 from ng_link import NgState
 
 import xml_parsing
 import link_utils
 
@@ -30,28 +33,14 @@
     # X vector => XZ direction
     deskew_factor = np.tan(np.deg2rad(theta))
     deskew = np.array([[1, 0, 0], [0, 1, 0], [deskew_factor, 0, 1]])
     matrix_3x4 = deskew @ matrix_3x4
 
     return matrix_3x4
 
-
-# Saving for whenever I-Spim -> Di-Spim
-"""
-Camera Alignment
-if camera_index == 1:
-    # Flip in z, mirror in x = Flip in y
-    correction = \
-    np.array([[1, 0, 0],
-              [0, -1, 0],
-              [0, 0, 1]])
-    matrix_3x4 = correction @ matrix_3x4
-"""
-
-
 def generate_dispim_link(
     base_channel_xml_path: str,
     cross_channel_xml_path: str,
     s3_path: str,
     max_dr: int = 800,
     opacity: float = 0.5,
     blend: str = "additive",
```

### Comparing `aind-ng-link-1.0.3/src/ng_link/exaspim_link.py` & `aind-ng-link-1.0.4/src/ng_link/exaspim_link.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""
+Library for generating exaspim link.
+"""
 import numpy as np
 
 from ng_link import NgState
 
 import xml_parsing
 import link_utils
 
-
 def omit_initial_offsets(view_transforms: dict[int, list[dict]]) -> None:
     """
     For OME-Zarr datasets, inital offsets are
     already encoded in the metadata and extracted my neuroglancer.
     This function removes the duplicate transform.
 
     Parameters
@@ -30,16 +32,15 @@
     xml_path: str,
     s3_path: str,
     max_dr: int = 200,
     opacity: float = 1.0,
     blend: str = "default",
     output_json_path: str = ".",
 ) -> None:
-    """
-    Creates an neuroglancer link to visualize
+    """Creates an neuroglancer link to visualize
     registration transforms on exaspim dataset pre-fusion.
 
     Parameters
     ------------------------
     xml_path: str
         Path of xml outputted by BigStitcher.
     s3_path: str
```

### Comparing `aind-ng-link-1.0.3/src/ng_link/link_utils.py` & `aind-ng-link-1.0.4/src/ng_link/link_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Utilities for nueroglancer links.
+"""
 from collections import defaultdict
 import numpy as np
 import re
 
 
 def calculate_net_transforms(
     view_transforms: dict[int, list[dict]]
```

### Comparing `aind-ng-link-1.0.3/src/ng_link/ng_layer.py` & `aind-ng-link-1.0.4/src/ng_link/ng_layer.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/src/ng_link/ng_state.py` & `aind-ng-link-1.0.4/src/ng_link/ng_state.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/src/ng_link/scripts/ccf_ref.csv` & `aind-ng-link-1.0.4/src/ng_link/scripts/ccf_ref.csv`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/src/ng_link/scripts/create_links.py` & `aind-ng-link-1.0.4/src/ng_link/scripts/create_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # from ng_link import exaspim_link
 from ng_link import dispim_link
 
-
 def main():
     # Fill in your own data
     base_channel_path = (
         "/Users/jonathan.wong/Projects/aind-ng-link/dispim_new.xml"
     )
     cross_channel_path = (
         "/Users/jonathan.wong/Projects/aind-ng-link/dispim_new_coreg.xml"
```

### Comparing `aind-ng-link-1.0.3/src/ng_link/scripts/generate_cff_cell_count.py` & `aind-ng-link-1.0.4/src/ng_link/scripts/generate_cff_cell_count.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/src/ng_link/utils/utils.py` & `aind-ng-link-1.0.4/src/ng_link/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.3/src/ng_link/xml_parsing.py` & `aind-ng-link-1.0.4/src/ng_link/xml_parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+"""
+Utilities for parsing BDV XML
+"""
 import xmltodict
 from collections import OrderedDict
 
-
 def extract_tile_paths(xml_path: str) -> dict[int, str]:
     """
     Parses BDV xml and outputs map of setup_id -> tile path.
 
     Parameters
     ------------------------
     xml_path: str
```

