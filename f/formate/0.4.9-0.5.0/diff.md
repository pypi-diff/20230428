# Comparing `tmp/formate-0.4.9.tar.gz` & `tmp/formate-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formate-0.4.9.tar", last modified: Fri Jul  2 08:12:06 2021, max compression
+gzip compressed data, was "formate-0.5.0.tar", last modified: Fri Apr 28 19:30:24 2023, max compression
```

## Comparing `formate-0.4.9.tar` & `formate-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-07-02 08:12:05.992165 formate-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5604 2021-07-02 08:12:06.000165 formate-0.4.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-07-02 08:12:06.000165 formate-0.4.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4632 2021-07-02 08:12:06.000165 formate-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     7261 2021-07-02 08:12:06.076166 formate-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5421 2021-07-02 08:12:05.984165 formate-0.4.9/formate/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2021-07-02 08:12:05.984165 formate-0.4.9/formate/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     6349 2021-07-02 08:12:05.988165 formate-0.4.9/formate/mini_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9250 2021-07-02 08:12:05.988165 formate-0.4.9/formate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2021-07-02 08:12:05.988165 formate-0.4.9/formate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3693 2021-07-02 08:12:05.988165 formate-0.4.9/formate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3826 2021-07-02 08:12:05.988165 formate-0.4.9/formate/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2021-07-02 08:12:05.988165 formate-0.4.9/formate/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-02 08:12:05.984165 formate-0.4.9/formate/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5454 2021-07-02 08:12:05.988165 formate-0.4.9/formate/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9929 2021-07-02 08:12:05.992165 formate-0.4.9/formate/reformat_generics.py
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2021-07-02 08:12:05.992165 formate-0.4.9/formate/dynamic_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7437 2023-04-28 19:30:24.991603 formate-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5669 2023-04-28 19:30:24.991603 formate-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-04-28 19:30:24.991603 formate-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5518 2023-04-28 19:30:24.987603 formate-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-28 19:30:24.979603 formate-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-04-28 19:29:48.075435 formate-0.5.0/formate/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-04-28 19:29:48.075435 formate-0.5.0/formate/mini_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9766 2023-04-28 19:29:48.075435 formate-0.5.0/formate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3127 2023-04-28 19:29:48.075435 formate-0.5.0/formate/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4097 2023-04-28 19:29:48.075435 formate-0.5.0/formate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-04-28 19:29:48.075435 formate-0.5.0/formate/dynamic_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9865 2023-04-28 19:29:48.075435 formate-0.5.0/formate/reformat_generics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3507 2023-04-28 19:29:48.075435 formate-0.5.0/formate/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 19:29:48.075435 formate-0.5.0/formate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5484 2023-04-28 19:29:48.075435 formate-0.5.0/formate/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3854 2023-04-28 19:29:48.075435 formate-0.5.0/formate/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6049 2023-04-28 19:29:48.075435 formate-0.5.0/formate/utils.py
```

### Comparing `formate-0.4.9/LICENSE` & `formate-0.5.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 Dominic Davis-Foster
+Copyright (c) 2021-2022 Dominic Davis-Foster
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `formate-0.4.9/README.rst` & `formate-0.5.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -40,48 +40,48 @@
 	* - Other
 	  - |license| |language| |requires|
 
 .. |docs| image:: https://img.shields.io/readthedocs/formate/latest?logo=read-the-docs
 	:target: https://formate.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
-.. |docs_check| image:: https://github.com/repo-helper/formate/workflows/Docs%20Check/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22Docs+Check%22
+.. |docs_check| image:: https://github.com/python-formate/formate/workflows/Docs%20Check/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
-.. |actions_linux| image:: https://github.com/repo-helper/formate/workflows/Linux/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22Linux%22
+.. |actions_linux| image:: https://github.com/python-formate/formate/workflows/Linux/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22Linux%22
 	:alt: Linux Test Status
 
-.. |actions_windows| image:: https://github.com/repo-helper/formate/workflows/Windows/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22Windows%22
+.. |actions_windows| image:: https://github.com/python-formate/formate/workflows/Windows/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22Windows%22
 	:alt: Windows Test Status
 
-.. |actions_macos| image:: https://github.com/repo-helper/formate/workflows/macOS/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22macOS%22
+.. |actions_macos| image:: https://github.com/python-formate/formate/workflows/macOS/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22macOS%22
 	:alt: macOS Test Status
 
-.. |actions_flake8| image:: https://github.com/repo-helper/formate/workflows/Flake8/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22Flake8%22
+.. |actions_flake8| image:: https://github.com/python-formate/formate/workflows/Flake8/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
-.. |actions_mypy| image:: https://github.com/repo-helper/formate/workflows/mypy/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22mypy%22
+.. |actions_mypy| image:: https://github.com/python-formate/formate/workflows/mypy/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://requires.io/github/repo-helper/formate/requirements.svg?branch=master
-	:target: https://requires.io/github/repo-helper/formate/requirements/?branch=master
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/python-formate/formate/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/python-formate/formate/
 	:alt: Requirements Status
 
-.. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/formate/master?logo=coveralls
-	:target: https://coveralls.io/github/repo-helper/formate?branch=master
+.. |coveralls| image:: https://img.shields.io/coveralls/github/python-formate/formate/master?logo=coveralls
+	:target: https://coveralls.io/github/python-formate/formate?branch=master
 	:alt: Coverage
 
-.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/formate?logo=codefactor
-	:target: https://www.codefactor.io/repository/github/repo-helper/formate
+.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/python-formate/formate?logo=codefactor
+	:target: https://www.codefactor.io/repository/github/python-formate/formate
 	:alt: CodeFactor Grade
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/formate
 	:target: https://pypi.org/project/formate/
 	:alt: PyPI - Package Version
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/formate?logo=python&logoColor=white
@@ -100,30 +100,30 @@
 	:target: https://anaconda.org/domdfcoding/formate
 	:alt: Conda - Package Version
 
 .. |conda-platform| image:: https://img.shields.io/conda/pn/domdfcoding/formate?label=conda%7Cplatform
 	:target: https://anaconda.org/domdfcoding/formate
 	:alt: Conda - Platform
 
-.. |license| image:: https://img.shields.io/github/license/repo-helper/formate
-	:target: https://github.com/repo-helper/formate/blob/master/LICENSE
+.. |license| image:: https://img.shields.io/github/license/python-formate/formate
+	:target: https://github.com/python-formate/formate/blob/master/LICENSE
 	:alt: License
 
-.. |language| image:: https://img.shields.io/github/languages/top/repo-helper/formate
+.. |language| image:: https://img.shields.io/github/languages/top/python-formate/formate
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/formate/v0.4.9
-	:target: https://github.com/repo-helper/formate/pulse
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/formate/v0.5.0
+	:target: https://github.com/python-formate/formate/pulse
 	:alt: GitHub commits since tagged version
 
-.. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/formate
-	:target: https://github.com/repo-helper/formate/commit/master
+.. |commits-latest| image:: https://img.shields.io/github/last-commit/python-formate/formate
+	:target: https://github.com/python-formate/formate/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/formate
 	:target: https://pypi.org/project/formate/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `formate-0.4.9/pyproject.toml` & `formate-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "formate"
