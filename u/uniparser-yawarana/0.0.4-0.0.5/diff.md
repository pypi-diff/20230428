# Comparing `tmp/uniparser_yawarana-0.0.4.tar.gz` & `tmp/uniparser_yawarana-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uniparser_yawarana-0.0.4.tar", last modified: Fri Jun  3 21:54:50 2022, max compression
+gzip compressed data, was "dist/uniparser_yawarana-0.0.5.tar", last modified: Fri Apr 28 20:33:23 2023, max compression
```

## Comparing `uniparser_yawarana-0.0.4.tar` & `uniparser_yawarana-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-06-03 21:54:50.000000 uniparser_yawarana-0.0.4/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      401 2022-06-03 21:54:45.000000 uniparser_yawarana-0.0.4/CITATION.cff
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-02 19:58:24.000000 uniparser_yawarana-0.0.4/LICENSE
--rw-r--r--   0 florianm  (1000) florianm  (1000)       92 2022-04-05 09:00:02.000000 uniparser_yawarana-0.0.4/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2462 2022-06-03 21:54:50.000000 uniparser_yawarana-0.0.4/PKG-INFO
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1476 2022-05-06 06:16:56.000000 uniparser_yawarana-0.0.4/README.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      366 2022-04-04 17:40:04.000000 uniparser_yawarana-0.0.4/pyproject.toml
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1770 2022-06-03 21:54:50.000000 uniparser_yawarana-0.0.4/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-04-04 08:29:49.000000 uniparser_yawarana-0.0.4/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-06-03 21:54:50.000000 uniparser_yawarana-0.0.4/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-06-03 21:54:50.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1655 2022-06-03 21:54:34.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana/__init__.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-06-03 21:54:50.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana/data/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      299 2022-06-03 16:55:34.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana/data/bad_analyses.txt
--rw-r--r--   0 florianm  (1000) florianm  (1000)      547 2022-06-03 16:55:34.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana/data/clitics.txt
--rw-r--r--   0 florianm  (1000) florianm  (1000)      811 2022-06-03 16:55:34.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana/data/disambiguation.cg3
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    29053 2022-06-03 21:54:21.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana/data/lexemes.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     4018 2022-06-03 16:55:34.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana/data/paradigms.txt
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-06-03 21:54:50.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2462 2022-06-03 21:54:49.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      599 2022-06-03 21:54:50.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-06-03 21:54:49.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-06-03 21:54:49.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      221 2022-06-03 21:54:49.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       19 2022-06-03 21:54:49.000000 uniparser_yawarana-0.0.4/src/uniparser_yawarana.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      401 2023-04-28 20:33:19.000000 uniparser_yawarana-0.0.5/CITATION.cff
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-02 19:58:24.000000 uniparser_yawarana-0.0.5/LICENSE
+-rw-r--r--   0 florianm  (1000) florianm  (1000)       92 2022-04-05 09:00:02.000000 uniparser_yawarana-0.0.5/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2198 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1212 2023-03-05 16:32:16.000000 uniparser_yawarana-0.0.5/README.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      366 2022-04-04 17:40:04.000000 uniparser_yawarana-0.0.5/pyproject.toml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1793 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-04-04 08:29:49.000000 uniparser_yawarana-0.0.5/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3656 2023-04-28 20:31:36.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/__init__.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      387 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/bad_analyses.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      282 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/clitics.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3449 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/derivations.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2042 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/disambiguation.cg3
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     8118 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/etym_lookup.yaml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        0 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/lex_rules.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    89222 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/lexemes.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    13143 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/paradigms.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2198 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      730 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      243 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       19 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/top_level.txt
```

### Comparing `uniparser_yawarana-0.0.4/LICENSE` & `uniparser_yawarana-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uniparser_yawarana-0.0.4/PKG-INFO` & `uniparser_yawarana-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniparser_yawarana
-Version: 0.0.4
+Version: 0.0.5
 Summary: A UniParser implementation for morphologically parsing and annotating Yawarana material.
 Home-page: https://github.com/fmatter/uniparser-yawarana
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fmatter/uniparser-yawarana/issues
 Keywords: linguistics,morphology
