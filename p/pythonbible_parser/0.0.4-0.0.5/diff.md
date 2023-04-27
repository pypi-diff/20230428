# Comparing `tmp/pythonbible_parser-0.0.4.tar.gz` & `tmp/pythonbible_parser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonbible_parser-0.0.4.tar", last modified: Fri Jul 15 23:03:06 2022, max compression
+gzip compressed data, was "pythonbible_parser-0.0.5.tar", last modified: Thu Apr 27 22:34:38 2023, max compression
```

## Comparing `pythonbible_parser-0.0.4.tar` & `pythonbible_parser-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2581 2022-07-13 16:20:44.520963 pythonbible_parser-0.0.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1518 2022-07-13 16:20:44.521237 pythonbible_parser-0.0.4/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1818 2022-07-13 16:20:44.521611 pythonbible_parser-0.0.4/.gitignore
--rw-r--r--   0        0        0     1465 2022-07-13 23:44:06.747895 pythonbible_parser-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       34 2022-07-13 16:20:44.521869 pythonbible_parser-0.0.4/.sourcery.yaml
--rw-r--r--   0        0        0     1070 2021-04-08 19:36:20.293057 pythonbible_parser-0.0.4/LICENSE
--rw-r--r--   0        0        0     1824 2022-07-13 16:20:44.522077 pythonbible_parser-0.0.4/README.md
--rw-r--r--   0        0        0     1391 2022-07-15 22:57:06.306028 pythonbible_parser-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      251 2022-07-15 22:57:06.306294 pythonbible_parser-0.0.4/pythonbible_parser/__init__.py
--rw-r--r--   0        0        0     2446 2022-07-13 23:44:06.748385 pythonbible_parser-0.0.4/pythonbible_parser/bible.py
--rw-r--r--   0        0        0     3440 2022-07-13 23:44:06.748576 pythonbible_parser-0.0.4/pythonbible_parser/bible_parser.py
--rw-r--r--   0        0        0     4233 2022-07-13 16:20:44.523140 pythonbible_parser-0.0.4/pythonbible_parser/data/asv/books.json
--rw-r--r--   0        0        0  4357398 2022-07-13 16:20:44.540952 pythonbible_parser-0.0.4/pythonbible_parser/data/asv/verses.json
--rw-r--r--   0        0        0     4521 2022-07-13 16:20:44.541402 pythonbible_parser-0.0.4/pythonbible_parser/data/kjv/books.json
--rw-r--r--   0        0        0  4607328 2022-07-13 16:20:44.564585 pythonbible_parser-0.0.4/pythonbible_parser/data/kjv/verses.json
--rw-r--r--   0        0        0      158 2022-07-13 23:44:06.748756 pythonbible_parser-0.0.4/pythonbible_parser/errors.py
--rw-r--r--   0        0        0     4131 2022-07-13 23:44:06.748926 pythonbible_parser-0.0.4/pythonbible_parser/json_converter.py
--rw-r--r--   0        0        0        0 2021-04-08 19:36:20.327169 pythonbible_parser-0.0.4/pythonbible_parser/osis/__init__.py
--rw-r--r--   0        0        0     3644 2022-07-13 23:44:06.749177 pythonbible_parser-0.0.4/pythonbible_parser/osis/constants.py
--rw-r--r--   0        0        0    11063 2022-07-15 22:57:06.306474 pythonbible_parser-0.0.4/pythonbible_parser/osis/old_osis_parser.py
--rw-r--r--   0        0        0    10842 2022-07-13 23:44:06.749840 pythonbible_parser-0.0.4/pythonbible_parser/osis/osis_book_parser.py
--rw-r--r--   0        0        0     6641 2022-07-13 23:44:06.750005 pythonbible_parser-0.0.4/pythonbible_parser/osis/osis_parser.py
--rw-r--r--   0        0        0     1132 2022-07-13 23:44:06.750100 pythonbible_parser-0.0.4/pythonbible_parser/osis/osis_utilities.py
--rw-r--r--   0        0        0      980 2022-07-13 23:44:06.750267 pythonbible_parser-0.0.4/pythonbible_parser/osis/sandbox.py
--rw-r--r--   0        0        0 26766028 2022-07-13 16:20:44.658718 pythonbible_parser-0.0.4/pythonbible_parser/osis/versions/asv.xml
--rw-r--r--   0        0        0 25242839 2022-07-13 16:20:44.790235 pythonbible_parser-0.0.4/pythonbible_parser/osis/versions/kjv.xml
--rw-r--r--   0        0        0       11 2022-07-13 23:44:06.750421 pythonbible_parser-0.0.4/requirements-dev.txt
--rw-r--r--   0        0        0       26 2022-07-13 16:20:44.794110 pythonbible_parser-0.0.4/requirements-test.txt
--rw-r--r--   0        0        0       37 2022-07-15 22:57:06.306611 pythonbible_parser-0.0.4/requirements.txt
--rw-r--r--   0        0        0     1029 2022-07-15 22:57:06.306870 pythonbible_parser-0.0.4/setup.cfg
--rw-r--r--   0        0        0        0 2021-04-08 19:36:20.445668 pythonbible_parser-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1338 2022-07-13 23:44:06.750952 pythonbible_parser-0.0.4/tests/bible_test.py
--rw-r--r--   0        0        0    26252 2022-07-13 23:44:06.751474 pythonbible_parser-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0     9998 2022-07-13 23:44:06.751697 pythonbible_parser-0.0.4/tests/old_osis_parser_test.py
--rw-r--r--   0        0        0      353 2022-07-13 16:20:44.797266 pythonbible_parser-0.0.4/tests/osis_constants_test.py
--rw-r--r--   0        0        0    11632 2022-07-13 23:44:06.752148 pythonbible_parser-0.0.4/tests/osis_parser_test.py
--rw-r--r--   0        0        0     1641 2022-07-13 16:20:44.797751 pythonbible_parser-0.0.4/tests/profiler_test.py
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 pythonbible_parser-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2581 2023-04-27 22:20:34.108063 pythonbible_parser-0.0.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1526 2023-04-27 22:20:34.108236 pythonbible_parser-0.0.5/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1818 2023-04-27 22:20:34.108378 pythonbible_parser-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1175 2023-04-27 22:20:34.108516 pythonbible_parser-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2023-04-27 22:20:34.108637 pythonbible_parser-0.0.5/.sourcery.yaml
+-rw-r--r--   0        0        0     1070 2023-04-27 22:20:34.108779 pythonbible_parser-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1837 2023-04-27 22:20:34.108926 pythonbible_parser-0.0.5/README.md
+-rw-r--r--   0        0        0     1389 2023-04-27 22:21:48.257070 pythonbible_parser-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-04-27 22:25:26.541640 pythonbible_parser-0.0.5/pythonbible_parser/__init__.py
+-rw-r--r--   0        0        0     2446 2023-04-27 22:20:34.109454 pythonbible_parser-0.0.5/pythonbible_parser/bible.py
+-rw-r--r--   0        0        0     3440 2023-04-27 22:20:34.109598 pythonbible_parser-0.0.5/pythonbible_parser/bible_parser.py
+-rw-r--r--   0        0        0     4233 2023-04-27 22:20:34.109906 pythonbible_parser-0.0.5/pythonbible_parser/data/asv/books.json
+-rw-r--r--   0        0        0  4357398 2023-04-27 22:20:34.133618 pythonbible_parser-0.0.5/pythonbible_parser/data/asv/verses.json
+-rw-r--r--   0        0        0     4521 2023-04-27 22:20:34.134060 pythonbible_parser-0.0.5/pythonbible_parser/data/kjv/books.json
+-rw-r--r--   0        0        0  4607328 2023-04-27 22:20:34.151307 pythonbible_parser-0.0.5/pythonbible_parser/data/kjv/verses.json
+-rw-r--r--   0        0        0      158 2023-04-27 22:20:34.151669 pythonbible_parser-0.0.5/pythonbible_parser/errors.py
+-rw-r--r--   0        0        0     4131 2023-04-27 22:20:34.151842 pythonbible_parser-0.0.5/pythonbible_parser/json_converter.py
+-rw-r--r--   0        0        0        0 2023-04-27 22:20:34.151967 pythonbible_parser-0.0.5/pythonbible_parser/osis/__init__.py
+-rw-r--r--   0        0        0     3644 2023-04-27 22:20:34.152143 pythonbible_parser-0.0.5/pythonbible_parser/osis/constants.py
+-rw-r--r--   0        0        0    11063 2023-04-27 22:20:34.152319 pythonbible_parser-0.0.5/pythonbible_parser/osis/old_osis_parser.py
+-rw-r--r--   0        0        0    10842 2023-04-27 22:20:34.152534 pythonbible_parser-0.0.5/pythonbible_parser/osis/osis_book_parser.py
+-rw-r--r--   0        0        0     6641 2023-04-27 22:20:34.152724 pythonbible_parser-0.0.5/pythonbible_parser/osis/osis_parser.py
+-rw-r--r--   0        0        0     1132 2023-04-27 22:20:34.152860 pythonbible_parser-0.0.5/pythonbible_parser/osis/osis_utilities.py
+-rw-r--r--   0        0        0      980 2023-04-27 22:20:34.153086 pythonbible_parser-0.0.5/pythonbible_parser/osis/sandbox.py
+-rw-r--r--   0        0        0 26766028 2023-04-27 22:20:34.265500 pythonbible_parser-0.0.5/pythonbible_parser/osis/versions/asv.xml
+-rw-r--r--   0        0        0 25242839 2023-04-27 22:20:34.377077 pythonbible_parser-0.0.5/pythonbible_parser/osis/versions/kjv.xml
+-rw-r--r--   0        0        0       11 2023-04-27 22:20:34.379897 pythonbible_parser-0.0.5/requirements-dev.txt
+-rw-r--r--   0        0        0       26 2023-04-27 22:20:34.380031 pythonbible_parser-0.0.5/requirements-test.txt
+-rw-r--r--   0        0        0       35 2023-04-27 22:21:48.260269 pythonbible_parser-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1029 2023-04-27 22:20:34.380301 pythonbible_parser-0.0.5/setup.cfg
+-rw-r--r--   0        0        0        0 2023-04-27 22:20:34.380429 pythonbible_parser-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1338 2023-04-27 22:20:34.380569 pythonbible_parser-0.0.5/tests/bible_test.py
+-rw-r--r--   0        0        0    26252 2023-04-27 22:20:34.380802 pythonbible_parser-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0     9998 2023-04-27 22:20:34.381020 pythonbible_parser-0.0.5/tests/old_osis_parser_test.py
+-rw-r--r--   0        0        0      353 2023-04-27 22:20:34.381160 pythonbible_parser-0.0.5/tests/osis_constants_test.py
+-rw-r--r--   0        0        0    11632 2023-04-27 22:20:34.381316 pythonbible_parser-0.0.5/tests/osis_parser_test.py
+-rw-r--r--   0        0        0     1641 2023-04-27 22:20:34.381460 pythonbible_parser-0.0.5/tests/profiler_test.py
+-rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 pythonbible_parser-0.0.5/PKG-INFO
```

### Comparing `pythonbible_parser-0.0.4/.github/workflows/codeql-analysis.yml` & `pythonbible_parser-0.0.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/.github/workflows/python-package.yml` & `pythonbible_parser-0.0.5/.github/workflows/python-package.yml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     branches: [ main ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, "3.10", "3.11-dev"]
+        python-version: [3.7, 3.8, 3.9, "3.10", "3.11", "3.12-dev"]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
```

### Comparing `pythonbible_parser-0.0.4/.gitignore` & `pythonbible_parser-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/LICENSE` & `pythonbible_parser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/README.md` & `pythonbible_parser-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ![CodeQL](https://github.com/avendesora/pythonbible-parser/workflows/CodeQL/badge.svg)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/8f7407c1b98040e185b81c945b78de22)](https://app.codacy.com/gh/avendesora/pythonbible-parser?utm_source=github.com&utm_medium=referral&utm_content=avendesora/pythonbible-parser&utm_campaign=Badge_Grade_Settings)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/avendesora/pythonbible-parser/main.svg)](https://results.pre-commit.ci/latest/github/avendesora/pythonbible-parser/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Python 3.10](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20dev-blue?logo=python&logoColor=lightgray)](https://www.python.org/downloads/)
+[![Python 3.11](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20dev-blue?logo=python&logoColor=lightgray)](https://www.python.org/downloads/)
 
 > **WARNING**: This is very much still a work in progress and does not yet have a
 > stable release. Breaking changes are expected.
 
 ## Installation
 
 ```shell script
```

### Comparing `pythonbible_parser-0.0.4/pyproject.toml` & `pythonbible_parser-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License"
 ]
 requires = [
     "defusedxml >=0.7.1",
-    "pythonbible ==0.7.4",
+    "pythonbible ==0.8",
 ]
 description-file = "README.md"
 requires-python = ">=3.7"
 
 [tool.flit.metadata.urls]
 Documentation = "https://github.com/avendesora/pythonbible-parser"
 Source = "https://github.com/avendesora/pythonbible-parser"
```

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/bible.py` & `pythonbible_parser-0.0.5/pythonbible_parser/bible.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/bible_parser.py` & `pythonbible_parser-0.0.5/pythonbible_parser/bible_parser.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/data/asv/books.json` & `pythonbible_parser-0.0.5/pythonbible_parser/data/asv/books.json`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/data/asv/verses.json` & `pythonbible_parser-0.0.5/pythonbible_parser/data/asv/verses.json`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/data/kjv/books.json` & `pythonbible_parser-0.0.5/pythonbible_parser/data/kjv/books.json`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/data/kjv/verses.json` & `pythonbible_parser-0.0.5/pythonbible_parser/data/kjv/verses.json`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/json_converter.py` & `pythonbible_parser-0.0.5/pythonbible_parser/json_converter.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/osis/constants.py` & `pythonbible_parser-0.0.5/pythonbible_parser/osis/constants.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/osis/old_osis_parser.py` & `pythonbible_parser-0.0.5/pythonbible_parser/osis/old_osis_parser.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/osis/osis_book_parser.py` & `pythonbible_parser-0.0.5/pythonbible_parser/osis/osis_book_parser.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/osis/osis_parser.py` & `pythonbible_parser-0.0.5/pythonbible_parser/osis/osis_parser.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/osis/osis_utilities.py` & `pythonbible_parser-0.0.5/pythonbible_parser/osis/osis_utilities.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/osis/sandbox.py` & `pythonbible_parser-0.0.5/pythonbible_parser/osis/sandbox.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/osis/versions/asv.xml` & `pythonbible_parser-0.0.5/pythonbible_parser/osis/versions/asv.xml`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/pythonbible_parser/osis/versions/kjv.xml` & `pythonbible_parser-0.0.5/pythonbible_parser/osis/versions/kjv.xml`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/setup.cfg` & `pythonbible_parser-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/tests/bible_test.py` & `pythonbible_parser-0.0.5/tests/bible_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/tests/conftest.py` & `pythonbible_parser-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/tests/old_osis_parser_test.py` & `pythonbible_parser-0.0.5/tests/old_osis_parser_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/tests/osis_parser_test.py` & `pythonbible_parser-0.0.5/tests/osis_parser_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/tests/profiler_test.py` & `pythonbible_parser-0.0.5/tests/profiler_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible_parser-0.0.4/PKG-INFO` & `pythonbible_parser-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonbible_parser
-Version: 0.0.4
+Version: 0.0.5
 Summary: The pythonbible-parser library.
 Home-page: https://github.com/avendesora/pythonbible-parser
 Author: Nathan Patton
 Author-email: npatton@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: defusedxml >=0.7.1
-Requires-Dist: pythonbible ==0.7.4
+Requires-Dist: pythonbible ==0.8
 Requires-Dist: pre-commit >=2.20.0 ; extra == "dev"
 Requires-Dist: pytest >=7.1.2 ; extra == "test"
 Requires-Dist: pytest-cov >=3.0.0 ; extra == "test"
 Project-URL: Documentation, https://github.com/avendesora/pythonbible-parser
 Project-URL: Source, https://github.com/avendesora/pythonbible-parser
 Provides-Extra: all
 Provides-Extra: dev
@@ -45,15 +45,15 @@
 
 ![CodeQL](https://github.com/avendesora/pythonbible-parser/workflows/CodeQL/badge.svg)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/8f7407c1b98040e185b81c945b78de22)](https://app.codacy.com/gh/avendesora/pythonbible-parser?utm_source=github.com&utm_medium=referral&utm_content=avendesora/pythonbible-parser&utm_campaign=Badge_Grade_Settings)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/avendesora/pythonbible-parser/main.svg)](https://results.pre-commit.ci/latest/github/avendesora/pythonbible-parser/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Python 3.10](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20dev-blue?logo=python&logoColor=lightgray)](https://www.python.org/downloads/)
+[![Python 3.11](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20dev-blue?logo=python&logoColor=lightgray)](https://www.python.org/downloads/)
 
 > **WARNING**: This is very much still a work in progress and does not yet have a
 > stable release. Breaking changes are expected.
 
 ## Installation
 
 ```shell script
```

