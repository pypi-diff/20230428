# Comparing `tmp/releases-2.1.0.tar.gz` & `tmp/releases-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpyadrnne_/dist/releases-2.1.0.tar", last modified: Sat Feb 25 00:01:32 2023, max compression
+gzip compressed data, was "/tmp/tmpgv3w2vb7/dist/releases-2.1.1.tar", last modified: Fri Apr 28 19:11:49 2023, max compression
```

## Comparing `releases-2.1.0.tar` & `releases-2.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)       31 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      502 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        9 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     4227 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2022-06-17 18:56:00.000000 releases-2.1.0/MANIFEST.in
--rw-r--r--   0 jforcier  (1000) users      (100)      327 2022-12-31 04:35:57.000000 releases-2.1.0/dev-requirements.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-02-25 00:01:32.000000 releases-2.1.0/setup.cfg
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)    11927 2023-02-24 22:24:17.000000 releases-2.1.0/docs/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    19093 2023-02-17 23:17:42.000000 releases-2.1.0/docs/concepts.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      162 2022-06-17 18:56:00.000000 releases-2.1.0/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     8141 2023-02-24 22:23:42.000000 releases-2.1.0/docs/usage.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      605 2022-12-18 03:30:08.000000 releases-2.1.0/docs/conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/releases/
--rw-r--r--   0 jforcier  (1000) users      (100)     2556 2023-02-16 19:52:34.000000 releases-2.1.0/releases/line_manager.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9939 2022-09-30 22:33:57.000000 releases-2.1.0/releases/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-02-24 22:23:42.000000 releases-2.1.0/releases/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7388 2023-02-16 19:52:34.000000 releases-2.1.0/releases/models.py
--rw-r--r--   0 jforcier  (1000) users      (100)    28550 2023-02-24 22:23:42.000000 releases-2.1.0/releases/__init__.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)     3500 2022-12-18 03:30:08.000000 releases-2.1.0/tests/_util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    10659 2023-02-24 22:23:42.000000 releases-2.1.0/tests/presentation.py
--rw-r--r--   0 jforcier  (1000) users      (100)      102 2023-02-24 22:23:42.000000 releases-2.1.0/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)    19083 2023-02-24 22:23:42.000000 releases-2.1.0/tests/organization.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5621 2022-12-19 02:06:53.000000 releases-2.1.0/tests/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2386 2023-02-16 19:51:03.000000 releases-2.1.0/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)      524 2022-08-27 19:49:59.000000 releases-2.1.0/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4227 2023-02-25 00:01:32.000000 releases-2.1.0/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-06-17 18:56:00.000000 releases-2.1.0/LICENSE
--rw-r--r--   0 jforcier  (1000) users      (100)     2314 2022-08-27 19:49:59.000000 releases-2.1.0/README.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 19:11:49.000000 releases-2.1.1/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2386 2023-02-16 19:51:03.000000 releases-2.1.1/setup.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 19:11:49.000000 releases-2.1.1/releases.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)        9 2023-04-28 19:11:49.000000 releases-2.1.1/releases.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     4227 2023-04-28 19:11:49.000000 releases-2.1.1/releases.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)      502 2023-04-28 19:11:49.000000 releases-2.1.1/releases.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-28 19:11:49.000000 releases-2.1.1/releases.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       31 2023-04-28 19:11:49.000000 releases-2.1.1/releases.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      311 2023-04-28 18:36:21.000000 releases-2.1.1/dev-requirements.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      524 2022-08-27 19:49:59.000000 releases-2.1.1/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4227 2023-04-28 19:11:49.000000 releases-2.1.1/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     2314 2022-08-27 19:49:59.000000 releases-2.1.1/README.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 19:11:49.000000 releases-2.1.1/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)      639 2023-04-28 18:54:19.000000 releases-2.1.1/docs/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      162 2022-06-17 18:56:00.000000 releases-2.1.1/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    12162 2023-04-28 19:11:46.000000 releases-2.1.1/docs/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    19093 2023-02-17 23:17:42.000000 releases-2.1.1/docs/concepts.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     8141 2023-04-28 18:54:19.000000 releases-2.1.1/docs/usage.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-28 19:11:49.000000 releases-2.1.1/setup.cfg
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-06-17 18:56:00.000000 releases-2.1.1/LICENSE
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2022-06-17 18:56:00.000000 releases-2.1.1/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 19:11:49.000000 releases-2.1.1/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3500 2022-12-18 03:30:08.000000 releases-2.1.1/tests/_util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    19083 2023-04-28 18:54:19.000000 releases-2.1.1/tests/organization.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      102 2023-04-28 18:54:19.000000 releases-2.1.1/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    10659 2023-04-28 18:54:19.000000 releases-2.1.1/tests/presentation.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5621 2022-12-19 02:06:53.000000 releases-2.1.1/tests/util.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 19:11:49.000000 releases-2.1.1/releases/
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-28 19:11:48.000000 releases-2.1.1/releases/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    28550 2023-04-28 18:54:19.000000 releases-2.1.1/releases/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9956 2023-04-28 18:54:21.000000 releases-2.1.1/releases/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2556 2023-02-16 19:52:34.000000 releases-2.1.1/releases/line_manager.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7388 2023-02-16 19:52:34.000000 releases-2.1.1/releases/models.py
```

### Comparing `releases-2.1.0/releases.egg-info/PKG-INFO` & `releases-2.1.1/releases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: releases
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Sphinx extension for changelog manipulation
 Home-page: https://github.com/bitprophet/releases
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: UNKNOWN
 Project-URL: Docs, https://releases.readthedocs.io
 Project-URL: Source, https://github.com/bitprophet/releases
