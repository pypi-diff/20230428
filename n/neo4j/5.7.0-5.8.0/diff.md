# Comparing `tmp/neo4j-5.7.0.tar.gz` & `tmp/neo4j-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j-5.7.0.tar", last modified: Fri Mar 31 10:07:21 2023, max compression
+gzip compressed data, was "neo4j-5.8.0.tar", last modified: Fri Apr 28 08:06:23 2023, max compression
```

## Comparing `neo4j-5.7.0.tar` & `neo4j-5.8.0.tar`

### file list

```diff
@@ -1,131 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.767443 neo4j-5.7.0/
--rw-r--r--   0 root         (0) root         (0)    11360 2023-03-31 10:04:59.000000 neo4j-5.7.0/LICENSE.APACHE2.txt
--rw-r--r--   0 root         (0) root         (0)     2762 2023-03-31 10:04:59.000000 neo4j-5.7.0/LICENSE.PYTHON.txt
--rw-r--r--   0 root         (0) root         (0)      423 2023-03-31 10:04:59.000000 neo4j-5.7.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-03-31 10:04:59.000000 neo4j-5.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      160 2023-03-31 10:04:59.000000 neo4j-5.7.0/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)     5946 2023-03-31 10:07:21.767443 neo4j-5.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5035 2023-03-31 10:04:59.000000 neo4j-5.7.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     2905 2023-03-31 10:07:21.000000 neo4j-5.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 10:07:21.767443 neo4j-5.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2442 2023-03-31 10:04:59.000000 neo4j-5.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.747443 neo4j-5.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.755443 neo4j-5.7.0/src/neo4j/
--rw-r--r--   0 root         (0) root         (0)     4572 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6621 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.755443 neo4j-5.7.0/src/neo4j/_async/
--rw-r--r--   0 root         (0) root         (0)      641 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/bookmark_manager.py
--rw-r--r--   0 root         (0) root         (0)    43585 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.755443 neo4j-5.7.0/src/neo4j/_async/io/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33210 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/io/_bolt.py
--rw-r--r--   0 root         (0) root         (0)    16109 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/io/_bolt3.py
--rw-r--r--   0 root         (0) root         (0)    22941 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/io/_bolt4.py
--rw-r--r--   0 root         (0) root         (0)    22436 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/io/_bolt5.py
--rw-r--r--   0 root         (0) root         (0)     9996 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/io/_common.py
--rw-r--r--   0 root         (0) root         (0)    33218 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/io/_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_async/work/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28075 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/work/result.py
--rw-r--r--   0 root         (0) root         (0)    26864 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/work/session.py
--rw-r--r--   0 root         (0) root         (0)    11289 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/work/transaction.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async/work/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_async_compat/
--rw-r--r--   0 root         (0) root         (0)      755 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async_compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14870 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async_compat/concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_async_compat/network/
--rw-r--r--   0 root         (0) root         (0)      872 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async_compat/network/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25858 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async_compat/network/_bolt_socket.py
--rw-r--r--   0 root         (0) root         (0)     6223 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async_compat/network/_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_async_compat/shims/
--rw-r--r--   0 root         (0) root         (0)     4939 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async_compat/shims/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_async_compat/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_codec/
--rw-r--r--   0 root         (0) root         (0)      641 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_codec/hydration/
--rw-r--r--   0 root         (0) root         (0)      898 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_codec/hydration/_interface/
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/_interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_codec/hydration/v1/
--rw-r--r--   0 root         (0) root         (0)      731 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7544 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/v1/hydration_handler.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/v1/spatial.py
--rw-r--r--   0 root         (0) root         (0)     8605 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/v1/temporal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.759443 neo4j-5.7.0/src/neo4j/_codec/hydration/v2/
--rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/v2/hydration_handler.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/hydration/v2/temporal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.763443 neo4j-5.7.0/src/neo4j/_codec/packstream/
--rw-r--r--   0 root         (0) root         (0)      707 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/packstream/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/packstream/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.763443 neo4j-5.7.0/src/neo4j/_codec/packstream/v1/
--rw-r--r--   0 root         (0) root         (0)    16696 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_codec/packstream/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18201 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_conf.py
--rw-r--r--   0 root         (0) root         (0)    11673 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_data.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_deadline.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3785 2023-03-31 10:07:19.000000 neo4j-5.7.0/src/neo4j/_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.763443 neo4j-5.7.0/src/neo4j/_optional_deps/
--rw-r--r--   0 root         (0) root         (0)      261 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_optional_deps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5907 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.763443 neo4j-5.7.0/src/neo4j/_spatial/
--rw-r--r--   0 root         (0) root         (0)     3871 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_spatial/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.763443 neo4j-5.7.0/src/neo4j/_sync/
--rw-r--r--   0 root         (0) root         (0)      641 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/bookmark_manager.py
--rw-r--r--   0 root         (0) root         (0)    42771 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.763443 neo4j-5.7.0/src/neo4j/_sync/io/
--rw-r--r--   0 root         (0) root         (0)     1154 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32755 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/io/_bolt.py
--rw-r--r--   0 root         (0) root         (0)    16000 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/io/_bolt3.py
--rw-r--r--   0 root         (0) root         (0)    22731 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/io/_bolt4.py
--rw-r--r--   0 root         (0) root         (0)    22271 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/io/_bolt5.py
--rw-r--r--   0 root         (0) root         (0)     9769 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/io/_common.py
--rw-r--r--   0 root         (0) root         (0)    32712 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/io/_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.763443 neo4j-5.7.0/src/neo4j/_sync/work/
--rw-r--r--   0 root         (0) root         (0)      988 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27584 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/work/result.py
--rw-r--r--   0 root         (0) root         (0)    26156 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/work/session.py
--rw-r--r--   0 root         (0) root         (0)    10873 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/work/transaction.py
--rw-r--r--   0 root         (0) root         (0)     7053 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_sync/work/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.767443 neo4j-5.7.0/src/neo4j/_work/
--rw-r--r--   0 root         (0) root         (0)     1030 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_work/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_work/eager_result.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_work/query.py
--rw-r--r--   0 root         (0) root         (0)    10365 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/_work/summary.py
--rw-r--r--   0 root         (0) root         (0)    10985 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/addressing.py
--rw-r--r--   0 root         (0) root         (0)    17950 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/api.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/conf.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/data.py
--rw-r--r--   0 root         (0) root         (0)     7802 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/debug.py
--rw-r--r--   0 root         (0) root         (0)    16536 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.767443 neo4j-5.7.0/src/neo4j/graph/
--rw-r--r--   0 root         (0) root         (0)    11098 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/meta.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/packstream.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/py.typed
--rw-r--r--   0 root         (0) root         (0)     1008 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.767443 neo4j-5.7.0/src/neo4j/spatial/
--rw-r--r--   0 root         (0) root         (0)     2081 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/spatial/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.767443 neo4j-5.7.0/src/neo4j/time/
--rw-r--r--   0 root         (0) root         (0)    94997 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/_arithmetic.py
--rw-r--r--   0 root         (0) root         (0)     2871 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/_clock_implementations.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/_metaclasses.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/arithmetic.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/clock_implementations.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/hydration.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/time/metaclasses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.767443 neo4j-5.7.0/src/neo4j/work/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1051 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/work/query.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-31 10:04:59.000000 neo4j-5.7.0/src/neo4j/work/summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 10:07:21.755443 neo4j-5.7.0/src/neo4j.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5946 2023-03-31 10:07:21.000000 neo4j-5.7.0/src/neo4j.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3045 2023-03-31 10:07:21.000000 neo4j-5.7.0/src/neo4j.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 10:07:21.000000 neo4j-5.7.0/src/neo4j.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-03-31 10:07:21.000000 neo4j-5.7.0/src/neo4j.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-31 10:07:21.000000 neo4j-5.7.0/src/neo4j.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.273798 neo4j-5.8.0/
+-rw-r--r--   0 root         (0) root         (0)    11360 2023-04-28 08:04:47.000000 neo4j-5.8.0/LICENSE.APACHE2.txt
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-04-28 08:04:47.000000 neo4j-5.8.0/LICENSE.PYTHON.txt
+-rw-r--r--   0 root         (0) root         (0)      423 2023-04-28 08:04:47.000000 neo4j-5.8.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-04-28 08:04:47.000000 neo4j-5.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      160 2023-04-28 08:04:47.000000 neo4j-5.8.0/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)     5946 2023-04-28 08:06:23.273798 neo4j-5.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-04-28 08:04:47.000000 neo4j-5.8.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-04-28 08:06:22.000000 neo4j-5.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 08:06:23.273798 neo4j-5.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-04-28 08:04:47.000000 neo4j-5.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.253798 neo4j-5.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.261798 neo4j-5.8.0/src/neo4j/
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6648 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.261798 neo4j-5.8.0/src/neo4j/_async/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6561 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/bookmark_manager.py
+-rw-r--r--   0 root         (0) root         (0)    49948 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.261798 neo4j-5.8.0/src/neo4j/_async/io/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35983 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/io/_bolt.py
+-rw-r--r--   0 root         (0) root         (0)    16740 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/io/_bolt3.py
+-rw-r--r--   0 root         (0) root         (0)    23378 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/io/_bolt4.py
+-rw-r--r--   0 root         (0) root         (0)    24676 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/io/_bolt5.py
+-rw-r--r--   0 root         (0) root         (0)    10670 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/io/_common.py
+-rw-r--r--   0 root         (0) root         (0)    38631 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/io/_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_async/work/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27782 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/work/result.py
+-rw-r--r--   0 root         (0) root         (0)    27600 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/work/session.py
+-rw-r--r--   0 root         (0) root         (0)    11289 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/work/transaction.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async/work/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_async_compat/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async_compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14870 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async_compat/concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_async_compat/network/
+-rw-r--r--   0 root         (0) root         (0)      872 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async_compat/network/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25841 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async_compat/network/_bolt_socket.py
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async_compat/network/_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_async_compat/shims/
+-rw-r--r--   0 root         (0) root         (0)     4939 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async_compat/shims/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_async_compat/util.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_auth_management.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_codec/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_codec/hydration/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_codec/hydration/_interface/
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/_interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_codec/hydration/v1/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7544 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/v1/hydration_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/v1/spatial.py
+-rw-r--r--   0 root         (0) root         (0)     8870 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/v1/temporal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_codec/hydration/v2/
+-rw-r--r--   0 root         (0) root         (0)      730 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/v2/hydration_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/hydration/v2/temporal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_codec/packstream/
+-rw-r--r--   0 root         (0) root         (0)      707 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/packstream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/packstream/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_codec/packstream/v1/
+-rw-r--r--   0 root         (0) root         (0)    16696 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_codec/packstream/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18295 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_conf.py
+-rw-r--r--   0 root         (0) root         (0)    11673 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_data.py
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_deadline.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-04-28 08:06:21.000000 neo4j-5.8.0/src/neo4j/_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_optional_deps/
+-rw-r--r--   0 root         (0) root         (0)      261 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_optional_deps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.265798 neo4j-5.8.0/src/neo4j/_spatial/
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_spatial/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.269798 neo4j-5.8.0/src/neo4j/_sync/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6377 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/bookmark_manager.py
+-rw-r--r--   0 root         (0) root         (0)    49052 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.269798 neo4j-5.8.0/src/neo4j/_sync/io/
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35506 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/io/_bolt.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/io/_bolt3.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/io/_bolt4.py
+-rw-r--r--   0 root         (0) root         (0)    24509 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/io/_bolt5.py
+-rw-r--r--   0 root         (0) root         (0)    10393 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/io/_common.py
+-rw-r--r--   0 root         (0) root         (0)    37987 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/io/_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.269798 neo4j-5.8.0/src/neo4j/_sync/work/
+-rw-r--r--   0 root         (0) root         (0)      988 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27291 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/work/result.py
+-rw-r--r--   0 root         (0) root         (0)    26864 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/work/session.py
+-rw-r--r--   0 root         (0) root         (0)    10873 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/work/transaction.py
+-rw-r--r--   0 root         (0) root         (0)     7268 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_sync/work/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.269798 neo4j-5.8.0/src/neo4j/_work/
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_work/eager_result.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_work/query.py
+-rw-r--r--   0 root         (0) root         (0)    10365 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/_work/summary.py
+-rw-r--r--   0 root         (0) root         (0)    10985 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/addressing.py
+-rw-r--r--   0 root         (0) root         (0)    18240 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/api.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/data.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/debug.py
+-rw-r--r--   0 root         (0) root         (0)    17262 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.269798 neo4j-5.8.0/src/neo4j/graph/
+-rw-r--r--   0 root         (0) root         (0)    11098 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/meta.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/packstream.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.269798 neo4j-5.8.0/src/neo4j/spatial/
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/spatial/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.273798 neo4j-5.8.0/src/neo4j/time/
+-rw-r--r--   0 root         (0) root         (0)    94998 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/_arithmetic.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/_clock_implementations.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/_metaclasses.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/arithmetic.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/clock_implementations.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/hydration.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/time/metaclasses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.273798 neo4j-5.8.0/src/neo4j/work/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/work/query.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-04-28 08:04:47.000000 neo4j-5.8.0/src/neo4j/work/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:23.261798 neo4j-5.8.0/src/neo4j.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5946 2023-04-28 08:06:23.000000 neo4j-5.8.0/src/neo4j.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-04-28 08:06:23.000000 neo4j-5.8.0/src/neo4j.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 08:06:23.000000 neo4j-5.8.0/src/neo4j.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-28 08:06:23.000000 neo4j-5.8.0/src/neo4j.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 08:06:23.000000 neo4j-5.8.0/src/neo4j.egg-info/top_level.txt
```

### Comparing `neo4j-5.7.0/LICENSE.APACHE2.txt` & `neo4j-5.8.0/LICENSE.APACHE2.txt`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/LICENSE.PYTHON.txt` & `neo4j-5.8.0/LICENSE.PYTHON.txt`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/PKG-INFO` & `neo4j-5.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j
-Version: 5.7.0
+Version: 5.8.0
 Summary: Neo4j Bolt driver for Python
 Author-email: "Neo4j, Inc." <drivers@neo4j.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/neo4j/neo4j-python-driver
 Keywords: neo4j,graph,database
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neo4j-5.7.0/README.rst` & `neo4j-5.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/pyproject.toml` & `neo4j-5.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 [project.urls]
 Homepage = "https://github.com/neo4j/neo4j-python-driver"
 
 [project.optional-dependencies]
 numpy = ["numpy >= 1.7.0, < 2.0.0"]
 pandas = [
-    "pandas >= 1.1.0, < 2.0.0",
+    "pandas >= 1.1.0, < 3.0.0",
     "numpy >= 1.7.0, < 2.0.0",
 ]
 
 [build-system]
 requires = [
     "setuptools~=65.6",
     "tomlkit~=0.11.6",
```

### Comparing `neo4j-5.7.0/setup.py` & `neo4j-5.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/__init__.py` & `neo4j-5.8.0/src/neo4j/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 )
 from ._data import Record
 from ._meta import (
     deprecated_package as _deprecated_package,
     deprecation_warn as _deprecation_warn,
     ExperimentalWarning,
     get_user_agent,
+    PreviewWarning,
     version as __version__,
 )
 from ._sync.driver import (
     BoltDriver,
     Driver,
     GraphDatabase,
     Neo4jDriver,
@@ -136,19 +137,21 @@
     "ManagedTransaction",
     "NotificationMinimumSeverity",
     "Neo4jDriver",
     "NotificationCategory",
     "NotificationFilter",
     "NotificationSeverity",
     "PoolConfig",
+    "PreviewWarning",
     "Query",
     "READ_ACCESS",
     "Record",
     "Result",
     "ResultSummary",
+    "RenewableAuth",
     "RoutingControl",
     "ServerInfo",
     "Session",
     "SessionConfig",
     "SummaryCounters",
     "SummaryNotification",
     "SummaryNotificationPosition",
```

### Comparing `neo4j-5.7.0/src/neo4j/_api.py` & `neo4j-5.8.0/src/neo4j/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,29 +204,30 @@
 
 class RoutingControl(str, Enum):
     """Selection which cluster members to route a query connect to.
 
     Inherits from :class:`str` and :class:`Enum`. Every driver API accepting a
     :class:`.RoutingControl` value will also accept a string
 
-        >>> RoutingControl.READERS == "r"
+        >>> RoutingControl.READ == "r"
         True
-        >>> RoutingControl.WRITERS == "w"
+        >>> RoutingControl.WRITE == "w"
         True
 
-    **This is experimental.**
-    It might be changed or removed any time even without prior notice.
-
     .. seealso::
         :attr:`.AsyncDriver.execute_query`, :attr:`.Driver.execute_query`
 
     .. versionadded:: 5.5
+
+    .. versionchanged:: 5.8
+        * renamed ``READERS`` to ``READ`` and ``WRITERS`` to ``WRITE``
+        * stabilized from experimental
     """
-    READERS = "r"
-    WRITERS = "w"
+    READ = "r"
+    WRITE = "w"
 
 
 if t.TYPE_CHECKING:
     T_RoutingControl = t.Union[
         RoutingControl,
         te.Literal["r", "w"],
     ]
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/__init__.py` & `neo4j-5.8.0/src/neo4j/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async/bookmark_manager.py` & `neo4j-5.8.0/src/neo4j/_async/bookmark_manager.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async/driver.py` & `neo4j-5.8.0/src/neo4j/_async/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,30 @@
     import typing_extensions as te
 
     from .._api import (
         T_NotificationDisabledCategory,
         T_NotificationMinimumSeverity,
     )
 
-
 from .._api import RoutingControl
 from .._async_compat.util import AsyncUtil
 from .._conf import (
     Config,
     PoolConfig,
     SessionConfig,
     TrustAll,
     TrustStore,
     WorkspaceConfig,
 )
 from .._meta import (
     deprecation_warn,
-    experimental,
     experimental_warn,
-    ExperimentalWarning,
+    preview,
+    preview_warn,
+    PreviewWarning,
     unclosed_resource_warn,
 )
 from .._work import EagerResult
 from ..addressing import Address
 from ..api import (
     AsyncBookmarkManager,
     Auth,
@@ -70,14 +70,19 @@
     URI_SCHEME_BOLT,
     URI_SCHEME_BOLT_SECURE,
     URI_SCHEME_BOLT_SELF_SIGNED_CERTIFICATE,
     URI_SCHEME_NEO4J,
     URI_SCHEME_NEO4J_SECURE,
     URI_SCHEME_NEO4J_SELF_SIGNED_CERTIFICATE,
 )
+from ..auth_management import (
+    AsyncAuthManager,
+    AsyncAuthManagers,
+)
+from ..exceptions import Neo4jError
 from .bookmark_manager import (
     AsyncNeo4jBookmarkManager,
     TBmConsumer as _TBmConsumer,
     TBmSupplier as _TBmSupplier,
 )
 from .work import (
     AsyncManagedTransaction,
@@ -89,14 +94,15 @@
 if t.TYPE_CHECKING:
     import ssl
     from enum import Enum
 
     import typing_extensions as te
 
     from .._api import T_RoutingControl
+    from ..api import _TAuth
 
 
     class _DefaultEnum(Enum):
         default = "default"
 
     _default = _DefaultEnum.default
 
@@ -113,15 +119,21 @@
     if t.TYPE_CHECKING:
 
         @classmethod
         def driver(
             cls,
             uri: str,
             *,
-            auth: t.Union[t.Tuple[t.Any, t.Any], Auth, None] = ...,
+            auth: t.Union[
+                # work around https://github.com/sphinx-doc/sphinx/pull/10880
+                # make sure TAuth is resolved in the docs
+                # TAuth,
+                t.Union[t.Tuple[t.Any, t.Any], Auth, None],
+                AsyncAuthManager,
+            ] = ...,
             max_connection_lifetime: float = ...,
             max_connection_pool_size: int = ...,
             connection_timeout: float = ...,
             trust: t.Union[
                 te.Literal["TRUST_ALL_CERTIFICATES"],
                 te.Literal["TRUST_SYSTEM_CA_SIGNED_CERTIFICATES"]
             ] = ...,
@@ -157,15 +169,21 @@
             ...
 
     else:
 
         @classmethod
         def driver(
             cls, uri: str, *,
-            auth: t.Union[t.Tuple[t.Any, t.Any], Auth, None] = None,
+            auth: t.Union[
+                # work around https://github.com/sphinx-doc/sphinx/pull/10880
+                # make sure TAuth is resolved in the docs
+                # TAuth,
+                t.Union[t.Tuple[t.Any, t.Any], Auth, None],
+                AsyncAuthManager,
+            ] = None,
             **config
         ) -> AsyncDriver:
             """Create a driver.
 
             :param uri: the connection URI for the driver,
                 see :ref:`async-uri-ref` for available URIs.
             :param auth: the authentication details,
@@ -173,14 +191,26 @@
             :param config: driver configuration key-word arguments,
                 see :ref:`async-driver-configuration-ref` for available
                 key-word arguments.
             """
 
             driver_type, security_type, parsed = parse_neo4j_uri(uri)
 
+            if not isinstance(auth, AsyncAuthManager):
+                with warnings.catch_warnings():
+                    warnings.filterwarnings(
+                        "ignore", message=r".*\bAuth managers\b.*",
+                        category=PreviewWarning
+                    )
+                    auth = AsyncAuthManagers.static(auth)
+            else:
+                preview_warn("Auth managers are a preview feature.",
+                             stack_level=2)
+            config["auth"] = auth
+
             # TODO: 6.0 - remove "trust" config option
             if "trust" in config.keys():
                 if config["trust"] not in (
                     TRUST_ALL_CERTIFICATES,
                     TRUST_SYSTEM_CA_SIGNED_CERTIFICATES
                 ):
                     from ..exceptions import ConfigurationError
@@ -250,25 +280,21 @@
                         stack_level=2
                     )
                     # TODO: 6.0 - raise instead of warning
                     # raise ValueError(
                     #     'Routing parameters are not supported with scheme '
                     #     '"bolt". Given URI "{}".'.format(uri)
                     # )
-                return cls.bolt_driver(parsed.netloc, auth=auth, **config)
+                return cls.bolt_driver(parsed.netloc, **config)
             # else driver_type == DRIVER_NEO4J
             routing_context = parse_routing_context(parsed.query)
-            return cls.neo4j_driver(parsed.netloc, auth=auth,
+            return cls.neo4j_driver(parsed.netloc,
                                     routing_context=routing_context, **config)
 
     @classmethod
-    @experimental(
-        "The bookmark manager feature is experimental. "
-        "It might be changed or removed any time even without prior notice."
-    )
     def bookmark_manager(
         cls,
         initial_bookmarks: t.Union[None, Bookmarks, t.Iterable[str]] = None,
         bookmarks_supplier: t.Optional[_TBmSupplier] = None,
         bookmarks_consumer: t.Optional[_TBmConsumer] = None
     ) -> AsyncBookmarkManager:
         """Create a :class:`.AsyncBookmarkManager` with default implementation.
@@ -321,65 +347,64 @@
             Function which will be called whenever the set of bookmarks
             handled by the bookmark manager gets updated with the new
             internal bookmark set. It will receive the new set of bookmarks
             as a :class:`.Bookmarks` object and return :data:`None`.
 
         :returns: A default implementation of :class:`AsyncBookmarkManager`.
 
-        **This is experimental.** (See :ref:`filter-warnings-ref`)
-        It might be changed or removed any time even without prior notice.
-
         .. versionadded:: 5.0
 
         .. versionchanged:: 5.3
             The bookmark manager no longer tracks bookmarks per database.
             This effectively changes the signature of almost all bookmark
             manager related methods:
 
             * ``initial_bookmarks`` is no longer a mapping from database name
               to bookmarks but plain bookmarks.
             * ``bookmarks_supplier`` no longer receives the database name as
               an argument.
             * ``bookmarks_consumer`` no longer receives the database name as
               an argument.
+
+        .. versionchanged:: 5.8 stabilized from experimental
         """
         return AsyncNeo4jBookmarkManager(
             initial_bookmarks=initial_bookmarks,
             bookmarks_supplier=bookmarks_supplier,
             bookmarks_consumer=bookmarks_consumer
         )
 
     @classmethod
-    def bolt_driver(cls, target, *, auth=None, **config):
+    def bolt_driver(cls, target, **config):
         """ Create a driver for direct Bolt server access that uses
         socket I/O and thread-based concurrency.
         """
         from .._exceptions import (
             BoltHandshakeError,
             BoltSecurityError,
         )
 
         try:
-            return AsyncBoltDriver.open(target, auth=auth, **config)
+            return AsyncBoltDriver.open(target, **config)
         except (BoltHandshakeError, BoltSecurityError) as error:
             from ..exceptions import ServiceUnavailable
             raise ServiceUnavailable(str(error)) from error
 
     @classmethod
-    def neo4j_driver(cls, *targets, auth=None, routing_context=None, **config):
+    def neo4j_driver(cls, *targets, routing_context=None, **config):
         """ Create a driver for routing-capable Neo4j service access
         that uses socket I/O and thread-based concurrency.
         """
         from .._exceptions import (
             BoltHandshakeError,
             BoltSecurityError,
         )
 
         try:
-            return AsyncNeo4jDriver.open(*targets, auth=auth, routing_context=routing_context, **config)
+            return AsyncNeo4jDriver.open(*targets, routing_context=routing_context, **config)
         except (BoltHandshakeError, BoltSecurityError) as error:
             from ..exceptions import ServiceUnavailable
             raise ServiceUnavailable(str(error)) from error
 
 
 class _Direct:
 
@@ -444,20 +469,15 @@
     _closed = False
 
     def __init__(self, pool, default_workspace_config):
         assert pool is not None
         assert default_workspace_config is not None
         self._pool = pool
         self._default_workspace_config = default_workspace_config
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore",
-                                    message=r".*\bbookmark manager\b.*",
-                                    category=ExperimentalWarning)
-            self._query_bookmark_manager = \
-                AsyncGraphDatabase.bookmark_manager()
+        self._query_bookmark_manager = AsyncGraphDatabase.bookmark_manager()
 
     async def __aenter__(self) -> AsyncDriver:
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
 
@@ -478,14 +498,17 @@
 
     @property
     def encrypted(self) -> bool:
         """Indicate whether the driver was configured to use encryption."""
         return bool(self._pool.pool_config.encrypted)
 
     def _prepare_session_config(self, **config):
+        if "auth" in config:
+            preview_warn("User switching is a preview feature.",
+                         stack_level=3)
         _normalize_notifications_config(config)
         return config
 
     if t.TYPE_CHECKING:
 
         def session(
             self,
@@ -495,14 +518,15 @@
             database: t.Optional[str] = ...,
             fetch_size: int = ...,
             impersonated_user: t.Optional[str] = ...,
             bookmarks: t.Union[t.Iterable[str], Bookmarks, None] = ...,
             default_access_mode: str = ...,
             bookmark_manager: t.Union[AsyncBookmarkManager,
                                       BookmarkManager, None] = ...,
+            auth: _TAuth = ...,
             notifications_min_severity: t.Optional[
                 T_NotificationMinimumSeverity
             ] = ...,
             notifications_disabled_categories: t.Optional[
                 t.Iterable[T_NotificationDisabledCategory]
             ] = ...,
 
@@ -537,62 +561,61 @@
             raise
         self._closed = True
 
     # overloads to work around https://github.com/python/mypy/issues/3737
     @t.overload
     async def execute_query(
         self,
-        query_: str,
+        query_: te.LiteralString,
         parameters_: t.Optional[t.Dict[str, t.Any]] = None,
-        routing_: T_RoutingControl = RoutingControl.WRITERS,
+        routing_: T_RoutingControl = RoutingControl.WRITE,
         database_: t.Optional[str] = None,
         impersonated_user_: t.Optional[str] = None,
         bookmark_manager_: t.Union[
             AsyncBookmarkManager, BookmarkManager, None
         ] = ...,
+        auth_: _TAuth = None,
         result_transformer_: t.Callable[
             [AsyncResult], t.Awaitable[EagerResult]
         ] = ...,
         **kwargs: t.Any
     ) -> EagerResult:
         ...
 
     @t.overload
     async def execute_query(
         self,
-        query_: str,
+        query_: te.LiteralString,
         parameters_: t.Optional[t.Dict[str, t.Any]] = None,
-        routing_: T_RoutingControl = RoutingControl.WRITERS,
+        routing_: T_RoutingControl = RoutingControl.WRITE,
         database_: t.Optional[str] = None,
         impersonated_user_: t.Optional[str] = None,
         bookmark_manager_: t.Union[
             AsyncBookmarkManager, BookmarkManager, None
         ] = ...,
+        auth_: _TAuth = None,
         result_transformer_: t.Callable[
             [AsyncResult], t.Awaitable[_T]
         ] = ...,
         **kwargs: t.Any
     ) -> _T:
         ...
 
-    @experimental(
-        "Driver.execute_query is experimental. "
-        "It might be changed or removed any time even without prior notice."
-    )
     async def execute_query(
         self,
-        query_: str,
+        query_: te.LiteralString,
         parameters_: t.Optional[t.Dict[str, t.Any]] = None,
-        routing_: T_RoutingControl = RoutingControl.WRITERS,
+        routing_: T_RoutingControl = RoutingControl.WRITE,
         database_: t.Optional[str] = None,
         impersonated_user_: t.Optional[str] = None,
         bookmark_manager_: t.Union[
             AsyncBookmarkManager, BookmarkManager, None,
             te.Literal[_DefaultEnum.default]
         ] = _default,
+        auth_: _TAuth = None,
         result_transformer_: t.Callable[
             [AsyncResult], t.Awaitable[t.Any]
         ] = AsyncResult.to_eager_result,
         **kwargs: t.Any
     ) -> t.Any:
         """Execute a query in a transaction function and return all results.
 
@@ -606,43 +629,44 @@
         ``CALL {} IN TRANSACTIONS`` or the older ``USING PERIODIC COMMIT``
         will not work (use :meth:`AsyncSession.run` for these).
 
         The method is roughly equivalent to::
 
             async def execute_query(
                 query_, parameters_, routing_, database_, impersonated_user_,
-                bookmark_manager_, result_transformer_, **kwargs
+                bookmark_manager_, auth_, result_transformer_, **kwargs
             ):
                 async def work(tx):
                     result = await tx.run(query_, parameters_, **kwargs)
                     return await result_transformer_(result)
 
                 async with driver.session(
                     database=database_,
                     impersonated_user=impersonated_user_,
                     bookmark_manager=bookmark_manager_,
+                    auth=auth_,
                 ) as session:
-                    if routing_ == RoutingControl.WRITERS:
+                    if routing_ == RoutingControl.WRITE:
                         return await session.execute_write(work)
-                    elif routing_ == RoutingControl.READERS:
+                    elif routing_ == RoutingControl.READ:
                         return await session.execute_read(work)
 
         Usage example::
 
             from typing import List
 
             import neo4j
 
 
             async def example(driver: neo4j.AsyncDriver) -> List[str]:
                 \"""Get the name of all 42 year-olds.\"""
                 records, summary, keys = await driver.execute_query(
                     "MATCH (p:Person {age: $age}) RETURN p.name",
                     {"age": 42},
-                    routing_=neo4j.RoutingControl.READERS,  # or just "r"
+                    routing_=neo4j.RoutingControl.READ,  # or just "r"
                     database_="neo4j",
                 )
                 assert keys == ["p.name"]  # not needed, just for illustration
                 # log_summary(summary)  # log some metadata
                 return [str(record["p.name"]) for record in records]
                 # or: return [str(record[0]) for record in records]
                 # or even: return list(map(lambda r: str(r[0]), records))
@@ -651,21 +675,22 @@
 
             import neo4j
 
 
             async def example(driver: neo4j.AsyncDriver) -> int:
                 \"""Call all young people "My dear" and get their count.\"""
                 record = await driver.execute_query(
-                    "MATCH (p:Person) WHERE p.age <= 15 "
+                    "MATCH (p:Person) WHERE p.age <= $age "
                     "SET p.nickname = 'My dear' "
                     "RETURN count(*)",
                     # optional routing parameter, as write is default
-                    # routing_=neo4j.RoutingControl.WRITERS,  # or just "w",
+                    # routing_=neo4j.RoutingControl.WRITE,  # or just "w",
                     database_="neo4j",
                     result_transformer_=neo4j.AsyncResult.single,
+                    age=15,
                 )
                 assert record is not None  # for typechecking and illustration
                 count = record[0]
                 assert isinstance(count, int)
                 return count
 
         :param query_: cypher query to execute
@@ -694,14 +719,28 @@
             This means that all query will be executed in the security context
             of the impersonated user. For this, the user for which the
             :class:`Driver` has been created needs to have the appropriate
             permissions.
 
             See also the Session config :ref:`impersonated-user-ref`.
         :type impersonated_user_: typing.Optional[str]
+        :param auth_:
+            Authentication information to use for this query.
+
+            By default, the driver configuration is used.
+
+            **This is a preview** (see :ref:`filter-warnings-ref`).
+            It might be changed without following the deprecation policy.
+            See also
+            https://github.com/neo4j/neo4j-python-driver/wiki/preview-features
+
+            See also the Session config :ref:`session-auth-ref`.
+        :type auth_: typing.Union[
+            typing.Tuple[typing.Any, typing.Any], neo4j.Auth, None
+        ]
         :param result_transformer_:
             A function that gets passed the :class:`neo4j.AsyncResult` object
             resulting from the query and converts it to a different type. The
             result of the transformer function is returned by this method.
 
             .. warning::
 
@@ -764,32 +803,34 @@
             Specify a bookmark manager to use.
 
             If present, the bookmark manager is used to keep the query causally
             consistent with all work executed using the same bookmark manager.
 
             Defaults to the driver's :attr:`.query_bookmark_manager`.
 
-            Pass :const:`None` to disable causal consistency.
+            Pass :data:`None` to disable causal consistency.
         :type bookmark_manager_:
             typing.Union[neo4j.AsyncBookmarkManager, neo4j.BookmarkManager,
                          None]
         :param kwargs: additional keyword parameters. None of these can end
             with a single underscore. This is to avoid collisions with the
             keyword configuration parameters of this method. If you need to
             pass such a parameter, use the ``parameters_`` parameter instead.
-            These take precedence over parameters passed as ``parameters_``.
+            Parameters passed as kwargs take precedence over those passed in
+            ``parameters_``.
         :type kwargs: typing.Any
 
         :returns: the result of the ``result_transformer``
         :rtype: T
 
-        **This is experimental.** (See :ref:`filter-warnings-ref`)
-        It might be changed or removed any time even without prior notice.
-
         .. versionadded:: 5.5
+
+        .. versionchanged:: 5.8
+            * Added the ``auth_`` parameter.
+            * Stabilized from experimental.
         """
         invalid_kwargs = [k for k in kwargs if
                           k[-2:-1] != "_" and k[-1:] == "_"]
         if invalid_kwargs:
             raise ValueError(
                 "keyword parameters must not end with a single '_'. Found: %r"
                 "\nYou either misspelled an existing configuration parameter "
@@ -801,37 +842,34 @@
 
         if bookmark_manager_ is _default:
             bookmark_manager_ = self._query_bookmark_manager
         assert bookmark_manager_ is not _default
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore",
-                                    message=r".*\bbookmark_manager\b.*",
-                                    category=ExperimentalWarning)
+                                    message=r"^User switching\b.*",
+                                    category=PreviewWarning)
             session = self.session(database=database_,
                                    impersonated_user=impersonated_user_,
-                                   bookmark_manager=bookmark_manager_)
+                                   bookmark_manager=bookmark_manager_,
+                                   auth=auth_)
         async with session:
-            if routing_ == RoutingControl.WRITERS:
+            if routing_ == RoutingControl.WRITE:
                 executor = session.execute_write
-            elif routing_ == RoutingControl.READERS:
+            elif routing_ == RoutingControl.READ:
                 executor = session.execute_read
             else:
                 raise ValueError("Invalid routing control value: %r"
                                  % routing_)
             return await executor(
                 _work, query_, parameters, result_transformer_
             )
 
     @property
-    @experimental(
-        "Driver.query_bookmark_manager is experimental. "
-        "It might be changed or removed any time even without prior notice."
-    )
-    def query_bookmark_manager(self) -> AsyncBookmarkManager:
+    def execute_query_bookmark_manager(self) -> AsyncBookmarkManager:
         """The driver's default query bookmark manager.
 
         This is the default :class:`AsyncBookmarkManager` used by
         :meth:`.execute_query`. This can be used to causally chain
         :meth:`.execute_query` calls and sessions. Example::
 
             async def example(driver: neo4j.AsyncDriver) -> None:
@@ -842,18 +880,20 @@
                     # every query inside this session will be causally chained
                     # (i.e., can read what was written by <QUERY 1>)
                     await session.run("<QUERY 2>")
                 # subsequent execute_query calls will be causally chained
                 # (i.e., can read what was written by <QUERY 2>)
                 await driver.execute_query("<QUERY 3>")
 
-        **This is experimental.** (See :ref:`filter-warnings-ref`)
-        It might be changed or removed any time even without prior notice.
-
         .. versionadded:: 5.5
+
+        .. versionchanged:: 5.8
+            * Renamed from ``query_bookmark_manager`` to
+              ``execute_query_bookmark_manager``.
+            * Stabilized from experimental.
         """
         return self._query_bookmark_manager
 
     if t.TYPE_CHECKING:
 
         async def verify_connectivity(
             self,
@@ -866,14 +906,15 @@
             database: t.Optional[str] = ...,
             fetch_size: int = ...,
             impersonated_user: t.Optional[str] = ...,
             bookmarks: t.Union[t.Iterable[str], Bookmarks, None] = ...,
             default_access_mode: str = ...,
             bookmark_manager: t.Union[AsyncBookmarkManager,
                                       BookmarkManager, None] = ...,
+            auth: t.Union[Auth, t.Tuple[t.Any, t.Any]] = ...,
             notifications_min_severity: t.Optional[
                 T_NotificationMinimumSeverity
             ] = ...,
             notifications_disabled_categories: t.Optional[
                 t.Iterable[T_NotificationDisabledCategory]
             ] = ...,
 
@@ -882,15 +923,14 @@
             retry_delay_multiplier: float = ...,
             retry_delay_jitter_factor: float = ...
         ) -> None:
             ...
 
     else:
 
-        # TODO: 6.0 - remove config argument
         async def verify_connectivity(self, **config) -> None:
             """Verify that the driver can establish a connection to the server.
 
             This verifies if the driver can establish a reading connection to a
             remote server or a cluster. Some data will be exchanged.
 
             .. note::
@@ -901,15 +941,15 @@
                 :meth:`session`.
 
                 .. warning::
                     All configuration key-word arguments are experimental.
                     They might be changed or removed in any future version
                     without prior notice.
 
-            :raises DriverError: if the driver cannot connect to the remote.
+            :raises Exception: if the driver cannot connect to the remote.
                 Use the exception to further understand the cause of the
                 connectivity problem.
 
             .. versionchanged:: 5.0
                 The undocumented return value has been removed.
                 If you need information about the remote server, use
                 :meth:`get_server_info` instead.
@@ -917,16 +957,15 @@
             if config:
                 experimental_warn(
                     "All configuration key-word arguments to "
                     "verify_connectivity() are experimental. They might be "
                     "changed or removed in any future version without prior "
                     "notice."
                 )
-            async with self.session(**config) as session:
-                await session._get_server_info()
+            await self._get_server_info()
 
     if t.TYPE_CHECKING:
 
         async def get_server_info(
             self,
             *,
             # all arguments are experimental
@@ -937,14 +976,15 @@
             database: t.Optional[str] = ...,
             fetch_size: int = ...,
             impersonated_user: t.Optional[str] = ...,
             bookmarks: t.Union[t.Iterable[str], Bookmarks, None] = ...,
             default_access_mode: str = ...,
             bookmark_manager: t.Union[AsyncBookmarkManager,
                                       BookmarkManager, None] = ...,
+            auth: t.Union[Auth, t.Tuple[t.Any, t.Any]] = ...,
             notifications_min_severity: t.Optional[
                 T_NotificationMinimumSeverity
             ] = ...,
             notifications_disabled_categories: t.Optional[
                 t.Iterable[T_NotificationDisabledCategory]
             ] = ...,
 
@@ -975,60 +1015,182 @@
                 :meth:`session`.
 
                 .. warning::
                     All configuration key-word arguments are experimental.
                     They might be changed or removed in any future version
                     without prior notice.
 
-            :raises DriverError: if the driver cannot connect to the remote.
+            :raises Exception: if the driver cannot connect to the remote.
                 Use the exception to further understand the cause of the
                 connectivity problem.
 
             .. versionadded:: 5.0
             """
             if config:
                 experimental_warn(
                     "All configuration key-word arguments to "
-                    "verify_connectivity() are experimental. They might be "
+                    "get_server_info() are experimental. They might be "
                     "changed or removed in any future version without prior "
                     "notice."
                 )
-            async with self.session(**config) as session:
-                return await session._get_server_info()
+            return await self._get_server_info()
 
-    @experimental("Feature support query, based on Bolt protocol version and Neo4j server version will change in the future.")
     async def supports_multi_db(self) -> bool:
         """ Check if the server or cluster supports multi-databases.
 
         :returns: Returns true if the server or cluster the driver connects to
             supports multi-databases, otherwise false.
 
         .. note::
-            Feature support query, based on Bolt Protocol Version and Neo4j
-            server version will change in the future.
+            Feature support query based solely on the Bolt protocol version.
+            The feature might still be disabled on the server side even if this
+            function return :const:`True`. It just guarantees that the driver
+            won't throw a :exc:`ConfigurationError` when trying to use this
+            driver feature.
         """
         async with self.session() as session:
             await session._connect(READ_ACCESS)
             assert session._connection
             return session._connection.supports_multiple_databases
 
+    if t.TYPE_CHECKING:
+
+        async def verify_authentication(
+            self,
+            auth: t.Union[Auth, t.Tuple[t.Any, t.Any], None] = None,
+            # all other arguments are experimental
+            # they may be change or removed any time without prior notice
+            session_connection_timeout: float = ...,
+            connection_acquisition_timeout: float = ...,
+            max_transaction_retry_time: float = ...,
+            database: t.Optional[str] = ...,
+            fetch_size: int = ...,
+            impersonated_user: t.Optional[str] = ...,
+            bookmarks: t.Union[t.Iterable[str], Bookmarks, None] = ...,
+            default_access_mode: str = ...,
+            bookmark_manager: t.Union[
+                AsyncBookmarkManager, BookmarkManager, None
+            ] = ...,
+
+            # undocumented/unsupported options
+            initial_retry_delay: float = ...,
+            retry_delay_multiplier: float = ...,
+            retry_delay_jitter_factor: float = ...
+        ) -> bool:
+            ...
+
+    else:
+
+        @preview("User switching is a preview feature.")
+        async def verify_authentication(
+            self,
+            auth: t.Union[Auth, t.Tuple[t.Any, t.Any], None] = None,
+            **config
+        ) -> bool:
+            """Verify that the authentication information is valid.
+
+            Like :meth:`.verify_connectivity`, but for checking authentication.
+
+            Try to establish a working read connection to the remote server or
+            a member of a cluster and exchange some data. In a cluster, there
+            is no guarantee about which server will be contacted. If the data
+            exchange is successful and the authentication information is valid,
+            :const:`True` is returned. Otherwise, the error will be matched
+            against a list of known authentication errors. If the error is on
+            that list, :const:`False` is returned indicating that the
+            authentication information is invalid. Otherwise, the error is
+            re-raised.
+
+            :param auth: authentication information to verify.
+                Same as the session config :ref:`auth-ref`.
+            :param config: accepts the same configuration key-word arguments as
+                :meth:`session`.
+
+                .. warning::
+                    All configuration key-word arguments (except ``auth``) are
+                    experimental. They might be changed or removed in any
+                    future version without prior notice.
+
+            :raises Exception: if the driver cannot connect to the remote.
+                Use the exception to further understand the cause of the
+                connectivity problem.
+
+            **This is a preview** (see :ref:`filter-warnings-ref`).
+            It might be changed without following the deprecation policy.
+            See also
+            https://github.com/neo4j/neo4j-python-driver/wiki/preview-features
+
+            .. versionadded:: 5.8
+            """
+            if config:
+                experimental_warn(
+                    "All configuration key-word arguments but auth to "
+                    "verify_authentication() are experimental. They might be "
+                    "changed or removed in any future version without prior "
+                    "notice."
+                )
+            config["auth"] = auth
+            if "database" not in config:
+                config["database"] = "system"
+            try:
+                with warnings.catch_warnings():
+                    warnings.filterwarnings(
+                        "ignore", message=r"^User switching\b.*",
+                        category=PreviewWarning
+                )
+                    session = self.session(**config)
+                async with session as session:
+                    await session._verify_authentication()
+            except Neo4jError as exc:
+                if exc.code in (
+                    "Neo.ClientError.Security.CredentialsExpired",
+                    "Neo.ClientError.Security.Forbidden",
+                    "Neo.ClientError.Security.TokenExpired",
+                    "Neo.ClientError.Security.Unauthorized",
+                ):
+                    return False
+                raise
+            return True
+
+
+    async def supports_session_auth(self) -> bool:
+        """Check if the remote supports connection re-authentication.
+
+        :returns: Returns true if the server or cluster the driver connects to
+            supports re-authentication of existing connections, otherwise
+            false.
+
+        .. note::
+            Feature support query based solely on the Bolt protocol version.
+            The feature might still be disabled on the server side even if this
+            function return :const:`True`. It just guarantees that the driver
+            won't throw a :exc:`ConfigurationError` when trying to use this
+            driver feature.
+
+        .. versionadded:: 5.8
+        """
+        async with self.session() as session:
+            await session._connect(READ_ACCESS)
+            assert session._connection
+            return session._connection.supports_re_auth
+
+    async def _get_server_info(self, **config) -> ServerInfo:
+        async with self.session(**config) as session:
+            return await session._get_server_info()
+
 
 async def _work(
     tx: AsyncManagedTransaction,
     query: str,
     parameters: t.Dict[str, t.Any],
     transformer: t.Callable[[AsyncResult], t.Awaitable[_T]]
 ) -> _T:
     res = await tx.run(query, parameters)
     if transformer is AsyncResult.to_eager_result:
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore",
-                                    message=r".*\bto_eager_result\b.*",
-                                    category=ExperimentalWarning)
-            return await transformer(res)
+        return await transformer(res)
     return await transformer(res)
 
 
 class AsyncBoltDriver(_Direct, AsyncDriver):
     """:class:`.AsyncBoltDriver` is instantiated for ``bolt`` URIs and
     addresses a single database machine. This may be a standalone server or
     could be a specific member of a cluster.
@@ -1037,27 +1199,27 @@
     the exact host and port detailed in the URI.
 
     This class is not supposed to be instantiated externally. Use
     :meth:`AsyncGraphDatabase.driver` instead.
     """
 
     @classmethod
