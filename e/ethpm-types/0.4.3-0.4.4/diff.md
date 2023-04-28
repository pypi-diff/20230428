# Comparing `tmp/ethpm-types-0.4.3.tar.gz` & `tmp/ethpm-types-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.4.3.tar", last modified: Fri Apr  7 18:12:22 2023, max compression
+gzip compressed data, was "ethpm-types-0.4.4.tar", last modified: Fri Apr 28 13:25:23 2023, max compression
```

## Comparing `ethpm-types-0.4.3.tar` & `ethpm-types-0.4.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.951879 ethpm-types-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-07 18:12:22.951879 ethpm-types-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.943879 ethpm-types-0.4.3/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.943879 ethpm-types-0.4.3/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 18:12:22.951879 ethpm-types-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.943879 ethpm-types-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.951879 ethpm-types-0.4.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/data/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/data/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/data/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/data/VyperContract.json
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_hexbytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_sourcemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.050359 ethpm-types-0.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-28 13:25:23.050359 ethpm-types-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.042358 ethpm-types-0.4.4/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.042358 ethpm-types-0.4.4/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 13:25:23.050359 ethpm-types-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.042358 ethpm-types-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.050359 ethpm-types-0.4.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/data/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/data/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/data/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/data/VyperContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_hexbytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_sourcemap.py
```

### Comparing `ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.github/release-drafter.yml` & `ethpm-types-0.4.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.github/workflows/commitlint.yaml` & `ethpm-types-0.4.4/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.github/workflows/docs.yaml` & `ethpm-types-0.4.4/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.github/workflows/prtitle.yaml` & `ethpm-types-0.4.4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.github/workflows/publish.yaml` & `ethpm-types-0.4.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.github/workflows/test.yaml` & `ethpm-types-0.4.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.gitignore` & `ethpm-types-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/.pre-commit-config.yaml` & `ethpm-types-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/CONTRIBUTING.md` & `ethpm-types-0.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/LICENSE` & `ethpm-types-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/PKG-INFO` & `ethpm-types-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.4.3
+Version: 0.4.4
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ethpm-types-0.4.3/README.md` & `ethpm-types-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/build_docs.py` & `ethpm-types-0.4.4/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/docs/_static/custom.css` & `ethpm-types-0.4.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/docs/_static/custom.js` & `ethpm-types-0.4.4/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/docs/_templates/layout.html` & `ethpm-types-0.4.4/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/docs/conf.py` & `ethpm-types-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/docs/favicon.ico` & `ethpm-types-0.4.4/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/docs/logo.gif` & `ethpm-types-0.4.4/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types/__init__.py` & `ethpm-types-0.4.4/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types/abi.py` & `ethpm-types-0.4.4/ethpm_types/abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types/ast.py` & `ethpm-types-0.4.4/ethpm_types/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             src (:class:`~ethpm_types.sourcemap.SourceMapItem`): The source map
               item to seek in the AST.
 
         Returns:
             Optional[``ASTNode``]: The matching node, if found, else ``None``.
         """
 
-        if self.src.start == src.start and self.src.length == src.length:
+        if self.src.start == src.start and (self.src.length or 0) == (src.length or 0):
             return self
 
         for child in self.children:
             node = child.get_node(src)
             if node:
                 return node
```

### Comparing `ethpm-types-0.4.3/ethpm_types/base.py` & `ethpm-types-0.4.4/ethpm_types/base.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types/contract_type.py` & `ethpm-types-0.4.4/ethpm_types/contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types/manifest.py` & `ethpm-types-0.4.4/ethpm_types/manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types/source.py` & `ethpm-types-0.4.4/ethpm_types/source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types/sourcemap.py` & `ethpm-types-0.4.4/ethpm_types/sourcemap.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types/utils.py` & `ethpm-types-0.4.4/ethpm_types/utils.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.4.4/ethpm_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.4.3
+Version: 0.4.4
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ethpm-types-0.4.3/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.4.4/ethpm_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.4.4/ethpm_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/pyproject.toml` & `ethpm-types-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/setup.py` & `ethpm-types-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/conftest.py` & `ethpm-types-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/data/OpenZeppelinContracts.json` & `ethpm-types-0.4.4/tests/data/OpenZeppelinContracts.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/data/SolidityContract.json` & `ethpm-types-0.4.4/tests/data/SolidityContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/data/TestStrategy.srcmap` & `ethpm-types-0.4.4/tests/data/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/data/VyperContract.json` & `ethpm-types-0.4.4/tests/data/VyperContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/test_ast.py` & `ethpm-types-0.4.4/tests/test_ast.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from ethpm_types import SourceMapItem
 from ethpm_types.ast import ASTNode
 
 AST_JSON = {
     "ast_type": "Module",
     "body": [
         {
@@ -91,15 +93,15 @@
                         "right": {
                             "ast_type": "Int",
                             "col_offset": 18,
                             "end_col_offset": 19,
                             "end_lineno": 7,
                             "lineno": 7,
                             "node_id": 13,
-                            "src": "111:1:0",
+                            "src": "111:0:0",
                             "value": 5,
                         },
                         "src": "104:8:0",
                     },
                 }
             ],
             "col_offset": 0,
@@ -148,7 +150,15 @@
     assert len(stmts) == 2
     assert stmts[0].ast_type == "arguments"
     assert stmts[1].ast_type == "arg"
     assert len(funcs) == 1
     assert node.get_defining_function((7, 11, 7, 14)) == funcs[0]
     assert node.get_defining_function([7, 11, 7, 14]) == funcs[0]
     assert node.get_defining_function((55, 11, 56, 14)) is None
+
+
+@pytest.mark.parametrize("length", (0, None))
+def test_ast_get_node_no_length(length):
+    node = ASTNode.parse_obj(AST_JSON)
+    idx = SourceMapItem(start=111, length=length, contract_id=None, jump_code="-")
+    actual = node.get_node(idx)
+    assert actual.ast_type == "Int"
```

### Comparing `ethpm-types-0.4.3/tests/test_cairo.py` & `ethpm-types-0.4.4/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/test_contract_type.py` & `ethpm-types-0.4.4/tests/test_contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/test_hexbytes.py` & `ethpm-types-0.4.4/tests/test_hexbytes.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/test_package_manifest.py` & `ethpm-types-0.4.4/tests/test_package_manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/test_pc_map.py` & `ethpm-types-0.4.4/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/test_schema_fuzzing.py` & `ethpm-types-0.4.4/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/test_source.py` & `ethpm-types-0.4.4/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.3/tests/test_sourcemap.py` & `ethpm-types-0.4.4/tests/test_sourcemap.py`

 * *Files identical despite different names*

