# Comparing `tmp/qiskit-qasm3-import-0.1.0.tar.gz` & `tmp/qiskit-qasm3-import-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-qasm3-import-0.1.0.tar", last modified: Thu Nov 10 01:40:08 2022, max compression
+gzip compressed data, was "qiskit-qasm3-import-0.2.0.tar", last modified: Fri Apr 28 15:19:54 2023, max compression
```

## Comparing `qiskit-qasm3-import-0.1.0.tar` & `qiskit-qasm3-import-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 01:40:08.065464 qiskit-qasm3-import-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11343 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6789 2022-11-10 01:40:08.065464 qiskit-qasm3-import-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6288 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-10 01:40:08.065464 qiskit-qasm3-import-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 01:40:08.061464 qiskit-qasm3-import-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 01:40:08.065464 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    24683 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/data.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    15997 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-11-10 01:39:52.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 01:40:08.065464 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6789 2022-11-10 01:40:08.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-11-10 01:40:08.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 01:40:08.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-10 01:40:08.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-10 01:40:08.000000 qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:54.515754 qiskit-qasm3-import-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-28 15:19:54.515754 qiskit-qasm3-import-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-28 15:19:54.515754 qiskit-qasm3-import-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:54.511754 qiskit-qasm3-import-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:54.515754 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:54.515754 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-28 15:19:54.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-28 15:19:54.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:19:54.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 15:19:54.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 15:19:54.000000 qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:54.515754 qiskit-qasm3-import-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/tests/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26639 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18480 2023-04-28 15:19:39.000000 qiskit-qasm3-import-0.2.0/tests/test_values.py
```

### Comparing `qiskit-qasm3-import-0.1.0/LICENSE` & `qiskit-qasm3-import-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022, Jake Lishman
+   Copyright 2022, Jake Lishman, IBM and Qiskit contributors
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `qiskit-qasm3-import-0.1.0/PKG-INFO` & `qiskit-qasm3-import-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: qiskit-qasm3-import
-Version: 0.1.0
+Version: 0.2.0
 Summary: Importer for parsing OpenQASM 3 strings into Qiskit circuits
-Home-page: https://github.com/jakelishman/qiskit-qasm3-import
+Home-page: https://github.com/Qiskit/qiskit-qasm3-import
 Author: Jake Lishman
 License: Apache 2.0 License
-Project-URL: Bug Tracker, https://github.com/jakelishman/qiskit-qasm3-import/issues
-Project-URL: Source Code, https://github.com/jakelishman/qiskit-qasm3-import
+Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-qasm3-import/issues
+Project-URL: Documentation, https://qiskit.github.io/qiskit-qasm3-import
+Project-URL: Source Code, https://github.com/Qiskit/qiskit-qasm3-import
 Description-Content-Type: text/markdown; variant=GFM
 Provides-Extra: all
 License-File: LICENSE
 
 # Importer from OpenQASM 3 to Qiskit
 
-[![License](https://img.shields.io/github/license/jakelishman/qiskit-qasm3-import.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/jakelishman/qiskit-qasm3-import.svg?style=popout-square)](https://github.com/jakelishman/qiskit-qasm3-import/releases)[![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm3-import.svg?style=popout-square)](https://pypi.org/project/qiskit-qasm3-import/)<!--- long-description-skip-end -->
+[![License](https://img.shields.io/github/license/Qiskit/qiskit-qasm3-import.svg?style=flat)](https://opensource.org/licenses/Apache-2.0)[![Release](https://img.shields.io/github/release/Qiskit/qiskit-qasm3-import.svg?style=flat)](https://github.com/Qiskit/qiskit-qasm3-import/releases)[![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm3-import.svg?style=flat)](https://pypi.org/project/qiskit-qasm3-import/)
 
 This repository provides the Python package `qiskit_qasm3_import`, which is a
 basic and temporary importer from OpenQASM 3 into Qiskit's `QuantumCircuit`.
 
-Qiskit itself does not yet have this functionality due to ongoing technical
-discussions about the future direction of various data structures within Terra.
-This project is a stop-gap measure until those issues can be resolved the
-correct way; Terra makes strong guarantees of stability and support in its
-interfaces, and we are not yet ready to make that commitment for this project.
+Qiskit itself accepts this package as an optional dependency if it is installed.
+In that case, Qiskit exposes the functions `qiskit.qasm3.load` and
+`qiskit.qasm3.loads`, which are wrappers around `qiskit_qasm3_import.parse`.
+This project is a stop-gap measure until various technical decisions can be
+resolved the correct way; Terra makes strong guarantees of stability and support
+in its interfaces, and we are not yet ready to make that commitment for this
+project, hence the minimal wrappers.
+
 
 ## Example
 
 The principal entry point to the package is the top-level `parse` function,
 which accepts a string containing a complete OpenQASM 3 programme.  This complex
 example shows a lot of the capabilities of the importer.
 
@@ -119,20 +123,26 @@
 ```
 
 
 ## Installation
 
 Install the latest release of the `qiskit_qasm3_import` package from pip:
 
-```bash
+```text
 pip install qiskit_qasm3_import
 ```
 
 This will automatically install all the dependencies as well (an OpenQASM 3
-parser, for example) if they are not already installed.
+parser, for example) if they are not already installed.  Alternatively, you can
+install Qiskit Terra directly with this package as an optional dependency by
+doing
+
+```text
+pip install qiskit-terra[qasm3-import]
+```
 
 
 ## Developing
 
 If you're looking to contribute to this project, please first read
 [our contributing guidelines](CONTRIBUTING.md).
 
@@ -141,15 +151,15 @@
 
 ```bash
 pip install -r requirements-dev.txt tox
 ```
 
 This installs a few more packages than the dependencies of the package at
 runtime, because there are some tools we use for testing also included, such as
-`tox` and `stestr`.
+`tox` and `pytest`.
 
 After the development requirements are installed, you can install an editable
 version of the package with
 
 ```bash
 pip install -e .
 ```
@@ -162,15 +172,17 @@
 
 After the development requirements have been installed, the command
 
 ```bash
 tox -e docs
 ```
 
-will build the HTML documentation, and place it in `docs/_build/html`.
+will build the HTML documentation, and place it in `docs/_build/html`.  The
+documentation state of the `main` branch of this repository is published to
+https://qiskit.github.io/qiskit-qasm3-import.
 
 
 ### Code style and linting
 
 The Python components of this repository are formatted using `black`.  You can
 run this on the required files by running
```

### Comparing `qiskit-qasm3-import-0.1.0/README.md` & `qiskit-qasm3-import-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Importer from OpenQASM 3 to Qiskit
 
