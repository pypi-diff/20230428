# Comparing `tmp/pysd-3.9.0.tar.gz` & `tmp/pysd-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysd-3.9.0.tar", last modified: Fri Dec 16 19:06:47 2022, max compression
+gzip compressed data, was "dist/pysd-3.9.1.tar", last modified: Sat Mar 11 19:09:36 2023, max compression
```

## Comparing `pysd-3.9.0.tar` & `pysd-3.9.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2022-12-16 19:06:39.000000 pysd-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-16 19:06:39.000000 pysd-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2022-12-16 19:06:47.000000 pysd-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2022-12-16 19:06:39.000000 pysd-3.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   121977 2022-12-16 19:06:39.000000 pysd-3.9.0/docs/images/PySD_Logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2022-12-16 19:06:39.000000 pysd-3.9.0/docs/images/PySD_Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30023 2022-12-16 19:06:39.000000 pysd-3.9.0/docs/images/PySD_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12532 2022-12-16 19:06:39.000000 pysd-3.9.0/docs/images/PySD_Logo_letters.png
--rw-r--r--   0 runner    (1001) docker     (123)    33101 2022-12-16 19:06:39.000000 pysd-3.9.0/docs/images/PySD_Logo_letters.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/builders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/builders/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/builders/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/builders/python/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/builders/python/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    80178 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/builders/python/python_expressions_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/builders/python/python_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32830 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/builders/python/python_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16099 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/builders/python/subscripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/cli/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/py_backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25455 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35135 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    26631 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/lookups.py
--rw-r--r--   0 runner    (1001) docker     (123)    72889 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17291 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/statefuls.py
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/py_backend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/pysd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/tools/benchmarking.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/tools/ncfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/translators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/translators/structures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15518 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/structures/abstract_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14771 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/structures/abstract_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/translators/vensim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/translators/vensim/parsing_grammars/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/parsing_grammars/common_grammar.peg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/parsing_grammars/components.peg
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/parsing_grammars/element_object.peg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/parsing_grammars/file_sections.peg
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/parsing_grammars/lookups.peg
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/parsing_grammars/section_elements.peg
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/parsing_grammars/sketch.peg
--rw-r--r--   0 runner    (1001) docker     (123)    27098 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/vensim_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/vensim_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/vensim_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/vensim_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/vensim/vensim_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/translators/xmile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/xmile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd/translators/xmile/parsing_grammars/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/xmile/parsing_grammars/equations.peg
--rw-r--r--   0 runner    (1001) docker     (123)    21010 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/xmile/xmile_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/xmile/xmile_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/xmile/xmile_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/xmile/xmile_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2022-12-16 19:06:39.000000 pysd-3.9.0/pysd/translators/xmile/xmile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-16 19:06:47.000000 pysd-3.9.0/pysd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-16 19:06:39.000000 pysd-3.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-16 19:06:47.000000 pysd-3.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1250 2022-12-16 19:06:39.000000 pysd-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-11 19:09:23.000000 pysd-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-11 19:09:23.000000 pysd-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-03-11 19:09:36.000000 pysd-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-03-11 19:09:23.000000 pysd-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   121977 2023-03-11 19:09:23.000000 pysd-3.9.1/docs/images/PySD_Logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-11 19:09:23.000000 pysd-3.9.1/docs/images/PySD_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30023 2023-03-11 19:09:23.000000 pysd-3.9.1/docs/images/PySD_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-03-11 19:09:23.000000 pysd-3.9.1/docs/images/PySD_Logo_letters.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33101 2023-03-11 19:09:23.000000 pysd-3.9.1/docs/images/PySD_Logo_letters.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/builders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/builders/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/builders/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/builders/python/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/builders/python/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80208 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/builders/python/python_expressions_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/builders/python/python_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32830 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/builders/python/python_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/builders/python/subscripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/cli/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/py_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25455 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26631 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73232 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/statefuls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/py_backend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/pysd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/tools/benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/tools/ncfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/translators/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/structures/abstract_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/structures/abstract_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/translators/vensim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/translators/vensim/parsing_grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/parsing_grammars/common_grammar.peg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/parsing_grammars/components.peg
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/parsing_grammars/element_object.peg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/parsing_grammars/file_sections.peg
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/parsing_grammars/lookups.peg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/parsing_grammars/section_elements.peg
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/parsing_grammars/sketch.peg
+-rw-r--r--   0 runner    (1001) docker     (123)    27098 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/vensim_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/vensim_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/vensim_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/vensim_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/vensim/vensim_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/translators/xmile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/xmile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd/translators/xmile/parsing_grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/xmile/parsing_grammars/equations.peg
+-rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/xmile/xmile_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/xmile/xmile_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/xmile/xmile_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/xmile/xmile_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-03-11 19:09:23.000000 pysd-3.9.1/pysd/translators/xmile/xmile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-03-11 19:09:35.000000 pysd-3.9.1/pysd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-03-11 19:09:36.000000 pysd-3.9.1/pysd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 19:09:35.000000 pysd-3.9.1/pysd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-11 19:09:35.000000 pysd-3.9.1/pysd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-11 19:09:35.000000 pysd-3.9.1/pysd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-11 19:09:23.000000 pysd-3.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-11 19:09:36.000000 pysd-3.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-03-11 19:09:23.000000 pysd-3.9.1/setup.py
```

### Comparing `pysd-3.9.0/LICENSE` & `pysd-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/PKG-INFO` & `pysd-3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysd
-Version: 3.9.0
+Version: 3.9.1
 Summary: System Dynamics Modeling in Python
 Home-page: https://github.com/SDXorg/pysd
 Author: PySD contributors
 License: LICENSE
 Description: # PySD
         
         [![Maintained](https://img.shields.io/badge/Maintained-Yes-brightgreen.svg)](https://github.com/SDXorg/pysd/pulse)
@@ -75,9 +75,10 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pysd-3.9.0/README.md` & `pysd-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/docs/images/PySD_Logo.ico` & `pysd-3.9.1/docs/images/PySD_Logo.ico`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/docs/images/PySD_Logo.png` & `pysd-3.9.1/docs/images/PySD_Logo.png`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/docs/images/PySD_Logo.svg` & `pysd-3.9.1/docs/images/PySD_Logo.svg`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/docs/images/PySD_Logo_letters.png` & `pysd-3.9.1/docs/images/PySD_Logo_letters.png`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/docs/images/PySD_Logo_letters.svg` & `pysd-3.9.1/docs/images/PySD_Logo_letters.svg`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/builders/python/imports.py` & `pysd-3.9.1/pysd/builders/python/imports.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/builders/python/namespace.py` & `pysd-3.9.1/pysd/builders/python/namespace.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/builders/python/python_expressions_builder.py` & `pysd-3.9.1/pysd/builders/python/python_expressions_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,14 +638,15 @@
                 # Create an xarray from the random function output
                 # NUMPY: not necessary
                 # generate an xarray from the output
                 subs = self.section.subscripts.simplify_subscript_input(
                     self.def_subs)[1]
                 expression = f"xr.DataArray({expression}, {subs}, "\
                     f"{list(self.def_subs)})"
+            calls["time"] = 1
 
         elif self.function == "active_initial":
             # Ee need to ensure that active initial outputs are always the
             # same and update dependencies as stateful object
             name = self.section.namespace.make_python_identifier(
                 self.element.identifier, prefix="_active_initial")
             final_subscripts = self.reorder(arguments, force="equal")
```

### Comparing `pysd-3.9.0/pysd/builders/python/python_functions.py` & `pysd-3.9.1/pysd/builders/python/python_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 # functions that can be diretcly applied over an array
 functionspace = {
     # directly build functions without dependencies
     "elmcount": ("len(%(0)s)", None),
 
     # directly build numpy based functions
+    "pi": ("np.pi", ("numpy",)),
     "abs": ("np.abs(%(0)s)", ("numpy",)),
     "min": ("np.minimum(%(0)s, %(1)s)", ("numpy",)),
     "max": ("np.maximum(%(0)s, %(1)s)", ("numpy",)),
     "exp": ("np.exp(%(0)s)", ("numpy",)),
     "sin": ("np.sin(%(0)s)", ("numpy",)),
     "cos": ("np.cos(%(0)s)", ("numpy",)),
     "tan": ("np.tan(%(0)s)", ("numpy",)),
```

### Comparing `pysd-3.9.0/pysd/builders/python/python_model_builder.py` & `pysd-3.9.1/pysd/builders/python/python_model_builder.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/builders/python/subscripts.py` & `pysd-3.9.1/pysd/builders/python/subscripts.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/cli/main.py` & `pysd-3.9.1/pysd/cli/main.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/cli/parser.py` & `pysd-3.9.1/pysd/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/allocation.py` & `pysd-3.9.1/pysd/py_backend/allocation.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/cache.py` & `pysd-3.9.1/pysd/py_backend/cache.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/components.py` & `pysd-3.9.1/pysd/py_backend/components.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/data.py` & `pysd-3.9.1/pysd/py_backend/data.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/external.py` & `pysd-3.9.1/pysd/py_backend/external.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/functions.py` & `pysd-3.9.1/pysd/py_backend/functions.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/lookups.py` & `pysd-3.9.1/pysd/py_backend/lookups.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/model.py` & `pysd-3.9.1/pysd/py_backend/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,14 +321,17 @@
                 self._constant_funcs.add(element)
 
     def _remove_constant_cache(self):
         for element in self._constant_funcs:
             self.components._set_component(
                 element,
                 getattr(self.components, element).function)
+            # remove attributes added with constant cache
+            delattr(getattr(self.components, element), 'function')
+            delattr(getattr(self.components, element), 'value')
         self._constant_funcs.clear()
 
     def _assign_cache_type(self):
         """
         Assigns the cache type to all the elements from the namespace.
         """
         self.cache_type = {"time": None}
@@ -1062,17 +1065,19 @@
 
             # this won't handle other statefuls...
             if '_integ_' + func_name in dir(self.components):
                 warnings.warn("Replacing the equation of stock "
                               "'{}' with params...".format(key),
                               stacklevel=2)
 
+            # copy attributes from the original object to proper working
+            # of internal functions
             new_function.__name__ = func_name
-            if dims:
-                new_function.dims = dims
+            new_function.__dict__.update(getattr(func, "__dict__", {}))
+            # set the new function
             self.components._set_component(func_name, new_function)
             if func_name in self.cache.cached_funcs:
                 self.cache.cached_funcs.remove(func_name)
 
     def _timeseries_component(self, series, dims):
         """ Internal function for creating a timeseries model element """
         # this is only called if the set_component function recognizes a
```

### Comparing `pysd-3.9.0/pysd/py_backend/output.py` & `pysd-3.9.1/pysd/py_backend/output.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/statefuls.py` & `pysd-3.9.1/pysd/py_backend/statefuls.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/py_backend/utils.py` & `pysd-3.9.1/pysd/py_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/pysd.py` & `pysd-3.9.1/pysd/pysd.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/tools/benchmarking.py` & `pysd-3.9.1/pysd/tools/benchmarking.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/tools/ncfiles.py` & `pysd-3.9.1/pysd/tools/ncfiles.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/structures/abstract_expressions.py` & `pysd-3.9.1/pysd/translators/structures/abstract_expressions.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/structures/abstract_model.py` & `pysd-3.9.1/pysd/translators/structures/abstract_model.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/parsing_grammars/common_grammar.peg` & `pysd-3.9.1/pysd/translators/vensim/parsing_grammars/common_grammar.peg`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/parsing_grammars/components.peg` & `pysd-3.9.1/pysd/translators/vensim/parsing_grammars/components.peg`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/parsing_grammars/element_object.peg` & `pysd-3.9.1/pysd/translators/vensim/parsing_grammars/element_object.peg`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/parsing_grammars/sketch.peg` & `pysd-3.9.1/pysd/translators/vensim/parsing_grammars/sketch.peg`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/vensim_element.py` & `pysd-3.9.1/pysd/translators/vensim/vensim_element.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/vensim_file.py` & `pysd-3.9.1/pysd/translators/vensim/vensim_file.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/vensim_section.py` & `pysd-3.9.1/pysd/translators/vensim/vensim_section.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/vensim_structures.py` & `pysd-3.9.1/pysd/translators/vensim/vensim_structures.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/vensim/vensim_utils.py` & `pysd-3.9.1/pysd/translators/vensim/vensim_utils.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/xmile/parsing_grammars/equations.peg` & `pysd-3.9.1/pysd/translators/xmile/parsing_grammars/equations.peg`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/xmile/xmile_element.py` & `pysd-3.9.1/pysd/translators/xmile/xmile_element.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/xmile/xmile_file.py` & `pysd-3.9.1/pysd/translators/xmile/xmile_file.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/xmile/xmile_section.py` & `pysd-3.9.1/pysd/translators/xmile/xmile_section.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/xmile/xmile_structures.py` & `pysd-3.9.1/pysd/translators/xmile/xmile_structures.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd/translators/xmile/xmile_utils.py` & `pysd-3.9.1/pysd/translators/xmile/xmile_utils.py`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/pysd.egg-info/PKG-INFO` & `pysd-3.9.1/pysd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysd
-Version: 3.9.0
+Version: 3.9.1
 Summary: System Dynamics Modeling in Python
 Home-page: https://github.com/SDXorg/pysd
 Author: PySD contributors
 License: LICENSE
 Description: # PySD
         
         [![Maintained](https://img.shields.io/badge/Maintained-Yes-brightgreen.svg)](https://github.com/SDXorg/pysd/pulse)
@@ -75,9 +75,10 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pysd-3.9.0/pysd.egg-info/SOURCES.txt` & `pysd-3.9.1/pysd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysd-3.9.0/setup.py` & `pysd-3.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Intended Audience :: Science/Research',
 
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     install_requires=open('requirements.txt').read().strip().split('\n'),
     package_data={
         'translators': [
             '*/parsing_grammars/*.peg'
         ]
     },
```

