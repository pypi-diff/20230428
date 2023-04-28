# Comparing `tmp/curies-0.5.3.tar.gz` & `tmp/curies-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curies-0.5.3.tar", last modified: Sun Mar 26 14:23:28 2023, max compression
+gzip compressed data, was "curies-0.5.4.tar", last modified: Fri Apr 28 13:06:22 2023, max compression
```

## Comparing `curies-0.5.3.tar` & `curies-0.5.4.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.455103 curies-0.5.3/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-07-31 23:04:00.000000 curies-0.5.3/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      394 2023-02-21 22:19:21.000000 curies-0.5.3/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)    11651 2023-03-26 14:23:28.455327 curies-0.5.3/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)    10132 2023-03-26 09:36:33.000000 curies-0.5.3/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.426009 curies-0.5.3/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.430020 curies-0.5.3/docs/source/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.441696 curies-0.5.3/docs/source/api/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1864 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.Converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      101 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.DuplicatePrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.DuplicateURIPrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      107 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.DuplicateValueError.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       86 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.Record.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.chain.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_bioregistry_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       94 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_fastapi_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_flask_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_flask_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_go_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_monarch_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      100 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_obo_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_prefixcommons_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.get_version.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      141 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      134 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      119 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.mapping_service.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-03-16 13:59:10.000000 curies-0.5.3/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7458 2023-03-26 14:23:27.000000 curies-0.5.3/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2538 2023-03-10 11:58:39.000000 curies-0.5.3/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      385 2022-12-09 17:27:17.000000 curies-0.5.3/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2668 2023-03-26 14:23:28.456316 curies-0.5.3/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.426950 curies-0.5.3/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.446946 curies-0.5.3/src/curies/
--rw-r--r--   0 cthoyt     (501) staff       (20)      941 2023-02-21 22:19:21.000000 curies-0.5.3/src/curies/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-02-21 22:19:21.000000 curies-0.5.3/src/curies/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    38646 2023-03-04 17:32:48.000000 curies-0.5.3/src/curies/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5065 2023-03-25 17:38:08.000000 curies-0.5.3/src/curies/cli.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.451146 curies-0.5.3/src/curies/mapping_service/
--rw-r--r--   0 cthoyt     (501) staff       (20)    14115 2023-03-26 09:35:44.000000 curies-0.5.3/src/curies/mapping_service/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-03-16 13:57:56.000000 curies-0.5.3/src/curies/mapping_service/rdflib_custom.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1490 2023-03-26 10:12:45.000000 curies-0.5.3/src/curies/mapping_service/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:01.000000 curies-0.5.3/src/curies/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     2033 2023-03-04 12:32:17.000000 curies-0.5.3/src/curies/sources.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      255 2023-03-26 14:23:27.000000 curies-0.5.3/src/curies/version.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     9620 2023-02-21 22:19:21.000000 curies-0.5.3/src/curies/web.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.449462 curies-0.5.3/src/curies.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)    11651 2023-03-26 14:23:28.000000 curies-0.5.3/src/curies.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1819 2023-03-26 14:23:28.000000 curies-0.5.3/src/curies.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-03-26 14:23:28.000000 curies-0.5.3/src/curies.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:24.000000 curies-0.5.3/src/curies.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      273 2023-03-26 14:23:28.000000 curies-0.5.3/src/curies.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        7 2023-03-26 14:23:28.000000 curies-0.5.3/src/curies.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-26 14:23:28.454564 curies-0.5.3/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       56 2022-07-31 23:04:00.000000 curies-0.5.3/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        0 2023-03-23 13:16:42.000000 curies-0.5.3/tests/rules.log
--rw-r--r--   0 cthoyt     (501) staff       (20)    17050 2023-03-04 17:32:48.000000 curies-0.5.3/tests/test_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4194 2023-03-26 10:14:41.000000 curies-0.5.3/tests/test_federated_sparql.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    13000 2023-03-26 09:35:44.000000 curies-0.5.3/tests/test_mapping_service.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2425 2023-03-10 12:55:57.000000 curies-0.5.3/tests/test_web.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.020704 curies-0.5.4/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-07-31 23:04:00.000000 curies-0.5.4/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      394 2023-04-28 13:05:54.000000 curies-0.5.4/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11651 2023-04-28 13:06:22.021134 curies-0.5.4/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10132 2023-04-28 13:05:54.000000 curies-0.5.4/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:21.989361 curies-0.5.4/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:21.993328 curies-0.5.4/docs/source/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.005335 curies-0.5.4/docs/source/api/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1864 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.Converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      101 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.DuplicatePrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.DuplicateURIPrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      107 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.DuplicateValueError.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       86 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.Record.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.chain.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_bioregistry_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       94 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_fastapi_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_flask_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_flask_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_go_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_monarch_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_obo_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_prefixcommons_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_version.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      141 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      134 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      119 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7458 2023-04-28 13:06:20.000000 curies-0.5.4/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2538 2023-03-10 11:58:39.000000 curies-0.5.4/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      385 2022-12-09 17:27:17.000000 curies-0.5.4/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2668 2023-04-28 13:06:22.022415 curies-0.5.4/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:21.990101 curies-0.5.4/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.010973 curies-0.5.4/src/curies/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      941 2023-02-21 22:19:21.000000 curies-0.5.4/src/curies/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-02-21 22:19:21.000000 curies-0.5.4/src/curies/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    38646 2023-04-13 06:17:21.000000 curies-0.5.4/src/curies/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5065 2023-04-13 07:17:14.000000 curies-0.5.4/src/curies/cli.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.016123 curies-0.5.4/src/curies/mapping_service/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-04-13 07:57:38.000000 curies-0.5.4/src/curies/mapping_service/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8222 2023-04-13 07:57:38.000000 curies-0.5.4/src/curies/mapping_service/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-03-26 20:29:12.000000 curies-0.5.4/src/curies/mapping_service/rdflib_custom.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4637 2023-04-28 13:05:54.000000 curies-0.5.4/src/curies/mapping_service/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:01.000000 curies-0.5.4/src/curies/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2033 2023-03-04 12:32:17.000000 curies-0.5.4/src/curies/sources.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      255 2023-04-28 13:06:20.000000 curies-0.5.4/src/curies/version.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9666 2023-04-13 06:43:24.000000 curies-0.5.4/src/curies/web.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.013893 curies-0.5.4/src/curies.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11651 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1853 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:24.000000 curies-0.5.4/src/curies.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      273 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        7 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.019823 curies-0.5.4/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       56 2022-07-31 23:04:00.000000 curies-0.5.4/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        0 2023-03-23 13:16:42.000000 curies-0.5.4/tests/rules.log
+-rw-r--r--   0 cthoyt     (501) staff       (20)    17050 2023-04-13 06:17:21.000000 curies-0.5.4/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-04-13 10:20:39.000000 curies-0.5.4/tests/test_federated_sparql.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    13426 2023-04-13 07:57:38.000000 curies-0.5.4/tests/test_mapping_service.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3271 2023-04-13 06:37:08.000000 curies-0.5.4/tests/test_web.py
```

### Comparing `curies-0.5.3/LICENSE` & `curies-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/PKG-INFO` & `curies-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.5.3
+Version: 0.5.4
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies Version: 0.5.3 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.5.4 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies Classifier:
```

### Comparing `curies-0.5.3/README.md` & `curies-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/docs/source/api/curies.Converter.rst` & `curies-0.5.4/docs/source/api/curies.Converter.rst`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/docs/source/conf.py` & `curies-0.5.4/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "curies"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.5.3"
+release = "0.5.4"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `curies-0.5.3/docs/source/index.rst` & `curies-0.5.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/setup.cfg` & `curies-0.5.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = curies
-version = 0.5.3
+version = 0.5.4
 description = Idiomatic conversion between URIs and compact URIs (CURIEs).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/curies
 download_url = https://github.com/cthoyt/curies/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/curies/issues
