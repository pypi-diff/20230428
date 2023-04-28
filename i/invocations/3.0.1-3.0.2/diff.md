# Comparing `tmp/invocations-3.0.1.tar.gz` & `tmp/invocations-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpd7oszf4e/dist/invocations-3.0.1.tar", last modified: Fri Jan  6 21:46:08 2023, max compression
+gzip compressed data, was "/tmp/tmpubuqxkl9/dist/invocations-3.0.2.tar", last modified: Fri Apr 28 15:17:15 2023, max compression
```

## Comparing `invocations-3.0.1.tar` & `invocations-3.0.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/
--rw-r--r--   0 jforcier  (1000) users      (100)      350 2023-01-06 19:17:20.000000 invocations-3.0.1/dev-requirements.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      243 2022-03-18 00:56:41.000000 invocations-3.0.1/MANIFEST.in
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-03-17 18:07:11.000000 invocations-3.0.1/LICENSE
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)     1116 2022-12-31 22:11:11.000000 invocations-3.0.1/tests/environment.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/autodoc/
--rw-r--r--   0 jforcier  (1000) users      (100)     2752 2022-12-31 22:11:11.000000 invocations-3.0.1/tests/autodoc/base.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/autodoc/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      425 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/autodoc/_support/mytasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)      259 2022-12-31 22:11:11.000000 invocations-3.0.1/tests/autodoc/_support/conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/autodoc/_support/docs/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/
--rw-r--r--   0 jforcier  (1000) users      (100)     3958 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/genindex.html
--rw-r--r--   0 jforcier  (1000) users      (100)     3108 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/py-modindex.html
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/.doctrees/
--rw-r--r--   0 jforcier  (1000) users      (100)     2657 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/.doctrees/index.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)     7645 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/.doctrees/api.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    14029 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle
--rw-r--r--   0 jforcier  (1000) users      (100)     5187 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/api.html
--rw-r--r--   0 jforcier  (1000) users      (100)     3553 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/index.html
--rw-r--r--   0 jforcier  (1000) users      (100)     2861 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/search.html
--rw-r--r--   0 jforcier  (1000) users      (100)     1375 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/searchindex.js
--rw-r--r--   0 jforcier  (1000) users      (100)      230 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/.buildinfo
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_sources/
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_sources/api.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_sources/index.rst.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/
--rw-r--r--   0 jforcier  (1000) users      (100)     4472 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/doctools.js
--rw-r--r--   0 jforcier  (1000) users      (100)     5327 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/pygments.css
--rw-r--r--   0 jforcier  (1000) users      (100)   288580 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js
--rw-r--r--   0 jforcier  (1000) users      (100)    11230 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/alabaster.css
--rw-r--r--   0 jforcier  (1000) users      (100)    14621 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/basic.css
--rw-r--r--   0 jforcier  (1000) users      (100)    19530 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/underscore.js
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/minus.png
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/plus.png
--rw-r--r--   0 jforcier  (1000) users      (100)     4418 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 jforcier  (1000) users      (100)    89501 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/jquery.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4758 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/language_data.js
--rw-r--r--   0 jforcier  (1000) users      (100)      415 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/documentation_options.js
--rw-r--r--   0 jforcier  (1000) users      (100)       42 2022-09-08 21:39:12.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/custom.css
--rw-r--r--   0 jforcier  (1000) users      (100)    18215 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/searchtools.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4712 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
--rw-r--r--   0 jforcier  (1000) users      (100)    68420 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
--rw-r--r--   0 jforcier  (1000) users      (100)      286 2022-12-22 02:25:27.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/file.png
--rw-r--r--   0 jforcier  (1000) users      (100)      296 2022-12-22 02:27:13.000000 invocations-3.0.1/tests/autodoc/_support/docs/_build/objects.inv
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/autodoc/_support/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/autodoc/_support/docs/api.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     3243 2022-10-29 02:26:37.000000 invocations-3.0.1/tests/checks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1890 2022-12-31 22:11:11.000000 invocations-3.0.1/tests/console.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/packaging/
--rw-r--r--   0 jforcier  (1000) users      (100)    48944 2022-12-31 22:11:11.000000 invocations-3.0.1/tests/packaging/release.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/packaging/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      261 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/no_unreleased_1.1_bugs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      185 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/unreleased_1.x_features.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/unreleased_1.1_bugs.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/tests/packaging/_support/fakepackage/
--rw-r--r--   0 jforcier  (1000) users      (100)       13 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/fakepackage/noversion.py
--rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/fakepackage/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/fakepackage/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/fakepackage/otherversion.py
--rw-r--r--   0 jforcier  (1000) users      (100)      179 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/no_unreleased_1.x_features.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/packaging/_support/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1066 2021-12-23 21:30:39.000000 invocations-3.0.1/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2542 2022-12-31 22:11:11.000000 invocations-3.0.1/tests/pytest_.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/docs/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)      233 2021-12-23 21:30:39.000000 invocations-3.0.1/docs/api/packaging.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2021-12-23 21:30:39.000000 invocations-3.0.1/docs/api/environment.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       53 2022-03-18 00:56:41.000000 invocations-3.0.1/docs/api/ci.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-12-23 21:30:39.000000 invocations-3.0.1/docs/api/docs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.0.1/docs/api/autodoc.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.0.1/docs/api/console.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       69 2021-12-23 21:30:39.000000 invocations-3.0.1/docs/api/pytest.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2091 2022-12-31 22:11:11.000000 invocations-3.0.1/docs/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)    11951 2023-01-06 21:46:05.000000 invocations-3.0.1/docs/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      189 2021-12-23 21:30:39.000000 invocations-3.0.1/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2335 2021-12-23 21:30:39.000000 invocations-3.0.1/README.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/invocations.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)     3271 2023-01-06 21:46:08.000000 invocations-3.0.1/invocations.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     4067 2023-01-06 21:46:08.000000 invocations-3.0.1/invocations.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)       12 2023-01-06 21:46:08.000000 invocations-3.0.1/invocations.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      124 2023-01-06 21:46:08.000000 invocations-3.0.1/invocations.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-01-06 21:46:08.000000 invocations-3.0.1/invocations.egg-info/dependency_links.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/invocations/
--rw-r--r--   0 jforcier  (1000) users      (100)     3866 2022-12-31 22:11:11.000000 invocations-3.0.1/invocations/ci.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1982 2022-12-31 22:11:11.000000 invocations-3.0.1/invocations/checks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1942 2023-01-06 21:40:43.000000 invocations-3.0.1/invocations/console.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5009 2022-12-17 18:26:26.000000 invocations-3.0.1/invocations/pytest.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-06 21:46:08.000000 invocations-3.0.1/invocations/packaging/
--rw-r--r--   0 jforcier  (1000) users      (100)     1069 2023-01-06 21:41:39.000000 invocations-3.0.1/invocations/packaging/semantic_version_monkey.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4399 2022-12-31 22:11:11.000000 invocations-3.0.1/invocations/packaging/vendorize.py
--rw-r--r--   0 jforcier  (1000) users      (100)    34040 2022-12-31 22:11:11.000000 invocations-3.0.1/invocations/packaging/release.py
--rw-r--r--   0 jforcier  (1000) users      (100)      296 2021-12-23 21:30:39.000000 invocations-3.0.1/invocations/packaging/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      621 2022-09-08 19:21:52.000000 invocations-3.0.1/invocations/environment.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-01-06 21:46:07.000000 invocations-3.0.1/invocations/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5910 2023-01-06 21:41:13.000000 invocations-3.0.1/invocations/testing.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1264 2021-12-23 21:30:39.000000 invocations-3.0.1/invocations/watch.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6534 2021-12-23 21:30:39.000000 invocations-3.0.1/invocations/docs.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.1/invocations/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      636 2022-06-17 16:03:46.000000 invocations-3.0.1/invocations/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3194 2022-12-31 22:11:11.000000 invocations-3.0.1/invocations/autodoc.py
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-01-06 21:46:08.000000 invocations-3.0.1/setup.cfg
--rw-r--r--   0 jforcier  (1000) users      (100)     4067 2023-01-06 21:46:08.000000 invocations-3.0.1/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     2682 2022-12-31 22:11:11.000000 invocations-3.0.1/setup.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)      124 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     3271 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       12 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      307 2023-01-16 22:33:01.000000 invocations-3.0.2/dev-requirements.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations/packaging/
+-rw-r--r--   0 jforcier  (1000) users      (100)      296 2021-12-23 21:30:39.000000 invocations-3.0.2/invocations/packaging/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4399 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/packaging/vendorize.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1069 2023-01-16 22:33:01.000000 invocations-3.0.2/invocations/packaging/semantic_version_monkey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    34040 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/packaging/release.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1982 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/checks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1942 2023-01-16 22:33:01.000000 invocations-3.0.2/invocations/console.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5009 2022-12-17 18:26:26.000000 invocations-3.0.2/invocations/pytest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1264 2021-12-23 21:30:39.000000 invocations-3.0.2/invocations/watch.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3194 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/autodoc.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6534 2023-04-12 22:47:06.000000 invocations-3.0.2/invocations/docs.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3866 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/ci.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      621 2022-09-08 19:21:52.000000 invocations-3.0.2/invocations/environment.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.2/invocations/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-28 15:17:14.000000 invocations-3.0.2/invocations/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5910 2023-01-16 22:33:01.000000 invocations-3.0.2/invocations/testing.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      636 2022-06-17 16:03:46.000000 invocations-3.0.2/invocations/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-28 15:17:15.000000 invocations-3.0.2/setup.cfg
+-rw-r--r--   0 jforcier  (1000) users      (100)     2335 2021-12-23 21:30:39.000000 invocations-3.0.2/README.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)    12161 2023-04-28 15:17:11.000000 invocations-3.0.2/docs/changelog.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)      233 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/packaging.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       53 2022-03-18 00:56:41.000000 invocations-3.0.2/docs/api/ci.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       69 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/pytest.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/docs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/environment.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/console.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/autodoc.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      189 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2091 2022-12-31 22:11:11.000000 invocations-3.0.2/docs/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2737 2023-04-28 15:16:14.000000 invocations-3.0.2/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-03-17 18:07:11.000000 invocations-3.0.2/LICENSE
+-rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-04-28 15:17:15.000000 invocations-3.0.2/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)      243 2022-03-18 00:56:41.000000 invocations-3.0.2/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1116 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/environment.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2752 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/autodoc/base.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      259 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/autodoc/_support/conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/docs/api.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/docs/index.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/
+-rw-r--r--   0 jforcier  (1000) users      (100)     5187 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/api.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     3108 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/py-modindex.html
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_sources/
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_sources/index.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_sources/api.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     1375 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/searchindex.js
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)     4758 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/language_data.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    14621 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/basic.css
+-rw-r--r--   0 jforcier  (1000) users      (100)     4712 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/plus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)    68420 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/minus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)      415 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/documentation_options.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     5327 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/pygments.css
+-rw-r--r--   0 jforcier  (1000) users      (100)       42 2022-09-08 21:39:12.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/custom.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    18215 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/searchtools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    11230 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/alabaster.css
+-rw-r--r--   0 jforcier  (1000) users      (100)   288580 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    89501 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/jquery.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    19530 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/underscore.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     4472 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/doctools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     4418 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 jforcier  (1000) users      (100)      286 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/file.png
+-rw-r--r--   0 jforcier  (1000) users      (100)     3553 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/index.html
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/
+-rw-r--r--   0 jforcier  (1000) users      (100)     7645 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/api.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    14029 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0 jforcier  (1000) users      (100)     2657 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)      296 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/objects.inv
+-rw-r--r--   0 jforcier  (1000) users      (100)      230 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.buildinfo
+-rw-r--r--   0 jforcier  (1000) users      (100)     3958 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/genindex.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     2861 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/search.html
+-rw-r--r--   0 jforcier  (1000) users      (100)      425 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/mytasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2542 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/pytest_.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1066 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1890 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/console.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/packaging/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/packaging/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      185 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/unreleased_1.x_features.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      179 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/no_unreleased_1.x_features.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/
+-rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/otherversion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       13 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/noversion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      261 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/no_unreleased_1.1_bugs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/unreleased_1.1_bugs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    48944 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/packaging/release.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3243 2022-10-29 02:26:37.000000 invocations-3.0.2/tests/checks.py
```

### Comparing `invocations-3.0.1/LICENSE` & `invocations-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/environment.py` & `invocations-3.0.2/tests/environment.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/base.py` & `invocations-3.0.2/tests/autodoc/base.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/genindex.html` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/genindex.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/py-modindex.html` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/.doctrees/index.doctree` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/.doctrees/api.doctree` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/api.html` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/api.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/index.html` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/index.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/search.html` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/search.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/searchindex.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/searchindex.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/doctools.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/pygments.css` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/alabaster.css` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/basic.css` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/underscore.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/jquery.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/language_data.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/searchtools.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js` & `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/checks.py` & `invocations-3.0.2/tests/checks.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/console.py` & `invocations-3.0.2/tests/console.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/packaging/release.py` & `invocations-3.0.2/tests/packaging/release.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/conftest.py` & `invocations-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/tests/pytest_.py` & `invocations-3.0.2/tests/pytest_.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/docs/conf.py` & `invocations-3.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/docs/changelog.rst` & `invocations-3.0.2/docs/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =========
 Changelog
 =========
 
