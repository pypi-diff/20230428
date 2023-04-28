# Comparing `tmp/clipped-0.3.0.tar.gz` & `tmp/clipped-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.3.0.tar", last modified: Tue Apr 25 12:19:07 2023, max compression
+gzip compressed data, was "clipped-0.3.1.tar", last modified: Fri Apr 28 16:29:17 2023, max compression
```

## Comparing `clipped-0.3.0.tar` & `clipped-0.3.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-25 12:19:07.692139 clipped-0.3.0/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-25 12:18:17.000000 clipped-0.3.0/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-25 12:19:07.692206 clipped-0.3.0/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-25 12:19:07.683940 clipped-0.3.0/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-25 12:19:07.685536 clipped-0.3.0/clipped/config/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/constants.py
--rw-r--r--   0 mourad     (501) staff       (20)      312 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/contexts.py
--rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/exceptions.py
--rw-r--r--   0 mourad     (501) staff       (20)     8943 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/manager.py
--rw-r--r--   0 mourad     (501) staff       (20)     6138 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/parser.py
--rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/patch_strategy.py
--rw-r--r--   0 mourad     (501) staff       (20)     4047 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/reader.py
--rw-r--r--   0 mourad     (501) staff       (20)    14833 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/schema.py
--rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/config/spec.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-25 12:19:07.686101 clipped-0.3.0/clipped/decorators/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/decorators/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/decorators/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/decorators/deprecation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/decorators/memoization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/decorators/signals.py
--rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/py.typed
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-25 12:19:07.687686 clipped-0.3.0/clipped/types/
--rw-r--r--   0 mourad     (501) staff       (20)     3914 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/docker_image.py
--rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/email.py
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)      698 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/numbers.py
--rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/ref_or_obj.py
--rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)      965 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/uri.py
--rw-r--r--   0 mourad     (501) staff       (20)      688 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/uuids.py
--rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/types/wasb.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-25 12:19:07.692029 clipped-0.3.0/clipped/utils/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1655 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/assertions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/bools.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/click.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/csv.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/dates.py
--rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/dicts.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/enums.py
--rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/git.py
--rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/http.py
--rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      420 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/json.py
--rw-r--r--   0 mourad     (501) staff       (20)     1163 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/logging.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/np.py
--rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/paths.py
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/requests.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/responses.py
--rw-r--r--   0 mourad     (501) staff       (20)      595 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/tz.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/units.py
--rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/urls.py
--rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/workers.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-25 12:18:17.000000 clipped-0.3.0/clipped/utils/yaml.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-25 12:19:07.684398 clipped-0.3.0/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-25 12:19:07.000000 clipped-0.3.0/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1901 2023-04-25 12:19:07.000000 clipped-0.3.0/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-25 12:19:07.000000 clipped-0.3.0/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-25 12:19:07.000000 clipped-0.3.0/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-25 12:19:07.692557 clipped-0.3.0/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-25 12:18:17.000000 clipped-0.3.0/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:29:17.587962 clipped-0.3.1/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-28 16:27:50.000000 clipped-0.3.1/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-28 16:29:17.588072 clipped-0.3.1/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:29:17.575031 clipped-0.3.1/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:29:17.578216 clipped-0.3.1/clipped/config/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/constants.py
+-rw-r--r--   0 mourad     (501) staff       (20)      312 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/contexts.py
+-rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/exceptions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8943 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/manager.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6138 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/parser.py
+-rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/patch_strategy.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4047 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/reader.py
+-rw-r--r--   0 mourad     (501) staff       (20)    14833 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/config/spec.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:29:17.579139 clipped-0.3.1/clipped/decorators/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/decorators/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/decorators/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/decorators/deprecation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/decorators/memoization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/decorators/signals.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/py.typed
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:29:17.581373 clipped-0.3.1/clipped/types/
+-rw-r--r--   0 mourad     (501) staff       (20)     3914 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/docker_image.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/email.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)      698 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/numbers.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/ref_or_obj.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)      965 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/uri.py
+-rw-r--r--   0 mourad     (501) staff       (20)      688 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/uuids.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/types/wasb.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:29:17.587797 clipped-0.3.1/clipped/utils/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1655 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/assertions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/bools.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/click.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/csv.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/dates.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3358 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/dicts.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/enums.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/git.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/http.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      420 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/json.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1163 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/logging.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/np.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/paths.py
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/requests.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/responses.py
+-rw-r--r--   0 mourad     (501) staff       (20)      595 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/tz.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/units.py
+-rw-r--r--   0 mourad     (501) staff       (20)      282 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/urls.py
+-rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/workers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-28 16:27:50.000000 clipped-0.3.1/clipped/utils/yaml.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:29:17.575870 clipped-0.3.1/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-28 16:29:17.000000 clipped-0.3.1/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1901 2023-04-28 16:29:17.000000 clipped-0.3.1/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-28 16:29:17.000000 clipped-0.3.1/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-28 16:29:17.000000 clipped-0.3.1/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-28 16:29:17.588648 clipped-0.3.1/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-28 16:27:50.000000 clipped-0.3.1/setup.py
```

### Comparing `clipped-0.3.0/PKG-INFO` & `clipped-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.3.0
+Version: 0.3.1
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.3.0 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.3.1 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.3.0/clipped/config/manager.py` & `clipped-0.3.1/clipped/config/manager.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/config/parser.py` & `clipped-0.3.1/clipped/config/parser.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/config/patch_strategy.py` & `clipped-0.3.1/clipped/config/patch_strategy.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/config/reader.py` & `clipped-0.3.1/clipped/config/reader.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/config/schema.py` & `clipped-0.3.1/clipped/config/schema.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/config/spec.py` & `clipped-0.3.1/clipped/config/spec.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/decorators/cached_property.py` & `clipped-0.3.1/clipped/decorators/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/decorators/deprecation.py` & `clipped-0.3.1/clipped/decorators/deprecation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/decorators/memoization.py` & `clipped-0.3.1/clipped/decorators/memoization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/decorators/signals.py` & `clipped-0.3.1/clipped/decorators/signals.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/formatting.py` & `clipped-0.3.1/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/manager_interface.py` & `clipped-0.3.1/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/__init__.py` & `clipped-0.3.1/clipped/types/__init__.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/docker_image.py` & `clipped-0.3.1/clipped/types/docker_image.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/email.py` & `clipped-0.3.1/clipped/types/email.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/gcs.py` & `clipped-0.3.1/clipped/types/gcs.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/lists.py` & `clipped-0.3.1/clipped/types/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/ref_or_obj.py` & `clipped-0.3.1/clipped/types/ref_or_obj.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/s3.py` & `clipped-0.3.1/clipped/types/s3.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/strings.py` & `clipped-0.3.1/clipped/types/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/uri.py` & `clipped-0.3.1/clipped/types/uri.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/uuids.py` & `clipped-0.3.1/clipped/types/uuids.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/types/wasb.py` & `clipped-0.3.1/clipped/types/wasb.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/assertions.py` & `clipped-0.3.1/clipped/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/bools.py` & `clipped-0.3.1/clipped/utils/bools.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/cmd.py` & `clipped-0.3.1/clipped/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/coroutine.py` & `clipped-0.3.1/clipped/utils/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/csv.py` & `clipped-0.3.1/clipped/utils/csv.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/dates.py` & `clipped-0.3.1/clipped/utils/dates.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/dicts.py` & `clipped-0.3.1/clipped/utils/dicts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Optional, Tuple
 
