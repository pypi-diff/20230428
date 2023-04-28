# Comparing `tmp/softnanotools-0.3.6.tar.gz` & `tmp/softnanotools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softnanotools-0.3.6.tar", last modified: Mon Dec  6 17:38:59 2021, max compression
+gzip compressed data, was "softnanotools-0.4.0.tar", last modified: Fri Apr 28 00:27:21 2023, max compression
```

## Comparing `softnanotools-0.3.6.tar` & `softnanotools-0.4.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.985503 softnanotools-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-12-06 17:38:51.000000 softnanotools-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-12-06 17:38:51.000000 softnanotools-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-12-06 17:38:59.985503 softnanotools-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-12-06 17:38:51.000000 softnanotools-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      417 2021-12-06 17:38:59.985503 softnanotools-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      885 2021-12-06 17:38:51.000000 softnanotools-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.985503 softnanotools-0.3.6/softnanotools/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-12-06 17:38:59.985503 softnanotools-0.3.6/softnanotools/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.981503 softnanotools-0.3.6/softnanotools/generate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/_components.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/_package.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/_script.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.981503 softnanotools-0.3.6/softnanotools/generate/git/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/generate/git/_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.981503 softnanotools-0.3.6/softnanotools/logger/
--rw-r--r--   0 runner    (1001) docker     (121)      452 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2901 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/logger/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.981503 softnanotools-0.3.6/softnanotools/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/notebooks/_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/notebooks/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.981503 softnanotools-0.3.6/softnanotools/runner/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/runner/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.985503 softnanotools-0.3.6/softnanotools/timer/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-12-06 17:38:51.000000 softnanotools-0.3.6/softnanotools/timer/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.981503 softnanotools-0.3.6/softnanotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-12-06 17:38:59.000000 softnanotools-0.3.6/softnanotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-12-06 17:38:59.000000 softnanotools-0.3.6/softnanotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-06 17:38:59.000000 softnanotools-0.3.6/softnanotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-12-06 17:38:59.000000 softnanotools-0.3.6/softnanotools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-06 17:38:59.000000 softnanotools-0.3.6/softnanotools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.985503 softnanotools-0.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.985503 softnanotools-0.3.6/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      649 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_generate/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_generate/test_components.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_generate/test_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_generate/test_package.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_generate/test_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_generate/test_script.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_generate/test_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.985503 softnanotools-0.3.6/test/test_logger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_logger/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:59.985503 softnanotools-0.3.6/test/test_notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_notebooks/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_notebooks/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-12-06 17:38:51.000000 softnanotools-0.3.6/test/test_notebooks/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-12-06 17:38:51.000000 softnanotools-0.3.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 00:27:05.000000 softnanotools-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 00:27:05.000000 softnanotools-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 00:27:21.332156 softnanotools-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-28 00:27:05.000000 softnanotools-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 00:27:05.000000 softnanotools-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 00:27:21.332156 softnanotools-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 00:27:05.000000 softnanotools-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/softnanotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 00:27:21.332156 softnanotools-0.4.0/softnanotools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/generate/git/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/git/_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/logger/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/notebooks/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/notebooks/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/runner/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/timer/_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.324156 softnanotools-0.4.0/softnanotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/test/test_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_logger/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/test/test_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_notebooks/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_notebooks/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_notebooks/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-28 00:27:05.000000 softnanotools-0.4.0/versioneer.py
```

### Comparing `softnanotools-0.3.6/LICENSE` & `softnanotools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `softnanotools-0.3.6/README.md` & `softnanotools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `softnanotools-0.3.6/setup.py` & `softnanotools-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 import versioneer
 
-with open("README.md", "r", encoding='utf-8') as f:
+with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="softnanotools",
     author="Debesh Mandal",
     description="Tools for computing",
     long_description=long_description,
@@ -17,13 +17,13 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.5",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     entry_points={
-        'console_scripts': [
-            'softnanotools=softnanotools.cli:main',
-            'softnanotools.generate=softnanotools.generate.cli:main',
+        "console_scripts": [
+            "softnanotools=softnanotools.cli:main",
+            "softnanotools.generate=softnanotools.generate.cli:main",
         ],
     },
 )