-[![License](https://img.shields.io/github/license/jakelishman/qiskit-qasm3-import.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/jakelishman/qiskit-qasm3-import.svg?style=popout-square)](https://github.com/jakelishman/qiskit-qasm3-import/releases)[![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm3-import.svg?style=popout-square)](https://pypi.org/project/qiskit-qasm3-import/)<!--- long-description-skip-end -->
+[![License](https://img.shields.io/github/license/Qiskit/qiskit-qasm3-import.svg?style=flat)](https://opensource.org/licenses/Apache-2.0)[![Release](https://img.shields.io/github/release/Qiskit/qiskit-qasm3-import.svg?style=flat)](https://github.com/Qiskit/qiskit-qasm3-import/releases)[![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm3-import.svg?style=flat)](https://pypi.org/project/qiskit-qasm3-import/)
 
 This repository provides the Python package `qiskit_qasm3_import`, which is a
 basic and temporary importer from OpenQASM 3 into Qiskit's `QuantumCircuit`.
 
-Qiskit itself does not yet have this functionality due to ongoing technical
-discussions about the future direction of various data structures within Terra.
-This project is a stop-gap measure until those issues can be resolved the
-correct way; Terra makes strong guarantees of stability and support in its
-interfaces, and we are not yet ready to make that commitment for this project.
+Qiskit itself accepts this package as an optional dependency if it is installed.
+In that case, Qiskit exposes the functions `qiskit.qasm3.load` and
+`qiskit.qasm3.loads`, which are wrappers around `qiskit_qasm3_import.parse`.
+This project is a stop-gap measure until various technical decisions can be
+resolved the correct way; Terra makes strong guarantees of stability and support
+in its interfaces, and we are not yet ready to make that commitment for this
+project, hence the minimal wrappers.
+
 
 ## Example
 
 The principal entry point to the package is the top-level `parse` function,
 which accepts a string containing a complete OpenQASM 3 programme.  This complex
 example shows a lot of the capabilities of the importer.
 
@@ -106,20 +109,26 @@
 ```
 
 
 ## Installation
 
 Install the latest release of the `qiskit_qasm3_import` package from pip:
 
-```bash
+```text
 pip install qiskit_qasm3_import
 ```
 
 This will automatically install all the dependencies as well (an OpenQASM 3
-parser, for example) if they are not already installed.
+parser, for example) if they are not already installed.  Alternatively, you can
+install Qiskit Terra directly with this package as an optional dependency by
+doing
+
+```text
+pip install qiskit-terra[qasm3-import]
+```
 
 
 ## Developing
 
 If you're looking to contribute to this project, please first read
 [our contributing guidelines](CONTRIBUTING.md).
 
@@ -128,15 +137,15 @@
 
 ```bash
 pip install -r requirements-dev.txt tox
 ```
 
 This installs a few more packages than the dependencies of the package at
 runtime, because there are some tools we use for testing also included, such as
-`tox` and `stestr`.
+`tox` and `pytest`.
 
 After the development requirements are installed, you can install an editable
 version of the package with
 
 ```bash
 pip install -e .
 ```
@@ -149,15 +158,17 @@
 
 After the development requirements have been installed, the command
 
 ```bash
 tox -e docs
 ```
 
-will build the HTML documentation, and place it in `docs/_build/html`.
+will build the HTML documentation, and place it in `docs/_build/html`.  The
+documentation state of the `main` branch of this repository is published to
+https://qiskit.github.io/qiskit-qasm3-import.
 
 
 ### Code style and linting
 
 The Python components of this repository are formatted using `black`.  You can
 run this on the required files by running
```

### Comparing `qiskit-qasm3-import-0.1.0/pyproject.toml` & `qiskit-qasm3-import-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "redefined-builtin",
     "redefined-outer-name",
     "suppressed-message",
     "too-few-public-methods",
     "too-many-public-methods",
     "too-many-arguments",
     "too-many-instance-attributes",
+    "too-many-lines",
     "too-many-locals",
     "trailing-whitespace",
     "ungrouped-imports",
     "unknown-option-value",
     "unnecessary-semicolon",
     "unneeded-not",
     "unused-wildcard-import",
```

### Comparing `qiskit-qasm3-import-0.1.0/setup.cfg` & `qiskit-qasm3-import-0.2.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [metadata]
 name = qiskit-qasm3-import
 version = attr:qiskit_qasm3_import.__version__
-url = https://github.com/jakelishman/qiskit-qasm3-import
+url = https://github.com/Qiskit/qiskit-qasm3-import
 description = Importer for parsing OpenQASM 3 strings into Qiskit circuits
 long_description = file: README.md
 long_description_content_type = text/markdown; variant=GFM
 license = Apache 2.0 License
 license_files = LICENSE
 project_urls = 
-	Bug Tracker = https://github.com/jakelishman/qiskit-qasm3-import/issues
-	Source Code = https://github.com/jakelishman/qiskit-qasm3-import
+	Bug Tracker = https://github.com/Qiskit/qiskit-qasm3-import/issues
+	Documentation = https://qiskit.github.io/qiskit-qasm3-import
+	Source Code = https://github.com/Qiskit/qiskit-qasm3-import
 author = Jake Lishman
 
 [options]
 packages = find:
 package_dir = 
 	= src
 install_requires =
```

### Comparing `qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/api.py` & `qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 
 from .converter import ConvertVisitor
 
 
 def convert(node: openqasm3.ast.Program) -> QuantumCircuit:
     """Convert a parsed OpenQASM 3 program in AST form, into a Qiskit
     :class:`~qiskit.circuit.QuantumCircuit`."""
-    return ConvertVisitor().convert(node)
+    return ConvertVisitor().convert(node).circuit
 
 
 def parse(string: str, /) -> QuantumCircuit:
     """Wrapper around :func:`.convert`, which first parses the OpenQASM 3 program into AST form, and
     then converts the output to Qiskit format."""
     return convert(openqasm3.parse(string))
```

### Comparing `qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/converter.py` & `qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 __all__ = ["ConvertVisitor"]
 
-import itertools
-import math
 import re
 import string
 import sys
 
 if sys.version_info < (3, 9):
     from typing import Iterator, Sequence
 else:
@@ -21,21 +19,25 @@
     Parameter,
     ParameterExpression,
     QuantumCircuit,
     QuantumRegister,
     Qubit,
 )
 from qiskit.circuit.parametertable import ParameterReferences
+from qiskit.transpiler import Layout
+from qiskit.transpiler.layout import TranspileLayout
 from qiskit.circuit.library import standard_gates as _std
 
 from . import types
 from .data import Scope, Symbol
 from .exceptions import ConversionError, raise_from_node
 from .expression import ValueResolver, resolve_condition
+from .state import State, SymbolTables, LocalScope, GateScope, is_physical
 
+_QASM2_IDENTIFIER = re.compile(r"[a-z]\w*", flags=re.ASCII)
 
 _STDGATES = {
     "p": (_std.PhaseGate, 1, 1),
     "x": (_std.XGate, 0, 1),
     "y": (_std.YGate, 0, 1),
     "z": (_std.ZGate, 0, 1),
     "h": (_std.HGate, 0, 1),
@@ -68,109 +70,54 @@
         1,
     ),
     "u1": (_std.U1Gate, 1, 1),
     "u2": (_std.U2Gate, 2, 1),
     "u3": (_std.U3Gate, 3, 1),
 }
 
-_BUILTINS = {
-    "U": Symbol(
-        "U",
-        _std.UGate,
-        types.Gate([types.Angle() for _ in [None] * 3], [types.Qubit()]),
-        Scope.BUILTIN,
-    ),
-    "pi": Symbol("pi", math.pi, types.Float(const=True), Scope.BUILTIN),
-    "π": Symbol("π", math.pi, types.Float(const=True), Scope.BUILTIN),
-    "tau": Symbol("tau", math.tau, types.Float(const=True), Scope.BUILTIN),
-    "τ": Symbol("τ", math.tau, types.Float(const=True), Scope.BUILTIN),
-    "euler": Symbol("euler", math.e, types.Float(const=True), Scope.BUILTIN),
-    "ℇ": Symbol("ℇ", math.e, types.Float(const=True), Scope.BUILTIN),
-}
-
-
-class State:
-    __slots__ = ("scope", "source", "circuit", "symbol_table", "_unique")
-
-    def __init__(self, scope: Scope, source: Optional[str] = None):
-        self.scope = scope
-        self.source = source
-        self.circuit = QuantumCircuit()
-        self.symbol_table = _BUILTINS.copy()
-        self._unique = (f"_{x}" for x in itertools.count())
-
-    def gate_scope(self):
-        """Get a new state for entry to a "gate" scope."""
-        # We use the entire source, because at the moment, that's what all the error messages
-        # expect; the nodes have references to the complete source in their spans.
-        out = State(Scope.GATE, self.source)
-        for name, item in self.symbol_table.items():
-            if (item.scope is Scope.BUILTIN) or (
-                item.scope is Scope.GLOBAL
-                and (
-                    isinstance(item.type, types.Gate)
-                    or isinstance(
-                        item.type, (types.Int, types.Uint, types.Float, types.Angle, types.Duration)
-                    )
-                    and item.type.const
-                )
-            ):
-                out.symbol_table[name] = item
-        return out
-
-    def local_scope(self):
-        """Get a new state on entry to a local block scope."""
-        # pylint: disable=protected-access
-        out = State.__new__(State)
-        out.scope = Scope.LOCAL
-        out.source = self.source
-        out.circuit = self.circuit  # No copy; we want to keep modifying this one.
-        out.symbol_table = self.symbol_table.copy()
-        out._unique = self._unique
-        return out
-
-    def unique_name(self, prefix=""):
-        """Get a name that is not defined in the current scope."""
-        while (name := f"{prefix}{next(self._unique)}") in self.symbol_table:
-            pass
-        return name
-
-
-_QASM2_IDENTIFIER = re.compile(r"[a-z]\w*", flags=re.ASCII)
-
 
 def _escape_qasm2(name: str) -> str:
     """Escape a `name` to produce a valid OpenQASM 2 identifier (ignoring things like reserved
     keywords).  This is necessary for registers as of Terra 0.22 beacuse their names have an
     initialisation check that they match this regex.  It should be able to be removed once that
     restriction is lifted."""
     if _QASM2_IDENTIFIER.fullmatch(name):
         return name
     name = re.sub(r"\W", "_", name)
     if not name or name[0] not in string.ascii_lowercase:
         name = "esc_" + name
     return name
 
 
+# A hardware-qubit symbol has the form '$' followed by digits.
+# The digits are the identifier used by backends.
+def hardware_qubit_map(symbol_table: SymbolTables):
+    "Return a `dict` mapping `Qubit` instances to `int`s representing physical qubit identifiers."
+    return {sym.data: int(sym.name[1:]) for sym in symbol_table.globals() if is_physical(sym)}
+
+
 class GateBuilder:
     def __init__(
         self, name: str, definition: QuantumCircuit, order: Optional[Sequence[Parameter]] = None
     ):
-        self.name = name
-        self.definition = definition
-        self.order = tuple(self.definition.parameters) if order is None else tuple(order)
+        self._name = name
+        self._definition = definition
+        self._order = tuple(self._definition.parameters) if order is None else tuple(order)
 
     def __call__(self, *parameters):
-        if len(parameters) != len(self.order):
-            raise ConversionError("incorrect number of parameters in call")
-        out = Gate(self.name, self.definition.num_qubits, parameters)
+        if len(parameters) != len(self._order):
+            raise ConversionError(
+                "incorrect number of parameters in call. Expecting "
+                f" {len(self._order)}, got {len(parameters)}."
+            )
+        out = Gate(self._name, self._definition.num_qubits, parameters)
         if parameters:
-            out._definition = self.definition.assign_parameters(dict(zip(self.order, parameters)))
+            out._definition = self._definition.assign_parameters(dict(zip(self._order, parameters)))
         else:
-            out._definition = self.definition.copy()
+            out._definition = self._definition.copy()
         return out
 
 
 class ConvertVisitor(QASMVisitor[State]):
     """Internal visitor of an OpenQASM 3 AST to convert it to a
     :class:`~qiskit.circuit.QuantumCircuit`.  The complete conversion is done by calling
     :meth:`convert` on a :class:`openqasm3.ast.Program` node.
@@ -182,18 +129,28 @@
     # scope for this simple package to gracefully handle arbitrary semantically invalid programs.
     # In some places, such as symbol definitions, we do some simple checks to help everyone's
     # sanity, as the reference package doesn't yet do this.
 
     # pylint: disable=missing-function-docstring,no-self-use,unused-argument
 
     def convert(self, node: ast.Program, *, source: Optional[str] = None) -> QuantumCircuit:
-        """Convert a program node into a :class:`~qiskit.circuit.QuantumCircuit`.  If given,
-        `source` is a string containing the OpenQASM 3 source code that was parsed into `node`.
-        This is used to generated improved error messages."""
-        return self.visit(node, State(Scope.GLOBAL, source)).circuit
+        """Convert a program node into a :class:`~qiskit.circuit.QuantumCircuit`.
+
+        If given, `source` is a string containing the OpenQASM 3 source code that was parsed into
+        `node`.  This is used to generated improved error messages. A :class:`.State` containing
+        information about the conversion is returned. The :class:`~qiskit.circuit.QuantumCircuit` is
+        stored in property thereof named `circuit`.
+        """
+
+        state = self.visit(node, State(source))
+        hardware_qubits = hardware_qubit_map(state.symbol_table)
+        if len(hardware_qubits) > 0:
+            # pylint: disable=protected-access
+            state.circuit._layout = TranspileLayout(Layout(hardware_qubits), hardware_qubits)
+        return state
 
     def _raise_previously_defined(self, new: Symbol, old: Symbol, node: ast.QASMNode) -> NoReturn:
         message = f"'{new.name}' is already defined."
         if old.definer and (span := old.definer.span) is not None:
             message += f" Previous definition on line {span.start_line}."
         raise_from_node(node, message)
 
@@ -206,17 +163,17 @@
         definer: ast.QASMNode,
         context: State,
     ) -> State:
         if context.scope is not Scope.GLOBAL:
             raise_from_node(definer, "gates can only be declared globally")
         type = types.Gate(n_parameters, n_qubits)
         symbol = Symbol(name, definition, type, Scope.GLOBAL, definer)
-        if (previous := context.symbol_table.get(name)) is not None:
+        if (previous := context.symbol_table.get(name, definer)) is not None:
             self._raise_previously_defined(symbol, previous, definer)
-        context.symbol_table[name] = symbol
+        context.symbol_table.insert(symbol)
         return context
 
     def _apply_gate_modifier(
         self, modifier: ast.QuantumGateModifier, gate: Gate, context: State
     ) -> Gate:
         if modifier.modifier is ast.GateModifierName.inv:
             return gate.inverse()
@@ -261,15 +218,15 @@
 
         # pylint: disable=protected-access
         if parameter in context.circuit._parameter_table:
             return
         context.circuit._parameter_table[parameter] = ParameterReferences(())
 
     def _resolve_generic(self, node: ast.Expression, context: State) -> Tuple[Any, types.Type]:
-        return ValueResolver(context.symbol_table).resolve(node)
+        return ValueResolver(context).resolve(node)
 
     def _resolve_constant_int(self, node: ast.Expression, context: State) -> int:
         value, type = self._resolve_generic(node, context)
         if not isinstance(type, (types.Int, types.Uint)) or not type.const:
             raise_from_node(node, "required a constant integer")
         return value
 
@@ -301,27 +258,27 @@
             raise_from_node(node, "required a bit or bit register")
         return value
 
     def _resolve_qarg(
         self, node: ast.Expression, context: State
     ) -> Union[Qubit, QuantumRegister, List[Qubit]]:
         value, type = self._resolve_generic(node, context)
-        if not isinstance(type, (types.Qubit, types.QubitArray)):
+        if not isinstance(type, (types.Qubit, types.HardwareQubit, types.QubitArray)):
             raise_from_node(node, "required a qubit or qubit register")
         return value
 
     def _resolve_condition(
         self, node: ast.Expression, context: State
     ) -> Union[Tuple[ClassicalRegister, int], Tuple[Clbit, bool]]:
-        lhs, rhs = resolve_condition(node, context.symbol_table)
+        lhs, rhs = resolve_condition(node, context)
         if not isinstance(lhs, (Clbit, ClassicalRegister)):
             name = context.unique_name()
             lhs = ClassicalRegister(name=_escape_qasm2(name), bits=lhs)
             context.circuit.add_register(lhs)
-            context.symbol_table[name] = Symbol(name, lhs, types.BitArray, Scope.NONE)
+            context.symbol_table.insert(Symbol(name, lhs, types.BitArray, Scope.NONE))
         return (lhs, rhs)
 
     # Everything below is the implementation of the visitor itself.  The general `visit` method is
     # derived from the base class.
 
     def generic_visit(self, node, context=None):
         raise_from_node(node, f"node of type {node.__class__.__name__} is not supported")
@@ -335,58 +292,59 @@
         if node.filename != "stdgates.inc":
             raise_from_node(node, "non-stdgates imports not currently supported")
         for name, (builder, n_arguments, n_qubits) in _STDGATES.items():
             context = self._define_gate(name, builder, n_arguments, n_qubits, node, context)
         return context
 
     def visit_QubitDeclaration(self, node: ast.QubitDeclaration, context: State) -> State:
+        context.addressing_mode.set_virtual_mode(node)
         name = node.qubit.name
         if node.size is None:
             bit = Qubit()
             context.circuit.add_bits([bit])
             symbol = Symbol(name, bit, types.Qubit(), Scope.GLOBAL, node)
         else:
             size = self._resolve_constant_int(node.size, context)
             register = QuantumRegister(size, name=_escape_qasm2(name))
             context.circuit.add_register(register)
             symbol = Symbol(name, register, types.QubitArray(size), Scope.GLOBAL, node)
-        context.symbol_table[name] = symbol
+        context.symbol_table.insert(symbol)
         return context
 
     def visit_QuantumGateDefinition(self, node: ast.QuantumGateDefinition, context: State) -> State:
-        inner = context.gate_scope()
-        parameters = [Parameter(name.name) for name in node.arguments]
-        for parameter in parameters:
-            inner.symbol_table[parameter.name] = Symbol(
-                parameter.name, parameter, types.Angle(), Scope.GATE, node
-            )
-            self._add_circuit_parameter(parameter, inner)
-        bits = [Qubit() for _ in node.qubits]
-        inner.circuit.add_bits(bits)
-        for name, bit in zip(node.qubits, bits):
-            inner.symbol_table[name.name] = Symbol(name.name, bit, types.Qubit(), Scope.GATE, node)
-        for statement in node.body:
-            inner = self.visit(statement, inner)
+        with GateScope(context) as inner:
+            parameters = [Parameter(name.name) for name in node.arguments]
+            for parameter in parameters:
+                inner.symbol_table.insert(
+                    Symbol(parameter.name, parameter, types.Angle(), Scope.GATE, node)
+                )
+                self._add_circuit_parameter(parameter, inner)
+            bits = [Qubit() for _ in node.qubits]
+            inner.circuit.add_bits(bits)
+            for name, bit in zip(node.qubits, bits):
+                inner.symbol_table.insert(Symbol(name.name, bit, types.Qubit(), Scope.GATE, node))
+            for statement in node.body:
+                self.visit(statement, inner)
         return self._define_gate(
             node.name.name,
             GateBuilder(node.name.name, inner.circuit),
             len(parameters),
             len(bits),
             node,
             context,
         )
 
     def visit_QuantumGate(self, node: ast.QuantumGate, context: State) -> State:
         if node.duration is not None:
             raise_from_node(node, "gates with durations are not supported.")
-        if (gate_symbol := context.symbol_table.get(node.name.name)) is None:
+        if (gate_symbol := context.symbol_table.get(node.name.name, node)) is None:
             raise_from_node(node, f"gate '{node.name.name}' is not defined.")
         if not isinstance(gate_symbol.type, types.Gate):
             message = f"'{node.name.name}' is a '{gate_symbol.type.pretty()}', not a gate."
-            if (span := getattr(gate_symbol.definer, "span", None)) is not None:
+            if (span := gate_symbol.definer.span) is not None:
                 message += f" Definition on line {span.start_line}"
             raise_from_node(node, message)
         gate_builder = gate_symbol.data
         arguments = [self._resolve_angle(argument, context) for argument in node.arguments]
         gate = gate_builder(*arguments)
         for modifier in reversed(node.modifiers):
             gate = self._apply_gate_modifier(modifier, gate, context)
@@ -443,15 +401,15 @@
             context.circuit.add_bits([bit])
             symbol = Symbol(name, bit, types.Bit(), context.scope, node)
         else:
             size = self._resolve_constant_int(node.type.size, context)
             register = ClassicalRegister(size, name=_escape_qasm2(name))
             context.circuit.add_register(register)
             symbol = Symbol(name, register, types.BitArray(size), context.scope, node)
-        context.symbol_table[name] = symbol
+        context.symbol_table.insert(symbol)
         if node.init_expression is not None:
             if not isinstance(node.init_expression, ast.QuantumMeasurement):
                 raise_from_node(
                     node.init_expression, "initialisation of classical bits is not supported"
                 )
             measured = self._resolve_qarg(node.init_expression.qubit, context)
             target = symbol.data
@@ -476,46 +434,46 @@
             )
             type = types.Angle(size=size)
         else:
             raise_from_node(node, "only 'float' and 'angle' inputs are supported")
         name = node.identifier.name
         parameter = Parameter(name)
         symbol = Symbol(name, parameter, type, Scope.GLOBAL, node)
-        context.symbol_table[name] = symbol
+        context.symbol_table.insert(symbol)
         self._add_circuit_parameter(parameter, context)
         return context
 
     def visit_BreakStatement(self, node: ast.BreakStatement, context: State) -> State:
         context.circuit.break_loop()
         return context
 
     def visit_ContinueStatement(self, node: ast.ContinueStatement, context: State) -> State:
         context.circuit.continue_loop()
         return context
 
     def visit_BranchingStatement(self, node: ast.BranchingStatement, context: State) -> State:
         condition = self._resolve_condition(node.condition, context)
         with context.circuit.if_test(condition) as else_:
-            inner = context.local_scope()
-            for statement in node.if_block:
-                inner = self.visit(statement, inner)
+            with LocalScope(context) as inner:
+                for statement in node.if_block:
+                    self.visit(statement, inner)
         if not node.else_block:
             return context
         with else_:
-            inner = context.local_scope()
-            for statement in node.else_block:
-                inner = self.visit(statement, inner)
+            with LocalScope(context) as inner:
+                for statement in node.else_block:
+                    self.visit(statement, inner)
         return context
 
     def visit_WhileLoop(self, node: ast.WhileLoop, context: State) -> State:
         condition = self._resolve_condition(node.while_condition, context)
         with context.circuit.while_loop(condition):
-            inner = context.local_scope()
-            for statement in node.block:
-                inner = self.visit(statement, inner)
+            with LocalScope(context) as inner:
+                for statement in node.block:
+                    self.visit(statement, inner)
         return context
 
     def visit_ForInLoop(self, node: ast.ForInLoop, context: State) -> State:
         if not isinstance(node.type, (ast.IntType, ast.UintType)):
             raise_from_node(node, "only integer loop variables are supported")
         indexset, indextype = self._resolve_generic(node.set_declaration, context)
         if not isinstance(indextype, (types.Range, types.Sequence)):
@@ -529,21 +487,21 @@
             indexset = (
                 range(indexset.start, indexset.stop)
                 if indexset.step is None
                 else range(indexset.start, indexset.stop, indexset.step)
             )
         var_type = types.Int() if isinstance(node.type, ast.IntType) else types.Uint()
         with context.circuit.for_loop(indexset) as parameter:
-            inner = context.local_scope()
-            name = node.identifier.name
-            symbol = Symbol(name, parameter, var_type, Scope.LOCAL, node)
-            inner.symbol_table[name] = symbol
-            self._add_circuit_parameter(parameter, inner)
-            for statement in node.block:
-                inner = self.visit(statement, inner)
+            with LocalScope(context) as inner:
+                name = node.identifier.name
+                symbol = Symbol(name, parameter, var_type, Scope.LOCAL, node)
+                inner.symbol_table.insert(symbol)
+                self._add_circuit_parameter(parameter, inner)
+                for statement in node.block:
+                    self.visit(statement, inner)
         return context
 
     def visit_DelayInstruction(self, node: ast.DelayInstruction, context: State) -> State:
         duration, unit = self._resolve_constant_duration(node.duration, context)
         if not node.qubits:
             context.circuit.delay(duration, unit=unit)
             return context
@@ -563,9 +521,9 @@
             register = QuantumRegister(name=inner_name, bits=bits)
         else:
             raise_from_node(
                 node.value,
                 f"aliases must be of registers of either clbits or qubits, not '{type.pretty()}'",
             )
         context.circuit.add_register(register)
-        context.symbol_table[name] = Symbol(name, register, type, context.scope, node)
+        context.symbol_table.insert(Symbol(name, register, type, context.scope, node))
         return context
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/data.py` & `qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class Scope(enum.Enum):
     """Types of scope in OpenQASM 3 programs."""
 
     GLOBAL = enum.auto()
     GATE = enum.auto()
     FUNCTION = enum.auto()
     LOCAL = enum.auto()
-    CALIBRATION = enum.auto()
+    CALIBRATION = enum.auto()  # Unused
     BUILTIN = enum.auto()
     # NONE scope is for when we're adding an implicit symbol to the table, but it shouldn't actually
     # be accessible by anything outside the context that defines it.  We might need to do this in
     # order to reserve a name that's being defined in the output circuit, but isn't present in the
     # OQ3 program.
     NONE = enum.auto()
 
@@ -35,7 +35,10 @@
         definer: Optional[ast.QASMNode] = None,
     ):
         self.name = name
         self.data = data
         self.type = type
         self.scope = scope
         self.definer = definer
+
+    def __repr__(self):
+        return f"Symbol(name={self.name}, data={self.data}, type={self.type}, scope={self.scope})"
```

### Comparing `qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/exceptions.py` & `qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from typing import NoReturn
+from typing import NoReturn, Optional
 
 from openqasm3 import ast
 
 
 class ConversionError(Exception):
     """Raised when an error occurs converting from the AST representation into a
     :class:`~qiskit.circuit.QuantumCircuit`.  This is often due to OpenQASM 3 constructs that have
     no equivalent in Qiskit."""
 
+    def __init__(self, message, node: Optional[ast.QASMNode] = None):
+        if node is not None and node.span is not None:
+            message = f"{node.span.start_line},{node.span.start_column}: {message}"
+        self.message = message
+        super().__init__(message)
+
 
 def raise_from_node(node: ast.QASMNode, message: str) -> NoReturn:
     """Raise a :exc:`.ConversionError` caused by the given `node`."""
-    if node.span is not None:
-        message = f"{node.span.start_line},{node.span.start_column}: {message}"
-    raise ConversionError(message)
+    raise ConversionError(message, node)
```

### Comparing `qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/expression.py` & `qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/expression.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 
 # The binary operator rules are just complicated.  Early return is probably the easiest.
 # pylint: disable=too-many-return-statements,too-many-branches
 
 
 __all__ = ["ValueResolver", "resolve_condition"]
 
-from typing import Any, Iterable, Mapping, Tuple, Union
+from typing import Any, Iterable, Tuple, Union, cast
 
 from openqasm3 import ast
 from openqasm3.visitor import QASMVisitor
-from qiskit.circuit import Clbit
+from qiskit.circuit import Clbit, Qubit
 
 from . import types
 from .exceptions import raise_from_node
-from .data import Symbol
+from .data import Symbol, Scope
+from . import state
 
 
 _IntegerT = Union[types.Never, types.Int, types.Uint]
+_NumericT = Union[types.Uint, types.Int, types.Float]
 
 
 def join_integer_types(left: _IntegerT, right: _IntegerT) -> _IntegerT:
     if isinstance(left, types.Never):
         return right
     if isinstance(right, types.Never):
         return left
@@ -43,48 +45,70 @@
     const = left.const and right.const
     size = None if left.size is None or right.size is None else max((left.size, right.size))
     if isinstance(left, types.Uint) and isinstance(right, types.Uint):
         return types.Uint(const, size)
     return types.Int(const, size)
 
 
+def join_numeric_types(left: _NumericT, right: _NumericT) -> _NumericT:
+    const = left.const and right.const
+    if isinstance(left, types.Float) and isinstance(right, types.Float):
+        size = None if left.size is None or right.size is None else max((left.size, right.size))
+        return types.Float(const, size)
+    if isinstance(left, types.Float):
+        return types.Float(const, left.size)
+    if isinstance(right, types.Float):
+        return types.Float(const, right.size)
+    # Cast because this can't return the never type since neither of the inputs are never.
+    return cast(_NumericT, join_integer_types(left, right))
+
+
 class ValueResolver(QASMVisitor):
     """A resolver for value-like objects that have exact Qiskit representations.  Everything handled
     here should resolve into a single Qiskit object (or occasionally a compound of such objects,
     like lists of bits).
 
-    These resolvers are intended to be short-lived.  Their instance state is the symbols that are
-    available to them.  There is no per-run state tracked."""
+    These resolvers are intended to be short-lived. Their instance state is the instance of
+    :class:`.State` created in :meth:`.ConvertVisitor.convert()`.
+    """
 
-    __slots__ = ("symbols",)
+    __slots__ = ("_context",)
 
     # pylint: disable=no-self-use
 
-    def __init__(self, symbols: Mapping[str, Symbol]):
-        self.symbols = symbols
+    def __init__(self, context: state.State):
+        self._context = context
 
     def resolve(self, node: ast.Expression) -> Tuple[Any, types.Type]:
         """The entry point to the resolver, resolving the AST node into a 2-tuple of a relevant
         Qiskit type, and the :class:`.Type` that it is an instance of."""
+
         return self.visit(node)
 
     def visit(self, node: ast.QASMNode, context: None = None) -> Tuple[Any, types.Type]:
-        value, type = super().visit(node, context)
+        value, type = super().visit(node)
         if isinstance(type, types.Error):
             raise_from_node(node, "type error")
         return value, type
 
     def generic_visit(self, node: ast.QASMNode, context: None = None):
         raise_from_node(node, f"'{node.__class__.__name__}' cannot be resolved into a Qiskit value")
 
     def visit_Identifier(self, node: ast.Identifier):
-        name = node.name
-        if name not in self.symbols:
-            raise_from_node(node, f"name '{name}' is not defined in this scope")
-        symbol = self.symbols[name]
+        cxt = self._context
+        if (symbol := cxt.symbol_table.get(node.name, node)) is not None:
+            return symbol.data, symbol.type
+        if not state.is_physical(node.name):
+            raise_from_node(node, f"Undefined symbol '{node.name}'.")
+
+        cxt.addressing_mode.set_physical_mode(node)
+        bit = Qubit()
+        cxt.circuit.add_bits([bit])
+        symbol = Symbol(node.name, bit, types.HardwareQubit(), Scope.GLOBAL, node)
+        cxt.symbol_table.insert(symbol)
         return symbol.data, symbol.type
 
     def visit_IntegerLiteral(self, node: ast.IntegerLiteral):
         return node.value, types.Int(const=True)
 
     def visit_FloatLiteral(self, node: ast.FloatLiteral):
         return node.value, types.Float(const=True)
@@ -158,89 +182,67 @@
         raise_from_node(node, f"unhandled unary operator '{node.op.name}'")
 
     def visit_BinaryExpression(self, node: ast.BinaryExpression):
         if node.op.name not in ("+", "-", "*", "/"):
             raise_from_node(node, f"unsupported binary operation '{node.op.name}'")
         lhs_value, lhs_type = self.visit(node.lhs)
         rhs_value, rhs_type = self.visit(node.rhs)
+        out_type: Union[None, types.Type] = None
+
+        # First, handle the simple implicit promotion rules for the standard numeric types (i.e. not
+        # angle).
+        numeric_t = (types.Int, types.Uint, types.Float)
+        if isinstance(lhs_type, numeric_t) and isinstance(rhs_type, numeric_t):
+            out_type = join_numeric_types(lhs_type, rhs_type)
 
         if node.op.name in ("+", "-"):
-            if isinstance(lhs_type, (types.Int, types.Uint)) and isinstance(
-                rhs_type, (types.Int, types.Uint)
-            ):
-                out_type = join_integer_types(lhs_type, rhs_type)
-                out_value = (
-                    lhs_value + rhs_value
-                    if node.op is ast.BinaryOperator["+"]
-                    else lhs_value - rhs_value
-                )
-                return out_value, out_type
-            if isinstance(lhs_type, (types.Float, types.Angle)) and type(lhs_type) == type(
-                rhs_type
-            ):
+            if isinstance(lhs_type, types.Angle) and isinstance(rhs_type, types.Angle):
                 const = lhs_type.const and rhs_type.const
                 size = (
                     None
                     if lhs_type.size is None or rhs_type.size is None
                     else max((lhs_type.size, rhs_type.size))
                 )
+                out_type = types.Angle(const, size)
+            if out_type is not None:
                 out_value = (
                     lhs_value + rhs_value
                     if node.op is ast.BinaryOperator["+"]
                     else lhs_value - rhs_value
                 )
-                return out_value, type(lhs_type)(const, size)
+                return out_value, out_type
 
         elif node.op is ast.BinaryOperator["/"]:
-            if isinstance(rhs_type, (types.Int, types.Uint)):
-                if isinstance(lhs_type, (types.Int, types.Uint)):
-                    return lhs_value // rhs_value, join_integer_types(lhs_type, rhs_type)
-                if isinstance(lhs_type, types.Float):
-                    const = lhs_type.const and rhs_type.const
-                    return lhs_value / rhs_value, types.Float(const, lhs_type.size)
-                if isinstance(lhs_type, types.Angle):
-                    const = lhs_type.const and rhs_type.const
-                    return lhs_value / rhs_value, types.Angle(const, lhs_type.size)
-            elif isinstance(lhs_type, types.Angle):
-                if isinstance(rhs_type, types.Angle):
+            if isinstance(lhs_type, types.Angle):
+                if isinstance(rhs_type, (types.Int, types.Uint)):
                     const = lhs_type.const and rhs_type.const
-                    if const:
-                        return int(lhs_value / rhs_value), types.Uint(const=const)
-                    return lhs_value / rhs_value, types.Uint(const=const)
-                # Already handled integer rhs.
-            elif isinstance(lhs_type, types.Float):
-                if isinstance(rhs_type, types.Float):
+                    out_type = types.Angle(const, lhs_type.size)
+                elif isinstance(rhs_type, types.Angle):
                     const = lhs_type.const and rhs_type.const
-                    size = (
-                        None
-                        if lhs_type.size is None or rhs_type.size is None
-                        else max((lhs_type.size, rhs_type.size))
-                    )
-                    return lhs_value / rhs_value, types.Float(const, size)
+                    out_type = types.Uint(const, None)
+            if out_type is not None:
+                out_value = (
+                    lhs_value // rhs_value
+                    if isinstance(out_type, (types.Int, types.Uint)) and out_type.const
+                    else lhs_value / rhs_value
+                )
+                return out_value, out_type
 
         elif node.op is ast.BinaryOperator["*"]:
-            if isinstance(rhs_type, (types.Int, types.Uint)):
-                if isinstance(lhs_type, (types.Int, types.Uint)):
-                    return lhs_value * rhs_value, join_integer_types(lhs_type, rhs_type)
-                if isinstance(lhs_type, types.Float):
-                    const = lhs_type.const and rhs_type.const
-                    return lhs_value * rhs_value, types.Float(const, lhs_type.size)
-                if isinstance(lhs_type, types.Angle):
-                    const = lhs_type.const and rhs_type.const
-                    return lhs_value * rhs_value, types.Angle(const, lhs_type.size)
-            elif isinstance(lhs_type, types.Float):
-                # Already handled integer rhs.
-                if isinstance(rhs_type, types.Float):
-                    const = lhs_type.const and rhs_type.const
-                    size = (
-                        None
-                        if lhs_type.size is None or rhs_type.size is None
-                        else max((lhs_type.size, rhs_type.size))
-                    )
-                    return lhs_value * rhs_value, types.Float(const, size)
+            if (
+                isinstance(lhs_type, types.Angle) and isinstance(rhs_type, (types.Int, types.Uint))
+            ) or (
+                isinstance(rhs_type, types.Angle) and isinstance(lhs_type, (types.Int, types.Uint))
+            ):
+                const = lhs_type.const and rhs_type.const
+                size = lhs_type.size if isinstance(lhs_type, types.Angle) else rhs_type.size
+                out_type = types.Angle(const, size)
+            if out_type is not None:
+                out_value = lhs_value * rhs_value
+                return out_value, out_type
 
         return None, types.Error()
 
     def _index_collection(
         self,
         collection: Any,
         collection_type: types.Type,
@@ -250,15 +252,14 @@
         if not isinstance(collection_type, (types.BitArray, types.QubitArray)):
             raise_from_node(
                 base,
                 f"only indexing (qu)bit arrays is supported, not '{collection_type.pretty()}'",
             )
         if isinstance(indexer, ast.DiscreteSet):
             set_values, set_type = self.visit(indexer)
-            assert isinstance(set_type, types.Sequence)
             if not set_values:
                 return [], type(collection_type)(0)
             if not (isinstance(set_type.base, (types.Int, types.Uint)) and set_type.base.const):
                 raise_from_node(
                     indexer, f"only const (u)int can be indices, not '{set_type.pretty()}'"
                 )
             return [collection[x] for x in set_values], type(collection_type)(len(set_values))
@@ -282,23 +283,23 @@
             collection, collection_type = self._index_collection(
                 collection, collection_type, index, node
             )
         return collection, collection_type
 
 
 def resolve_condition(
-    node: ast.Expression, symbols: Mapping[str, Symbol]
+    node: ast.Expression, context: state.State
 ) -> Union[Tuple[Clbit, bool], Tuple[Iterable[Clbit], int]]:
     """A resolver for conditions that can be converted into Qiskit's very basic equality form
     of either ``Clbit == bool`` or ``ClassicalRegister == int``.
 
     This effectively just handles very special outer cases, then delegates the rest of the work to a
     :class:`.ValueResolver`."""
 
-    value_resolver = ValueResolver(symbols)
+    value_resolver = ValueResolver(context)
 
     if isinstance(node, ast.BinaryExpression):
         if node.op not in (ast.BinaryOperator["=="], ast.BinaryOperator["!="]):
             raise_from_node(node, f"unhandled binary operator '{node.op.name}'")
         lhs_value, lhs_type = value_resolver.visit(node.lhs)
         rhs_value, rhs_type = value_resolver.visit(node.rhs)
         bad_type_message = (
```

### Comparing `qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import/types.py` & `qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,25 @@
     __slots__ = ()
 
     def pretty(self):
         return "qubit"
 
 
 @typing.final
+class HardwareQubit(Type):
+    """A hardware qubit.
+    This corresponds a hardware qubits referenced in Terra's :class:`~qiskit.transpiler.TranspilerLayout`."""
+
+    __slots__ = ()
+
+    def pretty(self):
+        return "hardware qubit"
+
+
+@typing.final
 class Int(Type):
     """An integer value.  This is generally only encountered as a constant and so is represented by
     a Python integer, but can also be the type of the Qiskit :class:`~qiskit.circuit.Parameter` used
     to represent ``for``-loop variables."""
 
     __slots__ = ("size", "const")
```

### Comparing `qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import.egg-info/PKG-INFO` & `qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: qiskit-qasm3-import
-Version: 0.1.0
+Version: 0.2.0
 Summary: Importer for parsing OpenQASM 3 strings into Qiskit circuits
-Home-page: https://github.com/jakelishman/qiskit-qasm3-import
+Home-page: https://github.com/Qiskit/qiskit-qasm3-import
 Author: Jake Lishman
 License: Apache 2.0 License
-Project-URL: Bug Tracker, https://github.com/jakelishman/qiskit-qasm3-import/issues
-Project-URL: Source Code, https://github.com/jakelishman/qiskit-qasm3-import
+Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-qasm3-import/issues
+Project-URL: Documentation, https://qiskit.github.io/qiskit-qasm3-import
+Project-URL: Source Code, https://github.com/Qiskit/qiskit-qasm3-import
 Description-Content-Type: text/markdown; variant=GFM
 Provides-Extra: all
 License-File: LICENSE
 
 # Importer from OpenQASM 3 to Qiskit
 
-[![License](https://img.shields.io/github/license/jakelishman/qiskit-qasm3-import.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/jakelishman/qiskit-qasm3-import.svg?style=popout-square)](https://github.com/jakelishman/qiskit-qasm3-import/releases)[![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm3-import.svg?style=popout-square)](https://pypi.org/project/qiskit-qasm3-import/)<!--- long-description-skip-end -->
+[![License](https://img.shields.io/github/license/Qiskit/qiskit-qasm3-import.svg?style=flat)](https://opensource.org/licenses/Apache-2.0)[![Release](https://img.shields.io/github/release/Qiskit/qiskit-qasm3-import.svg?style=flat)](https://github.com/Qiskit/qiskit-qasm3-import/releases)[![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm3-import.svg?style=flat)](https://pypi.org/project/qiskit-qasm3-import/)
 
 This repository provides the Python package `qiskit_qasm3_import`, which is a
 basic and temporary importer from OpenQASM 3 into Qiskit's `QuantumCircuit`.
 
-Qiskit itself does not yet have this functionality due to ongoing technical
-discussions about the future direction of various data structures within Terra.
-This project is a stop-gap measure until those issues can be resolved the
-correct way; Terra makes strong guarantees of stability and support in its
-interfaces, and we are not yet ready to make that commitment for this project.
+Qiskit itself accepts this package as an optional dependency if it is installed.
+In that case, Qiskit exposes the functions `qiskit.qasm3.load` and
+`qiskit.qasm3.loads`, which are wrappers around `qiskit_qasm3_import.parse`.
+This project is a stop-gap measure until various technical decisions can be
+resolved the correct way; Terra makes strong guarantees of stability and support
+in its interfaces, and we are not yet ready to make that commitment for this
+project, hence the minimal wrappers.
+
 
 ## Example
 
 The principal entry point to the package is the top-level `parse` function,
 which accepts a string containing a complete OpenQASM 3 programme.  This complex
 example shows a lot of the capabilities of the importer.
 
@@ -119,20 +123,26 @@
 ```
 
 
 ## Installation
 
 Install the latest release of the `qiskit_qasm3_import` package from pip:
 
-```bash
+```text
 pip install qiskit_qasm3_import
 ```
 
 This will automatically install all the dependencies as well (an OpenQASM 3
-parser, for example) if they are not already installed.
+parser, for example) if they are not already installed.  Alternatively, you can
+install Qiskit Terra directly with this package as an optional dependency by
+doing
+
+```text
+pip install qiskit-terra[qasm3-import]
+```
 
 
 ## Developing
 
 If you're looking to contribute to this project, please first read
 [our contributing guidelines](CONTRIBUTING.md).
 
@@ -141,15 +151,15 @@
 
 ```bash
 pip install -r requirements-dev.txt tox
 ```
 
 This installs a few more packages than the dependencies of the package at
 runtime, because there are some tools we use for testing also included, such as
-`tox` and `stestr`.
+`tox` and `pytest`.
 
 After the development requirements are installed, you can install an editable
 version of the package with
 
 ```bash
 pip install -e .
 ```
@@ -162,15 +172,17 @@
 
 After the development requirements have been installed, the command
 
 ```bash
 tox -e docs
 ```
 
-will build the HTML documentation, and place it in `docs/_build/html`.
+will build the HTML documentation, and place it in `docs/_build/html`.  The
+documentation state of the `main` branch of this repository is published to
+https://qiskit.github.io/qiskit-qasm3-import.
 
 
 ### Code style and linting
 
 The Python components of this repository are formatted using `black`.  You can
 run this on the required files by running
```

### Comparing `qiskit-qasm3-import-0.1.0/src/qiskit_qasm3_import.egg-info/SOURCES.txt` & `qiskit-qasm3-import-0.2.0/src/qiskit_qasm3_import.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,13 +4,17 @@
 setup.cfg
 src/qiskit_qasm3_import/__init__.py
 src/qiskit_qasm3_import/api.py
 src/qiskit_qasm3_import/converter.py
 src/qiskit_qasm3_import/data.py
 src/qiskit_qasm3_import/exceptions.py
 src/qiskit_qasm3_import/expression.py
+src/qiskit_qasm3_import/state.py
 src/qiskit_qasm3_import/types.py
 src/qiskit_qasm3_import.egg-info/PKG-INFO
 src/qiskit_qasm3_import.egg-info/SOURCES.txt
 src/qiskit_qasm3_import.egg-info/dependency_links.txt
 src/qiskit_qasm3_import.egg-info/requires.txt
-src/qiskit_qasm3_import.egg-info/top_level.txt
+src/qiskit_qasm3_import.egg-info/top_level.txt
+tests/test_conditions.py
+tests/test_convert.py
+tests/test_values.py
```

