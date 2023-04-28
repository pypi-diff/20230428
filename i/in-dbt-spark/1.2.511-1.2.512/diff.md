# Comparing `tmp/in-dbt-spark-1.2.511.tar.gz` & `tmp/in-dbt-spark-1.2.512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.2.511.tar", last modified: Wed Apr 19 22:38:03 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.2.512.tar", last modified: Fri Apr 28 10:15:06 2023, max compression
```

## Comparing `in-dbt-spark-1.2.511.tar` & `in-dbt-spark-1.2.512.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.573747 in-dbt-spark-1.2.511/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-19 22:38:03.573747 in-dbt-spark-1.2.511/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.565746 in-dbt-spark-1.2.511/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.565746 in-dbt-spark-1.2.511/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.569747 in-dbt-spark-1.2.511/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.569747 in-dbt-spark-1.2.511/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    21731 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.565746 in-dbt-spark-1.2.511/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.569747 in-dbt-spark-1.2.511/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.569747 in-dbt-spark-1.2.511/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/apply_retention.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.569747 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.569747 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.569747 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:38:03.573747 in-dbt-spark-1.2.511/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-19 22:38:03.000000 in-dbt-spark-1.2.511/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-19 22:38:03.000000 in-dbt-spark-1.2.511/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:38:03.000000 in-dbt-spark-1.2.511/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:38:03.000000 in-dbt-spark-1.2.511/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-19 22:38:03.000000 in-dbt-spark-1.2.511/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-19 22:38:03.000000 in-dbt-spark-1.2.511/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:38:03.573747 in-dbt-spark-1.2.511/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-19 22:37:51.000000 in-dbt-spark-1.2.511/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.597803 in-dbt-spark-1.2.512/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.585803 in-dbt-spark-1.2.512/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.585803 in-dbt-spark-1.2.512/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.589803 in-dbt-spark-1.2.512/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.589803 in-dbt-spark-1.2.512/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24549 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.585803 in-dbt-spark-1.2.512/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.589803 in-dbt-spark-1.2.512/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.589803 in-dbt-spark-1.2.512/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:15:06.597803 in-dbt-spark-1.2.512/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/setup.py
```

### Comparing `in-dbt-spark-1.2.511/PKG-INFO` & `in-dbt-spark-1.2.512/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.511
+Version: 1.2.512
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.511 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.512 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.511/README.md` & `in-dbt-spark-1.2.512/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/client.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,19 @@
         if self.managed_session:
             self.session.close()
 
     def get(self, endpoint: str = "", params: dict = None) -> dict:
         return self._request("GET", endpoint, params=params, headers=self.headers, cert=self.cert)
 
     def post(self, endpoint: str, data: dict = None) -> dict:
+        # TODO: Logging in debug mode to investigate on unable to create setu session on github action
+        #       Remove after the investigation
+        logger.debug(
+            f"POST request for url - {self.url}, endpoint - {endpoint} with headers - {self.headers}"
+        )
         return self._request("POST", endpoint, data, headers=self.headers, cert=self.cert)
 
     def delete(self, endpoint: str = "") -> dict:
         return self._request("DELETE", endpoint, headers=self.headers, cert=self.cert)
 
     def _request(
         self,
```

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/models.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/models.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/session.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,17 @@
 
     def wait_till_ready(self) -> None:
         """Wait for the session to be ready."""
         intervals = polling_intervals([1, 2, 3, 5], 10)
         while self.state in SESSION_STATE_NOT_READY:
             interval = next(intervals)
             logger.info(
-                f"Waiting to get spark resources for setu session - {self.session_id} .. Sleeping for {interval} seconds.."
+                f"Waiting to get spark resources for setu session - {self.session_id}, current state - {self.state.value}"
             )
+            logger.info(f"Sleeping for {interval} seconds..")
             time.sleep(interval)
         if self.state in SESSION_INVALID_STATE:
             raise dbt.exceptions.RuntimeException(
                 f" Setu session state = {self.state} Unable to create setu session with {self.session_id}"
             )
         self.print_session_details()
```

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/session_cursor.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/session_manager.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.2.512/dbt/adapters/setu/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/spark/column.py` & `in-dbt-spark-1.2.512/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.2.512/dbt/adapters/spark/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,18 @@
     }
 
     @classmethod
     def __pre_deserialize__(cls, data):
         data = super().__pre_deserialize__(data)
         if "database" not in data:
             data["database"] = None
-        # since we write OpenHouse tables by default
+        # since we write OpenHouse tables by default,
         # if 'schema' is defined but not in the expected 'openhouse.schema' format, prefix this automatically for the user
-        # TODO: re-enable this once we have successfully changed show table extended -> describe extended to avoid blocking
-        # the hive version of this dataset for now
-        # if "schema" in data and "." not in data["schema"]:
-        #     data["schema"] = DEFAULT_CATALOG + "." + data["schema"]
+        if "schema" in data and "." not in data["schema"]:
+            data["schema"] = DEFAULT_CATALOG + "." + data["schema"]
         return data
 
     def __post_init__(self):
 
         if self.method == SparkConnectionMethod.ODBC:
             try:
                 import pyodbc  # noqa: F401
