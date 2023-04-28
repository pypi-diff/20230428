# Comparing `tmp/protloc_mex1-0.0.0.tar.gz` & `tmp/protloc_mex1-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "protloc_mex1-0.0.1.tar", last modified: Fri Apr 28 11:54:26 2023, max compression
```

## Comparing `protloc_mex1-0.0.0.tar` & `protloc_mex1-0.0.1.tar`

### file list

```diff
@@ -1,42 +1,19 @@
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/README.txt
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/EGG-INFO/LICENSE
--rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/EGG-INFO/PKG-INFO
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/EGG-INFO/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/EGG-INFO/WHEEL
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/EGG-INFO/entry_points.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/EGG-INFO/requires.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/EGG-INFO/top_level.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/EGG-INFO/zip-safe
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/__main__.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/_cli.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/_entrypoints.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/_overrides.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/_types.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/_version_cls.py
--rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/config.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/discover.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/file_finder.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/file_finder_git.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/file_finder_hg.py
--rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/git.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/hacks.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/hg.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/hg_git.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/integration.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/scm_workdir.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/utils.py
--rw-r--r--   0        0        0    17034 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/_integration/__init__.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/_integration/pyproject_reading.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/.eggs/setuptools_scm-7.1.0-py3.9.egg/setuptools_scm/_integration/setuptools.py
--rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/protloc_mex1/AA_count.py
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/protloc_mex1/GO_count.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/protloc_mex1/SHAP_conduct.py
--rw-r--r--   0        0        0    28400 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/protloc_mex1/SHAP_plus.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/protloc_mex1/__init__.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/protloc_mex1/classifier_evalute.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 protloc_mex1-0.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-28 11:54:26.634986 protloc_mex1-0.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1143 2023-04-28 11:54:26.627385 protloc_mex1-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-04-26 08:22:56.000000 protloc_mex1-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 11:54:26.594816 protloc_mex1-0.0.1/protloc_mex1/
+-rw-rw-rw-   0        0        0    12015 2023-04-25 09:31:12.000000 protloc_mex1-0.0.1/protloc_mex1/AA_count.py
+-rw-rw-rw-   0        0        0     7581 2023-04-26 07:57:22.000000 protloc_mex1-0.0.1/protloc_mex1/GO_count.py
+-rw-rw-rw-   0        0        0     4597 2023-03-13 09:02:36.000000 protloc_mex1-0.0.1/protloc_mex1/SHAP_conduct.py
+-rw-rw-rw-   0        0        0    28400 2023-03-29 08:47:08.000000 protloc_mex1-0.0.1/protloc_mex1/SHAP_plus.py
+-rw-rw-rw-   0        0        0       37 2023-04-24 09:24:54.000000 protloc_mex1-0.0.1/protloc_mex1/__init__.py
+-rw-rw-rw-   0        0        0    10409 2023-04-25 10:52:28.000000 protloc_mex1-0.0.1/protloc_mex1/classifier_evalute.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:54:26.627385 protloc_mex1-0.0.1/protloc_mex1.egg-info/
+-rw-rw-rw-   0        0        0     1143 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      916 2023-04-28 11:53:19.000000 protloc_mex1-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 11:54:26.634986 protloc_mex1-0.0.1/setup.cfg
```

### Comparing `protloc_mex1-0.0.0/protloc_mex1/AA_count.py` & `protloc_mex1-0.0.1/protloc_mex1/AA_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.0/protloc_mex1/GO_count.py` & `protloc_mex1-0.0.1/protloc_mex1/GO_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.0/protloc_mex1/SHAP_conduct.py` & `protloc_mex1-0.0.1/protloc_mex1/SHAP_conduct.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.0/protloc_mex1/SHAP_plus.py` & `protloc_mex1-0.0.1/protloc_mex1/SHAP_plus.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.0/protloc_mex1/classifier_evalute.py` & `protloc_mex1-0.0.1/protloc_mex1/classifier_evalute.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.0/LICENSE.txt` & `protloc_mex1-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.0/README.md` & `protloc_mex1-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.0/pyproject.toml` & `protloc_mex1-0.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "protloc_mex1"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Ze Yu Luo", email="1024226968@qq.com" },
 ]
 description = "..."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-install_requires = [
+dependencies = [
         "biopython~=1.79",
         "numpy~=1.20.3",
         "pandas~=1.4.1",
         "scikit-learn~=1.0.2",
         "seaborn~=0.11.2",
         "matplotlib~=3.5.1",
         "shap~=0.41.0",
```

### Comparing `protloc_mex1-0.0.0/PKG-INFO` & `protloc_mex1-0.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: protloc_mex1
-Version: 0.0.0
-Summary: ...
-Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
-Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
-Author-email: Ze Yu Luo <1024226968@qq.com>
-License-File: LICENSE.txt
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# ProtLoc-mexl
-This project provides a pipeline for fast construction of subcellular localization prediction and model interpretation, with 42 amino acid feature characterization algorithms and GO feature extraction based on Doc2Vec. In addition, two random forest models for protein localization prediction are also provided.
-
-As the manuscript is still under review, we have not fully released the core code and pre-trained models of ProtLoc-Mex1. If you need the core code, please contact the author at 1024226968@qq.com by email.
+Metadata-Version: 2.1
+Name: protloc_mex1
+Version: 0.0.1
+Summary: ...
+Author-email: Ze Yu Luo <1024226968@qq.com>
+Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
+Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# ProtLoc-mexl
+This project provides a pipeline for fast construction of subcellular localization prediction and model interpretation, with 42 amino acid feature characterization algorithms and GO feature extraction based on Doc2Vec. In addition, two random forest models for protein localization prediction are also provided.
+
+As the manuscript is still under review, we have not fully released the core code and pre-trained models of ProtLoc-Mex1. If you need the core code, please contact the author at 1024226968@qq.com by email.
```