```

### Comparing `releases-2.1.0/docs/changelog.rst` & `releases-2.1.1/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+- :release:`2.1.1 <2023-04-28>`
+- :release:`2.0.1 <2023-04-28>`
+- :bug:`-` Fix up an internal utility which monkeypatches a Sphinx/docutils
+  internal, so that it accepts arbitrary args/kwargs instead of exploding on
+  newer Sphinxes.
 - :release:`2.1.0 <2023-02-24>`
 - :feature:`-` Add a new configuration setting,
   ``releases_supported_versions``, allowing you to limit how many "Next 1.x
   feature release" (or bugfix, etc) sections appear at the top of your
   changelog.
 - :feature:`-` Allow controlling the name of your development branch for source
   code links (eg "Next 1.x feature release" section headers) via the new
```

### Comparing `releases-2.1.0/docs/concepts.rst` & `releases-2.1.1/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/docs/usage.rst` & `releases-2.1.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/docs/conf.py` & `releases-2.1.1/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,7 +21,8 @@
 # RTD theme
 html_theme = "sphinx_rtd_theme"
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # Dogfood
 extensions.append("releases")
 releases_github_path = "bitprophet/releases"
+releases_supported_versions = [2]
```

### Comparing `releases-2.1.0/releases/line_manager.py` & `releases-2.1.1/releases/line_manager.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/releases/util.py` & `releases-2.1.1/releases/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         # - bring over all per-line buckets from manager (flattening)
         # Here, all that's left in the per-family bucket should be lines, not
         # unreleased_*
         ret.update(manager[family])
     return ret
 
 
-def _faux_write_doctree(self, docname, doctree):
+def _faux_write_doctree(self, docname, doctree, *args, **kwargs):
     self._read_doctree = doctree
 
 
 def get_doctree(path, **kwargs):
     """
     Obtain a mostly-rendered Sphinx doctree from the RST file at ``path``.
```

### Comparing `releases-2.1.0/releases/models.py` & `releases-2.1.1/releases/models.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/releases/__init__.py` & `releases-2.1.1/releases/__init__.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/tests/_util.py` & `releases-2.1.1/tests/_util.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/tests/presentation.py` & `releases-2.1.1/tests/presentation.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/tests/organization.py` & `releases-2.1.1/tests/organization.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/tests/util.py` & `releases-2.1.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/setup.py` & `releases-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/tasks.py` & `releases-2.1.1/tasks.py`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/PKG-INFO` & `releases-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: releases
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Sphinx extension for changelog manipulation
 Home-page: https://github.com/bitprophet/releases
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: UNKNOWN
 Project-URL: Docs, https://releases.readthedocs.io
 Project-URL: Source, https://github.com/bitprophet/releases
```

### Comparing `releases-2.1.0/LICENSE` & `releases-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `releases-2.1.0/README.rst` & `releases-2.1.1/README.rst`

 * *Files identical despite different names*