-    def open(cls, target, *, auth=None, **config):
+    def open(cls, target, **config):
         """
         :param target:
         :param auth:
         :param config: The values that can be specified are found in :class: `neo4j.PoolConfig` and :class: `neo4j.WorkspaceConfig`
 
         :returns:
         :rtype: :class: `neo4j.BoltDriver`
         """
         from .io import AsyncBoltPool
         address = cls.parse_target(target)
         pool_config, default_workspace_config = Config.consume_chain(config, PoolConfig, WorkspaceConfig)
-        pool = AsyncBoltPool.open(address, auth=auth, pool_config=pool_config, workspace_config=default_workspace_config)
+        pool = AsyncBoltPool.open(address, pool_config=pool_config, workspace_config=default_workspace_config)
         return cls(pool, default_workspace_config)
 
     def __init__(self, pool, default_workspace_config):
         _Direct.__init__(self, pool.address)
         AsyncDriver.__init__(self, pool, default_workspace_config)
         self._default_workspace_config = default_workspace_config
 
@@ -1085,19 +1247,19 @@
     cluster members.
 
     This class is not supposed to be instantiated externally. Use
     :meth:`AsyncGraphDatabase.driver` instead.
     """
 
     @classmethod
-    def open(cls, *targets, auth=None, routing_context=None, **config):
+    def open(cls, *targets, routing_context=None, **config):
         from .io import AsyncNeo4jPool
         addresses = cls.parse_targets(*targets)
         pool_config, default_workspace_config = Config.consume_chain(config, PoolConfig, WorkspaceConfig)
-        pool = AsyncNeo4jPool.open(*addresses, auth=auth, routing_context=routing_context, pool_config=pool_config, workspace_config=default_workspace_config)
+        pool = AsyncNeo4jPool.open(*addresses, routing_context=routing_context, pool_config=pool_config, workspace_config=default_workspace_config)
         return cls(pool, default_workspace_config)
 
     def __init__(self, pool, default_workspace_config):
         _Routing.__init__(self, [pool.address])
         AsyncDriver.__init__(self, pool, default_workspace_config)
 
     if not t.TYPE_CHECKING:
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/io/__init__.py` & `neo4j-5.8.0/src/neo4j/_sync/io/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,24 +20,26 @@
 This module contains the low-level functionality required for speaking
 Bolt. It is not intended to be used directly by driver users. Instead,
 the `session` module provides the main user-facing abstractions.
 """
 
 
 __all__ = [
-    "AsyncBolt",
-    "AsyncBoltPool",
-    "AsyncNeo4jPool",
+    "AcquireAuth",
+    "Bolt",
+    "BoltPool",
+    "Neo4jPool",
     "check_supported_server_product",
     "ConnectionErrorHandler",
 ]
 
 
-from ._bolt import AsyncBolt
+from ._bolt import Bolt
 from ._common import (
     check_supported_server_product,
     ConnectionErrorHandler,
 )
 from ._pool import (
-    AsyncBoltPool,
-    AsyncNeo4jPool,
+    AcquireAuth,
+    BoltPool,
+    Neo4jPool,
 )
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/io/_bolt.py` & `neo4j-5.8.0/src/neo4j/_async/io/_bolt.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,25 @@
 import abc
 import asyncio
 from collections import deque
 from logging import getLogger
 from time import perf_counter
 
 from ..._async_compat.network import AsyncBoltSocket
+from ..._async_compat.util import AsyncUtil
 from ..._codec.hydration import v1 as hydration_v1
 from ..._codec.packstream import v1 as packstream_v1
 from ..._conf import PoolConfig
 from ..._deadline import Deadline
 from ..._exceptions import (
     BoltError,
     BoltHandshakeError,
 )
 from ..._meta import get_user_agent
-from ...addressing import Address
+from ...addressing import ResolvedAddress
 from ...api import (
     ServerInfo,
     Version,
 )
 from ...exceptions import (
     AuthError,
     ConfigurationError,
@@ -54,14 +55,28 @@
 )
 
 
 # Set up logger
 log = getLogger("neo4j")
 
 
+class ServerStateManagerBase(abc.ABC):
+    @abc.abstractmethod
+    def __init__(self, init_state, on_change=None):
+        ...
+
+    @abc.abstractmethod
+    def transition(self, message, metadata):
+        ...
+
+    @abc.abstractmethod
+    def failed(self):
+        ...
+
+
 class AsyncBolt:
     """ Server connection for Bolt protocol.
 
     A :class:`.Bolt` should be constructed following a
     successful .open()
 
     Bolt handshake and takes the socket over which
@@ -100,21 +115,25 @@
 
     # Store the id of the most recent ran query to be able to reduce sent bits by
     # using the default (-1) to refer to the most recent query when pulling
     # results for it.
     most_recent_qid = None
 
     def __init__(self, unresolved_address, sock, max_connection_lifetime, *,
-                 auth=None, user_agent=None, routing_context=None,
-                 notifications_min_severity=None, notifications_disabled_categories=None):
+                 auth=None, auth_manager=None, user_agent=None,
+                 routing_context=None, notifications_min_severity=None,
+                 notifications_disabled_categories=None):
         self.unresolved_address = unresolved_address
         self.socket = sock
         self.local_port = self.socket.getsockname()[1]
-        self.server_info = ServerInfo(Address(sock.getpeername()),
-                                      self.PROTOCOL_VERSION)
+        self.server_info = ServerInfo(
+            ResolvedAddress(sock.getpeername(),
+                            host_name=unresolved_address.host),
+            self.PROTOCOL_VERSION
+        )
         # so far `connection.recv_timeout_seconds` is the only available
         # configuration hint that exists. Therefore, all hints can be stored at
         # connection level. This might change in the future.
         self.configuration_hints = {}
         self.patch = {}
         self.outbox = AsyncOutbox(
             self.socket, on_error=self._set_defunct_write,
@@ -133,43 +152,44 @@
 
         # Determine the user agent
         if user_agent:
             self.user_agent = user_agent
         else:
             self.user_agent = get_user_agent()
 
-        # Determine auth details
-        if not auth:
-            self.auth_dict = {}
-        elif isinstance(auth, tuple) and 2 <= len(auth) <= 3:
-            from ...api import Auth
-            self.auth_dict = vars(Auth("basic", *auth))
-        else:
-            try:
-                self.auth_dict = vars(auth)
-            except (KeyError, TypeError):
-                raise AuthError("Cannot determine auth details from %r" % auth)
-
-        # Check for missing password
-        try:
-            credentials = self.auth_dict["credentials"]
-        except KeyError:
-            pass
-        else:
-            if credentials is None:
-                raise AuthError("Password cannot be None")
+        self.auth = auth
+        self.auth_dict = self._to_auth_dict(auth)
+        self.auth_manager = auth_manager
 
         self.notifications_min_severity = notifications_min_severity
         self.notifications_disabled_categories = \
             notifications_disabled_categories
 
     def __del__(self):
         if not asyncio.iscoroutinefunction(self.close):
             self.close()
 
+    @abc.abstractmethod
+    def _get_server_state_manager(self) -> ServerStateManagerBase:
+        ...
+
+    @classmethod
+    def _to_auth_dict(cls, auth):
+        # Determine auth details
+        if not auth:
+            return {}
+        elif isinstance(auth, tuple) and 2 <= len(auth) <= 3:
+            from ...api import Auth
+            return vars(Auth("basic", *auth))
+        else:
+            try:
+                return vars(auth)
+            except (KeyError, TypeError):
+                raise AuthError("Cannot determine auth details from %r" % auth)
+
     @property
     def connection_id(self):
         return self.server_info._metadata.get("connection_id", "<unknown id>")
 
     @property
     @abc.abstractmethod
     def supports_multiple_results(self):
@@ -185,14 +205,28 @@
         """ Boolean flag to indicate if the connection version supports multiple
         databases.
         """
         pass
 
     @property
     @abc.abstractmethod
+    def supports_re_auth(self):
+        """Whether the connection version supports re-authentication."""
+        pass
+
+    def assert_re_auth_support(self):
+        if not self.supports_re_auth:
+            raise ConfigurationError(
+                "User switching is not supported for Bolt "
+                f"Protocol {self.PROTOCOL_VERSION!r}. Server Agent "
+                f"{self.server_info.agent!r}"
+            )
+
+    @property
+    @abc.abstractmethod
     def supports_notification_filtering(self):
         """Whether the connection version supports re-authentication."""
         pass
 
     def assert_notification_filtering_support(self):
         if not self.supports_notification_filtering:
             raise ConfigurationError(
@@ -314,21 +348,21 @@
         else:
             await AsyncBoltSocket.close_socket(s)
             return protocol_version
 
     # [bolt-version-bump] search tag when changing bolt version support
     @classmethod
     async def open(
-        cls, address, *, auth=None, deadline=None, routing_context=None,
-        pool_config=None
+        cls, address, *, auth_manager=None, deadline=None,
+        routing_context=None, pool_config=None
     ):
         """Open a new Bolt connection to a given server address.
 
         :param address:
-        :param auth:
+        :param auth_manager:
         :param deadline: how long to wait for the connection to be established
         :param routing_context: dict containing routing context
         :param pool_config:
 
         :returns: connected AsyncBolt instance
 
         :raise BoltHandshakeError:
@@ -382,28 +416,42 @@
         # elif protocol_version == (4, 0):
         #     from ._bolt4 import AsyncBolt4x0
         #     bolt_cls = AsyncBolt4x0
         elif protocol_version == (3, 0):
             from ._bolt3 import AsyncBolt3
             bolt_cls = AsyncBolt3
         else:
-            log.debug("[#%04X]  S: <CLOSE>", s.getsockname()[1])
+            log.debug("[#%04X]  C: <CLOSE>", s.getsockname()[1])
             await AsyncBoltSocket.close_socket(s)
 
             supported_versions = cls.protocol_handlers().keys()
             raise BoltHandshakeError(
                 "The neo4j server does not support communication with this "
                 "driver. This driver has support for Bolt protocols "
                 "{}.".format(tuple(map(str, supported_versions))),
                 address=address, request_data=handshake, response_data=data
             )
 
+        try:
+            auth = await AsyncUtil.callback(auth_manager.get_auth)
+        except asyncio.CancelledError as e:
+            log.debug("[#%04X]  C: <KILL> open auth manager failed: %r",
+                      s.getsockname()[1], e)
+            s.kill()
+            raise
+        except Exception as e:
+            log.debug("[#%04X]  C: <CLOSE> open auth manager failed: %r",
+                      s.getsockname()[1], e)
+            await s.close()
+            raise
+
         connection = bolt_cls(
             address, s, pool_config.max_connection_lifetime, auth=auth,
-            user_agent=pool_config.user_agent, routing_context=routing_context,
+            auth_manager=auth_manager, user_agent=pool_config.user_agent,
+            routing_context=routing_context,
             notifications_min_severity=pool_config.notifications_min_severity,
             notifications_disabled_categories=
                 pool_config.notifications_disabled_categories
         )
 
         try:
             connection.socket.set_deadline(deadline)
@@ -445,14 +493,53 @@
             Hooks to hydrate types (mapping from type (class) to
             dehydration function). Dehydration functions receive the value of
             type understood by packstream and are free to return anything.
         """
         pass
 
     @abc.abstractmethod
+    def logon(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGON message to the outgoing queue."""
+        pass
+
+    @abc.abstractmethod
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGOFF message to the outgoing queue."""
+        pass
+
+    def mark_unauthenticated(self):
+        """Mark the connection as unauthenticated."""
+        self.auth_dict = {}
+
+    def re_auth(
+        self, auth, auth_manager, force=False,
+        dehydration_hooks=None, hydration_hooks=None,
+    ):
+        """Append LOGON, LOGOFF to the outgoing queue.
+
+        If auth is the same as the current auth, this method does nothing.
+
+        :returns: whether the auth was changed
+        """
+        new_auth_dict = self._to_auth_dict(auth)
+        if not force and new_auth_dict == self.auth_dict:
+            self.auth_manager = auth_manager
+            self.auth = auth
+            return False
+        self.logoff(dehydration_hooks=dehydration_hooks,
+                     hydration_hooks=hydration_hooks)
+        self.auth_dict = new_auth_dict
+        self.auth_manager = auth_manager
+        self.auth = auth
+        self.logon(dehydration_hooks=dehydration_hooks,
+                    hydration_hooks=hydration_hooks)
+        return True
+
+
+    @abc.abstractmethod
     async def route(
         self, database=None, imp_user=None, bookmarks=None,
         dehydration_hooks=None, hydration_hooks=None
     ):
         """ Fetch a routing table from the server for the given
         `database`. For Bolt 4.3 and above, this appends a ROUTE
         message; for earlier versions, a procedure call is made via
