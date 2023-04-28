# Comparing `tmp/pkgmt-0.4.2.tar.gz` & `tmp/pkgmt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgmt-0.4.2.tar", last modified: Fri Apr 28 15:30:36 2023, max compression
+gzip compressed data, was "pkgmt-0.5.0.tar", last modified: Fri Apr 28 17:13:47 2023, max compression
```

## Comparing `pkgmt-0.4.2.tar` & `pkgmt-0.5.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.096998 pkgmt-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-28 15:30:19.000000 pkgmt-0.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 15:30:19.000000 pkgmt-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 15:30:19.000000 pkgmt-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 15:30:36.096998 pkgmt-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-28 15:30:19.000000 pkgmt-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 15:30:19.000000 pkgmt-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 15:30:36.096998 pkgmt-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-28 15:30:19.000000 pkgmt-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.088998 pkgmt-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.092998 pkgmt-0.4.2/src/pkgmt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.092998 pkgmt-0.4.2/src/pkgmt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.096998 pkgmt-0.4.2/src/pkgmt/assets/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.088998 pkgmt-0.4.2/src/pkgmt/assets/template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.096998 pkgmt-0.4.2/src/pkgmt/assets/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.088998 pkgmt-0.4.2/src/pkgmt/assets/template/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.096998 pkgmt-0.4.2/src/pkgmt/assets/template/src/name/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/src/name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.096998 pkgmt-0.4.2/src/pkgmt/assets/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/assets/template/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.096998 pkgmt-0.4.2/src/pkgmt/versioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/versioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/versioner/abstractversioner.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/versioner/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/versioner/versionernonsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 15:30:19.000000 pkgmt-0.4.2/src/pkgmt/versioner/versionersetup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:30:36.092998 pkgmt-0.4.2/src/pkgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 15:30:35.000000 pkgmt-0.4.2/src/pkgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-28 15:30:35.000000 pkgmt-0.4.2/src/pkgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:30:35.000000 pkgmt-0.4.2/src/pkgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 15:30:35.000000 pkgmt-0.4.2/src/pkgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 15:30:35.000000 pkgmt-0.4.2/src/pkgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 15:30:35.000000 pkgmt-0.4.2/src/pkgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-28 17:13:33.000000 pkgmt-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 17:13:33.000000 pkgmt-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 17:13:33.000000 pkgmt-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 17:13:47.865345 pkgmt-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-28 17:13:33.000000 pkgmt-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 17:13:33.000000 pkgmt-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 17:13:47.865345 pkgmt-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-28 17:13:33.000000 pkgmt-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.861345 pkgmt-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.861345 pkgmt-0.5.0/src/pkgmt/assets/template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.861345 pkgmt-0.5.0/src/pkgmt/assets/template/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/template/src/name/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/src/name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/versioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/abstractversioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/versionernonsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/versionersetup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/top_level.txt
```

### Comparing `pkgmt-0.4.2/CHANGELOG.md` & `pkgmt-0.5.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # CHANGELOG
 
+## 0.5.0 (2023-04-28)
+
+* [API Change] `pkgmt version` halts if there are uncommitted changes
+
 ## 0.4.2 (2023-04-28)
 
-* [Fix] note: No changes
+*No changes*
 
 ## 0.4.1 (2023-04-28)
 
-* [Fix] note: Never deployed due to a CI error
+*Never deployed due to a CI error*
+
 * [Fix] locking ipython to 8.12.0 on py3.8
 * [Fix] Fixing deprecations error
 
 ## 0.4.0 (2023-04-25)
 
 * [API Change] `pkgmt version` checks out and pulls the main/master branch as the first step
```

### Comparing `pkgmt-0.4.2/LICENSE` & `pkgmt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/README.md` & `pkgmt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/setup.py` & `pkgmt-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     "click",
     "invoke",
     # dependencies for linting and formatting
     "black",
     "nbqa",
     "flake8",
     "jupytext",
+    # ensure we have a valid IPython version since
+    # black needs it
     "ipython<=8.12.0; python_version == '3.8'",
 ]
 
 
 DEV = [
     "pytest",
     "twine",
```

### Comparing `pkgmt-0.4.2/src/pkgmt/assets/template/.github/workflows/ci.yml` & `pkgmt-0.5.0/src/pkgmt/assets/template/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/assets/template/.gitignore` & `pkgmt-0.5.0/src/pkgmt/assets/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/assets/template/setup.py` & `pkgmt-0.5.0/src/pkgmt/assets/template/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/assets/template/tasks.py` & `pkgmt-0.5.0/src/pkgmt/assets/template/tasks.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/changelog.py` & `pkgmt-0.5.0/src/pkgmt/changelog.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/cli.py` & `pkgmt-0.5.0/src/pkgmt/cli.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/config.py` & `pkgmt-0.5.0/src/pkgmt/config.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/dependencies.py` & `pkgmt-0.5.0/src/pkgmt/dependencies.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/deprecation.py` & `pkgmt-0.5.0/src/pkgmt/deprecation.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/dev.py` & `pkgmt-0.5.0/src/pkgmt/dev.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/formatting.py` & `pkgmt-0.5.0/src/pkgmt/formatting.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/github.py` & `pkgmt-0.5.0/src/pkgmt/github.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/hook.py` & `pkgmt-0.5.0/src/pkgmt/hook.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/links.py` & `pkgmt-0.5.0/src/pkgmt/links.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/new.py` & `pkgmt-0.5.0/src/pkgmt/new.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/test.py` & `pkgmt-0.5.0/src/pkgmt/test.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/versioneer.py` & `pkgmt-0.5.0/src/pkgmt/versioneer.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,23 @@
     4. Update header in CHANGELOG file, and ask to review CHANGELOG
     5. Create commit for new version, create git tag, and push
     6. Set new development version in package_name/_version.py, and CHANGELOG
     7. Commit new development version and push
     """
     _git_checkout_main_branch(pull=True)
 
+    pending = subprocess.check_output(["git", "status", "--short"])
+
+    if pending:
+        raise click.ClickException(
+            "Cannot run 'pkgmt version': you have pending files to commit. "
+            "Commit them or discard them and try again.\nDetected files:"
+            f"\n{pending.decode()}"
+        )
+
     if version_package:
         versioner = VersionerNonSetup(version_package, project_root=project_root)
     else:
         versioner = VersionerSetup(project_root=project_root)
 
     changelog_md_exists = (
         versioner.path_to_changelog and versioner.path_to_changelog.suffix == ".md"
```

### Comparing `pkgmt-0.4.2/src/pkgmt/versioner/abstractversioner.py` & `pkgmt-0.5.0/src/pkgmt/versioner/abstractversioner.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/versioner/util.py` & `pkgmt-0.5.0/src/pkgmt/versioner/util.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/versioner/versionernonsetup.py` & `pkgmt-0.5.0/src/pkgmt/versioner/versionernonsetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt/versioner/versionersetup.py` & `pkgmt-0.5.0/src/pkgmt/versioner/versionersetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.4.2/src/pkgmt.egg-info/SOURCES.txt` & `pkgmt-0.5.0/src/pkgmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

