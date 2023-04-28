# Comparing `tmp/cf_pandas-0.6.0.tar.gz` & `tmp/cf_pandas-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_pandas-0.6.0.tar", last modified: Tue Mar 21 17:14:16 2023, max compression
+gzip compressed data, was "cf_pandas-0.7.0.tar", last modified: Fri Apr 28 21:16:10 2023, max compression
```

## Comparing `cf_pandas-0.6.0.tar` & `cf_pandas-0.7.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.498472 cf_pandas-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.490472 cf_pandas-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.494472 cf_pandas-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/.github/workflows/linting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-21 17:14:16.498472 cf_pandas-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.494472 cf_pandas-0.6.0/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/binder/postBuild
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.494472 cf_pandas-0.6.0/cf_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/cf_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-21 17:14:16.000000 cf_pandas-0.6.0/cf_pandas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/cf_pandas/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/cf_pandas/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/cf_pandas/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/cf_pandas/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/cf_pandas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/cf_pandas/vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/cf_pandas/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.494472 cf_pandas-0.6.0/cf_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-21 17:14:16.000000 cf_pandas-0.6.0/cf_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-21 17:14:16.000000 cf_pandas-0.6.0/cf_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 17:14:16.000000 cf_pandas-0.6.0/cf_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 17:14:16.000000 cf_pandas-0.6.0/cf_pandas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 17:14:16.000000 cf_pandas-0.6.0/cf_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-21 17:14:16.000000 cf_pandas-0.6.0/cf_pandas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.498472 cf_pandas-0.6.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/ci/environment-py3.10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/ci/environment-py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/ci/environment-py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.498472 cf_pandas-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/demo_overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/demo_reg.md
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/demo_vocab.md
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/demo_widget.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/requirements-opt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-21 17:14:16.502472 cf_pandas-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:14:16.498472 cf_pandas-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/tests/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/tests/test_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/tests/test_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-21 17:14:09.000000 cf_pandas-0.6.0/tests/test_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.881054 cf_pandas-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.873054 cf_pandas-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.873054 cf_pandas-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/.github/workflows/linting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-28 21:16:10.881054 cf_pandas-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.877054 cf_pandas-0.7.0/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/binder/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.877054 cf_pandas-0.7.0/cf_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/cf_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 21:16:10.000000 cf_pandas-0.7.0/cf_pandas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/cf_pandas/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/cf_pandas/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/cf_pandas/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/cf_pandas/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/cf_pandas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/cf_pandas/vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/cf_pandas/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.877054 cf_pandas-0.7.0/cf_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-28 21:16:10.000000 cf_pandas-0.7.0/cf_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-28 21:16:10.000000 cf_pandas-0.7.0/cf_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:16:10.000000 cf_pandas-0.7.0/cf_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:16:10.000000 cf_pandas-0.7.0/cf_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 21:16:10.000000 cf_pandas-0.7.0/cf_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 21:16:10.000000 cf_pandas-0.7.0/cf_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.877054 cf_pandas-0.7.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/ci/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/ci/environment-py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/ci/environment-py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.881054 cf_pandas-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/demo_overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/demo_reg.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/demo_vocab.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/demo_widget.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/requirements-opt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-28 21:16:10.881054 cf_pandas-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:16:10.881054 cf_pandas-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/tests/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/tests/test_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/tests/test_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-28 21:16:02.000000 cf_pandas-0.7.0/tests/test_widget.py
```

### Comparing `cf_pandas-0.6.0/.github/workflows/release.yaml` & `cf_pandas-0.7.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/.github/workflows/test.yaml` & `cf_pandas-0.7.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/.gitignore` & `cf_pandas-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/.pre-commit-config.yaml` & `cf_pandas-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/LICENSE.txt` & `cf_pandas-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/PKG-INFO` & `cf_pandas-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_pandas
-Version: 0.6.0
+Version: 0.7.0
 Summary: an accessor for pandas objects that interprets CF attributes
 Home-page: https://github.com/axiom-data-science/cf-pandas
 Author: Axiom Data Science
 Author-email: AUTHOR@EMAIL.COM
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `cf_pandas-0.6.0/README.md` & `cf_pandas-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/cf_pandas/accessor.py` & `cf_pandas-0.7.0/cf_pandas/accessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,25 +54,28 @@
 
 
 @pd.api.extensions.register_dataframe_accessor("cf")
 class CFAccessor:
     """Dataframe accessor analogous to cf-xarray accessor."""
 
     def __init__(self, pandas_obj):
-        self._validate(pandas_obj)
+        # don't automatically validate but can when needed
+        # self._validate(pandas_obj)
         self._obj = pandas_obj
 
-    @staticmethod
-    def _validate(obj):
+    # @staticmethod
+    def _validate(self):
         """what is necessary for basic use."""
 
         # verify that necessary keys are present. Z would also be nice but might be missing.
         # but don't use the accessor to check
         keys = ["T", "longitude", "latitude"]
-        missing_keys = [key for key in keys if len(_get_axis_coord(obj, key)) == 0]
+        missing_keys = [
+            key for key in keys if len(_get_axis_coord(self._obj, key)) == 0
+        ]
         if len(missing_keys) > 0:
             raise AttributeError(
                 f'{"longitude", "latitude", "time"} must be identifiable in DataFrame but {missing_keys} are missing.'
             )
 
         # for key in keys:
         #     if len(_get_axis_coord(obj, "T")) == 0:
@@ -106,17 +109,20 @@
         valid_keys = _COORD_NAMES + _AXIS_NAMES
         if key in valid_keys:
             col_names = _get_axis_coord(self._obj, key)
 
         else:
             col_names = _get_custom_criteria(self._obj, key)
 
-        # return series
-        if len(col_names) == 1:
+        # return series for column
+        if len(col_names) == 1 and col_names[0] in self._obj.columns:
             return self._obj[col_names[0]]
+        # return index
+        elif len(col_names) == 1 and col_names[0] in self._obj.index.names:
+            return self._obj.index.get_level_values(col_names[0])
         # return DataFrame
         elif len(col_names) > 1:
             return self._obj[col_names]
         else:
             raise ValueError("Some error has occurred.")
 
     def __setitem__(self, key: str, values: Union[Sequence, Series]):
@@ -245,14 +251,40 @@
         vardict = {
             key: _get_custom_criteria(self._obj, key) for key in custom_criteria.keys()
         }
 
         return vardict
 
     @property
+    def axes_cols(self) -> List[str]:
+        """
+        Property that returns a list of column names from the axes mapping.
+
+        Returns
+        -------
+        list
+            Variable names that are the column names which represent axes.
+        """
+
+        return list(itertools.chain(*[*self.axes.values()]))
+
+    @property
+    def coordinates_cols(self) -> List[str]:
+        """
+        Property that returns a list of column names from the coordinates mapping.
+
+        Returns
+        -------
+        list
+            Variable names that are the column names which represent coordinates.
+        """
+
+        return list(itertools.chain(*[*self.coordinates.values()]))
+
+    @property
     def standard_names(self):
         """
         Returns a dictionary mapping standard_names to variable names, if there is a match. Compares with all cf-standard names.
 
         Returns
         -------
         dict
@@ -309,34 +341,22 @@
 
     valid_keys = _COORD_NAMES + _AXIS_NAMES
     if key not in valid_keys:
         raise KeyError(
             f"cf_xarray did not understand key {key!r}. Expected one of {valid_keys!r}"
         )
 
-    # search_in = set()
-    # attrs_or_encoding = ChainMap(obj.attrs, obj.encoding)
-    # coordinates = attrs_or_encoding.get("coordinates", None)
-
-    # # Handles case where the coordinates attribute is None
-    # # This is used to tell xarray to not write a coordinates attribute
-    # if coordinates:
-    #     search_in.update(coordinates.split(" "))
-    # if not search_in:
-    #     search_in = set(obj.coords)
-
-    # # maybe only do this for key in _AXIS_NAMES?
-    # search_in.update(obj.indexes)
-
-    # search_in = search_in & set(obj.coords)
+    # loop over column names and index names
     results: set = set()
-    for col in obj.columns:
-        # var = obj.coords[coord]
+    cols_and_indices = list(obj.columns)
+    cols_and_indices += obj.index.names
+    # remove None if in names from index
+    cols_and_indices = [name for name in cols_and_indices if name is not None]
+    for col in cols_and_indices:
         if key in coordinate_criteria:
-            # import pdb; pdb.set_trace()
             for criterion, expected in coordinate_criteria[key].items():
                 # allow for the column header having a space in it that separate
                 # the name from the units, for example
                 strings = col.split()
                 for string in strings:
                     string = string.lower()
                     if string.startswith("(") and string.endswith(")"):
@@ -346,22 +366,27 @@
                         # if col.attrs.get(criterion, None) in expected:
                         results.update((col,))
                     # if criterion == "units":
                     #     # deal with pint-backed objects
                     #     units = getattr(col.data, "units", None)
                     #     if units in expected:
                     #         results.update((col,))
-
         # also use the guess_regex approach by default, but only if no results so far
         # this takes the logic from cf-xarray guess_coord_axis
         if len(results) == 0:
-            if key in ("T", "time") and _is_datetime_like(obj[col]):
-                results.update((col,))
-                continue  # prevent second detection
-
+            if col in obj.columns:
+                if key in ("T", "time") and _is_datetime_like(obj[col]):
+                    results.update((col,))
+                    continue  # prevent second detection
+            elif col in obj.index.names:
+                if key in ("T", "time") and _is_datetime_like(
+                    obj.index.get_level_values(col)
+                ):
+                    results.update((col,))
+                    continue  # prevent second detection
             pattern = guess_regex[key]
             if pattern.match(col.lower()):
                 results.update((col,))
 
     return list(results)
```