@@ -763,15 +850,15 @@
             self.kill()
             raise error  # cancellation error should not be re-written
         if not self._closing:
             # If we fail while closing the connection, there is no need to
             # remove the connection from the pool, nor to try to close the
             # connection again.
             await self.close()
-            if self.pool:
+            if self.pool and not self._get_server_state_manager().failed():
                 await self.pool.deactivate(address=self.unresolved_address)
 
         # Iterate through the outstanding responses, and if any correspond
         # to COMMIT requests then raise an error to signal that we are
         # unable to confirm that the COMMIT completed successfully.
         if silent:
             return
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/io/_bolt3.py` & `neo4j-5.8.0/src/neo4j/_async/io/_bolt3.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from __future__ import annotations
+
+import typing as t
 from enum import Enum
 from logging import getLogger
 from ssl import SSLSocket
 
 from ..._exceptions import BoltProtocolError
 from ...api import (
     READ_ACCESS,
@@ -29,15 +32,18 @@
     ConfigurationError,
     DatabaseUnavailable,
     ForbiddenOnReadOnlyDatabase,
     Neo4jError,
     NotALeader,
     ServiceUnavailable,
 )
-from ._bolt import AsyncBolt
+from ._bolt import (
+    AsyncBolt,
+    ServerStateManagerBase,
+)
 from ._common import (
     check_supported_server_product,
     CommitResponse,
     InitResponse,
     Response,
 )
 
@@ -49,16 +55,16 @@
     CONNECTED = "CONNECTED"
     READY = "READY"
     STREAMING = "STREAMING"
     TX_READY_OR_TX_STREAMING = "TX_READY||TX_STREAMING"
     FAILED = "FAILED"
 
 
