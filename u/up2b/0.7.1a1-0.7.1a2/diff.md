# Comparing `tmp/up2b-0.7.1a1.tar.gz` & `tmp/up2b-0.7.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up2b-0.7.1a1.tar", last modified: Thu Mar  9 15:08:55 2023, max compression
+gzip compressed data, was "up2b-0.7.1a2.tar", last modified: Fri Apr 28 12:05:25 2023, max compression
```

## Comparing `up2b-0.7.1a1.tar` & `up2b-0.7.1a2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.024381 up2b-0.7.1a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.016381 up2b-0.7.1a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.016381 up2b-0.7.1a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-09 15:08:41.000000 up2b-0.7.1a1/.github/workflows/check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-09 15:08:41.000000 up2b-0.7.1a1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-09 15:08:41.000000 up2b-0.7.1a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-09 15:08:41.000000 up2b-0.7.1a1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-09 15:08:41.000000 up2b-0.7.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-03-09 15:08:55.020381 up2b-0.7.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-03-09 15:08:41.000000 up2b-0.7.1a1/README.en_US.md
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-03-09 15:08:41.000000 up2b-0.7.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-09 15:08:41.000000 up2b-0.7.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-09 15:08:41.000000 up2b-0.7.1a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 15:08:55.024381 up2b-0.7.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.020381 up2b-0.7.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-09 15:08:41.000000 up2b-0.7.1a1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.020381 up2b-0.7.1a1/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28768 2023-03-09 15:08:41.000000 up2b-0.7.1a1/tests/images/1.png
--rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-03-09 15:08:41.000000 up2b-0.7.1a1/tests/images/2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-03-09 15:08:41.000000 up2b-0.7.1a1/tests/images/3.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-09 15:08:41.000000 up2b-0.7.1a1/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-09 15:08:41.000000 up2b-0.7.1a1/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-09 15:08:41.000000 up2b-0.7.1a1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-09 15:08:41.000000 up2b-0.7.1a1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.020381 up2b-0.7.1a1/up2b/
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.020381 up2b-0.7.1a1/up2b/up2b_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.020381 up2b-0.7.1a1/up2b/up2b_lib/up2b_api/
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/up2b_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/up2b_api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/up2b_api/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/up2b_api/imgtg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/up2b_api/imgtu.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/up2b_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/up2b_api/sm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-03-09 15:08:41.000000 up2b-0.7.1a1/up2b/up2b_lib/watermark.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-09 15:08:54.000000 up2b-0.7.1a1/up2b/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:08:55.020381 up2b-0.7.1a1/up2b.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-03-09 15:08:54.000000 up2b-0.7.1a1/up2b.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-09 15:08:55.000000 up2b-0.7.1a1/up2b.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:08:54.000000 up2b-0.7.1a1/up2b.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-09 15:08:54.000000 up2b-0.7.1a1/up2b.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-09 15:08:54.000000 up2b-0.7.1a1/up2b.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-09 15:08:54.000000 up2b-0.7.1a1/up2b.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.184493 up2b-0.7.1a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.168493 up2b-0.7.1a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.172493 up2b-0.7.1a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-28 12:05:13.000000 up2b-0.7.1a2/.github/workflows/check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 12:05:13.000000 up2b-0.7.1a2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-28 12:05:13.000000 up2b-0.7.1a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 12:05:13.000000 up2b-0.7.1a2/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-28 12:05:13.000000 up2b-0.7.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-28 12:05:25.184493 up2b-0.7.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-28 12:05:13.000000 up2b-0.7.1a2/README.en_US.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-28 12:05:13.000000 up2b-0.7.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-28 12:05:13.000000 up2b-0.7.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 12:05:13.000000 up2b-0.7.1a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:05:25.184493 up2b-0.7.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.172493 up2b-0.7.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.176493 up2b-0.7.1a2/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28768 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/images/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/images/2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/images/3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.176493 up2b-0.7.1a2/up2b/
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.180493 up2b-0.7.1a2/up2b/up2b_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.184493 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/imgtg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/imgtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/sm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.176493 up2b-0.7.1a2/up2b.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/top_level.txt
```

### Comparing `up2b-0.7.1a1/.github/workflows/check.yaml` & `up2b-0.7.1a2/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/.github/workflows/publish.yaml` & `up2b-0.7.1a2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/LICENSE` & `up2b-0.7.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/PKG-INFO` & `up2b-0.7.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up2b
-Version: 0.7.1a1
+Version: 0.7.1a2
 Summary: 上传图片到图床
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up2b Version: 0.7.1a1 Summary:
+Metadata-Version: 2.1 Name: up2b Version: 0.7.1a2 Summary:
 ä¸ä¼ å¾çå°å¾åº Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2021 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `up2b-0.7.1a1/README.en_US.md` & `up2b-0.7.1a2/README.en_US.md`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/README.md` & `up2b-0.7.1a2/README.md`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/pyproject.toml` & `up2b-0.7.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/tests/images/1.png` & `up2b-0.7.1a2/tests/images/1.png`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/tests/images/2.jpeg` & `up2b-0.7.1a2/tests/images/2.jpeg`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/tests/images/3.jpeg` & `up2b-0.7.1a2/tests/images/3.jpeg`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/tests/server.py` & `up2b-0.7.1a2/tests/server.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/tests/test_upload.py` & `up2b-0.7.1a2/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/tests/test_utils.py` & `up2b-0.7.1a2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/up2b/__init__.py` & `up2b-0.7.1a2/up2b/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   __init__.py
 # @Created At:  2021-02-08 15:43:32
