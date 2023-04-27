# Comparing `tmp/pythonbible-0.7.4.tar.gz` & `tmp/pythonbible-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonbible-0.7.4.tar", last modified: Fri Jul 15 22:33:07 2022, max compression
+gzip compressed data, was "pythonbible-0.8.tar", last modified: Thu Apr 27 22:08:55 2023, max compression
```

## Comparing `pythonbible-0.7.4.tar` & `pythonbible-0.8.tar`

### file list

```diff
@@ -1,73 +1,72 @@
--rw-r--r--   0        0        0     2630 2022-07-15 02:43:34.958785 pythonbible-0.7.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1600 2022-06-23 21:02:45.766797 pythonbible-0.7.4/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1935 2022-07-15 02:43:34.959061 pythonbible-0.7.4/.gitignore
--rw-r--r--   0        0        0     1465 2022-07-15 02:43:34.959227 pythonbible-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3357 2021-04-03 20:49:36.993927 pythonbible-0.7.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1429 2022-07-15 02:43:34.959413 pythonbible-0.7.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1070 2021-04-03 20:49:36.994042 pythonbible-0.7.4/LICENSE
--rw-r--r--   0        0        0     7840 2022-07-15 02:43:34.959568 pythonbible-0.7.4/README.md
--rw-r--r--   0        0        0     1064 2021-09-28 17:34:57.215757 pythonbible-0.7.4/SECURITY.md
--rw-r--r--   0        0        0      638 2022-04-30 00:00:58.617967 pythonbible-0.7.4/docs/Makefile
--rw-r--r--   0        0        0      804 2022-04-30 00:00:58.621472 pythonbible-0.7.4/docs/make.bat
--rw-r--r--   0        0        0    15406 2022-04-30 00:00:58.621974 pythonbible-0.7.4/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0    14425 2022-04-30 00:00:58.622438 pythonbible-0.7.4/docs/source/_static/pythonbible-dark.png
--rw-r--r--   0        0        0    14457 2022-04-30 00:00:58.622895 pythonbible-0.7.4/docs/source/_static/pythonbible.png
--rw-r--r--   0        0        0    15577 2022-04-30 00:00:58.623362 pythonbible-0.7.4/docs/source/advanced_usage.rst
--rw-r--r--   0        0        0     5994 2022-04-30 00:00:58.623587 pythonbible-0.7.4/docs/source/basic_usage.rst
--rw-r--r--   0        0        0     5325 2022-04-30 00:00:58.623944 pythonbible-0.7.4/docs/source/book_abbreviations.rst
--rw-r--r--   0        0        0     3149 2022-07-15 22:31:09.990396 pythonbible-0.7.4/docs/source/conf.py
--rw-r--r--   0        0        0      872 2022-04-30 00:00:58.624518 pythonbible-0.7.4/docs/source/index.rst
--rw-r--r--   0        0        0      429 2022-07-15 02:43:34.959933 pythonbible-0.7.4/docs/source/installation.rst
--rw-r--r--   0        0        0    19612 2022-07-15 02:43:34.960220 pythonbible-0.7.4/docs/source/technical_reference.rst
--rw-r--r--   0        0        0     1425 2022-07-15 22:31:09.990654 pythonbible-0.7.4/pyproject.toml
--rw-r--r--   0        0        0    41533 2022-04-30 00:00:58.625947 pythonbible-0.7.4/pythonbible.png
--rw-r--r--   0        0        0     1562 2022-07-15 22:31:09.990867 pythonbible-0.7.4/pythonbible/__init__.py
--rw-r--r--   0        0        0        0 2021-04-03 20:49:36.994770 pythonbible-0.7.4/pythonbible/bible/__init__.py
--rw-r--r--   0        0        0     3464 2022-07-15 02:43:34.960757 pythonbible-0.7.4/pythonbible/bible/bible_parser.py
--rw-r--r--   0        0        0     4233 2022-07-15 02:43:34.960901 pythonbible-0.7.4/pythonbible/bible/data/asv/books.json
--rw-r--r--   0        0        0  4357398 2022-07-15 02:43:34.979846 pythonbible-0.7.4/pythonbible/bible/data/asv/verses.json
--rw-r--r--   0        0        0     4521 2022-07-15 02:43:34.981054 pythonbible-0.7.4/pythonbible/bible/data/kjv/books.json
--rw-r--r--   0        0        0  4607328 2022-07-15 02:43:35.006001 pythonbible-0.7.4/pythonbible/bible/data/kjv/verses.json
--rw-r--r--   0        0        0     4122 2022-07-15 02:43:35.006465 pythonbible-0.7.4/pythonbible/bible/json_converter.py
--rw-r--r--   0        0        0        0 2021-04-03 20:49:37.021270 pythonbible-0.7.4/pythonbible/bible/osis/__init__.py
--rw-r--r--   0        0        0     3171 2022-07-15 02:43:35.007266 pythonbible-0.7.4/pythonbible/bible/osis/constants.py
--rw-r--r--   0        0        0    11689 2022-07-15 22:31:09.991227 pythonbible-0.7.4/pythonbible/bible/osis/parser.py
--rw-r--r--   0        0        0 26766028 2022-07-15 02:43:35.095611 pythonbible-0.7.4/pythonbible/bible/osis/versions/asv.xml
--rw-r--r--   0        0        0 25242839 2022-07-15 02:43:35.209233 pythonbible-0.7.4/pythonbible/bible/osis/versions/kjv.xml
--rw-r--r--   0        0        0     6109 2022-07-15 22:31:09.991662 pythonbible-0.7.4/pythonbible/book_groups.py
--rw-r--r--   0        0        0     4359 2022-07-15 02:43:35.216902 pythonbible-0.7.4/pythonbible/books.py
--rw-r--r--   0        0        0     4546 2022-07-15 22:31:09.991890 pythonbible-0.7.4/pythonbible/converter.py
--rw-r--r--   0        0        0        0 2021-06-09 21:40:10.750554 pythonbible-0.7.4/pythonbible/counters/__init__.py
--rw-r--r--   0        0        0     1285 2022-07-15 02:43:35.222736 pythonbible-0.7.4/pythonbible/counters/book_counter.py
--rw-r--r--   0        0        0     1916 2022-07-15 22:31:09.992140 pythonbible-0.7.4/pythonbible/counters/chapter_counter.py
--rw-r--r--   0        0        0     2584 2022-07-15 02:43:35.228449 pythonbible-0.7.4/pythonbible/counters/verse_counter.py
--rw-r--r--   0        0        0     1835 2022-07-15 22:31:09.992327 pythonbible-0.7.4/pythonbible/errors.py
--rw-r--r--   0        0        0    17829 2022-07-15 02:43:35.231280 pythonbible-0.7.4/pythonbible/formatter.py
--rw-r--r--   0        0        0     1009 2022-07-15 22:31:09.992935 pythonbible-0.7.4/pythonbible/normalized_reference.py
--rw-r--r--   0        0        0     9166 2022-07-15 22:31:09.993299 pythonbible-0.7.4/pythonbible/parser.py
--rw-r--r--   0        0        0     9731 2022-07-15 02:43:35.237600 pythonbible-0.7.4/pythonbible/regular_expressions.py
--rw-r--r--   0        0        0     1471 2022-07-15 22:31:09.993518 pythonbible-0.7.4/pythonbible/roman_numeral_util.py
--rw-r--r--   0        0        0     3681 2022-07-15 22:31:09.993744 pythonbible-0.7.4/pythonbible/validator.py
--rw-r--r--   0        0        0    28189 2022-07-15 22:31:09.994078 pythonbible-0.7.4/pythonbible/verses.py
--rw-r--r--   0        0        0     9614 2022-07-15 02:43:35.238674 pythonbible-0.7.4/pythonbible/versions.py
--rw-r--r--   0        0        0       11 2022-07-15 22:31:09.994295 pythonbible-0.7.4/requirements-dev.txt
--rw-r--r--   0        0        0       27 2022-07-15 02:43:35.239060 pythonbible-0.7.4/requirements-docs.txt
--rw-r--r--   0        0        0       18 2022-07-15 02:43:35.239218 pythonbible-0.7.4/requirements-test.txt
--rw-r--r--   0        0        0       28 2022-07-15 02:43:35.239356 pythonbible-0.7.4/requirements.txt
--rw-r--r--   0        0        0     1538 2022-07-15 22:31:09.994485 pythonbible-0.7.4/setup.cfg
--rw-r--r--   0        0        0       54 2022-07-15 02:43:35.239677 pythonbible-0.7.4/tests/__init__.py
--rw-r--r--   0        0        0    60660 2022-07-15 22:31:09.994993 pythonbible-0.7.4/tests/conftest.py
--rw-r--r--   0        0        0     6418 2022-07-15 02:43:35.240320 pythonbible-0.7.4/tests/converter_test.py
--rw-r--r--   0        0        0     6523 2022-07-15 22:31:09.995294 pythonbible-0.7.4/tests/counters_test.py
--rw-r--r--   0        0        0     4805 2022-07-15 02:43:35.240557 pythonbible-0.7.4/tests/errors_test.py
--rw-r--r--   0        0        0    10300 2022-07-15 02:43:35.240682 pythonbible-0.7.4/tests/formatter_test.py
--rw-r--r--   0        0        0     3504 2022-07-15 22:31:09.995914 pythonbible-0.7.4/tests/json_converter_test.py
--rw-r--r--   0        0        0     9516 2022-07-15 02:43:35.240915 pythonbible-0.7.4/tests/parser_test.py
--rw-r--r--   0        0        0     6841 2022-07-15 02:43:35.241047 pythonbible-0.7.4/tests/regular_expressions_test.py
--rw-r--r--   0        0        0     6771 2022-07-15 02:43:35.241157 pythonbible-0.7.4/tests/validator_test.py
--rw-r--r--   0        0        0     3923 2022-07-15 02:43:35.241265 pythonbible-0.7.4/tests/verses_test.py
--rw-r--r--   0        0        0      170 2022-07-15 02:43:35.241442 pythonbible-0.7.4/tests/versions_test.py
--rw-r--r--   0        0        0      352 2022-07-15 02:43:35.241633 pythonbible-0.7.4/tests/zzz_osis_constants_test.py
--rw-r--r--   0        0        0     9983 2022-07-15 02:43:35.241754 pythonbible-0.7.4/tests/zzz_osis_parser_test.py
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 pythonbible-0.7.4/setup.py
--rw-r--r--   0        0        0      180 1970-01-01 00:00:00.000000 pythonbible-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     2630 2023-03-24 19:51:35.355519 pythonbible-0.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1608 2023-03-24 19:51:35.355673 pythonbible-0.8/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1935 2023-03-24 19:51:35.355817 pythonbible-0.8/.gitignore
+-rw-r--r--   0        0        0     1175 2023-04-27 21:39:04.002079 pythonbible-0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3357 2023-03-24 19:51:35.356089 pythonbible-0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1429 2023-03-24 19:51:35.356254 pythonbible-0.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1070 2023-03-24 19:51:35.356387 pythonbible-0.8/LICENSE
+-rw-r--r--   0        0        0     7833 2023-03-24 19:51:35.356553 pythonbible-0.8/README.md
+-rw-r--r--   0        0        0     1064 2023-03-24 19:51:35.356681 pythonbible-0.8/SECURITY.md
+-rw-r--r--   0        0        0      638 2023-03-24 19:51:35.356862 pythonbible-0.8/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-03-24 19:51:35.356988 pythonbible-0.8/docs/make.bat
+-rw-r--r--   0        0        0    15406 2023-03-24 19:51:35.357281 pythonbible-0.8/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0    14425 2023-03-24 19:51:35.357484 pythonbible-0.8/docs/source/_static/pythonbible-dark.png
+-rw-r--r--   0        0        0    14457 2023-03-24 19:51:35.357670 pythonbible-0.8/docs/source/_static/pythonbible.png
+-rw-r--r--   0        0        0    15577 2023-03-24 19:51:35.357845 pythonbible-0.8/docs/source/advanced_usage.rst
+-rw-r--r--   0        0        0     5994 2023-03-24 19:51:35.357992 pythonbible-0.8/docs/source/basic_usage.rst
+-rw-r--r--   0        0        0     5325 2023-03-24 19:51:35.358192 pythonbible-0.8/docs/source/book_abbreviations.rst
+-rw-r--r--   0        0        0     3147 2023-04-27 21:49:39.658260 pythonbible-0.8/docs/source/conf.py
+-rw-r--r--   0        0        0      872 2023-03-24 19:51:35.358461 pythonbible-0.8/docs/source/index.rst
+-rw-r--r--   0        0        0      429 2023-03-24 19:51:35.358586 pythonbible-0.8/docs/source/installation.rst
+-rw-r--r--   0        0        0    19612 2023-03-24 19:51:35.358796 pythonbible-0.8/docs/source/technical_reference.rst
+-rw-r--r--   0        0        0     1425 2023-03-24 19:51:35.358976 pythonbible-0.8/pyproject.toml
+-rw-r--r--   0        0        0    41533 2023-03-24 19:51:35.359288 pythonbible-0.8/pythonbible.png
+-rw-r--r--   0        0        0     1560 2023-04-27 21:49:39.652368 pythonbible-0.8/pythonbible/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 19:51:35.359690 pythonbible-0.8/pythonbible/bible/__init__.py
+-rw-r--r--   0        0        0     3464 2023-03-24 19:51:35.359839 pythonbible-0.8/pythonbible/bible/bible_parser.py
+-rw-r--r--   0        0        0     4233 2023-03-24 19:51:35.360232 pythonbible-0.8/pythonbible/bible/data/asv/books.json
+-rw-r--r--   0        0        0  4357398 2023-03-24 19:51:35.383466 pythonbible-0.8/pythonbible/bible/data/asv/verses.json
+-rw-r--r--   0        0        0     4521 2023-03-24 19:51:35.384052 pythonbible-0.8/pythonbible/bible/data/kjv/books.json
+-rw-r--r--   0        0        0  4607328 2023-03-24 19:51:35.416707 pythonbible-0.8/pythonbible/bible/data/kjv/verses.json
+-rw-r--r--   0        0        0     4122 2023-03-24 19:51:35.417460 pythonbible-0.8/pythonbible/bible/json_converter.py
+-rw-r--r--   0        0        0        0 2023-03-24 19:51:35.417707 pythonbible-0.8/pythonbible/bible/osis/__init__.py
+-rw-r--r--   0        0        0     3171 2023-03-24 19:51:35.417955 pythonbible-0.8/pythonbible/bible/osis/constants.py
+-rw-r--r--   0        0        0    11689 2023-03-24 19:51:35.418286 pythonbible-0.8/pythonbible/bible/osis/parser.py
+-rw-r--r--   0        0        0 26766028 2023-03-24 19:51:35.521836 pythonbible-0.8/pythonbible/bible/osis/versions/asv.xml
+-rw-r--r--   0        0        0 25242839 2023-03-24 19:51:35.594571 pythonbible-0.8/pythonbible/bible/osis/versions/kjv.xml
+-rw-r--r--   0        0        0     6109 2023-03-24 19:51:35.596544 pythonbible-0.8/pythonbible/book_groups.py
+-rw-r--r--   0        0        0     4359 2023-03-24 19:51:35.596686 pythonbible-0.8/pythonbible/books.py
+-rw-r--r--   0        0        0     4546 2023-03-24 19:51:35.596827 pythonbible-0.8/pythonbible/converter.py
+-rw-r--r--   0        0        0        0 2023-03-24 19:51:35.596958 pythonbible-0.8/pythonbible/counters/__init__.py
+-rw-r--r--   0        0        0     1285 2023-03-24 19:51:35.597086 pythonbible-0.8/pythonbible/counters/book_counter.py
+-rw-r--r--   0        0        0     1916 2023-03-24 19:51:35.597240 pythonbible-0.8/pythonbible/counters/chapter_counter.py
+-rw-r--r--   0        0        0     2584 2023-03-24 19:51:35.597358 pythonbible-0.8/pythonbible/counters/verse_counter.py
+-rw-r--r--   0        0        0     1835 2023-03-24 19:51:35.597477 pythonbible-0.8/pythonbible/errors.py
+-rw-r--r--   0        0        0    17764 2023-03-24 19:51:35.597667 pythonbible-0.8/pythonbible/formatter.py
+-rw-r--r--   0        0        0     1009 2023-03-24 19:51:35.597833 pythonbible-0.8/pythonbible/normalized_reference.py
+-rw-r--r--   0        0        0     9166 2023-04-27 18:58:05.716644 pythonbible-0.8/pythonbible/parser.py
+-rw-r--r--   0        0        0    10094 2023-04-27 21:45:08.908162 pythonbible-0.8/pythonbible/regular_expressions.py
+-rw-r--r--   0        0        0     1471 2023-03-24 19:51:35.598429 pythonbible-0.8/pythonbible/roman_numeral_util.py
+-rw-r--r--   0        0        0     3681 2023-03-24 19:51:35.598556 pythonbible-0.8/pythonbible/validator.py
+-rw-r--r--   0        0        0    28189 2023-03-24 19:51:35.598746 pythonbible-0.8/pythonbible/verses.py
+-rw-r--r--   0        0        0     9614 2023-03-24 19:51:35.598936 pythonbible-0.8/pythonbible/versions.py
+-rw-r--r--   0        0        0       11 2023-03-24 19:51:35.599082 pythonbible-0.8/requirements-dev.txt
+-rw-r--r--   0        0        0       27 2023-03-24 19:51:35.599213 pythonbible-0.8/requirements-docs.txt
+-rw-r--r--   0        0        0       18 2023-03-24 19:51:35.599336 pythonbible-0.8/requirements-test.txt
+-rw-r--r--   0        0        0       28 2023-03-24 19:51:35.599506 pythonbible-0.8/requirements.txt
+-rw-r--r--   0        0        0     1552 2023-03-24 19:51:35.599693 pythonbible-0.8/setup.cfg
+-rw-r--r--   0        0        0       54 2023-03-24 19:51:35.599980 pythonbible-0.8/tests/__init__.py
+-rw-r--r--   0        0        0    60660 2023-04-27 19:09:14.108894 pythonbible-0.8/tests/conftest.py
+-rw-r--r--   0        0        0     6418 2023-03-24 19:51:35.600966 pythonbible-0.8/tests/converter_test.py
+-rw-r--r--   0        0        0     6523 2023-03-24 19:51:35.601189 pythonbible-0.8/tests/counters_test.py
+-rw-r--r--   0        0        0     4805 2023-03-24 19:51:35.601414 pythonbible-0.8/tests/errors_test.py
+-rw-r--r--   0        0        0    10300 2023-03-24 19:51:35.601660 pythonbible-0.8/tests/formatter_test.py
+-rw-r--r--   0        0        0     3504 2023-03-24 19:51:35.601891 pythonbible-0.8/tests/json_converter_test.py
+-rw-r--r--   0        0        0    10322 2023-04-27 21:45:08.908442 pythonbible-0.8/tests/parser_test.py
+-rw-r--r--   0        0        0     8782 2023-04-27 21:45:08.908767 pythonbible-0.8/tests/regular_expressions_test.py
+-rw-r--r--   0        0        0     6771 2023-03-24 19:51:35.602518 pythonbible-0.8/tests/validator_test.py
+-rw-r--r--   0        0        0     3923 2023-03-24 19:51:35.602702 pythonbible-0.8/tests/verses_test.py
+-rw-r--r--   0        0        0      170 2023-03-24 19:51:35.602873 pythonbible-0.8/tests/versions_test.py
+-rw-r--r--   0        0        0      352 2023-03-24 19:51:35.603096 pythonbible-0.8/tests/zzz_osis_constants_test.py
+-rw-r--r--   0        0        0     9983 2023-03-24 19:51:35.603337 pythonbible-0.8/tests/zzz_osis_parser_test.py
+-rw-r--r--   0        0        0     9344 1970-01-01 00:00:00.000000 pythonbible-0.8/PKG-INFO
```

### Comparing `pythonbible-0.7.4/.github/workflows/codeql-analysis.yml` & `pythonbible-0.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/.github/workflows/python-package.yml` & `pythonbible-0.8/.github/workflows/python-package.yml`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       - 'feature/**'
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10', '3.11-dev']
+        python-version: [3.7, 3.8, 3.9, '3.10', '3.11', '3.12-dev']
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
```

