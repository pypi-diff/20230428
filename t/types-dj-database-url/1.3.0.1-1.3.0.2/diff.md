# Comparing `tmp/types-dj-database-url-1.3.0.1.tar.gz` & `tmp/types-dj-database-url-1.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-dj-database-url-1.3.0.1.tar", last modified: Mon Apr 24 12:30:06 2023, max compression
+gzip compressed data, was "types-dj-database-url-1.3.0.2.tar", last modified: Fri Apr 28 09:14:29 2023, max compression
```

## Comparing `types-dj-database-url-1.3.0.1.tar` & `types-dj-database-url-1.3.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/dj_database_url-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/dj_database_url-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/dj_database_url-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-24 12:30:06.000000 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-24 12:30:06.000000 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:30:06.000000 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 12:30:06.000000 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:14:29.451319 types-dj-database-url-1.3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-28 09:14:27.000000 types-dj-database-url-1.3.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 09:14:27.000000 types-dj-database-url-1.3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-28 09:14:29.451319 types-dj-database-url-1.3.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:14:29.451319 types-dj-database-url-1.3.0.2/dj_database_url-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 09:14:27.000000 types-dj-database-url-1.3.0.2/dj_database_url-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-28 09:14:27.000000 types-dj-database-url-1.3.0.2/dj_database_url-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:14:29.451319 types-dj-database-url-1.3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-28 09:14:27.000000 types-dj-database-url-1.3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:14:29.451319 types-dj-database-url-1.3.0.2/types_dj_database_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-28 09:14:29.000000 types-dj-database-url-1.3.0.2/types_dj_database_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-28 09:14:29.000000 types-dj-database-url-1.3.0.2/types_dj_database_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:14:29.000000 types-dj-database-url-1.3.0.2/types_dj_database_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 09:14:29.000000 types-dj-database-url-1.3.0.2/types_dj_database_url.egg-info/top_level.txt
```

### Comparing `types-dj-database-url-1.3.0.1/CHANGELOG.md` & `types-dj-database-url-1.3.0.2/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## 1.3.0.2 (2023-04-28)
+
+[stubsabot] Mark dj-database-url as obsolete since 2.0.0 (#10094)
+
+Release: https://pypi.org/pypi/dj-database-url/2.0.0
+Homepage: https://github.com/jazzband/dj-database-url
+Diff: https://github.com/jazzband/dj-database-url/compare/v1.3.0...v2.0.0
+
+Co-authored-by: stubsabot <>
+
 ## 1.3.0.1 (2023-04-24)
 
 [dj-database-url] Fix CONN_MAX_AGE and conn_max_age types (#10075)
 
 ## 1.3.0.0 (2023-03-30)
 
 Bump dj-database-url to 1.3.* (#9975)
```

### Comparing `types-dj-database-url-1.3.0.1/PKG-INFO` & `types-dj-database-url-1.3.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-dj-database-url
-Version: 1.3.0.1
+Version: 1.3.0.2
 Summary: Typing stubs for dj-database-url
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,14 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dj-database-url`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dj-database-url. All fixes for
 types and metadata should be contributed there.
 
+*Note:* The `dj-database-url` package includes type annotations or type stubs
+since version 2.0.0. Please uninstall the `types-dj-database-url`
+package if you use this or a newer version.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
+This package was generated from typeshed commit `dd7d2121c3c011c0c08843a54f56b1bc16b5f64e`.
```

### Comparing `types-dj-database-url-1.3.0.1/dj_database_url-stubs/__init__.pyi` & `types-dj-database-url-1.3.0.2/dj_database_url-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-dj-database-url-1.3.0.1/setup.py` & `types-dj-database-url-1.3.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,20 +11,25 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dj-database-url`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dj-database-url. All fixes for
 types and metadata should be contributed there.
 
+*Note:* The `dj-database-url` package includes type annotations or type stubs
+since version 2.0.0. Please uninstall the `types-dj-database-url`
+package if you use this or a newer version.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
+This package was generated from typeshed commit `dd7d2121c3c011c0c08843a54f56b1bc16b5f64e`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.3.0.1",
+      version="1.3.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md",
```

### Comparing `types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/PKG-INFO` & `types-dj-database-url-1.3.0.2/types_dj_database_url.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-dj-database-url
-Version: 1.3.0.1
+Version: 1.3.0.2
 Summary: Typing stubs for dj-database-url
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,14 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dj-database-url`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dj-database-url. All fixes for
 types and metadata should be contributed there.
 
+*Note:* The `dj-database-url` package includes type annotations or type stubs
+since version 2.0.0. Please uninstall the `types-dj-database-url`
+package if you use this or a newer version.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
+This package was generated from typeshed commit `dd7d2121c3c011c0c08843a54f56b1bc16b5f64e`.
```

