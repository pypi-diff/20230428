# Comparing `tmp/mypy-boto3-simspaceweaver-1.26.123.tar.gz` & `tmp/mypy-boto3-simspaceweaver-1.26.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-simspaceweaver-1.26.123.tar", last modified: Fri Apr 28 19:32:50 2023, max compression
+gzip compressed data, was "mypy-boto3-simspaceweaver-1.26.19.tar", last modified: Tue Nov 29 20:35:12 2022, max compression
```

## Comparing `mypy-boto3-simspaceweaver-1.26.123.tar` & `mypy-boto3-simspaceweaver-1.26.19.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:50.008092 mypy-boto3-simspaceweaver-1.26.123/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-04-28 19:32:50.008092 mypy-boto3-simspaceweaver-1.26.123/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:50.008092 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-28 19:32:25.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-28 19:32:25.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-04-28 19:32:25.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:50.008092 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-04-28 19:32:49.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-28 19:32:49.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:32:49.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:32:49.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 19:32:49.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 19:32:49.000000 mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:32:50.008092 mypy-boto3-simspaceweaver-1.26.123/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-28 19:32:24.000000 mypy-boto3-simspaceweaver-1.26.123/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.121234 mypy-boto3-simspaceweaver-1.26.19/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    13509 2022-11-29 20:35:12.121234 mypy-boto3-simspaceweaver-1.26.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12044 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.117234 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11206 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11185 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8118 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8116 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    10034 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10027 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.121234 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13509 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 20:35:12.121234 mypy-boto3-simspaceweaver-1.26.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/setup.py
```

### Comparing `mypy-boto3-simspaceweaver-1.26.123/LICENSE` & `mypy-boto3-simspaceweaver-1.26.19/LICENSE`

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

### Comparing `mypy-boto3-simspaceweaver-1.26.123/PKG-INFO` & `mypy-boto3-simspaceweaver-1.26.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-simspaceweaver
-Version: 1.26.123
-Summary: Type annotations for boto3.SimSpaceWeaver 1.26.123 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.19
+Summary: Type annotations for boto3.SimSpaceWeaver 1.26.19 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.26.123](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,15 +304,14 @@
 
 `mypy_boto3_simspaceweaver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
-    S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesTypeDef,
     ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
@@ -328,15 +326,14 @@
     StartClockInputRequestTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
-    CreateSnapshotInputRequestTypeDef,
     StartAppInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
@@ -355,42 +352,42 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.26.123/README.md` & `mypy-boto3-simspaceweaver-1.26.19/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.26.123](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,15 +273,14 @@
 
 `mypy_boto3_simspaceweaver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
-    S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesTypeDef,
     ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
@@ -296,15 +295,14 @@
     StartClockInputRequestTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
-    CreateSnapshotInputRequestTypeDef,
     StartAppInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
@@ -323,42 +321,42 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/client.py` & `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from .type_defs import (
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
     LaunchOverridesTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    S3DestinationTypeDef,
     S3LocationTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
 )
 
 __all__ = ("SimSpaceWeaverClient",)
 
@@ -81,24 +80,14 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#close)
         """
 
-    def create_snapshot(
-        self, *, Destination: S3DestinationTypeDef, Simulation: str
-    ) -> Dict[str, Any]:
-        """
-        Creates a snapshot of the specified simulation.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.create_snapshot)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#create_snapshot)
-        """
-
     def delete_app(self, *, App: str, Domain: str, Simulation: str) -> Dict[str, Any]:
         """
         Deletes the instance of the given custom app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.delete_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#delete_app)
         """
@@ -117,15 +106,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.describe_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#describe_app)
         """
 
     def describe_simulation(self, *, Simulation: str) -> DescribeSimulationOutputTypeDef:
         """
-        Returns the current state of the given simulation.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.describe_simulation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#describe_simulation)
         """
 
     def generate_presigned_url(
         self,
@@ -196,23 +185,22 @@
         """
 
     def start_simulation(
         self,
         *,
         Name: str,
         RoleArn: str,
+        SchemaS3Location: S3LocationTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
         MaximumDuration: str = ...,
-        SchemaS3Location: S3LocationTypeDef = ...,
-        SnapshotS3Location: S3LocationTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartSimulationOutputTypeDef:
         """
-        Starts a simulation with the given name.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_simulation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#start_simulation)
         """
 
     def stop_app(self, *, App: str, Domain: str, Simulation: str) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/client.pyi` & `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from .type_defs import (
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
     LaunchOverridesTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    S3DestinationTypeDef,
     S3LocationTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
 )
 
 __all__ = ("SimSpaceWeaverClient",)
 
@@ -75,23 +74,14 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#close)
         """
-    def create_snapshot(
-        self, *, Destination: S3DestinationTypeDef, Simulation: str
-    ) -> Dict[str, Any]:
-        """
-        Creates a snapshot of the specified simulation.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.create_snapshot)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#create_snapshot)
-        """
     def delete_app(self, *, App: str, Domain: str, Simulation: str) -> Dict[str, Any]:
         """
         Deletes the instance of the given custom app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.delete_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#delete_app)
         """
@@ -107,15 +97,15 @@
         Returns the state of the given custom app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.describe_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#describe_app)
         """
     def describe_simulation(self, *, Simulation: str) -> DescribeSimulationOutputTypeDef:
         """
-        Returns the current state of the given simulation.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.describe_simulation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#describe_simulation)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
@@ -179,23 +169,22 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#start_clock)
         """
     def start_simulation(
         self,
         *,
         Name: str,
         RoleArn: str,
+        SchemaS3Location: S3LocationTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
         MaximumDuration: str = ...,
-        SchemaS3Location: S3LocationTypeDef = ...,
-        SnapshotS3Location: S3LocationTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartSimulationOutputTypeDef:
         """
-        Starts a simulation with the given name.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_simulation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#start_simulation)
         """
     def stop_app(self, *, App: str, Domain: str, Simulation: str) -> Dict[str, Any]:
         """
         Stops the given custom app and shuts down all of its allocated compute
```

### Comparing `mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/literals.py` & `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,15 @@
 ClockTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 LifecycleManagementStrategyType = Literal[
     "ByRequest", "BySpatialSubdivision", "PerWorker", "Unknown"
 ]
 SimulationAppStatusType = Literal["ERROR", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"]
 SimulationAppTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 SimulationStatusType = Literal[
-    "DELETED",
-    "DELETING",
-    "FAILED",
-    "SNAPSHOT_IN_PROGRESS",
-    "STARTED",
-    "STARTING",
-    "STOPPED",
-    "STOPPING",
-    "UNKNOWN",
+    "DELETED", "DELETING", "FAILED", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
 ]
 SimulationTargetStatusType = Literal["DELETED", "STARTED", "STOPPED", "UNKNOWN"]
 SimSpaceWeaverServiceName = Literal["simspaceweaver"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -93,30 +85,27 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -145,15 +134,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -198,15 +186,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -217,38 +204,34 @@
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
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -287,26 +270,24 @@
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
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -334,16 +315,14 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -377,20 +356,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
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

### Comparing `mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/literals.pyi` & `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,15 @@
 ClockTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 LifecycleManagementStrategyType = Literal[
     "ByRequest", "BySpatialSubdivision", "PerWorker", "Unknown"
 ]
 SimulationAppStatusType = Literal["ERROR", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"]
 SimulationAppTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 SimulationStatusType = Literal[
-    "DELETED",
-    "DELETING",
-    "FAILED",
-    "SNAPSHOT_IN_PROGRESS",
-    "STARTED",
-    "STARTING",
-    "STOPPED",
-    "STOPPING",
-    "UNKNOWN",
+    "DELETED", "DELETING", "FAILED", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
 ]
 SimulationTargetStatusType = Literal["DELETED", "STARTED", "STOPPED", "UNKNOWN"]
 SimSpaceWeaverServiceName = Literal["simspaceweaver"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -91,30 +83,27 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -143,15 +132,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -196,15 +184,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -215,38 +202,34 @@
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
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -285,26 +268,24 @@
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
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -332,16 +313,14 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -375,20 +354,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
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

### Comparing `mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/type_defs.py` & `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,16 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
-    "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
     "LaunchOverridesTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
     "S3LocationTypeDef",
@@ -52,15 +50,14 @@
     "StartClockInputRequestTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
-    "CreateSnapshotInputRequestTypeDef",
     "StartAppInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "StartAppOutputTypeDef",
     "StartSimulationOutputTypeDef",
     "StartSimulationInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
@@ -75,23 +72,14 @@
     "CloudWatchLogsLogGroupTypeDef",
     {
         "LogGroupArn": str,
     },
     total=False,
 )
 
-S3DestinationTypeDef = TypedDict(
-    "S3DestinationTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKeyPrefix": str,
-    },
-    total=False,
-)
-
 DeleteAppInputRequestTypeDef = TypedDict(
     "DeleteAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -169,21 +157,19 @@
         "Domain": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAppsInputRequestTypeDef(
     _RequiredListAppsInputRequestTypeDef, _OptionalListAppsInputRequestTypeDef
 ):
     pass
 
-
 SimulationAppMetadataTypeDef = TypedDict(
     "SimulationAppMetadataTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
@@ -288,22 +274,14 @@
     "LogDestinationTypeDef",
     {
         "CloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
     total=False,
 )
 
-CreateSnapshotInputRequestTypeDef = TypedDict(
-    "CreateSnapshotInputRequestTypeDef",
-    {
-        "Destination": S3DestinationTypeDef,
-        "Simulation": str,
-    },
-)
-
 _RequiredStartAppInputRequestTypeDef = TypedDict(
     "_RequiredStartAppInputRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
     },
@@ -314,21 +292,19 @@
         "ClientToken": str,
         "Description": str,
         "LaunchOverrides": LaunchOverridesTypeDef,
     },
     total=False,
 )
 
-
 class StartAppInputRequestTypeDef(
     _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -354,36 +330,33 @@
 )
 
 _RequiredStartSimulationInputRequestTypeDef = TypedDict(
     "_RequiredStartSimulationInputRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
+        "SchemaS3Location": S3LocationTypeDef,
     },
 )
 _OptionalStartSimulationInputRequestTypeDef = TypedDict(
     "_OptionalStartSimulationInputRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
         "MaximumDuration": str,
-        "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartSimulationInputRequestTypeDef(
     _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
 ):
     pass
 
-
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -449,14 +422,12 @@
         "LiveSimulationState": LiveSimulationStateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaximumDuration": str,
         "Name": str,
         "RoleArn": str,
         "SchemaError": str,
         "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
-        "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver/type_defs.pyi` & `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
-    "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
     "LaunchOverridesTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
     "S3LocationTypeDef",
@@ -51,15 +51,14 @@
     "StartClockInputRequestTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
-    "CreateSnapshotInputRequestTypeDef",
     "StartAppInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "StartAppOutputTypeDef",
     "StartSimulationOutputTypeDef",
     "StartSimulationInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
@@ -74,23 +73,14 @@
     "CloudWatchLogsLogGroupTypeDef",
     {
         "LogGroupArn": str,
     },
     total=False,
 )
 
-S3DestinationTypeDef = TypedDict(
-    "S3DestinationTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKeyPrefix": str,
-    },
-    total=False,
-)
-
 DeleteAppInputRequestTypeDef = TypedDict(
     "DeleteAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -168,19 +158,21 @@
         "Domain": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAppsInputRequestTypeDef(
     _RequiredListAppsInputRequestTypeDef, _OptionalListAppsInputRequestTypeDef
 ):
     pass
 
+
 SimulationAppMetadataTypeDef = TypedDict(
     "SimulationAppMetadataTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
@@ -285,22 +277,14 @@
     "LogDestinationTypeDef",
     {
         "CloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
     total=False,
 )
 
-CreateSnapshotInputRequestTypeDef = TypedDict(
-    "CreateSnapshotInputRequestTypeDef",
-    {
-        "Destination": S3DestinationTypeDef,
-        "Simulation": str,
-    },
-)
-
 _RequiredStartAppInputRequestTypeDef = TypedDict(
     "_RequiredStartAppInputRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
     },
@@ -311,19 +295,21 @@
         "ClientToken": str,
         "Description": str,
         "LaunchOverrides": LaunchOverridesTypeDef,
     },
     total=False,
 )
 
