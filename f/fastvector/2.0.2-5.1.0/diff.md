# Comparing `tmp/fastvector-2.0.2.tar.gz` & `tmp/fastvector-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastvector-2.0.2.tar", last modified: Fri May 20 10:39:14 2022, max compression
+gzip compressed data, was "fastvector-5.1.0.tar", last modified: Fri Apr 28 09:43:59 2023, max compression
```

## Comparing `fastvector-2.0.2.tar` & `fastvector-5.1.0.tar`

### file list

```diff
@@ -1,21 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 10:39:14.073656 fastvector-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-05-20 10:38:53.000000 fastvector-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-05-20 10:39:14.073656 fastvector-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-05-20 10:38:53.000000 fastvector-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 10:39:14.073656 fastvector-2.0.2/fastvector/
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-05-20 10:38:53.000000 fastvector-2.0.2/fastvector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-05-20 10:38:53.000000 fastvector-2.0.2/fastvector/computations.py
--rw-r--r--   0 runner    (1001) docker     (121)  1050893 2022-05-20 10:39:13.000000 fastvector-2.0.2/fastvector/cython_computations.c
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-05-20 10:38:53.000000 fastvector-2.0.2/fastvector/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5464 2022-05-20 10:38:53.000000 fastvector-2.0.2/fastvector/vector.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-20 10:38:53.000000 fastvector-2.0.2/fastvector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 10:39:14.073656 fastvector-2.0.2/fastvector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-05-20 10:39:13.000000 fastvector-2.0.2/fastvector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-05-20 10:39:14.000000 fastvector-2.0.2/fastvector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 10:39:13.000000 fastvector-2.0.2/fastvector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 10:39:13.000000 fastvector-2.0.2/fastvector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-20 10:39:13.000000 fastvector-2.0.2/fastvector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-20 10:39:13.000000 fastvector-2.0.2/fastvector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-05-20 10:38:53.000000 fastvector-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-05-20 10:39:14.077656 fastvector-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-05-20 10:38:53.000000 fastvector-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:43:59.255129 fastvector-5.1.0/
+-rw-rw-rw-   0        0        0      288 2023-04-25 14:43:44.000000 fastvector-5.1.0/.editorconfig
+-rw-rw-rw-   0        0        0      145 2023-04-24 16:21:27.000000 fastvector-5.1.0/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-04-28 09:43:59.193131 fastvector-5.1.0/.github/
+drwxrwxrwx   0        0        0        0 2023-04-28 09:43:59.217126 fastvector-5.1.0/.github/workflows/
+-rw-rw-rw-   0        0        0      548 2022-08-26 06:02:06.000000 fastvector-5.1.0/.github/workflows/codeql-analysis.yml
+-rw-rw-rw-   0        0        0      397 2022-08-26 06:02:06.000000 fastvector-5.1.0/.github/workflows/documentation.yml
+-rw-rw-rw-   0        0        0      241 2022-08-26 06:02:06.000000 fastvector-5.1.0/.github/workflows/pre-commit.yml
+-rw-rw-rw-   0        0        0      707 2023-04-28 09:27:16.000000 fastvector-5.1.0/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0     1401 2022-08-26 06:02:06.000000 fastvector-5.1.0/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     1772 2023-04-24 16:32:47.000000 fastvector-5.1.0/.gitignore
+-rw-rw-rw-   0        0        0      868 2023-04-24 16:32:47.000000 fastvector-5.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1059 2022-08-26 06:02:06.000000 fastvector-5.1.0/LICENSE
+-rw-rw-rw-   0        0        0      842 2023-04-28 09:43:59.254132 fastvector-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2220 2023-04-28 09:38:10.000000 fastvector-5.1.0/README.md
+-rw-rw-rw-   0        0        0       96 2022-08-26 06:02:06.000000 fastvector-5.1.0/codecov.yml
+drwxrwxrwx   0        0        0        0 2023-04-28 09:43:59.220135 fastvector-5.1.0/docs/
+-rw-rw-rw-   0        0        0       53 2022-08-26 06:02:06.000000 fastvector-5.1.0/docs/api.md
+-rw-rw-rw-   0        0        0       54 2022-08-26 06:02:06.000000 fastvector-5.1.0/docs/index.md
+drwxrwxrwx   0        0        0        0 2023-04-28 09:43:59.222138 fastvector-5.1.0/examples/
+-rw-rw-rw-   0        0        0      175 2023-04-24 16:32:47.000000 fastvector-5.1.0/examples/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:43:59.226124 fastvector-5.1.0/fastvector/
+-rw-rw-rw-   0        0        0      102 2023-03-11 13:24:39.000000 fastvector-5.1.0/fastvector/__init__.py
+-rw-rw-rw-   0        0        0     4450 2023-04-24 16:32:47.000000 fastvector-5.1.0/fastvector/vector.py
+-rw-rw-rw-   0        0        0       22 2023-04-28 09:28:13.000000 fastvector-5.1.0/fastvector/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:43:59.249133 fastvector-5.1.0/fastvector.egg-info/
+-rw-rw-rw-   0        0        0      842 2023-04-28 09:43:59.000000 fastvector-5.1.0/fastvector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      656 2023-04-28 09:43:59.000000 fastvector-5.1.0/fastvector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:43:59.000000 fastvector-5.1.0/fastvector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      275 2023-04-28 09:43:59.000000 fastvector-5.1.0/fastvector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-28 09:43:59.000000 fastvector-5.1.0/fastvector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      830 2022-08-26 06:02:06.000000 fastvector-5.1.0/mkdocs.yml
+-rw-rw-rw-   0        0        0     3888 2023-04-28 09:43:31.000000 fastvector-5.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      323 2023-04-28 09:27:01.000000 fastvector-5.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       37 2023-04-28 09:17:35.000000 fastvector-5.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:43:59.255129 fastvector-5.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 09:43:59.253134 fastvector-5.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-26 06:02:06.000000 fastvector-5.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      402 2023-04-24 16:32:47.000000 fastvector-5.1.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     4169 2023-04-24 16:32:47.000000 fastvector-5.1.0/tests/test_vector.py
```

### Comparing `fastvector-2.0.2/LICENSE` & `fastvector-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastvector-2.0.2/README.md` & `fastvector-5.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,59 @@
 # FastVector
 
