# Comparing `tmp/softnanotools-0.4.0.tar.gz` & `tmp/softnanotools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softnanotools-0.4.0.tar", last modified: Fri Apr 28 00:27:21 2023, max compression
+gzip compressed data, was "softnanotools-0.4.1.tar", last modified: Fri Apr 28 00:38:41 2023, max compression
```

## Comparing `softnanotools-0.4.0.tar` & `softnanotools-0.4.1.tar`

### file list

```diff
@@ -1,64 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 00:27:05.000000 softnanotools-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 00:27:05.000000 softnanotools-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 00:27:21.332156 softnanotools-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-28 00:27:05.000000 softnanotools-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 00:27:05.000000 softnanotools-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 00:27:21.332156 softnanotools-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 00:27:05.000000 softnanotools-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/softnanotools/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 00:27:21.332156 softnanotools-0.4.0/softnanotools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/generate/git/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/generate/git/_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/logger/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/notebooks/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/notebooks/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/runner/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.328156 softnanotools-0.4.0/softnanotools/timer/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 00:27:05.000000 softnanotools-0.4.0/softnanotools/timer/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.324156 softnanotools-0.4.0/softnanotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 00:27:21.000000 softnanotools-0.4.0/softnanotools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_generate/test_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/test/test_logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_logger/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:21.332156 softnanotools-0.4.0/test/test_notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_notebooks/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_notebooks/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 00:27:05.000000 softnanotools-0.4.0/test/test_notebooks/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-28 00:27:05.000000 softnanotools-0.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 00:38:27.000000 softnanotools-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 00:38:27.000000 softnanotools-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 00:38:41.951171 softnanotools-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-28 00:38:27.000000 softnanotools-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 00:38:27.000000 softnanotools-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 00:38:41.951171 softnanotools-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 00:38:27.000000 softnanotools-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/softnanotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 00:38:41.951171 softnanotools-0.4.1/softnanotools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.947171 softnanotools-0.4.1/softnanotools/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/softnanotools/generate/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/.gitattributes.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/.pre-commit-config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/MANIFEST.in.template
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/__init__.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/_version.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/coverage.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/pyproject.toml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/quick-build.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/setup.cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/setup.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    68670 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/assets/versioneer.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/softnanotools/generate/git/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/generate/git/_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/softnanotools/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/logger/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/softnanotools/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/notebooks/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/notebooks/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/softnanotools/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/runner/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/softnanotools/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 00:38:27.000000 softnanotools-0.4.1/softnanotools/timer/_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.947171 softnanotools-0.4.1/softnanotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 00:38:41.000000 softnanotools-0.4.1/softnanotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-28 00:38:41.000000 softnanotools-0.4.1/softnanotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:38:41.000000 softnanotools-0.4.1/softnanotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 00:38:41.000000 softnanotools-0.4.1/softnanotools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 00:38:41.000000 softnanotools-0.4.1/softnanotools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_generate/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_generate/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_generate/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_generate/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_generate/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_generate/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_generate/test_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/test/test_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_logger/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:41.951171 softnanotools-0.4.1/test/test_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_notebooks/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_notebooks/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 00:38:27.000000 softnanotools-0.4.1/test/test_notebooks/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-28 00:38:27.000000 softnanotools-0.4.1/versioneer.py
```

### Comparing `softnanotools-0.4.0/LICENSE` & `softnanotools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/PKG-INFO` & `softnanotools-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softnanotools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for computing
 Home-page: https://github.com/softnanolab/softnanotools
 Author: Debesh Mandal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `softnanotools-0.4.0/README.md` & `softnanotools-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/setup.py` & `softnanotools-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/cli.py` & `softnanotools-0.4.1/softnanotools/cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/generate/_components.py` & `softnanotools-0.4.1/softnanotools/generate/_components.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/generate/_module.py` & `softnanotools-0.4.1/softnanotools/generate/_module.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/generate/_package.py` & `softnanotools-0.4.1/softnanotools/generate/_package.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/generate/_project.py` & `softnanotools-0.4.1/softnanotools/generate/_project.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/generate/_script.py` & `softnanotools-0.4.1/softnanotools/generate/_script.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/generate/_tests.py` & `softnanotools-0.4.1/softnanotools/generate/_tests.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/generate/cli.py` & `softnanotools-0.4.1/softnanotools/generate/cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/logger/_logger.py` & `softnanotools-0.4.1/softnanotools/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/notebooks/__init__.py` & `softnanotools-0.4.1/softnanotools/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/notebooks/_core.py` & `softnanotools-0.4.1/softnanotools/notebooks/_core.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/notebooks/_utils.py` & `softnanotools-0.4.1/softnanotools/notebooks/_utils.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/runner/_runner.py` & `softnanotools-0.4.1/softnanotools/runner/_runner.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools/timer/_timer.py` & `softnanotools-0.4.1/softnanotools/timer/_timer.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/softnanotools.egg-info/PKG-INFO` & `softnanotools-0.4.1/softnanotools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softnanotools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for computing
 Home-page: https://github.com/softnanolab/softnanotools
 Author: Debesh Mandal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `softnanotools-0.4.0/softnanotools.egg-info/SOURCES.txt` & `softnanotools-0.4.1/softnanotools.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,27 @@
 softnanotools/generate/_components.py
 softnanotools/generate/_module.py
 softnanotools/generate/_package.py
 softnanotools/generate/_project.py
 softnanotools/generate/_script.py
 softnanotools/generate/_tests.py
 softnanotools/generate/cli.py
+softnanotools/generate/assets/.gitattributes.template
+softnanotools/generate/assets/.gitignore.template
+softnanotools/generate/assets/.pre-commit-config.yaml.template
+softnanotools/generate/assets/MANIFEST.in.template
+softnanotools/generate/assets/README.md.template
+softnanotools/generate/assets/__init__.py.template
+softnanotools/generate/assets/_version.py.template
+softnanotools/generate/assets/coverage.yml.template
+softnanotools/generate/assets/pyproject.toml.template
+softnanotools/generate/assets/quick-build.yml.template
+softnanotools/generate/assets/setup.cfg.template
+softnanotools/generate/assets/setup.py.template
+softnanotools/generate/assets/versioneer.py.template
 softnanotools/generate/git/__init__.py
 softnanotools/generate/git/_actions.py
 softnanotools/logger/__init__.py
 softnanotools/logger/_logger.py
 softnanotools/notebooks/__init__.py
 softnanotools/notebooks/_core.py
 softnanotools/notebooks/_utils.py
```

### Comparing `softnanotools-0.4.0/test/test_generate/test_cli.py` & `softnanotools-0.4.1/test/test_generate/test_cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/test/test_generate/test_components.py` & `softnanotools-0.4.1/test/test_generate/test_components.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/test/test_generate/test_project.py` & `softnanotools-0.4.1/test/test_generate/test_project.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/test/test_logger/test_logger.py` & `softnanotools-0.4.1/test/test_logger/test_logger.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.0/versioneer.py` & `softnanotools-0.4.1/versioneer.py`

 * *Files identical despite different names*