-version = "0.4.9"
+version = "0.5.0"
 description = "Python formatting mate."
 readme = "README.rst"
 keywords = [ "formatting", "linting",]
 dynamic = []
 dependencies = [
     "astatine>=0.3.1",
     "asttokens>=2.0.4",
     "attr-utils>=0.5.5",
     "attrs>=20.3.0",
     "click>=7.1.2",
     "consolekit>=1.0.0",
     "dom-toml>=0.4.0",
     "domdf-python-tools>=2.5.0",
-    "isort<5.10.0,>=5.5.2",
+    "isort<5.11.0,>=5.5.2",
     "prettyprinter>=0.18.0",
     "typing-extensions>=3.7.4.3",
-    "yapf<0.32.0,>=0.30.0",
+    "yapf<0.33.0,>=0.30.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Typing :: Typed",
@@ -46,74 +48,78 @@
 email = "dominic@davis-foster.co.uk"
 
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
-Homepage = "https://github.com/repo-helper/formate"
-"Issue Tracker" = "https://github.com/repo-helper/formate/issues"
-"Source Code" = "https://github.com/repo-helper/formate"
+Homepage = "https://github.com/python-formate/formate"
+"Issue Tracker" = "https://github.com/python-formate/formate/issues"
+"Source Code" = "https://github.com/python-formate/formate"
 Documentation = "https://formate.readthedocs.io/en/latest"
 
 [project.scripts]
 formate = "formate.__main__:main"
 
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
 extras = "all"
 
 [tool.dep_checker]
 allowed_unused = [ "prettyprinter",]
 
 [tool.sphinx-pyproject]
-github_username = "repo-helper"
+github_username = "python-formate"
 github_repository = "formate"
 author = "Dominic Davis-Foster"
 project = "formate"
-copyright = "2020-2021 Dominic Davis-Foster"
+copyright = "2020-2022 Dominic Davis-Foster"
 language = "en"
 package_root = "formate"
 extensions = [
     "sphinx_toolbox",
     "sphinx_toolbox.more_autodoc",
     "sphinx_toolbox.more_autosummary",
     "sphinx_toolbox.documentation_summary",
     "sphinx_toolbox.tweaks.param_dash",
+    "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
     "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
-    "sphinxcontrib.toctree_plus",
     "sphinx_debuginfo",
+    "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
+    "html_section",
     "attr_utils.autoattrs",
     "sphinx_click",
     "sphinx_toolbox.pre_commit",
-    "sphinx_toolbox_experimental.html_section",
-    "sphinx_toolbox_experimental.autosummary_widths",
+    "sphinx_toolbox.more_autosummary.column_widths",
+    "sphinx_favicon",
+    "sphinx_toolbox_experimental.changelog",
     "sphinx_toolbox_experimental.missing_xref",
+    "local_extension",
 ]
 sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
@@ -136,14 +142,15 @@
     "role",
     "typeddict",
 ]
 add_module_names = false
 hide_none_rtype = true
 all_typevars = true
 overloads_location = "bottom"
+html_codeblock_linenos_style = "table"
 autodoc_exclude_members = [
     "__dict__",
     "__class__",
     "__dir__",
     "__weakref__",
     "__module__",
     "__annotations__",
@@ -155,19 +162,52 @@
     "__init__",
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
+[tool.mypy]
+python_version = "3.8"
+namespace_packages = true
+check_untyped_defs = true
+warn_unused_ignores = true
+no_implicit_optional = true
+plugins = [ "attr_utils.mypy_plugin",]
+show_error_codes = true
+
+[tool.snippet-fmt]
+directives = [ "code-block",]
+
 [project.entry-points.formate_hooks]
 reformat-generics = "formate.reformat_generics:reformat_generics"
 dynamic_quotes = "formate.dynamic_quotes:dynamic_quotes"
 noqa_reformat = "formate.mini_hooks:noqa_reformat"
 squish_stubs = "formate.mini_hooks:squish_stubs"
 ellipsis_reformat = "formate.ellipses:ellipsis_reformat"
 collections-import-rewrite = "formate.imports:rewrite_collections_abc_imports"
 isort = "formate:isort_hook"
 yapf = "formate:yapf_hook"
 
 [tool.dep_checker.name_mapping]
 attrs = "attr"
+
+[tool.dependency-dash."requirements.txt"]
+order = 10
+
+[tool.dependency-dash."tests/requirements.txt"]
+order = 20
+include = false
+
+[tool.dependency-dash."doc-source/requirements.txt"]
+order = 30
+include = false
+
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.TOML]
+reformat = true
+
+[tool.snippet-fmt.languages.ini]
+
+[tool.snippet-fmt.languages.json]
```

### Comparing `formate-0.4.9/PKG-INFO` & `formate-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: formate
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python formatting mate.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: formatting,linting
-Home-page: https://github.com/repo-helper/formate
-Project-URL: Issue Tracker, https://github.com/repo-helper/formate/issues
-Project-URL: Source Code, https://github.com/repo-helper/formate
+Home-page: https://github.com/python-formate/formate
+Project-URL: Issue Tracker, https://github.com/python-formate/formate/issues
+Project-URL: Source Code, https://github.com/python-formate/formate
 Project-URL: Documentation, https://formate.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -19,30 +19,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: astatine>=0.3.1
 Requires-Dist: asttokens>=2.0.4
 Requires-Dist: attr-utils>=0.5.5
 Requires-Dist: attrs>=20.3.0
 Requires-Dist: click>=7.1.2
 Requires-Dist: consolekit>=1.0.0
 Requires-Dist: dom-toml>=0.4.0
 Requires-Dist: domdf-python-tools>=2.5.0
-Requires-Dist: isort<5.10.0,>=5.5.2
+Requires-Dist: isort<5.11.0,>=5.5.2
 Requires-Dist: prettyprinter>=0.18.0
 Requires-Dist: typing-extensions>=3.7.4.3
-Requires-Dist: yapf<0.32.0,>=0.30.0
+Requires-Dist: yapf<0.33.0,>=0.30.0
 Description-Content-Type: text/x-rst
 
 
 ########
 formate
 ########
 
@@ -84,48 +86,48 @@
 	* - Other
 	  - |license| |language| |requires|
 
 .. |docs| image:: https://img.shields.io/readthedocs/formate/latest?logo=read-the-docs
 	:target: https://formate.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
