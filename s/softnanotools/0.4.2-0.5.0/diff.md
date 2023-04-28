# Comparing `tmp/softnanotools-0.4.2.tar.gz` & `tmp/softnanotools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softnanotools-0.4.2.tar", last modified: Fri Apr 28 00:41:53 2023, max compression
+gzip compressed data, was "softnanotools-0.5.0.tar", last modified: Fri Apr 28 15:27:33 2023, max compression
```

## Comparing `softnanotools-0.4.2.tar` & `softnanotools-0.5.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.664562 softnanotools-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 00:41:36.000000 softnanotools-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 00:41:36.000000 softnanotools-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 00:41:53.664562 softnanotools-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-28 00:41:36.000000 softnanotools-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 00:41:36.000000 softnanotools-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 00:41:53.664562 softnanotools-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 00:41:36.000000 softnanotools-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.664562 softnanotools-0.4.2/softnanotools/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 00:41:53.664562 softnanotools-0.4.2/softnanotools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.660562 softnanotools-0.4.2/softnanotools/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.660562 softnanotools-0.4.2/softnanotools/generate/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/.gitattributes.template
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/.pre-commit-config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/MANIFEST.in.template
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/__init__.py.template
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/_version.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/coverage.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/pyproject.toml.template
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/quick-build.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/setup.cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/setup.py.template
--rw-r--r--   0 runner    (1001) docker     (123)    68670 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/assets/versioneer.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.660562 softnanotools-0.4.2/softnanotools/generate/git/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/generate/git/_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.660562 softnanotools-0.4.2/softnanotools/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/logger/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.660562 softnanotools-0.4.2/softnanotools/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/notebooks/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/notebooks/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.660562 softnanotools-0.4.2/softnanotools/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/runner/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.660562 softnanotools-0.4.2/softnanotools/timer/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 00:41:36.000000 softnanotools-0.4.2/softnanotools/timer/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.656562 softnanotools-0.4.2/softnanotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 00:41:53.000000 softnanotools-0.4.2/softnanotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-28 00:41:53.000000 softnanotools-0.4.2/softnanotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:41:53.000000 softnanotools-0.4.2/softnanotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 00:41:53.000000 softnanotools-0.4.2/softnanotools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 00:41:53.000000 softnanotools-0.4.2/softnanotools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.660562 softnanotools-0.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.664562 softnanotools-0.4.2/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_generate/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_generate/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_generate/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_generate/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_generate/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_generate/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_generate/test_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.664562 softnanotools-0.4.2/test/test_logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_logger/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:53.664562 softnanotools-0.4.2/test/test_notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_notebooks/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_notebooks/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 00:41:36.000000 softnanotools-0.4.2/test/test_notebooks/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-28 00:41:36.000000 softnanotools-0.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 15:27:22.000000 softnanotools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 15:27:22.000000 softnanotools-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-28 15:27:33.129237 softnanotools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-28 15:27:22.000000 softnanotools-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 15:27:22.000000 softnanotools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 15:27:33.129237 softnanotools-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 15:27:22.000000 softnanotools-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/softnanotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 15:27:33.129237 softnanotools-0.5.0/softnanotools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/generate/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/.gitattributes.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/.pre-commit-config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/MANIFEST.in.template
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/__init__.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/_version.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/coverage.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/pyproject.toml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/quick-build.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/setup.cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/setup.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    68670 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/versioneer.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/generate/git/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/git/_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/logger/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/notebooks/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/notebooks/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/runner/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/timer/_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/test/test_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_logger/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/test/test_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_notebooks/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_notebooks/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_notebooks/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-28 15:27:22.000000 softnanotools-0.5.0/versioneer.py
```

### Comparing `softnanotools-0.4.2/LICENSE` & `softnanotools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/setup.py` & `softnanotools-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/cli.py` & `softnanotools-0.5.0/softnanotools/cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/_components.py` & `softnanotools-0.5.0/softnanotools/generate/_components.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/_module.py` & `softnanotools-0.5.0/softnanotools/generate/_module.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/_package.py` & `softnanotools-0.5.0/softnanotools/generate/_package.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/_project.py` & `softnanotools-0.5.0/softnanotools/generate/_project.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,35 +2,39 @@
 """_project.py - auto-generated by softnanotools."""
 import subprocess
 from typing import List, Union
 from pathlib import Path
 from . import _package
 
 from softnanotools.logger import Logger
+
 logger = Logger(__name__)
 
 ASSETS = Path(__file__).parent / "assets"
 
+
 def execute_template(fname: str, **kwargs) -> str:
     """Takes template from ASSETS folder and formats it with arguments"""
     # copy template from assets folder
     with open(ASSETS / f"{fname}.template", "r") as f:
         result = f.read()
         result = result.format(**kwargs)
     return result
 
+
 def write_template(folder: Union[str, Path], fname: str, content: str):
     """Writes template to file in a project directory"""
     # create folder if it doesn't exist
     folder.mkdir(parents=True, exist_ok=True)
     # write target file to dest
     with open(folder / fname, "w") as f:
         # write templated version with {subs} substitution rules
         f.write(content)
 