```

### Comparing `curies-0.5.3/src/curies/__init__.py` & `curies-0.5.4/src/curies/__init__.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/src/curies/api.py` & `curies-0.5.4/src/curies/api.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/src/curies/cli.py` & `curies-0.5.4/src/curies/cli.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/src/curies/mapping_service/rdflib_custom.py` & `curies-0.5.4/src/curies/mapping_service/rdflib_custom.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/src/curies/sources.py` & `curies-0.5.4/src/curies/sources.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/src/curies/web.py` & `curies-0.5.4/src/curies/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         >>> requests.get("http://localhost:8764/GO:0032571").url
         'http://amigo.geneontology.org/amigo/term/GO:0032571'
     """
     from flask import Blueprint, abort, redirect
 
     blueprint = Blueprint("metaresolver", __name__, **kwargs)
 
-    @blueprint.route("/<prefix>:<path:identifier>")  # type:ignore
+    @blueprint.route(f"/<prefix>{converter.delimiter}<path:identifier>")  # type:ignore
     def resolve(prefix: str, identifier: str) -> "Response":
         """Resolve a CURIE."""
         location = converter.expand_pair(prefix, identifier)
         if location is None:
             prefixes = "".join(f"\n- {p}" for p in sorted(converter.get_prefixes()))
             return abort(FAILURE_CODE, f"Invalid prefix: {prefix}. Use one of:{prefixes}")
         return redirect(location)
@@ -197,15 +197,15 @@
         'http://amigo.geneontology.org/amigo/term/GO:0032571'
     """
     from fastapi import APIRouter, HTTPException, Path
     from fastapi.responses import RedirectResponse
 
     api_router = APIRouter(**kwargs)
 