-.. |docs_check| image:: https://github.com/repo-helper/formate/workflows/Docs%20Check/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22Docs+Check%22
+.. |docs_check| image:: https://github.com/python-formate/formate/workflows/Docs%20Check/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
-.. |actions_linux| image:: https://github.com/repo-helper/formate/workflows/Linux/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22Linux%22
+.. |actions_linux| image:: https://github.com/python-formate/formate/workflows/Linux/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22Linux%22
 	:alt: Linux Test Status
 
-.. |actions_windows| image:: https://github.com/repo-helper/formate/workflows/Windows/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22Windows%22
+.. |actions_windows| image:: https://github.com/python-formate/formate/workflows/Windows/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22Windows%22
 	:alt: Windows Test Status
 
-.. |actions_macos| image:: https://github.com/repo-helper/formate/workflows/macOS/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22macOS%22
+.. |actions_macos| image:: https://github.com/python-formate/formate/workflows/macOS/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22macOS%22
 	:alt: macOS Test Status
 
-.. |actions_flake8| image:: https://github.com/repo-helper/formate/workflows/Flake8/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22Flake8%22
+.. |actions_flake8| image:: https://github.com/python-formate/formate/workflows/Flake8/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
-.. |actions_mypy| image:: https://github.com/repo-helper/formate/workflows/mypy/badge.svg
-	:target: https://github.com/repo-helper/formate/actions?query=workflow%3A%22mypy%22
+.. |actions_mypy| image:: https://github.com/python-formate/formate/workflows/mypy/badge.svg
+	:target: https://github.com/python-formate/formate/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://requires.io/github/repo-helper/formate/requirements.svg?branch=master
-	:target: https://requires.io/github/repo-helper/formate/requirements/?branch=master
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/python-formate/formate/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/python-formate/formate/
 	:alt: Requirements Status
 
-.. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/formate/master?logo=coveralls
-	:target: https://coveralls.io/github/repo-helper/formate?branch=master
+.. |coveralls| image:: https://img.shields.io/coveralls/github/python-formate/formate/master?logo=coveralls
+	:target: https://coveralls.io/github/python-formate/formate?branch=master
 	:alt: Coverage
 
-.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/formate?logo=codefactor
-	:target: https://www.codefactor.io/repository/github/repo-helper/formate
+.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/python-formate/formate?logo=codefactor
+	:target: https://www.codefactor.io/repository/github/python-formate/formate
 	:alt: CodeFactor Grade
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/formate
 	:target: https://pypi.org/project/formate/
 	:alt: PyPI - Package Version
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/formate?logo=python&logoColor=white
@@ -144,30 +146,30 @@
 	:target: https://anaconda.org/domdfcoding/formate
 	:alt: Conda - Package Version
 
 .. |conda-platform| image:: https://img.shields.io/conda/pn/domdfcoding/formate?label=conda%7Cplatform
 	:target: https://anaconda.org/domdfcoding/formate
 	:alt: Conda - Platform
 
-.. |license| image:: https://img.shields.io/github/license/repo-helper/formate
-	:target: https://github.com/repo-helper/formate/blob/master/LICENSE
+.. |license| image:: https://img.shields.io/github/license/python-formate/formate
+	:target: https://github.com/python-formate/formate/blob/master/LICENSE
 	:alt: License
 
-.. |language| image:: https://img.shields.io/github/languages/top/repo-helper/formate
+.. |language| image:: https://img.shields.io/github/languages/top/python-formate/formate
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/formate/v0.4.9
-	:target: https://github.com/repo-helper/formate/pulse
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/formate/v0.5.0
+	:target: https://github.com/python-formate/formate/pulse
 	:alt: GitHub commits since tagged version
 
-.. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/formate
-	:target: https://github.com/repo-helper/formate/commit/master
+.. |commits-latest| image:: https://img.shields.io/github/last-commit/python-formate/formate
+	:target: https://github.com/python-formate/formate/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/formate
 	:target: https://pypi.org/project/formate/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `formate-0.4.9/formate/classes.py` & `formate-0.5.0/formate/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # 3rd party
 import attr
 from attr_utils.pprinter import pretty_repr
 from attr_utils.serialise import serde
 from domdf_python_tools.typing import PathLike
 from typing_extensions import TypedDict
 
-__all__ = ["FormateConfigDict", "ExpandedHookDict", "HooksMapping", "EntryPoint", "Hook"]
+__all__ = ("FormateConfigDict", "ExpandedHookDict", "HooksMapping", "EntryPoint", "Hook")
 
 #: Type hint for the ``hooks`` key of the ``formate`` configuration mapping.
 HooksMapping = Mapping[str, Union[int, "ExpandedHookDict"]]
 
 
 class FormateConfigDict(TypedDict, total=False):
 	"""
@@ -79,15 +79,15 @@
 @pretty_repr
 @serde
 @attr.s
 class Hook:
 	"""
 	Represents a ``formate`` reformatting hook.
 
-	.. autosummary-widths:: 6/16 10/16
+	.. autosummary-widths:: 6/16
 	"""
 
 	#: The name of the hook. The name is normalized into lowercase, with underscores replaced by hyphens.
 	name: str = attr.ib()
 
 	#: The priority of the hook.
 	priority: int = attr.ib(default=10)
@@ -100,15 +100,15 @@
 
 	entry_point: Optional["EntryPoint"] = attr.ib(default=None)
 
 	#: A read-only view on the global configuration mapping, for hooks to do with as they wish.
 	global_config: Mapping[str, Any] = attr.ib(factory=dict)
 
 	@name.validator
-	def _normalize(self, attribute, value):
+	def _normalize(self, attribute, value):  # noqa: MAN001,MAN002
 		# this package
 		from formate.utils import _normalize_pattern
 
 		self.name = _normalize_pattern.sub('-', value).lower()
 
 	@classmethod
 	def parse(cls, data: HooksMapping) -> Iterator["Hook"]:
@@ -163,21 +163,21 @@
 	#: The name of the entry point. The name is normalized into lowercase, with underscores replaced by hyphens.
 	name: str = attr.ib()
 
 	#: The object the entry point refers to.
 	obj: Callable[..., str] = attr.ib()
 
 	@name.validator
-	def _normalize(self, attribute, value):
+	def _normalize(self, attribute, value):  # noqa: MAN001,MAN002
 		# this package
 		from formate.utils import _normalize_pattern
 
 		self.name = _normalize_pattern.sub('-', value).lower()
 
 	@obj.validator
-	def _validate_obj(self, attribute, value):
+	def _validate_obj(self, attribute, value):  # noqa: MAN001,MAN002
 		if not callable(value):
 			raise TypeError(f"Entry points must be callables (e.g. classes and functions), not {type(value)!r}.")
 
 
 if EntryPoint.to_dict.__doc__ is not None:
 	EntryPoint.to_dict.__doc__ += "\n\n:rtype:\n\n.. raw:: latex\n\n\t\\clearpage"
```

### Comparing `formate-0.4.9/formate/imports.py` & `formate-0.5.0/formate/imports.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 # 3rd party
 from domdf_python_tools.stringlist import DelimitedList
 
 # this package
 from formate.utils import Rewriter
 
-__all__ = ["CollectionsABCRewriter", "rewrite_collections_abc_imports"]
+__all__ = ("CollectionsABCRewriter", "rewrite_collections_abc_imports")
 
 
 class CollectionsABCRewriter(Rewriter):
 	"""
 	Identify deprecated :file:`from collections import {<abc>}` imports,
 	and rewrite them as :file:`from collections.abc import {<abc>}`.
 