-![Python](https://img.shields.io/badge/python-3.7+-blue)
+![Python](https://img.shields.io/badge/python-3.9+-blue)
 ![License](https://camo.githubusercontent.com/890acbdcb87868b382af9a4b1fac507b9659d9bf/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6c6963656e73652d4d49542d626c75652e737667)
-[![Build](https://github.com/franneck94/Python-Project-Template/workflows/ci-test/badge.svg)](https://github.com/franneck94/Python-Project-Template/actions?query=workflow%3Aci-test)
-[![codecov](https://codecov.io/gh/franneck94/python-project-template/branch/master/graph/badge.svg)](https://codecov.io/gh/franneck94/python-project-template)
-[![Documentation](https://img.shields.io/badge/ref-Documentation-blue)](https://franneck94.github.io/Python-Project-Template/)
+[![Build](https://github.com/franneck94/Python-Project-Template/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/franneck94/Python-Project-Template/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/franneck94/Python-Project-Template-Eng/branch/master/graph/badge.svg)](https://codecov.io/gh/franneck94/Python-Project-Template-Eng)
+[![Documentation](https://img.shields.io/badge/ref-Documentation-blue)](https://franneck94.github.io/Python-Project-Template-Eng/)
 
 ## Template For Python Projects
 
 This is a template for Python projects. What you get:
 
 - Source code and test code is seperated in different directories.
-- External libraries installed and managed by [Pip](https://pypi.org/project/pip/).
-- Setup for tests using [Pytest](https://docs.pytest.org/en/stable/).
-- Bechmark tests using [Pytest-Benchmark](https://github.com/ionelmc/pytest-benchmark)
-- Continuous testing with [Github-Actions](https://github.com/features/actions/).
+- External libraries installed and managed by [Pip](https://pypi.org/project/pip/) and [setuptools](https://setuptools.pypa.io/en/latest/) in a pyproject.toml.
+- Setup for tests using [Pytest](https://docs.pytest.org/en/stable/) and coverage with [Pytest-Cov](https://github.com/pytest-dev/pytest-cov).
+- Continuous testing with [Github-Actions](https://github.com/features/actions/) including [pre-commit](https://github.com/pre-commit/pre-commit).
 - Code coverage reports, including automatic upload to [Codecov](https://codecov.io).
 - Code documentation with [Mkdocs](https://www.mkdocs.org/).
-- Example of own Python package with the use of [Cython](https://cython.org/)
-- Optional: Use of [VSCode](https://code.visualstudio.com/) with the Python and UnitTest extension.
 
 ## Structure
 
 ``` text
-├── setup.py
-├── setup.cfg
 ├── pyproject.toml
 ├── ... other config files ...
 ├── tests
 │   ├── __init__.py
-│   ├── test_vector.py
-│   ├── test_computations.py
-│   └── conftest.py
+│   └── test_vector.py
 ├── docs
 │   ├── api.md
 │   └── index.md
 ├── fastvector
 │   ├── __init__.py
 │   ├── vector.py
-│   ├── dtypes.py
-│   ├── version.py
-│   └── cython_computations.pyx
-│   └── computations.py
-└── benchmarks
-│   ├── __init__.py
-│   └── test_computations.py
+│   └── version.py
 └── tests
     ├── __init__.py
-    ├── test_computations.py
     └── test_vector.py
 ```
 
 ### Commands
 
 ```bash
 # Build and Install (local)
-pip install -e .
+pip install -e .  # OR
+pip install -e ../Python-Project-Template  # OR
+pip install -e ../Python-Project-Template[all]
 ```
 
 ```bash
 # Test
-pytest tests
+pytest tests  # OR
+pytest .  # OR
+pytest
 ```
 
 ```bash
 # Code Coverage
 pytest --cov=fastvector tests --cov-report=html
 ```
-
-```bash
-# Benchmarks
-pytest --benchmark-columns=min,max,mean,stddev --benchmark-sort=mean benchmarks
-```
```