### Comparing `cf_pandas-0.6.0/cf_pandas/criteria.py` & `cf_pandas-0.7.0/cf_pandas/criteria.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,19 +99,26 @@
 for coord, attrs in coordinate_criteria.items():
     coordinate_criteria[coord]["long_name"] = coordinate_criteria[coord][
         "standard_name"
     ]
 coordinate_criteria["X"]["long_name"] += ("cell index along first dimension",)
 coordinate_criteria["Y"]["long_name"] += ("cell index along second dimension",)
 
+# changes allow for the pattern string to not be at the start of the comparison string
+# like (?=.*lon)
 guess_regex = {
-    "time": re.compile("\\bt\\b|(time|min|hour|day|week|month|year)[0-9]*"),
+    "time": re.compile("\\bt\\b|(?=.*time|min|hour|day|week|month|year)[0-9]*"),
+    # "time": re.compile("\\bt\\b|(time|min|hour|day|week|month|year)[0-9]*"),
     "Z": re.compile(
-        "(z|nav_lev|gdep|lv_|[o]*lev|bottom_top|sigma|h(ei)?ght|altitude|depth|"
+        "(z|nav_lev|gdep|lv_|[o]*lev|bottom_top|sigma|(?=.*dbars)|h(ei)?ght|altitude|depth|"
         "isobaric|pres|isotherm)[a-z_]*[0-9]*"
     ),
+    # "Z": re.compile(
+    #     "(z|nav_lev|gdep|lv_|[o]*lev|bottom_top|sigma|h(ei)?ght|altitude|depth|"
+    #     "isobaric|pres|isotherm)[a-z_]*[0-9]*"
+    # ),
     "Y": re.compile("y|j|nlat|nj"),
-    "latitude": re.compile("y?(nav_lat|lat|gphi)[a-z0-9]*"),
+    "latitude": re.compile("y?(nav_lat|(?=.*lat)|gphi)[a-z0-9]*"),
     "X": re.compile("x|i|nlon|ni"),
-    "longitude": re.compile("x?(nav_lon|lon|glam)[a-z0-9]*"),
+    "longitude": re.compile("x?(nav_lon|(?=.*lon)|glam)[a-z0-9]*"),
 }
 guess_regex["T"] = guess_regex["time"]