@@ -59,15 +59,15 @@
 		new_imports = []
 
 		collections_abc_imports: DelimitedList[str] = DelimitedList()
 		collections_imports: DelimitedList[str] = DelimitedList()
 
 		name: ast.alias
 		for name in node.names:
-			if name.name in collections.abc.__all__:
+			if name.name in collections.abc.__all__:  # pylint: disable=dotted-import-in-loop
 				collections_abc_imports.append(name.name)
 			else:
 				collections_imports.append(name.name)
 
 		text_range = self.tokens.get_text_range(node)
 
 		if collections_abc_imports:
```

### Comparing `formate-0.4.9/formate/mini_hooks.py` & `formate-0.5.0/formate/mini_hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from domdf_python_tools.paths import PathPlus
 from domdf_python_tools.stringlist import StringList
 from domdf_python_tools.typing import PathLike
 
 # this package
 from formate.config import wants_filename
 
-__all__ = ["noqa_reformat", "check_ast", "squish_stubs"]
+__all__ = ("noqa_reformat", "check_ast", "squish_stubs")
 
 
 def noqa_reformat(source: str) -> str:
 	"""
 	Pull ``# noqa: ...`` comments that immediately follow docstrings back up to the end of the correct line.
 
 	:param source: The source to reformat.
@@ -114,14 +114,17 @@
 class _MultilineFunction(_Function):
 	pass
 
 
 def _breakup_source(source: str) -> List[List[str]]:
 	blocks: List[List[str]] = [[]]
 
+	split_az_re = re.compile("[A-Za-z]")
+	split_az_underscore_re = re.compile("[A-Za-z)*_]")
+
 	for line in source.split('\n'):
 		if not line.strip():
 			if isinstance(blocks[-1], _Variables):
 				blocks[-1].append(line)
 
 		elif line.lstrip().startswith('@'):
 			if isinstance(blocks[-1], _Decorator):
@@ -141,20 +144,20 @@
 
 		elif line.rstrip().startswith(' ') or line.startswith('\t'):
 			if isinstance(blocks[-1], _Class):
 				blocks[-1].append(line)
 			elif isinstance(blocks[-1], _MultilineFunction):
 				if len(blocks[-1]) < 2:
 					blocks[-1].append(line)
-				elif re.split("[A-Za-z)*_]", line)[0] == re.split("[A-Za-z)*_]", blocks[-1][-1])[0]:
+				elif split_az_underscore_re.split(line)[0] == split_az_underscore_re.split(blocks[-1][-1])[0]:
 					blocks[-1].append(line)
 				else:
 					blocks.append(_Variables([line]))
 			elif isinstance(blocks[-1], _Function):
-				if re.split("[A-Za-z]", line)[0] == re.split("[A-Za-z]", blocks[-1][-1])[0]:
+				if split_az_re.split(line)[0] == split_az_re.split(blocks[-1][-1])[0]:
 					blocks.append(_Variables([line]))
 				elif line.rstrip().endswith(','):
 					blocks[-1] = _MultilineFunction([*blocks[-1], line])
 				else:
 					blocks.append(_Variables([line]))
 
 			elif isinstance(blocks[-1], _Variables):
@@ -167,27 +170,32 @@
 				blocks[-1].append(line)
 			else:
 				blocks.append(_Variables([line]))
 
 	return blocks
 
 
-def _reformat_blocks(blocks: List[List[str]]):
+def _reformat_blocks(blocks: List[List[str]]) -> StringList:
 
 	cursor = 1
 
+	tab_re = re.compile("^[ \t]+")
+
 	while cursor < len(blocks):
 
+		# pylint: disable=loop-invariant-statement
 		if isinstance(blocks[cursor - 1], (_MultilineFunction, _DecoratedFunction, _Class)):
 			# Add a blank line after _Variables, a multi-line function, or a decorated function
 			blocks.insert(cursor, [])
 			cursor += 1
 
-		if blocks[cursor] and blocks[cursor - 1] and re.match("^[ \t]+", blocks[cursor - 1][-1]
-																) and not re.match("^[ \t]+", blocks[cursor][0]):
+		if (
+				blocks[cursor] and blocks[cursor - 1] and tab_re.match(blocks[cursor - 1][-1])
+				and not tab_re.match(blocks[cursor][0])
+				):
 			# Add a blank line after a dedent
 			blocks.insert(cursor, [])
 			cursor += 1
 
 		if isinstance(blocks[cursor - 1], _Variables):
 			# Add a blank line before and after _Variables
 			blocks.insert(cursor - 1, [])
@@ -208,14 +216,15 @@
 		if isinstance(blocks[cursor], _Class):
 
 			if (
 					cursor + 1 < len(blocks) and isinstance(blocks[cursor + 1], _Function)
 					and not isinstance(blocks[cursor + 1], (_DecoratedFunction, _MultilineFunction))
 					and blocks[cursor][-1].lstrip().startswith("class") and blocks[cursor + 1][0][0].isspace()
 					):
+				# pylint: enable=loop-invariant-statement
 				blocks.insert(cursor, [])
 				cursor += 2
 			else:
 				blocks.insert(cursor, [])
 				blocks.insert(cursor + 2, [])
 				cursor += 3
```

### Comparing `formate-0.4.9/formate/__init__.py` & `formate-0.5.0/formate/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,23 +40,23 @@
 from domdf_python_tools.typing import PathLike
 from domdf_python_tools.words import TAB
 from isort.exceptions import FileSkipComment
 
 # this package
 from formate.classes import FormateConfigDict, Hook
 from formate.config import parse_hooks, wants_filename, wants_global_config
-from formate.utils import syntaxerror_for_file
+from formate.utils import _find_from_parents, syntaxerror_for_file
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.4.9"
+__version__: str = "0.5.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
-__all__ = ["call_hooks", "reformat_file", "Reformatter", "isort_hook", "yapf_hook"]
+__all__ = ("call_hooks", "reformat_file", "Reformatter", "isort_hook", "yapf_hook")
 
 # TODO: Ideas for hooks
 # * https://github.com/asottile/add-trailing-comma
 # * Replace collections imports with their typing equivalents where possible.
 # * nested with block reformat, dependent on linelength
 # * replace typing imports with typing_extensions where necessary. Needs min version flag
 # * replace e.g `import numpy as np` with `import numpy` and update all usages
@@ -140,15 +140,15 @@
 
 		parsed_kwargs = {}
 		import_headings = {}
 
 		for option, value in kwargs.items():
 			if option.startswith("import_heading"):
 				import_headings[option[len("import_heading") + 1:]] = value
-			elif option in isort_string_or_sequence:
+			elif option in isort_string_or_sequence:  # pylint: disable=loop-global-usage
 				if isinstance(value, str):
 					value = (value, )
 				elif not isinstance(value, Sequence):
 					value = (value, )
 
 				parsed_kwargs[option] = value
 
@@ -175,22 +175,29 @@
 	r"""
 	Call `yapf <https://github.com/google/yapf>`_, using the given keyword arguments as its configuration.
 
 	:param source: The source to reformat.
 	:param formate_global_config: The global configuration dictionary. Optional.
 	:param \*\*kwargs:
 