```

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.2.512/dbt/adapters/spark/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from concurrent.futures import Future
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union, Set
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union, Callable
 from typing_extensions import TypeAlias
 from dbt.contracts.graph.manifest import Manifest
 
 import agate
 from agate import Table
 
 from dbt.contracts.relation import RelationType
@@ -19,21 +19,23 @@
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.spark import SparkConnectionManager
 from dbt.adapters.spark import SparkRelation
 from dbt.adapters.spark import SparkColumn
 from dbt.adapters.base import BaseRelation
 from dbt.clients.agate_helper import DEFAULT_TYPE_TESTER
 from dbt.events import AdapterLogger
-from dbt.utils import executor
+from dbt.utils import executor, AttrDict
 
 logger = AdapterLogger("Spark")
 
 GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME = "get_columns_in_relation_raw"
 LIST_SCHEMAS_MACRO_NAME = "list_schemas"
 LIST_RELATIONS_MACRO_NAME = "list_relations_without_caching"
+LIST_RELATIONS_SHOW_TABLES_MACRO_NAME = "list_relations_show_tables_without_caching"
+DESCRIBE_TABLE_EXTENDED_MACRO_NAME = "describe_table_extended_without_caching"
 DROP_RELATION_MACRO_NAME = "drop_relation"
 FETCH_TBL_PROPERTIES_MACRO_NAME = "fetch_tbl_properties"
 
 CURRENT_CATALOG_MACRO_NAME = "current_catalog"
 USE_CATALOG_MACRO_NAME = "use_catalog"
 
 KEY_TABLE_OWNER = "Owner"
@@ -90,14 +92,15 @@
         "_hoodie_commit_seqno",
         "_hoodie_record_key",
         "_hoodie_partition_path",
         "_hoodie_file_name",
     ]
 
     Relation: TypeAlias = SparkRelation
+    RelationInfo = Tuple[str, str, str, str]
     Column: TypeAlias = SparkColumn
     ConnectionManager: TypeAlias = SparkConnectionManager
     AdapterSpecificConfigs: TypeAlias = SparkConfig
 
     @classmethod
     def date_function(cls) -> str:
         return "current_timestamp()"
@@ -134,52 +137,162 @@
                 "Attempted to cache a null schema for {}".format(name)
             )
         if dbt.flags.USE_CACHE:
             self.cache.add_schema(None, schema)
         # so jinja doesn't render things
         return ""
 
-    def list_relations_without_caching(
-        self, schema_relation: SparkRelation
-    ) -> List[SparkRelation]:
+    def _get_relation_information(
+        self, schema_relation: BaseRelation, row: agate.Row
+    ) -> RelationInfo:
+        """relation info was fetched with SHOW TABLES EXTENDED"""
+        try:
+            _schema, name, _, information = row
+        except ValueError:
+            raise dbt.exceptions.RuntimeException(
+                f'Invalid value from "show tables extended ...", got {len(row)} values, expected 4'
+            )
+
+        return schema_relation.database, _schema, name, information
+
+    def _get_relation_information_using_describe(
+        self, schema_relation: BaseRelation, row: agate.Row
+    ) -> RelationInfo:
+        """Relation info fetched using SHOW TABLES and an auxiliary DESCRIBE statement"""
+        try:
+            _schema, name = row
+        except ValueError:
+            raise dbt.exceptions.RuntimeException(
+                f'Invalid value from "show tables ...", got {len(row)} values, expected 2'
+            )
+
+        is_openhouse = schema_relation.database == "openhouse" or "." in schema_relation.schema
+
+        # database is needed where relations can exist in different catalogs
+        table_name = f"{_schema}.{name}"
+        if is_openhouse:
+            if not table_name.startswith("openhouse."):
+                table_name = "openhouse." + table_name
+            _schema = "openhouse." + _schema
+
+        try:
+            table_results = self.execute_macro(
+                DESCRIBE_TABLE_EXTENDED_MACRO_NAME, kwargs={"table_name": table_name}
+            )
+        except dbt.exceptions.RuntimeException as e:
+            logger.debug(f"Error while retrieving information about {table_name}: {e.msg}")
+            table_results = AttrDict()
+
+        information = ""
+        for info_row in table_results:
+            info_type, info_value, _ = info_row
+            if not info_type.startswith("#"):
+                information += f"{info_type}: {info_value}\n"
+
+        return schema_relation.database, _schema, name, information
+
+    def _build_spark_relation_list(
+        self,
+        schema_relation: BaseRelation,
+        row_list: agate.Table,
+        relation_info_func: Callable[[BaseRelation, agate.Row], RelationInfo],
+    ) -> List[BaseRelation]:
+        """Aggregate relations with format metadata included."""
+        relations = []
+        for row in row_list:
+            database, _schema, name, information = relation_info_func(schema_relation, row)
+
+            rel_type: RelationType = (
+                RelationType.View if "Type: VIEW" in information else RelationType.Table
+            )
+            is_delta: bool = "Provider: delta" in information
+            is_hudi: bool = "Provider: hudi" in information
+            is_iceberg: bool = "Provider: iceberg" in information
+            is_openhouse: bool = "Provider: openhouse" in information
+
+            relation: BaseRelation = self.Relation.create(  # type: ignore
+                database=database if database else None,
+                schema=_schema,
+                identifier=name,
+                type=rel_type,
+                information=information,
+                is_delta=is_delta,
+                is_iceberg=is_iceberg,
+                is_hudi=is_hudi,
+                is_openhouse=is_openhouse,
+            )
+            relations.append(relation)
+
+        return relations
+
+    def list_relations_without_caching(self, schema_relation: BaseRelation) -> List[BaseRelation]:
+        """Distinct Spark compute engines may not support the same SQL featureset. Thus, we must
+        try different methods to fetch relation information."""
+
+        kwargs = {"schema_relation": schema_relation}
+
         is_openhouse = schema_relation.database == "openhouse" or "." in schema_relation.schema
 
         try:
-            results = None
-            # if this is an OpenHouse/Iceberg relation, use `DESCRIBE EXTENDED` to grab metadata
-            # because `show table extended` does not work for DataSourceV2 tables (SPARK-33393)
             if is_openhouse:
-                results = self.execute_macro(
-                    GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME, kwargs={"relation": schema_relation}
+                # Iceberg behavior: 3-row result of relations obtained
+                show_table_rows = self.execute_macro(
+                    LIST_RELATIONS_SHOW_TABLES_MACRO_NAME, kwargs=kwargs
+                )
+                return self._build_spark_relation_list(
+                    schema_relation=schema_relation,
+                    row_list=show_table_rows,
+                    relation_info_func=self._get_relation_information_using_describe,
                 )
             else:
                 with self._catalog(schema_relation.database):
-                    results = self.execute_macro(
-                        LIST_RELATIONS_MACRO_NAME, kwargs={"schema_relation": schema_relation}
+                    show_table_extended_rows = self.execute_macro(
+                        LIST_RELATIONS_MACRO_NAME, kwargs=kwargs
+                    )
+                    return self._build_spark_relation_list(
+                        schema_relation=schema_relation,
+                        row_list=show_table_extended_rows,
+                        relation_info_func=self._get_relation_information,
                     )
         except dbt.exceptions.RuntimeException as e:
             errmsg = getattr(e, "msg", "")
+            print(errmsg)
             if f"Database '{schema_relation}' not found" in errmsg:
                 return []
+            # Iceberg compute engine behavior: show table
+            elif "SHOW TABLE EXTENDED is not supported for v2 tables" in errmsg:
+                # this happens with spark-iceberg with v2 iceberg tables
+                # https://issues.apache.org/jira/browse/SPARK-33393
+                try:
+                    # Iceberg behavior: 3-row result of relations obtained
+                    show_table_rows = self.execute_macro(
+                        LIST_RELATIONS_SHOW_TABLES_MACRO_NAME, kwargs=kwargs
+                    )
+                    return self._build_spark_relation_list(
+                        schema_relation=schema_relation,
+                        row_list=show_table_rows,
+                        relation_info_func=self._get_relation_information_using_describe,
+                    )
+                except dbt.exceptions.RuntimeException as e:
+                    description = "Error while retrieving information about"
+                    logger.debug(f"{description} {schema_relation}: {e.msg}")
+                    return []
             else:
-                description = "Error while retrieving information about"
-                logger.debug(f"{description} {schema_relation}: {e.msg}")
+                logger.debug(
+                    f"Error while retrieving information about {schema_relation}: {errmsg}"
+                )
                 return []
 
-        return (
-            [self.parse_describe_extended_for_relation(schema_relation, results)]
-            if is_openhouse
-            else self.parse_show_table_extended_for_relation(schema_relation, results)
-        )
-
     def get_relation(
         self, database: Optional[str], schema: str, identifier: str
     ) -> Optional[BaseRelation]:
         if not self.Relation.include_policy.database:
             database = None
+        else:
+            database = database if database else None
 
         return super().get_relation(database, schema, identifier)
 
     def parse_describe_extended(
         self, relation: Relation, raw_rows: List[agate.Row]
     ) -> List[SparkColumn]:
         # Convert the Row to a dict
@@ -206,73 +319,14 @@
                 column=column["col_name"],
                 column_index=idx,
                 dtype=column["data_type"],
             )
             for idx, column in enumerate(rows)
         ]
 
-    def parse_describe_extended_for_relation(
-        self, relation: Relation, raw_rows: List[agate.Row]
-    ) -> SparkRelation:
-        # Convert the Row to a dict
-        dict_rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
-        # Find the separator between the rows and the metadata provided
-        # by the DESCRIBE TABLE EXTENDED statement
-        pos = self.find_table_information_separator(dict_rows)
-
-        # Get metadata columns, removing rows that are comments
-        metadata = {
-            col["col_name"]: col["data_type"]
-            for col in raw_rows[pos + 1 :]
-            if not col["col_name"].startswith("#")
-        }
-
-        rel_type = metadata.get(KEY_TABLE_TYPE, "")
-        provider = metadata.get(KEY_TABLE_PROVIDER, "")
-        return self.Relation.create(
-            database=relation.database,
-            schema=relation.schema,
-            identifier=relation.identifier,
-            type=(RelationType.View if rel_type == "VIEW" else RelationType.Table),
-            # information is the returned metadata rows flattened as a newline separated string
-            information="\n".join([f"{key}: {value}" for key, value in metadata.items()]),
-            is_delta=(provider == "delta"),
-            is_hudi=(provider == "hudi"),
-            is_openhouse=(provider == "openhouse"),
-        )
-
-    def parse_show_table_extended_for_relation(
-        self, relation: Relation, raw_rows: List[agate.Row]
-    ) -> List[SparkRelation]:
-
-        relations = []
-        for row in raw_rows:
-            if len(row) != 4:
-                raise dbt.exceptions.RuntimeException(
-                    f'Invalid value from "show table extended ...", '
-                    f"got {len(row)} values, expected 4"
-                )
-            _schema, name, _, information = row
-            rel_type = RelationType.View if "Type: VIEW" in information else RelationType.Table
-            is_delta = "Provider: delta" in information
-            is_hudi = "Provider: hudi" in information
-            is_openhouse = "Provider: openhouse" in information
-            relation = self.Relation.create(
-                database=relation.database,
-                schema=_schema,
-                identifier=name,
-                type=rel_type,
-                information=information,
-                is_delta=is_delta,
-                is_hudi=is_hudi,
-                is_openhouse=is_openhouse,
-            )
-            relations.append(relation)
-        return relations
-
     @staticmethod
     def find_table_information_separator(rows: List[dict]) -> int:
         pos = 0
         for row in rows:
             if not row["col_name"] or row["col_name"].startswith("#"):
                 break
             pos += 1
@@ -387,52 +441,43 @@
 
         columns: List[Dict[str, Any]] = []
         for relation in self.list_relations(database, schema):
             logger.debug("Getting table schema for relation {}", relation)
             columns.extend(self._get_columns_for_catalog(relation))
         return agate.Table.from_object(columns, column_types=DEFAULT_TYPE_TESTER)
 
-    # overriding this method to optimize the performance of list_relations_without_caching
-    def _get_cache_schemas(self, manifest: Manifest) -> Set[BaseRelation]:
-        """Get the set of schema relations that the cache logic needs to
-        populate. This means only executable nodes are included.
-        """
-        relations = [
-            self.Relation.create_from(self.config, node)  # keep the identifier
-            for node in manifest.nodes.values()
-            if (node.is_relational and not node.is_ephemeral_model)
-        ]
-        sources = [
-            self.Relation.create_from(self.config, node)  # keep the identifier
-            for node in manifest.sources.values()
-        ]
-
-        return set(relations + sources)
-
     def list_schemas(self, database: str) -> List[str]:
         connection = self.connections.get_if_exists()
         if connection is not None:
             database = connection.credentials.database
             schema = connection.credentials.schema
 
         # in case the user is using "openhouse" as a catalog, the format of schema will be 'openhouse.db'.
-        # so derive the catalog/database vakye from schema until we support `openhouse` catalog natively.
+        # so derive the catalog/database value from schema until we support `openhouse` catalog natively.
         if schema is not None and "." in schema:
             tokens = schema.split(".")
             database = tokens[0]
             schema = tokens[1]
 
         # The catalog for `show table extended` needs to match the current catalog.
         with self._catalog(database):
             results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": schema})
         schema_list = [row[0] for row in results]
         return schema_list
 
     def check_schema_exists(self, database, schema):
-        results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
+        # in case the user is using "openhouse" as a catalog, the format of schema will be 'openhouse.db'.
+        # so derive the catalog/database value from schema until we support `openhouse` catalog natively.
+        if schema is not None and "." in schema:
+            tokens = schema.split(".")
+            database = tokens[0]
+            schema = tokens[1]
+        # The catalog for `show table extended` needs to match the current catalog.
+        with self._catalog(database):
+            results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": schema})
         exists = True if schema in [row[0] for row in results] else False
         return exists
 
     def get_rows_different_sql(
         self,
         relation_a: BaseRelation,
         relation_b: BaseRelation,
```

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.2.512/dbt/adapters/spark/relation.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 @dataclass(frozen=True, eq=False, repr=False)
 class SparkRelation(BaseRelation):
     quote_policy: SparkQuotePolicy = SparkQuotePolicy()
     include_policy: SparkIncludePolicy = SparkIncludePolicy()
     quote_character: str = "`"
     is_delta: Optional[bool] = None
     is_hudi: Optional[bool] = None
