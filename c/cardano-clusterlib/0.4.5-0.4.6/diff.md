# Comparing `tmp/cardano-clusterlib-0.4.5.tar.gz` & `tmp/cardano-clusterlib-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-clusterlib-0.4.5.tar", last modified: Fri Apr 21 11:16:25 2023, max compression
+gzip compressed data, was "cardano-clusterlib-0.4.6.tar", last modified: Fri Apr 28 13:29:52 2023, max compression
```

## Comparing `cardano-clusterlib-0.4.5.tar` & `cardano-clusterlib-0.4.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.628790 cardano-clusterlib-0.4.5/.github/
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.628790 cardano-clusterlib-0.4.5/.github/workflows/
--rw-r--r--   0 sara      (1000) sara      (1000)      353 2022-09-08 20:06:48.000000 cardano-clusterlib-0.4.5/.github/workflows/repo_lint.yaml
--rw-rw-r--   0 sara      (1000) sara      (1000)      948 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/.gitignore
--rw-r--r--   0 sara      (1000) sara      (1000)      698 2022-09-26 14:22:34.000000 cardano-clusterlib-0.4.5/.markdownlint.yaml
--rw-r--r--   0 sara      (1000) sara      (1000)     1347 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/.pre-commit-config.yaml
--rw-rw-r--   0 sara      (1000) sara      (1000)     2523 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/.pylintrc
--rw-rw-r--   0 sara      (1000) sara      (1000)      318 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/.readthedocs.yaml
--rw-r--r--   0 sara      (1000) sara      (1000)     3267 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/CODE-OF-CONDUCT.md
--rw-r--r--   0 sara      (1000) sara      (1000)    11360 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/LICENSE
--rw-r--r--   0 sara      (1000) sara      (1000)     1279 2023-04-14 14:27:56.000000 cardano-clusterlib-0.4.5/Makefile
--rw-r--r--   0 sara      (1000) sara      (1000)     7853 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/PKG-INFO
--rw-r--r--   0 sara      (1000) sara      (1000)     7170 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/README.md
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/cardano_clusterlib/
--rw-rw-r--   0 sara      (1000) sara      (1000)      174 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/__init__.py
--rw-r--r--   0 sara      (1000) sara      (1000)     8119 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/address_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     2593 2022-08-23 09:17:09.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib.py
--rw-r--r--   0 sara      (1000) sara      (1000)     7791 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib_helpers.py
--rw-r--r--   0 sara      (1000) sara      (1000)    14563 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib_klass.py
--rw-r--r--   0 sara      (1000) sara      (1000)     1086 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/consts.py
--rw-r--r--   0 sara      (1000) sara      (1000)     1111 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/coverage.py
--rw-rw-r--   0 sara      (1000) sara      (1000)       36 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/exceptions.py
--rw-r--r--   0 sara      (1000) sara      (1000)     3799 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/genesis_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     7438 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/governance_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     1554 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/helpers.py
--rw-r--r--   0 sara      (1000) sara      (1000)     2815 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/key_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     6004 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/node_group.py
--rw-rw-r--   0 sara      (1000) sara      (1000)        0 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/py.typed
--rw-r--r--   0 sara      (1000) sara      (1000)    18201 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/query_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)    13370 2023-04-14 14:27:56.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/stake_address_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)    12907 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/stake_pool_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     6849 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/structs.py
--rw-r--r--   0 sara      (1000) sara      (1000)    62035 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/transaction_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)    44202 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/txtools.py
--rw-rw-r--   0 sara      (1000) sara      (1000)      608 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/types.py
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/
--rw-r--r--   0 sara      (1000) sara      (1000)     7853 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/PKG-INFO
--rw-r--r--   0 sara      (1000) sara      (1000)     1383 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/SOURCES.txt
--rw-r--r--   0 sara      (1000) sara      (1000)        1 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/dependency_links.txt
--rw-r--r--   0 sara      (1000) sara      (1000)        1 2022-08-03 14:24:31.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/not-zip-safe
--rw-r--r--   0 sara      (1000) sara      (1000)       19 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/requires.txt
--rw-r--r--   0 sara      (1000) sara      (1000)       19 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/top_level.txt
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/docs/
--rw-rw-r--   0 sara      (1000) sara      (1000)      740 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/docs/Makefile
--rw-r--r--   0 sara      (1000) sara      (1000)       36 2022-09-26 14:22:34.000000 cardano-clusterlib-0.4.5/docs/requirements.txt
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/docs/source/
--rw-r--r--   0 sara      (1000) sara      (1000)     3694 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/docs/source/cardano_clusterlib.rst
--rw-r--r--   0 sara      (1000) sara      (1000)     4112 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/docs/source/conf.py
--rw-rw-r--   0 sara      (1000) sara      (1000)      491 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/docs/source/index.rst
--rw-rw-r--   0 sara      (1000) sara      (1000)       95 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/docs/source/modules.rst
--rw-rw-r--   0 sara      (1000) sara      (1000)       31 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/docs/source/readme.rst
--rw-rw-r--   0 sara      (1000) sara      (1000)      236 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/mypy.ini
--rw-r--r--   0 sara      (1000) sara      (1000)      577 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/pyproject.toml
--rw-r--r--   0 sara      (1000) sara      (1000)       59 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.5/requirements-dev.txt
--rw-r--r--   0 sara      (1000) sara      (1000)     1128 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/setup.cfg
--rw-rw-r--   0 sara      (1000) sara      (1000)      163 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/setup.py
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/upgrading/
--rw-r--r--   0 sara      (1000) sara      (1000)     7363 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/upgrading/refactor_to_0_4_0rc1.sed
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.612864 cardano-clusterlib-0.4.6/.github/
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/.github/workflows/
+-rw-r--r--   0 sara      (1000) sara      (1000)      353 2022-09-08 20:06:48.000000 cardano-clusterlib-0.4.6/.github/workflows/repo_lint.yaml
+-rw-rw-r--   0 sara      (1000) sara      (1000)      948 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/.gitignore
+-rw-r--r--   0 sara      (1000) sara      (1000)      698 2022-09-26 14:22:34.000000 cardano-clusterlib-0.4.6/.markdownlint.yaml
+-rw-r--r--   0 sara      (1000) sara      (1000)     1347 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/.pre-commit-config.yaml
+-rw-rw-r--   0 sara      (1000) sara      (1000)     2523 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/.pylintrc
+-rw-rw-r--   0 sara      (1000) sara      (1000)      318 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/.readthedocs.yaml
+-rw-r--r--   0 sara      (1000) sara      (1000)     3267 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/CODE-OF-CONDUCT.md
+-rw-r--r--   0 sara      (1000) sara      (1000)    11360 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/LICENSE
+-rw-r--r--   0 sara      (1000) sara      (1000)     1279 2023-04-14 14:27:56.000000 cardano-clusterlib-0.4.6/Makefile
+-rw-r--r--   0 sara      (1000) sara      (1000)     7853 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/PKG-INFO
+-rw-r--r--   0 sara      (1000) sara      (1000)     7170 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/README.md
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/cardano_clusterlib/
+-rw-rw-r--   0 sara      (1000) sara      (1000)      174 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/__init__.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     8119 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/address_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     2593 2022-08-23 09:17:09.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     7791 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib_helpers.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    14563 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib_klass.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     1086 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/consts.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     1111 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/coverage.py
+-rw-rw-r--   0 sara      (1000) sara      (1000)       36 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/exceptions.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     3799 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/genesis_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     7438 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/governance_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     1554 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/helpers.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     2815 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/key_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     6004 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/node_group.py
+-rw-rw-r--   0 sara      (1000) sara      (1000)        0 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/py.typed
+-rw-r--r--   0 sara      (1000) sara      (1000)    18201 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/query_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    13370 2023-04-14 14:27:56.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/stake_address_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    12907 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/stake_pool_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     6849 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/structs.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    62487 2023-04-28 13:18:20.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/transaction_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    44202 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/txtools.py
+-rw-rw-r--   0 sara      (1000) sara      (1000)      608 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/types.py
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/
+-rw-r--r--   0 sara      (1000) sara      (1000)     7853 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/PKG-INFO
+-rw-r--r--   0 sara      (1000) sara      (1000)     1383 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/SOURCES.txt
+-rw-r--r--   0 sara      (1000) sara      (1000)        1 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/dependency_links.txt
+-rw-r--r--   0 sara      (1000) sara      (1000)        1 2022-08-03 14:24:31.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/not-zip-safe
+-rw-r--r--   0 sara      (1000) sara      (1000)       19 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/requires.txt
+-rw-r--r--   0 sara      (1000) sara      (1000)       19 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/top_level.txt
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/docs/
+-rw-rw-r--   0 sara      (1000) sara      (1000)      740 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/docs/Makefile
+-rw-r--r--   0 sara      (1000) sara      (1000)       36 2022-09-26 14:22:34.000000 cardano-clusterlib-0.4.6/docs/requirements.txt
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/docs/source/
+-rw-r--r--   0 sara      (1000) sara      (1000)     3694 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/docs/source/cardano_clusterlib.rst
+-rw-r--r--   0 sara      (1000) sara      (1000)     4112 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/docs/source/conf.py
+-rw-rw-r--   0 sara      (1000) sara      (1000)      491 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/docs/source/index.rst
+-rw-rw-r--   0 sara      (1000) sara      (1000)       95 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/docs/source/modules.rst
+-rw-rw-r--   0 sara      (1000) sara      (1000)       31 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/docs/source/readme.rst
+-rw-rw-r--   0 sara      (1000) sara      (1000)      236 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/mypy.ini
+-rw-r--r--   0 sara      (1000) sara      (1000)      577 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/pyproject.toml
+-rw-r--r--   0 sara      (1000) sara      (1000)       59 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.6/requirements-dev.txt
+-rw-r--r--   0 sara      (1000) sara      (1000)     1128 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/setup.cfg
+-rw-rw-r--   0 sara      (1000) sara      (1000)      163 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/setup.py
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/upgrading/
+-rw-r--r--   0 sara      (1000) sara      (1000)     7363 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/upgrading/refactor_to_0_4_0rc1.sed
```

### Comparing `cardano-clusterlib-0.4.5/.gitignore` & `cardano-clusterlib-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/.markdownlint.yaml` & `cardano-clusterlib-0.4.6/.markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/.pre-commit-config.yaml` & `cardano-clusterlib-0.4.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/.pylintrc` & `cardano-clusterlib-0.4.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/CODE-OF-CONDUCT.md` & `cardano-clusterlib-0.4.6/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/LICENSE` & `cardano-clusterlib-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/Makefile` & `cardano-clusterlib-0.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/PKG-INFO` & `cardano-clusterlib-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `cardano-clusterlib-0.4.5/README.md` & `cardano-clusterlib-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/address_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib_helpers.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib_helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib_klass.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib_klass.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/consts.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/consts.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/coverage.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/coverage.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/genesis_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/genesis_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/governance_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/governance_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/helpers.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/key_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/key_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/node_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/node_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/query_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/query_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/stake_address_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/stake_address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/stake_pool_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/stake_pool_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/structs.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/structs.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/transaction_group.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/transaction_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,14 +338,15 @@
         script_txins: structs.OptionalScriptTxIn = (),
         return_collateral_txouts: structs.OptionalTxOuts = (),
         total_collateral_amount: Optional[int] = None,
         mint: structs.OptionalMint = (),
         tx_files: Optional[structs.TxFiles] = None,
         complex_certs: structs.OptionalScriptCerts = (),
         fee: int = 0,
+        required_signers: OptionalFiles = (),
         ttl: Optional[int] = None,
         withdrawals: structs.OptionalTxOuts = (),
         script_withdrawals: structs.OptionalScriptWithdrawals = (),
         deposit: Optional[int] = None,
         invalid_hereafter: Optional[int] = None,
         invalid_before: Optional[int] = None,
         join_txouts: bool = True,
@@ -367,14 +368,16 @@
                 (optional).
             mint: An iterable of `Mint`, specifying script minting data (optional).
             tx_files: A `structs.TxFiles` tuple containing files needed for the transaction
                 (optional).
             complex_certs: An iterable of `ComplexCert`, specifying certificates script data
                 (optional).
             fee: A fee amount (optional).
+            required_signers: An iterable of filepaths of the signing keys whose signatures
+                are required (optional).
             ttl: A last block when the transaction is still valid
                 (deprecated in favor of `invalid_hereafter`, optional).
             withdrawals: A list (iterable) of `TxOuts`, specifying reward withdrawals (optional).
             script_withdrawals: An iterable of `ScriptWithdrawal`, specifying withdrawal script
                 data (optional).
             deposit: A deposit amount needed by the transaction (optional).
             invalid_hereafter: A last block when the transaction is still valid (optional).
@@ -423,14 +426,15 @@
             txins=collected_data.txins,
             readonly_reference_txins=readonly_reference_txins,
             script_txins=script_txins,
             return_collateral_txouts=return_collateral_txouts,
             total_collateral_amount=total_collateral_amount,
             mint=mint,
             complex_certs=complex_certs,
+            required_signers=required_signers,
             withdrawals=collected_data.withdrawals,
             script_withdrawals=collected_data.script_withdrawals,
             invalid_hereafter=invalid_hereafter or ttl,
             invalid_before=invalid_before,
             join_txouts=join_txouts,
         )
 
@@ -1094,14 +1098,15 @@
         script_txins: structs.OptionalScriptTxIn = (),
         return_collateral_txouts: structs.OptionalTxOuts = (),
         total_collateral_amount: Optional[int] = None,
         mint: structs.OptionalMint = (),
         tx_files: Optional[structs.TxFiles] = None,
         complex_certs: structs.OptionalScriptCerts = (),
         fee: Optional[int] = None,
+        required_signers: OptionalFiles = (),
         ttl: Optional[int] = None,
         withdrawals: structs.OptionalTxOuts = (),
         script_withdrawals: structs.OptionalScriptWithdrawals = (),
         deposit: Optional[int] = None,
         invalid_hereafter: Optional[int] = None,
         invalid_before: Optional[int] = None,
         witness_count_add: int = 0,
@@ -1132,14 +1137,16 @@
                 (optional).
             mint: An iterable of `Mint`, specifying script minting data (optional).
             tx_files: A `structs.TxFiles` tuple containing files needed for the transaction
                 (optional).
             complex_certs: An iterable of `ComplexCert`, specifying certificates script data
                 (optional).
             fee: A fee amount (optional).
+            required_signers: An iterable of filepaths of the signing keys whose signatures
+                are required (optional).
             ttl: A last block when the transaction is still valid
                 (deprecated in favor of `invalid_hereafter`, optional).
             withdrawals: A list (iterable) of `TxOuts`, specifying reward withdrawals (optional).
             script_withdrawals: An iterable of `ScriptWithdrawal`, specifying withdrawal script
                 data (optional).
             deposit: A deposit amount needed by the transaction (optional).
             invalid_hereafter: A last block when the transaction is still valid (optional).
@@ -1201,14 +1208,15 @@
             script_txins=script_txins,
             return_collateral_txouts=return_collateral_txouts,
             total_collateral_amount=total_collateral_amount,
             mint=mint,
             tx_files=tx_files,
             complex_certs=complex_certs,
             fee=fee,
+            required_signers=required_signers,
             withdrawals=withdrawals,
             script_withdrawals=script_withdrawals,
             deposit=deposit,
             invalid_hereafter=invalid_hereafter or ttl,
             invalid_before=invalid_before,
             join_txouts=join_txouts,
             destination_dir=destination_dir,
```

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/txtools.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/txtools.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib/types.py` & `cardano-clusterlib-0.4.6/cardano_clusterlib/types.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/PKG-INFO` & `cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/SOURCES.txt` & `cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/docs/Makefile` & `cardano-clusterlib-0.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/docs/source/cardano_clusterlib.rst` & `cardano-clusterlib-0.4.6/docs/source/cardano_clusterlib.rst`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/docs/source/conf.py` & `cardano-clusterlib-0.4.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/pyproject.toml` & `cardano-clusterlib-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/setup.cfg` & `cardano-clusterlib-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.5/upgrading/refactor_to_0_4_0rc1.sed` & `cardano-clusterlib-0.4.6/upgrading/refactor_to_0_4_0rc1.sed`

 * *Files identical despite different names*