+- :release:`3.0.2 <2023-04-28>`
+- :support:`- backported` Unpin ``tabulate`` in our install requirements, it's
+  had many more releases since we instituted a defensive pin vs some bugs in
+  its later 0.7 line!
 - :release:`3.0.1 <2023-01-06>`
 - :bug:`-` We neglected to remove references to ``six`` in a few spots -
   including some that utilized Invoke's old vendor of same; this causes issues
   when trying to use development and upcoming versions of Invoke. Six is now
   truly gone!
 - :release:`3.0.0 <2022-12-31>`
 - :support:`-` Various fixes and doc updates re: the `~invocations.autodoc`
```

### Comparing `invocations-3.0.1/README.rst` & `invocations-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations.egg-info/SOURCES.txt` & `invocations-3.0.2/invocations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations.egg-info/PKG-INFO` & `invocations-3.0.2/invocations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invocations
-Version: 3.0.1
+Version: 3.0.2
 Summary: Common/best-practice Invoke tasks and collections
 Home-page: https://invocations.readthedocs.io
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/pyinvoke/invocations
 Project-URL: Changelog, https://invocations.readthedocs.io/en/latest/changelog.html
@@ -18,14 +18,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
```

### Comparing `invocations-3.0.1/invocations/ci.py` & `invocations-3.0.2/invocations/ci.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/checks.py` & `invocations-3.0.2/invocations/checks.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/console.py` & `invocations-3.0.2/invocations/console.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/pytest.py` & `invocations-3.0.2/invocations/pytest.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/packaging/semantic_version_monkey.py` & `invocations-3.0.2/invocations/packaging/semantic_version_monkey.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/packaging/vendorize.py` & `invocations-3.0.2/invocations/packaging/vendorize.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/packaging/release.py` & `invocations-3.0.2/invocations/packaging/release.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/environment.py` & `invocations-3.0.2/invocations/environment.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/testing.py` & `invocations-3.0.2/invocations/testing.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/watch.py` & `invocations-3.0.2/invocations/watch.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/docs.py` & `invocations-3.0.2/invocations/docs.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/util.py` & `invocations-3.0.2/invocations/util.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/invocations/autodoc.py` & `invocations-3.0.2/invocations/autodoc.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.1/PKG-INFO` & `invocations-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invocations
-Version: 3.0.1
+Version: 3.0.2
 Summary: Common/best-practice Invoke tasks and collections
 Home-page: https://invocations.readthedocs.io
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/pyinvoke/invocations
 Project-URL: Changelog, https://invocations.readthedocs.io/en/latest/changelog.html
@@ -18,14 +18,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
```

### Comparing `invocations-3.0.1/setup.py` & `invocations-3.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # NOTE: these used to be all optional (only complained about at import
     # time if missing), but that got hairy fast, and these are all
     # pure-Python packages, so it shouldn't be a huge burden for users to
     # obtain them.
     "blessings>=1.6",
     "releases>=1.6",
     "semantic_version>=2.4,<2.7",
-    "tabulate==0.7.5",
+    "tabulate>=0.7.5",
     "tqdm>=4.8.1",
     "twine>=1.15",
     "wheel>=0.24.0",
 ]
 
 setup(
     name="invocations",
@@ -52,14 +52,15 @@
         "License :: OSI Approved :: BSD License",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development",
```

