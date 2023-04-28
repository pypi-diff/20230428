# Comparing `tmp/sql2mermaid_cli-1.0.0.tar.gz` & `tmp/sql2mermaid_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql2mermaid_cli-1.0.0.tar", max compression
+gzip compressed data, was "sql2mermaid_cli-1.0.1.tar", max compression
```

## Comparing `sql2mermaid_cli-1.0.0.tar` & `sql2mermaid_cli-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1060 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     2180 2023-04-28 03:44:59.384120 sql2mermaid_cli-1.0.0/README.md
--rw-r--r--   0        0        0     1391 2023-04-28 05:27:40.342235 sql2mermaid_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.0/sql2mermaid_cli/__init__.py
--rw-r--r--   0        0        0     3872 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.0/sql2mermaid_cli/analyze.py
--rw-r--r--   0        0        0      496 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.0/sql2mermaid_cli/dependencies.py
--rw-r--r--   0        0        0      769 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.0/sql2mermaid_cli/file.py
--rw-r--r--   0        0        0     1081 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.0/sql2mermaid_cli/main.py
--rw-r--r--   0        0        0     1269 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.0/sql2mermaid_cli/mermaid.py
--rw-r--r--   0        0        0      597 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.0/sql2mermaid_cli/tables.py
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 sql2mermaid_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     2404 2023-04-28 05:50:55.412236 sql2mermaid_cli-1.0.1/README.md
+-rw-r--r--   0        0        0     1391 2023-04-28 05:51:04.362236 sql2mermaid_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.1/sql2mermaid_cli/__init__.py
+-rw-r--r--   0        0        0     3872 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.1/sql2mermaid_cli/analyze.py
+-rw-r--r--   0        0        0      496 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.1/sql2mermaid_cli/dependencies.py
+-rw-r--r--   0        0        0      769 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.1/sql2mermaid_cli/file.py
+-rw-r--r--   0        0        0     1081 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.1/sql2mermaid_cli/main.py
+-rw-r--r--   0        0        0     1269 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.1/sql2mermaid_cli/mermaid.py
+-rw-r--r--   0        0        0      597 2023-04-26 14:46:23.595988 sql2mermaid_cli-1.0.1/sql2mermaid_cli/tables.py
+-rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 sql2mermaid_cli-1.0.1/PKG-INFO
```

### Comparing `sql2mermaid_cli-1.0.0/LICENSE.md` & `sql2mermaid_cli-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sql2mermaid_cli-1.0.0/README.md` & `sql2mermaid_cli-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/nkato/sql2mermaid/python-tox.yml?event=push&label=pytest%20with%20py38)
 ![PyPI](https://img.shields.io/pypi/v/sql2mermaid)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sql2mermaid)
 
 ## sql2mermaid-cli
 `sql2mermaid-cli` is a CLI tool that converts SQL query into [mermaid.js](https://mermaid.js.org/) style!.
 
+![output-image](https://user-images.githubusercontent.com/20574756/235055268-3ecf0ec7-a3b7-45c3-93d9-fb032b14b4f6.gif)
+
 ## Required
 
 Python >=3.8.1
 
 ## Installation
 
 To install sql2mermaid-cli, use the following command:
 
 ```bash
-$ pip install git+https://github.com/sattosan/sql2mermaid-cli.git
+$ pip install sql2mermaid-cli
 ```
 
 ## Getting Started
 
 As a preparation, create a sample SQL file.
 
 ```bash
@@ -49,14 +51,19 @@
 foo[(foo)]
 
 bar --> baz
 root --> foo
 root --> bar
 ```
 
+The Mermaid diagram that is outputted can be visualized on the Mermaid Live Editor website.
+
+[Mermaid Live Editor](https://mermaid.live/)
+
+
 ## Options
 
 To save the output to a file, use the -o option followed by the path to the output file:
 
 ```bash
 $ sql2mermaid-cli -i input.sql -o output.txt
 ```
```

### Comparing `sql2mermaid_cli-1.0.0/pyproject.toml` & `sql2mermaid_cli-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql2mermaid-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = "CLI tool for converting SQL table dependencies to mermaid.js format."
 authors = ["sattosan <sato.yuya1211@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/sattosan/sql2mermaid-cli"
 
 [tool.poetry.scripts]
```

### Comparing `sql2mermaid_cli-1.0.0/sql2mermaid_cli/analyze.py` & `sql2mermaid_cli-1.0.1/sql2mermaid_cli/analyze.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid_cli-1.0.0/sql2mermaid_cli/file.py` & `sql2mermaid_cli-1.0.1/sql2mermaid_cli/file.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid_cli-1.0.0/sql2mermaid_cli/main.py` & `sql2mermaid_cli-1.0.1/sql2mermaid_cli/main.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid_cli-1.0.0/sql2mermaid_cli/mermaid.py` & `sql2mermaid_cli-1.0.1/sql2mermaid_cli/mermaid.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid_cli-1.0.0/sql2mermaid_cli/tables.py` & `sql2mermaid_cli-1.0.1/sql2mermaid_cli/tables.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid_cli-1.0.0/PKG-INFO` & `sql2mermaid_cli-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql2mermaid-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI tool for converting SQL table dependencies to mermaid.js format.
 Home-page: https://github.com/sattosan/sql2mermaid-cli
 License: MIT
 Author: sattosan
 Author-email: sato.yuya1211@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,24 +25,26 @@
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/nkato/sql2mermaid/python-tox.yml?event=push&label=pytest%20with%20py38)
 ![PyPI](https://img.shields.io/pypi/v/sql2mermaid)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sql2mermaid)
 
 ## sql2mermaid-cli
 `sql2mermaid-cli` is a CLI tool that converts SQL query into [mermaid.js](https://mermaid.js.org/) style!.
 
+![output-image](https://user-images.githubusercontent.com/20574756/235055268-3ecf0ec7-a3b7-45c3-93d9-fb032b14b4f6.gif)
+
 ## Required
 
 Python >=3.8.1
 
 ## Installation
 
 To install sql2mermaid-cli, use the following command:
 
 ```bash
-$ pip install git+https://github.com/sattosan/sql2mermaid-cli.git
+$ pip install sql2mermaid-cli
 ```
 
 ## Getting Started
 
 As a preparation, create a sample SQL file.
 
 ```bash
@@ -68,14 +70,19 @@
 foo[(foo)]
 
 bar --> baz
 root --> foo
 root --> bar
 ```
 
+The Mermaid diagram that is outputted can be visualized on the Mermaid Live Editor website.
+
+[Mermaid Live Editor](https://mermaid.live/)
+
+
 ## Options
 
 To save the output to a file, use the -o option followed by the path to the output file:
 
 ```bash
 $ sql2mermaid-cli -i input.sql -o output.txt
 ```
```