-# @Modified At: 2023-03-06 21:07:49
+# @Modified At: 2023-04-19 14:45:15
 # @Modified By: thepoy
 
 import sys
 import json
 import click
 
 from typing import Any, Dict, Optional, Tuple, Type, Union
@@ -316,15 +316,15 @@
 
 
 def print_list() -> int:
     conf = read_conf()
     auth_data: Optional[AuthData] = conf.get("auth_data")  # type: ignore
 
     if not auth_data:
-        selected_code = conf.get("image_bed", -1)
+        selected_code = conf.get("image_bed")
         if selected_code is None:
             logger.fatal(
                 "no image bed selected, "
                 + "you need to use `--choose-site` or `-c` to select the image bed first."
             )
 
         assert isinstance(selected_code, int)
@@ -354,13 +354,12 @@
         else:
             print_item(chr(10007), ds.fc.red, i)
 
     return 0
 
 
 def run_main():
-    with logger:
-        sys.exit(cli())
+    sys.exit(cli())
 
 
 if __name__ == "__main__":
     run_main()
```

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/cache.py` & `up2b-0.7.1a2/up2b/up2b_lib/cache.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/constants.py` & `up2b-0.7.1a2/up2b/up2b_lib/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   constants.py
 # @Created At:  2021-02-13 09:17:07
-# @Modified At: 2023-03-01 20:10:33
+# @Modified At: 2023-04-19 14:42:31
 # @Modified By: thepoy
 
 import sys
 import os
 
 from enum import IntEnum
 from pathlib import Path
@@ -47,18 +47,19 @@
 
 IMAGE_BEDS_HELP_MESSAGE = "\n\n".join([f"{v}: {k}" for k, v in IMAGE_BEDS_CODE.items()])
 
 
 IS_WINDOWS = sys.platform == "win32"
 IS_MACOS = sys.platform == "darwin"
 
-if IS_WINDOWS:
-    CONFIG_FOLDER_PATH = Path(os.environ["APPDATA"]) / "up2b"
-else:
-    CONFIG_FOLDER_PATH = Path(os.environ["HOME"]) / ".config" / "up2b"
+CONFIG_FOLDER_PATH = (
+    Path(os.environ["APPDATA"]) / "up2b"
+    if IS_WINDOWS
+    else Path(os.environ["HOME"]) / ".config" / "up2b"
+)
 
 if not CONFIG_FOLDER_PATH.exists():
     os.makedirs(CONFIG_FOLDER_PATH / "conf", 0o755)
 
 CONF_FILE = CONFIG_FOLDER_PATH / "conf" / "conf.up2b.json"
 CACHE_PATH = Path(gettempdir()) / "up2b"
 CACHE_DATABASE = CONFIG_FOLDER_PATH / "cache.db"
```

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/custom_types.py` & `up2b-0.7.1a2/up2b/up2b_lib/custom_types.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/i18n.py` & `up2b-0.7.1a2/up2b/up2b_lib/i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   i18n.py
 # @Created At:  2022-01-09 11:17:23