-from clipped.formatting import humanize_attrs
+from clipped.utils.humanize import humanize_attrs
 
 
 def deep_update(config: Dict, override_config: Dict):
     for k, v in override_config.items():
         if isinstance(v, dict):
             k_config = config.get(k, {})
             if isinstance(k_config, dict):
```

### Comparing `clipped-0.3.0/clipped/utils/enums.py` & `clipped-0.3.1/clipped/utils/enums.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/env.py` & `clipped-0.3.1/clipped/utils/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/git.py` & `clipped-0.3.1/clipped/utils/git.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/hashing.py` & `clipped-0.3.1/clipped/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/http.py` & `clipped-0.3.1/clipped/utils/http.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/humanize.py` & `clipped-0.3.1/clipped/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/imports.py` & `clipped-0.3.1/clipped/utils/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/indentation.py` & `clipped-0.3.1/clipped/utils/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/lists.py` & `clipped-0.3.1/clipped/utils/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/np.py` & `clipped-0.3.1/clipped/utils/np.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/paths.py` & `clipped-0.3.1/clipped/utils/paths.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/query_params.py` & `clipped-0.3.1/clipped/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/requests.py` & `clipped-0.3.1/clipped/utils/requests.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/responses.py` & `clipped-0.3.1/clipped/utils/responses.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/sanitizers.py` & `clipped-0.3.1/clipped/utils/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/serialization.py` & `clipped-0.3.1/clipped/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/strings.py` & `clipped-0.3.1/clipped/utils/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/tz.py` & `clipped-0.3.1/clipped/utils/tz.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/units.py` & `clipped-0.3.1/clipped/utils/units.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/validation.py` & `clipped-0.3.1/clipped/utils/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/versions.py` & `clipped-0.3.1/clipped/utils/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/workers.py` & `clipped-0.3.1/clipped/utils/workers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped/utils/yaml.py` & `clipped-0.3.1/clipped/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/clipped.egg-info/PKG-INFO` & `clipped-0.3.1/clipped.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.3.0
+Version: 0.3.1
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.3.0 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.3.1 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.3.0/clipped.egg-info/SOURCES.txt` & `clipped-0.3.1/clipped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/setup.cfg` & `clipped-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.3.0/setup.py` & `clipped-0.3.1/setup.py`

 * *Files identical despite different names*

