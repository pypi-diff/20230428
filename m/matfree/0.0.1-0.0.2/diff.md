# Comparing `tmp/matfree-0.0.1.tar.gz` & `tmp/matfree-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matfree-0.0.1.tar", last modified: Fri Apr 28 09:56:54 2023, max compression
+gzip compressed data, was "matfree-0.0.2.tar", last modified: Fri Apr 28 12:15:50 2023, max compression
```

## Comparing `matfree-0.0.1.tar` & `matfree-0.0.2.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.711866 matfree-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.699866 matfree-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.703866 matfree-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-28 09:56:39.000000 matfree-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 09:56:39.000000 matfree-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-28 09:56:39.000000 matfree-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-28 09:56:39.000000 matfree-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 09:56:39.000000 matfree-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 09:56:39.000000 matfree-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 09:56:54.711866 matfree-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-28 09:56:39.000000 matfree-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.703866 matfree-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.703866 matfree-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 09:56:39.000000 matfree-0.0.1/docs/api/decomp.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 09:56:39.000000 matfree-0.0.1/docs/api/hutch.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 09:56:39.000000 matfree-0.0.1/docs/api/montecarlo.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 09:56:39.000000 matfree-0.0.1/docs/api/slq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.703866 matfree-0.0.1/docs/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-28 09:56:39.000000 matfree-0.0.1/docs/benchmarks/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 09:56:39.000000 matfree-0.0.1/docs/benchmarks/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.703866 matfree-0.0.1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 09:56:39.000000 matfree-0.0.1/docs/dev/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-28 09:56:39.000000 matfree-0.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.707866 matfree-0.0.1/matfree/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 09:56:54.000000 matfree-0.0.1/matfree/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.711866 matfree-0.0.1/matfree/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/np.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/prng.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/backend/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/hutch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/slq.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-28 09:56:39.000000 matfree-0.0.1/matfree/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.707866 matfree-0.0.1/matfree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 09:56:54.000000 matfree-0.0.1/matfree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-28 09:56:54.000000 matfree-0.0.1/matfree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:56:54.000000 matfree-0.0.1/matfree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-28 09:56:54.000000 matfree-0.0.1/matfree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 09:56:54.000000 matfree-0.0.1/matfree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 09:56:39.000000 matfree-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-28 09:56:39.000000 matfree-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 09:56:54.711866 matfree-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 09:56:39.000000 matfree-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:56:54.711866 matfree-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 09:56:39.000000 matfree-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 09:56:39.000000 matfree-0.0.1/tests/test_autodiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-28 09:56:39.000000 matfree-0.0.1/tests/test_decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-28 09:56:39.000000 matfree-0.0.1/tests/test_hutch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-28 09:56:39.000000 matfree-0.0.1/tests/test_montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-28 09:56:39.000000 matfree-0.0.1/tests/test_slq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.030550 matfree-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-28 12:15:34.000000 matfree-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-28 12:15:34.000000 matfree-0.0.2/.github/workflows/doc-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 12:15:34.000000 matfree-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-28 12:15:34.000000 matfree-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-28 12:15:34.000000 matfree-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 12:15:34.000000 matfree-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 12:15:34.000000 matfree-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 12:15:50.038550 matfree-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-28 12:15:34.000000 matfree-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/api/decomp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/api/hutch.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/api/montecarlo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/api/slq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/benchmarks/control_variates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/benchmarks/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/dev/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/matfree/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 12:15:49.000000 matfree-0.0.2/matfree/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/matfree/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/prng.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/hutch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/slq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/matfree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-28 12:15:34.000000 matfree-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-28 12:15:34.000000 matfree-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 12:15:50.042550 matfree-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 12:15:34.000000 matfree-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_autodiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_hutch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_slq.py
```

### Comparing `matfree-0.0.1/.github/workflows/ci.yaml` & `matfree-0.0.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/.github/workflows/release.yml` & `matfree-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/.gitignore` & `matfree-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/.pre-commit-config.yaml` & `matfree-0.0.2/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 ---
 default_language_version:
   python: python3
 repos:
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
+    hooks:
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+      - id: check-merge-conflict
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
@@ -17,7 +24,11 @@
     hooks:
       - id: ruff
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
       - id: mypy
         args: [--no-strict-optional, --ignore-missing-imports]