+    is_iceberg: Optional[bool] = None
+    # TODO: make this a dict everywhere
     is_openhouse: Optional[bool] = None
     information: Optional[str] = None
 
     @classmethod
     def __pre_deserialize__(cls, data: Dict[Any, Any]) -> Dict[Any, Any]:
         data = super().__pre_deserialize__(data)
         if "database" not in data["path"]:
```

### Comparing `in-dbt-spark-1.2.511/dbt/adapters/spark/session.py` & `in-dbt-spark-1.2.512/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/adapters.sql`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+{% macro dbt_spark_tblproperties_clause() -%}
+  {%- set tblproperties = config.get('tblproperties') -%}
+  {%- if tblproperties is not none %}
+    tblproperties (
+      {%- for prop in tblproperties -%}
+      '{{ prop }}' = '{{ tblproperties[prop] }}' {% if not loop.last %}, {% endif %}
+      {%- endfor %}
+    )
+  {%- endif %}
+{%- endmacro -%}
+
 {% macro file_format_clause() %}
   {{ return(adapter.dispatch('file_format_clause', 'dbt')()) }}
 {%- endmacro -%}
 
 {% macro spark__file_format_clause() %}
   {%- set file_format = config.get('file_format', validator=validation.any[basestring]) -%}
   {%- if file_format is not none %}
@@ -137,15 +148,15 @@
 {% endmacro %}
 
 
 {% macro spark__create_table_as(temporary, relation, sql) -%}
   {% if temporary -%}
     {{ create_temporary_view(relation, sql) }}
   {%- else -%}
-    {% if config.get('file_format', validator=validation.any[basestring]) == 'delta' %}
+    {% if config.get('file_format', validator=validation.any[basestring]) in ['delta', 'iceberg'] %}
       create or replace table {{ relation }}
     {% else %}
       create table {{ relation }}
     {% endif %}
     {% if config.get('file_format', validator=validation.any[basestring]) != 'openhouse' %}
       {{ file_format_clause() }}
     {% endif %}
@@ -197,25 +208,49 @@
   {% call statement('get_columns_in_relation_raw', fetch_result=True) %}
       describe extended {{ relation.include(schema=(schema is not none)) }}
   {% endcall %}
   {% do return(load_result('get_columns_in_relation_raw').table) %}
 {% endmacro %}
 
 {% macro spark__get_columns_in_relation(relation) -%}
-  {{ return(adapter.get_columns_in_relation(relation)) }}
+  {% call statement('get_columns_in_relation', fetch_result=True) %}
+      describe extended {{ relation.include(schema=(schema is not none)) }}
+  {% endcall %}
+  {% do return(load_result('get_columns_in_relation').table) %}
 {% endmacro %}
 
 -- override macro to list only relations related to current dbt project
 {% macro spark__list_relations_without_caching(relation) %}
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
     show table extended in {{ relation.schema }} like '{{ relation.identifier or "*" }}'
   {% endcall %}
   {% do return(load_result('list_relations_without_caching').table) %}
 {% endmacro %}
 
+{% macro list_relations_show_tables_without_caching(schema_relation) %}
+  {#-- Spark with iceberg tables don't work with show table extended for #}
+  {#-- V2 iceberg tables #}
+  {#-- https://issues.apache.org/jira/browse/SPARK-33393 #}
+  {% call statement('list_relations_without_caching_show_tables', fetch_result=True) -%}
+    show tables in {{ schema_relation }} like '*'
+  {% endcall %}
+
+  {% do return(load_result('list_relations_without_caching_show_tables').table) %}
+{% endmacro %}
+
+{% macro describe_table_extended_without_caching(table_name) %}
+  {#-- Spark with iceberg tables don't work with show table extended for #}
+  {#-- V2 iceberg tables #}
+  {#-- https://issues.apache.org/jira/browse/SPARK-33393 #}
+  {% call statement('describe_table_extended_without_caching', fetch_result=True) -%}
+    describe extended {{ table_name }}
+  {% endcall %}
+  {% do return(load_result('describe_table_extended_without_caching').table) %}
+{% endmacro %}
+
 -- override macro to list only schemas related to current dbt project
 {% macro spark__list_schemas(database) -%}
   {% call statement('list_schemas', fetch_result=True, auto_begin=False) %}
     show databases like '{{ database or "*" }}'
   {% endcall %}
   {{ return(load_result('list_schemas').table) }}
 {% endmacro %}
@@ -264,27 +299,27 @@
   {%- elif raw_persist_docs -%}
         {{ exceptions.raise_compiler_error("Invalid value provided for 'persist_docs'. Expected dict but got value: " ~ raw_persist_docs) }}
   {% endif %}
 {% endmacro %}
 
 {% macro spark__alter_column_comment(relation, column_dict) %}
   {%- set file_format = config.get('file_format', default='openhouse') -%}
-  {% if file_format in ['delta', 'hudi', 'openhouse'] %}
+  {% if file_format in ['delta', 'hudi', 'iceberg', 'openhouse'] %}
     {% for column_name in column_dict %}
       {% set comment = column_dict[column_name]['description'] %}
       {% set escaped_comment = comment | replace('\'', '\\\'') %}
       {% set comment_query %}
-        {% if file_format in ['delta', 'hudi'] %}
-          alter table {{ relation }} change column
-            {{ adapter.quote(column_name) if column_dict[column_name]['quote'] else column_name }}
-            comment '{{ escaped_comment }}';
-        {% else %}
+        {% if relation.is_iceberg or relation.is_openhouse %}
           alter table {{ relation }} alter column
-             {{ adapter.quote(column_name) if column_dict[column_name]['quote'] else column_name }}
-             comment '{{ escaped_comment }}';
+              {{ adapter.quote(column_name) if column_dict[column_name]['quote'] else column_name }}
+              comment '{{ escaped_comment }}';
+        {% else %}
+          alter table {{ relation }} change column
+              {{ adapter.quote(column_name) if column_dict[column_name]['quote'] else column_name }}
+              comment '{{ escaped_comment }}';
         {% endif %}
       {% endset %}
       {% do run_query(comment_query) %}
     {% endfor %}
   {% endif %}
 {% endmacro %}
 
@@ -319,15 +354,23 @@
   {% endcall %}
 {% endmacro %}
 
 
 {% macro spark__alter_relation_add_remove_columns(relation, add_columns, remove_columns) %}
 
   {% if remove_columns %}
-    {% set platform_name = 'Delta Lake' if relation.is_delta else 'Apache Spark' %}
+    {% if relation.is_delta %}
+      {% set platform_name = 'Delta Lake' %}
+    {% elif relation.is_iceberg %}
+      {% set platform_name = 'Iceberg' %}
+    {% elif relation.is_openhouse %}
+      {% set platform_name = 'OpenHouse' %}
+    {% else %}
+      {% set platform_name = 'Apache Spark' %}
+    {% endif %}
     {{ exceptions.raise_compiler_error(platform_name + ' does not support dropping columns from tables') }}
   {% endif %}
 
   {% if add_columns is none %}
     {% set add_columns = [] %}
   {% endif %}
```

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/apply_retention.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/apply_retention.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     {% if not is_delta %} {#-- If Delta, we will `create or replace` below, so no need to drop --#}
       {% do adapter.drop_relation(existing_relation) %}
     {% endif %}
     {% set build_sql = create_table_as(False, target_relation, sql) %}
   {% else %}
     {% do run_query(create_table_as(True, tmp_relation, sql)) %}
     {% do process_schema_changes(on_schema_change, tmp_relation, existing_relation) %}
-    {% set build_sql = dbt_spark_get_incremental_sql(strategy, tmp_relation, target_relation, unique_key) %}
+    {% set build_sql = dbt_spark_get_incremental_sql(strategy, tmp_relation, target_relation, existing_relation, unique_key) %}
   {% endif %}
 
   {%- call statement('main') -%}
     {{ build_sql }}
   {%- endcall -%}
 
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode) %}
```

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-{% macro get_insert_overwrite_sql(source_relation, target_relation) %}
+{% macro get_insert_overwrite_sql(source_relation, target_relation, existing_relation) %}
 
     {%- set dest_columns = adapter.get_columns_in_relation(target_relation) -%}
     {%- set dest_cols_csv = dest_columns | map(attribute='quoted') | join(', ') -%}
-    insert overwrite table {{ target_relation }}
-    {% if config.get('file_format') != 'openhouse' %} {{ partition_cols(label="partition") }} {% endif %}
+    {% if existing_relation.is_iceberg or existing_relation.is_openhouse %}
+      {# removed table from statement for iceberg #}
+      insert overwrite {{ target_relation }}
+      {# removed partition_cols for iceberg as well #}
+    {% else %}
+      insert overwrite table {{ target_relation }}
+      {{ partition_cols(label="partition") }}
+    {% endif %}
     select {{dest_cols_csv}} from {{ source_relation.include(database=false, schema=false) }}
 
 {% endmacro %}
 
 
 {% macro get_insert_into_sql(source_relation, target_relation) %}
 
@@ -55,23 +61,23 @@
         {%- endfor %}
         {%- else %} * {% endif %}
 
       when not matched then insert *
 {% endmacro %}
 
 
-{% macro dbt_spark_get_incremental_sql(strategy, source, target, unique_key) %}
+{% macro dbt_spark_get_incremental_sql(strategy, source, target, existing, unique_key) %}
   {%- if strategy == 'append' -%}
     {#-- insert new records into existing table, without updating or overwriting #}
     {{ get_insert_into_sql(source, target) }}
   {%- elif strategy == 'insert_overwrite' -%}
     {#-- insert statements don't like CTEs, so support them via a temp view #}
-    {{ get_insert_overwrite_sql(source, target) }}
+    {{ get_insert_overwrite_sql(source, target, existing) }}
   {%- elif strategy == 'merge' -%}
-  {#-- merge all columns with databricks delta - schema changes are handled for us #}
+  {#-- merge all columns for datasources which implement MERGE INTO (e.g. databricks, iceberg, openhouse) - schema changes are handled for us #}
     {{ get_merge_sql(target, source, unique_key, dest_columns=none, predicates=none) }}
   {%- else -%}
     {% set no_sql_for_strategy_msg -%}
       No known SQL for the incremental strategy provided: {{ strategy }}
     {%- endset %}
     {%- do exceptions.raise_compiler_error(no_sql_for_strategy_msg) -%}
   {%- endif -%}
```

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/seed.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                                                   schema=target.schema,
                                                   database=none,
                                                   type='table') -%}
     {% set select = build_merge_sql_hive(target, source, insert_cols) %}
 
     {% call statement('build_snapshot_merge_relation') %}
         {{ log(" build_snapshot_merge_relation create_table_as description: ******* ") }}