+	If ``yapf_style`` is given as a keyword argument, use that style.
+	If a filename is given as the style it is searched for in the current and parent directories, and the style taken from the configuration in that file.
+
 	:returns: The reformatted source.
 	"""
 
 	# 3rd party
-	from yapf.yapflib.yapf_api import FormatCode  # type: ignore
+	from yapf.yapflib.yapf_api import FormatCode  # type: ignore[import]
 
 	if "yapf_style" in kwargs:
-		return FormatCode(source, style_config=str(kwargs["yapf_style"]))[0]
+		# yapf_style may be a filename or the name of a style
+		# If `yapf_style` is a filename (or the name of a style, as opposed to a path), look in CWD and parent directories
+		yapf_style = _find_from_parents(PathPlus(kwargs["yapf_style"]))
+
+		return FormatCode(source, style_config=str(yapf_style))[0]
 
 	else:
 		if "use_tabs" not in kwargs and formate_global_config:
 			if "indent" in (formate_global_config or {}):
 				kwargs["use_tabs"] = formate_global_config["indent"] == TAB
 
 		if "column_limit" not in kwargs and formate_global_config:
@@ -212,15 +219,15 @@
 class Reformatter:
 	"""
 	Reformat a Python source file.
 
 	:param filename: The filename to reformat.
 	:param config: The ``formate`` configuration, parsed from a TOML file (or similar).
 
-	.. autosummary-widths:: 5/16 11/16
+	.. autosummary-widths:: 5/16
 	"""
 
 	#: The filename being reformatted.
 	filename: str
 
 	#: The filename being reformatted, as a POSIX-style path.
 	file_to_format: PathPlus
@@ -292,15 +299,15 @@
 		self.file_to_format.write_text(self.to_string())
 
 
 def reformat_file(
 		filename: PathLike,
 		config: FormateConfigDict,
 		colour: ColourTrilean = None,
-		):
+		) -> int:
 	"""
 	Reformat the given file, and show the diff if changes were made.
 
 	:param filename: The filename to reformat.
 	:param config: The ``formate`` configuration, parsed from a TOML file (or similar).
 	:param colour: Whether to force coloured output on (:py:obj:`True`) or off (:py:obj:`False`).
```

### Comparing `formate-0.4.9/formate/exceptions.py` & `formate-0.5.0/formate/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # this package
 from formate.classes import Hook
 
-__all__ = ["HookNotFoundError"]
+__all__ = ("HookNotFoundError", )
 
 
 class HookNotFoundError(ValueError):
 	"""
 	Exception to indicate the specified hook could not be found.
 	"""
```

### Comparing `formate-0.4.9/formate/__main__.py` & `formate-0.5.0/formate/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,16 +36,17 @@
 from consolekit.options import MultiValueOption, colour_option, flag_option, verbose_option
 from consolekit.terminal_colours import ColourTrilean, resolve_color_default
 from consolekit.tracebacks import handle_tracebacks, traceback_option
 from domdf_python_tools.typing import PathLike
 
 # this package
 from formate import Reformatter
+from formate.utils import _find_from_parents
 
-__all__ = ["main"]
+__all__ = ("main", )
 
 
 @flag_option("--diff", "show_diff", help="Show a diff of changes made")
 @traceback_option()
 @colour_option()
 @verbose_option()
 @click.option(
@@ -56,29 +57,32 @@
 		cls=MultiValueOption,
 		help="Patterns for files to exclude from formatting.",
 		)
 @click.option(
 		"-c",
 		"--config-file",
 		type=click.STRING,
-		help="The path to the TOML configuration file to use.",
+		help=(
+				"The path or filename of the TOML configuration file to use. "
+				"If a filename is given it is searched for in the current and parent directories."
+				),
 		default="formate.toml",
 		show_default=True,
 		)
 @click.argument("filename", type=click.STRING, nargs=-1)
 @click_command()
 def main(
 		filename: Iterable[PathLike],
 		config_file: PathLike,
 		exclude: "Optional[List[str]]",
 		colour: "ColourTrilean" = None,
 		verbose: bool = False,
 		show_traceback: bool = False,
 		show_diff: bool = False,
-		):
+		) -> None:
 	"""
 	Reformat the given Python source files.
 	"""
 
 	# stdlib
 	import fnmatch
 	import re
@@ -88,27 +92,30 @@
 
 	# this package
 	from formate.config import load_toml
 	from formate.utils import SyntaxTracebackHandler, syntaxerror_for_file
 
 	retv = 0
 
+	# If `config_file` is a filename (rather than a path), look in CWD and parent directories
+	config_file = _find_from_parents(PathPlus(config_file))
+
 	try:
 		config = load_toml(config_file)
 	except FileNotFoundError:
 		raise click.UsageError(f"Config file '{config_file}' not found")
 
 	for path in filename:
 		for pattern in exclude or []:
-			if re.match(fnmatch.translate(pattern), str(path)):
+			if re.match(fnmatch.translate(pattern), str(path)):  # pylint: disable=loop-invariant-statement
 				continue
 
 		path = PathPlus(path)
 
-		if path.suffix not in {".py", ".pyi", ''} or path.is_dir():
+		if path.suffix not in {".py", ".pyi", ''} or path.is_dir():  # pylint: disable=loop-invariant-statement
 			if verbose >= 2:
 				click.echo(f"Skipping {path} as it doesn't appear to be a Python file")
 
 			continue
 
 		r = Reformatter(path, config=config)
```

### Comparing `formate-0.4.9/formate/config.py` & `formate-0.5.0/formate/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import dom_toml
 from domdf_python_tools.typing import PathLike
 
 # this package
 from formate.classes import FormateConfigDict, Hook
 from formate.utils import import_entry_points
 
-__all__ = ["parse_hooks", "parse_global_config", "load_toml", "wants_global_config", "wants_filename", "_C_str"]
+__all__ = ("parse_hooks", "parse_global_config", "load_toml", "wants_global_config", "wants_filename", "_C_str")
 
 _C_str = TypeVar("_C_str", bound=Callable[..., str])
 
 
 def parse_hooks(config: Mapping) -> List[Hook]:
 	"""
 	Given a mapping parsed from a TOML file (or similar), return a list of hooks selected by the user.
@@ -105,15 +105,15 @@
 	Decorator to indicate to ``formate`` that the global configuration should be passed to this hook.
 
 	The configuration will be provided as the ``formate_global_config``: :class:`~typing.Mapping` keyword argument.
 
 	:param func:
 	"""
 
