# Comparing `tmp/fasta_reader-3.0.0.tar.gz` & `tmp/fasta_reader-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasta_reader-3.0.0.tar", max compression
+gzip compressed data, was "fasta_reader-3.0.1.tar", max compression
```

## Comparing `fasta_reader-3.0.0.tar` & `fasta_reader-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1069 2022-08-26 07:28:18.000000 fasta_reader-3.0.0/LICENSE
--rw-r--r--   0        0        0      919 2023-03-02 06:06:57.377717 fasta_reader-3.0.0/README.md
--rw-r--r--   0        0        0      235 2023-03-02 05:01:40.883341 fasta_reader-3.0.0/fasta_reader/__init__.py
--rw-r--r--   0        0        0      360 2023-03-02 06:01:38.689544 fasta_reader-3.0.0/fasta_reader/anyfile.py
--rw-r--r--   0        0        0      522 2023-03-01 15:01:24.738199 fasta_reader-3.0.0/fasta_reader/errors.py
--rw-r--r--   0        0        0     1678 2023-03-01 16:41:41.139392 fasta_reader-3.0.0/fasta_reader/item.py
--rw-r--r--   0        0        0      660 2023-03-02 06:06:06.846887 fasta_reader-3.0.0/fasta_reader/read_fasta.py
--rw-r--r--   0        0        0     2044 2023-03-02 05:43:43.812105 fasta_reader-3.0.0/fasta_reader/reader.py
--rw-r--r--   0        0        0       81 2023-03-02 04:49:20.007071 fasta_reader-3.0.0/fasta_reader/uri.py
--rw-r--r--   0        0        0      679 2023-03-02 06:06:20.890334 fasta_reader-3.0.0/fasta_reader/write_fasta.py
--rw-r--r--   0        0        0      987 2023-03-02 06:03:24.398973 fasta_reader-3.0.0/fasta_reader/writer.py
--rw-r--r--   0        0        0      670 2023-03-02 06:04:36.411886 fasta_reader-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 fasta_reader-3.0.0/setup.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 fasta_reader-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-08-26 07:28:18.000000 fasta_reader-3.0.1/LICENSE
+-rw-r--r--   0        0        0      919 2023-03-02 06:06:57.377717 fasta_reader-3.0.1/README.md
+-rw-r--r--   0        0        0      235 2023-03-02 05:01:40.883341 fasta_reader-3.0.1/fasta_reader/__init__.py
+-rw-r--r--   0        0        0      360 2023-03-02 06:01:38.689544 fasta_reader-3.0.1/fasta_reader/anyfile.py
+-rw-r--r--   0        0        0      522 2023-03-01 15:01:24.738199 fasta_reader-3.0.1/fasta_reader/errors.py
+-rw-r--r--   0        0        0     1678 2023-03-01 16:41:41.139392 fasta_reader-3.0.1/fasta_reader/item.py
+-rw-r--r--   0        0        0      660 2023-03-02 06:06:06.846887 fasta_reader-3.0.1/fasta_reader/read_fasta.py
+-rw-r--r--   0        0        0     2044 2023-03-02 05:43:43.812105 fasta_reader-3.0.1/fasta_reader/reader.py
+-rw-r--r--   0        0        0       81 2023-03-02 04:49:20.007071 fasta_reader-3.0.1/fasta_reader/uri.py
+-rw-r--r--   0        0        0      679 2023-03-02 06:06:20.890334 fasta_reader-3.0.1/fasta_reader/write_fasta.py
+-rw-r--r--   0        0        0      987 2023-03-02 06:03:24.398973 fasta_reader-3.0.1/fasta_reader/writer.py
+-rw-r--r--   0        0        0      654 2023-04-28 15:34:57.438526 fasta_reader-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 fasta_reader-3.0.1/PKG-INFO
```

### Comparing `fasta_reader-3.0.0/LICENSE` & `fasta_reader-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.0/README.md` & `fasta_reader-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.0/fasta_reader/errors.py` & `fasta_reader-3.0.1/fasta_reader/errors.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.0/fasta_reader/item.py` & `fasta_reader-3.0.1/fasta_reader/item.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.0/fasta_reader/read_fasta.py` & `fasta_reader-3.0.1/fasta_reader/read_fasta.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.0/fasta_reader/reader.py` & `fasta_reader-3.0.1/fasta_reader/reader.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.0/fasta_reader/write_fasta.py` & `fasta_reader-3.0.1/fasta_reader/write_fasta.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.0/fasta_reader/writer.py` & `fasta_reader-3.0.1/fasta_reader/writer.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.0/pyproject.toml` & `fasta_reader-3.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "fasta-reader"
-version = "3.0.0"
+version = "3.0.1"
 description = "FASTA file reader/writer."
 authors = ["Danilo Horta <fdanilo.horta@pm.me>"]
 repository = "https://github.com/EBI-Metagenomics/fasta-reader"
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "fasta_reader" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 more-itertools = ">=9.1.0"
 xopen = ">=1.7.0"
-fsspec = { version = ">=2023.1.0", extras = ["http", "sftp", "s3", "github"] }
+fsspec = { version = ">=2023.1.0", extras = ["http", "sftp"] }
 
 [tool.poetry.group.dev.dependencies]
 deptry = ">=0.6.4"
 pre-commit = ">=2.20.0"
 pytest = ">=7.2.0"
 pytest-datafiles = ">=3.0.0"
```

### Comparing `fasta_reader-3.0.0/PKG-INFO` & `fasta_reader-3.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fasta-reader
-Version: 3.0.0
+Version: 3.0.1
 Summary: FASTA file reader/writer.
 Home-page: https://github.com/EBI-Metagenomics/fasta-reader
 License: MIT
 Author: Danilo Horta
 Author-email: fdanilo.horta@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fsspec[github,http,s3,sftp] (>=2023.1.0)
+Requires-Dist: fsspec[http,sftp] (>=2023.1.0)
 Requires-Dist: more-itertools (>=9.1.0)
 Requires-Dist: xopen (>=1.7.0)
 Project-URL: Repository, https://github.com/EBI-Metagenomics/fasta-reader
 Description-Content-Type: text/markdown
 
 # Welcome to fasta-reader 👋
```