```

### Comparing `softnanotools-0.3.6/softnanotools/generate/_components.py` & `softnanotools-0.4.0/softnanotools/generate/_components.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 #!/usr/bin/env python
-"""A module containing the common string-components found in Python
-files
-"""
+"""A module containing the common string-components found in Python files."""
+
 from pathlib import Path
-INDENT = '    '
+
+INDENT = "    "
+
 
 class ComponentContainer:
-    """Container for different components used in auto-generated Python
-    files
+    """Container for different components used in auto-generated Python files.
 
     Arguments:
         name: name of the file being generated (excluding .py)
     """
+
     shebang = "#!/usr/bin/env python"
 
-    if_name_statement = (
-        "if __name__ == '__main__':"
-    )
-    doctest_string = (
-        f'{INDENT}import doctest\n'
-        f'{INDENT}doctest.testmod()'
-    )
+    if_name_statement = "if __name__ == '__main__':"
+    doctest_string = f"{INDENT}import doctest\n" f"{INDENT}doctest.testmod()"
 
     def __init__(self, name: str):
         name = Path(name)
         self._path = Path(name)
         self._name = self._path.name
 
     @property
     def name(self) -> str:
-        split = self._name.split('.')
-        if split[-1] == 'py':
-            name = '.'.join(split[:-1])
+        split = self._name.split(".")
+        if split[-1] == "py":
+            name = ".".join(split[:-1])
         else:
             name = self._name
         return name
 
     @property
     def path(self) -> Path:
-        return self._path.parent / f'{self.name}.py'
+        return self._path.parent / f"{self.name}.py"
 
     @property
     def description(self) -> str:
         return f"{self.name}.py - auto-generated by softnanotools"
 
     @property
     def logger(self) -> str:
-        return (
-            "from softnanotools.logger import Logger\n"
-            "logger = Logger(__name__)\n"
-        )
+        return "from softnanotools.logger import Logger\n" "logger = Logger(__name__)\n"
 
     @property
     def docstring(self) -> str:
         return f'"""{self.description}"""'
 
     @property
     def parser(self) -> str:
@@ -70,15 +63,17 @@
             "def main(**kwargs):\n"
             f"{INDENT}logger.info('Running {self.name}...')\n"
             f"{INDENT}# insert code here\n"
             f"{INDENT}logger.info('Done!')\n"
             f"{INDENT}return\n"
         )
 
+
 class FileContainer:
     def __init__(self, name: str):
         self.name = name
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import doctest
-    doctest.testmod()
+
+    doctest.testmod()
```

### Comparing `softnanotools-0.3.6/softnanotools/generate/_module.py` & `softnanotools-0.4.0/softnanotools/generate/_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 from pathlib import Path
 from typing import Union
-
+from ._components import ComponentContainer
 from ..logger import Logger
 logger = Logger(__name__)
 
-from ._components import ComponentContainer
-
 class Module(ComponentContainer):
     def __init__(self, name: Union[str, Path]):
         super().__init__(name)
 
     @property
     def string(self) -> str:
         result = (
@@ -18,14 +16,15 @@
             f"{self.docstring}\n"
             f"{self.logger}\n"
             f"{self.if_name_statement}\n"
             f"{self.doctest_string}\n"
         )
         return result
 
+
 def generate(name: str, **kwargs):
 
     module = Module(name)
-    with open(module.path, 'w') as f:
+    with open(module.path, "w") as f:
         f.write(module.string)
 
-    return
+    return
```

### Comparing `softnanotools-0.3.6/softnanotools/logger/_logger.py` & `softnanotools-0.4.0/softnanotools/logger/_logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,81 @@
+"""Container for the Logger class.
+
+Classes:
+    Logger: tool for logging
+    NewLineFormatter: 
+        formatter for the logger, ensuring prefixes can be easily
+        added on each new line
+
+"""
 import logging
-import sys
 import os
 from pathlib import Path
 
 from typing import Union
 
+
 class NewLineFormatter(logging.Formatter):
-    """Custom Formatter to allow newlines"""
-    def __init__(self):
-        """Initialise with normal logging format string"""
-        logging.Formatter.__init__(self, '%(levelname)s: [%(name)s] %(message)s')
+    """Custom Formatter to allow newlines."""
 
+    def __init__(self):
+        """Initialise with normal logging format string."""
+        logging.Formatter.__init__(self, "%(levelname)s: [%(name)s] %(message)s")
 
     def format(self, record) -> str:
-        """Formatter to ensure that new lines include the prefix"""
+        """Formatter to ensure that new lines include the prefix."""
         msg = logging.Formatter.format(self, record)
 
         if record.message != "":
             parts = msg.split(record.message)
-            msg = msg.replace('\n', '\n' + parts[0])
+            msg = msg.replace("\n", "\n" + parts[0])
 
         return msg
 
+
 class Logger:
-    """Smart logger with formatting
+    """Smart logger with formatting.
 
     The default logging level is INFO, to allow debug
     statements, create the following environment variable
     ```
     export DEBUG_LEVEL=10
     ```
-    
-    Usage:
-        import softnanotools.logger
-        logger = softnanotools.logger.Logger(__name__)
-        logger.debug('Debug Message')
-        logger.info('Info Message')
-        logger.warning('Warning Message')
-        logger.error('Error Message')
-        logger.kill('Error Message')
+
+    Parameters:
+        name: name of the logger (appears in every message)
+        logfile: optional path to logfile where data will be written
+
+    >>> import softnanotools.logger
+    >>> logger = softnanotools.logger.Logger(__name__)
+    >>> logger.debug('Debug Message')
+    >>> logger.info('Info Message')
+    >>> logger.warning('Warning Message')
+    >>> logger.error('Error Message')
+    >>> logger.kill('Error Message')
     """