@@ -23,28 +23,18 @@
 Provides-Extra: publishing
 License-File: LICENSE
 
 # uniparser-yawarana
 
 A morphological parser for Yawarana ([yaba1248](https://glottolog.org/resource/languoid/id/yaba1248), [yar](https://iso639-3.sil.org/code/yar)).
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6510180.svg)](https://doi.org/10.5281/zenodo.6510180)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6510179.svg)](https://doi.org/10.5281/zenodo.6510179)
 ![License](https://img.shields.io/github/license/fmatter/uniparser-yawarana)
-[![Tests](https://img.shields.io/github/workflow/status/fmatter/uniparser-yawarana/tests?label=tests)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/tests.yml)
-[![Linting](https://img.shields.io/github/workflow/status/fmatter/uniparser-yawarana/lint?label=linting)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/lint.yml)
+[![Tests](https://img.shields.io/github/actions/workflow/status/fmatter/uniparser-yawarana/tests.yml?label=tests&branch=main)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/tests.yml)
+[![Linting](https://img.shields.io/github/actions/workflow/status/fmatter/uniparser-yawarana/lint.yml?label=linting&branch=main)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/lint.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/fmatter/uniparser-yawarana)](https://app.codecov.io/gh/fmatter/uniparser-yawarana/)
 [![PyPI](https://img.shields.io/pypi/v/uniparser-yawarana.svg)](https://pypi.org/project/uniparser-yawarana)
 ![Versions](https://img.shields.io/pypi/pyversions/uniparser-yawarana)
 
 This project uses the excellent [uniparser-morph](https://github.com/timarkh/uniparser-morph/) package.
 It is currently under development.
 
-The lexical material is largely sourced from this database:
-
-```
-@unpublished{caceres2020flex,
-title={Yawarana {FLEx} project with partially parsed and glossed texts and corresponding morpheme lexicon from {Natalia} {Cáceres} {Arandia}'s own fieldwork.},
-author={Cáceres Arandia, Natalia},
-year={2020},
-}
-```
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uniparser_yawarana-0.0.4/README.md` & `uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,40 @@
+Metadata-Version: 2.1
+Name: uniparser-yawarana
+Version: 0.0.5
+Summary: A UniParser implementation for morphologically parsing and annotating Yawarana material.
+Home-page: https://github.com/fmatter/uniparser-yawarana
+Author: Florian Matter
+Author-email: florianmatter@gmail.com
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/fmatter/uniparser-yawarana/issues
+Keywords: linguistics,morphology
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: publishing
+License-File: LICENSE
+
 # uniparser-yawarana
 
 A morphological parser for Yawarana ([yaba1248](https://glottolog.org/resource/languoid/id/yaba1248), [yar](https://iso639-3.sil.org/code/yar)).
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6510180.svg)](https://doi.org/10.5281/zenodo.6510180)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6510179.svg)](https://doi.org/10.5281/zenodo.6510179)
 ![License](https://img.shields.io/github/license/fmatter/uniparser-yawarana)
-[![Tests](https://img.shields.io/github/workflow/status/fmatter/uniparser-yawarana/tests?label=tests)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/tests.yml)
-[![Linting](https://img.shields.io/github/workflow/status/fmatter/uniparser-yawarana/lint?label=linting)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/lint.yml)
+[![Tests](https://img.shields.io/github/actions/workflow/status/fmatter/uniparser-yawarana/tests.yml?label=tests&branch=main)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/tests.yml)
+[![Linting](https://img.shields.io/github/actions/workflow/status/fmatter/uniparser-yawarana/lint.yml?label=linting&branch=main)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/lint.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/fmatter/uniparser-yawarana)](https://app.codecov.io/gh/fmatter/uniparser-yawarana/)
 [![PyPI](https://img.shields.io/pypi/v/uniparser-yawarana.svg)](https://pypi.org/project/uniparser-yawarana)
 ![Versions](https://img.shields.io/pypi/pyversions/uniparser-yawarana)
 
 This project uses the excellent [uniparser-morph](https://github.com/timarkh/uniparser-morph/) package.
 It is currently under development.
 
-The lexical material is largely sourced from this database:
-
-```
-@unpublished{caceres2020flex,
-title={Yawarana {FLEx} project with partially parsed and glossed texts and corresponding morpheme lexicon from {Natalia} {Cáceres} {Arandia}'s own fieldwork.},
-author={Cáceres Arandia, Natalia},
-year={2020},
-}
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uniparser_yawarana-0.0.4/setup.cfg` & `uniparser_yawarana-0.0.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	morphology
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = uniparser_yawarana
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/uniparser-yawarana/issues
 url = https://github.com/fmatter/uniparser-yawarana
-version = 0.0.4
+version = 0.0.5
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
@@ -35,15 +35,16 @@
 
 [options.data_files]
 
 [options.extras_require]
 dev = 
 	bump2version
 	coverage [toml]
-	prospector[with_pyroma]
+	prospector[with_pyroma]==1.7.6
+	pylint==2.14.1
 	isort
 	pytest
 	pytest-cov
 	sphinx
 	sphinx_rtd_theme
 	sphinx-autoapi
 	tox
```

### Comparing `uniparser_yawarana-0.0.4/src/uniparser_yawarana.egg-info/SOURCES.txt` & `uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,10 +10,13 @@
 src/uniparser_yawarana.egg-info/SOURCES.txt
 src/uniparser_yawarana.egg-info/dependency_links.txt
 src/uniparser_yawarana.egg-info/not-zip-safe
 src/uniparser_yawarana.egg-info/requires.txt
 src/uniparser_yawarana.egg-info/top_level.txt
 src/uniparser_yawarana/data/bad_analyses.txt
 src/uniparser_yawarana/data/clitics.txt
+src/uniparser_yawarana/data/derivations.txt
 src/uniparser_yawarana/data/disambiguation.cg3
+src/uniparser_yawarana/data/etym_lookup.yaml
+src/uniparser_yawarana/data/lex_rules.txt
 src/uniparser_yawarana/data/lexemes.txt
 src/uniparser_yawarana/data/paradigms.txt
```