+  - repo: https://github.com/lyz-code/yamlfix/
+    rev: 1.9.0
+    hooks:
+      - id: yamlfix
```

### Comparing `matfree-0.0.1/LICENSE` & `matfree-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/PKG-INFO` & `matfree-0.0.2/docs/index.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1
-Name: matfree
-Version: 0.0.1
-Summary: Trace estimation and so on
-Author: Nicholas Krämer
-Author-email: pekra@dtu.dk
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: cpu
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: format
-Provides-Extra: doc
-Provides-Extra: full
-License-File: LICENSE
-
 # matfree
 Randomised and deterministic matrix-free methods for trace estimation, matrix functions, and/or matrix factorisations.
+Builds on [JAX](https://jax.readthedocs.io/en/latest/).
+
+## Installation
+
+To install the package, run
+
+```commandline
+pip install matfree
+```
+
+**Important:** This assumes you already have a working installation of JAX.
+To install JAX, [follow these instructions](https://github.com/google/jax#installation).
+To combine `matfree` with a CPU version of JAX, run
+
+```commandline
+pip install matfree[cpu]
+```
+which is equivalent to combining `pip install jax[cpu]` with `pip install matfree`.
 
 
 ## Minimal example
 
 Imports:
 ```python
 >>> import jax
@@ -32,15 +33,15 @@
 
 ```
 
 ### Traces
 
 Estimate traces as such:
 ```python
->>> sample_fun = montecarlo.normal(shape=(2,), dtype=float)
+>>> sample_fun = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
 515.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
@@ -64,15 +65,15 @@
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
->>> keys = jax.random.split(key, num=10_000)  
+>>> keys = jax.random.split(key, num=10_000)
 >>> trace, diagonal = hutch.trace_and_diagonal(matvec, keys=keys, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
 509.0
 
 >>> print(jnp.round(diagonal))
 [222. 287.]
 
@@ -84,15 +85,15 @@
 [220. 286.]
 
 
 ```
 
 ## Contributing
 
-Contributions are absolutely welcome! 
+Contributions are absolutely welcome!
 Most contributions start with an issue.
 Please don't hesitate to create issues in which you
 ask for features, give feedback on performances, or simply want to reach out.
 
 To make a pull request, proceed as follows:
 Fork the repository.
 Install all dependencies with `pip install .[full]` or `pip install -e .[full]`.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `matfree-0.0.1/README.md` & `matfree-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,47 @@
 # matfree
 Randomised and deterministic matrix-free methods for trace estimation, matrix functions, and/or matrix factorisations.
+Builds on [JAX](https://jax.readthedocs.io/en/latest/).
+
+## Installation
+
+To install the package, run
+
+```commandline
+pip install matfree
+```
+
+**Important:** This assumes you already have a working installation of JAX.
+To install JAX, [follow these instructions](https://github.com/google/jax#installation).
+To combine `matfree` with a CPU version of JAX, run
+
+```commandline
+pip install matfree[cpu]
+```
+which is equivalent to combining `pip install jax[cpu]` with `pip install matfree`.
 
 
 ## Minimal example
 
 Imports:
 ```python
 >>> import jax
 >>> import jax.numpy as jnp
->>> from matfree import hutch, montecarlo
+>>> from matfree import hutch, montecarlo, slq
 
 >>> a = jnp.reshape(jnp.arange(12.), (6, 2))
 >>> key = jax.random.PRNGKey(1)
 
 ```
 
 ### Traces
 
 Estimate traces as such:
 ```python
->>> sample_fun = montecarlo.normal(shape=(2,), dtype=float)
+>>> sample_fun = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
 515.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
@@ -47,15 +65,15 @@
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
->>> keys = jax.random.split(key, num=10_000)  
+>>> keys = jax.random.split(key, num=10_000)
 >>> trace, diagonal = hutch.trace_and_diagonal(matvec, keys=keys, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
 509.0
 
 >>> print(jnp.round(diagonal))
 [222. 287.]
 
@@ -65,17 +83,35 @@
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
 
 
 ```
 
+### Determinants
+
+
+Estimate log-determinants as such:
+```python
+>>> a = jnp.reshape(jnp.arange(36.), (6, 6)) / 36
+>>> sample_fun = montecarlo.normal(shape=(6,))
+>>> matvec = lambda x: a.T @ (a @ x) + x
+>>> order = 3
+>>> logdet, _ = slq.trace_of_matfun(jnp.log, matvec, order, key=key, sample_fun=sample_fun)
+>>> print(jnp.round(logdet))
+3.0
+>>> # for comparison:
+>>> print(jnp.round(jnp.linalg.slogdet(a.T @ a + jnp.eye(6))[1]))
+3.0
+
+```
+
 ## Contributing
 
-Contributions are absolutely welcome! 
+Contributions are absolutely welcome!
 Most contributions start with an issue.
 Please don't hesitate to create issues in which you
 ask for features, give feedback on performances, or simply want to reach out.
 
 To make a pull request, proceed as follows:
 Fork the repository.
 Install all dependencies with `pip install .[full]` or `pip install -e .[full]`.
```

### Comparing `matfree-0.0.1/docs/benchmarks/control_variates.py` & `matfree-0.0.2/docs/benchmarks/control_variates.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/matfree/backend/func.py` & `matfree-0.0.2/matfree/backend/func.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/matfree/backend/np.py` & `matfree-0.0.2/matfree/backend/np.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/matfree/decomp.py` & `matfree-0.0.2/matfree/decomp.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/matfree/hutch.py` & `matfree-0.0.2/matfree/hutch.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,27 +14,46 @@
 
 def trace(matvec_fun, /, **kwargs):
     """Estimate the trace of a matrix stochastically."""
 
     def quadform(vec):
         return np.vecdot(vec, matvec_fun(vec))
 
-    return _stochastic_estimate(quadform, **kwargs)
+    return stochastic_estimate(quadform, **kwargs)
+
+
+def frobeniusnorm_squared(matvec_fun, /, **kwargs):
+    r"""Estimate the squared Frobenius norm of a matrix stochastically.
+
+    The Frobenius norm of a matrix $A$ is defined as
+
+    $$
+    \|A\|_F^2 = \text{trace}(A^\top A)
+    $$
+
+    so computing squared Frobenius norms amounts to trace estimation.
+    """
+
+    def quadform(vec):
+        Av = matvec_fun(vec)
+        return np.vecdot(Av, Av)
+
+    return stochastic_estimate(quadform, **kwargs)
 
 
 def diagonal(matvec_fun, /, **kwargs):
     """Estimate the diagonal of a matrix stochastically."""
 
     def quadform(vec):
         return vec * matvec_fun(vec)
 
-    return _stochastic_estimate(quadform, **kwargs)
+    return stochastic_estimate(quadform, **kwargs)
 
 
-def _stochastic_estimate(
+def stochastic_estimate(
     fun, /, *, key, sample_fun, num_batches=1, num_samples_per_batch=10_000
 ):
     """Hutchinson-style stochastic estimation."""
     fun_mc = montecarlo.montecarlo(fun, sample_fun=sample_fun)
     fun_single_batch = montecarlo.mean_vmap(fun_mc, num_samples_per_batch)
     fun_batched = montecarlo.mean_loop(fun_single_batch, num_batches)
     mean, _ = fun_batched(key)
```

### Comparing `matfree-0.0.1/matfree/montecarlo.py` & `matfree-0.0.2/matfree/montecarlo.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,24 +90,24 @@
     num_nans_new = num_nans + fx_is_nan * how_many_max
 
     # Update mean estimate
     mean_new = np.sum(np.asarray([mean * i, fx_values]), axis=0) / (i + 1)
     return _MState(mean=mean_new, key=subkey, num_nans=num_nans_new)
 
 
-def normal(*, shape, dtype):
+def normal(*, shape, dtype=float):
     """Construct a function that samples from a standard normal distribution."""
 
     def fun(key):
         return prng.normal(key, shape=shape, dtype=dtype)
 
     return fun
 
 
-def rademacher(*, shape, dtype):
+def rademacher(*, shape, dtype=float):
     """Normalised Rademacher distributions."""
 
     def fun(key):
         return prng.rademacher(key, shape=shape, dtype=dtype)
 
     return fun
```

### Comparing `matfree-0.0.1/matfree/slq.py` & `matfree-0.0.2/matfree/slq.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 """Stochastic Lanczos quadrature."""
 
 from matfree import decomp, montecarlo
-from matfree.backend import func, linalg, np, prng
+from matfree.backend import func, linalg, np
 
 
 def trace_of_matfun(
     matfun,
     Av,
     order,
     /,
     *,
     key,
-    num_samples_per_batch,
-    num_batches,
-    tangents_shape,
-    tangents_dtype,
-    sample_fun=prng.normal,
+    sample_fun,
+    num_samples_per_batch=10,
+    num_batches=1,
 ):
     """Compute the trace of the function of a matrix.
 
     For example, logdet(M) = trace(log(M)) ~ trace(U log(D) Ut) = E[v U log(D) Ut vt].
     """
-
-    def sample(k, /):
-        return sample_fun(k, shape=tangents_shape, dtype=tangents_dtype)
-
     quadform = quadratic_form_slq(matfun, Av, order)
-    quadform_mc = montecarlo.montecarlo(quadform, sample_fun=sample)
+    quadform_mc = montecarlo.montecarlo(quadform, sample_fun=sample_fun)
 
     quadform_batch = montecarlo.mean_vmap(quadform_mc, num_samples_per_batch)
     quadform_batch = montecarlo.mean_map(quadform_batch, num_batches)
     return quadform_batch(key)
 
 
 def quadratic_form_slq(matfun, Av, order, /):
```

### Comparing `matfree-0.0.1/matfree/test_util.py` & `matfree-0.0.2/matfree/test_util.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/matfree.egg-info/PKG-INFO` & `matfree-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.1
-Summary: Trace estimation and so on
+Version: 0.0.2
+Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
 Provides-Extra: test
@@ -13,34 +13,52 @@
 Provides-Extra: format
 Provides-Extra: doc
 Provides-Extra: full
 License-File: LICENSE
 
 # matfree
 Randomised and deterministic matrix-free methods for trace estimation, matrix functions, and/or matrix factorisations.
+Builds on [JAX](https://jax.readthedocs.io/en/latest/).
+
+## Installation
+
+To install the package, run
+
+```commandline
+pip install matfree
+```
+
+**Important:** This assumes you already have a working installation of JAX.
+To install JAX, [follow these instructions](https://github.com/google/jax#installation).
+To combine `matfree` with a CPU version of JAX, run
+
+```commandline
+pip install matfree[cpu]
+```
+which is equivalent to combining `pip install jax[cpu]` with `pip install matfree`.
 
 
 ## Minimal example
 
 Imports:
 ```python
 >>> import jax
 >>> import jax.numpy as jnp
->>> from matfree import hutch, montecarlo
+>>> from matfree import hutch, montecarlo, slq
 
 >>> a = jnp.reshape(jnp.arange(12.), (6, 2))
 >>> key = jax.random.PRNGKey(1)
 
 ```
 
 ### Traces
 
 Estimate traces as such:
 ```python
->>> sample_fun = montecarlo.normal(shape=(2,), dtype=float)
+>>> sample_fun = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
 515.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
@@ -64,15 +82,15 @@
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
->>> keys = jax.random.split(key, num=10_000)  
+>>> keys = jax.random.split(key, num=10_000)
 >>> trace, diagonal = hutch.trace_and_diagonal(matvec, keys=keys, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
 509.0
 
 >>> print(jnp.round(diagonal))
 [222. 287.]
 
@@ -82,17 +100,35 @@
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
 
 
 ```
 
+### Determinants
+
+
+Estimate log-determinants as such:
+```python
+>>> a = jnp.reshape(jnp.arange(36.), (6, 6)) / 36
+>>> sample_fun = montecarlo.normal(shape=(6,))
+>>> matvec = lambda x: a.T @ (a @ x) + x
+>>> order = 3
+>>> logdet, _ = slq.trace_of_matfun(jnp.log, matvec, order, key=key, sample_fun=sample_fun)
+>>> print(jnp.round(logdet))
+3.0
+>>> # for comparison:
+>>> print(jnp.round(jnp.linalg.slogdet(a.T @ a + jnp.eye(6))[1]))
+3.0
+
+```
+
 ## Contributing
 
-Contributions are absolutely welcome! 
+Contributions are absolutely welcome!
 Most contributions start with an issue.
 Please don't hesitate to create issues in which you
 ask for features, give feedback on performances, or simply want to reach out.
 
 To make a pull request, proceed as follows:
 Fork the repository.
 Install all dependencies with `pip install .[full]` or `pip install -e .[full]`.
```

### Comparing `matfree-0.0.1/matfree.egg-info/SOURCES.txt` & `matfree-0.0.2/matfree.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 Makefile
 README.md
 mkdocs.yml
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/ci.yaml
+.github/workflows/doc-publish.yml
 .github/workflows/release.yml
 docs/index.md
 docs/api/decomp.md
 docs/api/hutch.md
 docs/api/montecarlo.md
 docs/api/slq.md
 docs/benchmarks/control_variates.py
 docs/benchmarks/index.md
 docs/dev/index.md
+docs/javascripts/mathjax.js
 matfree/__init__.py
 matfree/_version.py
 matfree/decomp.py
 matfree/hutch.py
 matfree/montecarlo.py
 matfree/slq.py
 matfree/test_util.py
```

### Comparing `matfree-0.0.1/mkdocs.yml` & `matfree-0.0.2/mkdocs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -28,28 +28,37 @@
       scheme: slate
       primary: black
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
   font:
     text: Fira Sans
-    code: Inconsolata
   features: [navigation.tabs, navigation.footer]
 plugins:
   - search
   - mkdocstrings:
       handlers:
         python:
           options:
-            show_root_members_full_path: true
+            show_root_members_full_path: false
             show_category_heading: false
             docstring_style: numpy
             show_if_no_docstring: true
             show_signature_annotations: true
+            members_order: source
 watch: [matfree]
 extra:
   social:
     - icon: fontawesome/brands/twitter
       link: https://twitter.com/@pnkraemer
       name: Nico
   generator: false
 copyright: Copyright &copy; 2023 Nicholas Krämer
+markdown_extensions:
+  - pymdownx.superfences
+  - pymdownx.arithmatex:
+      generic: true
+extra_javascript:
+  # From: https://squidfunk.github.io/mkdocs-material/reference/mathjax/#mkdocsyml
+  - javascripts/mathjax.js
+  - https://polyfill.io/v3/polyfill.min.js?features=es6
+  - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
```

### Comparing `matfree-0.0.1/pyproject.toml` & `matfree-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/setup.cfg` & `matfree-0.0.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = matfree
-description = Trace estimation and so on
+description = Matrix-free numerical linear algebra including trace-estimation.
 author = Nicholas Krämer
 author_email = pekra@dtu.dk
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
@@ -22,16 +22,14 @@
 	%(test)s
 	pre-commit
 	ruff
 	mypy
 format = 
 	isort
 	black
-	yamlfix
-	end-of-file
 doc = 
 	mkdocs
 	mkdocs-material
 	mkdocstrings
 	mkdocstrings-python
 	matplotlib
 	tqdm
```

### Comparing `matfree-0.0.1/tests/test_autodiff.py` & `matfree-0.0.2/tests/test_autodiff.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for (selected) autodiff functionality."""
 
 
-from matfree import slq, test_util
+from matfree import montecarlo, slq, test_util
 from matfree.backend import np, prng, testing
 
 
 @testing.fixture
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
@@ -28,18 +28,18 @@
         return _logdet(s, order, key)
 
     testing.check_grads(fun, (A,), order=1, atol=1e-1, rtol=1e-1)
 
 
 def _logdet(A, order, key):
     n, _ = np.shape(A)
+    fun = montecarlo.normal(shape=(n,))
     received, num_nans = slq.trace_of_matfun(
         np.log,
         lambda v: A @ v,
         order,
         key=key,
         num_samples_per_batch=10,
         num_batches=1,
-        tangents_shape=(n,),
-        tangents_dtype=float,
+        sample_fun=fun,
     )
     return received
```

### Comparing `matfree-0.0.1/tests/test_decomp.py` & `matfree-0.0.2/tests/test_decomp.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/tests/test_hutch.py` & `matfree-0.0.2/tests/test_hutch.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,40 @@
     return prng.PRNGKey(seed=1)
 
 
 @testing.parametrize("num_batches", [1_000])
 @testing.parametrize("num_samples_per_batch", [1_000])
 @testing.parametrize("dim", [1, 10])
 @testing.parametrize("sample_fun", [montecarlo.normal, montecarlo.rademacher])
+def test_frobeniusnorm_squared(
+    fun, key, num_batches, num_samples_per_batch, dim, sample_fun
+):
+    """Assert that the Frobenius norm estimate is accurate."""
+    # Linearise function
+    x0 = prng.uniform(key, shape=(dim,))  # random lin. point
+    _, jvp = func.linearize(fun, x0)
+    J = func.jacfwd(fun)(x0)
+
+    # Estimate the trace
+    fun = sample_fun(shape=np.shape(x0), dtype=np.dtype(x0))
+    estimate = hutch.frobeniusnorm_squared(
+        jvp,
+        num_batches=num_batches,
+        key=key,
+        num_samples_per_batch=num_samples_per_batch,
+        sample_fun=fun,
+    )
+    truth = np.trace(J.T @ J)
+    assert np.allclose(estimate, truth, rtol=1e-2)
+
+
+@testing.parametrize("num_batches", [1_000])
+@testing.parametrize("num_samples_per_batch", [1_000])
+@testing.parametrize("dim", [1, 10])
+@testing.parametrize("sample_fun", [montecarlo.normal, montecarlo.rademacher])
 def test_trace(fun, key, num_batches, num_samples_per_batch, dim, sample_fun):
     """Assert that the estimated trace approximates the true trace accurately."""
     # Linearise function
     x0 = prng.uniform(key, shape=(dim,))  # random lin. point
     _, jvp = func.linearize(fun, x0)
     J = func.jacfwd(fun)(x0)
```

### Comparing `matfree-0.0.1/tests/test_montecarlo.py` & `matfree-0.0.2/tests/test_montecarlo.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.1/tests/test_slq.py` & `matfree-0.0.2/tests/test_slq.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for Lanczos functionality."""
 
-from matfree import slq, test_util
+from matfree import montecarlo, slq, test_util
 from matfree.backend import linalg, np, prng, testing
 
 
 @testing.fixture
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
@@ -19,20 +19,20 @@
 @testing.parametrize("order", [10])
 # usually: ~1.5 * num_significant_eigvals.
 # But logdet seems to converge sooo much faster.
 def test_logdet(A, order):
     """Assert that the log-determinant estimation matches the true log-determinant."""
     n, _ = np.shape(A)
     key = prng.PRNGKey(1)
+    fun = montecarlo.normal(shape=(n,))
     received, num_nans = slq.trace_of_matfun(
         np.log,
         lambda v: A @ v,
         order,
         key=key,
         num_samples_per_batch=10,
         num_batches=1,
-        tangents_shape=(n,),
-        tangents_dtype=np.dtype(A),
+        sample_fun=fun,
     )
     expected = linalg.slogdet(A)[1]
     print_if_assert_fails = ("error", np.abs(received - expected), "target:", expected)
     assert np.allclose(received, expected, atol=1e-2, rtol=1e-2), print_if_assert_fails
```