+
     def __init__(self, name: str, logfile: Union[str, Path] = None):
-        """Initialise using filename or custom name"""
-        if name == '__main__':
-            name = 'root'
+        """Initialise using filename or custom name."""
+        if name == "__main__":
+            name = "root"
         self.logger = logging.getLogger(name)
-        self.logger.setLevel(
-            int(os.environ.get('DEBUG_LEVEL', logging.INFO))
-        )
+        self.logger.propagate = False
+        self.logger.setLevel(int(os.environ.get("DEBUG_LEVEL", logging.INFO)))
 
         # manage default logging to stdout
         ch = logging.StreamHandler()
         ch.setFormatter(NewLineFormatter())
         self.logger.addHandler(ch)
 
         # >>> add option for file logging
 
         # if not given try and get from environment variable
         if not logfile:
-            logfile = os.environ.get('LOGFILE', False)
+            logfile = os.environ.get("LOGFILE", False)
 
         # create file handler (fh) and add to logger
         if logfile:
             fh = logging.FileHandler(logfile)
             fh.setFormatter(NewLineFormatter())
             self.logger.addHandler(fh)
 
@@ -71,29 +84,27 @@
         return self.logger.level
 
     @level.setter
     def level(self, value):
         self.logger.setLevel(value)
 
     def debug(self, message):
-        """Print a debug message for DEBUG_LEVEL<=10"""
+        """Print a debug message for DEBUG_LEVEL<=10."""
         self.logger.debug(message)
 
     def info(self, message):
-        """Print an info message for DEBUG_LEVEL<=20"""
+        """Print an info message for DEBUG_LEVEL<=20."""
         self.logger.info(message)
 
     def warning(self, message):
-        """Print a warning message for DEBUG_LEVEL<=30"""
+        """Print a warning message for DEBUG_LEVEL<=30."""
         self.logger.warning(message)
 
     def error(self, message):
-        """Print an error message for DEBUG_LEVEL<=40"""
+        """Print an error message for DEBUG_LEVEL<=40."""
         self.logger.error(message)
         raise SystemError(message)
 
-    def kill(self, message=''):
-        """Kill program and print message for DEBUG_LEVEL<=50"""
+    def kill(self, message=""):
+        """Kill program and print message for DEBUG_LEVEL<=50."""
         self.logger.critical(message)
         raise SystemExit(message)
-
-
```

### Comparing `softnanotools-0.3.6/softnanotools/notebooks/__init__.py` & `softnanotools-0.4.0/softnanotools/notebooks/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-The `notebooks` module contains tools for importing and
+"""The `notebooks` module contains tools for importing and
 scripting the generation of Jupyter Notebooks.
 
 To a computer scientist Jupyter Notebooks are nothing 
 but key:value objects that can be represented in a
 number of ways. For example the YAML file format 
 (which is a parent of JSON) can be used, or indeed its
 child JSON, or XML ... Okay, these are about it.
@@ -14,11 +13,10 @@
 
 classes:
     IPythonNotebook - notebook container
     IPythonCell - element in notebook
     IPythonTools - a class full of static methods
 
 """