+        {% do adapter.drop_relation(tmp_relation) %}
         {{ create_table_as(False, tmp_relation, select) }}
     {% endcall %}
 
     {% do return(tmp_relation) %}
 {% endmacro %}
 
 {% macro insert_overwrite(target, source) -%}
@@ -50,15 +51,20 @@
 {% endmacro %}
 
 
 
 {% macro spark__snapshot_merge_sql(target, source, insert_cols) -%}
 
     merge into {{ target }} as DBT_INTERNAL_DEST
-    using {{ source }} as DBT_INTERNAL_SOURCE
+    {% if target.is_iceberg %}
+      {# create view only supports a name (no catalog, or schema) #}
+      using {{ source.identifier }} as DBT_INTERNAL_SOURCE
+    {% else %}
+      using {{ source }} as DBT_INTERNAL_SOURCE
+    {% endif %}
     on DBT_INTERNAL_SOURCE.dbt_scd_id = DBT_INTERNAL_DEST.dbt_scd_id
     when matched
      and DBT_INTERNAL_DEST.dbt_valid_to is null
      and DBT_INTERNAL_SOURCE.dbt_change_type in ('update', 'delete')
         then update
         set dbt_valid_to = DBT_INTERNAL_SOURCE.dbt_valid_to
 
@@ -67,24 +73,44 @@
         then insert *
     ;
 {% endmacro %}
 
 
 {% macro spark_build_snapshot_staging_table(strategy, sql, target_relation, file_format) %}
     {% set tmp_identifier = target_relation.identifier ~ '__dbt_tmp' %}
-    {%- set tmp_relation = api.Relation.create(identifier=tmp_identifier,
-                                                  schema=target_relation.schema,
-                                                  database=none,
-                                                  type='view') -%}
+
+    {% if target_relation.is_iceberg %}
+      {# iceberg catalog does not support create view, but regular spark does. We removed the catalog and schema #}
+      {%- set tmp_relation = api.Relation.create(identifier=tmp_identifier,
+                                                    schema=none,
+                                                    database=none,
+                                                    type='view') -%}
+    {% elif target_relation.is_openhouse %}
+      {# Views spanning multiple catalogs have undefined behavior currently #}
+      {%- set tmp_relation = api.Relation.create(identifier=tmp_identifier,
+                                                    schema=target_relation.schema,
+                                                    database=target_relation.database,
+                                                    type='table') -%}
+    {% else %}
+      {%- set tmp_relation = api.Relation.create(identifier=tmp_identifier,
+                                                    schema=target_relation.schema,
+                                                    database=none,
+                                                    type='view') -%}
+    {% endif %}
 
     {% set select = snapshot_staging_table(strategy, sql, target_relation) %}
 
     {# needs to be a non-temp view so that its columns can be ascertained via `describe` #}
     {% call statement('build_snapshot_staging_relation') %}
-        {{ create_view_as(tmp_relation, select) }}
+        {% if target_relation.is_openhouse %}
+          {% do adapter.drop_relation(tmp_relation) %}
+          {{ create_table_as(False, tmp_relation, select) }}
+        {% else %}
+          {{ create_view_as(tmp_relation, select) }}
+        {% endif %}
     {% endcall %}
 
     {% do return(tmp_relation) %}
 {% endmacro %}
 
 
 {% macro spark__post_snapshot(staging_relation) %}
@@ -108,24 +134,24 @@
 {% materialization snapshot, adapter='spark' %}
   {%- set config = model['config'] -%}
 
   {%- set target_table = model.get('alias', model.get('name')) -%}
 
   {%- set strategy_name = config.get('strategy') -%}
   {%- set unique_key = config.get('unique_key') %}
-  {%- set file_format = config.get('file_format', 'parquet') -%}
+  {%- set file_format = config.get('file_format', 'openhouse') -%}
 
   {% set target_relation_exists, target_relation = get_or_create_relation(
           database=none,
           schema=model.schema,
           identifier=target_table,
           type='table') -%}
 
   {% if not adapter.check_schema_exists(model.database, model.schema) %}
-    {% do create_schema(model.database, model.schema) %}
+    {% do exceptions.raise_compiler_error("Self-serve schema creation is not currently supported in OpenHouse. Please reach out in #ask_openhouse to manually provision your database.") %}
   {% endif %}
 
   {%- if not target_relation.is_table -%}
     {% do exceptions.relation_wrong_type(target_relation, 'table') %}
   {%- endif -%}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
@@ -155,22 +181,25 @@
                                    | rejectattr('name', 'equalto', 'dbt_change_type')
                                    | rejectattr('name', 'equalto', 'DBT_CHANGE_TYPE')
                                    | rejectattr('name', 'equalto', 'dbt_unique_key')
                                    | rejectattr('name', 'equalto', 'DBT_UNIQUE_KEY')
                                    | list %}
 
       {% do create_columns(target_relation, missing_columns) %}
+
       {% set staging_columns = adapter.get_columns_in_relation(staging_table)
                                    | rejectattr('name', 'equalto', 'dbt_change_type')
                                    | rejectattr('name', 'equalto', 'DBT_CHANGE_TYPE')
                                    | rejectattr('name', 'equalto', 'dbt_unique_key')
                                    | rejectattr('name', 'equalto', 'DBT_UNIQUE_KEY')
                                    | list %}
-      -- only delta and hudi file_format supports merge_into, others use full outer join to merge snapshot and source table
-      {% if file_format in ['delta', 'hudi'] %}
+
+      -- only some file_formats support merge_into, others use full outer join to merge snapshot and source table
+      -- TODO DATAFND-1019: use MERGE INTO for OpenHouse when `merge into` starts using column id ordering rather than ordinal
+      {% if file_format in ['delta', 'iceberg', 'hudi'] %}
           {% set quoted_source_columns = [] %}
           {% for column in staging_columns %}
             {% do quoted_source_columns.append(adapter.quote(column.name)) %}
           {% endfor %}
 
           {% set final_sql = snapshot_merge_sql(
               target = target_relation,
@@ -199,14 +228,17 @@
       {% endif %}
   {% endif %}
 
   {% call statement('main') %}
       {{ final_sql }}
   {% endcall %}
 
+  {% set should_revoke = should_revoke(target_relation_exists, full_refresh_mode) %}
+  {% do apply_grants(target_relation, grant_config, should_revoke) %}
+
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
   {{ adapter.commit() }}
 
   {% if staging_table is defined %}
```

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/table.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/table.sql`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,18 @@
   -- setup: if the target relation already exists, drop it
   -- in case if the existing and future table is delta, we want to do a
   -- create or replace table instead of dropping, so we don't have the table unavailable
   {% if old_relation and not (old_relation.is_delta and file_format == 'delta') -%}
     {{ adapter.drop_relation(old_relation) }}
   {%- endif %}
 
+  {% if old_relation and not (old_relation.is_iceberg and file_format == 'iceberg') -%}
+    {{ adapter.drop_relation(old_relation) }}
+  {%- endif %}
+
   -- build model
   {% call statement('main') -%}
     {{ create_table_as(False, target_relation, sql) }}
   {%- endcall %}
 
   {% set should_revoke = should_revoke(old_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
```

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/materializations/validate.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/validate.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% macro dbt_spark_validate_get_file_format(raw_file_format) %}
   {#-- Validate the file format #}
 
-  {% set accepted_formats = ['text', 'csv', 'json', 'jdbc', 'parquet', 'orc', 'hive', 'delta', 'libsvm', 'hudi', 'openhouse'] %}
+  {% set accepted_formats = ['text', 'csv', 'json', 'jdbc', 'parquet', 'orc', 'hive', 'delta', 'libsvm', 'hudi', 'iceberg', 'openhouse'] %}
 
   {% set invalid_file_format_msg -%}
     Invalid file format provided: {{ raw_file_format }}
     Expected one of: {{ accepted_formats | join(', ') }}
   {%- endset %}
 
   {% if raw_file_format not in accepted_formats %}
@@ -22,33 +22,33 @@
   {% set invalid_strategy_msg -%}
     Invalid incremental strategy provided: {{ raw_strategy }}
     Expected one of: 'append', 'merge', 'insert_overwrite'
   {%- endset %}
 
   {% set invalid_merge_msg -%}
     Invalid incremental strategy provided: {{ raw_strategy }}
-    You can only choose this strategy when file_format is set to 'delta' or 'hudi'
+    You can only choose this strategy when file_format is set to 'delta' or 'iceberg' or 'hudi' or 'openhouse'
   {%- endset %}
 
   {% set invalid_insert_overwrite_delta_msg -%}
     Invalid incremental strategy provided: {{ raw_strategy }}
-    You cannot use this strategy when file_format is set to 'delta'
+    You cannot use this strategy when file_format is set to 'delta' or 'iceberg' or 'openhouse'
     Use the 'append' or 'merge' strategy instead
   {%- endset %}
 
   {% set invalid_insert_overwrite_endpoint_msg -%}
     Invalid incremental strategy provided: {{ raw_strategy }}
     You cannot use this strategy when connecting via endpoint
     Use the 'append' or 'merge' strategy instead
   {%- endset %}
 
   {% if raw_strategy not in ['append', 'merge', 'insert_overwrite'] %}
     {% do exceptions.raise_compiler_error(invalid_strategy_msg) %}
   {%-else %}
-    {% if raw_strategy == 'merge' and file_format not in ['delta', 'hudi'] %}
+    {% if raw_strategy == 'merge' and file_format not in ['delta', 'iceberg', 'hudi', 'openhouse'] %}
       {% do exceptions.raise_compiler_error(invalid_merge_msg) %}
     {% endif %}
     {% if raw_strategy == 'insert_overwrite' and file_format == 'delta' %}
       {% do exceptions.raise_compiler_error(invalid_insert_overwrite_delta_msg) %}
     {% endif %}
     {% if raw_strategy == 'insert_overwrite' and target.endpoint %}
       {% do exceptions.raise_compiler_error(invalid_insert_overwrite_endpoint_msg) %}
```

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.2.512/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.2.512/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.511
+Version: 1.2.512
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.511 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.512 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.511/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.2.512/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.511/setup.py` & `in-dbt-spark-1.2.512/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.2.511"
+package_version = "1.2.512"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.16.0",
```