### Comparing `pythonbible-0.7.4/.gitignore` & `pythonbible-0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/CODE_OF_CONDUCT.md` & `pythonbible-0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/CONTRIBUTING.md` & `pythonbible-0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/LICENSE` & `pythonbible-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/README.md` & `pythonbible-0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ![CodeQL](https://github.com/avendesora/pythonbible/workflows/CodeQL/badge.svg)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/dc1333c64b434f7bb813d08750462921)](https://www.codacy.com/gh/avendesora/pythonbible/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=avendesora/pythonbible&amp;utm_campaign=Badge_Grade)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/avendesora/pythonbible/main.svg)](https://results.pre-commit.ci/latest/github/avendesora/pythonbible/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Python 3.10](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20dev-blue?logo=python&logoColor=lightgray)](https://www.python.org/downloads/release/python-3105/)
+[![Python 3.11](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20dev-blue?logo=python&logoColor=lightgray)](https://www.python.org/downloads/)
 
 ## Documentation
 
 The full documentation for pythonbible can be found at [docs.python.bible](https://docs.python.bible).
 
 ## Installation
```

### Comparing `pythonbible-0.7.4/SECURITY.md` & `pythonbible-0.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/Makefile` & `pythonbible-0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/make.bat` & `pythonbible-0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/source/_static/favicon.ico` & `pythonbible-0.8/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/source/_static/pythonbible-dark.png` & `pythonbible-0.8/docs/source/_static/pythonbible-dark.png`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/source/_static/pythonbible.png` & `pythonbible-0.8/docs/source/_static/pythonbible.png`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/source/advanced_usage.rst` & `pythonbible-0.8/docs/source/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/source/basic_usage.rst` & `pythonbible-0.8/docs/source/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/source/book_abbreviations.rst` & `pythonbible-0.8/docs/source/book_abbreviations.rst`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/source/conf.py` & `pythonbible-0.8/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "pythonbible"
 copyright = "2020 Nathan Patton"
 author = "Nathan Patton"
 
 # The full version, including alpha/beta/rc tags
-release = "0.7.4"
+release = "0.8"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `pythonbible-0.7.4/docs/source/index.rst` & `pythonbible-0.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/docs/source/technical_reference.rst` & `pythonbible-0.8/docs/source/technical_reference.rst`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pyproject.toml` & `pythonbible-0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible.png` & `pythonbible-0.8/pythonbible.png`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/__init__.py` & `pythonbible-0.8/pythonbible/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 converting references into integer verse ids for efficient use/storage,
 converting verse ids back into normalized references, and formatting
 references as human-readable strings.
 """
 
 from __future__ import annotations
 
-__version__ = "0.7.4"
+__version__ = "0.8"
 
 from .bible.osis.parser import OSISParser
 from .book_groups import BOOK_GROUPS, BookGroup
 from .books import Book
 from .converter import (
     convert_reference_to_verse_ids,
     convert_references_to_verse_ids,
```

### Comparing `pythonbible-0.7.4/pythonbible/bible/bible_parser.py` & `pythonbible-0.8/pythonbible/bible/bible_parser.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/data/asv/books.json` & `pythonbible-0.8/pythonbible/bible/data/asv/books.json`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/data/asv/verses.json` & `pythonbible-0.8/pythonbible/bible/data/asv/verses.json`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/data/kjv/books.json` & `pythonbible-0.8/pythonbible/bible/data/kjv/books.json`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/data/kjv/verses.json` & `pythonbible-0.8/pythonbible/bible/data/kjv/verses.json`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/json_converter.py` & `pythonbible-0.8/pythonbible/bible/json_converter.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/osis/constants.py` & `pythonbible-0.8/pythonbible/bible/osis/constants.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/osis/parser.py` & `pythonbible-0.8/pythonbible/bible/osis/parser.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/osis/versions/asv.xml` & `pythonbible-0.8/pythonbible/bible/osis/versions/asv.xml`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/bible/osis/versions/kjv.xml` & `pythonbible-0.8/pythonbible/bible/osis/versions/kjv.xml`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/book_groups.py` & `pythonbible-0.8/pythonbible/book_groups.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/books.py` & `pythonbible-0.8/pythonbible/books.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/converter.py` & `pythonbible-0.8/pythonbible/converter.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/counters/book_counter.py` & `pythonbible-0.8/pythonbible/counters/book_counter.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/counters/chapter_counter.py` & `pythonbible-0.8/pythonbible/counters/chapter_counter.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/counters/verse_counter.py` & `pythonbible-0.8/pythonbible/counters/verse_counter.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/errors.py` & `pythonbible-0.8/pythonbible/errors.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/formatter.py` & `pythonbible-0.8/pythonbible/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,18 +217,15 @@
 
 def _get_book_title(book: Book, include_books: bool = True, **kwargs: Any) -> str:
     if not include_books:
         return ""
 
     version: Version = kwargs.get("version", DEFAULT_VERSION)
     full_title: bool = kwargs.get("full_title", False)
-    version_book_titles: BookTitles | None = get_book_titles(book, version)
-
-    if not version_book_titles:
-        return ""
+    version_book_titles: BookTitles = get_book_titles(book, version)
 
     return (
         version_book_titles.long_title
         if full_title
         else version_book_titles.short_title
     )
 
@@ -409,26 +406,22 @@
 
     for verse_id in verse_ids:
         book, chapter_number, verse_number = get_book_chapter_verse(verse_id)
 
         if book != current_book:
             current_book = book
             current_chapter = chapter_number
-            version_book_titles: BookTitles | None = get_book_titles(book, version)
-
-            if version_book_titles:
-                title: str = (
-                    version_book_titles.long_title
-                    if full_title
-                    else version_book_titles.short_title
-                )
-                text += _format_title(title, format_type, not text)
-
+            version_book_titles: BookTitles = get_book_titles(book, version)
+            title: str = (
+                version_book_titles.long_title
+                if full_title
+                else version_book_titles.short_title
+            )
+            text += _format_title(title, format_type, not text)
             text += _format_chapter(chapter_number, format_type)
-
         elif chapter_number != current_chapter:
             current_chapter = chapter_number
             text += _format_chapter(chapter_number, format_type)
 
         verse_text: str | None = get_verse_text(verse_id, version)
 
         if include_verse_numbers:
@@ -509,15 +502,15 @@
     """
     if verse_id not in VERSE_IDS:
         raise InvalidVerseError(verse_id=verse_id)
 
     try:
         version_verse_texts: dict[int, str] = _get_version_verse_texts(version)
     except FileNotFoundError as file_not_found_error:
-        raise MissingVerseFileError(file_not_found_error)
+        raise MissingVerseFileError(file_not_found_error) from file_not_found_error
 
     return version_verse_texts.get(verse_id)
 
 
 @lru_cache()
 def _get_version_verse_texts(version: Version) -> dict[int, str]:
     version_verse_texts: dict[int, str] | None = verse_texts.get(version)
@@ -536,36 +529,33 @@
 
         verse_texts[version] = version_verse_texts
 
     return version_verse_texts
 
 
 @lru_cache()
-def get_book_titles(
-    book: Book,
-    version: Version = DEFAULT_VERSION,
-) -> BookTitles | None:
+def get_book_titles(book: Book, version: Version = DEFAULT_VERSION) -> BookTitles:
     """
     Return the book titles for the given Book and optional Version.
 
     :param book: a book of the Bible
     :type book: Book
     :param version: a version of the Bible, defaults to American Standard
     :type version: Version
     :return: the long and short titles of the given book and version
-    :rtype: BookTitles | None
+    :rtype: BookTitles
     :raises MissingBookFileError: if the book file for the given book and version does
                                   not exist
     """
     try:
         version_book_titles: dict[Book, BookTitles] = _get_version_book_titles(version)
     except FileNotFoundError as file_not_found_error:
-        raise MissingBookFileError(file_not_found_error)
+        raise MissingBookFileError(file_not_found_error) from file_not_found_error
 
-    return version_book_titles.get(book)
+    return version_book_titles.get(book, BookTitles(book.title, book.title))
 
 
 @lru_cache()
 def _get_version_book_titles(version: Version) -> dict[Book, BookTitles]:
     version_book_titles: dict[Book, BookTitles] | None = book_titles.get(version)
 
     if version_book_titles is None:
```

### Comparing `pythonbible-0.7.4/pythonbible/normalized_reference.py` & `pythonbible-0.8/pythonbible/normalized_reference.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/parser.py` & `pythonbible-0.8/pythonbible/parser.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/regular_expressions.py` & `pythonbible-0.8/pythonbible/regular_expressions.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 
 SAMUEL_REGULAR_EXPRESSION = "(Samuel" r"|Sam\.*" r"|Sa\.*" r"|Sm\.*)"
 KINGS_REGULAR_EXPRESSION = "(Kings" r"|Kgs\.*" r"|Kin\.*" r"|Ki\.*)"
 CHRONICLES_REGULAR_EXPRESSION = (
     "(Chronicles" r"|Chron\.*" r"|Chro\.*" r"|Chr\.*" r"|Ch\.*)"
 )
-JOHN_REGULAR_EXPRESSION = "(John" r"|Joh\.*" r"|Jhn\.*" r"|Jo\.*" r"|Jn\.*)"
+JOHN_REGULAR_EXPRESSION = (
+    "(John" r"|Joh\.*" r"|Jhn\.*" r"|Jo\.*(?!shua|b|nah|el)" r"|Jn\.*)"
+)
 CORINTHIANS_REGULAR_EXPRESSION = r"Co\.*(?:r\.*(?:inthians)?)?"
 THESSALONIANS_REGULAR_EXPRESSION = r"Th\.*(?:(s|(es(?:s)?))\.*(?:alonians)?)?"
 TIMOTHY_REGULAR_EXPRESSION = r"Ti\.*(?:m\.*(?:othy)?)?"
 PETER_REGULAR_EXPRESSION = r"(Pe\.*(?:t\.*(?:er)?)?|Pt\.*)"
 
 MACCABEES_REGULAR_EXPRESSION = "(Maccabees" r"|Macc\.*" r"|Mac\.*" r"|Ma\.*" r"|M\.*)"
 
@@ -50,15 +52,15 @@
 SECOND_PAUL_EPISTLE = rf"{SECOND}|(Second\s+{EPISTLE_OF_PAUL_TO})"
 
 FIRST_GENERAL_EPISTLE = rf"{FIRST}|(First\s+{GENERAL_EPISTLE_OF})"
 SECOND_GENERAL_EPISTLE = rf"{SECOND}|(Second\s+{GENERAL_EPISTLE_OF})"
 THIRD_GENERAL_EPISTLE = rf"{THIRD}|(Third\s+{GENERAL_EPISTLE_OF})"
 
 # noinspection SpellCheckingInspection
-BOOK_REGULAR_EXPRESSIONS: dict[Book, str] = MappingProxyType(
+BOOK_REGULAR_EXPRESSIONS: MappingProxyType[Book, str] = MappingProxyType(
     {
         Book.GENESIS: r"Gen\.*(?:esis)?",
         Book.EXODUS: r"Exo\.*(?:d\.*)?(?:us)?",
         Book.LEVITICUS: r"Lev\.*(?:iticus)?",
         Book.NUMBERS: r"Num\.*(?:bers)?",
         Book.DEUTERONOMY: r"Deu\.*(?:t\.*)?(?:eronomy)?",
         Book.JOSHUA: "(Joshua" r"|Josh\.*" r"|Jos\.*" r"|Jsh\.*)",
@@ -105,15 +107,15 @@
         r"|Ps\.*)",
         Book.PROVERBS: "(Proverbs" r"|Prov\.*" r"|Pro\.*" r"|Prv\.*)",
         Book.ECCLESIASTES: r"(Ecclesiastes(?:\s+or\,\s+the\s+Preacher)?"
         r"|Eccles\.*(?!iasticus?)"
         r"|Eccle\.*(?!siasticus?)"
         r"|Eccl\.*(?!esiasticus?)(?!us?)"
         r"|Ecc\.*(?!lesiasticus?)(?!lus?)"
-        r"|Ec\.*(?!clesiasticus?)(?!clus?)"
+        r"|(?<!Z)Ec\.*(?!clesiasticus?)(?!clus?)"
         r"|Qoh\.*)",
         Book.SONG_OF_SONGS: r"(Song(?: of (Solomon|Songs|Sol\.*))?)"
         "|Canticles"
         "|(Canticle(?: of Canticles)?)"
         "|SOS"
         "|Cant",
         Book.ISAIAH: r"Isa\.*(?:iah)?",
@@ -126,15 +128,15 @@
         Book.DANIEL: r"Dan\.*(?:iel)?",
         Book.HOSEA: r"Hos\.*(?:ea)?",
         Book.JOEL: r"Joe\.*(?:l)?",
         Book.AMOS: r"Amo\.*(?:s)?",
         Book.OBADIAH: r"Oba\.*(?:d\.*(?:iah)?)?",
         Book.JONAH: "Jonah" r"|Jon\.*" r"|Jnh\.*",
         Book.MICAH: r"Mic\.*(?:ah)?",
-        Book.NAHUM: r"Nah\.*(?:um)?",
+        Book.NAHUM: r"(?<!Jo)Nah\.*(?:um)?",
         Book.HABAKKUK: r"Hab\.*(?:akkuk)?",
         Book.ZEPHANIAH: r"Zep\.*(?:h\.*(?:aniah)?)?",
         Book.HAGGAI: r"Hag\.*(?:gai)?",
         Book.ZECHARIAH: r"Zec\.*(?:h\.*(?:ariah)?)?",
         Book.MALACHI: r"Mal\.*(?:achi)?",
         Book.MATTHEW: r"Mat\.*(?:t\.*(?:hew)?)?",
         Book.MARK: "Mark" r"|Mar\.*" r"|Mrk\.*",
@@ -150,15 +152,15 @@
             prefix=FIRST_PAUL_EPISTLE,
         ),
         Book.CORINTHIANS_2: build_book_regular_expression(
             CORINTHIANS_REGULAR_EXPRESSION,
             prefix=SECOND_PAUL_EPISTLE,
         ),
         Book.GALATIANS: r"Gal\.*(?:atians)?",
-        Book.EPHESIANS: r"Eph\.*(?:es\.*(?:ians)?)?",
+        Book.EPHESIANS: r"(?<!Z)Eph\.*(?:es\.*(?:ians)?)?",
         Book.PHILIPPIANS: r"Ph(?:(p\.*)|(?:il\.*(?!e\.*(?:m\.*(?:on)?)?)(?:ippians)?))",
         Book.COLOSSIANS: r"Col\.*(?:ossians)?",
         Book.THESSALONIANS_1: build_book_regular_expression(
             THESSALONIANS_REGULAR_EXPRESSION,
             prefix=FIRST_PAUL_EPISTLE,
         ),
         Book.THESSALONIANS_2: build_book_regular_expression(
@@ -175,15 +177,15 @@
         ),
         Book.TITUS: r"Tit\.*(?:us)?",
         # assume 'Phi' is Philemon if Philippians failed
         Book.PHILEMON: "(Philemon|"
         r"Philem\.*|"
         r"Phile\.*|"
         r"Phlm\.*|"
-        r"Phi\.*|"
+        r"Phi\.*(?!l)|"
         r"Phm\.*)",
         Book.HEBREWS: r"Heb\.*(?:rews)?",
         Book.JAMES: r"Ja(?:me)?s\.*",
         Book.PETER_1: build_book_regular_expression(
             PETER_REGULAR_EXPRESSION,
             prefix=FIRST_GENERAL_EPISTLE,
         ),
@@ -199,59 +201,70 @@
             JOHN_REGULAR_EXPRESSION,
             prefix=SECOND_GENERAL_EPISTLE,
         ),
         Book.JOHN_3: build_book_regular_expression(
             JOHN_REGULAR_EXPRESSION,
             prefix=THIRD_GENERAL_EPISTLE,
         ),
-        Book.JUDE: r"Jud\.*(:?e)?",
+        Book.JUDE: r"Jud\.*(:?e)?(?!ges)",
         Book.REVELATION: build_book_regular_expression(
             r"Rev\.*(?:elation)?",
             suffix="of ((Jesus Christ)|John|(St. John the Divine))",
         ),
         Book.ESDRAS_1: build_book_regular_expression(
             "(Esdras" r"|Esdr\.*" r"|Esd\.*" r"|Es\.*)",
             FIRST,
         ),
         Book.TOBIT: "(Tobit" r"|Tob\.*" r"|Tb\.*)",
         Book.WISDOM_OF_SOLOMON: "(Wisdom of Solomon"
         "|Wisdom"
         r"|Wisd\.* of Sol\.*"
         r"|Wis\.*"
-        r"|Ws\.*)",
+        r"|(?<!Hebre)Ws\.*)",
         Book.ECCLESIASTICUS: "(Sirach" r"|Sir\.*" "|Ecclesiasticus" r"|Ecclus\.*)",
         Book.MACCABEES_1: build_book_regular_expression(
             MACCABEES_REGULAR_EXPRESSION,
             FIRST,
         ),
         Book.MACCABEES_2: build_book_regular_expression(
             MACCABEES_REGULAR_EXPRESSION,
             SECOND,
         ),
     },
 )
 
-BOOK_REGEX: str = "|".join(
-    rf"\b{regular_expression_value}\b\.?"
-    for regular_expression_value in BOOK_REGULAR_EXPRESSIONS.values()
-)
-
-CHAPTER_REGEX: str = r"(\d{1,3})"
-CHAPTER_VERSE_SEPARATOR: str = "([:.])"
-VERSE_REGEX: str = r"(\d{1,3})"
-CHAPTER_AND_VERSE_REGEX: str = (
-    rf"({CHAPTER_REGEX}(\s*{CHAPTER_VERSE_SEPARATOR}\s*{VERSE_REGEX})?)"
-)
-RANGE_REGEX: str = (
-    rf"({CHAPTER_AND_VERSE_REGEX}(\s*-\s*({CHAPTER_REGEX}\s*"
-    rf"{CHAPTER_VERSE_SEPARATOR}\s*)?{VERSE_REGEX})?)"
+DIGIT: str = r"(\d{1,3})"
+SPACE: str = r"\s*"
+COLON: str = rf"{SPACE}([:.]){SPACE}"
+DASH = rf"{SPACE}-{SPACE}"
+COMMA = rf"{SPACE},{SPACE}"
+
+BOOK: str = rf"\b({'|'.join(BOOK_REGULAR_EXPRESSIONS.values())})\b\.*"
+CHAPTER: str = DIGIT
+VERSE: str = DIGIT
+
+CHAPTER_AND_VERSE: str = rf"({CHAPTER}(?:{COLON}{VERSE})?)"
+
+# Possibly range regular expressions are:
+# 1. Book - Book (with optional chapter/verse)
+# 2. Chapter - Book (with optional chapter/verse)
+# 3. Chapter - Chapter (with optional verse)
+# 4. Verse - Book (with optional chapter/verse)
+# 5. Verse - Chapter:Verse (verse is required)
+# 6. Verse - Verse
+
+# TODO - this regex may have some false positives for ranges given the above rules.
+RANGE: str = (
+    rf"{DASH}(({BOOK}{SPACE}(?:{CHAPTER_AND_VERSE})?)|{CHAPTER_AND_VERSE}|{VERSE})"
+)
+
+ADDITIONAL_REFERENCE: str = rf"({COMMA}({CHAPTER_AND_VERSE}(?:{RANGE})?|{VERSE}))"
+FULL_CHAPTER_AND_VERSE: str = (
+    f"({CHAPTER_AND_VERSE}(?:{RANGE})?({ADDITIONAL_REFERENCE})*)"
 )
-ADDITIONAL_REFERENCE_REGEX: str = rf"(\s*,\s*({RANGE_REGEX}|{VERSE_REGEX}))"
-FULL_CHAPTER_AND_VERSE_REGEX: str = f"({RANGE_REGEX}({ADDITIONAL_REFERENCE_REGEX})*)"
-
-FULL_BOOK_REGEX = rf"({BOOK_REGEX})\s*({FULL_CHAPTER_AND_VERSE_REGEX})?"
-CROSS_BOOK_REGEX = rf"({FULL_BOOK_REGEX}(\s*-\s*({FULL_BOOK_REGEX}))?)"
+FULL_BOOK = rf"({BOOK}){SPACE}(?:{FULL_CHAPTER_AND_VERSE})?"
+CROSS_BOOK = rf"({FULL_BOOK}(?:{DASH}({FULL_BOOK}))?)"
 
 SCRIPTURE_REFERENCE_REGULAR_EXPRESSION: Pattern[str] = re.compile(
-    CROSS_BOOK_REGEX,
+    CROSS_BOOK,
     re.IGNORECASE | re.UNICODE,
 )
```

### Comparing `pythonbible-0.7.4/pythonbible/roman_numeral_util.py` & `pythonbible-0.8/pythonbible/roman_numeral_util.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/validator.py` & `pythonbible-0.8/pythonbible/validator.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/verses.py` & `pythonbible-0.8/pythonbible/verses.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/pythonbible/versions.py` & `pythonbible-0.8/pythonbible/versions.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/setup.cfg` & `pythonbible-0.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -41,23 +41,23 @@
     WPS230,
     WPS231,
     WPS326,
     WPS352
 
 per-file-ignores =
     docs/source/conf.py:A001,E501,E800,INP001,WPS462
-    pythonbible/__init__.py:F401,WPS201,WPS300,WPS410,WPS412
+    pythonbible/__init__.py:F401,WPS130,WPS201,WPS300,WPS410,WPS412
     pythonbible/bible/json_converter.py:WPS201
     pythonbible/bible/osis/parser.py:P103,S405,S314,WPS201,WPS336,WPS440,WPS433,WPS458
     pythonbible/book_groups.py:WPS115
     pythonbible/books.py:WPS114,WPS115
     pythonbible/formatter.py:WPS118,WPS201,WPS204,WPS226,WPS336
     pythonbible/osis/osis_parser.py:P103,WPS336
     pythonbible/parser.py:WPS232
-    pythonbible/roman_numeral_util.py:E741,WPS111,WPS115
+    pythonbible/roman_numeral_util.py:E741,WPS111,WPS121,WPS115
     pythonbible/regular_expressions.py:WPS226
     pythonbible/versions.py:WPS114,WPS115
     tests/__init__.py:WPS412
     tests/conftest.py:D100,D103,E501,WPS234,WPS432
     tests/errors_test.py:PT017,S101,WPS111,WPS118,WPS204,WPS328,WPS226
     tests/regular_expressions_test.py:PT018,S101
     tests/*.py:D100,D103,D104,S101,WPS114,WPS118,WPS204,WPS210,WPS218,WPS226,WPS326,WPS432
```

### Comparing `pythonbible-0.7.4/tests/conftest.py` & `pythonbible-0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/tests/converter_test.py` & `pythonbible-0.8/tests/converter_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/tests/counters_test.py` & `pythonbible-0.8/tests/counters_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/tests/errors_test.py` & `pythonbible-0.8/tests/errors_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/tests/formatter_test.py` & `pythonbible-0.8/tests/formatter_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/tests/json_converter_test.py` & `pythonbible-0.8/tests/json_converter_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/tests/parser_test.py` & `pythonbible-0.8/tests/parser_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -265,7 +265,29 @@
                 continue
 
             # When we parse the references with the alternative name
             alternative_references = bible.get_references(f"{alternative_name} 1:1-2")
 
             # Then the alternative references match the baseline references
             assert alternative_references == references
+
+
+# https://github.com/avendesora/pythonbible/issues/77
+# https://github.com/avendesora/pythonbible/issues/78
+def test_compound_references() -> None:
+    for book in bible.Book:
+        title = book.title
+        end_chapter = bible.get_number_of_chapters(book)
+        end_verse = bible.get_number_of_verses(book, end_chapter)
+        reference_string = f"{title} 1:1-{title} {end_chapter}:{end_verse}"
+        compound_results = bible.get_references(reference_string)
+        expected_result = bible.NormalizedReference(
+            book=book,
+            start_chapter=1,
+            start_verse=1,
+            end_chapter=end_chapter,
+            end_verse=end_verse,
+            end_book=book,
+        )
+
+        assert len(compound_results) == 1
+        assert compound_results[0] == expected_result
```

### Comparing `pythonbible-0.7.4/tests/regular_expressions_test.py` & `pythonbible-0.8/tests/regular_expressions_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 
 def test_chapter_regular_expression() -> None:
     # given a string with a chapter number
     chapter_string: str = "The chapter number is 132."
 
     # when evaluating that string against the chapter regular expression
     matches: Match[str] | None = re.search(
-        regular_expressions.CHAPTER_REGEX,
+        regular_expressions.CHAPTER,
         chapter_string,
     )
 
     # then the match is found
     assert matches and matches.group(0) == "132"
 
 
 def test_verse_regular_expression() -> None:
     # given a string with a verse number
     verse_string: str = "The verse number is 25."
 
     # when evaluating that string against the verse regular expression
     matches: Match[str] | None = re.search(
-        regular_expressions.VERSE_REGEX,
+        regular_expressions.VERSE,
         verse_string,
     )
 
     # then the match is found
     assert matches and matches.group(0) == "25"
 
 
@@ -47,42 +47,45 @@
         # given a string with a chapter and verse reference
         chapter_and_verse_string: str = (
             f"The chapter and verse reference is {reference}."
         )
 
         # when evaluating that string against the chapter and verse regular expression
         matches: Match[str] | None = re.search(
-            regular_expressions.CHAPTER_AND_VERSE_REGEX,
+            regular_expressions.CHAPTER_AND_VERSE,
             chapter_and_verse_string,
         )
 
         # then the match is found
         assert matches and matches.group(0) == reference
 
 
-def test_chapter_range_regular_expression() -> None:
-    chapter_range_references: list[str] = [
-        "1:2-3",
-        "3-4",
-        "142 : 5 - 53 : 23",
-        "43:    324 - 325",
-    ]
+def test_range_regular_expression() -> None:
+    range_references: dict[str, str] = {
+        "1:2-3": "-3",
+        "3-4": "-4",
+        "142 : 5 - 53 : 23": " - 53 : 23",
+        "43:    324 - 325": " - 325",
+        "Genesis - Deuteronomy": " - Deuteronomy",
+        "Genesis 1 - Exodus 2": " - Exodus 2",
+        "Genesis 1:1 - Exodus 2:2": " - Exodus 2:2",
+    }
 
-    for reference in chapter_range_references:
+    for reference, expected_match in range_references.items():
         # given a string with a chapter range reference
-        chapter_range_string: str = f"The chapter range reference is {reference}."
+        chapter_range_string: str = f"The chapter range reference is {reference}"
 
         # when evaluating that string against the chapter range regular expression
         matches: Match[str] | None = re.search(
-            regular_expressions.RANGE_REGEX,
+            regular_expressions.RANGE,
             chapter_range_string,
         )
 
         # then the match is found
-        assert matches and matches.group(0) == reference
+        assert matches and matches.group(0) == expected_match
 
 
 def test_additional_reference_regular_expression() -> None:
     additional_references: list[str] = [
         "1:2,4",
         "3-4,6",
         "123 : 5 - 13, 16 - 18",
@@ -92,15 +95,15 @@
     for reference in additional_references:
         # given a string with an additional reference
         additional_reference_string: str = f"The additional reference is {reference}."
 
         # when evaluating that string against the additional reference regular
         # expression
         matches: Match[str] | None = re.search(
-            regular_expressions.FULL_CHAPTER_AND_VERSE_REGEX,
+            regular_expressions.FULL_CHAPTER_AND_VERSE,
             additional_reference_string,
         )
 
         # then the match is found
         assert matches and matches.group(0) == reference
 
 
@@ -109,15 +112,15 @@
     full_string: str = (
         "You should read Matthew 1:18 - 2:18, Luke 3: 5-7, "
         "Psalm 130:4,8 and Jeremiah 29:32-30:10,11"
     )
 
     # when evaluating that string against the full regular expression
     matches: list[Match[str]] = re.findall(
-        regular_expressions.FULL_CHAPTER_AND_VERSE_REGEX,
+        regular_expressions.FULL_CHAPTER_AND_VERSE,
         full_string,
     )
 
     # then the matches are found
     assert len(matches) == 4
     assert matches[0][0] == "1:18 - 2:18"
     assert matches[1][0] == "3: 5-7"
@@ -205,11 +208,74 @@
     assert len(matches) == 1
 
 
 def test_cross_book_regex() -> None:
     # given a reference that ranges over multiple books
     text: str = "The books of the law are Genesis - Deuteronomy"
 
-    matches: list[Match[str]] = re.findall(regular_expressions.CROSS_BOOK_REGEX, text)
+    matches: list[Match[str]] = re.findall(regular_expressions.CROSS_BOOK, text)
 
     assert len(matches) == 1
     assert matches[0][0] == "Genesis - Deuteronomy"
+
+
+def test_jo() -> None:
+    # "Jo" should match to John, but make sure "Joshua", "Job", and "Jonah" do not
+    # match to John
+
+    # given a reference with the abbreviation "Jo"
+    text = "Jo 1:1"
+
+    # when evaluating the string to see if it matches the Philemon regular expression
+    matches = re.findall(
+        regular_expressions.BOOK_REGULAR_EXPRESSIONS.get(bible.Book.JOHN, ""),
+        text,
+    )
+
+    # then the match is found
+    assert len(matches) == 1
+
+    # given strings that should not match
+    test_strings = [
+        "Joshua",
+        "Job",
+        "Jonah",
+    ]
+
+    for text in test_strings:
+        # when evaluating the string to see if it matches the John regular expression
+        matches: list[Match[str]] = re.findall(
+            regular_expressions.BOOK_REGULAR_EXPRESSIONS.get(bible.Book.JOHN, ""),
+            f"{text} 1:1",
+        )
+
+        # then the matches are not found
+        assert not matches
+
+
+def test_jud() -> None:
+    # "Jud" should match to Jude, but make sure "Judges" does not match to Jude
+
+    # given a reference with the abbreviation "Jud"
+    text = "Jud 1:1"
+
+    # when evaluating the string to see if it matches the Philemon regular expression
+    matches = re.findall(
+        regular_expressions.BOOK_REGULAR_EXPRESSIONS.get(bible.Book.JUDE, ""),
+        text,
+    )
+
+    # then the match is found
+    assert len(matches) == 1
+
+    # given a reference that should not match
+    # given a reference with the abbreviation "Jud"
+    text = "Judges 1:1"
+
+    # when evaluating the string to see if it matches the Philemon regular expression
+    matches = re.findall(
+        regular_expressions.BOOK_REGULAR_EXPRESSIONS.get(bible.Book.JUDE, ""),
+        text,
+    )
+
+    # then the match is found
+    assert not matches
```

### Comparing `pythonbible-0.7.4/tests/validator_test.py` & `pythonbible-0.8/tests/validator_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/tests/verses_test.py` & `pythonbible-0.8/tests/verses_test.py`

 * *Files identical despite different names*

### Comparing `pythonbible-0.7.4/tests/zzz_osis_parser_test.py` & `pythonbible-0.8/tests/zzz_osis_parser_test.py`

 * *Files identical despite different names*