-# @Modified At: 2023-02-27 22:47:19
+# @Modified At: 2023-04-19 14:43:52
 # @Modified By: thepoy
 
 import json
 import os
 
 from typing import Dict
 from up2b.up2b_lib.constants import CONFIG_FOLDER_PATH
@@ -63,23 +63,22 @@
         logger.debug("the language used: [ en_US ]")
 
         return _i18ns["en_US"]
 
     lang = get_default_language()
     locale = _i18ns.get(lang)
     if locale:
-        logger.debug("the language used: [ %s ]", lang)
+        logger.debug("the language used", language=lang)
         return locale
 
     translation_file = _i18n_folder / (lang + ".json")
     if not os.path.exists(translation_file):
         logger.info(
-            "the language used is [ %s ], but no translation file for [ %s ] was found, so use [ en_US ]",
-            lang,
-            lang,
+            "the language used is [ %s ], but no translation file for [ %s ] was found, so use [ en_US ]"
+            % (lang, lang)
         )
         return _i18ns["en_US"]
 
-    logger.debug("translation file [ %s ] will be used", translation_file)
+    logger.debug("translation file will be used", file=translation_file)
 
     with translation_file.open() as f:
         return json.loads(f.read())
```

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/log.py` & `up2b-0.7.1a2/up2b/up2b_lib/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   log.py
 # @Created At:  2023-02-07 12:13:41
-# @Modified At: 2023-02-21 12:40:41
+# @Modified At: 2023-04-03 20:55:06
 # @Modified By: thepoy
 
 from colorful_logger import get_logger, child_logger as cl
 from colorful_logger.logger import is_debug
 from up2b.up2b_lib.constants import CONFIG_FOLDER_PATH
 
 log_file_path = None
@@ -25,8 +25,9 @@
 
 logger = get_logger(
     "up2b",
     show=show,
     file_path=log_file_path,
     add_file_path=False,
     disable_line_number_filter=True,
+    asynchronous=False,
 )
```

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/up2b_api/__init__.py` & `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   __init__.py
 # @Created At:  2021-02-13 09:02:21
-# @Modified At: 2023-03-06 21:01:59
+# @Modified At: 2023-04-19 14:41:12
 # @Modified By: thepoy
 
 import os
 import time
 import json
 import shutil
 import requests
 
 from io import BytesIO
 from abc import ABC, abstractmethod
-from typing import Optional, List, Tuple, Dict, Union
+from typing import Callable, Optional, List, Tuple, Dict, Union
 from pathlib import Path
 from up2b.up2b_lib.cache import Cache
 from up2b.up2b_lib.constants import (
     CONF_FILE,
     CACHE_PATH,
     IMAGE_BEDS_NAME,
     PYTHON_VERSION,
@@ -311,15 +311,15 @@
 
             return (url, md5, ok)
 
         logger.debug("缓存中未找到此图片链接")
         return (url, md5, ok)
 
     def upload_images(
-        self, *images: Union[ImageType, DownloadErrorResponse], to_console=True
+        self, *images: Union[ImageType, DownloadErrorResponse], to_console: bool = True
     ) -> List[Union[str, DownloadErrorResponse, UploadErrorResponse]]:
         self.check_login()
 
         check_image_exists(images)
 
         self._check_images_valid(images)
 
@@ -370,15 +370,17 @@
             "token": token,
             "username": username,
             "repo": repo,
             "folder": folder,
         }
         self._save_auth_info(auth_info)
 
-    def _upload(self, image: ImageType, data: Dict[str, str], request_method="put"):
+    def _upload(
+        self, image: ImageType, data: Dict[str, str], request_method: str = "put"
+    ) -> Union[str, UploadErrorResponse]:
         self.check_login()
 
         url, md5, ok = self._check_cache(image)  # type: ignore
 
         if ok and not self.ignore_cache:
             return url
 
@@ -414,15 +416,15 @@
             return uploaded_url
         else:
             error = resp.json()["message"]
             logger.error("upload failed", image=image, error=error)
             return UploadErrorResponse(resp.status_code, error, str(image))
 
     def upload_images(
-        self, *images: Union[ImageType, DownloadErrorResponse], to_console=True
+        self, *images: Union[ImageType, DownloadErrorResponse], to_console: bool = True
     ) -> List[Union[str, DownloadErrorResponse, UploadErrorResponse]]:
         self.check_login()
 
         check_image_exists(images)
 
         self._check_images_valid(images)
 