-	func.wants_global_config = True  # type: ignore
+	func.wants_global_config = True  # type: ignore[attr-defined]
 	return func
 
 
 def wants_filename(func: _C_str) -> _C_str:
 	"""
 	Decorator to indicate to ``formate`` that the filename being reformatted should be passed to this hook.
 
@@ -121,9 +121,9 @@
 	``formate_filename``: :py:obj:`~domdf_python_tools.typing.PathLike` keyword argument.
 
 	.. versionadded:: 0.2.0
 
 	:param func:
 	"""
 
-	func.wants_filename = True  # type: ignore
+	func.wants_filename = True  # type: ignore[attr-defined]
 	return func
```

### Comparing `formate-0.4.9/formate/ellipses.py` & `formate-0.5.0/formate/ellipses.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 import re
 import sys
 from typing import Union
 
 # this package
 from formate.utils import Rewriter
 
-__all__ = ["EllipsisRewriter", "ellipsis_reformat"]
+__all__ = ("EllipsisRewriter", "ellipsis_reformat")
 
 
 class EllipsisRewriter(Rewriter):
 	"""
 	Move ellipses (``...``) for type stubs onto the end of the stub definition.
 
 	:param source: The source to reformat.
@@ -62,15 +62,15 @@
 			self,
 			node: Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef],
 			) -> None:
 		"""
 		Responsible for the actual rewriting.
 		"""
 
-		if not node.body:
+		if not node.body:  # pragma: no cover
 			return
 
 		if not isinstance(node.body[0], ast.Expr):
 			return
 
 		if not isinstance(node.body[0].value, (ast.Constant, ast.Ellipsis)):
 			return
```

### Comparing `formate-0.4.9/formate/utils.py` & `formate-0.5.0/formate/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,34 +25,39 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import ast
 import os
+import pathlib
 import re
 import sys
 from contextlib import contextmanager
 from itertools import starmap
 from operator import itemgetter
-from typing import Dict, List, Tuple
+from typing import TYPE_CHECKING, Dict, Iterator, List, Tuple, TypeVar
 
 # 3rd party
-import asttokens  # type: ignore
+import asttokens
 import click
 from consolekit import terminal_colours
 from consolekit.tracebacks import TracebackHandler
 from domdf_python_tools.import_tools import discover_entry_points_by_name
 from domdf_python_tools.typing import PathLike
 
 # this package
 from formate.classes import EntryPoint, Hook
 from formate.exceptions import HookNotFoundError
 
-__all__ = ["import_entry_points", "normalize", "syntaxerror_for_file", "Rewriter", "SyntaxTracebackHandler"]
+if TYPE_CHECKING:
+	# stdlib
+	from typing import NoReturn
+
+__all__ = ("import_entry_points", "normalize", "syntaxerror_for_file", "Rewriter", "SyntaxTracebackHandler")
 
 _normalize_pattern = re.compile(r"[-_.]+")
 
 
 def normalize(name: str) -> str:
 	"""
 	Normalize the given name into lowercase, with underscores replaced by hyphens.
@@ -96,15 +101,15 @@
 	return {e.name: e for e in (starmap(EntryPoint, entry_points.items()))}
 
 
 class Rewriter(ast.NodeVisitor):
 	"""
 	ABC for rewriting Python source files from an AST and a token stream.
 
-	.. autosummary-widths:: 8/16 8/16
+	.. autosummary-widths:: 8/16
 	"""
 
 	#: The original source.
 	source: str
 
 	#: The tokenized source.
 	tokens: asttokens.ASTTokens
@@ -118,34 +123,38 @@
 	"""
 
 	def __init__(self, source: str):
 		self.source = source
 		self.tokens = asttokens.ASTTokens(source, parse=True)
 		self.replacements: List[Tuple[Tuple[int, int], str]] = []
 
+		assert self.tokens.tree is not None
+
 	def rewrite(self) -> str:
 		"""
 		Rewrite the source and return the new source.
 
 		:returns: The reformatted source.
 		"""
 
-		self.visit(self.tokens.tree)
+		tree = self.tokens.tree
+		assert tree is not None
+		self.visit(tree)
 
 		reformatted_source = self.source
 
 		# Work from the bottom up
 		for (start, end), replacement in sorted(self.replacements, key=itemgetter(0), reverse=True):
 			source_before = reformatted_source[:start]
 			source_after = reformatted_source[end:]
 			reformatted_source = ''.join([source_before, replacement, source_after])
 
 		return reformatted_source
 
-	def record_replacement(self, text_range: Tuple[int, int], new_source: str):
+	def record_replacement(self, text_range: Tuple[int, int], new_source: str) -> None:
 		"""
 		Record a region of text to be replaced.
 
 		:param text_range: The region of text to be replaced.
 		:param new_source: The new text for that region.
 		"""
 
@@ -153,25 +162,25 @@
 
 
 class SyntaxTracebackHandler(TracebackHandler):
 	"""
 	Subclass of :class:`consolekit.tracebacks.TracebackHandler` to additionally handle :exc:`SyntaxError`.
 	"""
 
-	def handle_SyntaxError(self, e: SyntaxError):  # noqa: D102
+	def handle_SyntaxError(self, e: SyntaxError) -> "NoReturn":  # noqa: D102
 		click.echo(terminal_colours.Fore.RED(f"Fatal: {e.__class__.__name__}: {e}"), err=True)
 		sys.exit(126)
 
-	def handle_HookNotFoundError(self, e: HookNotFoundError):  # noqa: D102
+	def handle_HookNotFoundError(self, e: HookNotFoundError) -> "NoReturn":  # noqa: D102
 		click.echo(terminal_colours.Fore.RED(f"Fatal: Hook not found: {e}"), err=True)
 		sys.exit(126)
 
 
 @contextmanager
-def syntaxerror_for_file(filename: PathLike):
+def syntaxerror_for_file(filename: PathLike) -> Iterator:
 	"""
 	Context manager to catch :exc:`SyntaxError` and set its filename to ``filename``
 	if the current filename is ``<unknown>``.
 
 	This is useful for syntax errors raised when parsing source into an AST.
 
 	:param filename:
@@ -182,7 +191,26 @@
 	try:
 		yield
 	except SyntaxError as e:
 		if e.filename == "<unknown>":
 			e.filename = os.fspath(filename)
 
 		raise e
