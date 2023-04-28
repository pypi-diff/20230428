# Comparing `tmp/mypy-boto3-directconnect-1.26.123.tar.gz` & `tmp/mypy-boto3-directconnect-1.26.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-directconnect-1.26.123.tar", last modified: Fri Apr 28 19:32:47 2023, max compression
+gzip compressed data, was "mypy-boto3-directconnect-1.26.91.tar", last modified: Tue Mar 14 19:48:00 2023, max compression
```

## Comparing `mypy-boto3-directconnect-1.26.123.tar` & `mypy-boto3-directconnect-1.26.91.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:47.884019 mypy-boto3-directconnect-1.26.123/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-04-28 19:32:47.884019 mypy-boto3-directconnect-1.26.123/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:47.860018 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47262 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54933 2023-04-28 19:32:02.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54886 2023-04-28 19:32:02.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:47.860018 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-04-28 19:32:47.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 19:32:47.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:32:47.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:32:47.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 19:32:47.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 19:32:47.000000 mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:32:47.884019 mypy-boto3-directconnect-1.26.123/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-28 19:32:01.000000 mypy-boto3-directconnect-1.26.123/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20297 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18786 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47262 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54933 2023-03-14 19:46:57.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54886 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20297 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/setup.py
```

### Comparing `mypy-boto3-directconnect-1.26.123/LICENSE` & `mypy-boto3-directconnect-1.26.91/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-directconnect-1.26.123/PKG-INFO` & `mypy-boto3-directconnect-1.26.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-directconnect
-Version: 1.26.123
-Summary: Type annotations for boto3.DirectConnect 1.26.123 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.91
+Summary: Type annotations for boto3.DirectConnect 1.26.91 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.26.123](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -500,42 +500,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-directconnect-1.26.123/README.md` & `mypy-boto3-directconnect-1.26.91/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.26.123](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -468,42 +468,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/__init__.py` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/__init__.pyi` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/__main__.py` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DirectConnect 1.26.123\nVersion:         1.26.123\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.DirectConnect 1.26.91\nVersion:         1.26.91\nBuilder"
+        " version: 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.123")
+    print("1.26.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/client.py` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/client.pyi` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/literals.py` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -332,15 +331,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -427,15 +425,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/literals.pyi` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -330,15 +329,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -425,15 +423,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/paginator.py` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/paginator.pyi` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/type_defs.py` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect/type_defs.pyi` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/PKG-INFO` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-directconnect
-Version: 1.26.123
-Summary: Type annotations for boto3.DirectConnect 1.26.123 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.91
+Summary: Type annotations for boto3.DirectConnect 1.26.91 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.26.123](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -500,42 +500,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-directconnect-1.26.123/mypy_boto3_directconnect.egg-info/SOURCES.txt` & `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.123/setup.py` & `mypy-boto3-directconnect-1.26.91/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-directconnect.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-directconnect",
-    version="1.26.123",
+    version="1.26.91",
     packages=["mypy_boto3_directconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DirectConnect 1.26.123 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.DirectConnect 1.26.91 service generated with mypy-boto3-builder"
+        " 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