@@ -454,19 +456,20 @@
         self.check_login()
 
         resp = self._get_all_images_in_image_bed()
         if resp.status_code != 200:
             return ErrorResponse(resp.status_code, resp.text)
 
         all_images_resp: List[Dict[str, str]] = resp.json()
-        images = []
+        images: List[GitGetAllImagesResponse] = []
         for file in all_images_resp:
             download_url = file["download_url"]
             if hasattr(self, "cdn_url") and callable(getattr(self, "cdn_url")):
-                download_url = self.cdn_url(file["download_url"])  # type: ignore
+                self.cdn_url: Callable[[str], str]
+                download_url: str = self.cdn_url(file["download_url"])
             images.append(
                 GitGetAllImagesResponse(
                     download_url,
                     file["sha"],
                     file["url"],
                 )
             )
```

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/up2b_api/__init__.pyi` & `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/__init__.pyi`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/up2b_api/github.py` & `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/github.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/up2b_api/imgtg.py` & `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/imgtg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   imgtg.py
 # @Created At:  2023-01-10 13:39:51
-# @Modified At: 2023-03-04 21:38:59
+# @Modified At: 2023-04-19 14:38:19
 # @Modified By: thepoy
 
 import os
 from pathlib import Path
 import re
 import time
 import json
 import mimetypes
 import requests
 
 from urllib import parse
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Set, Tuple, Union
 from up2b.up2b_lib.custom_types import (
     ErrorResponse,
     ImageBedType,
     ImageType,
     ImageStream,
     ImagePath,
     ImgtuResponse,
@@ -107,15 +107,15 @@
                 r'PF.obj.config.auth_token = "([a-f0-9]{40})"', resp.text
             )
             if not auth_token:
                 return None, None
             resp_set_cookie = resp.headers["Set-Cookie"].split("; ")[0]
             return auth_token.group(1), resp_set_cookie
         else:
-            logger.error("response error: status_code=%d", resp.status_code)
+            logger.error("response error", status_code=resp.status_code)
             return None, None
 
     @property
     def headers(self):
         assert self.cookie != None
 
         headers = self.__headers.copy()
@@ -137,15 +137,17 @@
         auth_token = auth_token.group(1)
         if not self.auth_info:
             self.auth_info = {}
 
         self.auth_info["token"] = self.token = auth_token
         self._save_auth_info(self.auth_info)
 
-    def __upload(self, image: ImageType, retries=0) -> Union[str, UploadErrorResponse]:
+    def __upload(
+        self, image: ImageType, retries: int = 0
+    ) -> Union[str, UploadErrorResponse]:
         self.check_login()
 
         url, md5, ok = self._check_cache(image)  # type: ignore
 
         if ok and not self.ignore_cache:
             return url
 
@@ -199,17 +201,17 @@
             json_resp = resp.json()
         except json.decoder.JSONDecodeError:
             return UploadErrorResponse(resp.status_code, resp.text, str(image))
 
         try:
             uploaded_url: str = json_resp["image"]["image"]["url"]
             logger.info(
-                "uploaded url: '%s' => '%s'",
-                image,
-                uploaded_url,
+                "uploaded url",
+                target=image,
+                url=uploaded_url,
             )
 
             self.cache.save(
                 md5,
                 IMAGE_BEDS_NAME[self.image_bed_code],
                 uploaded_url,
                 self.ignore_cache,
@@ -232,45 +234,45 @@
                 return self.__upload(image, retries + 1)
             else:
                 return UploadErrorResponse(
                     resp.status_code, resp.json()["error"]["message"], str(image)
                 )
 
     def upload_image(self, image_path: ImagePath) -> Union[str, UploadErrorResponse]:
-        logger.debug("uploading: %s", image_path)
+        logger.debug("uploading", image_path=image_path)
 
         image_path = self._add_watermark(image_path)
 
         if self.auto_compress:
             # 输入的是路径，返回的也必然是路径，忽略 pyright 的错误提示
             image_path = self._compress_image(image_path)  # type: ignore
 
         return self.__upload(image_path)
 
     def upload_image_stream(
         self, image: ImageStream
     ) -> Union[str, UploadErrorResponse]:
-        logger.debug("uploading: %s", image.filename)
+        logger.debug("uploading", filename=image.filename)
 
         if self.auto_compress:
             new_image = self._compress_image(image)
         else:
             new_image = image
 
         return self.__upload(new_image)
 
     def get_all_images(self) -> Union[List[ImgtuResponse], ErrorResponse]:
         self.check_login()
 
         url = self._url(self.username)
 
         # 集合去重
-        images = set()
+        images: Set[Tuple[str, ...]] = set()
 
-        def visit_next_page(url):
+        def visit_next_page(url: str):
             resp = requests.get(url, headers=self.__headers, timeout=self.timeout)
             resp.encoding = "utf-8"
 
             if resp.status_code != 200:
                 return ErrorResponse(resp.status_code, resp.text)
 
             # 只获取默认的公开相册里的图片
@@ -316,19 +318,19 @@
                     int(item[3]),
                     int(item[4]),
                 )
             )
 
         return result
 