+
+
+_P = TypeVar("_P", bound=pathlib.Path)
+
+
+def _find_from_parents(path: _P) -> _P:
+	"""
+	Try to find ``path`` in the current directory or its parents.
+
+	If the file can't be found ``path`` is returned.
+	"""
+
+	if len(path.parts) == 1 and not path.exists():
+		for parent in path.cwd().parents:
+			candidate = parent / path
+			if candidate.exists():
+				return candidate
+
+	return path
```

### Comparing `formate-0.4.9/formate/reformat_generics.py` & `formate-0.5.0/formate/reformat_generics.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,38 +38,40 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import ast
 import sys
-import textwrap
 import typing
 from collections.abc import Collection
 from io import StringIO
+from textwrap import indent as indent_string
 
 # 3rd party
 import astatine
-import asttokens  # type: ignore
+import asttokens
 from domdf_python_tools.stringlist import DelimitedList, StringList
 from domdf_python_tools.words import TAB
 
-__all__ = ["reformat_generics", "Generic", "List"]
+__all__ = ("reformat_generics", "Generic", "List")
 
 collection_types = {"Union", "List", "Tuple", "Set", "Dict", "Callable", "Optional", "Literal"}
 
 subclasses = [Collection]
+# pylint: disable=loop-global-usage
 while subclasses:
 	subclass = subclasses.pop(0)
 	if subclass.__module__ == "collections.abc":
 		collection_types.add(subclass.__name__)
 		subclasses.extend(subclass.__subclasses__())
+		# pylint: enable=loop-global-usage
 
 
-def get_slice_value(ast_slice):  # py36: ast.Index  # py39: ast.Tuple
+def get_slice_value(ast_slice):  # py36: ast.Index  # py39: ast.Tuple  # noqa: MAN001,MAN002
 	"""
 	Return the value of the slice in a Python version-independent way.
 
 	:param ast_slice:
 	"""
 
 	if sys.version_info < (3, 9):  # pragma: no cover (py39+)
@@ -99,19 +101,20 @@
 
 		:param line_offset:
 		"""
 
 		if line_offset + len(repr(self)) > 110:
 			# Line too long as is
 			elements: DelimitedList[str] = DelimitedList()
+			offset_plus_4 = line_offset + 4
 			for element in self.elements:
 				if isinstance(element, Generic):
-					elements.append(textwrap.indent(element.format(line_offset + 4), '\t'))
+					elements.append(indent_string(element.format(offset_plus_4), '\t'))
 				else:
-					elements.append(textwrap.indent(str(element), '\t'))
+					elements.append(indent_string(str(element), '\t'))
 			return f"{self.name}[\n{elements:,\n}\n	]"
 		else:
 			return repr(self)
 
 
 class List:
 	"""
@@ -123,21 +126,21 @@
 	def __init__(self, elements: typing.Sequence[typing.Union[str, Generic, "List"]]):
 		self.elements = DelimitedList(elements)
 
 	def __repr__(self) -> str:
 		return f"[{self.elements:, }]"
 
 
-class Visitor(ast.NodeVisitor):  # noqa: D101
+class Visitor(ast.NodeVisitor):
 	in_class = False
 
 	def __init__(self):
 		self.unions: typing.List[typing.Tuple[ast.Subscript, Generic, bool]] = []
 
-	def visit_Subscript(self, node: ast.Subscript) -> None:  # noqa: D102
+	def visit_Subscript(self, node: ast.Subscript) -> None:
 		if isinstance(node.value, ast.Name) and node.value.id in collection_types:
 			union = Generic(node.value.id, UnionVisitor().visit(get_slice_value(node.slice)))
 			self.unions.append((node, union, self.in_class))
 			return
 
 		elif isinstance(node.value, ast.Attribute):
 			if isinstance(node.value.value, ast.Name) and node.value.value.id in {"typing", "typing_extensions"}:
@@ -147,116 +150,118 @@
 							UnionVisitor().visit(get_slice_value(node.slice)),
 							)
 					self.unions.append((node, union, self.in_class))
 					return
 
 		self.generic_visit(node)
 
-	def visit(self, node: ast.AST) -> typing.List[typing.Tuple[ast.Subscript, Generic, bool]]:  # noqa: D102
+	def visit(self, node: ast.AST) -> typing.List[typing.Tuple[ast.Subscript, Generic, bool]]:
 		super().visit(node)
 		return self.unions
 
-	def visit_FunctionDef(self, node: ast.FunctionDef) -> None:  # noqa: D102
+	def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
 		return None
 
-	def visit_ClassDef(self, node: ast.ClassDef) -> None:  # noqa: D102
+	def visit_ClassDef(self, node: ast.ClassDef) -> None:
 		self.unions.extend(ClassVisitor().visit(node))
 
-	def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:  # noqa: D102
+	def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:
 		return None
 
 
-class ClassVisitor(Visitor):  # noqa: D101
+class ClassVisitor(Visitor):
 	in_class = True
 
-	def visit_ClassDef(self, node: ast.ClassDef) -> None:  # noqa: D102
+	def visit_ClassDef(self, node: ast.ClassDef) -> None:
 		self.generic_visit(node)
 
 
-class UnionVisitor(ast.NodeVisitor):  # noqa: D101
+class UnionVisitor(ast.NodeVisitor):
 
 	def __init__(self):
 		super().__init__()
 		self.structure: typing.List[typing.Union[str, Generic, List]] = []
 
-	def generic_visit(self, node: ast.AST) -> None:  # noqa: D102
+	def generic_visit(self, node: ast.AST) -> None:
 		super().generic_visit(node)
 
-	def visit_Name(self, node: ast.Name) -> None:  # noqa: D102
+	def visit_Name(self, node: ast.Name) -> None:
 		self.structure.append(f"{node.id}")
 
-	def visit_Attribute(self, node: ast.Attribute) -> None:  # noqa: D102
+	def visit_Attribute(self, node: ast.Attribute) -> None:
 		parts: DelimitedList[str] = DelimitedList()
 		value: typing.Union[ast.Name, ast.expr] = node.value
 
+		NameNode, AttributeNode = ast.Name, ast.Attribute
+
 		while True:
-			if isinstance(value, ast.Name):
+			if isinstance(value, NameNode):
 				parts.append(value.id)
 				break
-			elif isinstance(value, ast.Attribute):
-				parts.append(value.value.id)  # type: ignore
-				value = value.attr  # type: ignore
+			elif isinstance(value, AttributeNode):
+				parts.append(value.value.id)  # type: ignore[attr-defined]
+				value = value.attr  # type: ignore[assignment]
 			elif isinstance(value, str):
 				parts.append(value)
 				break
 			else:
 				raise NotImplementedError(f"Unsupported value type {type(value)}")
 
 		self.structure.append(f"{parts:.}.{node.attr}")
 
-	def visit_Subscript(self, node: ast.Subscript) -> None:  # noqa: D102
+	def visit_Subscript(self, node: ast.Subscript) -> None:
 		union = Generic(
 				'.'.join(astatine.get_attribute_name(node.value)),
 				UnionVisitor().visit(get_slice_value(node.slice)),
 				)
 		self.structure.append(union)
 