```

### Comparing `cf_pandas-0.6.0/cf_pandas/options.py` & `cf_pandas-0.7.0/cf_pandas/options.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/cf_pandas/reg.py` & `cf_pandas-0.7.0/cf_pandas/reg.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/cf_pandas/utils.py` & `cf_pandas-0.7.0/cf_pandas/utils.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/cf_pandas/vocab.py` & `cf_pandas-0.7.0/cf_pandas/vocab.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/cf_pandas/widget.py` & `cf_pandas-0.7.0/cf_pandas/widget.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/cf_pandas.egg-info/PKG-INFO` & `cf_pandas-0.7.0/cf_pandas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-pandas
-Version: 0.6.0
+Version: 0.7.0
 Summary: an accessor for pandas objects that interprets CF attributes
 Home-page: https://github.com/axiom-data-science/cf-pandas
 Author: Axiom Data Science
 Author-email: AUTHOR@EMAIL.COM
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `cf_pandas-0.6.0/cf_pandas.egg-info/SOURCES.txt` & `cf_pandas-0.7.0/cf_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/Makefile` & `cf_pandas-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/api.rst` & `cf_pandas-0.7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/conf.py` & `cf_pandas-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/demo_overview.md` & `cf_pandas-0.7.0/docs/demo_overview.md`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/demo_reg.md` & `cf_pandas-0.7.0/docs/demo_reg.md`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/demo_vocab.md` & `cf_pandas-0.7.0/docs/demo_vocab.md`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/demo_widget.md` & `cf_pandas-0.7.0/docs/demo_widget.md`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/environment.yml` & `cf_pandas-0.7.0/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/docs/index.rst` & `cf_pandas-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/pyproject.toml` & `cf_pandas-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/setup.cfg` & `cf_pandas-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/tests/test_accessor.py` & `cf_pandas-0.7.0/tests/test_accessor.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def test_validate():
     df = pd.DataFrame(
         columns=[
             "temp",
         ]
     )
     with pytest.raises(AttributeError):
-        df.cf.keys()
+        df.cf._validate()
 
 
 def test_match_criteria_key_accessor():
 
     df = pd.DataFrame(
         columns=[
             "temp",
@@ -124,7 +124,24 @@
 
 
 def test_get_by_guess_regex():
     df = pd.DataFrame(columns=["lon", "lat", "min"])
     assert df.cf["longitude"].name == "lon"
     assert df.cf["latitude"].name == "lat"
     assert df.cf["time"].name == "min"
+
+    df = pd.DataFrame(columns=["blah_lon", "table_lat"])
+    assert df.cf["longitude"].name == "blah_lon"
+    assert df.cf["latitude"].name == "table_lat"
+
+
+def test_index():
+    """Test when time is in index."""
+    df = pd.DataFrame(index=["m_time"])
+    df.index.rename("m_time", inplace=True)
+    assert df.cf["T"].name == "m_time"
+
+
+def test_cols():
+    df = pd.DataFrame(columns=["m_time", "lon", "lat", "temp"])
+    assert df.cf.axes_cols == ["m_time"]
+    assert sorted(df.cf.coordinates_cols) == ["lat", "lon", "m_time"]
```

### Comparing `cf_pandas-0.6.0/tests/test_reg.py` & `cf_pandas-0.7.0/tests/test_reg.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/tests/test_utils.py` & `cf_pandas-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/tests/test_vocab.py` & `cf_pandas-0.7.0/tests/test_vocab.py`

 * *Files identical despite different names*

### Comparing `cf_pandas-0.6.0/tests/test_widget.py` & `cf_pandas-0.7.0/tests/test_widget.py`

 * *Files identical despite different names*