-    @api_router.get("/{prefix}:{identifier}")  # type:ignore
+    @api_router.get(f"/{{prefix}}{converter.delimiter}{{identifier}}")  # type:ignore
     def resolve(
         prefix: str = Path(  # noqa:B008
             title="Prefix",
             description="The Bioregistry prefix corresponding to an identifier resource.",
             example="doid",
         ),
         identifier: str = Path(  # noqa:B008
```

### Comparing `curies-0.5.3/src/curies.egg-info/PKG-INFO` & `curies-0.5.4/src/curies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.5.3
+Version: 0.5.4
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies Version: 0.5.3 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.5.4 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies Classifier:
```

### Comparing `curies-0.5.3/src/curies.egg-info/SOURCES.txt` & `curies-0.5.4/src/curies.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/curies.egg-info/PKG-INFO
 src/curies.egg-info/SOURCES.txt
 src/curies.egg-info/dependency_links.txt
 src/curies.egg-info/not-zip-safe
 src/curies.egg-info/requires.txt
 src/curies.egg-info/top_level.txt
 src/curies/mapping_service/__init__.py
+src/curies/mapping_service/api.py
 src/curies/mapping_service/rdflib_custom.py
 src/curies/mapping_service/utils.py
 tests/__init__.py
 tests/rules.log
 tests/test_api.py
 tests/test_federated_sparql.py
 tests/test_mapping_service.py
```

### Comparing `curies-0.5.3/tests/test_api.py` & `curies-0.5.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.3/tests/test_mapping_service.py` & `curies-0.5.4/tests/test_mapping_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 
 from fastapi.testclient import TestClient
 from rdflib import OWL, SKOS
 from rdflib.query import ResultRow
 
 from curies import Converter
 from curies.mapping_service import (
-    CONTENT_TYPE_SYNONYMS,
     MappingServiceGraph,
     MappingServiceSPARQLProcessor,
-    _handle_header,
-    _prepare_predicates,
     get_fastapi_mapping_app,
     get_flask_mapping_app,
 )
-from curies.mapping_service.utils import CONTENT_TYPE_TO_HANDLER
+from curies.mapping_service.api import _prepare_predicates
+from curies.mapping_service.utils import (
+    CONTENT_TYPE_SYNONYMS,
+    CONTENT_TYPE_TO_HANDLER,
+    handle_header,
+    sparql_service_available,
+)
 
 VALID_CONTENT_TYPES = {
     *CONTENT_TYPE_TO_HANDLER,
     "",
     "*/*",
     *CONTENT_TYPE_SYNONYMS,
 }
@@ -112,15 +115,15 @@
             "application/xml;q=0.8,"
             "application/x-binary-rdf-results-table,"
             "application/sparql-results+json;q=0.8,"
             "application/json;q=0.8,"
             "text/csv;q=0.8,"
             "text/tab-separated-values;q=0.8"
         )
-        content_type = _handle_header(example_header)
+        content_type = handle_header(example_header)
         self.assertEqual("application/sparql-results+xml", content_type)
 
     def test_prepare_predicates(self):
         """Test preparation of predicates."""
         self.assertEqual({OWL.sameAs}, _prepare_predicates())
         self.assertEqual({OWL.sameAs}, _prepare_predicates(OWL.sameAs))
         self.assertEqual(
@@ -197,26 +200,26 @@
     def setUp(self) -> None:
         """Set up the test case with a converter."""
         super().setUp()
         self.converter = Converter.from_priority_prefix_map(PREFIX_MAP)
 
     def assert_mimetype(self, res, content_type):
         """Assert the correct MIMETYPE."""
-        content_type = _handle_header(content_type)
+        content_type = handle_header(content_type)
         mimetype = getattr(res, "mimetype", None)
         if hasattr(res, "mimetype"):  # this is from Flask
             self.assertEqual(content_type, mimetype)
         else:  # this is from FastAPI
             actual_content_type = res.headers.get("content-type")
             self.assertIsNotNone(actual_content_type)
             self.assertEqual(content_type, actual_content_type.split(";")[0].strip())
 
     def assert_parsed(self, res, content_type: str):
         """Test the result has the expected output."""
-        content_type = _handle_header(content_type)
+        content_type = handle_header(content_type)
         parse_func = CONTENT_TYPE_TO_HANDLER[content_type]
         records = parse_func(res.text)
         pairs = {(record["s"], record["o"]) for record in records}
         self.assertEqual(EXPECTED, pairs)
 
     def assert_get_sparql_results(self, client, sparql):
         """Test a sparql query returns expected values."""
@@ -326,7 +329,18 @@
     def test_get_service_query(self):
         """Test sparql generated by a service (that has values outside of where clause) with GET."""
         self.assert_get_sparql_results(self.client, SPARQL_FROM_SERVICE)
 
     def test_post_service_query(self):
         """Test sparql generated by a service (that has values outside of where clause) with POST."""
         self.assert_post_sparql_results(self.client, SPARQL_FROM_SERVICE)
+
+
+class TestUtils(unittest.TestCase):
+    """Test utilities."""
+
+    def test_availability(self):
+        """Test sparql service availability check."""
+        self.assertTrue(
+            sparql_service_available("https://query.wikidata.org/bigdata/namespace/wdq/sparql")
+        )
+        self.assertFalse(sparql_service_available("https://example.org"))
```

### Comparing `curies-0.5.3/tests/test_web.py` & `curies-0.5.4/tests/test_web.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,95 @@
 # -*- coding: utf-8 -*-
 
 """Tests for the simple web service."""
 
 import unittest
+from typing import ClassVar
 
 from fastapi.testclient import TestClient
 
 from curies import Converter
 from curies.web import FAILURE_CODE, get_fastapi_app, get_flask_app
 
 
 class ConverterMixin(unittest.TestCase):
     """A mixin that has a converter."""
 
+    delimiter: ClassVar[str] = ":"
+
     def setUp(self) -> None:
         """Set up the test case with a converter."""
         super().setUp()
         self.converter = Converter.from_prefix_map(
             {
                 "CHEBI": "http://purl.obolibrary.org/obo/CHEBI_",
                 "MONDO": "http://purl.obolibrary.org/obo/MONDO_",
                 "GO": "http://purl.obolibrary.org/obo/GO_",
                 "OBO": "http://purl.obolibrary.org/obo/",
-            }
+            },
+            delimiter=self.delimiter,
         )
 
 
 class TestFastAPI(ConverterMixin):
     """Test building a simple web service with FastAPI."""
 
     def setUp(self) -> None:
         """Set up the test case with a converter, blueprint, and app."""
         super().setUp()
         self.app = get_fastapi_app(self.converter)
         self.client = TestClient(self.app)
 
     def test_resolve_success(self):
         """Test resolution for a valid CURIE redirects properly."""
-        res = self.client.get("/GO:1234567", allow_redirects=False)
+        curie = self.converter.format_curie("GO", "1234567")
+        res = self.client.get(f"/{curie}", allow_redirects=False)
         self.assertEqual(302, res.status_code, msg=res.text)
 
     def test_resolve_failure(self):
         """Test resolution for an invalid CURIE aborts with 404."""
-        res = self.client.get("/NOPREFIX:NOIDENTIFIER", allow_redirects=False)
+        curie = self.converter.format_curie("NOPREFIX", "NOIDENTIFIER")
+        res = self.client.get(f"/{curie}", allow_redirects=False)
         self.assertEqual(FAILURE_CODE, res.status_code, msg=res.text)
 
 
+class TestFastAPISlashed(TestFastAPI):
+    """Test the FastAPI router with an alternate delimiter."""
+
+    delimiter = "/"
+
+    def test_delimiter(self):
+        """Test the delimiter."""
+        self.assertEqual("/", self.converter.delimiter)
+
+
 class TestFlaskBlueprint(ConverterMixin):
     """Test building a simple web service with Flask."""
 
     def setUp(self) -> None:
         """Set up the test case with a converter, blueprint, and app."""
         super().setUp()
         self.app = get_flask_app(self.converter)
 
     def test_resolve_success(self):
         """Test resolution for a valid CURIE redirects properly."""
+        curie = self.converter.format_curie("GO", "1234567")
         with self.app.test_client() as client:
-            res = client.get("/GO:1234567", follow_redirects=False)
+            res = client.get(f"/{curie}", follow_redirects=False)
             self.assertEqual(302, res.status_code, msg=res.text)
 
     def test_resolve_failure(self):
         """Test resolution for an invalid CURIE aborts with 404."""
+        curie = self.converter.format_curie("NOPREFIX", "NOIDENTIFIER")
         with self.app.test_client() as client:
-            res = client.get("/NOPREFIX:NOIDENTIFIER", follow_redirects=False)
+            res = client.get(f"/{curie}", follow_redirects=False)
             self.assertEqual(FAILURE_CODE, res.status_code, msg=res.text)
+
+
+class TestFlaskBlueprintSlashed(TestFlaskBlueprint):
+    """Test the flask blueprint with an alternate delimiter."""
+
+    delimiter = "/"
+
+    def test_delimiter(self):
+        """Test the delimiter."""
+        self.assertEqual("/", self.converter.delimiter)
```