+
 def generate(
     name,
     packages: List[str] = None,
     modules: List[str] = None,
     dry_run: bool = False,
     pre_commit: bool = False,
     pip_install: bool = False,
@@ -48,25 +52,17 @@
     _package.generate(root / name, modules=modules, packages=packages)
 
     # create test package
     _package.generate(root / 'test', modules=[f"test_{name}"])
 
     # create list of files to generate
     filenames = [
-        "setup.py",
-        "README.md",
-        "setup.cfg",
-        "_version.py",
-        "MANIFEST.in",
-        ".gitignore",
-        "pyproject.toml",
-        "quick-build.yml",
-        "coverage.yml",
-        "versioneer.py",
-        '.gitattributes'
+        "setup.py", "README.md", "setup.cfg", "_version.py", "MANIFEST.in",
+        ".gitignore", "pyproject.toml", "quick-build.yml", "coverage.yml",
+        "versioneer.py", '.gitattributes'
     ]
 
     if pre_commit:
         filenames.append(".pre-commit-config.yaml")
 
     folders = {
         '_version.py': root / name,
@@ -80,33 +76,60 @@
         templates[fname] = execute_template(fname, name=name)
 
         # add debug statement
         logger.debug(templates[fname])
 
         # write template to file
         write_template(
-            folders.get(fname, root), # use root folder if custom not specified
+            folders.get(fname,
+                        root),  # use root folder if custom not specified
             fname,
-            templates[fname]
-        )
+            templates[fname])
 
     if not dry_run:
-        subprocess.run(["git", "init", "-b", "main"], cwd=root)
+
+        if pip_install:
+            subprocess.run(["pip", "install", "-e", name])
+
+        # Initialise git repo with "main" as default branch
+        try:
+            subprocess.run(["git", "init"], cwd=root)
+        except Exception:
+            logger.warning(
+                "Running git failed, skipping all git steps by default, next "
+                "time use `--dry-run to avoid this warning!"
+            )
+            return
+        try:
+            subprocess.run(['git', 'branch', '-M', 'main'], cwd=root)
+        except Exception:
+            logger.warning(
+                "`git init` worked, but `git branch -M main` failed, consider"
+                " upgrading your version of git! Continuing to add files and "
+                "make first commit."
+            )
+            return
+
+
+
         if pre_commit:
-            subprocess.run(["pre-commit", "install"], cwd=root)
+            try:
+                subprocess.run(["pre-commit", "install"], cwd=root)
+            except Exception:
+                logger.kill(
+                    "`pre-commit install` failed, please reinstall "
+                    "pre-commit with pip install pre-commit or remove "
+                    "the --pre-commit flag!"
+                )
+
         subprocess.run(["git", "add", "."], cwd=root)
         subprocess.run([
-            "git",
-            "commit",
-            "-a",
-            "-m",
+            "git", "commit", "-a", "-m",
             f"'First commit for {name} by softnanotools!'"
         ], cwd=root)
-        if pip_install:
-            subprocess.run(["pip", "install", "-e", name])
 
     return
 
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
```

### Comparing `softnanotools-0.4.2/softnanotools/generate/_script.py` & `softnanotools-0.5.0/softnanotools/generate/_script.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/_tests.py` & `softnanotools-0.5.0/softnanotools/generate/_tests.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/assets/.gitignore.template` & `softnanotools-0.5.0/softnanotools/generate/assets/.gitignore.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/assets/README.md.template` & `softnanotools-0.5.0/softnanotools/generate/assets/README.md.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/assets/_version.py.template` & `softnanotools-0.5.0/softnanotools/generate/assets/_version.py.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/assets/coverage.yml.template` & `softnanotools-0.5.0/softnanotools/generate/assets/coverage.yml.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/assets/setup.cfg.template` & `softnanotools-0.5.0/softnanotools/generate/assets/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/assets/setup.py.template` & `softnanotools-0.5.0/softnanotools/generate/assets/setup.py.template`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     # url="",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.4",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `softnanotools-0.4.2/softnanotools/generate/assets/versioneer.py.template` & `softnanotools-0.5.0/softnanotools/generate/assets/versioneer.py.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/generate/cli.py` & `softnanotools-0.5.0/softnanotools/generate/cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/logger/_logger.py` & `softnanotools-0.5.0/softnanotools/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/notebooks/__init__.py` & `softnanotools-0.5.0/softnanotools/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/notebooks/_core.py` & `softnanotools-0.5.0/softnanotools/notebooks/_core.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/notebooks/_utils.py` & `softnanotools-0.5.0/softnanotools/notebooks/_utils.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/runner/_runner.py` & `softnanotools-0.5.0/softnanotools/runner/_runner.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools/timer/_timer.py` & `softnanotools-0.5.0/softnanotools/timer/_timer.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/softnanotools.egg-info/SOURCES.txt` & `softnanotools-0.5.0/softnanotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/test/test_generate/test_cli.py` & `softnanotools-0.5.0/test/test_generate/test_cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/test/test_generate/test_components.py` & `softnanotools-0.5.0/test/test_generate/test_components.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/test/test_generate/test_project.py` & `softnanotools-0.5.0/test/test_generate/test_project.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/test/test_logger/test_logger.py` & `softnanotools-0.5.0/test/test_logger/test_logger.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.4.2/versioneer.py` & `softnanotools-0.5.0/versioneer.py`

 * *Files identical despite different names*