-    def delete_image(self, img_id: str, retries=0):
-        logger.fatal("%s 不支持删除图片", self)
+    def delete_image(self, img_id: str, retries: int = 0):
+        logger.fatal("不支持删除图片", image_bed=self)
 
-    def delete_images(self, imgs_id: List[str], retries=0):
-        logger.fatal("%s 不支持删除图片", self)
+    def delete_images(self, imgs_id: List[str], retries: int = 0):
+        logger.fatal("不支持删除图片", image_bed=self)
 
     def _url(self, path: str) -> str:
         return self.base_url + path
 
     def __repr__(self):
         return "imgtg.com"
```

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/up2b_api/imgtu.py` & `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/imgtu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   imgtu.py
 # @Created At:  2021-02-13 09:04:37
-# @Modified At: 2023-03-04 21:38:13
+# @Modified At: 2023-04-19 14:48:44
 # @Modified By: thepoy
 
 import os
 from pathlib import Path
 import re
 import time
 import json
 import mimetypes
 import requests
 
 from urllib import parse
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Set, Tuple, Union
 from up2b.up2b_lib.custom_types import (
     ErrorResponse,
     ImageBedType,
     ImageType,
     ImageStream,
     ImagePath,
     ImgtuResponse,
@@ -107,15 +107,15 @@
                 r'PF.obj.config.auth_token = "([a-f0-9]{40})"', resp.text
             )
             if not auth_token:
                 return None, None
             resp_set_cookie = resp.headers["Set-Cookie"].split("; ")[0]
             return auth_token.group(1), resp_set_cookie
         else:
-            logger.error("response error: status_code=%d", resp.status_code)
+            logger.error("response error", status_code=resp.status_code)
             return None, None
 
     @property
     def headers(self):
         assert self.cookie != None
 
         headers = self.__headers.copy()
@@ -137,15 +137,17 @@
         auth_token = auth_token.group(1)
         if not self.auth_info:
             self.auth_info = {}
 
         self.auth_info["token"] = self.token = auth_token
         self._save_auth_info(self.auth_info)
 
-    def __upload(self, image: ImageType, retries=0) -> Union[str, UploadErrorResponse]:
+    def __upload(
+        self, image: ImageType, retries: int = 0
+    ) -> Union[str, UploadErrorResponse]:
         url, md5, ok = self._check_cache(image)  # type: ignore
 
         if ok and not self.ignore_cache:
             return url
 
         self.check_login()
 
@@ -199,17 +201,17 @@
             json_resp = resp.json()
         except json.decoder.JSONDecodeError:
             return UploadErrorResponse(resp.status_code, resp.text, str(image))
 
         try:
             uploaded_url: str = json_resp["image"]["image"]["url"]
             logger.info(
-                "uploaded url: '%s' => '%s'",
-                image,
-                uploaded_url,
+                "uploaded url",
+                target=image,
+                url=uploaded_url,
             )
 
             self.cache.save(
                 md5,
                 IMAGE_BEDS_NAME[self.image_bed_code],
                 uploaded_url,
                 self.ignore_cache,
@@ -219,47 +221,47 @@
         except KeyError:
             if json_resp["error"]["message"] == "请求被拒绝 (auth_token)":
                 if retries >= 3:
                     return UploadErrorResponse(
                         resp.status_code, resp.json()["error"]["message"], str(image)
                     )
 
-                logger.warn(
-                    "`auth_token` has expired, the program will try to update `auth_token` automatically, number of retries: %d",
-                    retries + 1,
+                logger.warning(
+                    "`auth_token` has expired, the program will try to update `auth_token` automatically, number of retries",
+                    retries=retries + 1,
                 )
                 self._update_auth_token()
 
                 return self.__upload(image, retries + 1)
             else:
                 return UploadErrorResponse(
                     resp.status_code, resp.json()["error"]["message"], str(image)
                 )
 
     def upload_image(self, image_path: ImagePath) -> Union[str, UploadErrorResponse]:
-        logger.debug("uploading: %s", image_path)
+        logger.debug("uploading", image_path=image_path)
 
         return self.__upload(image_path)
 
     def upload_image_stream(
         self, image: ImageStream
     ) -> Union[str, UploadErrorResponse]:
-        logger.debug("uploading: %s", image.filename)
+        logger.debug("uploading:", filename=image.filename)
 
         return self.__upload(image)
 
     def get_all_images(self) -> Union[List[ImgtuResponse], ErrorResponse]:
         self.check_login()
 
         url = self._url(self.username)
 
         # 集合去重
-        images = set()
+        images: Set[Tuple[str, ...]] = set()
 
-        def visit_next_page(url):
+        def visit_next_page(url: str):
             resp = requests.get(url, headers=self.__headers, timeout=self.timeout)
             resp.encoding = "utf-8"
 
             if resp.status_code != 200:
                 return ErrorResponse(resp.status_code, resp.text)
 
             # 只获取默认的公开相册里的图片
@@ -305,15 +307,15 @@
                     int(item[3]),
                     int(item[4]),
                 )
             )
 
         return result
 
-    def delete_image(self, img_id: str, retries=0) -> Optional[ErrorResponse]:
+    def delete_image(self, img_id: str, retries: int = 0) -> Optional[ErrorResponse]:
         self.check_login()
 
         url = self._url("json")
         data = {
             "auth_token": self.token,
             "action": "delete",
             "single": "true",
@@ -338,15 +340,17 @@
                 return self.delete_image(img_id, retries + 1)
 
         if resp.status_code == 200:
             return None
 
         return ErrorResponse(resp.status_code, resp.json()["error"]["message"])
 
-    def delete_images(self, imgs_id: List[str], retries=0) -> Dict[str, ErrorResponse]:
+    def delete_images(
+        self, imgs_id: List[str], retries: int = 0
+    ) -> Dict[str, ErrorResponse]:
         self.check_login()
 
         url = self._url("json")
         data = {
             "auth_token": self.token,
             "action": "delete",
             "from": "list",
@@ -359,16 +363,16 @@
         )
         json_resp = resp.json()
         if resp.status_code == 400:
             if json_resp["error"]["message"] == "请求被拒绝 (auth_token)":
                 if retries >= 3:
                     # 删除多张图片时如果重试3次仍无法成功响应则退出程序
                     logger.fatal(
-                        "authentication information is invalid: %s",
-                        resp.json()["error"]["message"],
+                        "authentication information is invalid",
+                        error=resp.json()["error"]["message"],
                     )
 
                 logger.warn(
                     "`auth_token` has expired, the program will try to update `auth_token` automatically, number of retries: %d",
                     retries + 1,
                 )
                 self._update_auth_token()
```

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/up2b_api/sm.py` & `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/sm.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/utils.py` & `up2b-0.7.1a2/up2b/up2b_lib/utils.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/up2b/up2b_lib/watermark.py` & `up2b-0.7.1a2/up2b/up2b_lib/watermark.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a1/up2b.egg-info/PKG-INFO` & `up2b-0.7.1a2/up2b.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up2b
-Version: 0.7.1a1
+Version: 0.7.1a2
 Summary: 上传图片到图床
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up2b Version: 0.7.1a1 Summary:
+Metadata-Version: 2.1 Name: up2b Version: 0.7.1a2 Summary:
 ä¸ä¼ å¾çå°å¾åº Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2021 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `up2b-0.7.1a1/up2b.egg-info/SOURCES.txt` & `up2b-0.7.1a2/up2b.egg-info/SOURCES.txt`

 * *Files identical despite different names*