+
 class StartAppInputRequestTypeDef(
     _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -349,34 +335,35 @@
 )
 
 _RequiredStartSimulationInputRequestTypeDef = TypedDict(
     "_RequiredStartSimulationInputRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
+        "SchemaS3Location": S3LocationTypeDef,
     },
 )
 _OptionalStartSimulationInputRequestTypeDef = TypedDict(
     "_OptionalStartSimulationInputRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
         "MaximumDuration": str,
-        "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartSimulationInputRequestTypeDef(
     _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
 ):
     pass
 
+
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -442,14 +429,12 @@
         "LiveSimulationState": LiveSimulationStateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaximumDuration": str,
         "Name": str,
         "RoleArn": str,
         "SchemaError": str,
         "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
-        "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/PKG-INFO` & `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-simspaceweaver
-Version: 1.26.123
-Summary: Type annotations for boto3.SimSpaceWeaver 1.26.123 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.19
+Summary: Type annotations for boto3.SimSpaceWeaver 1.26.19 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.26.123](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,15 +304,14 @@
 
 `mypy_boto3_simspaceweaver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
-    S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesTypeDef,
     ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
@@ -328,15 +326,14 @@
     StartClockInputRequestTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
-    CreateSnapshotInputRequestTypeDef,
     StartAppInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
@@ -355,42 +352,42 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.26.123/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt` & `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.26.123/setup.py` & `mypy-boto3-simspaceweaver-1.26.19/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 """
 Setup script for mypy-boto3-simspaceweaver.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-simspaceweaver",
-    version="1.26.123",
+    version="1.26.19",
     packages=["mypy_boto3_simspaceweaver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SimSpaceWeaver 1.26.123 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SimSpaceWeaver 1.26.19 service generated with"
+        " mypy-boto3-builder 7.11.11"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 simspaceweaver type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_simspaceweaver": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_simspaceweaver": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/",
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