-from ._core import IPythonCell, IPythonNotebook, MARKDOWN, CODE
 from ._utils import IPythonTools
 
 merge = IPythonTools.merge
```

### Comparing `softnanotools-0.3.6/softnanotools/notebooks/_utils.py` & `softnanotools-0.4.0/softnanotools/notebooks/_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,40 @@
+"""Jupyter and IPython Notebook Tools.
+
+Classes:
+    IPythonTools: A collection of tools for manipulating IPython notebooks
+"""
 from ._core import IPythonCell, IPythonNotebook
 from typing import List
 
+
 class IPythonTools:
-    """A container for tools for manipulating IPython Notebooks"""
+    """A container for tools for manipulating IPython Notebooks."""
 
     @staticmethod
     def merge(files: List[str], out: str = None, **kwargs):
-        """Merge a list of IPython files"""
+        """Merge a list of IPython files.
+
+        Params:
+            files: list of filepaths (useful with wildcards or globs)
+            out: optional output file
+
+        Returns:
+            IPythonNotebook instance containing the merged cells
+            from the list of filepaths
+
+        Raises:
+            AssertionError: if any standards are not met
+        """
         output = IPythonNotebook()
         notebooks = []
         for fname in files:
             notebooks.append(IPythonNotebook(fname=fname))
-            for cell in notebooks[-1].data['cells']:
-                if cell.get('outputs', None):
-                    del cell['outputs']
-                if cell.get('execution_count', None):
-                    del cell['execution_count']
-                output.data['cells'].append(vars(IPythonCell(cell)))
+            for cell in notebooks[-1].data["cells"]:
+                if cell.get("outputs", None):
+                    del cell["outputs"]
+                if cell.get("execution_count", None):
+                    del cell["execution_count"]
+                output.data["cells"].append(vars(IPythonCell(cell)))
         if out:
             output.write(out)
         return output
-
```

### Comparing `softnanotools-0.3.6/softnanotools/timer/_timer.py` & `softnanotools-0.4.0/softnanotools/timer/_timer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
-"""Timer classes with in-built summaries"""
+"""Timer classes with in-built summaries."""
 import time
 from typing import Any
 from ..logger import Logger
+
 logger = Logger(__name__)
 
-class Timer():
+
+class Timer:
     def __init__(self):
         self.times = {}
         self.names = {}
 
     def __call__(self, fn, *args, code: Any = None, **kwargs):
         start = time.perf_counter()
         result = fn(*args, **kwargs)
@@ -26,13 +28,10 @@
     def summary(self) -> str:
         result = (
             f"Timing Summary ({self.total:.6f}s)\n"
             "----------------------------------\n"
             f"{'Code':<9}{'Name':<16}{'Time':<6}\n"
         )
         for key in self.times:
-            result += (
-                f"<{key:.>5}>  {self.names[key]:<15}"
-                f" {self.times[key]:.6f}s\n"
-            )
+            result += f"<{key:.>5}>  {self.names[key]:<15}" f" {self.times[key]:.6f}s\n"
         result += "----------------------------------"
-        return result
+        return result
```

### Comparing `softnanotools-0.3.6/softnanotools.egg-info/SOURCES.txt` & `softnanotools-0.4.0/softnanotools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 softnanotools/__init__.py
 softnanotools/_version.py
 softnanotools/cli.py
 softnanotools.egg-info/PKG-INFO
```

### Comparing `softnanotools-0.3.6/test/test_generate/test_cli.py` & `softnanotools-0.4.0/test/test_generate/test_cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.3.6/test/test_generate/test_components.py` & `softnanotools-0.4.0/test/test_generate/test_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     container.parser
     container.main_function
     container.shebang
     container.doctest_string
     return
 
 def test_FileContainer():
-    container = components.FileContainer('example')
+    components.FileContainer('example')
     return
 
 if __name__ == '__main__':
     test_ComponentContainer()
     test_FileContainer()
```

### Comparing `softnanotools-0.3.6/test/test_logger/test_logger.py` & `softnanotools-0.4.0/test/test_logger/test_logger.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.3.6/versioneer.py` & `softnanotools-0.4.0/versioneer.py`

 * *Files identical despite different names*