-class ServerStateManager:
-    _STATE_TRANSITIONS = {
+class ServerStateManager(ServerStateManagerBase):
+    _STATE_TRANSITIONS: t.Dict[Enum, t.Dict[str, Enum]] = {
         ServerStates.CONNECTED: {
             "hello": ServerStates.READY,
         },
         ServerStates.READY: {
             "run": ServerStates.STREAMING,
             "begin": ServerStates.TX_READY_OR_TX_STREAMING,
         },
@@ -87,39 +93,47 @@
         state_before = self.state
         self.state = self._STATE_TRANSITIONS\
             .get(self.state, {})\
             .get(message, self.state)
         if state_before != self.state and callable(self._on_change):
             self._on_change(state_before, self.state)
 
+    def failed(self):
+        return self.state == ServerStates.FAILED
+
 
 class AsyncBolt3(AsyncBolt):
     """ Protocol handler for Bolt 3.
 
     This is supported by Neo4j versions 3.5, 4.0, 4.1, 4.2, 4.3, and 4.4.
     """
 
     PROTOCOL_VERSION = Version(3, 0)
 
     supports_multiple_results = False
 
     supports_multiple_databases = False
 
+    supports_re_auth = False
+
     supports_notification_filtering = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._server_state_manager = ServerStateManager(
             ServerStates.CONNECTED, on_change=self._on_server_state_change
         )
 
     def _on_server_state_change(self, old_state, new_state):
         log.debug("[#%04X]  _: <CONNECTION> state: %s > %s", self.local_port,
                   old_state.name, new_state.name)
 
+    def _get_server_state_manager(self) -> ServerStateManagerBase:
+        return self._server_state_manager
+
     @property
     def is_reset(self):
         # We can't be sure of the server's state if there are still pending
         # responses. Unless the last message we sent was RESET. In that case
         # the server state will always be READY when we're done.
         if (self.responses and self.responses[-1]
                 and self.responses[-1].message == "reset"):
@@ -155,14 +169,22 @@
                      response=InitResponse(self, "hello", hydration_hooks,
                                            on_success=self.server_info.update),
                      dehydration_hooks=dehydration_hooks)
         await self.send_all()
         await self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
+    def logon(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGON message to the outgoing queue."""
+        self.assert_re_auth_support()
+
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGOFF message to the outgoing queue."""
+        self.assert_re_auth_support()
+
     async def route(
         self, database=None, imp_user=None, bookmarks=None,
         dehydration_hooks=None, hydration_hooks=None
     ):
         if database is not None:
             raise ConfigurationError(
                 "Database name parameter for selecting database is not "
@@ -393,14 +415,13 @@
                     await self.pool.deactivate(address=self.unresolved_address)
                 raise
             except (NotALeader, ForbiddenOnReadOnlyDatabase):
                 if self.pool:
                     self.pool.on_write_failure(address=self.unresolved_address)
                 raise
             except Neo4jError as e:
-                if self.pool and e._invalidates_all_connections():
-                    await self.pool.mark_all_stale()
+                await self.pool.on_neo4j_error(e, self)
                 raise
         else:
             raise BoltProtocolError("Unexpected response message with signature %02X" % summary_signature, address=self.unresolved_address)
 
         return len(details), 1
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/io/_bolt4.py` & `neo4j-5.8.0/src/neo4j/_async/io/_bolt4.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from logging import getLogger
 from ssl import SSLSocket
 
-from ..._async_compat.util import AsyncUtil
 from ..._exceptions import BoltProtocolError
 from ...api import (
     READ_ACCESS,
     SYSTEM_DATABASE,
     Version,
 )
 from ...exceptions import (
     ConfigurationError,
     DatabaseUnavailable,
     ForbiddenOnReadOnlyDatabase,
     Neo4jError,
     NotALeader,
     ServiceUnavailable,
 )
-from ._bolt import AsyncBolt
+from ._bolt import (
+    AsyncBolt,
+    ServerStateManagerBase,
+)
 from ._bolt3 import (
     ServerStateManager,
     ServerStates,
 )
 from ._common import (
     check_supported_server_product,
     CommitResponse,
@@ -58,26 +60,31 @@
 
     PROTOCOL_VERSION = Version(4, 0)
 
     supports_multiple_results = True
 
     supports_multiple_databases = True
 
+    supports_re_auth = False
+
     supports_notification_filtering = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._server_state_manager = ServerStateManager(
             ServerStates.CONNECTED, on_change=self._on_server_state_change
         )
 
     def _on_server_state_change(self, old_state, new_state):
         log.debug("[#%04X]  _: <CONNECTION> state: %s > %s", self.local_port,
                   old_state.name, new_state.name)
 
+    def _get_server_state_manager(self) -> ServerStateManagerBase:
+        return self._server_state_manager
+
     @property
     def is_reset(self):
         # We can't be sure of the server's state if there are still pending
         # responses. Unless the last message we sent was RESET. In that case
         # the server state will always be READY when we're done.
         if (self.responses and self.responses[-1]
                 and self.responses[-1].message == "reset"):
@@ -115,14 +122,22 @@
                          on_success=self.server_info.update
                      ),
                      dehydration_hooks=dehydration_hooks)
         await self.send_all()
         await self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
+    def logon(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGON message to the outgoing queue."""
+        self.assert_re_auth_support()
+
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGOFF message to the outgoing queue."""
+        self.assert_re_auth_support()
+
     async def route(
         self, database=None, imp_user=None, bookmarks=None,
         dehydration_hooks=None, hydration_hooks=None
     ):
         if imp_user is not None:
             raise ConfigurationError(
                 "Impersonation is not supported in Bolt Protocol {!r}. "
@@ -349,16 +364,16 @@
                     await self.pool.deactivate(address=self.unresolved_address)
                 raise
             except (NotALeader, ForbiddenOnReadOnlyDatabase):
                 if self.pool:
                     self.pool.on_write_failure(address=self.unresolved_address)
                 raise
             except Neo4jError as e:
-                if self.pool and e._invalidates_all_connections():
-                    await self.pool.mark_all_stale()
+                if self.pool:
+                    await self.pool.on_neo4j_error(e, self)
                 raise
         else:
             raise BoltProtocolError("Unexpected response message with signature "
                                     "%02X" % ord(summary_signature), self.unresolved_address)
 
         return len(details), 1
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/io/_bolt5.py` & `neo4j-5.8.0/src/neo4j/_sync/io/_bolt5.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import typing as t
+from enum import Enum
 from logging import getLogger
 from ssl import SSLSocket
 
 from ..._codec.hydration import v2 as hydration_v2
 from ..._exceptions import BoltProtocolError
 from ...api import (
     READ_ACCESS,
@@ -28,60 +30,74 @@
 from ...exceptions import (
     DatabaseUnavailable,
     ForbiddenOnReadOnlyDatabase,
     Neo4jError,
     NotALeader,
     ServiceUnavailable,
 )
-from ._bolt import AsyncBolt
+from ._bolt import (
+    Bolt,
+    ServerStateManagerBase,
+)
 from ._bolt3 import (
     ServerStateManager,
     ServerStates,
 )
 from ._common import (
     check_supported_server_product,
     CommitResponse,
     InitResponse,
+    LogonResponse,
     Response,
 )
 
 
 log = getLogger("neo4j")
 
 
-class AsyncBolt5x0(AsyncBolt):
-    """Protocol handler for Bolt 5.0. """
+class Bolt5x0(Bolt):
+    """Protocol handler for Bolt 5.0."""
 
     PROTOCOL_VERSION = Version(5, 0)
 
     HYDRATION_HANDLER_CLS = hydration_v2.HydrationHandler
 
     supports_multiple_results = True
 
     supports_multiple_databases = True
 
+    supports_re_auth = False
+
+    supports_notification_filtering = False
+
+    server_states: t.Any = ServerStates
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._server_state_manager = ServerStateManager(
-            ServerStates.CONNECTED, on_change=self._on_server_state_change
+            self.server_states.CONNECTED,
+            on_change=self._on_server_state_change
         )
 
     def _on_server_state_change(self, old_state, new_state):
         log.debug("[#%04X]  _: <CONNECTION> state: %s > %s", self.local_port,
                   old_state.name, new_state.name)
 
+    def _get_server_state_manager(self) -> ServerStateManagerBase:
+        return self._server_state_manager
+
     @property
     def is_reset(self):
         # We can't be sure of the server's state if there are still pending
         # responses. Unless the last message we sent was RESET. In that case
         # the server state will always be READY when we're done.
         if (self.responses and self.responses[-1]
                 and self.responses[-1].message == "reset"):
             return True
-        return self._server_state_manager.state == ServerStates.READY
+        return self._server_state_manager.state == self.server_states.READY
 
     @property
     def encrypted(self):
         return isinstance(self.socket, SSLSocket)
 
     @property
     def der_encoded_server_certificate(self):
@@ -89,15 +105,15 @@
 
     def get_base_headers(self):
         headers = {"user_agent": self.user_agent}
         if self.routing_context is not None:
             headers["routing"] = self.routing_context
         return headers
 
-    async def hello(self, dehydration_hooks=None, hydration_hooks=None):
+    def hello(self, dehydration_hooks=None, hydration_hooks=None):
         if (
             self.notifications_min_severity is not None
             or self.notifications_disabled_categories is not None
         ):
             self.assert_notification_filtering_support()
 
         def on_success(metadata):
@@ -122,19 +138,27 @@
         if "credentials" in logged_headers:
             logged_headers["credentials"] = "*******"
         log.debug("[#%04X]  C: HELLO %r", self.local_port, logged_headers)
         self._append(b"\x01", (headers,),
                      response=InitResponse(self, "hello", hydration_hooks,
                                            on_success=on_success),
                      dehydration_hooks=dehydration_hooks)
-        await self.send_all()
-        await self.fetch_all()
+        self.send_all()
+        self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
-    async def route(self, database=None, imp_user=None, bookmarks=None,
+    def logon(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGON message to the outgoing queue."""
+        self.assert_re_auth_support()
+
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGOFF message to the outgoing queue."""
+        self.assert_re_auth_support()
+
+    def route(self, database=None, imp_user=None, bookmarks=None,
                     dehydration_hooks=None, hydration_hooks=None):
         routing_context = self.routing_context or {}
         db_context = {}
         if database is not None:
             db_context.update(db=database)
         if imp_user is not None:
             db_context.update(imp_user=imp_user)
@@ -145,16 +169,16 @@
             bookmarks = []
         else:
             bookmarks = list(bookmarks)
         self._append(b"\x66", (routing_context, bookmarks, db_context),
                      response=Response(self, "route", hydration_hooks,
                                        on_success=metadata.update),
                      dehydration_hooks=hydration_hooks)
-        await self.send_all()
-        await self.fetch_all()
+        self.send_all()
+        self.fetch_all()
         return [metadata.get("rt")]
 
     def run(self, query, parameters=None, mode=None, bookmarks=None,
             metadata=None, timeout=None, db=None, imp_user=None,
             notifications_min_severity=None,
             notifications_disabled_categories=None, dehydration_hooks=None,
             hydration_hooks=None, **handlers):
@@ -266,15 +290,15 @@
     def rollback(self, dehydration_hooks=None, hydration_hooks=None,
                  **handlers):
         log.debug("[#%04X]  C: ROLLBACK", self.local_port)
         self._append(b"\x13", (),
                      Response(self, "rollback", hydration_hooks, **handlers),
                      dehydration_hooks=dehydration_hooks)
 
-    async def reset(self, dehydration_hooks=None, hydration_hooks=None):
+    def reset(self, dehydration_hooks=None, hydration_hooks=None):
         """Reset the connection.
 
         Add a RESET message to the outgoing queue, send it and consume all
         remaining messages.
         """
 
         def fail(metadata):
@@ -282,22 +306,22 @@
                                     self.unresolved_address)
 
         log.debug("[#%04X]  C: RESET", self.local_port)
         self._append(b"\x0F",
                      response=Response(self, "reset", hydration_hooks,
                                        on_failure=fail),
                      dehydration_hooks=dehydration_hooks)
-        await self.send_all()
-        await self.fetch_all()
+        self.send_all()
+        self.fetch_all()
 
     def goodbye(self, dehydration_hooks=None, hydration_hooks=None):
         log.debug("[#%04X]  C: GOODBYE", self.local_port)
         self._append(b"\x02", (), dehydration_hooks=dehydration_hooks)
 
-    async def _process_message(self, tag, fields):
+    def _process_message(self, tag, fields):
         """Process at most one message from the server, if available.
 
         :returns: 2-tuple of number of detail messages and number of summary
                  messages fetched
         """
         details = []
         summary_signature = summary_metadata = None
@@ -308,63 +332,116 @@
             summary_metadata = fields[0]
         else:
             summary_signature = tag
 
         if details:
             # Do not log any data
             log.debug("[#%04X]  S: RECORD * %d", self.local_port, len(details))
-            await self.responses[0].on_records(details)
+            self.responses[0].on_records(details)
 
         if summary_signature is None:
             return len(details), 0
 
         response = self.responses.popleft()
         response.complete = True
         if summary_signature == b"\x70":
             log.debug("[#%04X]  S: SUCCESS %r", self.local_port,
                       summary_metadata)
             self._server_state_manager.transition(response.message,
                                                   summary_metadata)
-            await response.on_success(summary_metadata or {})
+            response.on_success(summary_metadata or {})
         elif summary_signature == b"\x7E":
             log.debug("[#%04X]  S: IGNORED", self.local_port)
-            await response.on_ignored(summary_metadata or {})
+            response.on_ignored(summary_metadata or {})
         elif summary_signature == b"\x7F":
             log.debug("[#%04X]  S: FAILURE %r", self.local_port,
                       summary_metadata)
-            self._server_state_manager.state = ServerStates.FAILED
+            self._server_state_manager.state = self.server_states.FAILED
             try:
-                await response.on_failure(summary_metadata or {})
+                response.on_failure(summary_metadata or {})
             except (ServiceUnavailable, DatabaseUnavailable):
                 if self.pool:
-                    await self.pool.deactivate(address=self.unresolved_address)
+                    self.pool.deactivate(address=self.unresolved_address)
                 raise
             except (NotALeader, ForbiddenOnReadOnlyDatabase):
                 if self.pool:
                     self.pool.on_write_failure(address=self.unresolved_address)
                 raise
             except Neo4jError as e:
-                if self.pool and e._invalidates_all_connections():
-                    await self.pool.mark_all_stale()
+                if self.pool:
+                    self.pool.on_neo4j_error(e, self)
                 raise
         else:
             raise BoltProtocolError(
                 "Unexpected response message with signature %02X" % ord(
                     summary_signature
                 ), self.unresolved_address
             )
 
         return len(details), 1
 
 
-class AsyncBolt5x1(AsyncBolt5x0):
+class ServerStates5x1(Enum):
+    CONNECTED = "CONNECTED"
+    READY = "READY"
+    STREAMING = "STREAMING"
+    TX_READY_OR_TX_STREAMING = "TX_READY||TX_STREAMING"
+    FAILED = "FAILED"
+    AUTHENTICATION = "AUTHENTICATION"
+
+
+class ServerStateManager5x1(ServerStateManager):
+    _STATE_TRANSITIONS = {  # type: ignore
+        ServerStates5x1.CONNECTED: {
+            "hello": ServerStates5x1.AUTHENTICATION,
+        },
+        ServerStates5x1.AUTHENTICATION: {
+            "logon": ServerStates5x1.READY,
+        },
+        ServerStates5x1.READY: {
+            "run": ServerStates5x1.STREAMING,
+            "begin": ServerStates5x1.TX_READY_OR_TX_STREAMING,
+            "logoff": ServerStates5x1.AUTHENTICATION,
+        },
+        ServerStates5x1.STREAMING: {
+            "pull": ServerStates5x1.READY,
+            "discard": ServerStates5x1.READY,
+            "reset": ServerStates5x1.READY,
+        },
+        ServerStates5x1.TX_READY_OR_TX_STREAMING: {
+            "commit": ServerStates5x1.READY,
+            "rollback": ServerStates5x1.READY,
+            "reset": ServerStates5x1.READY,
+        },
+        ServerStates5x1.FAILED: {
+            "reset": ServerStates5x1.READY,
+        }
+    }
+
+
+    def failed(self):
+        return self.state == ServerStates5x1.FAILED
+
+
+class Bolt5x1(Bolt5x0):
+    """Protocol handler for Bolt 5.1."""
 
     PROTOCOL_VERSION = Version(5, 1)
 
-    async def hello(self, dehydration_hooks=None, hydration_hooks=None):
+    supports_re_auth = True
+
+    server_states = ServerStates5x1
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._server_state_manager = ServerStateManager5x1(
+            ServerStates5x1.CONNECTED, on_change=self._on_server_state_change
+        )
+
+    def hello(self, dehydration_hooks=None, hydration_hooks=None):
         if (
             self.notifications_min_severity is not None
             or self.notifications_disabled_categories is not None
         ):
             self.assert_notification_filtering_support()
 
         def on_success(metadata):
@@ -379,51 +456,60 @@
                 else:
                     log.info("[#%04X]  _: <CONNECTION> Server supplied an "
                              "invalid value for "
                              "connection.recv_timeout_seconds (%r). Make sure "
                              "the server and network is set up correctly.",
                              self.local_port, recv_timeout)
 
-        extra = self.get_base_headers()
-        log.debug("[#%04X]  C: HELLO %r", self.local_port, extra)
-        self._append(b"\x01", (extra,),
+        headers = self.get_base_headers()
+        logged_headers = dict(headers)
+        log.debug("[#%04X]  C: HELLO %r", self.local_port, logged_headers)
+        self._append(b"\x01", (headers,),
                      response=InitResponse(self, "hello", hydration_hooks,
                                            on_success=on_success),
                      dehydration_hooks=dehydration_hooks)
-
-        self.logon(dehydration_hooks, hydration_hooks)
-        await self.send_all()
-        await self.fetch_all()
+        self.logon(dehydration_hooks=dehydration_hooks,
+                   hydration_hooks=hydration_hooks)
+        self.send_all()
+        self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
     def logon(self, dehydration_hooks=None, hydration_hooks=None):
         logged_auth_dict = dict(self.auth_dict)
         if "credentials" in logged_auth_dict:
             logged_auth_dict["credentials"] = "*******"
         log.debug("[#%04X]  C: LOGON %r", self.local_port, logged_auth_dict)
         self._append(b"\x6A", (self.auth_dict,),
-                     response=Response(self, "logon", hydration_hooks),
+                     response=LogonResponse(self, "logon", hydration_hooks),
+                     dehydration_hooks=dehydration_hooks)
+
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        log.debug("[#%04X]  C: LOGOFF", self.local_port)
+        self._append(b"\x6B",
+                     response=LogonResponse(self, "logoff", hydration_hooks),
                      dehydration_hooks=dehydration_hooks)
 
 
-class AsyncBolt5x2(AsyncBolt5x1):
+class Bolt5x2(Bolt5x1):
 
     PROTOCOL_VERSION = Version(5, 2)
 
+    supports_notification_filtering = True
+
     def get_base_headers(self):
         headers = super().get_base_headers()
         if self.notifications_min_severity is not None:
-            headers["notifications_minimum_severity"] =\
+            headers["notifications_minimum_severity"] = \
                 self.notifications_min_severity
         if self.notifications_disabled_categories is not None:
             headers["notifications_disabled_categories"] = \
                 self.notifications_disabled_categories
         return headers
 
-    async def hello(self, dehydration_hooks=None, hydration_hooks=None):
+    def hello(self, dehydration_hooks=None, hydration_hooks=None):
         def on_success(metadata):
             self.configuration_hints.update(metadata.pop("hints", {}))
             self.server_info.update(metadata)
             if "connection.recv_timeout_seconds" in self.configuration_hints:
                 recv_timeout = self.configuration_hints[
                     "connection.recv_timeout_seconds"
                 ]
@@ -440,27 +526,18 @@
         log.debug("[#%04X]  C: HELLO %r", self.local_port, extra)
         self._append(b"\x01", (extra,),
                      response=InitResponse(self, "hello", hydration_hooks,
                                            on_success=on_success),
                      dehydration_hooks=dehydration_hooks)
 
         self.logon(dehydration_hooks, hydration_hooks)
-        await self.send_all()
-        await self.fetch_all()
+        self.send_all()
+        self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
-    def logon(self, dehydration_hooks=None, hydration_hooks=None):
-        logged_auth_dict = dict(self.auth_dict)
-        if "credentials" in logged_auth_dict:
-            logged_auth_dict["credentials"] = "*******"
-        log.debug("[#%04X]  C: LOGON %r", self.local_port, logged_auth_dict)
-        self._append(b"\x6A", (self.auth_dict,),
-                     response=Response(self, "logon", hydration_hooks),
-                     dehydration_hooks=dehydration_hooks)
-
     def run(self, query, parameters=None, mode=None, bookmarks=None,
             metadata=None, timeout=None, db=None, imp_user=None,
             notifications_min_severity=None,
             notifications_disabled_categories=None, dehydration_hooks=None,
             hydration_hooks=None, **handlers):
         if not parameters:
             parameters = {}
@@ -531,13 +608,13 @@
                 raise TypeError("Timeout must be a number (in seconds)")
             if extra["tx_timeout"] < 0:
                 raise ValueError("Timeout must be a number >= 0")
         if notifications_min_severity is not None:
             extra["notifications_minimum_severity"] = \
                 notifications_min_severity
         if notifications_disabled_categories is not None:
-            extra["notifications_disabled_categories"] =\
+            extra["notifications_disabled_categories"] = \
                 notifications_disabled_categories
         log.debug("[#%04X]  C: BEGIN %r", self.local_port, extra)
         self._append(b"\x11", (extra,),
                      Response(self, "begin", hydration_hooks, **handlers),
                      dehydration_hooks=dehydration_hooks)
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/io/_common.py` & `neo4j-5.8.0/src/neo4j/_async/io/_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -252,27 +252,42 @@
         handler = self.handlers.get("on_ignored")
         await AsyncUtil.callback(handler, metadata)
         handler = self.handlers.get("on_summary")
         await AsyncUtil.callback(handler)
 
 
 class InitResponse(Response):
+    async def on_failure(self, metadata):
+        # No sense in resetting the connection,
+        # the server will have closed it already.
+        self.connection.kill()
+        handler = self.handlers.get("on_failure")
+        await AsyncUtil.callback(handler, metadata)
+        handler = self.handlers.get("on_summary")
+        await AsyncUtil.callback(handler)
+        metadata["message"] = metadata.get(
+            "message",
+            "Connection initialisation failed due to an unknown error"
+        )
+        raise Neo4jError.hydrate(**metadata)
+
 
+class LogonResponse(InitResponse):
     async def on_failure(self, metadata):
-        code = metadata.get("code")
-        if code == "Neo.ClientError.Security.Unauthorized":
-            raise Neo4jError.hydrate(**metadata)
-        else:
-            raise ServiceUnavailable(
-                metadata.get("message", "Connection initialisation failed")
-            )
+        # No sense in resetting the connection,
+        # the server will have closed it already.
+        self.connection.kill()
+        handler = self.handlers.get("on_failure")
+        await AsyncUtil.callback(handler, metadata)
+        handler = self.handlers.get("on_summary")
+        await AsyncUtil.callback(handler)
+        raise Neo4jError.hydrate(**metadata)
 
 
 class CommitResponse(Response):
-
     pass
 
 
 def check_supported_server_product(agent):
     """ Checks that a server product is supported by the driver by
     looking at the server agent string.
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/io/_pool.py` & `neo4j-5.8.0/src/neo4j/_async/io/_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,61 +12,81 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from __future__ import annotations
+
 import abc
 import asyncio
 import logging
+import typing as t
 from collections import (
     defaultdict,
     deque,
 )
+from copy import copy
+from dataclasses import dataclass
 from logging import getLogger
 from random import choice
 
 from ..._async_compat.concurrency import (
     AsyncCondition,
     AsyncCooperativeRLock,
     AsyncRLock,
 )
 from ..._async_compat.network import AsyncNetworkUtil
+from ..._async_compat.util import AsyncUtil
 from ..._conf import (
     PoolConfig,
     WorkspaceConfig,
 )
 from ..._deadline import (
     connection_deadline,
     Deadline,
 )
 from ..._exceptions import BoltError
 from ..._routing import RoutingTable
+from ..._sync.auth_management import StaticAuthManager
 from ...api import (
     READ_ACCESS,
     WRITE_ACCESS,
 )
+from ...auth_management import (
+    AsyncAuthManager,
+    AuthManager,
+)
 from ...exceptions import (
     ClientError,
     ConfigurationError,
     DriverError,
     Neo4jError,
     ReadServiceUnavailable,
     ServiceUnavailable,
     SessionExpired,
+    TokenExpired,
+    TokenExpiredRetryable,
     WriteServiceUnavailable,
 )
+from ..auth_management import AsyncStaticAuthManager
 from ._bolt import AsyncBolt
 
 
 # Set up logger
 log = getLogger("neo4j")
 
 
+@dataclass
+class AcquireAuth:
+    auth: t.Union[AsyncAuthManager, AuthManager, None]
+    force_auth: bool = False
+
+
 class AsyncIOPool(abc.ABC):
     """ A collection of connections to one or more server addresses.
     """
 
     def __init__(self, opener, pool_config, workspace_config):
         assert callable(opener)
         assert isinstance(pool_config, PoolConfig)
@@ -82,67 +102,91 @@
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
 
+    async def get_auth(self):
+        return await AsyncUtil.callback(self.pool_config.auth.get_auth)
+
     async def _acquire_from_pool(self, address):
         with self.lock:
             for connection in list(self.connections.get(address, [])):
                 if connection.in_use:
                     continue
                 connection.pool = self
                 connection.in_use = True
                 return connection
         return None  # no free connection available
 
+    def _remove_connection(self, connection):
+        address = connection.unresolved_address
+        with self.lock:
+            log.debug(
+                "[#%04X]  _: <POOL> remove connection from pool %r %s",
+                connection.local_port, address, connection.connection_id
+            )
+            try:
+                self.connections.get(address, []).remove(connection)
+            except ValueError:
+                # If closure fails (e.g. because the server went
+                # down), all connections to the same address will
+                # be removed. Therefore, we silently ignore if the
+                # connection isn't in the pool anymore.
+                pass
+
     async def _acquire_from_pool_checked(
         self, address, health_check, deadline
     ):
         while not deadline.expired():
             connection = await self._acquire_from_pool(address)
             if not connection:
                 return None  # no free connection available
             if not await health_check(connection, deadline):
                 # `close` is a noop on already closed connections.
                 # This is to make sure that the connection is
                 # gracefully closed, e.g. if it's just marked as
                 # `stale` but still alive.
                 if log.isEnabledFor(logging.DEBUG):
                     log.debug(
-                        "[#%04X]  _: <POOL> removing old connection %s "
+                        "[#%04X]  _: <POOL> found unhealthy connection %s "
                         "(closed=%s, defunct=%s, stale=%s, in_use=%s)",
                         connection.local_port, connection.connection_id,
                         connection.closed(), connection.defunct(),
                         connection.stale(), connection.in_use
                     )
                 await connection.close()
-                with self.lock:
-                    try:
-                        self.connections.get(address, []).remove(connection)
-                    except ValueError:
-                        # If closure fails (e.g. because the server went
-                        # down), all connections to the same address will
-                        # be removed. Therefore, we silently ignore if the
-                        # connection isn't in the pool anymore.
-                        pass
+                self._remove_connection(connection)
                 continue  # try again with a new connection
             else:
                 return connection
 
-    def _acquire_new_later(self, address, deadline):
+    def _acquire_new_later(self, address, auth, deadline):
         async def connection_creator():
             released_reservation = False
             try:
                 try:
-                    connection = await self.opener(address, deadline)
+                    connection = await self.opener(
+                        address, auth or self.pool_config.auth, deadline
+                    )
                 except ServiceUnavailable:
                     await self.deactivate(address)
                     raise
+                if auth:
+                    # It's unfortunate that we have to create a connection
+                    # first to determine if the session-level auth is supported
+                    # by the protocol or not.
+                    try:
+                        connection.assert_re_auth_support()
+                    except ConfigurationError:
+                        log.debug("[#%04X]  _: <POOL> no re-auth support",
+                                  connection.local_port)
+                        await connection.close()
+                        raise
                 connection.pool = self
                 connection.in_use = True
                 with self.lock:
                     self.connections_reservations[address] -= 1
                     released_reservation = True
                     self.connections[address].append(connection)
                 return connection
@@ -160,21 +204,55 @@
                          + self.connections_reservations[address])
             if infinite_pool_size or pool_size < max_pool_size:
                 # there's room for a new connection
                 self.connections_reservations[address] += 1
                 return connection_creator
         return None
 
-    async def _acquire(self, address, deadline, liveness_check_timeout):
+    async def _re_auth_connection(self, connection, auth, force):
+        if auth:
+            # Assert session auth is supported by the protocol.
+            # The Bolt implementation will try as hard as it can to make the
+            # re-auth work. So if the session auth token is identical to the
+            # driver auth token, the connection doesn't have to do anything so
+            # it won't fail regardless of the protocol version.
+            connection.assert_re_auth_support()
+        new_auth_manager = auth or self.pool_config.auth
+        log_auth = "******" if auth else "None"
+        new_auth = await AsyncUtil.callback(new_auth_manager.get_auth)
+        try:
+            updated = connection.re_auth(new_auth, new_auth_manager,
+                                         force=force)
+            log.debug("[#%04X]  _: <POOL> checked re_auth auth=%s updated=%s "
+                      "force=%s",
+                      connection.local_port, log_auth, updated, force)
+        except Exception as exc:
+            log.debug("[#%04X]  _: <POOL> check re_auth failed %r auth=%s "
+                      "force=%s",
+                      connection.local_port, exc, log_auth, force)
+            raise
+        assert not force or updated  # force=True implies updated=True
+        if force:
+            await connection.send_all()
+            await connection.fetch_all()
+
+    async def _acquire(
+        self, address, auth, deadline, liveness_check_timeout
+    ):
         """ Acquire a connection to a given address from the pool.
         The address supplied should always be an IP address, not
         a host name.
 
         This method is thread safe.
         """
+        if auth is None:
+            auth = AcquireAuth(None)
+        force_auth = auth.force_auth
+        auth = auth.auth
+
         async def health_check(connection_, deadline_):
             if (connection_.closed()
                     or connection_.defunct()
                     or connection_.stale()):
                 return False
             if liveness_check_timeout is not None:
                 if connection_.is_idle_for(liveness_check_timeout):
@@ -189,21 +267,41 @@
 
         while True:
             # try to find a free connection in the pool
             connection = await self._acquire_from_pool_checked(
                 address, health_check, deadline
             )
             if connection:
-                log.debug("[#%04X]  _: <POOL> handing out existing connection "
-                          "%s", connection.local_port,
-                          connection.connection_id)
+                log.debug("[#%04X]  _: <POOL> picked existing connection %s",
+                          connection.local_port, connection.connection_id)
+                try:
+                    await self._re_auth_connection(
+                        connection, auth, force_auth
+                    )
+                except ConfigurationError:
+                    if auth:
+                        # protocol version lacks support for re-auth
+                        # => session auth token is not supported
+                        raise
+                    # expiring tokens supported by flushing the pool
+                    # => give up this connection
+                    log.debug("[#%04X]  _: <POOL> backwards compatible "
+                              "auth token refresh: purge connection",
+                              connection.local_port)
+                    await connection.close()
+                    await self.release(connection)
+                    continue
+                log.debug("[#%04X]  _: <POOL> handing out existing connection",
+                          connection.local_port)
                 return connection
             # all connections in pool are in-use
             with self.lock:
-                connection_creator = self._acquire_new_later(address, deadline)
+                connection_creator = self._acquire_new_later(
+                    address, auth, deadline,
+                )
                 if connection_creator:
                     break
 
                 # failed to obtain a connection from pool because the
                 # pool is full and no free connection in the pool
                 timeout = deadline.to_timeout()
                 if (
@@ -216,23 +314,25 @@
                         "{!r}s (timeout)".format(deadline.original_timeout)
                     )
         log.debug("[#0000]  _: <POOL> trying to hand out new connection")
         return await connection_creator()
 
     @abc.abstractmethod
     async def acquire(
-        self, access_mode, timeout, database, bookmarks, liveness_check_timeout
+        self, access_mode, timeout, database, bookmarks, auth: AcquireAuth,
+        liveness_check_timeout
     ):
         """ Acquire a connection to a server that can satisfy a set of parameters.
 
         :param access_mode:
         :param timeout: timeout for the core acquisition
             (excluding potential preparation like fetching routing tables).
         :param database:
         :param bookmarks:
+        :param auth:
         :param liveness_check_timeout:
         """
         ...
 
     def kill_and_release(self, *connections):
         """ Release connections back into the pool after closing them.
 
@@ -259,32 +359,32 @@
         cancelled = None
         for connection in connections:
             if not (connection.defunct()
                     or connection.closed()
                     or connection.is_reset):
                 if cancelled is not None:
                     log.debug(
-                        "[#%04X]  _: <POOL> released unclean connection %s",
+                        "[#%04X]  _: <POOL> kill unclean connection %s",
                         connection.local_port, connection.connection_id
                     )
                     connection.kill()
                     continue
                 try:
                     log.debug(
-                        "[#%04X]  _: <POOL> released unclean connection %s",
+                        "[#%04X]  _: <POOL> release unclean connection %s",
                         connection.local_port, connection.connection_id
                     )
                     await connection.reset()
-                except (Neo4jError, DriverError, BoltError) as e:
+                except (Neo4jError, DriverError, BoltError) as exc:
                     log.debug("[#%04X]  _: <POOL> failed to reset connection "
-                              "on release: %r", connection.local_port, e)
-                except asyncio.CancelledError as e:
+                              "on release: %r", connection.local_port, exc)
+                except asyncio.CancelledError as exc:
                     log.debug("[#%04X]  _: <POOL> cancelled reset connection "
-                              "on release: %r", connection.local_port, e)
-                    cancelled = e
+                              "on release: %r", connection.local_port, exc)
+                    cancelled = exc
                     connection.kill()
         with self.lock:
             for connection in connections:
                 connection.in_use = False
                 log.debug(
                     "[#%04X]  _: <POOL> released %s",
                     connection.local_port, connection.connection_id
@@ -347,14 +447,35 @@
         await self._close_connections(closable_connections)
 
     def on_write_failure(self, address):
         raise WriteServiceUnavailable(
             "No write service available for pool {}".format(self)
         )
 
+    async def on_neo4j_error(self, error, connection):
+        assert isinstance(error, Neo4jError)
+        if error._unauthenticates_all_connections():
+            address = connection.unresolved_address
+            log.debug(
+                "[#0000]  _: <POOL> mark all connections to %r as "
+                "unauthenticated", address
+            )
+            with self.lock:
+                for connection in self.connections.get(address, ()):
+                    connection.mark_unauthenticated()
+        if error._requires_new_credentials():
+            await AsyncUtil.callback(
+                connection.auth_manager.on_auth_expired,
+                connection.auth
+            )
+        if (isinstance(error, TokenExpired)
+            and not isinstance(self.pool_config.auth, (AsyncStaticAuthManager,
+                                                       StaticAuthManager))):
+            error.__class__ = TokenExpiredRetryable
+
     async def close(self):
         """ Close all connections and empty the pool.
         This method is thread safe.
         """
         log.debug("[#0000]  _: <POOL> close")
         try:
             connections = []
@@ -366,28 +487,27 @@
         except TypeError:
             pass
 
 
 class AsyncBoltPool(AsyncIOPool):
 
     @classmethod
-    def open(cls, address, *, auth, pool_config, workspace_config):
+    def open(cls, address, *, pool_config, workspace_config):
         """Create a new BoltPool
 
         :param address:
-        :param auth:
         :param pool_config:
         :param workspace_config:
         :returns: BoltPool
         """
 
-        async def opener(addr, deadline):
+        async def opener(addr, auth_manager, deadline):
             return await AsyncBolt.open(
-                addr, auth=auth, deadline=deadline, routing_context=None,
-                pool_config=pool_config
+                addr, auth_manager=auth_manager, deadline=deadline,
+                routing_context=None, pool_config=pool_config
             )
 
         pool = cls(opener, pool_config, workspace_config, address)
         log.debug("[#0000]  _: <POOL> created, direct address %r", address)
         return pool
 
     def __init__(self, opener, pool_config, workspace_config, address):
@@ -395,53 +515,53 @@
         self.address = address
 
     def __repr__(self):
         return "<{} address={!r}>".format(self.__class__.__name__,
                                           self.address)
 
     async def acquire(
-        self, access_mode, timeout, database, bookmarks, liveness_check_timeout
+        self, access_mode, timeout, database, bookmarks, auth: AcquireAuth,
+        liveness_check_timeout
     ):
         # The access_mode and database is not needed for a direct connection,
         # it's just there for consistency.
         log.debug("[#0000]  _: <POOL> acquire direct connection, "
                   "access_mode=%r, database=%r", access_mode, database)
         deadline = Deadline.from_timeout_or_deadline(timeout)
         return await self._acquire(
-            self.address, deadline, liveness_check_timeout
+            self.address, auth, deadline, liveness_check_timeout
         )
 
 
 class AsyncNeo4jPool(AsyncIOPool):
     """ Connection pool with routing table.
     """
 
     @classmethod
-    def open(cls, *addresses, auth, pool_config, workspace_config,
+    def open(cls, *addresses, pool_config, workspace_config,
              routing_context=None):
         """Create a new Neo4jPool
 
         :param addresses: one or more address as positional argument
-        :param auth:
         :param pool_config:
         :param workspace_config:
         :param routing_context:
         :returns: Neo4jPool
         """
 
         address = addresses[0]
         if routing_context is None:
             routing_context = {}
         elif "address" in routing_context:
             raise ConfigurationError("The key 'address' is reserved for routing context.")
         routing_context["address"] = str(address)
 
-        async def opener(addr, deadline):
+        async def opener(addr, auth_manager, deadline):
             return await AsyncBolt.open(
-                addr, auth=auth, deadline=deadline,
+                addr, auth_manager=auth_manager, deadline=deadline,
                 routing_context=routing_context, pool_config=pool_config
             )
 
         pool = cls(opener, pool_config, workspace_config, address)
         log.debug("[#0000]  _: <POOL> created, routing address %r", address)
         return pool
 
@@ -474,67 +594,74 @@
                 self.routing_tables[database] = RoutingTable(
                     database=database,
                     routers=[self.address]
                 )
             return self.routing_tables[database]
 
     async def fetch_routing_info(
-        self, address, database, imp_user, bookmarks, acquisition_timeout
+        self, address, database, imp_user, bookmarks, auth, acquisition_timeout
     ):
         """ Fetch raw routing info from a given router address.
 
         :param address: router address
         :param database: the database name to get routing table for
         :param imp_user: the user to impersonate while fetching the routing
                          table
         :type imp_user: str or None
         :param bookmarks: iterable of bookmark values after which the routing
                           info should be fetched
+        :param auth: auth
         :param acquisition_timeout: connection acquisition timeout
 
         :returns: list of routing records, or None if no connection
             could be established or if no readers or writers are present
         :raise ServiceUnavailable: if the server does not support
             routing, or if routing support is broken or outdated
         """
         deadline = Deadline.from_timeout_or_deadline(acquisition_timeout)
         log.debug("[#0000]  _: <POOL> _acquire router connection, "
                   "database=%r, address=%r", database, address)
-        cx = await self._acquire(address, deadline, None)
+        if auth:
+            auth = copy(auth)
+            auth.force_auth = False
+        cx = await self._acquire(address, auth, deadline, None)
         try:
             routing_table = await cx.route(
                 database=database or self.workspace_config.database,
                 imp_user=imp_user or self.workspace_config.impersonated_user,
                 bookmarks=bookmarks
             )
         finally:
             await self.release(cx)
         return routing_table
 
     async def fetch_routing_table(
-        self, *, address, acquisition_timeout, database, imp_user, bookmarks
+        self, *, address, acquisition_timeout, database, imp_user,
+        bookmarks, auth
     ):
         """ Fetch a routing table from a given router address.
 
         :param address: router address
         :param acquisition_timeout: connection acquisition timeout
         :param database: the database name
         :type: str
         :param imp_user: the user to impersonate while fetching the routing
                          table
         :type imp_user: str or None
         :param bookmarks: bookmarks used when fetching routing table
+        :param auth: auth
 
         :returns: a new RoutingTable instance or None if the given router is
                  currently unable to provide routing information
         """
         new_routing_info = None
         try:
             new_routing_info = await self.fetch_routing_info(
-                address, database, imp_user, bookmarks, acquisition_timeout
+                address, database, imp_user, bookmarks, auth,
+                acquisition_timeout
             )
         except Neo4jError as e:
             # checks if the code is an error that is caused by the client. In
             # this case there is no sense in trying to fetch a RT from another
             # router. Hence, the driver should fail fast during discovery.
             if e._is_fatal_during_discovery():
                 raise
@@ -572,16 +699,16 @@
                       "server %s", address)
             return None
 
         # At least one of each is fine, so return this table
         return new_routing_table
 
     async def _update_routing_table_from(
-        self, *routers, database, imp_user, bookmarks, acquisition_timeout,
-        database_callback
+        self, *routers, database, imp_user, bookmarks, auth,
+        acquisition_timeout, database_callback
     ):
         """ Try to update routing tables with the given routers.
 
         :returns: True if the routing table is successfully updated,
         otherwise False
         """
         if routers:
@@ -589,15 +716,16 @@
                       "table from {}".format(", ".join(map(repr, routers))))
         for router in routers:
             async for address in AsyncNetworkUtil.resolve_address(
                 router, resolver=self.pool_config.resolver
             ):
                 new_routing_table = await self.fetch_routing_table(
                     address=address, acquisition_timeout=acquisition_timeout,
-                    database=database, imp_user=imp_user, bookmarks=bookmarks
+                    database=database, imp_user=imp_user, bookmarks=bookmarks,
+                    auth=auth
                 )
                 if new_routing_table is not None:
                     new_database = new_routing_table.database
                     old_routing_table = await self.get_or_create_routing_table(
                         new_database
                     )
                     old_routing_table.update(new_routing_table)
@@ -609,25 +737,26 @@
                     if callable(database_callback):
                         database_callback(new_database)
                     return True
             await self.deactivate(router)
         return False
 
     async def update_routing_table(
-        self, *, database, imp_user, bookmarks, acquisition_timeout=None,
-        database_callback=None
+        self, *, database, imp_user, bookmarks, auth=None,
+        acquisition_timeout=None, database_callback=None
     ):
         """ Update the routing table from the first router able to provide
         valid routing information.
 
         :param database: The database name
         :param imp_user: the user to impersonate while fetching the routing
                          table
         :type imp_user: str or None
         :param bookmarks: bookmarks used when fetching routing table
+        :param auth: auth
         :param acquisition_timeout: connection acquisition timeout
         :param database_callback: A callback function that will be called with
             the database name as only argument when a new routing table has been
             acquired. This database name might different from `database` if that
             was None and the underlying protocol supports reporting back the
             actual database.
 
@@ -641,32 +770,32 @@
             prefer_initial_routing_address = \
                 self.routing_tables[database].initialized_without_writers
 
             if prefer_initial_routing_address:
                 # TODO: Test this state
                 if await self._update_routing_table_from(
                     self.address, database=database,
-                    imp_user=imp_user, bookmarks=bookmarks,
+                    imp_user=imp_user, bookmarks=bookmarks, auth=auth,
                     acquisition_timeout=acquisition_timeout,
                     database_callback=database_callback
                 ):
                     # Why is only the first initial routing address used?
                     return
             if await self._update_routing_table_from(
-                *(existing_routers - {self.address}),
-                database=database, imp_user=imp_user, bookmarks=bookmarks,
+                *(existing_routers - {self.address}), database=database,
+                imp_user=imp_user, bookmarks=bookmarks, auth=auth,
                 acquisition_timeout=acquisition_timeout,
                 database_callback=database_callback
             ):
                 return
 
             if not prefer_initial_routing_address:
                 if await self._update_routing_table_from(
                     self.address, database=database,
-                    imp_user=imp_user, bookmarks=bookmarks,
+                    imp_user=imp_user, bookmarks=bookmarks, auth=auth,
                     acquisition_timeout=acquisition_timeout,
                     database_callback=database_callback
                 ):
                     # Why is only the first initial routing address used?
                     return
 
             # None of the routers have been successful, so just fail
@@ -677,15 +806,15 @@
         routing_table = await self.get_or_create_routing_table(database)
         servers = routing_table.servers()
         for address in list(self.connections):
             if address._unresolved not in servers:
                 await super(AsyncNeo4jPool, self).deactivate(address)
 
     async def ensure_routing_table_is_fresh(
-        self, *, access_mode, database, imp_user, bookmarks,
+        self, *, access_mode, database, imp_user, bookmarks, auth=None,
         acquisition_timeout=None, database_callback=None
     ):
         """ Update the routing table if stale.
 
         This method performs two freshness checks, before and after acquiring
         the refresh lock. If the routing table is already fresh on entry, the
         method exits immediately; otherwise, the refresh lock is acquired and
@@ -714,15 +843,15 @@
                 # table is still valid
                 log.debug("[#0000]  _: <POOL> using existing routing table %r",
                           routing_table)
                 return False
 
             await self.update_routing_table(
                 database=database, imp_user=imp_user, bookmarks=bookmarks,
-                acquisition_timeout=acquisition_timeout,
+                auth=auth, acquisition_timeout=acquisition_timeout,
                 database_callback=database_callback
             )
             await self.update_connection_pool(database=database)
 
             return True
 
     async def _select_address(self, *, access_mode, database):
@@ -751,15 +880,16 @@
             else:
                 raise WriteServiceUnavailable(
                     "No write service currently available"
                 )
         return choice(addresses_by_usage[min(addresses_by_usage)])
 
     async def acquire(
-        self, access_mode, timeout, database, bookmarks, liveness_check_timeout
+        self, access_mode, timeout, database, bookmarks,
+        auth: t.Optional[AcquireAuth], liveness_check_timeout
     ):
         if access_mode not in (WRITE_ACCESS, READ_ACCESS):
             raise ClientError("Non valid 'access_mode'; {}".format(access_mode))
         if not timeout:
             raise ClientError("'timeout' must be a float larger than 0; {}"
                               .format(timeout))
 
@@ -771,15 +901,15 @@
         #         bookmarks=bookmarks, acquisition_timeout=timeout
         #     )
 
         log.debug("[#0000]  _: <POOL> acquire routing connection, "
                   "access_mode=%r, database=%r", access_mode, database)
         await self.ensure_routing_table_is_fresh(
             access_mode=access_mode, database=database,
-            imp_user=None, bookmarks=bookmarks,
+            imp_user=None, bookmarks=bookmarks, auth=auth,
             acquisition_timeout=timeout
         )
 
         while True:
             try:
                 # Get an address for a connection that have the fewest in-use
                 # connections.
@@ -790,15 +920,15 @@
                 raise SessionExpired("Failed to obtain connection towards '%s' server." % access_mode) from err
             try:
                 log.debug("[#0000]  _: <POOL> acquire address, database=%r "
                           "address=%r", database, address)
                 deadline = Deadline.from_timeout_or_deadline(timeout)
                 # should always be a resolved address
                 connection = await self._acquire(
-                    address, deadline, liveness_check_timeout
+                    address, auth, deadline, liveness_check_timeout,
                 )
             except (ServiceUnavailable, SessionExpired):
                 await self.deactivate(address=address)
             else:
                 return connection
 
     async def deactivate(self, address):
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/work/__init__.py` & `neo4j-5.8.0/src/neo4j/_async/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async/work/result.py` & `neo4j-5.8.0/src/neo4j/_async/work/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,31 +15,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from __future__ import annotations
 
 import typing as t
-from collections import (
-    deque,
-    namedtuple,
-)
+from collections import deque
 from warnings import warn
 
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
 from ..._async_compat.util import AsyncUtil
 from ..._codec.hydration import BrokenHydrationObject
 from ..._data import (
     Record,
     RecordTableRowExporter,
 )
-from ..._meta import experimental
 from ..._work import (
     EagerResult,
     ResultSummary,
 )
 from ...exceptions import (
     ResultConsumedError,
     ResultNotSingleError,
@@ -278,15 +274,15 @@
                 await self._connection.fetch_message()
 
     async def _buffer(self, n=None):
         """Try to fill `self._record_buffer` with n records.
 
         Might end up with more records in the buffer if the fetch size makes it
         overshoot.
-        Might ent up with fewer records in the buffer if there are not enough
+        Might end up with fewer records in the buffer if there are not enough
         records available.
         """
         if self._out_of_scope:
             raise ResultConsumedError(self, _RESULT_OUT_OF_SCOPE_ERROR)
         if self._consumed:
             raise ResultConsumedError(self, _RESULT_CONSUMED_ERROR)
         if n is not None and len(self._record_buffer) >= n:
@@ -604,34 +600,29 @@
         .. versionchanged:: 5.0
             Can raise :exc:`ResultConsumedError`.
 
         .. seealso:: :meth:`.Record.data`
         """
         return [record.data(*keys) async for record in self]
 
-    @experimental(
-        "Result.to_eager_result is experimental. "
-        "It might be changed or removed any time even without prior notice."
-    )
     async def to_eager_result(self) -> EagerResult:
         """Convert this result to an :class:`.EagerResult`.
 
         This method exhausts the result and triggers a :meth:`.consume`.
 
         :returns: all remaining records in the result stream, the result's
             summary, and keys as an :class:`.EagerResult` instance.
 
         :raises ResultConsumedError: if the transaction from which this result
             was obtained has been closed or the Result has been explicitly
             consumed.
 
-        **This is experimental.** (See :ref:`filter-warnings-ref`)
-        It might be changed or removed any time even without prior notice.
-
         .. versionadded:: 5.5
+
+        .. versionchanged:: 5.8 stabilized from experimental
         """
 
         await self._buffer_all()
         return EagerResult(
             keys=list(self.keys()),
             records=await AsyncUtil.list(self),
             summary=await self.consume()
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/work/session.py` & `neo4j-5.8.0/src/neo4j/_async/work/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,41 @@
 # limitations under the License.
 
 
 from __future__ import annotations
 
 import asyncio
 import typing as t
+import warnings
 from logging import getLogger
 from random import random
 from time import perf_counter
 
 from ..._async_compat import async_sleep
 from ..._async_compat.util import AsyncUtil
 from ..._conf import SessionConfig
-from ..._meta import deprecated
+from ..._meta import (
+    deprecated,
+    PreviewWarning,
+)
 from ..._work import Query
 from ...api import (
     Bookmarks,
     READ_ACCESS,
     WRITE_ACCESS,
 )
 from ...exceptions import (
     ClientError,
     DriverError,
     Neo4jError,
     ServiceUnavailable,
     SessionExpired,
     TransactionError,
 )
+from ..auth_management import AsyncAuthManagers
 from .result import AsyncResult
 from .transaction import (
     AsyncManagedTransaction,
     AsyncTransaction,
 )
 from .workspace import AsyncWorkspace
 
@@ -93,15 +98,25 @@
     _auto_result = None
 
     # The state this session is in.
     _state_failed = False
 
     def __init__(self, pool, session_config):
         assert isinstance(session_config, SessionConfig)
+        if session_config.auth is not None:
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    "ignore", message=r".*\bAuth managers\b.*",
+                    category=PreviewWarning
+                )
+                session_config.auth = AsyncAuthManagers.static(
+                    session_config.auth
+                )
         super().__init__(pool, session_config)
+        self._config = session_config
         self._initialize_bookmarks(session_config.bookmarks)
         self._bookmark_manager = session_config.bookmark_manager
 
     async def __aenter__(self) -> AsyncSession:
         return self
 
     async def __aexit__(self, exception_type, exception_value, traceback):
@@ -109,19 +124,21 @@
             if issubclass(exception_type, asyncio.CancelledError):
                 self._handle_cancellation(message="__aexit__")
                 self._closed = True
                 return
             self._state_failed = True
         await self.close()
 
-    async def _connect(self, access_mode, **access_kwargs):
+    async def _connect(self, access_mode, **acquire_kwargs):
         if access_mode is None:
             access_mode = self._config.default_access_mode
         try:
-            await super()._connect(access_mode, **access_kwargs)
+            await super()._connect(
+                access_mode, auth=self._config.auth, **acquire_kwargs
+            )
         except asyncio.CancelledError:
             self._handle_cancellation(message="_connect")
             raise
 
     async def _disconnect(self, sync=False):
         try:
             return await super()._disconnect(sync=sync)
@@ -158,14 +175,19 @@
     async def _get_server_info(self):
         assert not self._connection
         await self._connect(READ_ACCESS, liveness_check_timeout=0)
         server_info = self._connection.server_info
         await self._disconnect()
         return server_info
 
+    async def _verify_authentication(self):
+        assert not self._connection
+        await self._connect(READ_ACCESS, force_auth=True)
+        await self._disconnect()
+
     async def close(self) -> None:
         """Close the session.
 
         This will release any borrowed resources, such as connections, and will
         roll back any outstanding transactions.
         """
         if self._closed:
```

### Comparing `neo4j-5.7.0/src/neo4j/_async/work/transaction.py` & `neo4j-5.8.0/src/neo4j/_async/work/transaction.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async/work/workspace.py` & `neo4j-5.8.0/src/neo4j/_async/work/workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 )
 from ...api import Bookmarks
 from ...exceptions import (
     ServiceUnavailable,
     SessionError,
     SessionExpired,
 )
-from ..io import AsyncNeo4jPool
+from ..io import (
+    AcquireAuth,
+    AsyncNeo4jPool,
+)
 
 
 log = logging.getLogger("neo4j")
 
 
 class AsyncWorkspace:
 
@@ -126,16 +129,21 @@
         )
 
     async def _update_bookmark(self, bookmark):
         if not bookmark:
             return
         await self._update_bookmarks((bookmark,))
 
-    async def _connect(self, access_mode, **acquire_kwargs):
+    async def _connect(self, access_mode, auth=None, **acquire_kwargs):
         acquisition_timeout = self._config.connection_acquisition_timeout
+        auth = AcquireAuth(
+            auth,
+            force_auth=acquire_kwargs.pop("force_auth", False),
+        )
+
         if self._connection:
             # TODO: Investigate this
             # log.warning("FIXME: should always disconnect before connect")
             await self._connection.send_all()
             await self._connection.fetch_all()
             await self._disconnect()
         if not self._cached_database:
@@ -150,22 +158,24 @@
                 # we shall use this database explicitly for all subsequent
                 # actions within this session.
                 log.debug("[#0000]  _: <WORKSPACE> resolve home database")
                 await self._pool.update_routing_table(
                     database=self._config.database,
                     imp_user=self._config.impersonated_user,
                     bookmarks=await self._get_bookmarks(),
+                    auth=auth,
                     acquisition_timeout=acquisition_timeout,
                     database_callback=self._set_cached_database
                 )
         acquire_kwargs_ = {
             "access_mode": access_mode,
             "timeout": acquisition_timeout,
             "database": self._config.database,
             "bookmarks": await self._get_bookmarks(),
+            "auth": auth,
             "liveness_check_timeout": None,
         }
         acquire_kwargs_.update(acquire_kwargs)
         self._connection = await self._pool.acquire(**acquire_kwargs_)
         self._connection_access_mode = access_mode
 
     async def _disconnect(self, sync=False):
```

### Comparing `neo4j-5.7.0/src/neo4j/_async_compat/__init__.py` & `neo4j-5.8.0/src/neo4j/_async_compat/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async_compat/concurrency.py` & `neo4j-5.8.0/src/neo4j/_async_compat/concurrency.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async_compat/network/__init__.py` & `neo4j-5.8.0/src/neo4j/_async_compat/network/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async_compat/network/_bolt_socket.py` & `neo4j-5.8.0/src/neo4j/_async_compat/network/_bolt_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # limitations under the License.
 
 
 from __future__ import annotations
 
 import asyncio
 import logging
-import selectors
 import struct
 import typing as t
 from socket import (
     AF_INET,
     AF_INET6,
     SHUT_RDWR,
     SO_KEEPALIVE,
```

### Comparing `neo4j-5.7.0/src/neo4j/_async_compat/network/_util.py` & `neo4j-5.8.0/src/neo4j/_async_compat/network/_util.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async_compat/shims/__init__.py` & `neo4j-5.8.0/src/neo4j/_async_compat/shims/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_async_compat/util.py` & `neo4j-5.8.0/src/neo4j/_async_compat/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
 import typing as t
 from functools import wraps
 
-from .._meta import experimental
-
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
     _T = t.TypeVar("_T")
     _P = te.ParamSpec("_P")
```

### Comparing `neo4j-5.7.0/src/neo4j/_codec/__init__.py` & `neo4j-5.8.0/src/neo4j/_codec/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/__init__.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/_common.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/_interface/__init__.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/v1/__init__.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/v1/hydration_handler.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/v1/hydration_handler.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/v1/spatial.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/v1/spatial.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/v1/temporal.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/v1/temporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # limitations under the License.
 
 
 from datetime import (
     datetime,
     time,
     timedelta,
+    timezone,
 )
 
 from ...._optional_deps import (
     np,
     pd,
 )
 from ....time import (
@@ -34,14 +35,17 @@
     MIN_YEAR,
     NANO_SECONDS,
     Time,
 )
 from ...packstream import Structure
 
 
+ANY_BUILTIN_DATETIME = datetime(1970, 1, 1)
+
+
 def get_date_unix_epoch():
     return Date(1970, 1, 1)
 
 
 def get_date_unix_epoch_ordinal():
     return get_date_unix_epoch().to_ordinal()
 
@@ -168,18 +172,23 @@
         seconds, nanoseconds = seconds_and_nanoseconds(value)
         return Structure(b"f", seconds, nanoseconds, tz.zone)
     elif hasattr(tz, "key") and tz.key and isinstance(tz.key, str):
         # with named zoneinfo (Python 3.9+) time zone
         seconds, nanoseconds = seconds_and_nanoseconds(value)
         return Structure(b"f", seconds, nanoseconds, tz.key)
     else:
+        if isinstance(tz, timezone):
+            # offset of the timezone is constant, so any date will do
+            offset = tz.utcoffset(ANY_BUILTIN_DATETIME)
+        else:
+            offset = tz.utcoffset(value)
         # with time offset
         seconds, nanoseconds = seconds_and_nanoseconds(value)
         return Structure(b"F", seconds, nanoseconds,
-                         int(tz.utcoffset(value).total_seconds()))
+                         int(offset.total_seconds()))
 
 
 if np is not None:
     def dehydrate_np_datetime(value):
         """ Dehydrator for `numpy.datetime64` values.
 
         :param value:
```

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/v2/__init__.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/v2/hydration_handler.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/v2/hydration_handler.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/hydration/v2/temporal.py` & `neo4j-5.8.0/src/neo4j/_codec/hydration/v2/temporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,20 @@
         return Structure(b"i", seconds, nanoseconds, tz.zone)
     elif hasattr(tz, "key") and tz.key and isinstance(tz.key, str):
         # with named zoneinfo (Python 3.9+) time zone
         seconds, nanoseconds = seconds_and_nanoseconds(value)
         return Structure(b"i", seconds, nanoseconds, tz.key)
     else:
         # with time offset
+        if isinstance(tz, timezone):
+            # offset of the timezone is constant, so any date will do
+            offset = tz.utcoffset(datetime(1970, 1, 1))
+        else:
+            offset = tz.utcoffset(value)
         seconds, nanoseconds = seconds_and_nanoseconds(value)
-        offset = tz.utcoffset(value)
         if offset.microseconds:
             raise ValueError("Bolt protocol does not support sub-second "
                              "UTC offsets.")
         offset_seconds = offset.days * 86400 + offset.seconds
         return Structure(b"I", seconds, nanoseconds, offset_seconds)
```

### Comparing `neo4j-5.7.0/src/neo4j/_codec/packstream/__init__.py` & `neo4j-5.8.0/src/neo4j/_codec/packstream/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/packstream/_common.py` & `neo4j-5.8.0/src/neo4j/_codec/packstream/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_codec/packstream/v1/__init__.py` & `neo4j-5.8.0/src/neo4j/_codec/packstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_conf.py` & `neo4j-5.8.0/src/neo4j/_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,14 +403,17 @@
     user_agent = get_user_agent()
     # Specify the client agent name.
 
     #: Socket Keep Alive (Python and .NET Driver Specific)
     keep_alive = True
     # Specify whether TCP keep-alive should be enabled.
 
+    #: Authentication provider
+    auth = None
+
     #: Lowest notification severity for the server to return
     notifications_min_severity = None
 
     #: List of notification categories for the server to ignore
     notifications_disabled_categories = None
 
     def get_ssl_context(self):
@@ -493,28 +496,31 @@
     fetch_size = 1000
 
     #: User to impersonate
     impersonated_user = None
     # Note that you need appropriate permissions to do so.
 
     #: Bookmark Manager
-    bookmark_manager = ExperimentalOption(None)
+    bookmark_manager = None
     # Specify the bookmark manager to be used for sessions by default.
 
 
 class SessionConfig(WorkspaceConfig):
     """ Session configuration.
     """
 
     #: Bookmarks
     bookmarks = None
 
     #: Default AccessMode
     default_access_mode = WRITE_ACCESS
 
+    #: Auth token to temporarily switch the user
+    auth = None
+
     #: Lowest notification severity for the server to return
     notifications_min_severity = None
 
     #: List of notification categories for the server to ignore
     notifications_disabled_categories = None
```

### Comparing `neo4j-5.7.0/src/neo4j/_data.py` & `neo4j-5.8.0/src/neo4j/_data.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_deadline.py` & `neo4j-5.8.0/src/neo4j/_deadline.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_exceptions.py` & `neo4j-5.8.0/src/neo4j/_exceptions.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_meta.py` & `neo4j-5.8.0/src/neo4j/_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 _FuncT = t.TypeVar("_FuncT", bound=t.Callable)
 
 
 # Can be automatically overridden in builds
 package = "neo4j"
-version = "5.7.0"
+version = "5.8.0"
 deprecated_package = False
 
 
 def get_user_agent():
     """ Obtain the default user agent string sent to the server after
     a successful handshake.
     """
@@ -90,31 +90,50 @@
     def decorator(f):
         return property(deprecated(message)(f))
     return t.cast(property, decorator)
 
 
 class ExperimentalWarning(Warning):
     """ Base class for warnings about experimental features.
+
+    .. deprecated:: 5.8
+        we now use "preview" instead of "experimental".
     """
 
 
 def experimental_warn(message, stack_level=1):
     warn(message, category=ExperimentalWarning, stacklevel=stack_level + 1)
 
 
+class PreviewWarning(Warning):
+    """ Base class for warnings about experimental features.
+    """
+
+
+def preview_warn(message, stack_level=1):
+    message += (
+        " It might be changed without following the deprecation policy. "
+        "See also "
+        "https://github.com/neo4j/neo4j-python-driver/wiki/preview-features."
+    )
+    warn(message, category=PreviewWarning, stacklevel=stack_level + 1)
+
+
 def experimental(message) -> t.Callable[[_FuncT], _FuncT]:
     """ Decorator for tagging experimental functions and methods.
 
     ::
 
         @experimental("'foo' is an experimental function and may be "
                       "removed in a future release")
         def foo(x):
             pass
 
+    .. deprecated:: 5.8
+        we now use "preview" instead of "experimental".
     """
     def decorator(f):
         if asyncio.iscoroutinefunction(f):
             @wraps(f)
             async def inner(*args, **kwargs):
                 experimental_warn(message, stack_level=2)
                 return await f(*args, **kwargs)
@@ -127,14 +146,41 @@
                 return f(*args, **kwargs)
 
             return inner
 
     return decorator
 
 
+def preview(message) -> t.Callable[[_FuncT], _FuncT]:
+    """
+    Decorator for tagging preview functions and methods.
+
+        @preview("foo is a preview.")
+        def foo(x):
+            pass
+    """
+    def decorator(f):
+        if asyncio.iscoroutinefunction(f):
+            @wraps(f)
+            async def inner(*args, **kwargs):
+                preview_warn(message, stack_level=2)
+                return await f(*args, **kwargs)
+
+            return inner
+        else:
+            @wraps(f)
+            def inner(*args, **kwargs):
+                preview_warn(message, stack_level=2)
+                return f(*args, **kwargs)
+
+            return inner
+
+    return decorator
+
+
 def unclosed_resource_warn(obj):
     msg = f"Unclosed {obj!r}."
     trace = tracemalloc.get_object_traceback(obj)
     if trace:
         msg += "\nObject allocated at (most recent call last):\n"
         msg += "\n".join(trace.format())
     else:
```

### Comparing `neo4j-5.7.0/src/neo4j/_routing.py` & `neo4j-5.8.0/src/neo4j/_routing.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_spatial/__init__.py` & `neo4j-5.8.0/src/neo4j/_spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_sync/__init__.py` & `neo4j-5.8.0/src/neo4j/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_sync/bookmark_manager.py` & `neo4j-5.8.0/src/neo4j/_sync/bookmark_manager.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_sync/driver.py` & `neo4j-5.8.0/src/neo4j/_sync/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,18 @@
     SessionConfig,
     TrustAll,
     TrustStore,
     WorkspaceConfig,
 )
 from .._meta import (
     deprecation_warn,
-    experimental,
     experimental_warn,
-    ExperimentalWarning,
+    preview,
+    preview_warn,
+    PreviewWarning,
     unclosed_resource_warn,
 )
 from .._work import EagerResult
 from ..addressing import Address
 from ..api import (
     Auth,
     BookmarkManager,
@@ -68,14 +69,19 @@
     URI_SCHEME_BOLT,
     URI_SCHEME_BOLT_SECURE,
     URI_SCHEME_BOLT_SELF_SIGNED_CERTIFICATE,
     URI_SCHEME_NEO4J,
     URI_SCHEME_NEO4J_SECURE,
     URI_SCHEME_NEO4J_SELF_SIGNED_CERTIFICATE,
 )
+from ..auth_management import (
+    AuthManager,
+    AuthManagers,
+)
+from ..exceptions import Neo4jError
 from .bookmark_manager import (
     Neo4jBookmarkManager,
     TBmConsumer as _TBmConsumer,
     TBmSupplier as _TBmSupplier,
 )
 from .work import (
     ManagedTransaction,
@@ -87,14 +93,15 @@
 if t.TYPE_CHECKING:
     import ssl
     from enum import Enum
 
     import typing_extensions as te
 
     from .._api import T_RoutingControl
+    from ..api import _TAuth
 
 
     class _DefaultEnum(Enum):
         default = "default"
 
     _default = _DefaultEnum.default
 
@@ -111,15 +118,21 @@
     if t.TYPE_CHECKING:
 
         @classmethod
         def driver(
             cls,
             uri: str,
             *,
-            auth: t.Union[t.Tuple[t.Any, t.Any], Auth, None] = ...,
+            auth: t.Union[
+                # work around https://github.com/sphinx-doc/sphinx/pull/10880
+                # make sure TAuth is resolved in the docs
+                # TAuth,
+                t.Union[t.Tuple[t.Any, t.Any], Auth, None],
+                AuthManager,
+            ] = ...,
             max_connection_lifetime: float = ...,
             max_connection_pool_size: int = ...,
             connection_timeout: float = ...,
             trust: t.Union[
                 te.Literal["TRUST_ALL_CERTIFICATES"],
                 te.Literal["TRUST_SYSTEM_CA_SIGNED_CERTIFICATES"]
             ] = ...,
@@ -155,15 +168,21 @@
             ...
 
     else:
 
         @classmethod
         def driver(
             cls, uri: str, *,
-            auth: t.Union[t.Tuple[t.Any, t.Any], Auth, None] = None,
+            auth: t.Union[
+                # work around https://github.com/sphinx-doc/sphinx/pull/10880
+                # make sure TAuth is resolved in the docs
+                # TAuth,
+                t.Union[t.Tuple[t.Any, t.Any], Auth, None],
+                AuthManager,
+            ] = None,
             **config
         ) -> Driver:
             """Create a driver.
 
             :param uri: the connection URI for the driver,
                 see :ref:`uri-ref` for available URIs.
             :param auth: the authentication details,
@@ -171,14 +190,26 @@
             :param config: driver configuration key-word arguments,
                 see :ref:`driver-configuration-ref` for available
                 key-word arguments.
             """
 
             driver_type, security_type, parsed = parse_neo4j_uri(uri)
 
+            if not isinstance(auth, AuthManager):
+                with warnings.catch_warnings():
+                    warnings.filterwarnings(
+                        "ignore", message=r".*\bAuth managers\b.*",
+                        category=PreviewWarning
+                    )
+                    auth = AuthManagers.static(auth)
+            else:
+                preview_warn("Auth managers are a preview feature.",
+                             stack_level=2)
+            config["auth"] = auth
+
             # TODO: 6.0 - remove "trust" config option
             if "trust" in config.keys():
                 if config["trust"] not in (
                     TRUST_ALL_CERTIFICATES,
                     TRUST_SYSTEM_CA_SIGNED_CERTIFICATES
                 ):
                     from ..exceptions import ConfigurationError
@@ -248,25 +279,21 @@
                         stack_level=2
                     )
                     # TODO: 6.0 - raise instead of warning
                     # raise ValueError(
                     #     'Routing parameters are not supported with scheme '
                     #     '"bolt". Given URI "{}".'.format(uri)
                     # )
-                return cls.bolt_driver(parsed.netloc, auth=auth, **config)
+                return cls.bolt_driver(parsed.netloc, **config)
             # else driver_type == DRIVER_NEO4J
             routing_context = parse_routing_context(parsed.query)
-            return cls.neo4j_driver(parsed.netloc, auth=auth,
+            return cls.neo4j_driver(parsed.netloc,
                                     routing_context=routing_context, **config)
 
     @classmethod
-    @experimental(
-        "The bookmark manager feature is experimental. "
-        "It might be changed or removed any time even without prior notice."
-    )
     def bookmark_manager(
         cls,
         initial_bookmarks: t.Union[None, Bookmarks, t.Iterable[str]] = None,
         bookmarks_supplier: t.Optional[_TBmSupplier] = None,
         bookmarks_consumer: t.Optional[_TBmConsumer] = None
     ) -> BookmarkManager:
         """Create a :class:`.BookmarkManager` with default implementation.
@@ -319,65 +346,64 @@
             Function which will be called whenever the set of bookmarks
             handled by the bookmark manager gets updated with the new
             internal bookmark set. It will receive the new set of bookmarks
             as a :class:`.Bookmarks` object and return :data:`None`.
 
         :returns: A default implementation of :class:`BookmarkManager`.
 
-        **This is experimental.** (See :ref:`filter-warnings-ref`)
-        It might be changed or removed any time even without prior notice.
-
         .. versionadded:: 5.0
 
         .. versionchanged:: 5.3
             The bookmark manager no longer tracks bookmarks per database.
             This effectively changes the signature of almost all bookmark
             manager related methods:
 
             * ``initial_bookmarks`` is no longer a mapping from database name
               to bookmarks but plain bookmarks.
             * ``bookmarks_supplier`` no longer receives the database name as
               an argument.
             * ``bookmarks_consumer`` no longer receives the database name as
               an argument.
+
+        .. versionchanged:: 5.8 stabilized from experimental
         """
         return Neo4jBookmarkManager(
             initial_bookmarks=initial_bookmarks,
             bookmarks_supplier=bookmarks_supplier,
             bookmarks_consumer=bookmarks_consumer
         )
 
     @classmethod
-    def bolt_driver(cls, target, *, auth=None, **config):
+    def bolt_driver(cls, target, **config):
         """ Create a driver for direct Bolt server access that uses
         socket I/O and thread-based concurrency.
         """
         from .._exceptions import (
             BoltHandshakeError,
             BoltSecurityError,
         )
 
         try:
-            return BoltDriver.open(target, auth=auth, **config)
+            return BoltDriver.open(target, **config)
         except (BoltHandshakeError, BoltSecurityError) as error:
             from ..exceptions import ServiceUnavailable
             raise ServiceUnavailable(str(error)) from error
 
     @classmethod
-    def neo4j_driver(cls, *targets, auth=None, routing_context=None, **config):
+    def neo4j_driver(cls, *targets, routing_context=None, **config):
         """ Create a driver for routing-capable Neo4j service access
         that uses socket I/O and thread-based concurrency.
         """
         from .._exceptions import (
             BoltHandshakeError,
             BoltSecurityError,
         )
 
         try:
-            return Neo4jDriver.open(*targets, auth=auth, routing_context=routing_context, **config)
+            return Neo4jDriver.open(*targets, routing_context=routing_context, **config)
         except (BoltHandshakeError, BoltSecurityError) as error:
             from ..exceptions import ServiceUnavailable
             raise ServiceUnavailable(str(error)) from error
 
 
 class _Direct:
 
@@ -442,20 +468,15 @@
     _closed = False
 
     def __init__(self, pool, default_workspace_config):
         assert pool is not None
         assert default_workspace_config is not None
         self._pool = pool
         self._default_workspace_config = default_workspace_config
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore",
-                                    message=r".*\bbookmark manager\b.*",
-                                    category=ExperimentalWarning)
-            self._query_bookmark_manager = \
-                GraphDatabase.bookmark_manager()
+        self._query_bookmark_manager = GraphDatabase.bookmark_manager()
 
     def __enter__(self) -> Driver:
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -476,14 +497,17 @@
 
     @property
     def encrypted(self) -> bool:
         """Indicate whether the driver was configured to use encryption."""
         return bool(self._pool.pool_config.encrypted)
 
     def _prepare_session_config(self, **config):
+        if "auth" in config:
+            preview_warn("User switching is a preview feature.",
+                         stack_level=3)
         _normalize_notifications_config(config)
         return config
 
     if t.TYPE_CHECKING:
 
         def session(
             self,
@@ -493,14 +517,15 @@
             database: t.Optional[str] = ...,
             fetch_size: int = ...,
             impersonated_user: t.Optional[str] = ...,
             bookmarks: t.Union[t.Iterable[str], Bookmarks, None] = ...,
             default_access_mode: str = ...,
             bookmark_manager: t.Union[BookmarkManager,
                                       BookmarkManager, None] = ...,
+            auth: _TAuth = ...,
             notifications_min_severity: t.Optional[
                 T_NotificationMinimumSeverity
             ] = ...,
             notifications_disabled_categories: t.Optional[
                 t.Iterable[T_NotificationDisabledCategory]
             ] = ...,
 
@@ -535,62 +560,61 @@
             raise
         self._closed = True
 
     # overloads to work around https://github.com/python/mypy/issues/3737
     @t.overload
     def execute_query(
         self,
-        query_: str,
+        query_: te.LiteralString,
         parameters_: t.Optional[t.Dict[str, t.Any]] = None,
-        routing_: T_RoutingControl = RoutingControl.WRITERS,
+        routing_: T_RoutingControl = RoutingControl.WRITE,
         database_: t.Optional[str] = None,
         impersonated_user_: t.Optional[str] = None,
         bookmark_manager_: t.Union[
             BookmarkManager, BookmarkManager, None
         ] = ...,
+        auth_: _TAuth = None,
         result_transformer_: t.Callable[
             [Result], t.Union[EagerResult]
         ] = ...,
         **kwargs: t.Any
     ) -> EagerResult:
         ...
 
     @t.overload
     def execute_query(
         self,
-        query_: str,
+        query_: te.LiteralString,
         parameters_: t.Optional[t.Dict[str, t.Any]] = None,
-        routing_: T_RoutingControl = RoutingControl.WRITERS,
+        routing_: T_RoutingControl = RoutingControl.WRITE,
         database_: t.Optional[str] = None,
         impersonated_user_: t.Optional[str] = None,
         bookmark_manager_: t.Union[
             BookmarkManager, BookmarkManager, None
         ] = ...,
+        auth_: _TAuth = None,
         result_transformer_: t.Callable[
             [Result], t.Union[_T]
         ] = ...,
         **kwargs: t.Any
     ) -> _T:
         ...
 
-    @experimental(
-        "Driver.execute_query is experimental. "
-        "It might be changed or removed any time even without prior notice."
-    )
     def execute_query(
         self,
-        query_: str,
+        query_: te.LiteralString,
         parameters_: t.Optional[t.Dict[str, t.Any]] = None,
-        routing_: T_RoutingControl = RoutingControl.WRITERS,
+        routing_: T_RoutingControl = RoutingControl.WRITE,
         database_: t.Optional[str] = None,
         impersonated_user_: t.Optional[str] = None,
         bookmark_manager_: t.Union[
             BookmarkManager, BookmarkManager, None,
             te.Literal[_DefaultEnum.default]
         ] = _default,
+        auth_: _TAuth = None,
         result_transformer_: t.Callable[
             [Result], t.Union[t.Any]
         ] = Result.to_eager_result,
         **kwargs: t.Any
     ) -> t.Any:
         """Execute a query in a transaction function and return all results.
 
@@ -604,43 +628,44 @@
         ``CALL {} IN TRANSACTIONS`` or the older ``USING PERIODIC COMMIT``
         will not work (use :meth:`Session.run` for these).
 
         The method is roughly equivalent to::
 
             def execute_query(
                 query_, parameters_, routing_, database_, impersonated_user_,
-                bookmark_manager_, result_transformer_, **kwargs
+                bookmark_manager_, auth_, result_transformer_, **kwargs
             ):
                 def work(tx):
                     result = tx.run(query_, parameters_, **kwargs)
                     return result_transformer_(result)
 
                 with driver.session(
                     database=database_,
                     impersonated_user=impersonated_user_,
                     bookmark_manager=bookmark_manager_,
+                    auth=auth_,
                 ) as session:
-                    if routing_ == RoutingControl.WRITERS:
+                    if routing_ == RoutingControl.WRITE:
                         return session.execute_write(work)
-                    elif routing_ == RoutingControl.READERS:
+                    elif routing_ == RoutingControl.READ:
                         return session.execute_read(work)
 
         Usage example::
 
             from typing import List
 
             import neo4j
 
 
             def example(driver: neo4j.Driver) -> List[str]:
                 \"""Get the name of all 42 year-olds.\"""
                 records, summary, keys = driver.execute_query(
                     "MATCH (p:Person {age: $age}) RETURN p.name",
                     {"age": 42},
-                    routing_=neo4j.RoutingControl.READERS,  # or just "r"
+                    routing_=neo4j.RoutingControl.READ,  # or just "r"
                     database_="neo4j",
                 )
                 assert keys == ["p.name"]  # not needed, just for illustration
                 # log_summary(summary)  # log some metadata
                 return [str(record["p.name"]) for record in records]
                 # or: return [str(record[0]) for record in records]
                 # or even: return list(map(lambda r: str(r[0]), records))
@@ -649,21 +674,22 @@
 
             import neo4j
 
 
             def example(driver: neo4j.Driver) -> int:
                 \"""Call all young people "My dear" and get their count.\"""
                 record = driver.execute_query(
-                    "MATCH (p:Person) WHERE p.age <= 15 "
+                    "MATCH (p:Person) WHERE p.age <= $age "
                     "SET p.nickname = 'My dear' "
                     "RETURN count(*)",
                     # optional routing parameter, as write is default
-                    # routing_=neo4j.RoutingControl.WRITERS,  # or just "w",
+                    # routing_=neo4j.RoutingControl.WRITE,  # or just "w",
                     database_="neo4j",
                     result_transformer_=neo4j.Result.single,
+                    age=15,
                 )
                 assert record is not None  # for typechecking and illustration
                 count = record[0]
                 assert isinstance(count, int)
                 return count
 
         :param query_: cypher query to execute
@@ -692,14 +718,28 @@
             This means that all query will be executed in the security context
             of the impersonated user. For this, the user for which the
             :class:`Driver` has been created needs to have the appropriate
             permissions.
 
             See also the Session config :ref:`impersonated-user-ref`.
         :type impersonated_user_: typing.Optional[str]
+        :param auth_:
+            Authentication information to use for this query.
+
+            By default, the driver configuration is used.
+
+            **This is a preview** (see :ref:`filter-warnings-ref`).
+            It might be changed without following the deprecation policy.
+            See also
+            https://github.com/neo4j/neo4j-python-driver/wiki/preview-features
+
+            See also the Session config :ref:`session-auth-ref`.
+        :type auth_: typing.Union[
+            typing.Tuple[typing.Any, typing.Any], neo4j.Auth, None
+        ]
         :param result_transformer_:
             A function that gets passed the :class:`neo4j.Result` object
             resulting from the query and converts it to a different type. The
             result of the transformer function is returned by this method.
 
             .. warning::
 
@@ -762,32 +802,34 @@
             Specify a bookmark manager to use.
 
             If present, the bookmark manager is used to keep the query causally
             consistent with all work executed using the same bookmark manager.
 
             Defaults to the driver's :attr:`.query_bookmark_manager`.
 
-            Pass :const:`None` to disable causal consistency.
+            Pass :data:`None` to disable causal consistency.
         :type bookmark_manager_:
             typing.Union[neo4j.BookmarkManager, neo4j.BookmarkManager,
                          None]
         :param kwargs: additional keyword parameters. None of these can end
             with a single underscore. This is to avoid collisions with the
             keyword configuration parameters of this method. If you need to
             pass such a parameter, use the ``parameters_`` parameter instead.
-            These take precedence over parameters passed as ``parameters_``.
+            Parameters passed as kwargs take precedence over those passed in
+            ``parameters_``.
         :type kwargs: typing.Any
 
         :returns: the result of the ``result_transformer``
         :rtype: T
 
-        **This is experimental.** (See :ref:`filter-warnings-ref`)
-        It might be changed or removed any time even without prior notice.
-
         .. versionadded:: 5.5
+
+        .. versionchanged:: 5.8
+            * Added the ``auth_`` parameter.
+            * Stabilized from experimental.
         """
         invalid_kwargs = [k for k in kwargs if
                           k[-2:-1] != "_" and k[-1:] == "_"]
         if invalid_kwargs:
             raise ValueError(
                 "keyword parameters must not end with a single '_'. Found: %r"
                 "\nYou either misspelled an existing configuration parameter "
@@ -799,37 +841,34 @@
 
         if bookmark_manager_ is _default:
             bookmark_manager_ = self._query_bookmark_manager
         assert bookmark_manager_ is not _default
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore",
-                                    message=r".*\bbookmark_manager\b.*",
-                                    category=ExperimentalWarning)
+                                    message=r"^User switching\b.*",
+                                    category=PreviewWarning)
             session = self.session(database=database_,
                                    impersonated_user=impersonated_user_,
-                                   bookmark_manager=bookmark_manager_)
+                                   bookmark_manager=bookmark_manager_,
+                                   auth=auth_)
         with session:
-            if routing_ == RoutingControl.WRITERS:
+            if routing_ == RoutingControl.WRITE:
                 executor = session.execute_write
-            elif routing_ == RoutingControl.READERS:
+            elif routing_ == RoutingControl.READ:
                 executor = session.execute_read
             else:
                 raise ValueError("Invalid routing control value: %r"
                                  % routing_)
             return executor(
                 _work, query_, parameters, result_transformer_
             )
 
     @property
-    @experimental(
-        "Driver.query_bookmark_manager is experimental. "
-        "It might be changed or removed any time even without prior notice."
-    )
-    def query_bookmark_manager(self) -> BookmarkManager:
+    def execute_query_bookmark_manager(self) -> BookmarkManager:
         """The driver's default query bookmark manager.
 
         This is the default :class:`BookmarkManager` used by
         :meth:`.execute_query`. This can be used to causally chain
         :meth:`.execute_query` calls and sessions. Example::
 
             def example(driver: neo4j.Driver) -> None:
@@ -840,18 +879,20 @@
                     # every query inside this session will be causally chained
                     # (i.e., can read what was written by <QUERY 1>)
                     session.run("<QUERY 2>")
                 # subsequent execute_query calls will be causally chained
                 # (i.e., can read what was written by <QUERY 2>)
                 driver.execute_query("<QUERY 3>")
 
-        **This is experimental.** (See :ref:`filter-warnings-ref`)
-        It might be changed or removed any time even without prior notice.
-
         .. versionadded:: 5.5
+
+        .. versionchanged:: 5.8
+            * Renamed from ``query_bookmark_manager`` to
+              ``execute_query_bookmark_manager``.
+            * Stabilized from experimental.
         """
         return self._query_bookmark_manager
 
     if t.TYPE_CHECKING:
 
         def verify_connectivity(
             self,
@@ -864,14 +905,15 @@
             database: t.Optional[str] = ...,
             fetch_size: int = ...,
             impersonated_user: t.Optional[str] = ...,
             bookmarks: t.Union[t.Iterable[str], Bookmarks, None] = ...,
             default_access_mode: str = ...,
             bookmark_manager: t.Union[BookmarkManager,
                                       BookmarkManager, None] = ...,
+            auth: t.Union[Auth, t.Tuple[t.Any, t.Any]] = ...,
             notifications_min_severity: t.Optional[
                 T_NotificationMinimumSeverity
             ] = ...,
             notifications_disabled_categories: t.Optional[
                 t.Iterable[T_NotificationDisabledCategory]
             ] = ...,
 
@@ -880,15 +922,14 @@
             retry_delay_multiplier: float = ...,
             retry_delay_jitter_factor: float = ...
         ) -> None:
             ...
 
     else:
 
-        # TODO: 6.0 - remove config argument
         def verify_connectivity(self, **config) -> None:
             """Verify that the driver can establish a connection to the server.
 
             This verifies if the driver can establish a reading connection to a
             remote server or a cluster. Some data will be exchanged.
 
             .. note::
@@ -899,15 +940,15 @@
                 :meth:`session`.
 
                 .. warning::
                     All configuration key-word arguments are experimental.
                     They might be changed or removed in any future version
                     without prior notice.
 
-            :raises DriverError: if the driver cannot connect to the remote.
+            :raises Exception: if the driver cannot connect to the remote.
                 Use the exception to further understand the cause of the
                 connectivity problem.
 
             .. versionchanged:: 5.0
                 The undocumented return value has been removed.
                 If you need information about the remote server, use
                 :meth:`get_server_info` instead.
@@ -915,16 +956,15 @@
             if config:
                 experimental_warn(
                     "All configuration key-word arguments to "
                     "verify_connectivity() are experimental. They might be "
                     "changed or removed in any future version without prior "
                     "notice."
                 )
-            with self.session(**config) as session:
-                session._get_server_info()
+            self._get_server_info()
 
     if t.TYPE_CHECKING:
 
         def get_server_info(
             self,
             *,
             # all arguments are experimental
@@ -935,14 +975,15 @@
             database: t.Optional[str] = ...,
             fetch_size: int = ...,
             impersonated_user: t.Optional[str] = ...,
             bookmarks: t.Union[t.Iterable[str], Bookmarks, None] = ...,
             default_access_mode: str = ...,
             bookmark_manager: t.Union[BookmarkManager,
                                       BookmarkManager, None] = ...,
+            auth: t.Union[Auth, t.Tuple[t.Any, t.Any]] = ...,
             notifications_min_severity: t.Optional[
                 T_NotificationMinimumSeverity
             ] = ...,
             notifications_disabled_categories: t.Optional[
                 t.Iterable[T_NotificationDisabledCategory]
             ] = ...,
 
@@ -973,60 +1014,182 @@
                 :meth:`session`.
 
                 .. warning::
                     All configuration key-word arguments are experimental.
                     They might be changed or removed in any future version
                     without prior notice.
 
-            :raises DriverError: if the driver cannot connect to the remote.
+            :raises Exception: if the driver cannot connect to the remote.
                 Use the exception to further understand the cause of the
                 connectivity problem.
 
             .. versionadded:: 5.0
             """
             if config:
                 experimental_warn(
                     "All configuration key-word arguments to "
-                    "verify_connectivity() are experimental. They might be "
+                    "get_server_info() are experimental. They might be "
                     "changed or removed in any future version without prior "
                     "notice."
                 )
-            with self.session(**config) as session:
-                return session._get_server_info()
+            return self._get_server_info()
 
-    @experimental("Feature support query, based on Bolt protocol version and Neo4j server version will change in the future.")
     def supports_multi_db(self) -> bool:
         """ Check if the server or cluster supports multi-databases.
 
         :returns: Returns true if the server or cluster the driver connects to
             supports multi-databases, otherwise false.
 
         .. note::
-            Feature support query, based on Bolt Protocol Version and Neo4j
-            server version will change in the future.
+            Feature support query based solely on the Bolt protocol version.
+            The feature might still be disabled on the server side even if this
+            function return :const:`True`. It just guarantees that the driver
+            won't throw a :exc:`ConfigurationError` when trying to use this
+            driver feature.
         """
         with self.session() as session:
             session._connect(READ_ACCESS)
             assert session._connection
             return session._connection.supports_multiple_databases
 
+    if t.TYPE_CHECKING:
+
+        def verify_authentication(
+            self,
+            auth: t.Union[Auth, t.Tuple[t.Any, t.Any], None] = None,
+            # all other arguments are experimental
+            # they may be change or removed any time without prior notice
+            session_connection_timeout: float = ...,
+            connection_acquisition_timeout: float = ...,
+            max_transaction_retry_time: float = ...,
+            database: t.Optional[str] = ...,
+            fetch_size: int = ...,
+            impersonated_user: t.Optional[str] = ...,
+            bookmarks: t.Union[t.Iterable[str], Bookmarks, None] = ...,
+            default_access_mode: str = ...,
+            bookmark_manager: t.Union[
+                BookmarkManager, BookmarkManager, None
+            ] = ...,
+
+            # undocumented/unsupported options
+            initial_retry_delay: float = ...,
+            retry_delay_multiplier: float = ...,
+            retry_delay_jitter_factor: float = ...
+        ) -> bool:
+            ...
+
+    else:
+
+        @preview("User switching is a preview feature.")
+        def verify_authentication(
+            self,
+            auth: t.Union[Auth, t.Tuple[t.Any, t.Any], None] = None,
+            **config
+        ) -> bool:
+            """Verify that the authentication information is valid.
+
+            Like :meth:`.verify_connectivity`, but for checking authentication.
+
+            Try to establish a working read connection to the remote server or
+            a member of a cluster and exchange some data. In a cluster, there
+            is no guarantee about which server will be contacted. If the data
+            exchange is successful and the authentication information is valid,
+            :const:`True` is returned. Otherwise, the error will be matched
+            against a list of known authentication errors. If the error is on
+            that list, :const:`False` is returned indicating that the
+            authentication information is invalid. Otherwise, the error is
+            re-raised.
+
+            :param auth: authentication information to verify.
+                Same as the session config :ref:`auth-ref`.
+            :param config: accepts the same configuration key-word arguments as
+                :meth:`session`.
+
+                .. warning::
+                    All configuration key-word arguments (except ``auth``) are
+                    experimental. They might be changed or removed in any
+                    future version without prior notice.
+
+            :raises Exception: if the driver cannot connect to the remote.
+                Use the exception to further understand the cause of the
+                connectivity problem.
+
+            **This is a preview** (see :ref:`filter-warnings-ref`).
+            It might be changed without following the deprecation policy.
+            See also
+            https://github.com/neo4j/neo4j-python-driver/wiki/preview-features
+
+            .. versionadded:: 5.8
+            """
+            if config:
+                experimental_warn(
+                    "All configuration key-word arguments but auth to "
+                    "verify_authentication() are experimental. They might be "
+                    "changed or removed in any future version without prior "
+                    "notice."
+                )
+            config["auth"] = auth
+            if "database" not in config:
+                config["database"] = "system"
+            try:
+                with warnings.catch_warnings():
+                    warnings.filterwarnings(
+                        "ignore", message=r"^User switching\b.*",
+                        category=PreviewWarning
+                )
+                    session = self.session(**config)
+                with session as session:
+                    session._verify_authentication()
+            except Neo4jError as exc:
+                if exc.code in (
+                    "Neo.ClientError.Security.CredentialsExpired",
+                    "Neo.ClientError.Security.Forbidden",
+                    "Neo.ClientError.Security.TokenExpired",
+                    "Neo.ClientError.Security.Unauthorized",
+                ):
+                    return False
+                raise
+            return True
+
+
+    def supports_session_auth(self) -> bool:
+        """Check if the remote supports connection re-authentication.
+
+        :returns: Returns true if the server or cluster the driver connects to
+            supports re-authentication of existing connections, otherwise
+            false.
+
+        .. note::
+            Feature support query based solely on the Bolt protocol version.
+            The feature might still be disabled on the server side even if this
+            function return :const:`True`. It just guarantees that the driver
+            won't throw a :exc:`ConfigurationError` when trying to use this
+            driver feature.
+
+        .. versionadded:: 5.8
+        """
+        with self.session() as session:
+            session._connect(READ_ACCESS)
+            assert session._connection
+            return session._connection.supports_re_auth
+
+    def _get_server_info(self, **config) -> ServerInfo:
+        with self.session(**config) as session:
+            return session._get_server_info()
+
 
 def _work(
     tx: ManagedTransaction,
     query: str,
     parameters: t.Dict[str, t.Any],
     transformer: t.Callable[[Result], t.Union[_T]]
 ) -> _T:
     res = tx.run(query, parameters)
     if transformer is Result.to_eager_result:
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore",
-                                    message=r".*\bto_eager_result\b.*",
-                                    category=ExperimentalWarning)
-            return transformer(res)
+        return transformer(res)
     return transformer(res)
 
 
 class BoltDriver(_Direct, Driver):
     """:class:`.BoltDriver` is instantiated for ``bolt`` URIs and
     addresses a single database machine. This may be a standalone server or
     could be a specific member of a cluster.
@@ -1035,27 +1198,27 @@
     the exact host and port detailed in the URI.
 
     This class is not supposed to be instantiated externally. Use
     :meth:`GraphDatabase.driver` instead.
     """
 
     @classmethod
-    def open(cls, target, *, auth=None, **config):
+    def open(cls, target, **config):
         """
         :param target:
         :param auth:
         :param config: The values that can be specified are found in :class: `neo4j.PoolConfig` and :class: `neo4j.WorkspaceConfig`
 
         :returns:
         :rtype: :class: `neo4j.BoltDriver`
         """
         from .io import BoltPool
         address = cls.parse_target(target)
         pool_config, default_workspace_config = Config.consume_chain(config, PoolConfig, WorkspaceConfig)
-        pool = BoltPool.open(address, auth=auth, pool_config=pool_config, workspace_config=default_workspace_config)
+        pool = BoltPool.open(address, pool_config=pool_config, workspace_config=default_workspace_config)
         return cls(pool, default_workspace_config)
 
     def __init__(self, pool, default_workspace_config):
         _Direct.__init__(self, pool.address)
         Driver.__init__(self, pool, default_workspace_config)
         self._default_workspace_config = default_workspace_config
 
@@ -1083,19 +1246,19 @@
     cluster members.
 
     This class is not supposed to be instantiated externally. Use
     :meth:`GraphDatabase.driver` instead.
     """
 
     @classmethod
-    def open(cls, *targets, auth=None, routing_context=None, **config):
+    def open(cls, *targets, routing_context=None, **config):
         from .io import Neo4jPool
         addresses = cls.parse_targets(*targets)
         pool_config, default_workspace_config = Config.consume_chain(config, PoolConfig, WorkspaceConfig)
-        pool = Neo4jPool.open(*addresses, auth=auth, routing_context=routing_context, pool_config=pool_config, workspace_config=default_workspace_config)
+        pool = Neo4jPool.open(*addresses, routing_context=routing_context, pool_config=pool_config, workspace_config=default_workspace_config)
         return cls(pool, default_workspace_config)
 
     def __init__(self, pool, default_workspace_config):
         _Routing.__init__(self, [pool.address])
         Driver.__init__(self, pool, default_workspace_config)
 
     if not t.TYPE_CHECKING:
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/io/__init__.py` & `neo4j-5.8.0/src/neo4j/time/clock_implementations.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,33 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# TODO: 6.0 - remove this file
 
-"""
-This module contains the low-level functionality required for speaking
-Bolt. It is not intended to be used directly by driver users. Instead,
-the `session` module provides the main user-facing abstractions.
-"""
+
+from .._meta import deprecation_warn
+from ._clock_implementations import (
+    LibCClock,
+    PEP564Clock,
+    SafeClock,
+)
 
 
 __all__ = [
-    "Bolt",
-    "BoltPool",
-    "Neo4jPool",
-    "check_supported_server_product",
-    "ConnectionErrorHandler",
+    "SafeClock",
+    "PEP564Clock",
+    "LibCClock",
 ]
 
-
-from ._bolt import Bolt
-from ._common import (
-    check_supported_server_product,
-    ConnectionErrorHandler,
-)
-from ._pool import (
-    BoltPool,
-    Neo4jPool,
+deprecation_warn(
+    "The module `neo4j.time.clock_implementations` was made internal and will "
+    "no longer be available for import in future versions.",
+    stack_level=2
 )
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/io/_bolt.py` & `neo4j-5.8.0/src/neo4j/_sync/io/_bolt.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,24 +21,25 @@
 import abc
 import asyncio
 from collections import deque
 from logging import getLogger
 from time import perf_counter
 
 from ..._async_compat.network import BoltSocket
+from ..._async_compat.util import Util
 from ..._codec.hydration import v1 as hydration_v1
 from ..._codec.packstream import v1 as packstream_v1
 from ..._conf import PoolConfig
 from ..._deadline import Deadline
 from ..._exceptions import (
     BoltError,
     BoltHandshakeError,
 )
 from ..._meta import get_user_agent
-from ...addressing import Address
+from ...addressing import ResolvedAddress
 from ...api import (
     ServerInfo,
     Version,
 )
 from ...exceptions import (
     AuthError,
     ConfigurationError,
@@ -54,14 +55,28 @@
 )
 
 
 # Set up logger
 log = getLogger("neo4j")
 
 
+class ServerStateManagerBase(abc.ABC):
+    @abc.abstractmethod
+    def __init__(self, init_state, on_change=None):
+        ...
+
+    @abc.abstractmethod
+    def transition(self, message, metadata):
+        ...
+
+    @abc.abstractmethod
+    def failed(self):
+        ...
+
+
 class Bolt:
     """ Server connection for Bolt protocol.
 
     A :class:`.Bolt` should be constructed following a
     successful .open()
 
     Bolt handshake and takes the socket over which
@@ -100,21 +115,25 @@
 
     # Store the id of the most recent ran query to be able to reduce sent bits by
     # using the default (-1) to refer to the most recent query when pulling
     # results for it.
     most_recent_qid = None
 
     def __init__(self, unresolved_address, sock, max_connection_lifetime, *,
-                 auth=None, user_agent=None, routing_context=None,
-                 notifications_min_severity=None, notifications_disabled_categories=None):
+                 auth=None, auth_manager=None, user_agent=None,
+                 routing_context=None, notifications_min_severity=None,
+                 notifications_disabled_categories=None):
         self.unresolved_address = unresolved_address
         self.socket = sock
         self.local_port = self.socket.getsockname()[1]
-        self.server_info = ServerInfo(Address(sock.getpeername()),
-                                      self.PROTOCOL_VERSION)
+        self.server_info = ServerInfo(
+            ResolvedAddress(sock.getpeername(),
+                            host_name=unresolved_address.host),
+            self.PROTOCOL_VERSION
+        )
         # so far `connection.recv_timeout_seconds` is the only available
         # configuration hint that exists. Therefore, all hints can be stored at
         # connection level. This might change in the future.
         self.configuration_hints = {}
         self.patch = {}
         self.outbox = Outbox(
             self.socket, on_error=self._set_defunct_write,
@@ -133,43 +152,44 @@
 
         # Determine the user agent
         if user_agent:
             self.user_agent = user_agent
         else:
             self.user_agent = get_user_agent()
 
-        # Determine auth details
-        if not auth:
-            self.auth_dict = {}
-        elif isinstance(auth, tuple) and 2 <= len(auth) <= 3:
-            from ...api import Auth
-            self.auth_dict = vars(Auth("basic", *auth))
-        else:
-            try:
-                self.auth_dict = vars(auth)
-            except (KeyError, TypeError):
-                raise AuthError("Cannot determine auth details from %r" % auth)
-
-        # Check for missing password
-        try:
-            credentials = self.auth_dict["credentials"]
-        except KeyError:
-            pass
-        else:
-            if credentials is None:
-                raise AuthError("Password cannot be None")
+        self.auth = auth
+        self.auth_dict = self._to_auth_dict(auth)
+        self.auth_manager = auth_manager
 
         self.notifications_min_severity = notifications_min_severity
         self.notifications_disabled_categories = \
             notifications_disabled_categories
 
     def __del__(self):
         if not asyncio.iscoroutinefunction(self.close):
             self.close()
 
+    @abc.abstractmethod
+    def _get_server_state_manager(self) -> ServerStateManagerBase:
+        ...
+
+    @classmethod
+    def _to_auth_dict(cls, auth):
+        # Determine auth details
+        if not auth:
+            return {}
+        elif isinstance(auth, tuple) and 2 <= len(auth) <= 3:
+            from ...api import Auth
+            return vars(Auth("basic", *auth))
+        else:
+            try:
+                return vars(auth)
+            except (KeyError, TypeError):
+                raise AuthError("Cannot determine auth details from %r" % auth)
+
     @property
     def connection_id(self):
         return self.server_info._metadata.get("connection_id", "<unknown id>")
 
     @property
     @abc.abstractmethod
     def supports_multiple_results(self):
@@ -185,14 +205,28 @@
         """ Boolean flag to indicate if the connection version supports multiple
         databases.
         """
         pass
 
     @property
     @abc.abstractmethod
+    def supports_re_auth(self):
+        """Whether the connection version supports re-authentication."""
+        pass
+
+    def assert_re_auth_support(self):
+        if not self.supports_re_auth:
+            raise ConfigurationError(
+                "User switching is not supported for Bolt "
+                f"Protocol {self.PROTOCOL_VERSION!r}. Server Agent "
+                f"{self.server_info.agent!r}"
+            )
+
+    @property
+    @abc.abstractmethod
     def supports_notification_filtering(self):
         """Whether the connection version supports re-authentication."""
         pass
 
     def assert_notification_filtering_support(self):
         if not self.supports_notification_filtering:
             raise ConfigurationError(
@@ -314,21 +348,21 @@
         else:
             BoltSocket.close_socket(s)
             return protocol_version
 
     # [bolt-version-bump] search tag when changing bolt version support
     @classmethod
     def open(
-        cls, address, *, auth=None, deadline=None, routing_context=None,
-        pool_config=None
+        cls, address, *, auth_manager=None, deadline=None,
+        routing_context=None, pool_config=None
     ):
         """Open a new Bolt connection to a given server address.
 
         :param address:
-        :param auth:
+        :param auth_manager:
         :param deadline: how long to wait for the connection to be established
         :param routing_context: dict containing routing context
         :param pool_config:
 
         :returns: connected Bolt instance
 
         :raise BoltHandshakeError:
@@ -382,28 +416,42 @@
         # elif protocol_version == (4, 0):
         #     from ._bolt4 import AsyncBolt4x0
         #     bolt_cls = AsyncBolt4x0
         elif protocol_version == (3, 0):
             from ._bolt3 import Bolt3
             bolt_cls = Bolt3
         else:
-            log.debug("[#%04X]  S: <CLOSE>", s.getsockname()[1])
+            log.debug("[#%04X]  C: <CLOSE>", s.getsockname()[1])
             BoltSocket.close_socket(s)
 
             supported_versions = cls.protocol_handlers().keys()
             raise BoltHandshakeError(
                 "The neo4j server does not support communication with this "
                 "driver. This driver has support for Bolt protocols "
                 "{}.".format(tuple(map(str, supported_versions))),
                 address=address, request_data=handshake, response_data=data
             )
 
+        try:
+            auth = Util.callback(auth_manager.get_auth)
+        except asyncio.CancelledError as e:
+            log.debug("[#%04X]  C: <KILL> open auth manager failed: %r",
+                      s.getsockname()[1], e)
+            s.kill()
+            raise
+        except Exception as e:
+            log.debug("[#%04X]  C: <CLOSE> open auth manager failed: %r",
+                      s.getsockname()[1], e)
+            s.close()
+            raise
+
         connection = bolt_cls(
             address, s, pool_config.max_connection_lifetime, auth=auth,
-            user_agent=pool_config.user_agent, routing_context=routing_context,
+            auth_manager=auth_manager, user_agent=pool_config.user_agent,
+            routing_context=routing_context,
             notifications_min_severity=pool_config.notifications_min_severity,
             notifications_disabled_categories=
                 pool_config.notifications_disabled_categories
         )
 
         try:
             connection.socket.set_deadline(deadline)
@@ -445,14 +493,53 @@
             Hooks to hydrate types (mapping from type (class) to
             dehydration function). Dehydration functions receive the value of
             type understood by packstream and are free to return anything.
         """
         pass
 
     @abc.abstractmethod
+    def logon(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGON message to the outgoing queue."""
+        pass
+
+    @abc.abstractmethod
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGOFF message to the outgoing queue."""
+        pass
+
+    def mark_unauthenticated(self):
+        """Mark the connection as unauthenticated."""
+        self.auth_dict = {}
+
+    def re_auth(
+        self, auth, auth_manager, force=False,
+        dehydration_hooks=None, hydration_hooks=None,
+    ):
+        """Append LOGON, LOGOFF to the outgoing queue.
+
+        If auth is the same as the current auth, this method does nothing.
+
+        :returns: whether the auth was changed
+        """
+        new_auth_dict = self._to_auth_dict(auth)
+        if not force and new_auth_dict == self.auth_dict:
+            self.auth_manager = auth_manager
+            self.auth = auth
+            return False
+        self.logoff(dehydration_hooks=dehydration_hooks,
+                     hydration_hooks=hydration_hooks)
+        self.auth_dict = new_auth_dict
+        self.auth_manager = auth_manager
+        self.auth = auth
+        self.logon(dehydration_hooks=dehydration_hooks,
+                    hydration_hooks=hydration_hooks)
+        return True
+
+
+    @abc.abstractmethod
     def route(
         self, database=None, imp_user=None, bookmarks=None,
         dehydration_hooks=None, hydration_hooks=None
     ):
         """ Fetch a routing table from the server for the given
         `database`. For Bolt 4.3 and above, this appends a ROUTE
         message; for earlier versions, a procedure call is made via
@@ -763,15 +850,15 @@
             self.kill()
             raise error  # cancellation error should not be re-written
         if not self._closing:
             # If we fail while closing the connection, there is no need to
             # remove the connection from the pool, nor to try to close the
             # connection again.
             self.close()
-            if self.pool:
+            if self.pool and not self._get_server_state_manager().failed():
                 self.pool.deactivate(address=self.unresolved_address)
 
         # Iterate through the outstanding responses, and if any correspond
         # to COMMIT requests then raise an error to signal that we are
         # unable to confirm that the COMMIT completed successfully.
         if silent:
             return
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/io/_bolt3.py` & `neo4j-5.8.0/src/neo4j/_sync/io/_bolt3.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from __future__ import annotations
+
+import typing as t
 from enum import Enum
 from logging import getLogger
 from ssl import SSLSocket
 
 from ..._exceptions import BoltProtocolError
 from ...api import (
     READ_ACCESS,
@@ -29,15 +32,18 @@
     ConfigurationError,
     DatabaseUnavailable,
     ForbiddenOnReadOnlyDatabase,
     Neo4jError,
     NotALeader,
     ServiceUnavailable,
 )
-from ._bolt import Bolt
+from ._bolt import (
+    Bolt,
+    ServerStateManagerBase,
+)
 from ._common import (
     check_supported_server_product,
     CommitResponse,
     InitResponse,
     Response,
 )
 
@@ -49,16 +55,16 @@
     CONNECTED = "CONNECTED"
     READY = "READY"
     STREAMING = "STREAMING"
     TX_READY_OR_TX_STREAMING = "TX_READY||TX_STREAMING"
     FAILED = "FAILED"
 
 
-class ServerStateManager:
-    _STATE_TRANSITIONS = {
+class ServerStateManager(ServerStateManagerBase):
+    _STATE_TRANSITIONS: t.Dict[Enum, t.Dict[str, Enum]] = {
         ServerStates.CONNECTED: {
             "hello": ServerStates.READY,
         },
         ServerStates.READY: {
             "run": ServerStates.STREAMING,
             "begin": ServerStates.TX_READY_OR_TX_STREAMING,
         },
@@ -87,39 +93,47 @@
         state_before = self.state
         self.state = self._STATE_TRANSITIONS \
             .get(self.state, {}) \
             .get(message, self.state)
         if state_before != self.state and callable(self._on_change):
             self._on_change(state_before, self.state)
 
+    def failed(self):
+        return self.state == ServerStates.FAILED
+
 
 class Bolt3(Bolt):
     """ Protocol handler for Bolt 3.
 
     This is supported by Neo4j versions 3.5, 4.0, 4.1, 4.2, 4.3, and 4.4.
     """
 
     PROTOCOL_VERSION = Version(3, 0)
 
     supports_multiple_results = False
 
     supports_multiple_databases = False
 
+    supports_re_auth = False
+
     supports_notification_filtering = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._server_state_manager = ServerStateManager(
             ServerStates.CONNECTED, on_change=self._on_server_state_change
         )
 
     def _on_server_state_change(self, old_state, new_state):
         log.debug("[#%04X]  _: <CONNECTION> state: %s > %s", self.local_port,
                   old_state.name, new_state.name)
 
+    def _get_server_state_manager(self) -> ServerStateManagerBase:
+        return self._server_state_manager
+
     @property
     def is_reset(self):
         # We can't be sure of the server's state if there are still pending
         # responses. Unless the last message we sent was RESET. In that case
         # the server state will always be READY when we're done.
         if (self.responses and self.responses[-1]
                 and self.responses[-1].message == "reset"):
@@ -155,14 +169,22 @@
                      response=InitResponse(self, "hello", hydration_hooks,
                                            on_success=self.server_info.update),
                      dehydration_hooks=dehydration_hooks)
         self.send_all()
         self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
+    def logon(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGON message to the outgoing queue."""
+        self.assert_re_auth_support()
+
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGOFF message to the outgoing queue."""
+        self.assert_re_auth_support()
+
     def route(
         self, database=None, imp_user=None, bookmarks=None,
         dehydration_hooks=None, hydration_hooks=None
     ):
         if database is not None:
             raise ConfigurationError(
                 "Database name parameter for selecting database is not "
@@ -393,14 +415,13 @@
                     self.pool.deactivate(address=self.unresolved_address)
                 raise
             except (NotALeader, ForbiddenOnReadOnlyDatabase):
                 if self.pool:
                     self.pool.on_write_failure(address=self.unresolved_address)
                 raise
             except Neo4jError as e:
-                if self.pool and e._invalidates_all_connections():
-                    self.pool.mark_all_stale()
+                self.pool.on_neo4j_error(e, self)
                 raise
         else:
             raise BoltProtocolError("Unexpected response message with signature %02X" % summary_signature, address=self.unresolved_address)
 
         return len(details), 1
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/io/_bolt4.py` & `neo4j-5.8.0/src/neo4j/_sync/io/_bolt4.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,30 +15,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from logging import getLogger
 from ssl import SSLSocket
 
-from ..._async_compat.util import Util
 from ..._exceptions import BoltProtocolError
 from ...api import (
     READ_ACCESS,
     SYSTEM_DATABASE,
     Version,
 )
 from ...exceptions import (
     ConfigurationError,
     DatabaseUnavailable,
     ForbiddenOnReadOnlyDatabase,
     Neo4jError,
     NotALeader,
     ServiceUnavailable,
 )
-from ._bolt import Bolt
+from ._bolt import (
+    Bolt,
+    ServerStateManagerBase,
+)
 from ._bolt3 import (
     ServerStateManager,
     ServerStates,
 )
 from ._common import (
     check_supported_server_product,
     CommitResponse,
@@ -58,26 +60,31 @@
 
     PROTOCOL_VERSION = Version(4, 0)
 
     supports_multiple_results = True
 
     supports_multiple_databases = True
 
+    supports_re_auth = False
+
     supports_notification_filtering = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._server_state_manager = ServerStateManager(
             ServerStates.CONNECTED, on_change=self._on_server_state_change
         )
 
     def _on_server_state_change(self, old_state, new_state):
         log.debug("[#%04X]  _: <CONNECTION> state: %s > %s", self.local_port,
                   old_state.name, new_state.name)
 
+    def _get_server_state_manager(self) -> ServerStateManagerBase:
+        return self._server_state_manager
+
     @property
     def is_reset(self):
         # We can't be sure of the server's state if there are still pending
         # responses. Unless the last message we sent was RESET. In that case
         # the server state will always be READY when we're done.
         if (self.responses and self.responses[-1]
                 and self.responses[-1].message == "reset"):
@@ -115,14 +122,22 @@
                          on_success=self.server_info.update
                      ),
                      dehydration_hooks=dehydration_hooks)
         self.send_all()
         self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
+    def logon(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGON message to the outgoing queue."""
+        self.assert_re_auth_support()
+
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGOFF message to the outgoing queue."""
+        self.assert_re_auth_support()
+
     def route(
         self, database=None, imp_user=None, bookmarks=None,
         dehydration_hooks=None, hydration_hooks=None
     ):
         if imp_user is not None:
             raise ConfigurationError(
                 "Impersonation is not supported in Bolt Protocol {!r}. "
@@ -349,16 +364,16 @@
                     self.pool.deactivate(address=self.unresolved_address)
                 raise
             except (NotALeader, ForbiddenOnReadOnlyDatabase):
                 if self.pool:
                     self.pool.on_write_failure(address=self.unresolved_address)
                 raise
             except Neo4jError as e:
-                if self.pool and e._invalidates_all_connections():
-                    self.pool.mark_all_stale()
+                if self.pool:
+                    self.pool.on_neo4j_error(e, self)
                 raise
         else:
             raise BoltProtocolError("Unexpected response message with signature "
                                     "%02X" % ord(summary_signature), self.unresolved_address)
 
         return len(details), 1
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/io/_bolt5.py` & `neo4j-5.8.0/src/neo4j/_async/io/_bolt5.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import typing as t
+from enum import Enum
 from logging import getLogger
 from ssl import SSLSocket
 
 from ..._codec.hydration import v2 as hydration_v2
 from ..._exceptions import BoltProtocolError
 from ...api import (
     READ_ACCESS,
@@ -28,60 +30,74 @@
 from ...exceptions import (
     DatabaseUnavailable,
     ForbiddenOnReadOnlyDatabase,
     Neo4jError,
     NotALeader,
     ServiceUnavailable,
 )
-from ._bolt import Bolt
+from ._bolt import (
+    AsyncBolt,
+    ServerStateManagerBase,
+)
 from ._bolt3 import (
     ServerStateManager,
     ServerStates,
 )
 from ._common import (
     check_supported_server_product,
     CommitResponse,
     InitResponse,
+    LogonResponse,
     Response,
 )
 
 
 log = getLogger("neo4j")
 
 
-class Bolt5x0(Bolt):
-    """Protocol handler for Bolt 5.0. """
+class AsyncBolt5x0(AsyncBolt):
+    """Protocol handler for Bolt 5.0."""
 
     PROTOCOL_VERSION = Version(5, 0)
 
     HYDRATION_HANDLER_CLS = hydration_v2.HydrationHandler
 
     supports_multiple_results = True
 
     supports_multiple_databases = True
 
+    supports_re_auth = False
+
+    supports_notification_filtering = False
+
+    server_states: t.Any = ServerStates
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._server_state_manager = ServerStateManager(
-            ServerStates.CONNECTED, on_change=self._on_server_state_change
+            self.server_states.CONNECTED,
+            on_change=self._on_server_state_change
         )
 
     def _on_server_state_change(self, old_state, new_state):
         log.debug("[#%04X]  _: <CONNECTION> state: %s > %s", self.local_port,
                   old_state.name, new_state.name)
 
+    def _get_server_state_manager(self) -> ServerStateManagerBase:
+        return self._server_state_manager
+
     @property
     def is_reset(self):
         # We can't be sure of the server's state if there are still pending
         # responses. Unless the last message we sent was RESET. In that case
         # the server state will always be READY when we're done.
         if (self.responses and self.responses[-1]
                 and self.responses[-1].message == "reset"):
             return True
-        return self._server_state_manager.state == ServerStates.READY
+        return self._server_state_manager.state == self.server_states.READY
 
     @property
     def encrypted(self):
         return isinstance(self.socket, SSLSocket)
 
     @property
     def der_encoded_server_certificate(self):
@@ -89,15 +105,15 @@
 
     def get_base_headers(self):
         headers = {"user_agent": self.user_agent}
         if self.routing_context is not None:
             headers["routing"] = self.routing_context
         return headers
 
-    def hello(self, dehydration_hooks=None, hydration_hooks=None):
+    async def hello(self, dehydration_hooks=None, hydration_hooks=None):
         if (
             self.notifications_min_severity is not None
             or self.notifications_disabled_categories is not None
         ):
             self.assert_notification_filtering_support()
 
         def on_success(metadata):
@@ -122,19 +138,27 @@
         if "credentials" in logged_headers:
             logged_headers["credentials"] = "*******"
         log.debug("[#%04X]  C: HELLO %r", self.local_port, logged_headers)
         self._append(b"\x01", (headers,),
                      response=InitResponse(self, "hello", hydration_hooks,
                                            on_success=on_success),
                      dehydration_hooks=dehydration_hooks)
-        self.send_all()
-        self.fetch_all()
+        await self.send_all()
+        await self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
-    def route(self, database=None, imp_user=None, bookmarks=None,
+    def logon(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGON message to the outgoing queue."""
+        self.assert_re_auth_support()
+
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        """Append a LOGOFF message to the outgoing queue."""
+        self.assert_re_auth_support()
+
+    async def route(self, database=None, imp_user=None, bookmarks=None,
                     dehydration_hooks=None, hydration_hooks=None):
         routing_context = self.routing_context or {}
         db_context = {}
         if database is not None:
             db_context.update(db=database)
         if imp_user is not None:
             db_context.update(imp_user=imp_user)
@@ -145,16 +169,16 @@
             bookmarks = []
         else:
             bookmarks = list(bookmarks)
         self._append(b"\x66", (routing_context, bookmarks, db_context),
                      response=Response(self, "route", hydration_hooks,
                                        on_success=metadata.update),
                      dehydration_hooks=hydration_hooks)
-        self.send_all()
-        self.fetch_all()
+        await self.send_all()
+        await self.fetch_all()
         return [metadata.get("rt")]
 
     def run(self, query, parameters=None, mode=None, bookmarks=None,
             metadata=None, timeout=None, db=None, imp_user=None,
             notifications_min_severity=None,
             notifications_disabled_categories=None, dehydration_hooks=None,
             hydration_hooks=None, **handlers):
@@ -266,15 +290,15 @@
     def rollback(self, dehydration_hooks=None, hydration_hooks=None,
                  **handlers):
         log.debug("[#%04X]  C: ROLLBACK", self.local_port)
         self._append(b"\x13", (),
                      Response(self, "rollback", hydration_hooks, **handlers),
                      dehydration_hooks=dehydration_hooks)
 
-    def reset(self, dehydration_hooks=None, hydration_hooks=None):
+    async def reset(self, dehydration_hooks=None, hydration_hooks=None):
         """Reset the connection.
 
         Add a RESET message to the outgoing queue, send it and consume all
         remaining messages.
         """
 
         def fail(metadata):
@@ -282,22 +306,22 @@
                                     self.unresolved_address)
 
         log.debug("[#%04X]  C: RESET", self.local_port)
         self._append(b"\x0F",
                      response=Response(self, "reset", hydration_hooks,
                                        on_failure=fail),
                      dehydration_hooks=dehydration_hooks)
-        self.send_all()
-        self.fetch_all()
+        await self.send_all()
+        await self.fetch_all()
 
     def goodbye(self, dehydration_hooks=None, hydration_hooks=None):
         log.debug("[#%04X]  C: GOODBYE", self.local_port)
         self._append(b"\x02", (), dehydration_hooks=dehydration_hooks)
 
-    def _process_message(self, tag, fields):
+    async def _process_message(self, tag, fields):
         """Process at most one message from the server, if available.
 
         :returns: 2-tuple of number of detail messages and number of summary
                  messages fetched
         """
         details = []
         summary_signature = summary_metadata = None
@@ -308,63 +332,116 @@
             summary_metadata = fields[0]
         else:
             summary_signature = tag
 
         if details:
             # Do not log any data
             log.debug("[#%04X]  S: RECORD * %d", self.local_port, len(details))
-            self.responses[0].on_records(details)
+            await self.responses[0].on_records(details)
 
         if summary_signature is None:
             return len(details), 0
 
         response = self.responses.popleft()
         response.complete = True
         if summary_signature == b"\x70":
             log.debug("[#%04X]  S: SUCCESS %r", self.local_port,
                       summary_metadata)
             self._server_state_manager.transition(response.message,
                                                   summary_metadata)
-            response.on_success(summary_metadata or {})
+            await response.on_success(summary_metadata or {})
         elif summary_signature == b"\x7E":
             log.debug("[#%04X]  S: IGNORED", self.local_port)
-            response.on_ignored(summary_metadata or {})
+            await response.on_ignored(summary_metadata or {})
         elif summary_signature == b"\x7F":
             log.debug("[#%04X]  S: FAILURE %r", self.local_port,
                       summary_metadata)
-            self._server_state_manager.state = ServerStates.FAILED
+            self._server_state_manager.state = self.server_states.FAILED
             try:
-                response.on_failure(summary_metadata or {})
+                await response.on_failure(summary_metadata or {})
             except (ServiceUnavailable, DatabaseUnavailable):
                 if self.pool:
-                    self.pool.deactivate(address=self.unresolved_address)
+                    await self.pool.deactivate(address=self.unresolved_address)
                 raise
             except (NotALeader, ForbiddenOnReadOnlyDatabase):
                 if self.pool:
                     self.pool.on_write_failure(address=self.unresolved_address)
                 raise
             except Neo4jError as e:
-                if self.pool and e._invalidates_all_connections():
-                    self.pool.mark_all_stale()
+                if self.pool:
+                    await self.pool.on_neo4j_error(e, self)
                 raise
         else:
             raise BoltProtocolError(
                 "Unexpected response message with signature %02X" % ord(
                     summary_signature
                 ), self.unresolved_address
             )
 
         return len(details), 1
 
 
-class Bolt5x1(Bolt5x0):
+class ServerStates5x1(Enum):
+    CONNECTED = "CONNECTED"
+    READY = "READY"
+    STREAMING = "STREAMING"
+    TX_READY_OR_TX_STREAMING = "TX_READY||TX_STREAMING"
+    FAILED = "FAILED"
+    AUTHENTICATION = "AUTHENTICATION"
+
+
+class ServerStateManager5x1(ServerStateManager):
+    _STATE_TRANSITIONS = {  # type: ignore
+        ServerStates5x1.CONNECTED: {
+            "hello": ServerStates5x1.AUTHENTICATION,
+        },
+        ServerStates5x1.AUTHENTICATION: {
+            "logon": ServerStates5x1.READY,
+        },
+        ServerStates5x1.READY: {
+            "run": ServerStates5x1.STREAMING,
+            "begin": ServerStates5x1.TX_READY_OR_TX_STREAMING,
+            "logoff": ServerStates5x1.AUTHENTICATION,
+        },
+        ServerStates5x1.STREAMING: {
+            "pull": ServerStates5x1.READY,
+            "discard": ServerStates5x1.READY,
+            "reset": ServerStates5x1.READY,
+        },
+        ServerStates5x1.TX_READY_OR_TX_STREAMING: {
+            "commit": ServerStates5x1.READY,
+            "rollback": ServerStates5x1.READY,
+            "reset": ServerStates5x1.READY,
+        },
+        ServerStates5x1.FAILED: {
+            "reset": ServerStates5x1.READY,
+        }
+    }
+
+
+    def failed(self):
+        return self.state == ServerStates5x1.FAILED
+
+
+class AsyncBolt5x1(AsyncBolt5x0):
+    """Protocol handler for Bolt 5.1."""
 
     PROTOCOL_VERSION = Version(5, 1)
 
-    def hello(self, dehydration_hooks=None, hydration_hooks=None):
+    supports_re_auth = True
+
+    server_states = ServerStates5x1
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._server_state_manager = ServerStateManager5x1(
+            ServerStates5x1.CONNECTED, on_change=self._on_server_state_change
+        )
+
+    async def hello(self, dehydration_hooks=None, hydration_hooks=None):
         if (
             self.notifications_min_severity is not None
             or self.notifications_disabled_categories is not None
         ):
             self.assert_notification_filtering_support()
 
         def on_success(metadata):
@@ -379,51 +456,60 @@
                 else:
                     log.info("[#%04X]  _: <CONNECTION> Server supplied an "
                              "invalid value for "
                              "connection.recv_timeout_seconds (%r). Make sure "
                              "the server and network is set up correctly.",
                              self.local_port, recv_timeout)
 
-        extra = self.get_base_headers()
-        log.debug("[#%04X]  C: HELLO %r", self.local_port, extra)
-        self._append(b"\x01", (extra,),
+        headers = self.get_base_headers()
+        logged_headers = dict(headers)
+        log.debug("[#%04X]  C: HELLO %r", self.local_port, logged_headers)
+        self._append(b"\x01", (headers,),
                      response=InitResponse(self, "hello", hydration_hooks,
                                            on_success=on_success),
                      dehydration_hooks=dehydration_hooks)
-
-        self.logon(dehydration_hooks, hydration_hooks)
-        self.send_all()
-        self.fetch_all()
+        self.logon(dehydration_hooks=dehydration_hooks,
+                   hydration_hooks=hydration_hooks)
+        await self.send_all()
+        await self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
     def logon(self, dehydration_hooks=None, hydration_hooks=None):
         logged_auth_dict = dict(self.auth_dict)
         if "credentials" in logged_auth_dict:
             logged_auth_dict["credentials"] = "*******"
         log.debug("[#%04X]  C: LOGON %r", self.local_port, logged_auth_dict)
         self._append(b"\x6A", (self.auth_dict,),
-                     response=Response(self, "logon", hydration_hooks),
+                     response=LogonResponse(self, "logon", hydration_hooks),
+                     dehydration_hooks=dehydration_hooks)
+
+    def logoff(self, dehydration_hooks=None, hydration_hooks=None):
+        log.debug("[#%04X]  C: LOGOFF", self.local_port)
+        self._append(b"\x6B",
+                     response=LogonResponse(self, "logoff", hydration_hooks),
                      dehydration_hooks=dehydration_hooks)
 
 
-class Bolt5x2(Bolt5x1):
+class AsyncBolt5x2(AsyncBolt5x1):
 
     PROTOCOL_VERSION = Version(5, 2)
 
+    supports_notification_filtering = True
+
     def get_base_headers(self):
         headers = super().get_base_headers()
         if self.notifications_min_severity is not None:
             headers["notifications_minimum_severity"] = \
                 self.notifications_min_severity
         if self.notifications_disabled_categories is not None:
             headers["notifications_disabled_categories"] = \
                 self.notifications_disabled_categories
         return headers
 
-    def hello(self, dehydration_hooks=None, hydration_hooks=None):
+    async def hello(self, dehydration_hooks=None, hydration_hooks=None):
         def on_success(metadata):
             self.configuration_hints.update(metadata.pop("hints", {}))
             self.server_info.update(metadata)
             if "connection.recv_timeout_seconds" in self.configuration_hints:
                 recv_timeout = self.configuration_hints[
                     "connection.recv_timeout_seconds"
                 ]
@@ -440,27 +526,18 @@
         log.debug("[#%04X]  C: HELLO %r", self.local_port, extra)
         self._append(b"\x01", (extra,),
                      response=InitResponse(self, "hello", hydration_hooks,
                                            on_success=on_success),
                      dehydration_hooks=dehydration_hooks)
 
         self.logon(dehydration_hooks, hydration_hooks)
-        self.send_all()
-        self.fetch_all()
+        await self.send_all()
+        await self.fetch_all()
         check_supported_server_product(self.server_info.agent)
 
-    def logon(self, dehydration_hooks=None, hydration_hooks=None):
-        logged_auth_dict = dict(self.auth_dict)
-        if "credentials" in logged_auth_dict:
-            logged_auth_dict["credentials"] = "*******"
-        log.debug("[#%04X]  C: LOGON %r", self.local_port, logged_auth_dict)
-        self._append(b"\x6A", (self.auth_dict,),
-                     response=Response(self, "logon", hydration_hooks),
-                     dehydration_hooks=dehydration_hooks)
-
     def run(self, query, parameters=None, mode=None, bookmarks=None,
             metadata=None, timeout=None, db=None, imp_user=None,
             notifications_min_severity=None,
             notifications_disabled_categories=None, dehydration_hooks=None,
             hydration_hooks=None, **handlers):
         if not parameters:
             parameters = {}
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/io/_common.py` & `neo4j-5.8.0/src/neo4j/_sync/io/_common.py`

 * *Files 16% similar despite different names*

```diff
@@ -252,27 +252,42 @@
         handler = self.handlers.get("on_ignored")
         Util.callback(handler, metadata)
         handler = self.handlers.get("on_summary")
         Util.callback(handler)
 
 
 class InitResponse(Response):
+    def on_failure(self, metadata):
+        # No sense in resetting the connection,
+        # the server will have closed it already.
+        self.connection.kill()
+        handler = self.handlers.get("on_failure")
+        Util.callback(handler, metadata)
+        handler = self.handlers.get("on_summary")
+        Util.callback(handler)
+        metadata["message"] = metadata.get(
+            "message",
+            "Connection initialisation failed due to an unknown error"
+        )
+        raise Neo4jError.hydrate(**metadata)
+
 
+class LogonResponse(InitResponse):
     def on_failure(self, metadata):
-        code = metadata.get("code")
-        if code == "Neo.ClientError.Security.Unauthorized":
-            raise Neo4jError.hydrate(**metadata)
-        else:
-            raise ServiceUnavailable(
-                metadata.get("message", "Connection initialisation failed")
-            )
+        # No sense in resetting the connection,
+        # the server will have closed it already.
+        self.connection.kill()
+        handler = self.handlers.get("on_failure")
+        Util.callback(handler, metadata)
+        handler = self.handlers.get("on_summary")
+        Util.callback(handler)
+        raise Neo4jError.hydrate(**metadata)
 
 
 class CommitResponse(Response):
-
     pass
 
 
 def check_supported_server_product(agent):
     """ Checks that a server product is supported by the driver by
     looking at the server agent string.
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/io/_pool.py` & `neo4j-5.8.0/src/neo4j/_sync/io/_pool.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,61 +12,78 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from __future__ import annotations
+
 import abc
 import asyncio
 import logging
+import typing as t
 from collections import (
     defaultdict,
     deque,
 )
+from copy import copy
+from dataclasses import dataclass
 from logging import getLogger
 from random import choice
 
 from ..._async_compat.concurrency import (
     Condition,
     CooperativeRLock,
     RLock,
 )
 from ..._async_compat.network import NetworkUtil
+from ..._async_compat.util import Util
 from ..._conf import (
     PoolConfig,
     WorkspaceConfig,
 )
 from ..._deadline import (
     connection_deadline,
     Deadline,
 )
 from ..._exceptions import BoltError
 from ..._routing import RoutingTable
+from ..._sync.auth_management import StaticAuthManager
 from ...api import (
     READ_ACCESS,
     WRITE_ACCESS,
 )
+from ...auth_management import AuthManager
 from ...exceptions import (
     ClientError,
     ConfigurationError,
     DriverError,
     Neo4jError,
     ReadServiceUnavailable,
     ServiceUnavailable,
     SessionExpired,
+    TokenExpired,
+    TokenExpiredRetryable,
     WriteServiceUnavailable,
 )
+from ..auth_management import StaticAuthManager
 from ._bolt import Bolt
 
 
 # Set up logger
 log = getLogger("neo4j")
 
 
+@dataclass
+class AcquireAuth:
+    auth: t.Union[AuthManager, AuthManager, None]
+    force_auth: bool = False
+
+
 class IOPool(abc.ABC):
     """ A collection of connections to one or more server addresses.
     """
 
     def __init__(self, opener, pool_config, workspace_config):
         assert callable(opener)
         assert isinstance(pool_config, PoolConfig)
@@ -82,67 +99,91 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
+    def get_auth(self):
+        return Util.callback(self.pool_config.auth.get_auth)
+
     def _acquire_from_pool(self, address):
         with self.lock:
             for connection in list(self.connections.get(address, [])):
                 if connection.in_use:
                     continue
                 connection.pool = self
                 connection.in_use = True
                 return connection
         return None  # no free connection available
 
+    def _remove_connection(self, connection):
+        address = connection.unresolved_address
+        with self.lock:
+            log.debug(
+                "[#%04X]  _: <POOL> remove connection from pool %r %s",
+                connection.local_port, address, connection.connection_id
+            )
+            try:
+                self.connections.get(address, []).remove(connection)
+            except ValueError:
+                # If closure fails (e.g. because the server went
+                # down), all connections to the same address will
+                # be removed. Therefore, we silently ignore if the
+                # connection isn't in the pool anymore.
+                pass
+
     def _acquire_from_pool_checked(
         self, address, health_check, deadline
     ):
         while not deadline.expired():
             connection = self._acquire_from_pool(address)
             if not connection:
                 return None  # no free connection available
             if not health_check(connection, deadline):
                 # `close` is a noop on already closed connections.
                 # This is to make sure that the connection is
                 # gracefully closed, e.g. if it's just marked as
                 # `stale` but still alive.
                 if log.isEnabledFor(logging.DEBUG):
                     log.debug(
-                        "[#%04X]  _: <POOL> removing old connection %s "
+                        "[#%04X]  _: <POOL> found unhealthy connection %s "
                         "(closed=%s, defunct=%s, stale=%s, in_use=%s)",
                         connection.local_port, connection.connection_id,
                         connection.closed(), connection.defunct(),
                         connection.stale(), connection.in_use
                     )
                 connection.close()
-                with self.lock:
-                    try:
-                        self.connections.get(address, []).remove(connection)
-                    except ValueError:
-                        # If closure fails (e.g. because the server went
-                        # down), all connections to the same address will
-                        # be removed. Therefore, we silently ignore if the
-                        # connection isn't in the pool anymore.
-                        pass
+                self._remove_connection(connection)
                 continue  # try again with a new connection
             else:
                 return connection
 
-    def _acquire_new_later(self, address, deadline):
+    def _acquire_new_later(self, address, auth, deadline):
         def connection_creator():
             released_reservation = False
             try:
                 try:
-                    connection = self.opener(address, deadline)
+                    connection = self.opener(
+                        address, auth or self.pool_config.auth, deadline
+                    )
                 except ServiceUnavailable:
                     self.deactivate(address)
                     raise
+                if auth:
+                    # It's unfortunate that we have to create a connection
+                    # first to determine if the session-level auth is supported
+                    # by the protocol or not.
+                    try:
+                        connection.assert_re_auth_support()
+                    except ConfigurationError:
+                        log.debug("[#%04X]  _: <POOL> no re-auth support",
+                                  connection.local_port)
+                        connection.close()
+                        raise
                 connection.pool = self
                 connection.in_use = True
                 with self.lock:
                     self.connections_reservations[address] -= 1
                     released_reservation = True
                     self.connections[address].append(connection)
                 return connection
@@ -160,21 +201,55 @@
                          + self.connections_reservations[address])
             if infinite_pool_size or pool_size < max_pool_size:
                 # there's room for a new connection
                 self.connections_reservations[address] += 1
                 return connection_creator
         return None
 
-    def _acquire(self, address, deadline, liveness_check_timeout):
+    def _re_auth_connection(self, connection, auth, force):
+        if auth:
+            # Assert session auth is supported by the protocol.
+            # The Bolt implementation will try as hard as it can to make the
+            # re-auth work. So if the session auth token is identical to the
+            # driver auth token, the connection doesn't have to do anything so
+            # it won't fail regardless of the protocol version.
+            connection.assert_re_auth_support()
+        new_auth_manager = auth or self.pool_config.auth
+        log_auth = "******" if auth else "None"
+        new_auth = Util.callback(new_auth_manager.get_auth)
+        try:
+            updated = connection.re_auth(new_auth, new_auth_manager,
+                                         force=force)
+            log.debug("[#%04X]  _: <POOL> checked re_auth auth=%s updated=%s "
+                      "force=%s",
+                      connection.local_port, log_auth, updated, force)
+        except Exception as exc:
+            log.debug("[#%04X]  _: <POOL> check re_auth failed %r auth=%s "
+                      "force=%s",
+                      connection.local_port, exc, log_auth, force)
+            raise
+        assert not force or updated  # force=True implies updated=True
+        if force:
+            connection.send_all()
+            connection.fetch_all()
+
+    def _acquire(
+        self, address, auth, deadline, liveness_check_timeout
+    ):
         """ Acquire a connection to a given address from the pool.
         The address supplied should always be an IP address, not
         a host name.
 
         This method is thread safe.
         """
+        if auth is None:
+            auth = AcquireAuth(None)
+        force_auth = auth.force_auth
+        auth = auth.auth
+
         def health_check(connection_, deadline_):
             if (connection_.closed()
                     or connection_.defunct()
                     or connection_.stale()):
                 return False
             if liveness_check_timeout is not None:
                 if connection_.is_idle_for(liveness_check_timeout):
@@ -189,21 +264,41 @@
 
         while True:
             # try to find a free connection in the pool
             connection = self._acquire_from_pool_checked(
                 address, health_check, deadline
             )
             if connection:
-                log.debug("[#%04X]  _: <POOL> handing out existing connection "
-                          "%s", connection.local_port,
-                          connection.connection_id)
+                log.debug("[#%04X]  _: <POOL> picked existing connection %s",
+                          connection.local_port, connection.connection_id)
+                try:
+                    self._re_auth_connection(
+                        connection, auth, force_auth
+                    )
+                except ConfigurationError:
+                    if auth:
+                        # protocol version lacks support for re-auth
+                        # => session auth token is not supported
+                        raise
+                    # expiring tokens supported by flushing the pool
+                    # => give up this connection
+                    log.debug("[#%04X]  _: <POOL> backwards compatible "
+                              "auth token refresh: purge connection",
+                              connection.local_port)
+                    connection.close()
+                    self.release(connection)
+                    continue
+                log.debug("[#%04X]  _: <POOL> handing out existing connection",
+                          connection.local_port)
                 return connection
             # all connections in pool are in-use
             with self.lock:
-                connection_creator = self._acquire_new_later(address, deadline)
+                connection_creator = self._acquire_new_later(
+                    address, auth, deadline,
+                )
                 if connection_creator:
                     break
 
                 # failed to obtain a connection from pool because the
                 # pool is full and no free connection in the pool
                 timeout = deadline.to_timeout()
                 if (
@@ -216,23 +311,25 @@
                         "{!r}s (timeout)".format(deadline.original_timeout)
                     )
         log.debug("[#0000]  _: <POOL> trying to hand out new connection")
         return connection_creator()
 
     @abc.abstractmethod
     def acquire(
-        self, access_mode, timeout, database, bookmarks, liveness_check_timeout
+        self, access_mode, timeout, database, bookmarks, auth: AcquireAuth,
+        liveness_check_timeout
     ):
         """ Acquire a connection to a server that can satisfy a set of parameters.
 
         :param access_mode:
         :param timeout: timeout for the core acquisition
             (excluding potential preparation like fetching routing tables).
         :param database:
         :param bookmarks:
+        :param auth:
         :param liveness_check_timeout:
         """
         ...
 
     def kill_and_release(self, *connections):
         """ Release connections back into the pool after closing them.
 
@@ -259,32 +356,32 @@
         cancelled = None
         for connection in connections:
             if not (connection.defunct()
                     or connection.closed()
                     or connection.is_reset):
                 if cancelled is not None:
                     log.debug(
-                        "[#%04X]  _: <POOL> released unclean connection %s",
+                        "[#%04X]  _: <POOL> kill unclean connection %s",
                         connection.local_port, connection.connection_id
                     )
                     connection.kill()
                     continue
                 try:
                     log.debug(
-                        "[#%04X]  _: <POOL> released unclean connection %s",
+                        "[#%04X]  _: <POOL> release unclean connection %s",
                         connection.local_port, connection.connection_id
                     )
                     connection.reset()
-                except (Neo4jError, DriverError, BoltError) as e:
+                except (Neo4jError, DriverError, BoltError) as exc:
                     log.debug("[#%04X]  _: <POOL> failed to reset connection "
-                              "on release: %r", connection.local_port, e)
-                except asyncio.CancelledError as e:
+                              "on release: %r", connection.local_port, exc)
+                except asyncio.CancelledError as exc:
                     log.debug("[#%04X]  _: <POOL> cancelled reset connection "
-                              "on release: %r", connection.local_port, e)
-                    cancelled = e
+                              "on release: %r", connection.local_port, exc)
+                    cancelled = exc
                     connection.kill()
         with self.lock:
             for connection in connections:
                 connection.in_use = False
                 log.debug(
                     "[#%04X]  _: <POOL> released %s",
                     connection.local_port, connection.connection_id
@@ -347,14 +444,35 @@
         self._close_connections(closable_connections)
 
     def on_write_failure(self, address):
         raise WriteServiceUnavailable(
             "No write service available for pool {}".format(self)
         )
 
+    def on_neo4j_error(self, error, connection):
+        assert isinstance(error, Neo4jError)
+        if error._unauthenticates_all_connections():
+            address = connection.unresolved_address
+            log.debug(
+                "[#0000]  _: <POOL> mark all connections to %r as "
+                "unauthenticated", address
+            )
+            with self.lock:
+                for connection in self.connections.get(address, ()):
+                    connection.mark_unauthenticated()
+        if error._requires_new_credentials():
+            Util.callback(
+                connection.auth_manager.on_auth_expired,
+                connection.auth
+            )
+        if (isinstance(error, TokenExpired)
+            and not isinstance(self.pool_config.auth, (StaticAuthManager,
+                                                       StaticAuthManager))):
+            error.__class__ = TokenExpiredRetryable
+
     def close(self):
         """ Close all connections and empty the pool.
         This method is thread safe.
         """
         log.debug("[#0000]  _: <POOL> close")
         try:
             connections = []
@@ -366,28 +484,27 @@
         except TypeError:
             pass
 
 
 class BoltPool(IOPool):
 
     @classmethod
-    def open(cls, address, *, auth, pool_config, workspace_config):
+    def open(cls, address, *, pool_config, workspace_config):
         """Create a new BoltPool
 
         :param address:
-        :param auth:
         :param pool_config:
         :param workspace_config:
         :returns: BoltPool
         """
 
-        def opener(addr, deadline):
+        def opener(addr, auth_manager, deadline):
             return Bolt.open(
-                addr, auth=auth, deadline=deadline, routing_context=None,
-                pool_config=pool_config
+                addr, auth_manager=auth_manager, deadline=deadline,
+                routing_context=None, pool_config=pool_config
             )
 
         pool = cls(opener, pool_config, workspace_config, address)
         log.debug("[#0000]  _: <POOL> created, direct address %r", address)
         return pool
 
     def __init__(self, opener, pool_config, workspace_config, address):
@@ -395,53 +512,53 @@
         self.address = address
 
     def __repr__(self):
         return "<{} address={!r}>".format(self.__class__.__name__,
                                           self.address)
 
     def acquire(
-        self, access_mode, timeout, database, bookmarks, liveness_check_timeout
+        self, access_mode, timeout, database, bookmarks, auth: AcquireAuth,
+        liveness_check_timeout
     ):
         # The access_mode and database is not needed for a direct connection,
         # it's just there for consistency.
         log.debug("[#0000]  _: <POOL> acquire direct connection, "
                   "access_mode=%r, database=%r", access_mode, database)
         deadline = Deadline.from_timeout_or_deadline(timeout)
         return self._acquire(
-            self.address, deadline, liveness_check_timeout
+            self.address, auth, deadline, liveness_check_timeout
         )
 
 
 class Neo4jPool(IOPool):
     """ Connection pool with routing table.
     """
 
     @classmethod
-    def open(cls, *addresses, auth, pool_config, workspace_config,
+    def open(cls, *addresses, pool_config, workspace_config,
              routing_context=None):
         """Create a new Neo4jPool
 
         :param addresses: one or more address as positional argument
-        :param auth:
         :param pool_config:
         :param workspace_config:
         :param routing_context:
         :returns: Neo4jPool
         """
 
         address = addresses[0]
         if routing_context is None:
             routing_context = {}
         elif "address" in routing_context:
             raise ConfigurationError("The key 'address' is reserved for routing context.")
         routing_context["address"] = str(address)
 
-        def opener(addr, deadline):
+        def opener(addr, auth_manager, deadline):
             return Bolt.open(
-                addr, auth=auth, deadline=deadline,
+                addr, auth_manager=auth_manager, deadline=deadline,
                 routing_context=routing_context, pool_config=pool_config
             )
 
         pool = cls(opener, pool_config, workspace_config, address)
         log.debug("[#0000]  _: <POOL> created, routing address %r", address)
         return pool
 
@@ -474,67 +591,74 @@
                 self.routing_tables[database] = RoutingTable(
                     database=database,
                     routers=[self.address]
                 )
             return self.routing_tables[database]
 
     def fetch_routing_info(
-        self, address, database, imp_user, bookmarks, acquisition_timeout
+        self, address, database, imp_user, bookmarks, auth, acquisition_timeout
     ):
         """ Fetch raw routing info from a given router address.
 
         :param address: router address
         :param database: the database name to get routing table for
         :param imp_user: the user to impersonate while fetching the routing
                          table
         :type imp_user: str or None
         :param bookmarks: iterable of bookmark values after which the routing
                           info should be fetched
+        :param auth: auth
         :param acquisition_timeout: connection acquisition timeout
 
         :returns: list of routing records, or None if no connection
             could be established or if no readers or writers are present
         :raise ServiceUnavailable: if the server does not support
             routing, or if routing support is broken or outdated
         """
         deadline = Deadline.from_timeout_or_deadline(acquisition_timeout)
         log.debug("[#0000]  _: <POOL> _acquire router connection, "
                   "database=%r, address=%r", database, address)
-        cx = self._acquire(address, deadline, None)
+        if auth:
+            auth = copy(auth)
+            auth.force_auth = False
+        cx = self._acquire(address, auth, deadline, None)
         try:
             routing_table = cx.route(
                 database=database or self.workspace_config.database,
                 imp_user=imp_user or self.workspace_config.impersonated_user,
                 bookmarks=bookmarks
             )
         finally:
             self.release(cx)
         return routing_table
 
     def fetch_routing_table(
-        self, *, address, acquisition_timeout, database, imp_user, bookmarks
+        self, *, address, acquisition_timeout, database, imp_user,
+        bookmarks, auth
     ):
         """ Fetch a routing table from a given router address.
 
         :param address: router address
         :param acquisition_timeout: connection acquisition timeout
         :param database: the database name
         :type: str
         :param imp_user: the user to impersonate while fetching the routing
                          table
         :type imp_user: str or None
         :param bookmarks: bookmarks used when fetching routing table
+        :param auth: auth
 
         :returns: a new RoutingTable instance or None if the given router is
                  currently unable to provide routing information
         """
         new_routing_info = None
         try:
             new_routing_info = self.fetch_routing_info(
-                address, database, imp_user, bookmarks, acquisition_timeout
+                address, database, imp_user, bookmarks, auth,
+                acquisition_timeout
             )
         except Neo4jError as e:
             # checks if the code is an error that is caused by the client. In
             # this case there is no sense in trying to fetch a RT from another
             # router. Hence, the driver should fail fast during discovery.
             if e._is_fatal_during_discovery():
                 raise
@@ -572,16 +696,16 @@
                       "server %s", address)
             return None
 
         # At least one of each is fine, so return this table
         return new_routing_table
 
     def _update_routing_table_from(
-        self, *routers, database, imp_user, bookmarks, acquisition_timeout,
-        database_callback
+        self, *routers, database, imp_user, bookmarks, auth,
+        acquisition_timeout, database_callback
     ):
         """ Try to update routing tables with the given routers.
 
         :returns: True if the routing table is successfully updated,
         otherwise False
         """
         if routers:
@@ -589,15 +713,16 @@
                       "table from {}".format(", ".join(map(repr, routers))))
         for router in routers:
             for address in NetworkUtil.resolve_address(
                 router, resolver=self.pool_config.resolver
             ):
                 new_routing_table = self.fetch_routing_table(
                     address=address, acquisition_timeout=acquisition_timeout,
-                    database=database, imp_user=imp_user, bookmarks=bookmarks
+                    database=database, imp_user=imp_user, bookmarks=bookmarks,
+                    auth=auth
                 )
                 if new_routing_table is not None:
                     new_database = new_routing_table.database
                     old_routing_table = self.get_or_create_routing_table(
                         new_database
                     )
                     old_routing_table.update(new_routing_table)
@@ -609,25 +734,26 @@
                     if callable(database_callback):
                         database_callback(new_database)
                     return True
             self.deactivate(router)
         return False
 
     def update_routing_table(
-        self, *, database, imp_user, bookmarks, acquisition_timeout=None,
-        database_callback=None
+        self, *, database, imp_user, bookmarks, auth=None,
+        acquisition_timeout=None, database_callback=None
     ):
         """ Update the routing table from the first router able to provide
         valid routing information.
 
         :param database: The database name
         :param imp_user: the user to impersonate while fetching the routing
                          table
         :type imp_user: str or None
         :param bookmarks: bookmarks used when fetching routing table
+        :param auth: auth
         :param acquisition_timeout: connection acquisition timeout
         :param database_callback: A callback function that will be called with
             the database name as only argument when a new routing table has been
             acquired. This database name might different from `database` if that
             was None and the underlying protocol supports reporting back the
             actual database.
 
@@ -641,32 +767,32 @@
             prefer_initial_routing_address = \
                 self.routing_tables[database].initialized_without_writers
 
             if prefer_initial_routing_address:
                 # TODO: Test this state
                 if self._update_routing_table_from(
                     self.address, database=database,
-                    imp_user=imp_user, bookmarks=bookmarks,
+                    imp_user=imp_user, bookmarks=bookmarks, auth=auth,
                     acquisition_timeout=acquisition_timeout,
                     database_callback=database_callback
                 ):
                     # Why is only the first initial routing address used?
                     return
             if self._update_routing_table_from(
-                *(existing_routers - {self.address}),
-                database=database, imp_user=imp_user, bookmarks=bookmarks,
+                *(existing_routers - {self.address}), database=database,
+                imp_user=imp_user, bookmarks=bookmarks, auth=auth,
                 acquisition_timeout=acquisition_timeout,
                 database_callback=database_callback
             ):
                 return
 
             if not prefer_initial_routing_address:
                 if self._update_routing_table_from(
                     self.address, database=database,
-                    imp_user=imp_user, bookmarks=bookmarks,
+                    imp_user=imp_user, bookmarks=bookmarks, auth=auth,
                     acquisition_timeout=acquisition_timeout,
                     database_callback=database_callback
                 ):
                     # Why is only the first initial routing address used?
                     return
 
             # None of the routers have been successful, so just fail
@@ -677,15 +803,15 @@
         routing_table = self.get_or_create_routing_table(database)
         servers = routing_table.servers()
         for address in list(self.connections):
             if address._unresolved not in servers:
                 super(Neo4jPool, self).deactivate(address)
 
     def ensure_routing_table_is_fresh(
-        self, *, access_mode, database, imp_user, bookmarks,
+        self, *, access_mode, database, imp_user, bookmarks, auth=None,
         acquisition_timeout=None, database_callback=None
     ):
         """ Update the routing table if stale.
 
         This method performs two freshness checks, before and after acquiring
         the refresh lock. If the routing table is already fresh on entry, the
         method exits immediately; otherwise, the refresh lock is acquired and
@@ -714,15 +840,15 @@
                 # table is still valid
                 log.debug("[#0000]  _: <POOL> using existing routing table %r",
                           routing_table)
                 return False
 
             self.update_routing_table(
                 database=database, imp_user=imp_user, bookmarks=bookmarks,
-                acquisition_timeout=acquisition_timeout,
+                auth=auth, acquisition_timeout=acquisition_timeout,
                 database_callback=database_callback
             )
             self.update_connection_pool(database=database)
 
             return True
 
     def _select_address(self, *, access_mode, database):
@@ -751,15 +877,16 @@
             else:
                 raise WriteServiceUnavailable(
                     "No write service currently available"
                 )
         return choice(addresses_by_usage[min(addresses_by_usage)])
 
     def acquire(
-        self, access_mode, timeout, database, bookmarks, liveness_check_timeout
+        self, access_mode, timeout, database, bookmarks,
+        auth: t.Optional[AcquireAuth], liveness_check_timeout
     ):
         if access_mode not in (WRITE_ACCESS, READ_ACCESS):
             raise ClientError("Non valid 'access_mode'; {}".format(access_mode))
         if not timeout:
             raise ClientError("'timeout' must be a float larger than 0; {}"
                               .format(timeout))
 
@@ -771,15 +898,15 @@
         #         bookmarks=bookmarks, acquisition_timeout=timeout
         #     )
 
         log.debug("[#0000]  _: <POOL> acquire routing connection, "
                   "access_mode=%r, database=%r", access_mode, database)
         self.ensure_routing_table_is_fresh(
             access_mode=access_mode, database=database,
-            imp_user=None, bookmarks=bookmarks,
+            imp_user=None, bookmarks=bookmarks, auth=auth,
             acquisition_timeout=timeout
         )
 
         while True:
             try:
                 # Get an address for a connection that have the fewest in-use
                 # connections.
@@ -790,15 +917,15 @@
                 raise SessionExpired("Failed to obtain connection towards '%s' server." % access_mode) from err
             try:
                 log.debug("[#0000]  _: <POOL> acquire address, database=%r "
                           "address=%r", database, address)
                 deadline = Deadline.from_timeout_or_deadline(timeout)
                 # should always be a resolved address
                 connection = self._acquire(
-                    address, deadline, liveness_check_timeout
+                    address, auth, deadline, liveness_check_timeout,
                 )
             except (ServiceUnavailable, SessionExpired):
                 self.deactivate(address=address)
             else:
                 return connection
 
     def deactivate(self, address):
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/work/__init__.py` & `neo4j-5.8.0/src/neo4j/_sync/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_sync/work/result.py` & `neo4j-5.8.0/src/neo4j/_sync/work/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,31 +15,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from __future__ import annotations
 
 import typing as t
-from collections import (
-    deque,
-    namedtuple,
-)
+from collections import deque
 from warnings import warn
 
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
 from ..._async_compat.util import Util
 from ..._codec.hydration import BrokenHydrationObject
 from ..._data import (
     Record,
     RecordTableRowExporter,
 )
-from ..._meta import experimental
 from ..._work import (
     EagerResult,
     ResultSummary,
 )
 from ...exceptions import (
     ResultConsumedError,
     ResultNotSingleError,
@@ -278,15 +274,15 @@
                 self._connection.fetch_message()
 
     def _buffer(self, n=None):
         """Try to fill `self._record_buffer` with n records.
 
         Might end up with more records in the buffer if the fetch size makes it
         overshoot.
-        Might ent up with fewer records in the buffer if there are not enough
+        Might end up with fewer records in the buffer if there are not enough
         records available.
         """
         if self._out_of_scope:
             raise ResultConsumedError(self, _RESULT_OUT_OF_SCOPE_ERROR)
         if self._consumed:
             raise ResultConsumedError(self, _RESULT_CONSUMED_ERROR)
         if n is not None and len(self._record_buffer) >= n:
@@ -604,34 +600,29 @@
         .. versionchanged:: 5.0
             Can raise :exc:`ResultConsumedError`.
 
         .. seealso:: :meth:`.Record.data`
         """
         return [record.data(*keys) for record in self]
 
-    @experimental(
-        "Result.to_eager_result is experimental. "
-        "It might be changed or removed any time even without prior notice."
-    )
     def to_eager_result(self) -> EagerResult:
         """Convert this result to an :class:`.EagerResult`.
 
         This method exhausts the result and triggers a :meth:`.consume`.
 
         :returns: all remaining records in the result stream, the result's
             summary, and keys as an :class:`.EagerResult` instance.
 
         :raises ResultConsumedError: if the transaction from which this result
             was obtained has been closed or the Result has been explicitly
             consumed.
 
-        **This is experimental.** (See :ref:`filter-warnings-ref`)
-        It might be changed or removed any time even without prior notice.
-
         .. versionadded:: 5.5
+
+        .. versionchanged:: 5.8 stabilized from experimental
         """
 
         self._buffer_all()
         return EagerResult(
             keys=list(self.keys()),
             records=Util.list(self),
             summary=self.consume()
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/work/session.py` & `neo4j-5.8.0/src/neo4j/_sync/work/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,41 @@
 # limitations under the License.
 
 
 from __future__ import annotations
 
 import asyncio
 import typing as t
+import warnings
 from logging import getLogger
 from random import random
 from time import perf_counter
 
 from ..._async_compat import sleep
 from ..._async_compat.util import Util
 from ..._conf import SessionConfig
-from ..._meta import deprecated
+from ..._meta import (
+    deprecated,
+    PreviewWarning,
+)
 from ..._work import Query
 from ...api import (
     Bookmarks,
     READ_ACCESS,
     WRITE_ACCESS,
 )
 from ...exceptions import (
     ClientError,
     DriverError,
     Neo4jError,
     ServiceUnavailable,
     SessionExpired,
     TransactionError,
 )
+from ..auth_management import AuthManagers
 from .result import Result
 from .transaction import (
     ManagedTransaction,
     Transaction,
 )
 from .workspace import Workspace
 
@@ -93,15 +98,25 @@
     _auto_result = None
 
     # The state this session is in.
     _state_failed = False
 
     def __init__(self, pool, session_config):
         assert isinstance(session_config, SessionConfig)
+        if session_config.auth is not None:
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    "ignore", message=r".*\bAuth managers\b.*",
+                    category=PreviewWarning
+                )
+                session_config.auth = AuthManagers.static(
+                    session_config.auth
+                )
         super().__init__(pool, session_config)
+        self._config = session_config
         self._initialize_bookmarks(session_config.bookmarks)
         self._bookmark_manager = session_config.bookmark_manager
 
     def __enter__(self) -> Session:
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
@@ -109,19 +124,21 @@
             if issubclass(exception_type, asyncio.CancelledError):
                 self._handle_cancellation(message="__exit__")
                 self._closed = True
                 return
             self._state_failed = True
         self.close()
 
-    def _connect(self, access_mode, **access_kwargs):
+    def _connect(self, access_mode, **acquire_kwargs):
         if access_mode is None:
             access_mode = self._config.default_access_mode
         try:
-            super()._connect(access_mode, **access_kwargs)
+            super()._connect(
+                access_mode, auth=self._config.auth, **acquire_kwargs
+            )
         except asyncio.CancelledError:
             self._handle_cancellation(message="_connect")
             raise
 
     def _disconnect(self, sync=False):
         try:
             return super()._disconnect(sync=sync)
@@ -158,14 +175,19 @@
     def _get_server_info(self):
         assert not self._connection
         self._connect(READ_ACCESS, liveness_check_timeout=0)
         server_info = self._connection.server_info
         self._disconnect()
         return server_info
 
+    def _verify_authentication(self):
+        assert not self._connection
+        self._connect(READ_ACCESS, force_auth=True)
+        self._disconnect()
+
     def close(self) -> None:
         """Close the session.
 
         This will release any borrowed resources, such as connections, and will
         roll back any outstanding transactions.
         """
         if self._closed:
```

### Comparing `neo4j-5.7.0/src/neo4j/_sync/work/transaction.py` & `neo4j-5.8.0/src/neo4j/_sync/work/transaction.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_sync/work/workspace.py` & `neo4j-5.8.0/src/neo4j/_sync/work/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 )
 from ...api import Bookmarks
 from ...exceptions import (
     ServiceUnavailable,
     SessionError,
     SessionExpired,
 )
-from ..io import Neo4jPool
+from ..io import (
+    AcquireAuth,
+    Neo4jPool,
+)
 
 
 log = logging.getLogger("neo4j")
 
 
 class Workspace:
 
@@ -126,16 +129,21 @@
         )
 
     def _update_bookmark(self, bookmark):
         if not bookmark:
             return
         self._update_bookmarks((bookmark,))
 
-    def _connect(self, access_mode, **acquire_kwargs):
+    def _connect(self, access_mode, auth=None, **acquire_kwargs):
         acquisition_timeout = self._config.connection_acquisition_timeout
+        auth = AcquireAuth(
+            auth,
+            force_auth=acquire_kwargs.pop("force_auth", False),
+        )
+
         if self._connection:
             # TODO: Investigate this
             # log.warning("FIXME: should always disconnect before connect")
             self._connection.send_all()
             self._connection.fetch_all()
             self._disconnect()
         if not self._cached_database:
@@ -150,22 +158,24 @@
                 # we shall use this database explicitly for all subsequent
                 # actions within this session.
                 log.debug("[#0000]  _: <WORKSPACE> resolve home database")
                 self._pool.update_routing_table(
                     database=self._config.database,
                     imp_user=self._config.impersonated_user,
                     bookmarks=self._get_bookmarks(),
+                    auth=auth,
                     acquisition_timeout=acquisition_timeout,
                     database_callback=self._set_cached_database
                 )
         acquire_kwargs_ = {
             "access_mode": access_mode,
             "timeout": acquisition_timeout,
             "database": self._config.database,
             "bookmarks": self._get_bookmarks(),
+            "auth": auth,
             "liveness_check_timeout": None,
         }
         acquire_kwargs_.update(acquire_kwargs)
         self._connection = self._pool.acquire(**acquire_kwargs_)
         self._connection_access_mode = access_mode
 
     def _disconnect(self, sync=False):
```

### Comparing `neo4j-5.7.0/src/neo4j/_work/__init__.py` & `neo4j-5.8.0/src/neo4j/_work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_work/eager_result.py` & `neo4j-5.8.0/src/neo4j/_work/eager_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,25 +29,24 @@
      * records - the list of records returned by the query
        (list of :class:`.Record` objects)
      * summary - the summary of the query execution
        (:class:`.ResultSummary` object)
      * keys - the list of keys returned by the query
        (see :attr:`AsyncResult.keys` and :attr:`.Result.keys`)
 
-    **This is experimental.** (See :ref:`filter-warnings-ref`)
-    It might be changed or removed any time even without prior notice.
-
     .. seealso::
         :attr:`.AsyncDriver.execute_query`, :attr:`.Driver.execute_query`
             Which by default return an instance of this class.
 
         :attr:`.AsyncResult.to_eager_result`, :attr:`.Result.to_eager_result`
             Which can be used to convert to instance of this class.
 
     .. versionadded:: 5.5
+
+    .. versionchanged:: 5.8 stabilized from experimental
     """
     #: Alias for field 0 (``eager_result[0]``)
     records: t.List[Record]
     #: Alias for field 1 (``eager_result[1]``)
     summary: ResultSummary
     #: Alias for field 2 (``eager_result[2]``)
     keys: t.List[str]
```

### Comparing `neo4j-5.7.0/src/neo4j/_work/query.py` & `neo4j-5.8.0/src/neo4j/_work/query.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/_work/summary.py` & `neo4j-5.8.0/src/neo4j/_work/summary.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/addressing.py` & `neo4j-5.8.0/src/neo4j/addressing.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/api.py` & `neo4j-5.8.0/src/neo4j/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 """ Base classes and helpers.
 """
 
+
 from __future__ import annotations
 
 import abc
 import typing as t
 from urllib.parse import (
     parse_qs,
     urlparse,
@@ -99,18 +101,29 @@
         if credentials:
             self.credentials = credentials
         if realm:
             self.realm = realm
         if parameters:
             self.parameters = parameters
 
+    def __eq__(self, other):
+        if not isinstance(other, Auth):
+            return NotImplemented
+        return vars(self) == vars(other)
+
 
 # For backwards compatibility
 AuthToken = Auth
 
+# if t.TYPE_CHECKING:
+# commented out as work around for
+# https://github.com/sphinx-doc/sphinx/pull/10880
+# make sure TAuth is resolved in the docs, else they're pretty useless
+_TAuth = t.Union[t.Tuple[t.Any, t.Any], Auth, None]
+
 
 def basic_auth(
     user: str, password: str, realm: t.Optional[str] = None
 ) -> Auth:
     """Generate a basic auth token for a given user and password.
 
     This will set the scheme to "basic" for the auth token.
@@ -393,28 +406,27 @@
     interface. Create a child class to implement a specific bookmark manager
     or make use of the default implementation provided by the driver through
     :meth:`.GraphDatabase.bookmark_manager()`.
 
     .. note::
         All methods must be concurrency safe.
 
-    **This is experimental.**
-    It might be changed or removed any time even without prior notice.
-
     .. versionadded:: 5.0
 
     .. versionchanged:: 5.3
         The bookmark manager no longer tracks bookmarks per database.
         This effectively changes the signature of almost all bookmark
         manager related methods:
 
         * :meth:`.update_bookmarks` has no longer a ``database`` argument.
         * :meth:`.get_bookmarks` has no longer a ``database`` argument.
         * The ``get_all_bookmarks`` method was removed.
         * The ``forget`` method was removed.
+
+    .. versionchanged:: 5.8 stabilized from experimental
     """
 
     @abc.abstractmethod
     def update_bookmarks(
         self, previous_bookmarks: t.Collection[str],
         new_bookmarks: t.Collection[str]
     ) -> None:
@@ -438,21 +450,20 @@
 
 class AsyncBookmarkManager(_Protocol, metaclass=abc.ABCMeta):
     """Same as :class:`.BookmarkManager` but with async methods.
 
     The driver comes with a default implementation of the async bookmark
     manager accessible through :attr:`.AsyncGraphDatabase.bookmark_manager()`.
 
-    **This is experimental.**
-    It might be changed or removed any time even without prior notice.
-
     .. versionadded:: 5.0
 
     .. versionchanged:: 5.3
         See :class:`.BookmarkManager` for changes.
+
+    .. versionchanged:: 5.8 stabilized from experimental
     """
 
     @abc.abstractmethod
     async def update_bookmarks(
         self, previous_bookmarks: t.Collection[str],
         new_bookmarks: t.Collection[str]
     ) -> None:
```

### Comparing `neo4j-5.7.0/src/neo4j/conf.py` & `neo4j-5.8.0/src/neo4j/conf.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/data.py` & `neo4j-5.8.0/src/neo4j/data.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/debug.py` & `neo4j-5.8.0/src/neo4j/debug.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/exceptions.py` & `neo4j-5.8.0/src/neo4j/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,23 +228,26 @@
         :returns: :const:`True` if the error is retryable,
             :const:`False` otherwise.
 
         .. versionadded:: 5.0
         """
         return False
 
-    def _invalidates_all_connections(self) -> bool:
+    def _unauthenticates_all_connections(self) -> bool:
         return self.code == "Neo.ClientError.Security.AuthorizationExpired"
 
+    def _requires_new_credentials(self) -> bool:
+        return self.code == "Neo.ClientError.Security.TokenExpired"
+
     # TODO: 6.0 - Remove this alias
     invalidates_all_connections = deprecated(
         "Neo4jError.invalidates_all_connections is deprecated and will be "
         "removed in a future version. It is an internal method and not meant "
         "for external use."
-    )(_invalidates_all_connections)
+    )(_unauthenticates_all_connections)
 
     def _is_fatal_during_discovery(self) -> bool:
         # checks if the code is an error that is caused by the client. In this
         # case the driver should fail fast during discovery.
         if not isinstance(self.code, str):
             return False
         if self.code in ("Neo.ClientError.Database.DatabaseNotFound",
@@ -305,17 +308,33 @@
     """
 
 
 # Neo4jError > ClientError > AuthError > TokenExpired
 class TokenExpired(AuthError):
     """ Raised when the authentication token has expired.
 
-    A new driver instance with a fresh authentication token needs to be created.
+    A new driver instance with a fresh authentication token needs to be
+    created, unless the driver was configured using a non-static
+    :class:`.AuthManager`. In that case, the error will be
+    :exc:`.TokenExpiredRetryable` instead.
+    """
+
+
+# Neo4jError > ClientError > AuthError > TokenExpired > TokenExpiredRetryable
+class TokenExpiredRetryable(TokenExpired):
+    """Raised when the authentication token has expired but can be refreshed.
+
+    This is the same server error as :exc:`.TokenExpired`, but raised when
+    the driver is configured to be able to refresh the token, hence making
+    the error retryable.
     """
 
+    def is_retryable(self) -> bool:
+        return True
+
 
 # Neo4jError > ClientError > Forbidden
 class Forbidden(ClientError):
     """
     """
```

### Comparing `neo4j-5.7.0/src/neo4j/graph/__init__.py` & `neo4j-5.8.0/src/neo4j/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/meta.py` & `neo4j-5.8.0/src/neo4j/meta.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/packstream.py` & `neo4j-5.8.0/src/neo4j/packstream.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/routing.py` & `neo4j-5.8.0/src/neo4j/routing.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/spatial/__init__.py` & `neo4j-5.8.0/src/neo4j/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/time/__init__.py` & `neo4j-5.8.0/src/neo4j/time/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1388,15 +1388,15 @@
     :param second: the second of the time. Must be in range 0 <= second < 60.
     :param nanosecond: the nanosecond of the time.
         Must be in range 0 <= nanosecond < 999999999.
     :param tzinfo: timezone or None to get a local :class:`.Time`.
 
     :raises ValueError: if one of the parameters is out of range.
 
-    ..versionchanged:: 5.0
+    .. versionchanged:: 5.0
         The parameter ``second`` no longer accepts :class:`float` values.
     """
 
     # CONSTRUCTOR #
 
     def __new__(
         cls,
@@ -1508,15 +1508,15 @@
 
         :param ticks: nanoseconds since midnight
         :param tz: optional timezone
 
         :raises ValueError: if ticks is out of bounds
             (0 <= ticks < 86400000000000)
 
-        ..versionchanged:: 5.0
+        .. versionchanged:: 5.0
             The parameter ``ticks`` no longer accepts :class:`float` values
             but only :class:`int`. It's now nanoseconds since midnight instead
             of seconds.
         """
         if not isinstance(ticks, int):
             raise TypeError("Ticks must be int")
         if 0 <= ticks < 86400000000000:
@@ -2541,15 +2541,15 @@
             return self.combine(date_, time_)
 
     def as_timezone(self, tz: _tzinfo) -> DateTime:
         """Convert this :class:`.DateTime` to another timezone.
 
         :param tz: the new timezone
 
-        :returns: the same object if ``tz`` is :const:``None``.
+        :returns: the same object if ``tz`` is :data:``None``.
             Else, a new :class:`.DateTime` that's the same point in time but in
             a different timezone.
         """
         if self.tzinfo is None:
             return self
         offset = t.cast(timedelta, self.utcoffset())
         utc = (self - offset).replace(tzinfo=tz)
```

### Comparing `neo4j-5.7.0/src/neo4j/time/__main__.py` & `neo4j-5.8.0/src/neo4j/time/__main__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/time/_arithmetic.py` & `neo4j-5.8.0/src/neo4j/time/_arithmetic.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/time/_clock_implementations.py` & `neo4j-5.8.0/src/neo4j/time/_clock_implementations.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/time/_metaclasses.py` & `neo4j-5.8.0/src/neo4j/time/_metaclasses.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/time/arithmetic.py` & `neo4j-5.8.0/src/neo4j/time/arithmetic.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/time/clock_implementations.py` & `neo4j-5.8.0/src/neo4j/time/metaclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# TODO: 6.0 - remove this file
-
 
 from .._meta import deprecation_warn
-from ._clock_implementations import (
-    LibCClock,
-    PEP564Clock,
-    SafeClock,
+from ._metaclasses import (
+    DateTimeType,
+    DateType,
+    TimeType,
 )
 
 
 __all__ = [
-    "SafeClock",
-    "PEP564Clock",
-    "LibCClock",
+    "DateType",
+    "TimeType",
+    "DateTimeType",
 ]
 
 deprecation_warn(
-    "The module `neo4j.time.clock_implementations` was made internal and will "
+    "The module `neo4j.time.metaclasses` was made internal and will "
     "no longer be available for import in future versions.",
     stack_level=2
 )
```

### Comparing `neo4j-5.7.0/src/neo4j/time/hydration.py` & `neo4j-5.8.0/src/neo4j/time/hydration.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/time/metaclasses.py` & `neo4j-5.8.0/src/neo4j/auth_management.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,26 +12,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from .._meta import deprecation_warn
-from ._metaclasses import (
-    DateTimeType,
-    DateType,
-    TimeType,
+from ._async.auth_management import AsyncAuthManagers
+from ._auth_management import (
+    AsyncAuthManager,
+    AuthManager,
+    ExpiringAuth,
 )
+from ._sync.auth_management import AuthManagers
 
 
 __all__ = [
-    "DateType",
-    "TimeType",
-    "DateTimeType",
+    "AsyncAuthManager",
+    "AsyncAuthManagers",
+    "AuthManager",
+    "AuthManagers",
+    "ExpiringAuth",
 ]
-
-deprecation_warn(
-    "The module `neo4j.time.metaclasses` was made internal and will "
-    "no longer be available for import in future versions.",
-    stack_level=2
-)
```

### Comparing `neo4j-5.7.0/src/neo4j/work/__init__.py` & `neo4j-5.8.0/src/neo4j/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/work/query.py` & `neo4j-5.8.0/src/neo4j/work/query.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j/work/summary.py` & `neo4j-5.8.0/src/neo4j/work/summary.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.7.0/src/neo4j.egg-info/PKG-INFO` & `neo4j-5.8.0/src/neo4j.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j
-Version: 5.7.0
+Version: 5.8.0
 Summary: Neo4j Bolt driver for Python
 Author-email: "Neo4j, Inc." <drivers@neo4j.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/neo4j/neo4j-python-driver
 Keywords: neo4j,graph,database
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neo4j-5.7.0/src/neo4j.egg-info/SOURCES.txt` & `neo4j-5.8.0/src/neo4j.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,36 +4,39 @@
 MANIFEST.in
 NOTICE.txt
 README.rst
 pyproject.toml
 setup.py
 src/neo4j/__init__.py
 src/neo4j/_api.py
+src/neo4j/_auth_management.py
 src/neo4j/_conf.py
 src/neo4j/_data.py
 src/neo4j/_deadline.py
 src/neo4j/_exceptions.py
 src/neo4j/_meta.py
 src/neo4j/_routing.py
 src/neo4j/addressing.py
 src/neo4j/api.py
+src/neo4j/auth_management.py
 src/neo4j/conf.py
 src/neo4j/data.py
 src/neo4j/debug.py
 src/neo4j/exceptions.py
 src/neo4j/meta.py
 src/neo4j/packstream.py
 src/neo4j/py.typed
 src/neo4j/routing.py
 src/neo4j.egg-info/PKG-INFO
 src/neo4j.egg-info/SOURCES.txt
 src/neo4j.egg-info/dependency_links.txt
 src/neo4j.egg-info/requires.txt
 src/neo4j.egg-info/top_level.txt
 src/neo4j/_async/__init__.py
+src/neo4j/_async/auth_management.py
 src/neo4j/_async/bookmark_manager.py
 src/neo4j/_async/driver.py
 src/neo4j/_async/io/__init__.py
 src/neo4j/_async/io/_bolt.py
 src/neo4j/_async/io/_bolt3.py
 src/neo4j/_async/io/_bolt4.py
 src/neo4j/_async/io/_bolt5.py
@@ -64,14 +67,15 @@
 src/neo4j/_codec/hydration/v2/temporal.py
 src/neo4j/_codec/packstream/__init__.py
 src/neo4j/_codec/packstream/_common.py
 src/neo4j/_codec/packstream/v1/__init__.py
 src/neo4j/_optional_deps/__init__.py
 src/neo4j/_spatial/__init__.py
 src/neo4j/_sync/__init__.py
+src/neo4j/_sync/auth_management.py
 src/neo4j/_sync/bookmark_manager.py
 src/neo4j/_sync/driver.py
 src/neo4j/_sync/io/__init__.py
 src/neo4j/_sync/io/_bolt.py
 src/neo4j/_sync/io/_bolt3.py
 src/neo4j/_sync/io/_bolt4.py
 src/neo4j/_sync/io/_bolt5.py
```