-	def visit_List(self, node: ast.List) -> None:  # noqa: D102
+	def visit_List(self, node: ast.List) -> None:
 		elements = []
 		for child in node.elts:
 			elements.extend(UnionVisitor().visit(child))
 		self.structure.append(List(elements))
 
-	def visit_Load(self, node: ast.Load) -> None:  # noqa: D102
+	def visit_Load(self, node: ast.Load) -> None:
 		return None
 
-	def visit_FunctionDef(self, node: ast.FunctionDef) -> None:  # noqa: D102
+	def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
 		return None
 
-	def visit_ClassDef(self, node: ast.ClassDef) -> None:  # noqa: D102
+	def visit_ClassDef(self, node: ast.ClassDef) -> None:
 		self.generic_visit(node)
 
-	def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:  # noqa: D102
+	def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:
 		return None
 
-	def visit_NameConstant(self, node: ast.NameConstant) -> None:  # noqa: D102
+	def visit_NameConstant(self, node: ast.NameConstant) -> None:
 		self.structure.append(node.value)
 
 	if sys.version_info[:2] < (3, 8):  # pragma: no cover (py38+)
 
-		def visit_Str(self, node: ast.Str) -> None:  # noqa: D102
+		def visit_Str(self, node: ast.Str) -> None:
 			self.structure.append(f'"{node.s}"')
 
-		def visit_Ellipsis(self, node: ast.Ellipsis) -> None:  # noqa: D102
+		def visit_Ellipsis(self, node: ast.Ellipsis) -> None:
 			self.structure.append("...")
 
 	else:  # pragma: no cover (<py38)
 
-		def visit_Constant(self, node: ast.Constant) -> None:  # noqa: D102
+		def visit_Constant(self, node: ast.Constant) -> None:
 			if isinstance(node.value, str):
 				self.structure.append(f'"{node.value}"')
 			elif node.value is Ellipsis:
 				self.structure.append("...")
 			elif node.value is None or isinstance(node.value, bool):
-				self.structure.append(node.value)
+				self.structure.append(str(node.value))
 			else:
 				print(node, node.value)
 				self.generic_visit(node)
 
-	def visit(self, node: ast.AST) -> typing.List[typing.Union[str, Generic, List]]:  # noqa: D102
+	def visit(self, node: ast.AST) -> typing.List[typing.Union[str, Generic, List]]:
 		super().visit(node)
 		return self.structure
 
 
 def reformat_generics(
 		source: str,
 		formate_global_config: typing.Optional[typing.Mapping] = None,
@@ -277,19 +282,21 @@
 		\clearpage
 	"""  # noqa: D400
 
 	offset = 0
 	buf = StringIO()
 	visitor = Visitor()
 	atok = asttokens.ASTTokens(source, parse=True)
+	tree = atok.tree
+	assert tree is not None
 
 	indent = (formate_global_config or {}).get("indent", kwargs.get("indent", TAB))
 
 	try:
-		for union_node, union_obj, in_class in visitor.visit(atok.tree):
+		for union_node, union_obj, in_class in visitor.visit(tree):
 			text_range = atok.get_text_range(union_node)
 			buf.write(source[offset:text_range[0]])
 
 			reversed_line = source[offset:text_range[0]][::-1]
 
 			if '\n' in reversed_line:
 				line_offset = reversed_line.index('\n')
@@ -297,15 +304,15 @@
 				line_offset = 0
 
 			formatted_obj = StringList(union_obj.format(line_offset))
 
 			if in_class and len(formatted_obj) > 1:
 				buf.write(formatted_obj[0])
 				buf.write('\n')
-				buf.write(textwrap.indent(str(StringList(formatted_obj[1:])), indent))
+				buf.write(indent_string(str(StringList(formatted_obj[1:])), indent))
 			elif in_class:
 				buf.write(formatted_obj[0])
 			else:
 				buf.write(str(formatted_obj))
 
 			offset = text_range[1]
```

### Comparing `formate-0.4.9/formate/dynamic_quotes.py` & `formate-0.5.0/formate/dynamic_quotes.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,51 +40,51 @@
 
 # 3rd party
 from domdf_python_tools.utils import double_repr_string
 
 # this package
 from formate.utils import Rewriter
 
-__all__ = ["dynamic_quotes"]
+__all__ = ("dynamic_quotes", )
 
 
-class QuoteRewriter(Rewriter):  # noqa: D101
+class QuoteRewriter(Rewriter):
 
 	if sys.version_info[:2] < (3, 8):  # pragma: no cover (py38+)
 
-		def visit_Str(self, node: ast.Str) -> None:  # noqa: D102
+		def visit_Str(self, node: ast.Str) -> None:
 			self.rewrite_quotes_for_node(node)
 	else:  # pragma: no cover (<py38)
 
-		def visit_Constant(self, node: ast.Constant) -> None:  # noqa: D102
+		def visit_Constant(self, node: ast.Constant) -> None:
 			if isinstance(node.value, str):
 				self.rewrite_quotes_for_node(node)
 			else:
 				self.generic_visit(node)
 
 	def visit_definition(self, node: Union[ast.ClassDef, ast.FunctionDef, ast.AsyncFunctionDef]) -> None:
 		"""
 		Mark the docstring of the function or class to identify it later.
 
 		:param node:
 		"""
 
 		if node.body and isinstance(node.body[0], ast.Expr):
 			doc_node = node.body[0].value
-			doc_node.is_docstring = True  # type: ignore
+			doc_node.is_docstring = True  # type: ignore[attr-defined]
 
 		self.generic_visit(node)
 
-	def visit_ClassDef(self, node: ast.ClassDef) -> None:  # noqa: D102
+	def visit_ClassDef(self, node: ast.ClassDef) -> None:
 		self.visit_definition(node)
 
-	def visit_FunctionDef(self, node: ast.FunctionDef) -> None:  # noqa: D102
+	def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
 		self.visit_definition(node)
 
-	def visit_ASyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:  # noqa: D102
+	def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:
 		self.visit_definition(node)
 
 	def rewrite_quotes_for_node(self, node: Union[ast.Str, ast.Constant]) -> None:
 		"""
 		Mark the area for rewriting quotes in the given node.
 
 		:param node:
@@ -131,18 +131,18 @@
 
 
 class _LazyTranslate(Mapping):
 	"""
 	Escapes surrogates in the range U+D800 to U+DFFF, so they are left unchanged in the source.
 	"""
 
-	def __iter__(self):
+	def __iter__(self):  # noqa: MAN002
 		raise NotImplementedError
 
-	def __len__(self):
+	def __len__(self):  # noqa: MAN002
 		raise NotImplementedError
 
 	def __getitem__(self, item: int) -> str:
 		if item in range(55296, 57343):
 			return repr(chr(item)).strip("'")
 		else:
 			return chr(item)
```

